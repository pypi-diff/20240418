# Comparing `tmp/stac-fastapi.api-2.4.9.tar.gz` & `tmp/stac_fastapi_api-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.api-2.4.9.tar", last modified: Fri Nov 17 14:07:19 2023, max compression
+gzip compressed data, was "stac_fastapi_api-2.5.0.tar", last modified: Wed Apr 17 06:29:45 2024, max compression
```

## Comparing `stac-fastapi.api-2.4.9.tar` & `stac_fastapi_api-2.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:19.855767 stac-fastapi.api-2.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-17 14:07:19.855767 stac-fastapi.api-2.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-17 14:07:19.859767 stac-fastapi.api-2.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:19.851767 stac-fastapi.api-2.4.9/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:19.855767 stac-fastapi.api-2.4.9/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:19.855767 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-17 14:07:19.000000 stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:19.855767 stac-fastapi.api-2.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-11-17 14:07:03.000000 stac-fastapi.api-2.4.9/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 06:29:45.601338 stac_fastapi_api-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.593338 stac_fastapi_api-2.5.0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:29:45.000000 stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:45.597338 stac_fastapi_api-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-17 06:29:24.000000 stac_fastapi_api-2.5.0/tests/test_middleware.py
```

### Comparing `stac-fastapi.api-2.4.9/PKG-INFO` & `stac_fastapi_api-2.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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
 Requires-Dist: brotli_asgi
@@ -23,11 +27,13 @@
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: pystac[validation]==1.*; extra == "dev"
+Provides-Extra: benchmark
+Requires-Dist: pytest-benchmark; extra == "benchmark"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
```

### Comparing `stac-fastapi.api-2.4.9/setup.py` & `stac_fastapi_api-2.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
         "pre-commit",
         "requests",
         "pystac[validation]==1.*",
     ],
+    "benchmark": [
+        "pytest-benchmark",
+    ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
 }
 
 
 setup(
     name="stac-fastapi.api",
     description="An implementation of STAC API based on the FastAPI framework.",
@@ -34,14 +37,18 @@
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

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/app.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fastapi app creation."""
+
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import attr
 from brotli_asgi import BrotliMiddleware
 from fastapi import APIRouter, FastAPI
 from fastapi.openapi.utils import get_openapi
 from fastapi.params import Depends
@@ -79,18 +80,30 @@
                 redoc_url=None,
             ),
             takes_self=True,
         ),
         converter=update_openapi,
     )
     router: APIRouter = attr.ib(default=attr.Factory(APIRouter))
-    title: str = attr.ib(default="stac-fastapi")
-    api_version: str = attr.ib(default="0.1")
+    title: str = attr.ib(
+        default=attr.Factory(
+            lambda self: self.settings.stac_fastapi_title, takes_self=True
+        )
+    )
+    api_version: str = attr.ib(
+        default=attr.Factory(
+            lambda self: self.settings.stac_fastapi_version, takes_self=True
+        )
+    )
     stac_version: str = attr.ib(default=STAC_VERSION)
-    description: str = attr.ib(default="stac-fastapi")
+    description: str = attr.ib(
+        default=attr.Factory(
+            lambda self: self.settings.stac_fastapi_description, takes_self=True
+        )
+    )
     search_get_request_model: Type[BaseSearchGetRequest] = attr.ib(
         default=BaseSearchGetRequest
     )
     search_post_request_model: Type[BaseSearchPostRequest] = attr.ib(
         default=BaseSearchPostRequest
     )
     pagination_extension = attr.ib(default=TokenPaginationExtension)
@@ -128,17 +141,15 @@
             response_model=LandingPage
             if self.settings.enable_response_models
             else None,
             response_class=self.response_class,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.landing_page, EmptyRequest, self.response_class
-            ),
+            endpoint=create_async_endpoint(self.client.landing_page, EmptyRequest),
         )
 
     def register_conformance_classes(self):
         """Register conformance classes (GET /conformance).
 
         Returns:
             None
@@ -149,17 +160,15 @@
             response_model=ConformanceClasses
             if self.settings.enable_response_models
             else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.conformance, EmptyRequest, self.response_class
-            ),
+            endpoint=create_async_endpoint(self.client.conformance, EmptyRequest),
         )
 
     def register_get_item(self):
         """Register get item endpoint (GET /collections/{collection_id}/items/{item_id}).
 
         Returns:
             None
@@ -168,17 +177,15 @@
             name="Get Item",
             path="/collections/{collection_id}/items/{item_id}",
             response_model=Item if self.settings.enable_response_models else None,
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.get_item, ItemUri, GeoJSONResponse
-            ),
+            endpoint=create_async_endpoint(self.client.get_item, ItemUri),
         )
 
     def register_post_search(self):
         """Register search endpoint (POST /search).
 
         Returns:
             None
@@ -191,15 +198,15 @@
             if self.settings.enable_response_models
             else None,
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=create_async_endpoint(
-                self.client.post_search, self.search_post_request_model, GeoJSONResponse
+                self.client.post_search, self.search_post_request_model
             ),
         )
 
     def register_get_search(self):
         """Register search endpoint (GET /search).
 
         Returns:
@@ -213,15 +220,15 @@
             if self.settings.enable_response_models
             else None,
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(
-                self.client.get_search, self.search_get_request_model, GeoJSONResponse
+                self.client.get_search, self.search_get_request_model
             ),
         )
 
     def register_get_collections(self):
         """Register get collections endpoint (GET /collections).
 
         Returns:
@@ -233,17 +240,15 @@
             response_model=Collections
             if self.settings.enable_response_models
             else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.all_collections, EmptyRequest, self.response_class
-            ),
+            endpoint=create_async_endpoint(self.client.all_collections, EmptyRequest),
         )
 
     def register_get_collection(self):
         """Register get collection endpoint (GET /collection/{collection_id}).
 
         Returns:
             None
@@ -252,17 +257,15 @@
             name="Get Collection",
             path="/collections/{collection_id}",
             response_model=Collection if self.settings.enable_response_models else None,
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.get_collection, CollectionUri, self.response_class
-            ),
+            endpoint=create_async_endpoint(self.client.get_collection, CollectionUri),
         )
 
     def register_get_item_collection(self):
         """Register get item collection endpoint (GET /collection/{collection_id}/items).
 
         Returns:
             None
@@ -283,17 +286,15 @@
             response_model=ItemCollection
             if self.settings.enable_response_models
             else None,
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.item_collection, request_model, GeoJSONResponse
-            ),
+            endpoint=create_async_endpoint(self.client.item_collection, request_model),
         )
 
     def register_core(self):
         """Register core STAC endpoints.
 
             GET /
             GET /conformance
```

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/config.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/errors.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/middleware.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/models.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import importlib.util
 from typing import Optional, Type, Union
 
 import attr
 from fastapi import Body, Path
 from pydantic import BaseModel, create_model
 from pydantic.fields import UndefinedType
+from stac_pydantic.shared import BBox
 
 from stac_fastapi.types.extension import ApiExtension
+from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import (
     APIRequest,
     BaseSearchGetRequest,
     BaseSearchPostRequest,
-    str2list,
+    str2bbox,
 )
 
 
 def create_request_model(
     model_name="SearchGetRequest",
     base_model: Union[Type[BaseModel], APIRequest] = BaseSearchGetRequest,
     extensions: Optional[ApiExtension] = None,
@@ -120,16 +122,16 @@
 
 
 @attr.s
 class ItemCollectionUri(CollectionUri):
     """Get item collection."""
 
     limit: int = attr.ib(default=10)
-    bbox: Optional[str] = attr.ib(default=None, converter=str2list)
-    datetime: Optional[str] = attr.ib(default=None)
+    bbox: Optional[BBox] = attr.ib(default=None, converter=str2bbox)
+    datetime: Optional[DateTimeType] = attr.ib(default=None)
 
 
 class POSTTokenPagination(BaseModel):
     """Token pagination model for POST requests."""
 
     token: Optional[str] = None
```

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/openapi.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi/api/routes.py` & `stac_fastapi_api-2.5.0/stac_fastapi/api/routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Route factories."""
+
 import functools
 import inspect
+import warnings
 from typing import Any, Callable, Dict, List, Optional, Type, TypedDict, Union
 
 from fastapi import Depends, params
 from fastapi.dependencies.utils import get_parameterless_sub_dependant
 from pydantic import BaseModel
 from starlette.concurrency import run_in_threadpool
 from starlette.requests import Request
-from starlette.responses import JSONResponse, Response
+from starlette.responses import Response
 from starlette.routing import BaseRoute, Match
 from starlette.status import HTTP_204_NO_CONTENT
 
 from stac_fastapi.api.models import APIRequest
 
 
-def _wrap_response(resp: Any, response_class: Type[Response]) -> Response:
-    if isinstance(resp, Response):
+def _wrap_response(resp: Any) -> Any:
+    if resp is not None:
         return resp
-    elif resp is not None:
-        return response_class(resp)
     else:  # None is returned as 204 No Content
         return Response(status_code=HTTP_204_NO_CONTENT)
 
 
 def sync_to_async(func):
     """Run synchronous function asynchronously in a background thread."""
 
@@ -33,55 +33,56 @@
 
     return run
 
 
 def create_async_endpoint(
     func: Callable,
     request_model: Union[Type[APIRequest], Type[BaseModel], Dict],
-    response_class: Type[Response] = JSONResponse,
+    response_class: Optional[Type[Response]] = None,
 ):
     """Wrap a function in a coroutine which may be used to create a FastAPI endpoint.
 
     Synchronous functions are executed asynchronously using a background thread.
     """
+
+    if response_class:
+        warnings.warns(
+            "`response_class` option is deprecated, please set the Response class directly in the endpoint.",  # noqa: E501
+            DeprecationWarning,
+        )
+
     if not inspect.iscoroutinefunction(func):
         func = sync_to_async(func)
 
     if issubclass(request_model, APIRequest):
 
         async def _endpoint(
             request: Request,
             request_data: request_model = Depends(),  # type:ignore
         ):
             """Endpoint."""
-            return _wrap_response(
-                await func(request=request, **request_data.kwargs()), response_class
-            )
+            return _wrap_response(await func(request=request, **request_data.kwargs()))
 
     elif issubclass(request_model, BaseModel):
 
         async def _endpoint(
             request: Request,
             request_data: request_model,  # type:ignore
         ):
             """Endpoint."""
-            return _wrap_response(
-                await func(request_data, request=request), response_class
-            )
+            return _wrap_response(await func(request_data, request=request))
 
     else:
 
         async def _endpoint(
             request: Request,
             request_data: Dict[str, Any],  # type:ignore
         ):
             """Endpoint."""
-            return _wrap_response(
-                await func(request_data, request=request), response_class
-            )
+            return _wrap_response(await func(request_data, request=request))
 
     return _endpoint
 
 
 class Scope(TypedDict, total=False):
     """More strict version of Starlette's Scope."""
```

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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
 Requires-Dist: brotli_asgi
@@ -23,11 +27,13 @@
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: pystac[validation]==1.*; extra == "dev"
+Provides-Extra: benchmark
+Requires-Dist: pytest-benchmark; extra == "benchmark"
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pdocs; extra == "docs"
```

### Comparing `stac-fastapi.api-2.4.9/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-2.5.0/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.9/tests/test_api.py` & `stac_fastapi_api-2.5.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,28 +57,28 @@
                 response.headers["content-type"]
                 == "application/vnd.oai.openapi+json;version=3.0"
             )
 
     def test_build_api_with_route_dependencies(self):
         routes = [
             {"path": "/collections", "method": "POST"},
-            {"path": "/collections", "method": "PUT"},
+            {"path": "/collections/{collectionId}", "method": "PUT"},
             {"path": "/collections/{collectionId}", "method": "DELETE"},
             {"path": "/collections/{collectionId}/items", "method": "POST"},
             {"path": "/collections/{collectionId}/items/{itemId}", "method": "PUT"},
             {"path": "/collections/{collectionId}/items/{itemId}", "method": "DELETE"},
         ]
         dependencies = [Depends(must_be_bob)]
         api = self._build_api(route_dependencies=[(routes, dependencies)])
         self._assert_dependency_applied(api, routes)
 
     def test_add_route_dependencies_after_building_api(self):
         routes = [
             {"path": "/collections", "method": "POST"},
-            {"path": "/collections", "method": "PUT"},
+            {"path": "/collections/{collectionId}", "method": "PUT"},
             {"path": "/collections/{collectionId}", "method": "DELETE"},
             {"path": "/collections/{collectionId}/items", "method": "POST"},
             {"path": "/collections/{collectionId}/items/{itemId}", "method": "PUT"},
             {"path": "/collections/{collectionId}/items/{itemId}", "method": "DELETE"},
         ]
         api = self._build_api()
         api.add_route_dependencies(scopes=routes, dependencies=[Depends(must_be_bob)])
```

### Comparing `stac-fastapi.api-2.4.9/tests/test_middleware.py` & `stac_fastapi_api-2.5.0/tests/test_middleware.py`

 * *Files identical despite different names*

