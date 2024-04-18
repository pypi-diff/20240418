# Comparing `tmp/entegywrapper-7.2.1.tar.gz` & `tmp/entegywrapper-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entegywrapper-7.2.1.tar", max compression
+gzip compressed data, was "entegywrapper-7.2.2.tar", max compression
```

## Comparing `entegywrapper-7.2.1.tar` & `entegywrapper-7.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2739 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/README.md
--rw-r--r--   0        0        0     8497 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/attendance_tracking/__init__.py
--rw-r--r--   0        0        0     5790 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/attendance_tracking/attendance_tracking.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/content/__init__.py
--rw-r--r--   0        0        0    12219 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/content/categories.py
--rw-r--r--   0        0        0    11413 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/content/content.py
--rw-r--r--   0        0        0     3276 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/content/documents.py
--rw-r--r--   0        0        0     6983 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/content/multi_link.py
--rw-r--r--   0        0        0      716 2024-04-11 08:54:30.181347 entegywrapper-7.2.1/entegywrapper/errors.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/notification/__init__.py
--rw-r--r--   0        0        0     5749 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/notification/notification.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/plugins/__init__.py
--rw-r--r--   0        0        0     1323 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/plugins/ext_auth.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/points/__init__.py
--rw-r--r--   0        0        0     4729 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/points/point_management.py
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/__init__.py
--rw-r--r--   0        0        0     4286 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/profile_custom.py
--rw-r--r--   0        0        0    11869 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/profile_links.py
--rw-r--r--   0        0        0     2354 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/profile_payments.py
--rw-r--r--   0        0        0     6126 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/profile_types.py
--rw-r--r--   0        0        0    16593 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/profiles/profiles.py
--rw-r--r--   0        0        0        1 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/py.typed
--rw-r--r--   0        0        0        0 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/__init__.py
--rw-r--r--   0        0        0      236 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/attendance_tracking.py
--rw-r--r--   0        0        0     6771 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/content.py
--rw-r--r--   0        0        0      286 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/lead_capture.py
--rw-r--r--   0        0        0      334 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/page_settings.py
--rw-r--r--   0        0        0     1260 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/points.py
--rw-r--r--   0        0        0     4717 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/profile.py
--rw-r--r--   0        0        0     2068 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/project.py
--rw-r--r--   0        0        0      329 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/entegywrapper/schemas/schedule.py
--rw-r--r--   0        0        0      920 2024-04-11 08:54:30.185347 entegywrapper-7.2.1/pyproject.toml
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2739 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/README.md
+-rw-r--r--   0        0        0     8479 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/entegywrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/entegywrapper/attendance_tracking/__init__.py
+-rw-r--r--   0        0        0     5790 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/entegywrapper/attendance_tracking/attendance_tracking.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/entegywrapper/content/__init__.py
+-rw-r--r--   0        0        0    12282 2024-04-18 00:31:50.999487 entegywrapper-7.2.2/entegywrapper/content/categories.py
+-rw-r--r--   0        0        0    11413 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/content/content.py
+-rw-r--r--   0        0        0     3276 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/content/documents.py
+-rw-r--r--   0        0        0     6983 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/content/multi_link.py
+-rw-r--r--   0        0        0      716 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/errors.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/notification/__init__.py
+-rw-r--r--   0        0        0     5749 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/notification/notification.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/plugins/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/plugins/ext_auth.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/points/__init__.py
+-rw-r--r--   0        0        0     4729 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/points/point_management.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/__init__.py
+-rw-r--r--   0        0        0     4286 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/profile_custom.py
+-rw-r--r--   0        0        0    11869 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/profile_links.py
+-rw-r--r--   0        0        0     2354 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/profile_payments.py
+-rw-r--r--   0        0        0     6126 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/profile_types.py
+-rw-r--r--   0        0        0    16614 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/profiles/profiles.py
+-rw-r--r--   0        0        0        1 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/py.typed
+-rw-r--r--   0        0        0        0 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/__init__.py
+-rw-r--r--   0        0        0      236 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/attendance_tracking.py
+-rw-r--r--   0        0        0     6771 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/content.py
+-rw-r--r--   0        0        0      286 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/lead_capture.py
+-rw-r--r--   0        0        0      334 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/page_settings.py
+-rw-r--r--   0        0        0     1260 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/points.py
+-rw-r--r--   0        0        0     4717 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/profile.py
+-rw-r--r--   0        0        0     2068 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/project.py
+-rw-r--r--   0        0        0      329 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/entegywrapper/schemas/schedule.py
+-rw-r--r--   0        0        0      920 2024-04-18 00:31:51.003486 entegywrapper-7.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 entegywrapper-7.2.2/PKG-INFO
```

### Comparing `entegywrapper-7.2.1/README.md` & `entegywrapper-7.2.2/README.md`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/__init__.py` & `entegywrapper-7.2.2/entegywrapper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import os
 import sys
 import time
 from enum import Enum
 from json import JSONEncoder
-from typing import Any, Callable
+from typing import Callable
 
 import requests
 from requests.structures import CaseInsensitiveDict
 
-from entegywrapper.errors import EntegyInvalidAPIKeyError, EntegyNoDataError
+from .errors import EntegyInvalidAPIKeyError, EntegyNoDataError
 
 sys.path.append(os.path.dirname(__file__))
 
 API_ENDPOINTS = {
     "AU": "https://api.entegy.com.au",
     "US": "https://api-us.entegy.com.au",
     "EU": "https://api-eu.entegy.com.au",
```

### Comparing `entegywrapper-7.2.1/entegywrapper/attendance_tracking/attendance_tracking.py` & `entegywrapper-7.2.2/entegywrapper/attendance_tracking/attendance_tracking.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/content/categories.py` & `entegywrapper-7.2.2/entegywrapper/content/categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,18 @@
 
         `EntegyFailedRequestError`: if the API request fails
 
     Returns
     -------
         `bool`: whether the categories were deselected successfully
     """
-    data = {"templateType": template_type, "categories": categories}
+    data = {
+        "templateType": template_type,
+        "categories": [category.model_dump() for category in categories],
+    }
 
     if module_id is not None:
         data["moduleId"] = module_id
     elif external_reference is not None:
         data["externalReference"] = external_reference
     else:
         raise ValueError("Please specify an identifier")
```

### Comparing `entegywrapper-7.2.1/entegywrapper/content/content.py` & `entegywrapper-7.2.2/entegywrapper/content/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/content/documents.py` & `entegywrapper-7.2.2/entegywrapper/content/documents.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/content/multi_link.py` & `entegywrapper-7.2.2/entegywrapper/content/multi_link.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/errors.py` & `entegywrapper-7.2.2/entegywrapper/errors.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/notification/notification.py` & `entegywrapper-7.2.2/entegywrapper/notification/notification.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/plugins/ext_auth.py` & `entegywrapper-7.2.2/entegywrapper/plugins/ext_auth.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/points/point_management.py` & `entegywrapper-7.2.2/entegywrapper/points/point_management.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/profiles/profile_custom.py` & `entegywrapper-7.2.2/entegywrapper/profiles/profile_custom.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/profiles/profile_links.py` & `entegywrapper-7.2.2/entegywrapper/profiles/profile_links.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/profiles/profile_payments.py` & `entegywrapper-7.2.2/entegywrapper/profiles/profile_payments.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/profiles/profile_types.py` & `entegywrapper-7.2.2/entegywrapper/profiles/profile_types.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/profiles/profiles.py` & `entegywrapper-7.2.2/entegywrapper/profiles/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Generator, Optional
+from typing import TYPE_CHECKING, Any, Generator, Optional
 
 from entegywrapper.errors import EntegyFailedRequestError, EntegyServerError
 from entegywrapper.schemas.profile import (
     Profile,
     ProfileCreate,
     ProfileIdentifier,
     ProfileType,
@@ -49,15 +49,15 @@
 
         `created_after` (`str`, optional): only select profiles created after this time; defaults to `None`
 
     Yields
     ------
         `Generator[Profile, None, None]`: user profiles
     """
-    data = {
+    data: dict[str, Any] = {
         "pagination": {"start": 0, "limit": 1000},
         "includeCustomFields": include_custom_fields,
         "includePermissions": include_permissions,
     }
 
     if status is not None:
         data["status"] = status
```

### Comparing `entegywrapper-7.2.1/entegywrapper/schemas/content.py` & `entegywrapper-7.2.2/entegywrapper/schemas/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/schemas/points.py` & `entegywrapper-7.2.2/entegywrapper/schemas/points.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/schemas/profile.py` & `entegywrapper-7.2.2/entegywrapper/schemas/profile.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/entegywrapper/schemas/project.py` & `entegywrapper-7.2.2/entegywrapper/schemas/project.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.2.1/pyproject.toml` & `entegywrapper-7.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0a5"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "entegywrapper"
-version = "7.2.1"
+version = "7.2.2"
 requires-python = ">=3.10"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "entegywrapper"
-version = "7.2.1"
+version = "7.2.2"
 description = "Python SDK for the Entegy API"
 authors = [
     "Situ Development <developer@situ.com.au>",
     "William Sawyer <william@situ.com.au>",
     "Nathan Thomas <nathan@situ.com.au>",
 ]
 readme = "README.md"
```

### Comparing `entegywrapper-7.2.1/PKG-INFO` & `entegywrapper-7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entegywrapper
-Version: 7.2.1
+Version: 7.2.2
 Summary: Python SDK for the Entegy API
 Home-page: https://github.com/SituDevelopment/entegy-sdk-python
 Author: Situ Development
 Author-email: developer@situ.com.au
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

