# Comparing `tmp/chess2vec-0.1.3b3.tar.gz` & `tmp/chess2vec-0.1.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.3b3.tar", max compression
+gzip compressed data, was "chess2vec-0.1.4b1.tar", max compression
```

## Comparing `chess2vec-0.1.3b3.tar` & `chess2vec-0.1.4b1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.3b3/README.md
--rw-r--r--   0        0        0     5582 2024-04-17 21:16:47.895949 chess2vec-0.1.3b3/chess2vec/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.3b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.3b3/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.3b3/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-17 21:16:58.389446 chess2vec-0.1.3b3/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.3b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.4b1/README.md
+-rw-r--r--   0        0        0     4301 2024-04-17 23:02:52.220580 chess2vec-0.1.4b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.4b1/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.4b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1682 2024-04-17 22:29:19.024554 chess2vec-0.1.4b1/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.4b1/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.4b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-17 23:03:30.090569 chess2vec-0.1.4b1/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.4b1/PKG-INFO
```

### Comparing `chess2vec-0.1.3b3/chess2vec/__init__.py` & `chess2vec-0.1.4b1/chess2vec/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,163 @@
 from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
 import numpy as np
-import scipy.sparse
 from tqdm import tqdm
 
-import chess2vec._utils.sparse as spu
+import chess2vec._utils as _u
+import chess2vec._utils.sparse as _spu
 
 VEC_BLOCK = 64 * 64
 VEC_SIZE = 5 * VEC_BLOCK
 
 
-class csr_matrix_builder:
-    def __init__(self):
-        self.data = []
-        self.rows = []
-        self.columns = []
-
-    def add_entry(self, rows, columns, data=None):
-        self.columns += columns
-
-        if isinstance(rows, int):
-            rows = [rows for _ in range(len(columns))]
-
-        self.rows += rows
-
-        if data is None:
-            data = [1 for _ in range(len(rows))]
-
-        self.data += data
-
-    def build(self, shape, dtype=np.float32):
-        return scipy.sparse.csr_matrix(
-            (self.data, (self.rows, self.columns)), shape=shape, dtype=dtype
-        )
-
-
-def _actions(board: chess.Board):
-    for move in board.legal_moves:
-        pt = board.piece_type_at(move.from_square)
-
-        if not board.turn:
-            move.from_square ^= 0x38
-            move.to_square ^= 0x38
-
-        idx = 64 * move.from_square + move.to_square
-
-        match pt:
-            case chess.QUEEN:
-                yield from (VEC_BLOCK * 2 + idx, VEC_BLOCK * 3 + idx)
-            case chess.KING:
-                yield VEC_BLOCK * 4 + idx
-            case _:
-                yield VEC_BLOCK * (pt - 1) + idx
+class PositionEncoder:
+    def __init__(self, with_fen: bool = True) -> None:
+        self.actions = _spu.csr_matrix((0, VEC_SIZE), dtype=np.uint8)
 
+        self.with_fen = with_fen
 
-class PositionEncoder:
-    def __init__(self) -> None:
-        self.positions = []
-        self._actions_matrix = scipy.sparse.csr_matrix((0, VEC_SIZE), dtype=np.uint8)
-
-    def _load_indices(self, rows, columns):
-        mat = scipy.sparse.csr_matrix(
-            (
-                np.ones_like(columns, dtype=np.uint8),
-                (rows, columns),
-            ),
-            shape=(int(np.max(rows)) + 1, VEC_SIZE),
-        )
+        if self.with_fen:
+            self.labels = []
 
-        self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
+    def _update_labels(self, labels: Iterable[str]):
+        if self.with_fen:
+            self.labels += labels
 
     def load_fen(self, x: Iterable[str]):
-        rows, columns = [], []
-        row_idx = 0
+        builder = _spu.csr_matrix_builder()
+        idx = 0
 
         for fen in x:
             board = chess.Board(fen)
 
-            actions = list(_actions(board))
-            columns += actions
-            rows += [row_idx for _ in range(len(actions))]
+            builder.add_entry(idx, list(_u.actions(board)))
 
-            row_idx += 1
+            idx += 1
 
-        self._load_indices(rows, columns)
-        self.positions += list(x)
+        self._update_labels(list(x))
+        self.actions = _spu.vstack(
+            [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
+        )
 
-    def load_pgn(self, x: TextIO, max_games: int = None, status: bool=False):
+    def load_pgn(self, x: TextIO, max_games: int = None, status: bool = False):
         if max_games <= 0:
             return
 
         if max_games is None:
             max_games = float("inf")
 
-        builder = csr_matrix_builder()
-        positions = []
+        builder = _spu.csr_matrix_builder()
         idx = num_game = 0
-        
+
         if status:
             bar = tqdm(total=max_games)
 
         game = chess.pgn.read_game(x)
 
         while game and num_game < max_games:
             board = game.board()
 
-            builder.add_entry(idx, list(_actions(board)))
-            positions.append(board.fen())
+            builder.add_entry(idx, list(_u.actions(board)))
+            self._update_labels([board.fen()])
 
             idx += 1
 
             for move in game.mainline_moves():
                 board.push(move)
 
-                builder.add_entry(idx, list(_actions(board)))
-                positions.append(board.fen())
+                builder.add_entry(idx, list(_u.actions(board)))
+                self._update_labels([board.fen()])
 
                 idx += 1
 
             if status:
                 bar.update(1)
 
             game = chess.pgn.read_game(x)
             num_game += 1
 
-        self._actions_matrix = scipy.sparse.vstack(
-            [self._actions_matrix, builder.build((idx, VEC_SIZE), np.uint8)]
+        self.actions = _spu.vstack(
+            [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
         )
-        self.positions += positions
-        
+
         if status:
             bar.close()
 
     def load_npz(self, x: Iterable[str]):
+        """loads data from .npz file"""
         for file in x:
             with np.load(file) as loaded:
                 indices = loaded["mat_indices"]
-                mat = scipy.sparse.csr_matrix(
+
+                mat = _spu.csr_matrix(
                     (
                         np.ones_like(indices, dtype=np.uint8),
                         indices,
                         loaded["mat_indptr"],
                     ),
                     shape=(loaded["size"], VEC_SIZE),
                 )
 
-                positions = list(loaded["positions"])
+                self.actions = _spu.vstack([self.actions, mat])
+                self._update_labels(list(loaded["labels"]))
 
-            self._actions_matrix = scipy.sparse.vstack([self._actions_matrix, mat])
-            self.positions += positions
+    def save(self, file: str) -> None:
+        """saves the already loaded data to a compressed .npz file."""
 
-    def save(self, file) -> None:
-        np.savez_compressed(
-            file,
-            mat_indices=self._actions_matrix.indices,
-            mat_indptr=self._actions_matrix.indptr,
+        _save_dict = {}
+        _save_dict.update(
+            mat_indices=self.actions.indices,
+            mat_indptr=self.actions.indptr,
             size=self.size,
-            positions=self.positions,
         )
 
+        if self.with_fen:
+            _save_dict.update(labels=self.labels)
+
+        np.savez_compressed(file, **_save_dict)
+
     @property
     def size(self) -> int:
-        return self._actions_matrix.shape[0]
-
-    def batched(self, batch_size: int = None):
-        if batch_size is None:
-            batch_size = self.size
+        return self.actions.shape[0]
 
+    def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
             child = self.__new__(type(self))
-            child._actions_matrix = self._actions_matrix[idx : idx + batch_size]
-            child.positions = self.positions[idx : idx + batch_size]
+            child.__init__(self.with_fen)
+
+            child.actions = self.actions[idx : idx + batch_size]
+            child._update_labels(self.labels[idx : idx + batch_size])
 
             yield child
 
     def shuffle(self, *, seed: int = 42):
         rng = np.random.default_rng(seed)
-        idx = rng.permutation(len(self._actions_matrix))
+        idx = rng.permutation(len(self.actions))
+
+        self.actions = self.actions[idx]
 
-        self._actions_matrix = self._actions_matrix[idx]
-        self.positions = list(np.array(self.positions)[idx])
+        if self.with_fen:
+            self.labels = list(np.array(self.labels)[idx])
 
     def cov(self) -> np.ndarray:
-        return spu.cov(self._actions_matrix.T).toarray()
+        return _spu.scov(self.actions.T).toarray()
 
     def encode(self) -> np.ndarray: ...
 
     def __add__(self, item):
         assert isinstance(item, type(self))
 
         new = self.__new__(type(self))
-        new._actions_matrix = scipy.sparse.vstack(
-            [self._actions_matrix, item._actions_matrix]
-        )
-        new.positions = self.positions + item.positions
+        new.__init__(self.with_fen)
+
+        new.actions = _spu.vstack([self.actions, item.actions])
+
+        if self.with_fen:
+            new.labels = self.labels + item.labels
 
         return new
 
     def __repr__(self):
         return "PositionEncoder(size={})".format(self.size)
```

### Comparing `chess2vec-0.1.3b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.4b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.3b3/chess2vec/_utils/vector.py` & `chess2vec-0.1.4b1/chess2vec/_utils/vector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 
 
 def norm_l2(a: np.ndarray) -> np.ndarray:
-    """compute the l2 norm of a batch of vectors."""
+    """computes the l2 (euclidean) norm of the batch `a` of vectors."""
     assert a.ndim == 2
     return np.sqrt(np.sum(a**2, axis=1))
 
 
 def distance_l2(a: np.ndarray, b: np.ndarray) -> np.ndarray:
-    """compute the l2 (euclidean distance) between two batches of vectors."""
+    """computes the l2 (euclidean) distance between batch `a` and batch `b` of vectors."""
     return norm_l2(a - b)
 
 
 def cosine(a: np.ndarray, b: np.ndarray) -> np.ndarray:
-    """compute the cosine similarity between two batches of vectors."""
+    """computes the cosine similarity between batch `a` and batch `b` of vectors."""
     return np.sum(a * b, axis=1) / (norm_l2(a) * norm_l2(b))
```

### Comparing `chess2vec-0.1.3b3/PKG-INFO` & `chess2vec-0.1.4b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.3b3
+Version: 0.1.4b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

