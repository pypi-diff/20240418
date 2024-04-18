# Comparing `tmp/chess2vec-0.1.5b5.tar.gz` & `tmp/chess2vec-0.1.5b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.5b5.tar", max compression
+gzip compressed data, was "chess2vec-0.1.5b6.tar", max compression
```

## Comparing `chess2vec-0.1.5b5.tar` & `chess2vec-0.1.5b6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b5/README.md
--rw-r--r--   0        0        0     4339 2024-04-17 23:50:26.570551 chess2vec-0.1.5b5/chess2vec/__init__.py
--rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b5/chess2vec/_utils/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0     1727 2024-04-17 23:49:42.736185 chess2vec-0.1.5b5/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b5/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b5/chess2vec/pgn.py
--rw-r--r--   0        0        0      358 2024-04-17 23:51:43.819016 chess2vec-0.1.5b5/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b6/README.md
+-rw-r--r--   0        0        0     4391 2024-04-18 00:05:26.724889 chess2vec-0.1.5b6/chess2vec/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b6/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b6/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1727 2024-04-17 23:49:42.736185 chess2vec-0.1.5b6/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b6/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b6/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-18 00:05:38.431156 chess2vec-0.1.5b6/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b6/PKG-INFO
```

### Comparing `chess2vec-0.1.5b5/chess2vec/__init__.py` & `chess2vec-0.1.5b6/chess2vec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable, TextIO
 
 import chess
 import chess.pgn
 import numpy as np
 from tqdm import tqdm
+import gc
 
 import chess2vec._utils as _u
 import chess2vec._utils.sparse as _spu
 
 VEC_SIZE = 5 * 64 * 64
 
 
@@ -71,14 +72,16 @@
                 builder.add_entry(idx, actions, 1, np.uint8)
                 self._update_labels([board.fen()])
 
                 idx += 1
 
             if status:
                 bar.update(1)
+                
+            gc.collect()
 
             game = chess.pgn.read_game(x)
             num_game += 1
 
         self.actions = _spu.vstack(
             [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
         )
```

### Comparing `chess2vec-0.1.5b5/chess2vec/_utils/__init__.py` & `chess2vec-0.1.5b6/chess2vec/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b5/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.5b6/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b5/chess2vec/_utils/sparse.py` & `chess2vec-0.1.5b6/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b5/chess2vec/_utils/vector.py` & `chess2vec-0.1.5b6/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b5/PKG-INFO` & `chess2vec-0.1.5b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.5b5
+Version: 0.1.5b6
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
