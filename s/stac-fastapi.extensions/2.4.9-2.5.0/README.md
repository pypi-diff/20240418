# Comparing `tmp/stac-fastapi.extensions-2.4.9.tar.gz` & `tmp/stac_fastapi_extensions-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.extensions-2.4.9.tar", last modified: Fri Nov 17 14:07:16 2023, max compression
+gzip compressed data, was "stac_fastapi_extensions-2.5.0.tar", last modified: Wed Apr 17 06:29:41 2024, max compression
```

## Comparing `stac-fastapi.extensions-2.4.9.tar` & `stac_fastapi_extensions-2.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.167742 stac-fastapi.extensions-2.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-17 14:07:16.167742 stac-fastapi.extensions-2.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-17 14:07:16.167742 stac-fastapi.extensions-2.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.159742 stac-fastapi.extensions-2.4.9/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.159742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.159742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.159742 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-17 14:07:16.000000 stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:16.163742 stac-fastapi.extensions-2.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-11-17 14:07:03.000000 stac-fastapi.extensions-2.4.9/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-17 06:29:41.753322 stac_fastapi_extensions-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.745322 stac_fastapi_extensions-2.5.0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.745322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:29:41.000000 stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:41.749322 stac_fastapi_extensions-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-17 06:29:24.000000 stac_fastapi_extensions-2.5.0/tests/test_transaction.py
```

### Comparing `stac-fastapi.extensions-2.4.9/PKG-INFO` & `stac_fastapi_extensions-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.9
+Version: 2.5.0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
 Requires-Dist: stac-fastapi.types
```

### Comparing `stac-fastapi.extensions-2.4.9/setup.py` & `stac_fastapi_extensions-2.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     keywords="STAC FastAPI COG",
     author="Arturo Engineering",
     author_email="engineering@arturo.ai",
     url="https://github.com/stac-utils/stac-fastapi",
     license="MIT",
```

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/__init__.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/context.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Context extension."""
+
+import warnings
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
 
@@ -20,14 +22,22 @@
     conformance_classes: List[str] = attr.ib(
         factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.2/item-search#context"]
     )
     schema_href: Optional[str] = attr.ib(
         default="https://raw.githubusercontent.com/stac-api-extensions/context/v1.0.0-rc.2/json-schema/schema.json"
     )
 
+    def __attrs_post_init__(self):
+        """init."""
+        warnings.warm(
+            "The ContextExtension is deprecated and will be removed in 3.0.",
+            DeprecationWarning,
+            stacklevel=1,
+        )
+
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
             app: target FastAPI application.
 
         Returns:
```

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/fields.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/fields.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/fields/request.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/filter.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/filter/request.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/filter/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/pagination.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/query/query.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/query/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/request.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/sort/sort.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/sort/sort.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/core/transaction.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/core/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Transaction extension."""
+
 from typing import List, Optional, Type, Union
 
 import attr
 from fastapi import APIRouter, Body, FastAPI
 from stac_pydantic import Collection, Item
 from starlette.responses import JSONResponse, Response
 
@@ -113,18 +114,18 @@
             methods=["POST"],
             endpoint=create_async_endpoint(
                 self.client.create_collection, stac_types.Collection
             ),
         )
 
     def register_update_collection(self):
-        """Register update collection endpoint (PUT /collections)."""
+        """Register update collection endpoint (PUT /collections/{collection_id})."""
         self.router.add_api_route(
             name="Update Collection",
-            path="/collections",
+            path="/collections/{collection_id}",
             response_model=Collection if self.settings.enable_response_models else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["PUT"],
             endpoint=create_async_endpoint(
                 self.client.update_collection, stac_types.Collection
```

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac_fastapi_extensions-2.5.0/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.9
+Version: 2.5.0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
 Requires-Dist: stac-fastapi.types
```

### Comparing `stac-fastapi.extensions-2.4.9/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac_fastapi_extensions-2.5.0/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.9/tests/test_transaction.py` & `stac_fastapi_extensions-2.5.0/tests/test_transaction.py`

 * *Files identical despite different names*

