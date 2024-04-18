# Comparing `tmp/stac_fastapi_api-2.5.0.tar.gz` & `tmp/stac_fastapi_api-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_api-2.5.0.tar", last modified: Wed Apr 17 06:29:45 2024, max compression
+gzip compressed data, was "stac_fastapi_api-2.5.1.tar", last modified: Thu Apr 18 05:52:37 2024, max compression
```

## Comparing `stac_fastapi_api-2.5.0.tar` & `stac_fastapi_api-2.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 06:29:45.601338 stac_fastapi_api-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.593338 stac_fastapi_api-2.5.0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:37.420040 stac_fastapi_api-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-18 05:52:37.420040 stac_fastapi_api-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 05:52:37.420040 stac_fastapi_api-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:37.416041 stac_fastapi_api-2.5.1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:37.416041 stac_fastapi_api-2.5.1/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:37.420040 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 05:52:37.000000 stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:37.416041 stac_fastapi_api-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-18 05:52:22.000000 stac_fastapi_api-2.5.1/tests/test_middleware.py
```

### Comparing `stac_fastapi_api-2.5.0/PKG-INFO` & `stac_fastapi_api-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.5.0
+Version: 2.5.1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-2.5.0/setup.py` & `stac_fastapi_api-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/app.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/config.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/errors.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/middleware.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/models.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/openapi.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi/api/routes.py` & `stac_fastapi_api-2.5.1/stac_fastapi/api/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ):
     """Wrap a function in a coroutine which may be used to create a FastAPI endpoint.
 
     Synchronous functions are executed asynchronously using a background thread.
     """
 
     if response_class:
-        warnings.warns(
+        warnings.warn(
             "`response_class` option is deprecated, please set the Response class directly in the endpoint.",  # noqa: E501
             DeprecationWarning,
         )
 
     if not inspect.iscoroutinefunction(func):
         func = sync_to_async(func)
```

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.5.0
+Version: 2.5.1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-2.5.1/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/tests/test_api.py` & `stac_fastapi_api-2.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.0/tests/test_middleware.py` & `stac_fastapi_api-2.5.1/tests/test_middleware.py`

 * *Files identical despite different names*

