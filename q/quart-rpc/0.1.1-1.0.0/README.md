# Comparing `tmp/quart_rpc-0.1.1.tar.gz` & `tmp/quart_rpc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rpc-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quart_rpc-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quart_rpc-0.1.1.tar` & `quart_rpc-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-0.1.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-0.1.1/LICENSE
--rw-r--r--   0        0        0     2398 2024-04-17 12:28:45.946021 quart_rpc-0.1.1/README.md
--rw-r--r--   0        0        0      351 2024-04-17 12:10:17.218479 quart_rpc-0.1.1/app/__init__.py
--rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-17 12:30:28.691197 quart_rpc-0.1.1/quart_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 quart_rpc-0.1.1/quart_rpc/latest.py
--rw-r--r--   0        0        0     4991 2024-04-17 11:54:48.947774 quart_rpc-0.1.1/quart_rpc/version_1_0.py
--rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-0.1.1/requirements/development.txt
--rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-0.1.1/requirements/main.txt
--rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-0.1.1/test.py
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 quart_rpc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3338 2024-04-18 10:28:37.230981 quart_rpc-1.0.0/README.md
+-rw-r--r--   0        0        0     1024 2024-04-18 09:57:23.895002 quart_rpc-1.0.0/app/__init__.py
+-rw-r--r--   0        0        0     1860 2024-04-18 09:33:26.433854 quart_rpc-1.0.0/app/templates/index.html
+-rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-18 10:22:40.782750 quart_rpc-1.0.0/quart_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.0.0/quart_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.0.0/quart_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.0.0/quart_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.0.0/quart_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 09:20:55.788505 quart_rpc-1.0.0/quart_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 09:29:34.502455 quart_rpc-1.0.0/quart_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1099 2024-04-18 09:29:34.502494 quart_rpc-1.0.0/quart_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5484 2024-04-18 10:19:59.977860 quart_rpc-1.0.0/quart_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.0.0/quart_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.0.0/requirements/development.txt
+-rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.0.0/requirements/main.txt
+-rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-1.0.0/test.py
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 quart_rpc-1.0.0/PKG-INFO
```

### Comparing `quart_rpc-0.1.1/.gitignore` & `quart_rpc-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.1/LICENSE` & `quart_rpc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.1/README.md` & `quart_rpc-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -133,7 +133,62 @@
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
+    app,   # or RPC(blueprint, ...)
+    url_prefix="/rpc", 
+    session_auth=RPCAuthSessionKey("logged_in", [True]),
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+or a list of RPCAuthSessionKey:
+
+```python
+...
+RPC(
+    app,   # or RPC(blueprint, ...)
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
+    app,   # or RPC(blueprint, ...)
+    url_prefix="/rpc", 
+    host_auth=["127.0.0.1:5000"],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
```

### Comparing `quart_rpc-0.1.1/pyproject.toml` & `quart_rpc-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.1/PKG-INFO` & `quart_rpc-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-rpc
-Version: 0.1.1
+Version: 1.0.0
 Summary: Turn Quart into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -151,7 +151,61 @@
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
+    app,   # or RPC(blueprint, ...)
+    url_prefix="/rpc", 
+    session_auth=RPCAuthSessionKey("logged_in", [True]),
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+or a list of RPCAuthSessionKey:
+
+```python
+...
+RPC(
+    app,   # or RPC(blueprint, ...)
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
+    app,   # or RPC(blueprint, ...)
+    url_prefix="/rpc", 
+    host_auth=["127.0.0.1:5000"],
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
```
