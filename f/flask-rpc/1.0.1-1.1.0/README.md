# Comparing `tmp/flask_rpc-1.0.1.tar.gz` & `tmp/flask_rpc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-1.0.1.tar` & `flask_rpc-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-1.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-1.0.1/LICENSE
--rw-r--r--   0        0        0     4209 2024-04-18 10:37:58.725071 flask_rpc-1.0.1/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-1.0.1/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-1.0.1/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-1.0.1/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-1.0.1/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-1.0.1/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-1.0.1/app/rpc/__init__.py
--rw-r--r--   0        0        0      522 2024-04-18 09:59:24.864451 flask_rpc-1.0.1/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-1.0.1/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-1.0.1/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-1.0.1/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-1.0.1/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-1.0.1/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-1.0.1/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-1.0.1/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-1.0.1/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1295 2024-04-18 10:12:44.085102 flask_rpc-1.0.1/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-18 10:38:04.662265 flask_rpc-1.0.1/flask_rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-04-18 09:45:56.143643 flask_rpc-1.0.1/flask_rpc/latest.py
--rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 flask_rpc-1.0.1/flask_rpc/version_1_0/__init__.py
--rw-r--r--   0        0        0      160 2024-04-18 09:54:54.237265 flask_rpc-1.0.1/flask_rpc/version_1_0/_protocols.py
--rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 flask_rpc-1.0.1/flask_rpc/version_1_0/auth_session_key.py
--rw-r--r--   0        0        0      130 2024-04-18 09:20:55.788505 flask_rpc-1.0.1/flask_rpc/version_1_0/model.py
--rw-r--r--   0        0        0      480 2024-04-18 09:29:34.502455 flask_rpc-1.0.1/flask_rpc/version_1_0/request.py
--rw-r--r--   0        0        0     1099 2024-04-18 09:29:34.502494 flask_rpc-1.0.1/flask_rpc/version_1_0/response.py
--rw-r--r--   0        0        0     5472 2024-04-18 10:20:32.444314 flask_rpc-1.0.1/flask_rpc/version_1_0/rpc.py
--rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 flask_rpc-1.0.1/flask_rpc/version_1_0/utilities.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-1.0.1/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-1.0.1/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-1.0.1/test.py
--rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 flask_rpc-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4170 2024-04-18 11:07:36.421515 flask_rpc-1.1.0/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-1.1.0/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-1.1.0/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-1.1.0/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-1.1.0/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-1.1.0/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-1.1.0/app/rpc/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-18 09:59:24.864451 flask_rpc-1.1.0/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-1.1.0/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-1.1.0/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-1.1.0/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-1.1.0/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-1.1.0/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-1.1.0/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-1.1.0/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-1.1.0/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1290 2024-04-18 11:06:57.530208 flask_rpc-1.1.0/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-18 11:09:27.832512 flask_rpc-1.1.0/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:45:56.143643 flask_rpc-1.1.0/flask_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 flask_rpc-1.1.0/flask_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:54:54.237265 flask_rpc-1.1.0/flask_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 flask_rpc-1.1.0/flask_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 11:07:12.257730 flask_rpc-1.1.0/flask_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 11:07:12.256482 flask_rpc-1.1.0/flask_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1099 2024-04-18 11:07:12.258841 flask_rpc-1.1.0/flask_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5472 2024-04-18 11:07:12.254722 flask_rpc-1.1.0/flask_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 flask_rpc-1.1.0/flask_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-1.1.0/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-1.1.0/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-1.1.0/test.py
+-rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 flask_rpc-1.1.0/PKG-INFO
```

### Comparing `flask_rpc-1.0.1/.gitignore` & `flask_rpc-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/LICENSE` & `flask_rpc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/README.md` & `flask_rpc-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 Flask - Remote Procedure Call (RPC) is a simple
 library that allows you to expose functions
 in your Flask application to be called
 remotely. It is designed to be straightforward
 to use and easy to understand.
 
-Flask-RPC does not follow any current already existing
-RPC standard, but uses its own standard,
-and primarily works with JSON over HTTP POST
-requests to call functions.
+Flask-RPC uses mRPC as its protocol, which is a
+micro JSON-based protocol that allows for
+easy communication between the client and server.
 
 This extension is designed to stay slim and provides
 methods for generating requests and request responses.
 
 It does not enforce or validate the data passed in, or the
 data being sent back; this is left to the user to implement
 in whatever way they feel comfortable (or not at all, if there's
@@ -36,40 +35,40 @@
 
 The typical request/response cycle is as follows:
 
 **Request**
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "function": "add_numbers",
   "data": [
     1,
     2,
     3
   ]
 }
 ```
 
 **Response**
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
 
 ## Usage
 
 [This repo](https://github.com/CheeseCake87/flask-rpc) contains a working example of Flask-RPC.
 
-It also includes an example of using the [JS library](https://github.com/CheeseCake87/flask-rpc-js) that helps
+It also includes an example of using the [JS library](https://github.com/CheeseCake87/wrpc-js) that helps
 in making requests via fetch to Flask-RPC.
 
 ### Simplest example
 
 ```python
 from flask import Flask
 
@@ -134,34 +133,34 @@
     json=RPCRequest.build(
         function="add_numbers",
         data=[1, 2, 3]
     )
 )
 ```
 
-or, if you're using the [JS library](https://github.com/CheeseCake87/flask-rpc-js):
+or, if you're using the [JS library](https://github.com/CheeseCake87/wrpc-js):
 
 ```js
 fetch("/rpc", {
     method: "POST",
     headers: {
         "Content-Type": "application/json"
     },
-    body: frpc(
+    body: wrpc(
         function_ = "add_numbers",
         data = [1, 2, 3]
     )
 })
 ```
 
 Will return:
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
 
 ## Security
```

### Comparing `flask_rpc-1.0.1/app/__init__.py` & `flask_rpc-1.1.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/app/models/clients.py` & `flask_rpc-1.1.0/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/app/models/users.py` & `flask_rpc-1.1.0/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/app/rpc/auth/__init__.py` & `flask_rpc-1.1.0/app/rpc/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/app/rpc/clients/funcs/__init__.py` & `flask_rpc-1.1.0/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/app/templates/index.html` & `flask_rpc-1.1.0/app/templates/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 <html lang="gb">
 <head>
     <title>Development</title>
-    <script src="https://unpkg.com/flask-rpc-js@latest/cdn.js"></script>
+    <script src="https://unpkg.com/wrpc-js@latest/cdn.js"></script>
     <script>
         {# The examples below are setting and getting session cookies over fetch #}
         function set_session() {
             fetch(
                 'http://127.0.0.1:5000/rpc/auth/login',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
-                    body: frpc('login', null),
+                    body: wrpc('login', null),
                 }
             )
                 .then(response => response.json())
                 .then(data => console.log(data));
         }
 
         function do_fetch() {
             fetch(
                 'http://127.0.0.1:5000/rpc/auth',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
-                    body: frpc('session', null),
+                    body: wrpc('session', null),
                 }
             )
                 .then(response => response.json())
                 .then(data => console.log(data));
         }
     </script>
 </head>
```

### Comparing `flask_rpc-1.0.1/flask_rpc/version_1_0/response.py` & `flask_rpc-1.1.0/flask_rpc/version_1_0/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         Version 1.0.
 
         :param message: Str
         :param data: Any (JSON serializable)
         :return:
         """
-        r = {"frpc": 1.0, "ok": False}
+        r = {"wrpc": 1.0, "ok": False}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
@@ -41,15 +41,15 @@
 
         Version 1.0.
 
         :param data: Any (JSON serializable)
         :param message: Str
         :return:
         """
-        r = {"frpc": 1.0, "ok": True}
+        r = {"wrpc": 1.0, "ok": True}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
```

### Comparing `flask_rpc-1.0.1/flask_rpc/version_1_0/rpc.py` & `flask_rpc-1.1.0/flask_rpc/version_1_0/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
             return RPCResponse.fail("Request must be JSON.")
 
         _json = request.get_json()
 
         if not _json:
             return RPCResponse.fail("Request must not be empty.")
 
-        if not _json.get("frpc") == 1.0:
-            return RPCResponse.fail("Invalid frpc version.")
+        if not _json.get("wrpc") == 1.0:
+            return RPCResponse.fail("Invalid wrpc version.")
 
         try:
             rpcm = RPCModel(**_json)
         except ValidationError:
             return RPCResponse.fail("Invalid request.")
 
         try:
```

### Comparing `flask_rpc-1.0.1/flask_rpc/version_1_0/utilities.py` & `flask_rpc-1.1.0/flask_rpc/version_1_0/utilities.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/pyproject.toml` & `flask_rpc-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/test.py` & `flask_rpc-1.1.0/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.0.1/PKG-INFO` & `flask_rpc-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 1.0.1
+Version: 1.1.0
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,18 +25,17 @@
 
 Flask - Remote Procedure Call (RPC) is a simple
 library that allows you to expose functions
 in your Flask application to be called
 remotely. It is designed to be straightforward
 to use and easy to understand.
 
-Flask-RPC does not follow any current already existing
-RPC standard, but uses its own standard,
-and primarily works with JSON over HTTP POST
-requests to call functions.
+Flask-RPC uses mRPC as its protocol, which is a
+micro JSON-based protocol that allows for
+easy communication between the client and server.
 
 This extension is designed to stay slim and provides
 methods for generating requests and request responses.
 
 It does not enforce or validate the data passed in, or the
 data being sent back; this is left to the user to implement
 in whatever way they feel comfortable (or not at all, if there's
@@ -53,40 +52,40 @@
 
 The typical request/response cycle is as follows:
 
 **Request**
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "function": "add_numbers",
   "data": [
     1,
     2,
     3
   ]
 }
 ```
 
 **Response**
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
 
 ## Usage
 
 [This repo](https://github.com/CheeseCake87/flask-rpc) contains a working example of Flask-RPC.
 
-It also includes an example of using the [JS library](https://github.com/CheeseCake87/flask-rpc-js) that helps
+It also includes an example of using the [JS library](https://github.com/CheeseCake87/wrpc-js) that helps
 in making requests via fetch to Flask-RPC.
 
 ### Simplest example
 
 ```python
 from flask import Flask
 
@@ -151,34 +150,34 @@
     json=RPCRequest.build(
         function="add_numbers",
         data=[1, 2, 3]
     )
 )
 ```
 
-or, if you're using the [JS library](https://github.com/CheeseCake87/flask-rpc-js):
+or, if you're using the [JS library](https://github.com/CheeseCake87/wrpc-js):
 
 ```js
 fetch("/rpc", {
     method: "POST",
     headers: {
         "Content-Type": "application/json"
     },
-    body: frpc(
+    body: wrpc(
         function_ = "add_numbers",
         data = [1, 2, 3]
     )
 })
 ```
 
 Will return:
 
 ```json
 {
-  "frpc": 1.0,
+  "wrpc": 1.0,
   "ok": true,
   "message": "Function 'add_numbers' executed successfully",
   "data": 6
 }
 ```
 
 ## Security
```

