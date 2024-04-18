# Comparing `tmp/types_pyone-0.1.6.1.tar.gz` & `tmp/types_pyone-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_pyone-0.1.6.1.tar", last modified: Mon Apr 15 13:29:26 2024, max compression
+gzip compressed data, was "types_pyone-0.1.7.tar", last modified: Thu Apr 18 09:02:27 2024, max compression
```

## Comparing `types_pyone-0.1.6.1.tar` & `types_pyone-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-15 13:29:26.394731 types_pyone-0.1.6.1/
--rw-rw-r--   0 evil      (1000) evil      (1000)     1069 2024-04-15 11:50:21.000000 types_pyone-0.1.6.1/LICENSE
--rw-r--r--   0 evil      (1000) evil      (1000)      755 2024-04-15 13:29:26.394731 types_pyone-0.1.6.1/PKG-INFO
--rw-rw-r--   0 evil      (1000) evil      (1000)      129 2024-04-15 13:27:39.000000 types_pyone-0.1.6.1/README.md
--rw-rw-r--   0 evil      (1000) evil      (1000)      732 2024-04-15 13:28:39.000000 types_pyone-0.1.6.1/pyproject.toml
--rw-rw-r--   0 evil      (1000) evil      (1000)       38 2024-04-15 13:29:26.394731 types_pyone-0.1.6.1/setup.cfg
-drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-15 13:29:26.390733 types_pyone-0.1.6.1/src/
-drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-15 13:29:26.390733 types_pyone-0.1.6.1/src/pyone/
--rw-rw-r--   0 evil      (1000) evil      (1000)     2039 2024-04-15 09:44:25.000000 types_pyone-0.1.6.1/src/pyone/__init__.pyi
--rw-rw-r--   0 evil      (1000) evil      (1000)      559 2024-04-15 09:45:20.000000 types_pyone-0.1.6.1/src/pyone/acl.pyi
--rw-rw-r--   0 evil      (1000) evil      (1000)      455 2024-04-15 09:43:34.000000 types_pyone-0.1.6.1/src/pyone/helpers.pyi
--rw-rw-r--   0 evil      (1000) evil      (1000)        0 2024-04-15 10:03:41.000000 types_pyone-0.1.6.1/src/pyone/py.typed
--rw-rw-r--   0 evil      (1000) evil      (1000)      363 2024-04-15 09:03:03.000000 types_pyone-0.1.6.1/src/pyone/server.pyi
--rw-rw-r--   0 evil      (1000) evil      (1000)     1054 2024-04-15 09:45:43.000000 types_pyone-0.1.6.1/src/pyone/tester.pyi
--rw-rw-r--   0 evil      (1000) evil      (1000)      698 2024-04-15 09:45:52.000000 types_pyone-0.1.6.1/src/pyone/util.pyi
-drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-15 13:29:26.394731 types_pyone-0.1.6.1/src/types_pyone.egg-info/
--rw-r--r--   0 evil      (1000) evil      (1000)      755 2024-04-15 13:29:26.000000 types_pyone-0.1.6.1/src/types_pyone.egg-info/PKG-INFO
--rw-rw-r--   0 evil      (1000) evil      (1000)      369 2024-04-15 13:29:26.000000 types_pyone-0.1.6.1/src/types_pyone.egg-info/SOURCES.txt
--rw-rw-r--   0 evil      (1000) evil      (1000)        1 2024-04-15 13:29:26.000000 types_pyone-0.1.6.1/src/types_pyone.egg-info/dependency_links.txt
--rw-rw-r--   0 evil      (1000) evil      (1000)        6 2024-04-15 13:29:26.000000 types_pyone-0.1.6.1/src/types_pyone.egg-info/requires.txt
--rw-rw-r--   0 evil      (1000) evil      (1000)        6 2024-04-15 13:29:26.000000 types_pyone-0.1.6.1/src/types_pyone.egg-info/top_level.txt
+drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-18 09:02:27.623977 types_pyone-0.1.7/
+-rw-rw-r--   0 evil      (1000) evil      (1000)     1069 2024-04-15 11:50:21.000000 types_pyone-0.1.7/LICENSE
+-rw-r--r--   0 evil      (1000) evil      (1000)      753 2024-04-18 09:02:27.623977 types_pyone-0.1.7/PKG-INFO
+-rw-rw-r--   0 evil      (1000) evil      (1000)      129 2024-04-15 13:27:39.000000 types_pyone-0.1.7/README.md
+-rw-rw-r--   0 evil      (1000) evil      (1000)      730 2024-04-18 09:02:01.000000 types_pyone-0.1.7/pyproject.toml
+-rw-rw-r--   0 evil      (1000) evil      (1000)       38 2024-04-18 09:02:27.623977 types_pyone-0.1.7/setup.cfg
+drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-18 09:02:27.619978 types_pyone-0.1.7/src/
+drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-18 09:02:27.619978 types_pyone-0.1.7/src/pyone/
+-rw-rw-r--   0 evil      (1000) evil      (1000)     2650 2024-04-18 08:58:46.000000 types_pyone-0.1.7/src/pyone/__init__.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)      559 2024-04-15 09:45:20.000000 types_pyone-0.1.7/src/pyone/acl.pyi
+drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-18 09:02:27.619978 types_pyone-0.1.7/src/pyone/bindings/
+-rw-rw-r--   0 evil      (1000) evil      (1000)      426 2024-04-18 08:56:40.000000 types_pyone-0.1.7/src/pyone/bindings/__init__.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)        0 2024-04-18 08:52:03.000000 types_pyone-0.1.7/src/pyone/bindings/supbind.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)      455 2024-04-15 09:43:34.000000 types_pyone-0.1.7/src/pyone/helpers.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)        0 2024-04-15 10:03:41.000000 types_pyone-0.1.7/src/pyone/py.typed
+-rw-rw-r--   0 evil      (1000) evil      (1000)      363 2024-04-15 09:03:03.000000 types_pyone-0.1.7/src/pyone/server.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)     1054 2024-04-15 09:45:43.000000 types_pyone-0.1.7/src/pyone/tester.pyi
+-rw-rw-r--   0 evil      (1000) evil      (1000)      698 2024-04-15 09:45:52.000000 types_pyone-0.1.7/src/pyone/util.pyi
+drwxrwxr-x   0 evil      (1000) evil      (1000)        0 2024-04-18 09:02:27.623977 types_pyone-0.1.7/src/types_pyone.egg-info/
+-rw-r--r--   0 evil      (1000) evil      (1000)      753 2024-04-18 09:02:27.000000 types_pyone-0.1.7/src/types_pyone.egg-info/PKG-INFO
+-rw-rw-r--   0 evil      (1000) evil      (1000)      432 2024-04-18 09:02:27.000000 types_pyone-0.1.7/src/types_pyone.egg-info/SOURCES.txt
+-rw-rw-r--   0 evil      (1000) evil      (1000)        1 2024-04-18 09:02:27.000000 types_pyone-0.1.7/src/types_pyone.egg-info/dependency_links.txt
+-rw-rw-r--   0 evil      (1000) evil      (1000)        6 2024-04-18 09:02:27.000000 types_pyone-0.1.7/src/types_pyone.egg-info/requires.txt
+-rw-rw-r--   0 evil      (1000) evil      (1000)        6 2024-04-18 09:02:27.000000 types_pyone-0.1.7/src/types_pyone.egg-info/top_level.txt
```

### Comparing `types_pyone-0.1.6.1/LICENSE` & `types_pyone-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `types_pyone-0.1.6.1/PKG-INFO` & `types_pyone-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyone
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Type stubs for pyone library
 Author: d34d5p4rr0w
 Project-URL: Homepage, https://github.com/d34d5p4rr0w/types-pyone
 Project-URL: Issues, https://github.com/d34d5p4rr0w/types-pyone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `types_pyone-0.1.6.1/pyproject.toml` & `types_pyone-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "types-pyone"
-version = "0.1.6.1"
+version = "0.1.7"
 authors = [
   { name="d34d5p4rr0w" },
 ]
 description = "Type stubs for pyone library"
 readme = "README.md"
 dependencies = [
     "pyone"
```

### Comparing `types_pyone-0.1.6.1/src/pyone/acl.pyi` & `types_pyone-0.1.7/src/pyone/acl.pyi`

 * *Files identical despite different names*

### Comparing `types_pyone-0.1.6.1/src/pyone/tester.pyi` & `types_pyone-0.1.7/src/pyone/tester.pyi`

 * *Files identical despite different names*

### Comparing `types_pyone-0.1.6.1/src/pyone/util.pyi` & `types_pyone-0.1.7/src/pyone/util.pyi`

 * *Files identical despite different names*

### Comparing `types_pyone-0.1.6.1/src/types_pyone.egg-info/PKG-INFO` & `types_pyone-0.1.7/src/types_pyone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyone
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Type stubs for pyone library
 Author: d34d5p4rr0w
 Project-URL: Homepage, https://github.com/d34d5p4rr0w/types-pyone
 Project-URL: Issues, https://github.com/d34d5p4rr0w/types-pyone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

