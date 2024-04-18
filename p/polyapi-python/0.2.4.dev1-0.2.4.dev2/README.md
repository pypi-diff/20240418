# Comparing `tmp/polyapi_python-0.2.4.dev1.tar.gz` & `tmp/polyapi_python-0.2.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.4.dev1.tar", last modified: Wed Apr 17 19:06:11 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.4.dev2.tar", last modified: Thu Apr 18 19:48:37 2024, max compression
```

## Comparing `polyapi_python-0.2.4.dev1.tar` & `polyapi_python-0.2.4.dev2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-17 19:06:11.000000 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 19:06:11.000000 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:06:11.000000 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 19:06:11.000000 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 19:06:11.000000 polyapi_python-0.2.4.dev1/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:06:11.470075 polyapi_python-0.2.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-17 19:06:03.000000 polyapi_python-0.2.4.dev1/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:37.030874 polyapi_python-0.2.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-18 19:48:37.026874 polyapi_python-0.2.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:37.026874 polyapi_python-0.2.4.dev2/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:37.026874 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-18 19:48:37.000000 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-18 19:48:37.000000 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:48:37.000000 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-18 19:48:37.000000 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 19:48:37.000000 polyapi_python-0.2.4.dev2/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:48:37.030874 polyapi_python-0.2.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:37.026874 polyapi_python-0.2.4.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 19:48:32.000000 polyapi_python-0.2.4.dev2/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.4.dev1/LICENSE` & `polyapi_python-0.2.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/PKG-INFO` & `polyapi_python-0.2.4.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev1
+Version: 0.2.4.dev2
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,14 @@
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: jsonschema-gentypes==2.4.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: stdlib_list==0.10.0
 Requires-Dist: colorama==0.4.4
 Requires-Dist: python-socketio[asyncio_client]==5.11.1
 Requires-Dist: truststore==0.8.0
-Requires-Dist: pyjwt==2.3.0
 
 # PolyAPI Python Library
 
 The PolyAPI Python Library lets you use and define PolyAPI functions using Python.
 
 ## PolyAPI Quickstart
```

### Comparing `polyapi_python-0.2.4.dev1/README.md` & `polyapi_python-0.2.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/api.py` & `polyapi_python-0.2.4.dev2/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/auth.py` & `polyapi_python-0.2.4.dev2/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/cli.py` & `polyapi_python-0.2.4.dev2/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/client.py` & `polyapi_python-0.2.4.dev2/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/config.py` & `polyapi_python-0.2.4.dev2/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/error_handler.py` & `polyapi_python-0.2.4.dev2/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/execute.py` & `polyapi_python-0.2.4.dev2/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/function_cli.py` & `polyapi_python-0.2.4.dev2/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/generate.py` & `polyapi_python-0.2.4.dev2/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/schema.py` & `polyapi_python-0.2.4.dev2/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/server.py` & `polyapi_python-0.2.4.dev2/polyapi/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 {args}
 ) -> {return_type_name}:
     \"""{function_description}
 
     Function ID: {function_id}
     \"""
     resp = execute("{function_type}", "{function_id}", {data})
-    return {return_action}
+    try:
+        return {return_action}
+    except:
+        return resp.text
 """
 
 
 def render_server_function(
     function_type: str,
     function_name: str,
     function_id: str,
@@ -50,18 +53,10 @@
     )
     return func_str, func_type_defs
 
 
 def _get_server_return_action(return_type_name: str) -> str:
     if return_type_name == "str":
         return_action = "resp.text"
-    elif return_type_name == "Any":
-        return_action = "resp.text"
-    elif return_type_name == "int":
-        return_action = "int(resp.text.replace('(int) ', ''))"
-    elif return_type_name == "float":
-        return_action = "float(resp.text.replace('(float) ', ''))"
-    elif return_type_name == "bool":
-        return_action = "False if resp.text == 'False' else True"
     else:
         return_action = "resp.json()"
     return return_action
```

### Comparing `polyapi_python-0.2.4.dev1/polyapi/typedefs.py` & `polyapi_python-0.2.4.dev2/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/utils.py` & `polyapi_python-0.2.4.dev2/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/variables.py` & `polyapi_python-0.2.4.dev2/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi/webhook.py` & `polyapi_python-0.2.4.dev2/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.4.dev2/polyapi_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev1
+Version: 0.2.4.dev2
 Summary: The PolyAPI Python Client
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,14 @@
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: jsonschema-gentypes==2.4.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: stdlib_list==0.10.0
 Requires-Dist: colorama==0.4.4
 Requires-Dist: python-socketio[asyncio_client]==5.11.1
 Requires-Dist: truststore==0.8.0
-Requires-Dist: pyjwt==2.3.0
 
 # PolyAPI Python Library
 
 The PolyAPI Python Library lets you use and define PolyAPI functions using Python.
 
 ## PolyAPI Quickstart
```

### Comparing `polyapi_python-0.2.4.dev1/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.4.dev2/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/pyproject.toml` & `polyapi_python-0.2.4.dev2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.4.dev1"
+version = "0.2.4.dev2"
 description = "The PolyAPI Python Client"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
     "stdlib_list==0.10.0",
     "colorama==0.4.4",
     "python-socketio[asyncio_client]==5.11.1",
     "truststore==0.8.0",
-    "pyjwt==2.3.0",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://github.com/polyapi/polyapi-python"
```

### Comparing `polyapi_python-0.2.4.dev1/tests/test_api.py` & `polyapi_python-0.2.4.dev2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/tests/test_auth.py` & `polyapi_python-0.2.4.dev2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/tests/test_function_cli.py` & `polyapi_python-0.2.4.dev2/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/tests/test_server.py` & `polyapi_python-0.2.4.dev2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/tests/test_utils.py` & `polyapi_python-0.2.4.dev2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev1/tests/test_variables.py` & `polyapi_python-0.2.4.dev2/tests/test_variables.py`

 * *Files identical despite different names*

