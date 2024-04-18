# Comparing `tmp/chess2vec-0.1.5b9.tar.gz` & `tmp/chess2vec-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.5b9.tar", max compression
+gzip compressed data, was "chess2vec-0.2.0b1.tar", max compression
```

## Comparing `chess2vec-0.1.5b9.tar` & `chess2vec-0.2.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b9/README.md
--rw-r--r--   0        0        0     4339 2024-04-18 00:12:40.421495 chess2vec-0.1.5b9/chess2vec/__init__.py
--rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b9/chess2vec/_utils/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b9/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0     1726 2024-04-18 00:12:43.831445 chess2vec-0.1.5b9/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b9/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b9/chess2vec/pgn.py
--rw-r--r--   0        0        0      358 2024-04-18 00:13:09.414415 chess2vec-0.1.5b9/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b9/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.0b1/README.md
+-rw-r--r--   0        0        0     4218 2024-04-18 13:42:48.596980 chess2vec-0.2.0b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-18 13:38:23.643154 chess2vec-0.2.0b1/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.2.0b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1726 2024-04-18 00:12:43.831445 chess2vec-0.2.0b1/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.0b1/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.0b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-18 13:43:36.784349 chess2vec-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.0b1/PKG-INFO
```

### Comparing `chess2vec-0.1.5b9/chess2vec/__init__.py` & `chess2vec-0.2.0b1/chess2vec/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,35 @@
-from typing import Iterable, TextIO
+from typing import Iterable, Literal, TextIO
 
 import chess
 import chess.pgn
 import numpy as np
 from tqdm import tqdm
 
 import chess2vec._utils as _u
 import chess2vec._utils.sparse as _spu
 
-VEC_SIZE = 5 * 64 * 64
 
+class ActionLoader:
+    def __init__(self, *, with_fen=False, pool_size=1):
+        self.pool_size = pool_size
+        self.entry_size = 5 * (8 // self.pool_size) ** 4
 
-class PositionLoader:
-    def __init__(self, with_fen: bool = True) -> None:
-        self.actions = _spu.csr_matrix((0, VEC_SIZE), dtype=np.uint8)
-
+        self.entries = _spu.csr_matrix((0, self.entry_size), dtype=np.uint8)
         self.with_fen = with_fen
 
         if self.with_fen:
             self.labels = []
 
     def _update_labels(self, labels: Iterable[str]):
         if self.with_fen:
             self.labels += labels
 
-    def load_fen(self, x: Iterable[str]):
-        builder = _spu.csr_matrix_builder()
-        idx = 0
-
-        for fen in x:
-            board = chess.Board(fen)
-
-            builder.add_entry(idx, list(_u.actions(board)), 1, np.uint8)
-
-            idx += 1
-
-        self._update_labels(list(x))
-        self.actions = _spu.vstack(
-            [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
-        )
-
     def load_pgn(self, x: TextIO, max_games: int = None, status: bool = False):
-        if max_games <= 0:
-            return
+        assert max_games > 0
 
         if max_games is None:
             max_games = float("inf")
 
         builder = _spu.csr_matrix_builder()
         idx = num_game = 0
 
@@ -54,37 +37,37 @@
             bar = tqdm(total=max_games)
 
         game = chess.pgn.read_game(x)
 
         while game and num_game < max_games:
             board = game.board()
 
-            actions = list(_u.actions(board))
-            builder.add_entry(idx, actions, 1, np.uint8)
+            columns, data = _u.actions(board, self.pool_size)
+            builder.add_entry(idx, columns, data, np.uint8)
             self._update_labels([board.fen()])
 
             idx += 1
 
             for move in game.mainline_moves():
                 board.push(move)
 
-                actions = list(_u.actions(board))
-                builder.add_entry(idx, actions, 1, np.uint8)
+                columns, data = _u.actions(board, self.pool_size)
+                builder.add_entry(idx,columns, data, np.uint8)
                 self._update_labels([board.fen()])
 
                 idx += 1
 
             if status:
                 bar.update(1)
 
             game = chess.pgn.read_game(x)
             num_game += 1
 
-        self.actions = _spu.vstack(
-            [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
+        self.entries = _spu.vstack(
+            [self.entries, builder.build((idx, self.entry_size), np.uint8)]
         )
 
         if status:
             bar.close()
 
     def load_npz(self, x: Iterable[str]):
         """loads data from .npz file"""
@@ -94,69 +77,79 @@
 
                 mat = _spu.csr_matrix(
                     (
                         np.ones_like(indices, dtype=np.uint8),
                         indices,
                         loaded["mat_indptr"],
                     ),
-                    shape=(loaded["size"], VEC_SIZE),
+                    shape=(loaded["size"], self.entry_size),
                 )
 
-                self.actions = _spu.vstack([self.actions, mat])
+                self.entries = _spu.vstack([self.entries, mat])
                 self._update_labels(list(loaded["labels"]))
 
     def save(self, file: str) -> None:
         """saves the already loaded data to a compressed .npz file."""
 
         _save_dict = {}
         _save_dict.update(
-            mat_indices=self.actions.indices,
-            mat_indptr=self.actions.indptr,
+            mat_indices=self.entries.indices,
+            mat_indptr=self.entries.indptr,
             size=self.size,
         )
 
         if self.with_fen:
             _save_dict.update(labels=self.labels)
 
         np.savez_compressed(file, **_save_dict)
 
     @property
     def size(self) -> int:
-        return self.actions.shape[0]
+        return self.entries.shape[0]
 
     def batched(self, batch_size: int):
         for idx in range(0, self.size, batch_size):
             child = self.__new__(type(self))
             child.__init__(self.with_fen)
 
-            child.actions = self.actions[idx : idx + batch_size]
+            child.entries = self.entries[idx : idx + batch_size]
             child._update_labels(self.labels[idx : idx + batch_size])
 
             yield child
 
     def shuffle(self, *, seed: int = 42):
         rng = np.random.default_rng(seed)
-        idx = rng.permutation(len(self.actions))
+        idx = rng.permutation(len(self.entries))
 
-        self.actions = self.actions[idx]
+        self.entries = self.entries[idx]
 
         if self.with_fen:
             self.labels = list(np.array(self.labels)[idx])
 
     def cov(self) -> np.ndarray:
-        return _spu.scov(self.actions.T).toarray()
+        return _spu.scov(self.entries.T).toarray()
 
     def __add__(self, item):
         assert isinstance(item, type(self))
 
         new = self.__new__(type(self))
         new.__init__(self.with_fen)
 
-        new.actions = _spu.vstack([self.actions, item.actions])
+        new.entries = _spu.vstack([self.entries, item.entries])
 
         if self.with_fen:
             new.labels = self.labels + item.labels
 
         return new
 
     def __repr__(self):
         return "PositionLoader(size={})".format(self.size)
+
+
+class PositionLoader:
+    def __init__(
+        self,
+        *,
+        with_fen: bool = True,
+        pool_size: int = 1,
+    ) -> None:
+        raise NotImplementedError
```

### Comparing `chess2vec-0.1.5b9/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.2.0b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b9/chess2vec/_utils/sparse.py` & `chess2vec-0.2.0b1/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b9/chess2vec/_utils/vector.py` & `chess2vec-0.2.0b1/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b9/PKG-INFO` & `chess2vec-0.2.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.5b9
+Version: 0.2.0b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

