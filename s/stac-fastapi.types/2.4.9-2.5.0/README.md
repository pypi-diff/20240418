# Comparing `tmp/stac-fastapi.types-2.4.9.tar.gz` & `tmp/stac_fastapi_types-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.types-2.4.9.tar", last modified: Fri Nov 17 14:07:12 2023, max compression
+gzip compressed data, was "stac_fastapi_types-2.5.0.tar", last modified: Wed Apr 17 06:29:37 2024, max compression
```

## Comparing `stac-fastapi.types-2.4.9.tar` & `stac_fastapi_types-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:12.643719 stac-fastapi.types-2.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-17 14:07:12.643719 stac-fastapi.types-2.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-17 14:07:12.643719 stac-fastapi.types-2.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:12.639719 stac-fastapi.types-2.4.9/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:12.643719 stac-fastapi.types-2.4.9/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    24029 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:12.639719 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-17 14:07:12.000000 stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:07:12.643719 stac-fastapi.types-2.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/tests/test_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2023-11-17 14:07:03.000000 stac-fastapi.types-2.4.9/tests/test_rfc3339.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:37.833306 stac_fastapi_types-2.5.0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:29:37.000000 stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:29:37.837306 stac_fastapi_types-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/tests/test_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-17 06:29:24.000000 stac_fastapi_types-2.5.0/tests/test_rfc3339.py
```

### Comparing `stac-fastapi.types-2.4.9/PKG-INFO` & `stac_fastapi_types-2.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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
 Requires-Dist: fastapi>=0.73.0
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/config.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,19 @@
             as distinct columns in the database.
     """
 
     # TODO: Remove `default_includes` attribute so we can use
     # `pydantic.BaseSettings` instead
     default_includes: Optional[Set[str]] = None
 
+    stac_fastapi_title: str = "stac-fastapi"
+    stac_fastapi_description: str = "stac-fastapi"
+    stac_fastapi_version: str = "0.1"
+    stac_fastapi_landing_id: str = "stac-fastapi"
+
     app_host: str = "0.0.0.0"
     app_port: int = 8000
     reload: bool = True
     enable_response_models: bool = False
 
     openapi_url: str = "/api"
     docs_url: str = "/api.html"
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/conformance.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/core.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Base clients."""
+
 import abc
-from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 from urllib.parse import urljoin
 
 import attr
 from fastapi import Request
 from stac_pydantic.links import Relations
-from stac_pydantic.shared import MimeTypes
+from stac_pydantic.shared import BBox, MimeTypes
 from stac_pydantic.version import STAC_VERSION
 from starlette.responses import Response
 
 from stac_fastapi.types import stac as stac_types
+from stac_fastapi.types.config import ApiSettings
 from stac_fastapi.types.conformance import BASE_CONFORMANCE_CLASSES
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.requests import get_base_url
+from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import BaseSearchPostRequest
 from stac_fastapi.types.stac import Conformance
 
 NumType = Union[float, int]
 StacType = Dict[str, Any]
 
+api_settings = ApiSettings()
+
 
 @attr.s  # type:ignore
 class BaseTransactionsClient(abc.ABC):
     """Defines a pattern for implementing the STAC API Transaction Extension."""
 
     @abc.abstractmethod
     def create_item(
@@ -97,26 +101,26 @@
         Returns:
             The collection that was created.
         """
         ...
 
     @abc.abstractmethod
     def update_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection_id: str, collection: stac_types.Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
-        Called with `PUT /collections`. It is expected that this item already
-        exists.  The update should do a diff against the saved collection and
+        Called with `PUT /collections/{collection_id}`. It is expected that this item
+        already exists.  The update should do a diff against the saved collection and
         perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
 
         Args:
-            collection: the collection (must be complete)
-            collection_id: the id of the collection from the resource path
+            collection_id: id of the existing collection to be updated
+            collection: the updated collection (must be complete)
 
         Returns:
             The updated collection.
         """
         ...
 
     @abc.abstractmethod
@@ -210,25 +214,26 @@
         Returns:
             The collection that was created.
         """
         ...
 
     @abc.abstractmethod
     async def update_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection_id: str, collection: stac_types.Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
-        Called with `PUT /collections`. It is expected that this item already
-        exists.  The update should do a diff against the saved collection and
+        Called with `PUT /collections/{collection_id}`. It is expected that this item
+        already exists.  The update should do a diff against the saved collection and
         perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
 
         Args:
-            collection: the collection (must be complete)
+            collection_id: id of the existing collection to be updated
+            collection: the updated collection (must be complete)
 
         Returns:
             The updated collection.
         """
         ...
 
     @abc.abstractmethod
@@ -249,17 +254,17 @@
 
 
 @attr.s
 class LandingPageMixin(abc.ABC):
     """Create a STAC landing page (GET /)."""
 
     stac_version: str = attr.ib(default=STAC_VERSION)
-    landing_page_id: str = attr.ib(default="stac-fastapi")
-    title: str = attr.ib(default="stac-fastapi")
-    description: str = attr.ib(default="stac-fastapi")
+    landing_page_id: str = attr.ib(default=api_settings.stac_fastapi_landing_id)
+    title: str = attr.ib(default=api_settings.stac_fastapi_title)
+    description: str = attr.ib(default=api_settings.stac_fastapi_description)
 
     def _landing_page(
         self,
         base_url: str,
         conformance_classes: List[str],
         extension_schemas: List[str],
     ) -> stac_types.LandingPage:
@@ -285,15 +290,15 @@
                     "rel": "data",
                     "type": MimeTypes.json,
                     "href": urljoin(base_url, "collections"),
                 },
                 {
                     "rel": Relations.conformance.value,
                     "type": MimeTypes.json,
-                    "title": "STAC/WFS3 conformance classes implemented by this server",
+                    "title": "STAC/OGC conformance classes implemented by this server",
                     "href": urljoin(base_url, "conformance"),
                 },
                 {
                     "rel": Relations.search.value,
                     "type": MimeTypes.geojson,
                     "title": "STAC search",
                     "href": urljoin(base_url, "search"),
@@ -363,14 +368,28 @@
         base_url = get_base_url(request)
         landing_page = self._landing_page(
             base_url=base_url,
             conformance_classes=self.conformance_classes(),
             extension_schemas=[],
         )
 
+        # Add Queryables link
+        if self.extension_is_enabled("FilterExtension"):
+            landing_page["links"].append(
+                {
+                    # TODO: replace this with Relations.queryables.value,
+                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/queryables",
+                    # TODO: replace this with MimeTypes.jsonschema,
+                    "type": "application/schema+json",
+                    "title": "Queryables",
+                    "href": urljoin(base_url, "queryables"),
+                    "method": "GET",
+                }
+            )
+
         # Add Collections links
         collections = self.all_collections(request=kwargs["request"])
         for collection in collections["collections"]:
             landing_page["links"].append(
                 {
                     "rel": Relations.child.value,
                     "type": MimeTypes.json.value,
@@ -432,16 +451,16 @@
         ...
 
     @abc.abstractmethod
     def get_search(
         self,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = 10,
         query: Optional[str] = None,
         token: Optional[str] = None,
         fields: Optional[List[str]] = None,
         sortby: Optional[str] = None,
         intersects: Optional[str] = None,
         **kwargs,
@@ -495,16 +514,16 @@
         """
         ...
 
     @abc.abstractmethod
     def item_collection(
         self,
         collection_id: str,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: int = 10,
         token: str = None,
         **kwargs,
     ) -> stac_types.ItemCollection:
         """Get all items from a specific collection.
 
         Called with `GET /collections/{collection_id}/items`
@@ -560,14 +579,30 @@
         request: Request = kwargs["request"]
         base_url = get_base_url(request)
         landing_page = self._landing_page(
             base_url=base_url,
             conformance_classes=self.conformance_classes(),
             extension_schemas=[],
         )
+
+        # Add Queryables link
+        if self.extension_is_enabled("FilterExtension"):
+            landing_page["links"].append(
+                {
+                    # TODO: replace this with Relations.queryables.value,
+                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/queryables",
+                    # TODO: replace this with MimeTypes.jsonschema,
+                    "type": "application/schema+json",
+                    "title": "Queryables",
+                    "href": urljoin(base_url, "queryables"),
+                    "method": "GET",
+                }
+            )
+
+        # Add Collections links
         collections = await self.all_collections(request=kwargs["request"])
         for collection in collections["collections"]:
             landing_page["links"].append(
                 {
                     "rel": Relations.child.value,
                     "type": MimeTypes.json.value,
                     "title": collection.get("title") or collection.get("id"),
@@ -577,29 +612,25 @@
 
         # Add OpenAPI URL
         landing_page["links"].append(
             {
                 "rel": "service-desc",
                 "type": "application/vnd.oai.openapi+json;version=3.0",
                 "title": "OpenAPI service description",
-                "href": urljoin(
-                    str(request.base_url), request.app.openapi_url.lstrip("/")
-                ),
+                "href": urljoin(base_url, request.app.openapi_url.lstrip("/")),
             }
         )
 
         # Add human readable service-doc
         landing_page["links"].append(
             {
                 "rel": "service-doc",
                 "type": "text/html",
                 "title": "OpenAPI service documentation",
-                "href": urljoin(
-                    str(request.base_url), request.app.docs_url.lstrip("/")
-                ),
+                "href": urljoin(base_url, request.app.docs_url.lstrip("/")),
             }
         )
 
         return landing_page
 
     async def conformance(self, **kwargs) -> stac_types.Conformance:
         """Conformance classes.
@@ -628,16 +659,16 @@
         ...
 
     @abc.abstractmethod
     async def get_search(
         self,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = 10,
         query: Optional[str] = None,
         token: Optional[str] = None,
         fields: Optional[List[str]] = None,
         sortby: Optional[str] = None,
         intersects: Optional[str] = None,
         **kwargs,
@@ -695,16 +726,16 @@
         """
         ...
 
     @abc.abstractmethod
     async def item_collection(
         self,
         collection_id: str,
-        bbox: Optional[List[NumType]] = None,
-        datetime: Optional[Union[str, datetime]] = None,
+        bbox: Optional[BBox] = None,
+        datetime: Optional[DateTimeType] = None,
         limit: int = 10,
         token: str = None,
         **kwargs,
     ) -> stac_types.ItemCollection:
         """Get all items from a specific collection.
 
         Called with `GET /collections/{collection_id}/items`
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/errors.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/extension.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/links.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import attr
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import MimeTypes
 
 # These can be inferred from the item/collection so they aren't included in the database
 # Instead they are dynamically generated when querying the database using the
 # classes defined below
-INFERRED_LINK_RELS = ["self", "item", "parent", "collection", "root"]
+INFERRED_LINK_RELS = ["self", "item", "parent", "collection", "root", "items"]
 
 
 def filter_links(links: List[Dict]) -> List[Dict]:
     """Remove inferred links."""
     return [link for link in links if link["rel"] not in INFERRED_LINK_RELS]
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/rfc3339.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/rfc3339.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """rfc3339."""
 import re
 from datetime import datetime, timezone
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import iso8601
 from pystac.utils import datetime_to_str
 
 RFC33339_PATTERN = (
     r"^(\d\d\d\d)\-(\d\d)\-(\d\d)(T|t)(\d\d):(\d\d):(\d\d)([.]\d+)?"
     r"(Z|([-+])(\d\d):(\d\d))$"
 )
 
+DateTimeType = Union[
+    datetime,
+    Tuple[datetime, datetime],
+    Tuple[datetime, None],
+    Tuple[None, datetime],
+]
+
 
 def rfc3339_str_to_datetime(s: str) -> datetime:
     """Convert a string conforming to RFC 3339 to a :class:`datetime.datetime`.
 
     Uses :meth:`iso8601.parse_date` under the hood.
 
     Args:
@@ -36,15 +43,15 @@
 
     # Parse with pyiso8601
     return iso8601.parse_date(s)
 
 
 def str_to_interval(
     interval: str,
-) -> Optional[Tuple[Optional[datetime], Optional[datetime]]]:
+) -> Optional[DateTimeType]:
     """Extract a tuple of datetimes from an interval string.
 
     Interval strings are defined by
     OGC API - Features Part 1 for the datetime query parameter value. These follow the
     form '1985-04-12T23:20:50.52Z/1986-04-12T23:20:50.52Z', and allow either the start
     or end (but not both) to be open-ended with '..' or ''.
 
@@ -55,15 +62,18 @@
     Raises:
         ValueError: If the string is not a valid interval string.
     """
     if not interval:
         raise ValueError("Empty interval string is invalid.")
 
     values = interval.split("/")
-    if len(values) != 2:
+    if len(values) == 1:
+        # Single date for == date case
+        return rfc3339_str_to_datetime(values[0])
+    elif len(values) > 2:
         raise ValueError(
             f"Interval string '{interval}' contains more than one forward slash."
         )
 
     start = None
     end = None
     if values[0] not in ["..", ""]:
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/search.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from datetime import datetime
 from enum import auto
 from types import DynamicClassAttribute
 from typing import Any, Callable, Dict, Generator, List, Optional, Union
 
 import attr
 from geojson_pydantic.geometries import (
+    GeometryCollection,
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
     _GeometryBase,
 )
-from pydantic import BaseModel, ConstrainedInt, validator
+from pydantic import BaseModel, ConstrainedInt, Field, validator
 from pydantic.errors import NumberNotGtError
 from pydantic.validators import int_validator
 from stac_pydantic.shared import BBox
 from stac_pydantic.utils import AutoValueEnum
 
-from stac_fastapi.types.rfc3339 import rfc3339_str_to_datetime, str_to_interval
+from stac_fastapi.types.rfc3339 import DateTimeType, str_to_interval
 
 # Be careful: https://github.com/samuelcolvin/pydantic/issues/1423#issuecomment-642797287
 NumType = Union[float, int]
 
 
 class Limit(ConstrainedInt):
     """An positive integer that maxes out at 10,000."""
@@ -78,14 +79,22 @@
 
 def str2list(x: str) -> Optional[List]:
     """Convert string to list base on , delimiter."""
     if x:
         return x.split(",")
 
 
+def str2bbox(x: str) -> Optional[BBox]:
+    """Convert string to BBox based on , delimiter."""
+    if x:
+        t = tuple(float(v) for v in str2list(x))
+        assert len(t) == 4
+        return t
+
+
 @attr.s  # type:ignore
 class APIRequest(abc.ABC):
     """Generic API Request base class."""
 
     def kwargs(self) -> Dict:
         """Transform api request params into format which matches the signature of the
         endpoint."""
@@ -94,17 +103,17 @@
 
 @attr.s
 class BaseSearchGetRequest(APIRequest):
     """Base arguments for GET Request."""
 
     collections: Optional[str] = attr.ib(default=None, converter=str2list)
     ids: Optional[str] = attr.ib(default=None, converter=str2list)
-    bbox: Optional[str] = attr.ib(default=None, converter=str2list)
-    intersects: Optional[str] = attr.ib(default=None)
-    datetime: Optional[str] = attr.ib(default=None)
+    bbox: Optional[BBox] = attr.ib(default=None, converter=str2bbox)
+    intersects: Optional[str] = attr.ib(default=None, converter=str2list)
+    datetime: Optional[DateTimeType] = attr.ib(default=None, converter=str_to_interval)
     limit: Optional[int] = attr.ib(default=10)
 
 
 class BaseSearchPostRequest(BaseModel):
     """Search model.
 
     Replace base model in STAC-pydantic as it includes additional fields, not in the core
@@ -115,42 +124,50 @@
     https://github.com/stac-utils/stac-pydantic/pull/100
     """
 
     collections: Optional[List[str]]
     ids: Optional[List[str]]
     bbox: Optional[BBox]
     intersects: Optional[
-        Union[Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon]
+        Union[
+            Point,
+            MultiPoint,
+            LineString,
+            MultiLineString,
+            Polygon,
+            MultiPolygon,
+            GeometryCollection,
+        ]
     ]
-    datetime: Optional[str]
-    limit: Optional[Limit] = 10
+    datetime: Optional[DateTimeType]
+    limit: Optional[Limit] = Field(default=10)
 
     @property
     def start_date(self) -> Optional[datetime]:
         """Extract the start date from the datetime string."""
-        interval = str_to_interval(self.datetime)
-        return interval[0] if interval else None
+        return self.datetime[0] if self.datetime else None
 
     @property
     def end_date(self) -> Optional[datetime]:
         """Extract the end date from the datetime string."""
-        interval = str_to_interval(self.datetime)
-        return interval[1] if interval else None
+        return self.datetime[1] if self.datetime else None
 
     @validator("intersects")
     def validate_spatial(cls, v, values):
         """Check bbox and intersects are not both supplied."""
         if v and values["bbox"]:
             raise ValueError("intersects and bbox parameters are mutually exclusive")
         return v
 
-    @validator("bbox")
-    def validate_bbox(cls, v: BBox):
+    @validator("bbox", pre=True)
+    def validate_bbox(cls, v: Union[str, BBox]) -> BBox:
         """Check order of supplied bbox coordinates."""
         if v:
+            if type(v) == str:
+                v = str2bbox(v)
             # Validate order
             if len(v) == 4:
                 xmin, ymin, xmax, ymax = v
             else:
                 xmin, ymin, min_elev, xmax, ymax, max_elev = v
                 if max_elev < min_elev:
                     raise ValueError(
@@ -169,42 +186,19 @@
 
             # Validate against WGS84
             if xmin < -180 or ymin < -90 or xmax > 180 or ymax > 90:
                 raise ValueError("Bounding box must be within (-180, -90, 180, 90)")
 
         return v
 
-    @validator("datetime")
-    def validate_datetime(cls, v):
-        """Validate datetime."""
-        if "/" in v:
-            values = v.split("/")
-        else:
-            # Single date is interpreted as end date
-            values = ["..", v]
-
-        dates = []
-        for value in values:
-            if value == ".." or value == "":
-                dates.append("..")
-                continue
-
-            # throws ValueError if invalid RFC 3339 string
-            dates.append(rfc3339_str_to_datetime(value))
-
-        if dates[0] == ".." and dates[1] == "..":
-            raise ValueError(
-                "Invalid datetime range, both ends of range may not be open"
-            )
-
-        if ".." not in dates and dates[0] > dates[1]:
-            raise ValueError(
-                "Invalid datetime range, must match format (begin_date, end_date)"
-            )
-
+    @validator("datetime", pre=True)
+    def validate_datetime(cls, v: Union[str, DateTimeType]) -> DateTimeType:
+        """Parse datetime."""
+        if type(v) == str:
+            v = str_to_interval(v)
         return v
 
     @property
     def spatial_filter(self) -> Optional[_GeometryBase]:
         """Return a geojson-pydantic object representing the spatial filter for the search
         request.
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi/types/stac.py` & `stac_fastapi_types-2.5.0/stac_fastapi/types/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """STAC types."""
 import sys
 from typing import Any, Dict, List, Literal, Optional, Union
 
+from stac_pydantic.shared import BBox
+
 # Avoids a Pydantic error:
 # TypeError: You should use `typing_extensions.TypedDict` instead of
 # `typing.TypedDict` with Python < 3.9.2.  Without it, there is no way to
 # differentiate required and optional fields when subclassed.
 if sys.version_info < (3, 9, 2):
     from typing_extensions import TypedDict
 else:
@@ -60,15 +62,15 @@
     """STAC Item."""
 
     type: Literal["Feature"]
     stac_version: str
     stac_extensions: Optional[List[str]]
     id: str
     geometry: Dict[str, Any]
-    bbox: List[NumType]
+    bbox: BBox
     properties: Dict[str, Any]
     links: List[Dict[str, Any]]
     assets: Dict[str, Any]
     collection: str
 
 
 class ItemCollection(TypedDict, total=False):
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/PKG-INFO` & `stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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
 Requires-Dist: fastapi>=0.73.0
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
```

### Comparing `stac-fastapi.types-2.4.9/stac_fastapi.types.egg-info/SOURCES.txt` & `stac_fastapi_types-2.5.0/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.9/tests/test_limit.py` & `stac_fastapi_types-2.5.0/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.9/tests/test_rfc3339.py` & `stac_fastapi_types-2.5.0/tests/test_rfc3339.py`

 * *Files identical despite different names*

