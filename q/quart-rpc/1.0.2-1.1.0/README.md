# Comparing `tmp/quart_rpc-1.0.2.tar.gz` & `tmp/quart_rpc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rpc-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quart_rpc-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quart_rpc-1.0.2.tar` & `quart_rpc-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.0.2/LICENSE
--rw-r--r--   0        0        0     3322 2024-04-18 10:51:12.008254 quart_rpc-1.0.2/README.md
--rw-r--r--   0        0        0     1024 2024-04-18 09:57:23.895002 quart_rpc-1.0.2/app/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-18 10:52:01.414189 quart_rpc-1.0.2/app/templates/index.html
--rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-18 10:51:27.646532 quart_rpc-1.0.2/quart_rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.0.2/quart_rpc/latest.py
--rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.0.2/quart_rpc/version_1_0/__init__.py
--rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.0.2/quart_rpc/version_1_0/_protocols.py
--rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.0.2/quart_rpc/version_1_0/auth_session_key.py
--rw-r--r--   0        0        0      130 2024-04-18 09:20:55.788505 quart_rpc-1.0.2/quart_rpc/version_1_0/model.py
--rw-r--r--   0        0        0      480 2024-04-18 09:29:34.502455 quart_rpc-1.0.2/quart_rpc/version_1_0/request.py
--rw-r--r--   0        0        0     1099 2024-04-18 09:29:34.502494 quart_rpc-1.0.2/quart_rpc/version_1_0/response.py
--rw-r--r--   0        0        0     5484 2024-04-18 10:19:59.977860 quart_rpc-1.0.2/quart_rpc/version_1_0/rpc.py
--rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.0.2/quart_rpc/version_1_0/utilities.py
--rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.0.2/requirements/development.txt
--rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.0.2/requirements/main.txt
--rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-1.0.2/test.py
--rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 quart_rpc-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3322 2024-04-18 11:06:57.528560 quart_rpc-1.1.0/README.md
+-rw-r--r--   0        0        0     1024 2024-04-18 09:57:23.895002 quart_rpc-1.1.0/app/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-18 11:05:10.605491 quart_rpc-1.1.0/app/templates/index.html
+-rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-18 11:10:40.087655 quart_rpc-1.1.0/quart_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.1.0/quart_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.1.0/quart_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.1.0/quart_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.1.0/quart_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 11:05:19.979675 quart_rpc-1.1.0/quart_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 11:05:19.992185 quart_rpc-1.1.0/quart_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1099 2024-04-18 11:05:19.986245 quart_rpc-1.1.0/quart_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5484 2024-04-18 11:05:19.972570 quart_rpc-1.1.0/quart_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.1.0/quart_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.1.0/requirements/development.txt
+-rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.1.0/requirements/main.txt
+-rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-1.1.0/test.py
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 quart_rpc-1.1.0/PKG-INFO
```

### Comparing `quart_rpc-1.0.2/.gitignore` & `quart_rpc-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.0.2/LICENSE` & `quart_rpc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.0.2/README.md` & `quart_rpc-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 
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
 
 [This repo](https://github.com/CheeseCake87/quart-rpc) contains a working example of Quart-RPC.
 
-It also includes an example of using the [JS library](https://github.com/CheeseCake87/frpc-js) that helps
+It also includes an example of using the [JS library](https://github.com/CheeseCake87/wrpc-js) that helps
 in making requests via fetch to Quart-RPC.
 
 ### Simplest example
 
 ```python
 from quart import Quart
 
@@ -108,34 +108,34 @@
     json=RPCRequest.build(
         function="add_numbers",
         data=[1, 2, 3]
     )
 )
 ```
 
-or, if you're using the [JS library](https://github.com/CheeseCake87/frpc-js):
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

### Comparing `quart_rpc-1.0.2/app/__init__.py` & `quart_rpc-1.1.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.0.2/app/templates/index.html` & `quart_rpc-1.1.0/app/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <html lang="gb">
 <head>
 
     <title>Quart-RPC</title>
 
     <script src="//unpkg.com/alpinejs" defer></script>
-    <script src="https://unpkg.com/frpc-js@latest/cdn.js"></script>
+    <script src="https://unpkg.com/wrpc-js@latest/cdn.js"></script>
 
     <script>
         document.addEventListener('alpine:init', () => {
             Alpine.data('rpc', () => ({
 
                 result_text: 'awaiting action',
                 result: null,
@@ -16,15 +16,15 @@
                 check_auth() {
                     fetch('/rpc', {
                         method: 'POST',
                         include: 'credentials',
                         headers: {
                             'Content-Type': 'application/json',
                         },
-                        body: frpc('add_numbers', [1, 2, 3])
+                        body: wrpc('add_numbers', [1, 2, 3])
                     })
                         .then(response => response.json())
                         .then(jsond => {
                             console.log(jsond)
                             if (jsond.ok) {
                                 this.result_text = "Success";
                                 this.result = jsond.data;
```

### Comparing `quart_rpc-1.0.2/pyproject.toml` & `quart_rpc-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.0.2/quart_rpc/version_1_0/response.py` & `quart_rpc-1.1.0/quart_rpc/version_1_0/response.py`

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

### Comparing `quart_rpc-1.0.2/quart_rpc/version_1_0/rpc.py` & `quart_rpc-1.1.0/quart_rpc/version_1_0/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,16 +153,16 @@
             return RPCResponse.fail("Request must be JSON.")
 
         _json = await request.get_json()
 
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

### Comparing `quart_rpc-1.0.2/quart_rpc/version_1_0/utilities.py` & `quart_rpc-1.1.0/quart_rpc/version_1_0/utilities.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.0.2/PKG-INFO` & `quart_rpc-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-rpc
-Version: 1.0.2
+Version: 1.1.0
 Summary: Turn Quart into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,40 +27,40 @@
 
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
 
 [This repo](https://github.com/CheeseCake87/quart-rpc) contains a working example of Quart-RPC.
 
-It also includes an example of using the [JS library](https://github.com/CheeseCake87/frpc-js) that helps
+It also includes an example of using the [JS library](https://github.com/CheeseCake87/wrpc-js) that helps
 in making requests via fetch to Quart-RPC.
 
 ### Simplest example
 
 ```python
 from quart import Quart
 
@@ -125,34 +125,34 @@
     json=RPCRequest.build(
         function="add_numbers",
         data=[1, 2, 3]
     )
 )
 ```
 
-or, if you're using the [JS library](https://github.com/CheeseCake87/frpc-js):
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

