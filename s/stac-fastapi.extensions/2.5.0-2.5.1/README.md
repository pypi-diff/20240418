# Comparing `tmp/stac_fastapi_extensions-2.5.0.tar.gz` & `tmp/stac_fastapi_extensions-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_extensions-2.5.0.tar", last modified: Wed Apr 17 06:29:41 2024, max compression
+gzip compressed data, was "stac_fastapi_extensions-2.5.1.tar", last modified: Thu Apr 18 05:52:34 2024, max compression
```

## Comparing `stac_fastapi_extensions-2.5.0.tar` & `stac_fastapi_extensions-2.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.745322 stac_fastapi_extensions-2.5.0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.745322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.172022 stac_fastapi_extensions-2.5.1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.176022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.176022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.176022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.176022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 05:52:34.000000 stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:52:34.180022 stac_fastapi_extensions-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-18 05:52:22.000000 stac_fastapi_extensions-2.5.1/tests/test_transaction.py
```

### Comparing `stac_fastapi_extensions-2.5.0/PKG-INFO` & `stac_fastapi_extensions-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
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

### Comparing `stac_fastapi_extensions-2.5.0/setup.py` & `stac_fastapi_extensions-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/__init__.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/context.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     )
     schema_href: Optional[str] = attr.ib(
         default="https://raw.githubusercontent.com/stac-api-extensions/context/v1.0.0-rc.2/json-schema/schema.json"
     )
 
     def __attrs_post_init__(self):
         """init."""
-        warnings.warm(
+        warnings.warn(
             "The ContextExtension is deprecated and will be removed in 3.0.",
             DeprecationWarning,
             stacklevel=1,
         )
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
```

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/fields.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/fields.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/request.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/filter.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/request.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/filter/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/pagination.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/query.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/query/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/request.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/sort.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/sort/sort.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/transaction.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/core/transaction.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac_fastapi_extensions-2.5.1/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
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

### Comparing `stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac_fastapi_extensions-2.5.1/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.0/tests/test_transaction.py` & `stac_fastapi_extensions-2.5.1/tests/test_transaction.py`

 * *Files identical despite different names*

