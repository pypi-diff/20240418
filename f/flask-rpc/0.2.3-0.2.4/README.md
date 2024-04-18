# Comparing `tmp/flask_rpc-0.2.3.tar.gz` & `tmp/flask_rpc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.2.3.tar` & `flask_rpc-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.3/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.3/LICENSE
--rw-r--r--   0        0        0     3159 2024-04-13 10:47:58.119119 flask_rpc-0.2.3/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.3/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.3/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.3/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.3/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.3/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.3/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.3/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.3/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.3/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.3/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.3/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.3/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.3/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-0.2.3/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.3/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.3/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-17 11:59:29.370829 flask_rpc-0.2.3/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.3/flask_rpc/latest.py
--rw-r--r--   0        0        0     4964 2024-04-17 11:54:48.950561 flask_rpc-0.2.3/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.3/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.3/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.3/test.py
--rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 flask_rpc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3282 2024-04-17 12:29:00.576196 flask_rpc-0.2.4/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.4/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.4/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.4/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.4/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.4/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.4/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.4/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.4/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.4/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.4/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.4/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.4/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.4/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-0.2.4/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.4/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.4/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-17 12:29:29.413116 flask_rpc-0.2.4/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.4/flask_rpc/latest.py
+-rw-r--r--   0        0        0     4964 2024-04-17 11:54:48.950561 flask_rpc-0.2.4/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.4/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.4/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.4/test.py
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 flask_rpc-0.2.4/PKG-INFO
```

### Comparing `flask_rpc-0.2.3/.gitignore` & `flask_rpc-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/LICENSE` & `flask_rpc-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/README.md` & `flask_rpc-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,28 @@
 app = Flask(__name__)
 rpc = RPC(app, url_prefix="/rpc")  # or RPC(blueprint)
 rpc.functions(
     add_numbers=add_numbers
 )
 ```
 
+or
+
+```python
+...
+RPC(
+    app,
+    url_prefix="/rpc",
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
 `RPC(...)`
 
 Will register a POST route with the app or blueprint that you pass in.
 
 `rpc.functions(...)`
 
 Will register the functions that you pass in to be called remotely.
```

### Comparing `flask_rpc-0.2.3/app/__init__.py` & `flask_rpc-0.2.4/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/app/models/clients.py` & `flask_rpc-0.2.4/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/app/models/users.py` & `flask_rpc-0.2.4/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.2.4/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/app/templates/index.html` & `flask_rpc-0.2.4/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/flask_rpc/version_1_0.py` & `flask_rpc-0.2.4/flask_rpc/version_1_0.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/pyproject.toml` & `flask_rpc-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/test.py` & `flask_rpc-0.2.4/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.3/PKG-INFO` & `flask_rpc-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.2.3
+Version: 0.2.4
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -104,14 +104,28 @@
 app = Flask(__name__)
 rpc = RPC(app, url_prefix="/rpc")  # or RPC(blueprint)
 rpc.functions(
     add_numbers=add_numbers
 )
 ```
 
+or
+
+```python
+...
+RPC(
+    app,
+    url_prefix="/rpc",
+    functions={
+        "add_numbers": add_numbers
+    }
+)
+...
+```
+
 `RPC(...)`
 
 Will register a POST route with the app or blueprint that you pass in.
 
 `rpc.functions(...)`
 
 Will register the functions that you pass in to be called remotely.
```

