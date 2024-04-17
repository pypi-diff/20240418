# Comparing `tmp/chess2vec-0.1.5b1.tar.gz` & `tmp/chess2vec-0.1.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.5b1.tar", max compression
+gzip compressed data, was "chess2vec-0.1.5b2.tar", max compression
```

## Comparing `chess2vec-0.1.5b1.tar` & `chess2vec-0.1.5b2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b1/README.md
--rw-r--r--   0        0        0     4256 2024-04-17 23:21:15.918125 chess2vec-0.1.5b1/chess2vec/__init__.py
--rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b1/chess2vec/_utils/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0     1682 2024-04-17 23:09:58.018684 chess2vec-0.1.5b1/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b1/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b1/chess2vec/pgn.py
--rw-r--r--   0        0        0      358 2024-04-17 23:21:43.580323 chess2vec-0.1.5b1/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b2/README.md
+-rw-r--r--   0        0        0     4262 2024-04-17 23:24:12.272314 chess2vec-0.1.5b2/chess2vec/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b2/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1682 2024-04-17 23:09:58.018684 chess2vec-0.1.5b2/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b2/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b2/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-17 23:24:20.066208 chess2vec-0.1.5b2/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b2/PKG-INFO
```

### Comparing `chess2vec-0.1.5b1/chess2vec/__init__.py` & `chess2vec-0.1.5b2/chess2vec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
             builder.add_entry(idx, list(_u.actions(board)), np.uint8)
 
             idx += 1
 
         self._update_labels(list(x))
         self.actions = _spu.vstack(
-            [self.actions, builder.build((idx, VEC_SIZE), np.uint8)]
+            [self.actions, builder.build((idx, VEC_SIZE), np.uint8(1))]
         )
 
     def load_pgn(self, x: TextIO, max_games: int = None, status: bool = False):
         if max_games <= 0:
             return
 
         if max_games is None:
@@ -62,15 +62,15 @@
             self._update_labels([board.fen()])
 
             idx += 1
 
             for move in game.mainline_moves():
                 board.push(move)
 
-                builder.add_entry(idx, list(_u.actions(board)), np.uint8)
+                builder.add_entry(idx, list(_u.actions(board)), np.uint8(1))
                 self._update_labels([board.fen()])
 
                 idx += 1
 
             if status:
                 bar.update(1)
```

### Comparing `chess2vec-0.1.5b1/chess2vec/_utils/__init__.py` & `chess2vec-0.1.5b2/chess2vec/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b1/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.5b2/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b1/chess2vec/_utils/sparse.py` & `chess2vec-0.1.5b2/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b1/chess2vec/_utils/vector.py` & `chess2vec-0.1.5b2/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b1/PKG-INFO` & `chess2vec-0.1.5b2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.5b1
+Version: 0.1.5b2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

