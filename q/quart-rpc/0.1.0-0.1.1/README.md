# Comparing `tmp/quart_rpc-0.1.0.tar.gz` & `tmp/quart_rpc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rpc-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quart_rpc-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quart_rpc-0.1.0.tar` & `quart_rpc-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-0.1.0/LICENSE
--rw-r--r--   0        0        0     2404 2024-04-17 11:52:14.442324 quart_rpc-0.1.0/README.md
--rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-16 14:30:11.100187 quart_rpc-0.1.0/quart_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 quart_rpc-0.1.0/quart_rpc/latest.py
--rw-r--r--   0        0        0     4991 2024-04-17 11:54:48.947774 quart_rpc-0.1.0/quart_rpc/version_1_0.py
--rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-0.1.0/requirements/development.txt
--rw-r--r--   0        0        0        5 2024-04-16 16:23:25.735540 quart_rpc-0.1.0/requirements/main.txt
--rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 quart_rpc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2398 2024-04-17 12:28:45.946021 quart_rpc-0.1.1/README.md
+-rw-r--r--   0        0        0      351 2024-04-17 12:10:17.218479 quart_rpc-0.1.1/app/__init__.py
+-rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-17 12:30:28.691197 quart_rpc-0.1.1/quart_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 quart_rpc-0.1.1/quart_rpc/latest.py
+-rw-r--r--   0        0        0     4991 2024-04-17 11:54:48.947774 quart_rpc-0.1.1/quart_rpc/version_1_0.py
+-rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-0.1.1/requirements/development.txt
+-rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-0.1.1/requirements/main.txt
+-rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-0.1.1/test.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 quart_rpc-0.1.1/PKG-INFO
```

### Comparing `quart_rpc-0.1.0/.gitignore` & `quart_rpc-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.0/LICENSE` & `quart_rpc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.0/README.md` & `quart_rpc-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 )
 ```
 
 or 
 
 ```python
 ...
-rpc = RPC(
+RPC(
     app,   # or RPC(blueprint, ...)
     url_prefix="/rpc", 
     functions={
         "add_numbers": add_numbers
     }
 )
 ...
```

### Comparing `quart_rpc-0.1.0/pyproject.toml` & `quart_rpc-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.0/quart_rpc/version_1_0.py` & `quart_rpc-0.1.1/quart_rpc/version_1_0.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-0.1.0/PKG-INFO` & `quart_rpc-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-rpc
-Version: 0.1.0
+Version: 0.1.1
 Summary: Turn Quart into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -82,15 +82,15 @@
 )
 ```
 
 or 
 
 ```python
 ...
-rpc = RPC(
+RPC(
     app,   # or RPC(blueprint, ...)
     url_prefix="/rpc", 
     functions={
         "add_numbers": add_numbers
     }
 )
 ...
```

