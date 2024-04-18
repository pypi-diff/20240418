# Comparing `tmp/makenew_pypackage-5.1.0.tar.gz` & `tmp/makenew_pypackage-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makenew_pypackage-5.1.0.tar", max compression
+gzip compressed data, was "makenew_pypackage-5.1.1.tar", max compression
```

## Comparing `makenew_pypackage-5.1.0.tar` & `makenew_pypackage-5.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0     7662 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/README.rst
--rw-r--r--   0        0        0       46 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/__init__.py
--rw-r--r--   0        0        0       56 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/todo.py
--rw-r--r--   0        0        0      156 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/makenew_pypackage/todo_test.py
--rw-r--r--   0        0        0      615 2024-04-18 07:21:35.843815 makenew_pypackage-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 makenew_pypackage-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     7662 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/README.rst
+-rw-r--r--   0        0        0       46 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/makenew_pypackage/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/makenew_pypackage/todo.py
+-rw-r--r--   0        0        0      156 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/makenew_pypackage/todo_test.py
+-rw-r--r--   0        0        0      615 2024-04-18 07:41:03.282618 makenew_pypackage-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 makenew_pypackage-5.1.1/PKG-INFO
```

### Comparing `makenew_pypackage-5.1.0/LICENSE.txt` & `makenew_pypackage-5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `makenew_pypackage-5.1.0/README.rst` & `makenew_pypackage-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `makenew_pypackage-5.1.0/pyproject.toml` & `makenew_pypackage-5.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makenew-pypackage"
-version = "5.1.0"
+version = "5.1.1"
 description = "Package skeleton for a Python module."
 authors = ["Evan Sosenko <razorx@evansosenko.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/makenew/pypackage"
 repository = "https://github.com/makenew/pypackage"
```

### Comparing `makenew_pypackage-5.1.0/PKG-INFO` & `makenew_pypackage-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makenew-pypackage
-Version: 5.1.0
+Version: 5.1.1
 Summary: Package skeleton for a Python module.
 Home-page: https://github.com/makenew/pypackage
 License: MIT
 Author: Evan Sosenko
 Author-email: razorx@evansosenko.com
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

