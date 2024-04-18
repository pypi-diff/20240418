# Comparing `tmp/das_readability-1.0.7.tar.gz` & `tmp/das_readability-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "das_readability-1.0.7.tar", max compression
+gzip compressed data, was "das_readability-1.0.9.tar", max compression
```

## Comparing `das_readability-1.0.7.tar` & `das_readability-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       35 2024-04-17 11:49:15.852161 das_readability-1.0.7/LICENSE
--rw-r--r--   0        0        0     1821 2024-04-18 10:02:08.774946 das_readability-1.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-17 11:33:43.740872 das_readability-1.0.7/das_readability/__init__.py
--rw-r--r--   0        0        0       87 2024-04-18 08:01:24.044671 das_readability-1.0.7/das_readability/__main__.py
--rw-r--r--   0        0        0     6876 2024-04-18 09:51:07.179652 das_readability-1.0.7/das_readability/readability.py
--rw-r--r--   0        0        0     1060 2024-04-18 11:09:01.469219 das_readability-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 das_readability-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-04-18 11:20:57.182356 das_readability-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1821 2024-04-18 11:20:57.182356 das_readability-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 11:20:57.182356 das_readability-1.0.9/das_readability/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-18 11:20:57.182356 das_readability-1.0.9/das_readability/__main__.py
+-rw-r--r--   0        0        0     6876 2024-04-18 11:20:57.186357 das_readability-1.0.9/das_readability/readability.py
+-rw-r--r--   0        0        0     1060 2024-04-18 11:20:57.186357 das_readability-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 das_readability-1.0.9/PKG-INFO
```

### Comparing `das_readability-1.0.7/README.md` & `das_readability-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `das_readability-1.0.7/das_readability/readability.py` & `das_readability-1.0.9/das_readability/readability.py`

 * *Files identical despite different names*

### Comparing `das_readability-1.0.7/pyproject.toml` & `das_readability-1.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "das-readability"
-version = "1.0.7"
+version = "1.0.9"
 description = "Checks the readability of markdown files in a directory and its subdirectories."
 authors = ["lzvb <lzvb@novonordisk.com>"]
 license = "Copyright (C) 2024 Novo Nordisk A/S"
 readme = "README.md"
 packages = [{include = "das_readability"}]
 repository = "https://github.com/innersource-nn/das-readability"
 documentation = "https://github.com/innersource-nn/das-readability"
```

### Comparing `das_readability-1.0.7/PKG-INFO` & `das_readability-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: das-readability
-Version: 1.0.7
+Version: 1.0.9
 Summary: Checks the readability of markdown files in a directory and its subdirectories.
 Home-page: https://github.com/innersource-nn/das-readability
 License: Copyright (C) 2024 Novo Nordisk A/S
 Keywords: readability,markdown,textstat,cli,smog,reading,ease,flesch
 Author: lzvb
 Author-email: lzvb@novonordisk.com
 Requires-Python: >=3.9.7,<4.0.0
```

