# Comparing `tmp/chess2vec-0.1.4b1.tar.gz` & `tmp/chess2vec-0.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.4b1.tar", max compression
+gzip compressed data, was "chess2vec-0.1.5b1.tar", max compression
```

## Comparing `chess2vec-0.1.4b1.tar` & `chess2vec-0.1.5b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.4b1/README.md
--rw-r--r--   0        0        0     4301 2024-04-17 23:02:52.220580 chess2vec-0.1.4b1/chess2vec/__init__.py
--rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.4b1/chess2vec/_utils/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.4b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0     1682 2024-04-17 22:29:19.024554 chess2vec-0.1.4b1/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.4b1/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.4b1/chess2vec/pgn.py
--rw-r--r--   0        0        0      358 2024-04-17 23:03:30.090569 chess2vec-0.1.4b1/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.4b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b1/README.md
+-rw-r--r--   0        0        0     4256 2024-04-17 23:21:15.918125 chess2vec-0.1.5b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b1/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1682 2024-04-17 23:09:58.018684 chess2vec-0.1.5b1/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b1/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-17 23:21:43.580323 chess2vec-0.1.5b1/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b1/PKG-INFO
```

### Comparing `chess2vec-0.1.4b1/chess2vec/__init__.py` & `chess2vec-0.1.5b1/chess2vec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import chess.pgn
 import numpy as np
 from tqdm import tqdm
 
 import chess2vec._utils as _u
 import chess2vec._utils.sparse as _spu
 
-VEC_BLOCK = 64 * 64
-VEC_SIZE = 5 * VEC_BLOCK
+VEC_SIZE = 5 * 64 * 64
 
 
-class PositionEncoder:
+class PositionLoader:
     def __init__(self, with_fen: bool = True) -> None:
         self.actions = _spu.csr_matrix((0, VEC_SIZE), dtype=np.uint8)
 
         self.with_fen = with_fen
 
         if self.with_fen:
             self.labels = []
@@ -28,15 +27,15 @@
     def load_fen(self, x: Iterable[str]):
         builder = _spu.csr_matrix_builder()
         idx = 0
 
         for fen in x:
             board = chess.Board(fen)
 
-            builder.add_entry(idx, list(_u.actions(board)))
+            builder.add_entry(idx, list(_u.actions(board)), np.uint8)
 
             idx += 1
 
         self._update_labels(list(x))
         self.actions = _spu.vstack(
             [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
         )
@@ -63,15 +62,15 @@
             self._update_labels([board.fen()])
 
             idx += 1
 
             for move in game.mainline_moves():
                 board.push(move)
 
-                builder.add_entry(idx, list(_u.actions(board)))
+                builder.add_entry(idx, list(_u.actions(board)), np.uint8)
                 self._update_labels([board.fen()])
 
                 idx += 1
 
             if status:
                 bar.update(1)
 
@@ -140,24 +139,22 @@
 
         if self.with_fen:
             self.labels = list(np.array(self.labels)[idx])
 
     def cov(self) -> np.ndarray:
         return _spu.scov(self.actions.T).toarray()
 
-    def encode(self) -> np.ndarray: ...
-
     def __add__(self, item):
         assert isinstance(item, type(self))
 
         new = self.__new__(type(self))
         new.__init__(self.with_fen)
 
         new.actions = _spu.vstack([self.actions, item.actions])
 
         if self.with_fen:
             new.labels = self.labels + item.labels
 
         return new
 
     def __repr__(self):
-        return "PositionEncoder(size={})".format(self.size)
+        return "PositionLoader(size={})".format(self.size)
```

### Comparing `chess2vec-0.1.4b1/chess2vec/_utils/__init__.py` & `chess2vec-0.1.5b1/chess2vec/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.4b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.5b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.4b1/chess2vec/_utils/sparse.py` & `chess2vec-0.1.5b1/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.4b1/chess2vec/_utils/vector.py` & `chess2vec-0.1.5b1/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.4b1/PKG-INFO` & `chess2vec-0.1.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.4b1
+Version: 0.1.5b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

