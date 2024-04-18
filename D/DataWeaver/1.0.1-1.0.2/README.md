# Comparing `tmp/dataweaver-1.0.1.tar.gz` & `tmp/dataweaver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataweaver-1.0.1.tar", last modified: Wed Apr 17 12:24:30 2024, max compression
+gzip compressed data, was "dataweaver-1.0.2.tar", last modified: Wed Apr 17 12:48:02 2024, max compression
```

## Comparing `dataweaver-1.0.1.tar` & `dataweaver-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:24:30.976466 dataweaver-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 12:24:18.000000 dataweaver-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-17 12:24:30.976466 dataweaver-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-17 12:24:18.000000 dataweaver-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 12:24:18.000000 dataweaver-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:24:30.976466 dataweaver-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:24:30.976466 dataweaver-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:24:30.976466 dataweaver-1.0.1/src/DataWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-17 12:24:30.000000 dataweaver-1.0.1/src/DataWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-17 12:24:30.000000 dataweaver-1.0.1/src/DataWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:24:30.000000 dataweaver-1.0.1/src/DataWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 12:24:30.000000 dataweaver-1.0.1/src/DataWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 12:24:30.000000 dataweaver-1.0.1/src/DataWeaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:24:30.976466 dataweaver-1.0.1/src/data_weaver/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 12:24:18.000000 dataweaver-1.0.1/src/data_weaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-17 12:24:18.000000 dataweaver-1.0.1/src/data_weaver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-17 12:24:18.000000 dataweaver-1.0.1/src/data_weaver/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-17 12:24:18.000000 dataweaver-1.0.1/src/data_weaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:48:02.752875 dataweaver-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 12:47:55.000000 dataweaver-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-17 12:48:02.752875 dataweaver-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-17 12:47:55.000000 dataweaver-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-17 12:47:55.000000 dataweaver-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:48:02.752875 dataweaver-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:48:02.752875 dataweaver-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:48:02.752875 dataweaver-1.0.2/src/DataWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-17 12:48:02.000000 dataweaver-1.0.2/src/DataWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-17 12:48:02.000000 dataweaver-1.0.2/src/DataWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:48:02.000000 dataweaver-1.0.2/src/DataWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 12:48:02.000000 dataweaver-1.0.2/src/DataWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 12:48:02.000000 dataweaver-1.0.2/src/DataWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:48:02.752875 dataweaver-1.0.2/src/data_weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 12:47:55.000000 dataweaver-1.0.2/src/data_weaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 12:47:55.000000 dataweaver-1.0.2/src/data_weaver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-17 12:47:55.000000 dataweaver-1.0.2/src/data_weaver/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-17 12:47:55.000000 dataweaver-1.0.2/src/data_weaver/utils.py
```

### Comparing `dataweaver-1.0.1/LICENSE` & `dataweaver-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.1/PKG-INFO` & `dataweaver-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataweaver-1.0.1/README.md` & `dataweaver-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.1/pyproject.toml` & `dataweaver-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DataWeaver"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "RICHARD Quentin", email = "richard.quentin88@gmail.com"}]
 description = "DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing."
 readme = "README.md"
 license = {text = "MIT License"}  # Update the license as appropriate
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dataweaver-1.0.1/src/DataWeaver.egg-info/PKG-INFO` & `dataweaver-1.0.2/src/DataWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataweaver-1.0.1/src/data_weaver/main.py` & `dataweaver-1.0.2/src/data_weaver/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import csv
 import yaml
 import os
 
 config = {}
 
 async def transform_value(value, field):
-    transform = config.get('transforms').get(field)
+    transform = config.get('transforms', {}).get(field)
     if transform and value is not None:
         print("Transforming value for field:", field, "with value:", value, "and transform:", transform)
         return await parse_transform(transform, value)
     return value
 
 async def get_new_key(key: str):
     """
@@ -43,17 +43,17 @@
     Returns:
         None
     """
     print("Mapping fields for data:", data)
     for key, source_key in config.get('mapping').items():
         print("Mapping key:", key, "with source key:", source_key)
         if isinstance(source_key, dict):
-            value = { key: data[key] for key in source_key}
+            value = { key: data.get(key) for key in source_key}
         elif isinstance(source_key, list):
-            value = [ data[key] for key in source_key]
+            value = [ data.get(key) for key in source_key]
         else : 
             value = data.get(source_key)
         
         final_value = await transform_value(value, key)
         final_result[key] = final_value
 
     # for full_key, value in data.items():
@@ -79,16 +79,16 @@
     #     if isinstance(value, dict):
     #         await parse_entry(value, final_result, full_key)
     #     elif isinstance(value, list):
     #         for i, item in enumerate(value):
     #             await parse_entry(item, final_result, full_key)
     #     else:
     await map_fields(object, final_result)
-
-    for key, value in config.get('additionalFields').items():
+    
+    for key, value in config.get('additionalFields', {}).items():
         final_value = await transform_value(value, key)
         final_result[key] = final_value
 
 async def process_entry(entry):
     final_result = {}
     flat_object = crush(entry)
     await parse_entry(flat_object, final_result)
```

### Comparing `dataweaver-1.0.1/src/data_weaver/transforms.py` & `dataweaver-1.0.2/src/data_weaver/transforms.py`

 * *Files identical despite different names*

### Comparing `dataweaver-1.0.1/src/data_weaver/utils.py` & `dataweaver-1.0.2/src/data_weaver/utils.py`

 * *Files identical despite different names*

