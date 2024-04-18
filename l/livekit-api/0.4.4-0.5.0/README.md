# Comparing `tmp/livekit-api-0.4.4.tar.gz` & `tmp/livekit_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-api-0.4.4.tar", last modified: Fri Apr  5 00:30:50 2024, max compression
+gzip compressed data, was "livekit_api-0.5.0.tar", last modified: Thu Apr 18 18:12:19 2024, max compression
```

## Comparing `livekit-api-0.4.4.tar` & `livekit_api-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-05 00:30:50.982386 livekit-api-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 00:30:38.000000 livekit-api-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.978386 livekit-api-0.4.4/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/livekit/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/egress_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/ingress_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/livekit_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/room_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/twirp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 00:30:38.000000 livekit-api-0.4.4/livekit/api/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/livekit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 00:30:50.000000 livekit-api-0.4.4/livekit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 00:30:38.000000 livekit-api-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:30:50.982386 livekit-api-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-05 00:30:38.000000 livekit-api-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:30:50.982386 livekit-api-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-05 00:30:38.000000 livekit-api-0.4.4/tests/test_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-05 00:30:38.000000 livekit-api-0.4.4/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:19.347726 livekit_api-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 18:12:19.347726 livekit_api-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 18:12:06.000000 livekit_api-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:19.343726 livekit_api-0.5.0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:19.347726 livekit_api-0.5.0/livekit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/egress_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/ingress_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/livekit_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/room_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/sip_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/twirp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-18 18:12:06.000000 livekit_api-0.5.0/livekit/api/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:19.347726 livekit_api-0.5.0/livekit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 18:12:19.000000 livekit_api-0.5.0/livekit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-18 18:12:19.000000 livekit_api-0.5.0/livekit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:12:19.000000 livekit_api-0.5.0/livekit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 18:12:19.000000 livekit_api-0.5.0/livekit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 18:12:19.000000 livekit_api-0.5.0/livekit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 18:12:06.000000 livekit_api-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:12:19.347726 livekit_api-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-18 18:12:06.000000 livekit_api-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:19.347726 livekit_api-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-18 18:12:06.000000 livekit_api-0.5.0/tests/test_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-18 18:12:06.000000 livekit_api-0.5.0/tests/test_webhook.py
```

### Comparing `livekit-api-0.4.4/PKG-INFO` & `livekit_api-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-api
-Version: 0.4.4
+Version: 0.5.0
 Summary: Python Server API for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,18 +15,18 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: pyjwt>=2.0.0
 Requires-Dist: aiohttp>=3.9.0
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
-Requires-Dist: livekit-protocol<1,>=0.3.0
+Requires-Dist: livekit-protocol<1,>=0.5.0
 
 # LiveKit Server APIs
 
 Access LiveKit server APIs and generate access tokens.
```

### Comparing `livekit-api-0.4.4/livekit/api/__init__.py` & `livekit_api-0.5.0/livekit/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 # flake8: noqa
 # re-export packages from protocol
 from livekit.protocol.egress import *
 from livekit.protocol.ingress import *
 from livekit.protocol.models import *
 from livekit.protocol.room import *
 from livekit.protocol.webhook import *
+from livekit.protocol.sip import *
 
 from .twirp_client import TwirpError, TwirpErrorCode
 from .livekit_api import LiveKitAPI
 from .access_token import VideoGrants, AccessToken, TokenVerifier
 from .webhook import WebhookReceiver
 from .version import __version__
```

### Comparing `livekit-api-0.4.4/livekit/api/_service.py` & `livekit_api-0.5.0/livekit/api/_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/access_token.py` & `livekit_api-0.5.0/livekit/api/access_token.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/egress_service.py` & `livekit_api-0.5.0/livekit/api/egress_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/ingress_service.py` & `livekit_api-0.5.0/livekit/api/ingress_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/livekit_api.py` & `livekit_api-0.5.0/livekit/api/livekit_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import aiohttp
 import os
 from .room_service import RoomService
 from .egress_service import EgressService
 from .ingress_service import IngressService
+from .sip_service import SipService
 from typing import Optional
 
 
 class LiveKitAPI:
     def __init__(
         self,
         url: Optional[str] = None,
@@ -25,22 +26,27 @@
         if not api_key or not api_secret:
             raise ValueError("api_key and api_secret must be set")
 
         self._session = aiohttp.ClientSession(timeout=timeout)
         self._room = RoomService(self._session, url, api_key, api_secret)
         self._ingress = IngressService(self._session, url, api_key, api_secret)
         self._egress = EgressService(self._session, url, api_key, api_secret)
+        self._sip = SipService(self._session, url, api_key, api_secret)
 
     @property
     def room(self):
         return self._room
 
     @property
     def ingress(self):
         return self._ingress
 
     @property
     def egress(self):
         return self._egress
 
+    @property
+    def sip(self):
+        return self._sip
+
     async def aclose(self):
         await self._session.close()
```

### Comparing `livekit-api-0.4.4/livekit/api/room_service.py` & `livekit_api-0.5.0/livekit/api/room_service.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/twirp_client.py` & `livekit_api-0.5.0/livekit/api/twirp_client.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit/api/webhook.py` & `livekit_api-0.5.0/livekit/api/webhook.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/livekit_api.egg-info/PKG-INFO` & `livekit_api-0.5.0/livekit_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-api
-Version: 0.4.4
+Version: 0.5.0
 Summary: Python Server API for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
@@ -15,18 +15,18 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: pyjwt>=2.0.0
 Requires-Dist: aiohttp>=3.9.0
 Requires-Dist: protobuf>=3
 Requires-Dist: types-protobuf<5,>=4
-Requires-Dist: livekit-protocol<1,>=0.3.0
+Requires-Dist: livekit-protocol<1,>=0.5.0
 
 # LiveKit Server APIs
 
 Access LiveKit server APIs and generate access tokens.
```

### Comparing `livekit-api-0.4.4/livekit_api.egg-info/SOURCES.txt` & `livekit_api-0.5.0/livekit_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 livekit/api/_service.py
 livekit/api/access_token.py
 livekit/api/egress_service.py
 livekit/api/ingress_service.py
 livekit/api/livekit_api.py
 livekit/api/py.typed
 livekit/api/room_service.py
+livekit/api/sip_service.py
 livekit/api/twirp_client.py
 livekit/api/version.py
 livekit/api/webhook.py
 livekit_api.egg-info/PKG-INFO
 livekit_api.egg-info/SOURCES.txt
 livekit_api.egg-info/dependency_links.txt
 livekit_api.egg-info/requires.txt
```

### Comparing `livekit-api-0.4.4/setup.py` & `livekit_api-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
-    python_requires=">=3.8.0",
+    python_requires=">=3.9.0",
     install_requires=[
         "pyjwt>=2.0.0",
         "aiohttp>=3.9.0",
         "protobuf>=3",
         "types-protobuf>=4,<5",
-        "livekit-protocol>=0.3.0,<1",
+        "livekit-protocol>=0.5.0,<1",
     ],
     package_data={
         "livekit.api": ["py.typed", "*.pyi", "**/*.pyi"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

### Comparing `livekit-api-0.4.4/tests/test_access_token.py` & `livekit_api-0.5.0/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `livekit-api-0.4.4/tests/test_webhook.py` & `livekit_api-0.5.0/tests/test_webhook.py`

 * *Files identical despite different names*

