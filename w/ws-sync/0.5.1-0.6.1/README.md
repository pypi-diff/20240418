# Comparing `tmp/ws_sync-0.5.1.tar.gz` & `tmp/ws_sync-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_sync-0.5.1.tar", max compression
+gzip compressed data, was "ws_sync-0.6.1.tar", max compression
```

## Comparing `ws_sync-0.5.1.tar` & `ws_sync-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     4912 2024-02-20 18:33:05.515422 ws_sync-0.5.1/README.md
--rw-r--r--   0        0        0      374 2024-03-20 20:11:14.216019 ws_sync-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      105 2024-01-31 22:36:00.124200 ws_sync-0.5.1/ws_sync/__init__.py
--rw-r--r--   0        0        0      842 2024-01-31 22:47:04.922252 ws_sync-0.5.1/ws_sync/id.py
--rw-r--r--   0        0        0     5195 2024-03-19 01:00:21.532814 ws_sync-0.5.1/ws_sync/session.py
--rw-r--r--   0        0        0    12805 2024-03-20 20:10:37.550469 ws_sync-0.5.1/ws_sync/sync.py
--rw-r--r--   0        0        0      435 2024-03-12 17:30:00.703593 ws_sync-0.5.1/ws_sync/utils.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ws_sync-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4912 2024-02-20 18:33:05.515422 ws_sync-0.6.1/README.md
+-rw-r--r--   0        0        0      374 2024-04-18 01:05:03.783505 ws_sync-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      429 2024-04-03 03:54:28.931620 ws_sync-0.6.1/ws_sync/__init__.py
+-rw-r--r--   0        0        0     3484 2024-04-03 03:52:59.911008 ws_sync-0.6.1/ws_sync/decorators.py
+-rw-r--r--   0        0        0      842 2024-01-31 22:47:04.922252 ws_sync-0.6.1/ws_sync/id.py
+-rw-r--r--   0        0        0     4912 2024-04-18 01:04:18.002636 ws_sync-0.6.1/ws_sync/session.py
+-rw-r--r--   0        0        0    16688 2024-04-03 05:19:45.797505 ws_sync-0.6.1/ws_sync/sync.py
+-rw-r--r--   0        0        0      705 2024-04-03 03:01:49.284779 ws_sync-0.6.1/ws_sync/utils.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ws_sync-0.6.1/PKG-INFO
```

### Comparing `ws_sync-0.5.1/README.md` & `ws_sync-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ws_sync-0.5.1/ws_sync/id.py` & `ws_sync-0.6.1/ws_sync/id.py`

 * *Files identical despite different names*

### Comparing `ws_sync-0.5.1/ws_sync/session.py` & `ws_sync-0.6.1/ws_sync/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,34 @@
+from __future__ import annotations
 from logging import Logger
 import traceback
 from typing import Callable
+from contextvars import ContextVar
+
 from starlette.websockets import WebSocket, WebSocketDisconnect
 
 from .utils import nonblock_call
 
-# global default session, which can be temporarily overwritten by the context manager
-_global_session = None
-
-
-def get_global_session():
-    global _global_session
-    if _global_session is None:
-        raise Exception(
-            "No global session found. Please use the Session context manager."
-        )
-    return _global_session
+# session context
+session_context: ContextVar[Session] = ContextVar("session_context")
 
 
 class Session:
     """
     This is a counter-part to the SessionManager in the frontend.
     There should be one instance of this class per user session, even across reconnects of the websocket. This means the states that belong to the user session should be subscribed to the events of this class.
     It defines a simple state-syncing protocol between the frontend and the backend, every event being of type {type: str, data: any}.
     """
 
     def __init__(self, logger: Logger = None):
         self.ws = None
         self.event_handlers: dict[str, Callable] = {}  # triggered on event
         self.init_handlers: list[Callable] = []  # triggered on connection init
         self.logger = logger
+        self.state = None  # user-assigned state associated with the session
 
     @property
     def is_connected(self):
         return self.ws is not None
 
     # ===== Low-Level: Register Event Callbacks =====#
     def register_event(self, event: str, callback: Callable):
@@ -132,16 +127,12 @@
                 self.ws = None
                 await ws.close()
             except:
                 pass
 
     # ===== High-Level: Context Manager =====#
     def __enter__(self):
-        global _global_session
-        self._prev_global_connection = _global_session
-        _global_session = self
+        session_context.set(self)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        global _global_session
-        _global_session = self._prev_global_connection
-        self._prev_global_connection = None
+        session_context.reset()
```

### Comparing `ws_sync-0.5.1/PKG-INFO` & `ws_sync-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-sync
-Version: 0.5.1
+Version: 0.6.1
 Summary: Keep objects synchronized over a persistent WebSocket session
 Author: Joong-Won Seo
 Author-email: joong.won.seo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

