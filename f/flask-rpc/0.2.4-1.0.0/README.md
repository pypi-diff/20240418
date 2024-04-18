# Comparing `tmp/flask_rpc-0.2.4.tar.gz` & `tmp/flask_rpc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.2.4.tar` & `flask_rpc-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.4/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.4/LICENSE
--rw-r--r--   0        0        0     3282 2024-04-17 12:29:00.576196 flask_rpc-0.2.4/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.4/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.4/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.4/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.4/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.4/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.4/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.4/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.4/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.4/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.4/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.4/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.4/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.4/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-0.2.4/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.4/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.4/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-17 12:29:29.413116 flask_rpc-0.2.4/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.4/flask_rpc/latest.py
--rw-r--r--   0        0        0     4964 2024-04-17 11:54:48.950561 flask_rpc-0.2.4/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.4/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.4/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.4/test.py
--rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 flask_rpc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4215 2024-04-18 10:28:37.234054 flask_rpc-1.0.0/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-1.0.0/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-1.0.0/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-1.0.0/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-1.0.0/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-1.0.0/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-1.0.0/app/rpc/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-18 09:59:24.864451 flask_rpc-1.0.0/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-1.0.0/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-1.0.0/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-1.0.0/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-1.0.0/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-1.0.0/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-1.0.0/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-1.0.0/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-1.0.0/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1295 2024-04-18 10:12:44.085102 flask_rpc-1.0.0/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-18 10:22:32.871556 flask_rpc-1.0.0/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:45:56.143643 flask_rpc-1.0.0/flask_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 flask_rpc-1.0.0/flask_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:54:54.237265 flask_rpc-1.0.0/flask_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 flask_rpc-1.0.0/flask_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 09:20:55.788505 flask_rpc-1.0.0/flask_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 09:29:34.502455 flask_rpc-1.0.0/flask_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1099 2024-04-18 09:29:34.502494 flask_rpc-1.0.0/flask_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5472 2024-04-18 10:20:32.444314 flask_rpc-1.0.0/flask_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 flask_rpc-1.0.0/flask_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-1.0.0/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-1.0.0/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-1.0.0/test.py
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 flask_rpc-1.0.0/PKG-INFO
```

### Comparing `flask_rpc-0.2.4/.gitignore` & `flask_rpc-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/LICENSE` & `flask_rpc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/README.md` & `flask_rpc-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 RPC standard, but uses its own standard,
 and primarily works with JSON over HTTP POST
 requests to call functions.
 
 This extension is designed to stay slim and provides
 methods for generating requests and request responses.
 
-It does not enforce or validate the data passed in, or the 
-data being sent back; this is left to the user to implement 
+It does not enforce or validate the data passed in, or the
+data being sent back; this is left to the user to implement
 in whatever way they feel comfortable (or not at all, if there's
 no need for it)
 
 Flask-RPC does validate the request coming in using
 Pydantic.
 
 This is to ensure that the request is structured
@@ -159,7 +159,63 @@
 {
   "frpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
+
+## Security
+
+You can lock down using RPC routes by using sessions and or host checking.
+
+### Session Auth
+
+`from quart_rpc.latest import RPCAuthSessionKey`
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    session_auth=RPCAuthSessionKey("logged_in", [True]),
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
+or a list of RPCAuthSessionKey:
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    session_auth=[
+        RPCAuthSessionKey("logged_in", [True]),
+        RPCAuthSessionKey("user_type", ["admin"])
+    ],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
+### Host Auth
+
+In the following example, only requests from `127.0.0.1:5000` will be accepted.
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    host_auth=["127.0.0.1:5000"],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
```

### Comparing `flask_rpc-0.2.4/app/__init__.py` & `flask_rpc-1.0.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/app/models/clients.py` & `flask_rpc-1.0.0/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/app/models/users.py` & `flask_rpc-1.0.0/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/app/rpc/clients/funcs/__init__.py` & `flask_rpc-1.0.0/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/app/templates/index.html` & `flask_rpc-1.0.0/app/templates/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <head>
     <title>Development</title>
     <script src="https://unpkg.com/flask-rpc-js@latest/cdn.js"></script>
     <script>
         {# The examples below are setting and getting session cookies over fetch #}
         function set_session() {
             fetch(
-                'http://127.0.0.1:5000/rpc/auth',
+                'http://127.0.0.1:5000/rpc/auth/login',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
                     body: frpc('login', null),
                 }
```

### Comparing `flask_rpc-0.2.4/flask_rpc/version_1_0.py` & `flask_rpc-1.0.0/flask_rpc/version_1_0/rpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,33 @@
 import typing as t
 
-from flask import Flask, Blueprint, request
-from pydantic import BaseModel, ValidationError
+from flask import Blueprint, Flask, request, session
+from pydantic import ValidationError
 
-
-class RPCModel(BaseModel):
-    frpc: float
-    function: str
-    data: t.Any
-
-
-class RPCRequest:
-    @classmethod
-    def build(
-        cls,
-        function: str,
-        data: t.Union[
-            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
-        ] = None,
-    ) -> t.Dict[str, t.Any]:
-        """
-        Build a request.
-
-        Version 1.0.
-
-        :param function: Str
-        :param data: Any (JSON serializable)
-        :return:
-        """
-        return {"frpc": 1.0, "function": function, "data": data}
-
-
-class RPCResponse:
-    @classmethod
-    def fail(
-        cls,
-        message: str = None,
-        data: t.Union[
-            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
-        ] = None,
-    ):
-        """
-        Return a failed response.
-
-        Version 1.0.
-
-        :param message: Str
-        :param data: Any (JSON serializable)
-        :return:
-        """
-        r = {"frpc": 1.0, "ok": False}
-
-        if message:
-            r["message"] = message
-        if data:
-            r["data"] = data
-
-        return r
-
-    @classmethod
-    def success(
-        cls,
-        data: t.Union[
-            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
-        ] = None,
-        message: str = None,
-    ):
-        """
-        Return a successful response.
-
-        Version 1.0.
-
-        :param data: Any (JSON serializable)
-        :param message: Str
-        :return:
-        """
-        r = {"frpc": 1.0, "ok": True}
-
-        if message:
-            r["message"] = message
-        if data:
-            r["data"] = data
-
-        return r
+from ._protocols import RPCAuthSessionKey
+from .model import RPCModel
+from .response import RPCResponse
+from .utilities import snake_case
 
 
 class RPC:
     LOOKUP: t.Dict[str, t.Callable]
 
+    _host_auth: t.List[str]
+    _session_auth: t.Union[RPCAuthSessionKey, t.List[RPCAuthSessionKey]]
+
     def __init__(
         self,
         app_or_blueprint: t.Union[Flask, Blueprint],
+        functions: t.Optional[t.Dict[str, t.Callable]] = None,
         url_prefix: str = "/",
-        functions: t.Dict[str, t.Callable] = None,
+        host_auth: t.Optional[t.List[str]] = None,
+        session_auth: t.Optional[
+            t.Union[RPCAuthSessionKey, t.List[RPCAuthSessionKey]]
+        ] = None,
     ):
         """
         Register the RPC route.
 
         :param app_or_blueprint: Flask / Blueprint
         :param url_prefix: Str
         """
@@ -110,14 +41,32 @@
             )
 
         self._register_route(app_or_blueprint, url_prefix)
 
         if functions:
             self.functions(**functions)
 
+        if host_auth:
+            self.host_auth(host_auth)
+        else:
+            self.host_auth([])
+
+        if session_auth:
+            self.session_auth(session_auth)
+        else:
+            self.session_auth([])
+
+    def host_auth(self, hosts: t.List[str]):
+        self._host_auth = hosts
+
+    def session_auth(
+        self, auth_session_keys: t.Union[RPCAuthSessionKey, t.List[RPCAuthSessionKey]]
+    ):
+        self._session_auth = auth_session_keys
+
     def functions(self, **kwargs: t.Callable):
         """
         Register RPC functions.
 
         remote_name=local_name
 
         :param kwargs:
@@ -157,41 +106,71 @@
                 raise ValueError(f"Function {f.__name__} already exists.")
 
             self.LOOKUP[f.__name__] = f
 
     def _register_route(
         self, route_compatible: t.Union[Flask, Blueprint], url_prefix: str
     ):
+        if not url_prefix.startswith("/"):
+            url_prefix = f"/{url_prefix}"
+
+        _default = ("/", "/rpc")
+        _blueprint_name = ""
+        if isinstance(route_compatible, Blueprint):
+            _blueprint_name = f"_{route_compatible.name}"
+
         route_compatible.add_url_rule(
             url_prefix,
             view_func=self._rpc_route,
+            endpoint="_rpc"
+            if url_prefix in _default
+            else f"_rpc{_blueprint_name}_{snake_case(url_prefix)}",
             provide_automatic_options=True,
             methods=["POST"],
         )
 
     def _rpc_route(self):
+        if not self.LOOKUP:
+            return RPCResponse.fail("No functions registered.")
+
+        if self._session_auth:
+            if isinstance(self._session_auth, RPCAuthSessionKey):
+                if not self._session_auth.check(session):
+                    return RPCResponse.fail("Unauthorized.")
+
+            if isinstance(self._session_auth, list):
+                for auth_session_key in self._session_auth:
+                    if isinstance(auth_session_key, RPCAuthSessionKey):
+                        if not auth_session_key.check(session):
+                            return RPCResponse.fail("Unauthorized.")
+                    else:
+                        raise ValueError("Invalid session_auth type.")
+
+        if self._host_auth:
+            if request.host not in self._host_auth:
+                return RPCResponse.fail(f"Unauthorized ({request.host})")
+
         if not request.is_json:
             return RPCResponse.fail("Request must be JSON.")
 
-        if not request.json:
+        _json = request.get_json()
+
+        if not _json:
             return RPCResponse.fail("Request must not be empty.")
 
-        if not request.json.get("frpc") == 1.0:
+        if not _json.get("frpc") == 1.0:
             return RPCResponse.fail("Invalid frpc version.")
 
         try:
-            rpcm = RPCModel(**request.json)
+            rpcm = RPCModel(**_json)
         except ValidationError:
             return RPCResponse.fail("Invalid request.")
 
         try:
             assert rpcm.function in self.LOOKUP
         except AssertionError:
             return RPCResponse.fail("Invalid function.")
 
         if successful_response := self.LOOKUP[rpcm.function](rpcm.data):
             return successful_response
 
         return RPCResponse.fail("Unsuccessful command execution.")
-
-
-__all__ = ["RPC", "RPCResponse", "RPCModel"]
```

### Comparing `flask_rpc-0.2.4/pyproject.toml` & `flask_rpc-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/test.py` & `flask_rpc-1.0.0/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.4/PKG-INFO` & `flask_rpc-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.2.4
+Version: 1.0.0
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -33,16 +33,16 @@
 RPC standard, but uses its own standard,
 and primarily works with JSON over HTTP POST
 requests to call functions.
 
 This extension is designed to stay slim and provides
 methods for generating requests and request responses.
 
-It does not enforce or validate the data passed in, or the 
-data being sent back; this is left to the user to implement 
+It does not enforce or validate the data passed in, or the
+data being sent back; this is left to the user to implement
 in whatever way they feel comfortable (or not at all, if there's
 no need for it)
 
 Flask-RPC does validate the request coming in using
 Pydantic.
 
 This is to ensure that the request is structured
@@ -177,7 +177,62 @@
   "frpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
 
+## Security
+
+You can lock down using RPC routes by using sessions and or host checking.
+
+### Session Auth
+
+`from quart_rpc.latest import RPCAuthSessionKey`
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    session_auth=RPCAuthSessionKey("logged_in", [True]),
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
+or a list of RPCAuthSessionKey:
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    session_auth=[
+        RPCAuthSessionKey("logged_in", [True]),
+        RPCAuthSessionKey("user_type", ["admin"])
+    ],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
+### Host Auth
+
+In the following example, only requests from `127.0.0.1:5000` will be accepted.
+
+```python
+...
+RPC(
+    app,  # or RPC(blueprint, ...)
+    url_prefix="/rpc",
+    host_auth=["127.0.0.1:5000"],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
```

