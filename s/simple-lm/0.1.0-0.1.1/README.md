# Comparing `tmp/simple_lm-0.1.0.tar.gz` & `tmp/simple_lm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_lm-0.1.0.tar", max compression
+gzip compressed data, was "simple_lm-0.1.1.tar", max compression
```

## Comparing `simple_lm-0.1.0.tar` & `simple_lm-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      665 2024-04-18 06:03:15.343416 simple_lm-0.1.0/README.md
--rw-r--r--   0        0        0      424 2024-04-18 06:08:38.739837 simple_lm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 04:07:30.232837 simple_lm-0.1.0/simple_lm/__init__.py
--rw-r--r--   0        0        0     2012 2024-04-18 06:17:38.267379 simple_lm-0.1.0/simple_lm/core.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 simple_lm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      665 2024-04-18 06:03:15.343416 simple_lm-0.1.1/README.md
+-rw-r--r--   0        0        0      424 2024-04-18 06:28:04.460273 simple_lm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-18 06:27:42.611100 simple_lm-0.1.1/simple_lm/__init__.py
+-rw-r--r--   0        0        0     2012 2024-04-18 06:17:38.267379 simple_lm-0.1.1/simple_lm/core.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 simple_lm-0.1.1/PKG-INFO
```

### Comparing `simple_lm-0.1.0/README.md` & `simple_lm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simple_lm-0.1.0/simple_lm/core.py` & `simple_lm-0.1.1/simple_lm/core.py`

 * *Files identical despite different names*

### Comparing `simple_lm-0.1.0/PKG-INFO` & `simple_lm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-lm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple abstraction over instructor for LLM apps
 License: MIT
 Author: Joe Petrantoni
 Author-email: 79169021+jpetrantoni@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

