# Comparing `tmp/dash-id-utils-0.0.1.tar.gz` & `tmp/dash-id-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-id-utils-0.0.1.tar", last modified: Mon Nov  6 07:22:31 2023, max compression
+gzip compressed data, was "dash-id-utils-0.0.2.tar", last modified: Thu Apr 18 08:21:09 2024, max compression
```

## Comparing `dash-id-utils-0.0.1.tar` & `dash-id-utils-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2023-11-06 07:22:31.703973 dash-id-utils-0.0.1/
--rw-r--r--   0 wfluo      (502) staff       (20)     1175 2023-11-06 07:22:31.703748 dash-id-utils-0.0.1/PKG-INFO
--rw-r--r--   0 wfluo      (502) staff       (20)      909 2023-11-06 07:06:05.000000 dash-id-utils-0.0.1/README.md
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2023-11-06 07:22:31.701577 dash-id-utils-0.0.1/dash_id_utils/
--rw-r--r--   0 wfluo      (502) staff       (20)     2056 2023-11-06 07:10:35.000000 dash-id-utils-0.0.1/dash_id_utils/__init__.py
-drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2023-11-06 07:22:31.703495 dash-id-utils-0.0.1/dash_id_utils.egg-info/
--rw-r--r--   0 wfluo      (502) staff       (20)     1175 2023-11-06 07:22:31.000000 dash-id-utils-0.0.1/dash_id_utils.egg-info/PKG-INFO
--rw-r--r--   0 wfluo      (502) staff       (20)      228 2023-11-06 07:22:31.000000 dash-id-utils-0.0.1/dash_id_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wfluo      (502) staff       (20)        1 2023-11-06 07:22:31.000000 dash-id-utils-0.0.1/dash_id_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wfluo      (502) staff       (20)        5 2023-11-06 07:22:31.000000 dash-id-utils-0.0.1/dash_id_utils.egg-info/requires.txt
--rw-r--r--   0 wfluo      (502) staff       (20)       14 2023-11-06 07:22:31.000000 dash-id-utils-0.0.1/dash_id_utils.egg-info/top_level.txt
--rw-r--r--   0 wfluo      (502) staff       (20)       38 2023-11-06 07:22:31.704100 dash-id-utils-0.0.1/setup.cfg
--rw-r--r--   0 wfluo      (502) staff       (20)      567 2023-11-06 07:22:28.000000 dash-id-utils-0.0.1/setup.py
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-18 08:21:09.600802 dash-id-utils-0.0.2/
+-rw-r--r--   0 wfluo      (502) staff       (20)     1175 2024-04-18 08:21:09.600589 dash-id-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 wfluo      (502) staff       (20)      909 2023-11-06 07:06:05.000000 dash-id-utils-0.0.2/README.md
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-18 08:21:09.595523 dash-id-utils-0.0.2/dash_id_utils/
+-rw-r--r--   0 wfluo      (502) staff       (20)     2372 2024-04-18 08:20:32.000000 dash-id-utils-0.0.2/dash_id_utils/__init__.py
+drwxr-xr-x   0 wfluo      (502) staff       (20)        0 2024-04-18 08:21:09.600288 dash-id-utils-0.0.2/dash_id_utils.egg-info/
+-rw-r--r--   0 wfluo      (502) staff       (20)     1175 2024-04-18 08:21:09.000000 dash-id-utils-0.0.2/dash_id_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wfluo      (502) staff       (20)      228 2024-04-18 08:21:09.000000 dash-id-utils-0.0.2/dash_id_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)        1 2024-04-18 08:21:09.000000 dash-id-utils-0.0.2/dash_id_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)        5 2024-04-18 08:21:09.000000 dash-id-utils-0.0.2/dash_id_utils.egg-info/requires.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)       14 2024-04-18 08:21:09.000000 dash-id-utils-0.0.2/dash_id_utils.egg-info/top_level.txt
+-rw-r--r--   0 wfluo      (502) staff       (20)       38 2024-04-18 08:21:09.600871 dash-id-utils-0.0.2/setup.cfg
+-rw-r--r--   0 wfluo      (502) staff       (20)      567 2024-04-18 08:20:37.000000 dash-id-utils-0.0.2/setup.py
```

### Comparing `dash-id-utils-0.0.1/PKG-INFO` & `dash-id-utils-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-id-utils
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/pragmatic-dash/dash-id-utils
 Author: mapix
 Author-email: mapix.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dash-id-utils-0.0.1/README.md` & `dash-id-utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dash-id-utils-0.0.1/dash_id_utils/__init__.py` & `dash-id-utils-0.0.2/dash_id_utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from copy import copy
+import json
+
 from dash import ALL, Output, Input, State
 
+
 __all__ = ["DashIDGenerator", "DashIDWrapper"]
 
 
 class DashIDWrapper:
     def __init__(self, id):
         self.id = id
 
@@ -15,14 +18,19 @@
         return Output(self.get_identifier(), property, allow_duplicate=allow_duplicate)
 
     def get_input(self, property):
         return Input(self.get_identifier(), property)
 
     def get_state(self, property):
         return State(self.get_identifier(), property)
+    
+    def __str__(self):
+        if isinstance(self.id, dict):
+            return json.dumps(self.id, sort_keys=True, separators=(",", ":"))
+        return str(self.id)
 
 
 class DashIDGenerator:
     def __init__(
         self,
         page="default",
         type="default",
@@ -67,7 +75,11 @@
             return Input(self.get_pattern(pattern), property)
         return Input(self.get_identifier(), property)
 
     def get_state(self, property, pattern=None):
         if pattern:
             return State(self.get_pattern(pattern), property)
         return State(self.get_identifier(), property)
+
+    def __str__(self):
+        id_ = self.get_identifier()
+        return json.dumps(id_, sort_keys=True, separators=(",", ":"))
```

### Comparing `dash-id-utils-0.0.1/dash_id_utils.egg-info/PKG-INFO` & `dash-id-utils-0.0.2/dash_id_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-id-utils
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/pragmatic-dash/dash-id-utils
 Author: mapix
 Author-email: mapix.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `dash-id-utils-0.0.1/setup.py` & `dash-id-utils-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 extra = {}
 
 with open('README.md', 'rt') as f:
     extra['long_description'] = f.read()
 
 setup(
     name='dash-id-utils',
-    version='0.0.1',
+    version='0.0.2',
     description='',
     author='mapix',
     author_email='mapix.me@gmail.com',
     url='https://github.com/pragmatic-dash/dash-id-utils',
     license='MIT',
     packages=find_packages(),
     long_description_content_type='text/markdown',
```

