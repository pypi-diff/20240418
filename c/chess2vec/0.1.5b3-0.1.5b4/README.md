# Comparing `tmp/chess2vec-0.1.5b3.tar.gz` & `tmp/chess2vec-0.1.5b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.1.5b3.tar", max compression
+gzip compressed data, was "chess2vec-0.1.5b4.tar", max compression
```

## Comparing `chess2vec-0.1.5b3.tar` & `chess2vec-0.1.5b4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b3/README.md
--rw-r--r--   0        0        0     4366 2024-04-17 23:45:07.782783 chess2vec-0.1.5b3/chess2vec/__init__.py
--rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b3/chess2vec/_utils/__init__.py
--rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
--rw-r--r--   0        0        0     1771 2024-04-17 23:43:54.230883 chess2vec-0.1.5b3/chess2vec/_utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b3/chess2vec/_utils/vector.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b3/chess2vec/pgn.py
--rw-r--r--   0        0        0      358 2024-04-17 23:45:21.206458 chess2vec-0.1.5b3/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.5b4/README.md
+-rw-r--r--   0        0        0     4275 2024-04-17 23:46:45.325231 chess2vec-0.1.5b4/chess2vec/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-17 22:35:26.885433 chess2vec-0.1.5b4/chess2vec/_utils/__init__.py
+-rw-r--r--   0        0        0     1910 2024-04-16 20:11:28.318615 chess2vec-0.1.5b4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc
+-rw-r--r--   0        0        0     1771 2024-04-17 23:43:54.230883 chess2vec-0.1.5b4/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.1.5b4/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.1.5b4/chess2vec/pgn.py
+-rw-r--r--   0        0        0      358 2024-04-17 23:46:53.455432 chess2vec-0.1.5b4/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.1.5b4/PKG-INFO
```

### Comparing `chess2vec-0.1.5b3/chess2vec/__init__.py` & `chess2vec-0.1.5b4/chess2vec/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,16 +58,14 @@
         while game and num_game < max_games:
             board = game.board()
 
             builder.add_entry(idx, list(_u.actions(board)), 1, np.uint8)
             self._update_labels([board.fen()])
 
             idx += 1
-            
-            print(len(builder.data), len(builder.rows), len(builder.columns))
 
             for move in game.mainline_moves():
                 board.push(move)
 
                 builder.add_entry(idx, list(_u.actions(board)), 1, np.uint8)
                 self._update_labels([board.fen()])
```

### Comparing `chess2vec-0.1.5b3/chess2vec/_utils/__init__.py` & `chess2vec-0.1.5b4/chess2vec/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b3/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc` & `chess2vec-0.1.5b4/chess2vec/_utils/__pycache__/sparse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b3/chess2vec/_utils/sparse.py` & `chess2vec-0.1.5b4/chess2vec/_utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b3/chess2vec/_utils/vector.py` & `chess2vec-0.1.5b4/chess2vec/_utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.1.5b3/PKG-INFO` & `chess2vec-0.1.5b4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.1.5b3
+Version: 0.1.5b4
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

