# Comparing `tmp/mkquartodocs-0.5.8.tar.gz` & `tmp/mkquartodocs-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkquartodocs-0.5.8.tar", max compression
+gzip compressed data, was "mkquartodocs-0.5.9.tar", max compression
```

## Comparing `mkquartodocs-0.5.8.tar` & `mkquartodocs-0.5.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-10-17 20:19:07.708370 mkquartodocs-0.5.8/LICENSE
--rw-r--r--   0        0        0     3088 2023-10-17 20:19:07.708370 mkquartodocs-0.5.8/docs/README.md
--rw-r--r--   0        0        0        0 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/mkquartodocs/__init__.py
--rw-r--r--   0        0        0     2938 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/mkquartodocs/context.py
--rw-r--r--   0        0        0     2795 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/mkquartodocs/extension.py
--rw-r--r--   0        0        0     2169 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/mkquartodocs/logging.py
--rw-r--r--   0        0        0     3413 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/mkquartodocs/plugin.py
--rw-r--r--   0        0        0     2123 2023-10-17 20:19:07.712369 mkquartodocs-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 mkquartodocs-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 16:28:28.384695 mkquartodocs-0.5.9/LICENSE
+-rw-r--r--   0        0        0     3088 2024-04-18 16:28:28.384695 mkquartodocs-0.5.9/docs/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/mkquartodocs/__init__.py
+-rw-r--r--   0        0        0     2938 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/mkquartodocs/context.py
+-rw-r--r--   0        0        0     2795 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/mkquartodocs/extension.py
+-rw-r--r--   0        0        0     2169 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/mkquartodocs/logging.py
+-rw-r--r--   0        0        0     3413 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/mkquartodocs/plugin.py
+-rw-r--r--   0        0        0     2123 2024-04-18 16:28:28.388695 mkquartodocs-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 mkquartodocs-0.5.9/PKG-INFO
```

### Comparing `mkquartodocs-0.5.8/LICENSE` & `mkquartodocs-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/docs/README.md` & `mkquartodocs-0.5.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/mkquartodocs/context.py` & `mkquartodocs-0.5.9/mkquartodocs/context.py`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/mkquartodocs/extension.py` & `mkquartodocs-0.5.9/mkquartodocs/extension.py`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/mkquartodocs/logging.py` & `mkquartodocs-0.5.9/mkquartodocs/logging.py`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/mkquartodocs/plugin.py` & `mkquartodocs-0.5.9/mkquartodocs/plugin.py`

 * *Files identical despite different names*

### Comparing `mkquartodocs-0.5.8/pyproject.toml` & `mkquartodocs-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "mkquartodocs"
-version = "0.5.8"
+version = "0.5.9"
 description = ""
 authors = ["J. Sebastian Paez <jspaezp@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "mkquartodocs" }]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 mkdocs = "^1.4.2"
 jupyter = "^1.0.0"
 nbformat = "^5.7.3"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.check.dependencies]
 black = "^22.8.0"
```

### Comparing `mkquartodocs-0.5.8/PKG-INFO` & `mkquartodocs-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mkquartodocs
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 License: Apache 2.0
 Author: J. Sebastian Paez
 Author-email: jspaezp@users.noreply.github.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: nbformat (>=5.7.3,<6.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
```

