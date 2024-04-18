# Comparing `tmp/wkregister-0.0.2.tar.gz` & `tmp/wkregister-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkregister-0.0.2.tar", last modified: Thu Apr 18 17:21:47 2024, max compression
+gzip compressed data, was "wkregister-0.0.3.tar", last modified: Thu Apr 18 17:46:35 2024, max compression
```

## Comparing `wkregister-0.0.2.tar` & `wkregister-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.603553 wkregister-0.0.2/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.2/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:21:47.603308 wkregister-0.0.2/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.2/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 17:21:33.000000 wkregister-0.0.2/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 17:21:47.603598 wkregister-0.0.2/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.599502 wkregister-0.0.2/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.599870 wkregister-0.0.2/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.2/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      633 2024-04-18 17:20:58.000000 wkregister-0.0.2/src/test/test_logs.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      386 2024-04-16 17:18:54.000000 wkregister-0.0.2/src/test.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.601693 wkregister-0.0.2/src/wkregister/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.2/src/wkregister/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1849 2024-04-18 17:21:06.000000 wkregister-0.0.2/src/wkregister/decorator.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      420 2024-04-16 16:16:25.000000 wkregister-0.0.2/src/wkregister/models.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-16 17:09:58.000000 wkregister-0.0.2/src/wkregister/producer.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      690 2024-04-18 17:18:56.000000 wkregister-0.0.2/src/wkregister/util.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.602987 wkregister-0.0.2/src/wkregister.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/requires.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.449318 wkregister-0.0.3/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.3/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:46:35.449054 wkregister-0.0.3/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.3/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 17:46:25.000000 wkregister-0.0.3/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 17:46:35.449372 wkregister-0.0.3/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.446571 wkregister-0.0.3/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.446812 wkregister-0.0.3/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.3/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      668 2024-04-18 17:44:42.000000 wkregister-0.0.3/src/test/test_logs.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      417 2024-04-18 17:44:39.000000 wkregister-0.0.3/src/test.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.447713 wkregister-0.0.3/src/wkregister/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.3/src/wkregister/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1849 2024-04-18 17:43:59.000000 wkregister-0.0.3/src/wkregister/decorator.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      561 2024-04-18 17:43:57.000000 wkregister-0.0.3/src/wkregister/models.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-18 17:39:56.000000 wkregister-0.0.3/src/wkregister/producer.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      702 2024-04-18 17:45:49.000000 wkregister-0.0.3/src/wkregister/util.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:46:35.448795 wkregister-0.0.3/src/wkregister.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/requires.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:46:35.000000 wkregister-0.0.3/src/wkregister.egg-info/top_level.txt
```

### Comparing `wkregister-0.0.2/LICENSE` & `wkregister-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.2/PKG-INFO` & `wkregister-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkregister-0.0.2/README.md` & `wkregister-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.2/pyproject.toml` & `wkregister-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wkregister"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gustavo", email="gustavo.gordillo.giron@gmail.com" },
 ]
 description = "A wk register library for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wkregister-0.0.2/src/test/test_logs.py` & `wkregister-0.0.3/src/test/test_logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         org="nmi",
         key="commonsense",
         userId="2",
         actionType="update",
         status="success",
         errorMessage=None,
         service="pay-service",
+        payload={"hola": "mundo"},
     )
     return {"result": a + b, "record": record}
 
 
 class TestLogs(unittest.TestCase):
 
     def test_log(self):
```

### Comparing `wkregister-0.0.2/src/wkregister/decorator.py` & `wkregister-0.0.3/src/wkregister/decorator.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.2/src/wkregister/producer.py` & `wkregister-0.0.3/src/wkregister/producer.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.2/src/wkregister/util.py` & `wkregister-0.0.3/src/wkregister/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from wkregister.models import Records
 from typing import Callable, Any
+import json
 
 
 def kafkaParams(result: Any):
 
     # Retrieve 'record' or 'log', defaulting to None if neither is found
     log: Records = (result).get("record") or (result).get("log")
     # Check if 'log' was not retrieved and inform the user
```

### Comparing `wkregister-0.0.2/src/wkregister.egg-info/PKG-INFO` & `wkregister-0.0.3/src/wkregister.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

