# Comparing `tmp/chess2vec-0.2.1b6.tar.gz` & `tmp/chess2vec-0.2.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.2.1b6.tar", max compression
+gzip compressed data, was "chess2vec-0.2.1b7.tar", max compression
```

## Comparing `chess2vec-0.2.1b6.tar` & `chess2vec-0.2.1b7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b6/README.md
--rw-r--r--   0        0        0     4760 2024-04-18 18:15:03.143759 chess2vec-0.2.1b6/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b6/chess2vec/pgn.py
--rw-r--r--   0        0        0      571 2024-04-18 18:14:08.796474 chess2vec-0.2.1b6/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b6/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b6/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      358 2024-04-18 18:13:55.736327 chess2vec-0.2.1b6/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.2.1b7/README.md
+-rw-r--r--   0        0        0     4809 2024-04-18 18:16:32.898139 chess2vec-0.2.1b7/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-17 22:29:40.471647 chess2vec-0.2.1b7/chess2vec/pgn.py
+-rw-r--r--   0        0        0      571 2024-04-18 18:14:08.796474 chess2vec-0.2.1b7/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-18 15:35:59.781506 chess2vec-0.2.1b7/chess2vec/utils/sparse.py
+-rw-r--r--   0        0        0      583 2024-04-17 22:32:50.132164 chess2vec-0.2.1b7/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      358 2024-04-18 18:16:37.114855 chess2vec-0.2.1b7/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 chess2vec-0.2.1b7/PKG-INFO
```

### Comparing `chess2vec-0.2.1b6/chess2vec/__init__.py` & `chess2vec-0.2.1b7/chess2vec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,17 @@
                         indices,
                         loaded["mat_indptr"],
                     ),
                     shape=(loaded["size"], self.entry_size),
                 )
 
                 self.entries = sparse.vstack([self.entries, mat])
-                self._update_labels(list(loaded.get("labels")))
+                
+                if self.with_fen:
+                    self.labels += list(loaded.get("labels"))
 
     def save(self, file: str) -> None:
         """saves the already loaded data to a compressed .npz file."""
 
         _save_dict = {}
         _save_dict.update(
             mat_indices=self.entries.indices,
```

### Comparing `chess2vec-0.2.1b6/chess2vec/utils/__init__.py` & `chess2vec-0.2.1b7/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b6/chess2vec/utils/sparse.py` & `chess2vec-0.2.1b7/chess2vec/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b6/chess2vec/utils/vector.py` & `chess2vec-0.2.1b7/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.2.1b6/PKG-INFO` & `chess2vec-0.2.1b7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.2.1b6
+Version: 0.2.1b7
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

