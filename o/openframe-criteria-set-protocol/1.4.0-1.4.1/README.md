# Comparing `tmp/openframe_criteria_set_protocol-1.4.0.tar.gz` & `tmp/openframe_criteria_set_protocol-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openframe_criteria_set_protocol-1.4.0.tar", last modified: Thu Apr 18 11:45:39 2024, max compression
+gzip compressed data, was "openframe_criteria_set_protocol-1.4.1.tar", last modified: Thu Apr 18 12:05:22 2024, max compression
```

## Comparing `openframe_criteria_set_protocol-1.4.0.tar` & `openframe_criteria_set_protocol-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.305583 openframe_criteria_set_protocol-1.4.0/
--rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.0/LICENSE
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 11:45:39.305395 openframe_criteria_set_protocol-1.4.0/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.0/README.md
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.301723 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/
--rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.303976 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/errors.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/services.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     6201 2024-04-18 11:43:46.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/types.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     1628 2024-03-08 19:22:46.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/utils.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.305206 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 11:45:39.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-04-18 11:45:39.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-04-18 11:45:39.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 11:45:39.000000 openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/top_level.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-04-18 11:43:46.000000 openframe_criteria_set_protocol-1.4.0/pyproject.toml
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 11:45:39.305628 openframe_criteria_set_protocol-1.4.0/setup.cfg
--rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-04-18 11:43:46.000000 openframe_criteria_set_protocol-1.4.0/setup.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.304235 openframe_criteria_set_protocol-1.4.0/tests/
--rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.0/tests/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 11:45:39.304855 openframe_criteria_set_protocol-1.4.0/tests/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.0/tests/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.0/tests/v1/test_schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.0/tests/v1/test_types.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.593548 openframe_criteria_set_protocol-1.4.1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.1/LICENSE
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 12:05:22.593289 openframe_criteria_set_protocol-1.4.1/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.1/README.md
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.589259 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.591838 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/errors.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/services.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     6201 2024-04-18 11:43:46.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/types.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     1628 2024-03-08 19:22:46.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/utils.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.593065 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 12:05:22.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-04-18 12:05:22.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-04-18 12:05:22.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 12:05:22.000000 openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/top_level.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-04-18 12:05:16.000000 openframe_criteria_set_protocol-1.4.1/pyproject.toml
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 12:05:22.593618 openframe_criteria_set_protocol-1.4.1/setup.cfg
+-rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-04-18 12:05:16.000000 openframe_criteria_set_protocol-1.4.1/setup.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.592077 openframe_criteria_set_protocol-1.4.1/tests/
+-rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.1/tests/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 12:05:22.592654 openframe_criteria_set_protocol-1.4.1/tests/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.1/tests/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.1/tests/v1/test_schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.1/tests/v1/test_types.py
```

### Comparing `openframe_criteria_set_protocol-1.4.0/LICENSE` & `openframe_criteria_set_protocol-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/PKG-INFO` & `openframe_criteria_set_protocol-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.0
+Version: 1.4.1
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.0/README.md` & `openframe_criteria_set_protocol-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/errors.py` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/errors.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/schemas.py` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/services.py` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/services.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/types.py` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/types.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol/v1/utils.py` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol/v1/utils.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/PKG-INFO` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.0
+Version: 1.4.1
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.0/openframe_criteria_set_protocol.egg-info/SOURCES.txt` & `openframe_criteria_set_protocol-1.4.1/openframe_criteria_set_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/pyproject.toml` & `openframe_criteria_set_protocol-1.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openframe-criteria-set-protocol"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
     { name="Andrés Angulo", email="aa@openframe.org" },
 ]
 description = "A protocol and tools for defining and working with criteria sets"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `openframe_criteria_set_protocol-1.4.0/tests/v1/test_schemas.py` & `openframe_criteria_set_protocol-1.4.1/tests/v1/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.0/tests/v1/test_types.py` & `openframe_criteria_set_protocol-1.4.1/tests/v1/test_types.py`

 * *Files identical despite different names*

