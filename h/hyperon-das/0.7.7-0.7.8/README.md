# Comparing `tmp/hyperon_das-0.7.7.tar.gz` & `tmp/hyperon_das-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das-0.7.7.tar", max compression
+gzip compressed data, was "hyperon_das-0.7.8.tar", max compression
```

## Comparing `hyperon_das-0.7.7.tar` & `hyperon_das-0.7.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1081 2024-04-17 13:55:50.226589 hyperon_das-0.7.7/LICENCE
--rw-r--r--   0        0        0    12442 2024-04-17 13:55:50.226589 hyperon_das-0.7.7/README.md
--rw-r--r--   0        0        0      108 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/__init__.py
--rw-r--r--   0        0        0       33 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/cache/__init__.py
--rw-r--r--   0        0        0    19594 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/cache/iterators.py
--rw-r--r--   0        0        0     6871 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/client.py
--rw-r--r--   0        0        0      127 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/constants.py
--rw-r--r--   0        0        0    31206 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/das.py
--rw-r--r--   0        0        0     1830 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/decorators.py
--rw-r--r--   0        0        0     1012 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/exceptions.py
--rw-r--r--   0        0        0     1072 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/logger.py
--rw-r--r--   0        0        0       39 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/pattern_matcher/__init__.py
--rw-r--r--   0        0        0      274 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/pattern_matcher/constants.py
--rw-r--r--   0        0        0    31913 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/pattern_matcher/pattern_matcher.py
--rw-r--r--   0        0        0    20941 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/query_engines.py
--rw-r--r--   0        0        0     1712 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/traverse_engines.py
--rw-r--r--   0        0        0     6700 2024-04-17 13:55:50.270588 hyperon_das-0.7.7/hyperon_das/utils.py
--rw-r--r--   0        0        0     1315 2024-04-17 13:55:59.998551 hyperon_das-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-18 19:43:54.505900 hyperon_das-0.7.8/LICENCE
+-rw-r--r--   0        0        0    12442 2024-04-18 19:43:54.505900 hyperon_das-0.7.8/README.md
+-rw-r--r--   0        0        0      108 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/cache/__init__.py
+-rw-r--r--   0        0        0    19594 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/cache/iterators.py
+-rw-r--r--   0        0        0     6871 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/client.py
+-rw-r--r--   0        0        0      127 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/constants.py
+-rw-r--r--   0        0        0    31206 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/das.py
+-rw-r--r--   0        0        0     1830 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/decorators.py
+-rw-r--r--   0        0        0     1012 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/logger.py
+-rw-r--r--   0        0        0       39 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/constants.py
+-rw-r--r--   0        0        0    31913 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/pattern_matcher/pattern_matcher.py
+-rw-r--r--   0        0        0    20938 2024-04-18 19:43:54.545900 hyperon_das-0.7.8/hyperon_das/query_engines.py
+-rw-r--r--   0        0        0     1712 2024-04-18 19:43:54.549900 hyperon_das-0.7.8/hyperon_das/traverse_engines.py
+-rw-r--r--   0        0        0     6700 2024-04-18 19:43:54.549900 hyperon_das-0.7.8/hyperon_das/utils.py
+-rw-r--r--   0        0        0     1315 2024-04-18 19:44:04.006019 hyperon_das-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.8/PKG-INFO
```

### Comparing `hyperon_das-0.7.7/LICENCE` & `hyperon_das-0.7.8/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/README.md` & `hyperon_das-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/cache/iterators.py` & `hyperon_das-0.7.8/hyperon_das/cache/iterators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/client.py` & `hyperon_das-0.7.8/hyperon_das/client.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/das.py` & `hyperon_das-0.7.8/hyperon_das/das.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/decorators.py` & `hyperon_das-0.7.8/hyperon_das/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/exceptions.py` & `hyperon_das-0.7.8/hyperon_das/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/logger.py` & `hyperon_das-0.7.8/hyperon_das/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/pattern_matcher/pattern_matcher.py` & `hyperon_das-0.7.8/hyperon_das/pattern_matcher/pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/query_engines.py` & `hyperon_das-0.7.8/hyperon_das/query_engines.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             )
         elif link_targets is not None:
             try:
                 return self.local_backend.get_matched_links(link_type, link_targets, **kwargs)
             except LinkDoesNotExist:
                 return None, [] if kwargs.get('cursor') is not None else []
         elif link_type != WILDCARD:
-            return self.local_backend.get_matched_type(link_type, **kwargs)
+            return self.local_backend.get_all_links(link_type, **kwargs)
         else:
             das_error(
                 ValueError(
                     f"Invalid parameters. link_type = {link_type} target_types = {target_types} link_targets = {link_targets}"
                 )
             )
```

### Comparing `hyperon_das-0.7.7/hyperon_das/traverse_engines.py` & `hyperon_das-0.7.8/hyperon_das/traverse_engines.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/hyperon_das/utils.py` & `hyperon_das-0.7.8/hyperon_das/utils.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.7/pyproject.toml` & `hyperon_das-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyperon-das"
-version = "0.7.7"
+version = "0.7.8"
 description = "Query Engine API for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das"}]
 
 [tool.poetry.urls]
 "Documentation" = "https://singnet.github.io/das-query-engine"
 "Code" = "https://github.com/singnet/das-query-engine"
 "Bug Tracker" = "https://github.com/singnet/das-query-engine/issues"
 "Releases" = "https://github.com/singnet/das-query-engine/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
-hyperon-das-atomdb = "0.6.6"
+hyperon-das-atomdb = "0.6.7"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 black = "^23.9.1"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das-0.7.7/PKG-INFO` & `hyperon_das-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperon-das
-Version: 0.7.7
+Version: 0.7.8
 Summary: Query Engine API for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyperon-das-atomdb (==0.6.6)
+Requires-Dist: hyperon-das-atomdb (==0.6.7)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-query-engine/issues
 Project-URL: Code, https://github.com/singnet/das-query-engine
 Project-URL: Documentation, https://singnet.github.io/das-query-engine
 Project-URL: Releases, https://github.com/singnet/das-query-engine/releases
 Description-Content-Type: text/markdown
```

