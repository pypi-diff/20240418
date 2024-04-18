# Comparing `tmp/chess2vec-0.2.1b2.tar.gz` & `tmp/chess2vec-0.2.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.2.1b2.tar", max compression
+gzip compressed data, was "chess2vec-0.2.1b3.tar", max compression
```

## Comparing `chess2vec-0.2.1b2.tar` & `chess2vec-0.2.1b3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b2/README.md
--rw-r--r--   0        0        0     4209 2024-04-18 16:05:15.756722 chess2vec-0.2.1b2/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b2/chess2vec/pgn.py
--rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b2/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b2/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b2/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-18 16:05:21.870151 chess2vec-0.2.1b2/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b3/README.md
+-rw-r--r--   0        0        0     4175 2024-04-18 16:07:58.865951 chess2vec-0.2.1b3/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b3/chess2vec/pgn.py
+-rw-r--r--   0        0        0      565 2024-04-18 15:47:24.923043 chess2vec-0.2.1b3/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b3/chess2vec/utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b3/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-18 16:08:10.062793 chess2vec-0.2.1b3/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b3/PKG-INFO
```

### Comparing `chess2vec-0.2.1b2/chess2vec/__init__.py` & `chess2vec-0.2.1b3/chess2vec/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 
 class PositionLoader:
     def __init__(self, *, with_fen=False, rep: Literal["piece", "action"] = "piece"):
         self.rep = rep
 
         if self.rep == "piece":
-            self.entries = sparse.csr_matrix((0,), dtype=np.uint8)
-            self._entries_getter = utils.yield_pieces
             self.entry_size = 2 * 6 * 64
+            self._entries_getter = utils.yield_pieces
 
         elif self.rep == "action":
-            self.entries = sparse.csr_matrix((0, 6 * 64 * 64), dtype=np.uint8)
-            self._entries_getter = utils.yield_actions
             self.entry_size = 6 * 64 * 64
-
+            self._entries_getter = utils.yield_actions
+            
         else:
             raise TypeError
-
+            
+        self.entries = sparse.csr_matrix((0, self.entry_size), dtype=np.uint8)
         self.with_fen = with_fen
+        
         if self.with_fen:
             self.labels = []
 
     def _update_labels(self, labels: Iterable[str]):
         if self.with_fen:
             self.labels += labels
```

### Comparing `chess2vec-0.2.1b2/chess2vec/utils/__init__.py` & `chess2vec-0.2.1b3/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b2/chess2vec/utils/sparse.py` & `chess2vec-0.2.1b3/chess2vec/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b2/chess2vec/utils/vector.py` & `chess2vec-0.2.1b3/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b2/PKG-INFO` & `chess2vec-0.2.1b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.2.1b2
+Version: 0.2.1b3
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

