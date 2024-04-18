# Comparing `tmp/kv-api-0.1.3.tar.gz` & `tmp/kv_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-api-0.1.3.tar", last modified: Sat Apr  6 08:39:05 2024, max compression
+gzip compressed data, was "kv_api-0.1.4.tar", last modified: Thu Apr 18 07:01:32 2024, max compression
```

## Comparing `kv-api-0.1.3.tar` & `kv_api-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.973111 kv-api-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-06 08:39:05.973111 kv-api-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv-api-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-06 08:39:03.000000 kv-api-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 08:39:05.973111 kv-api-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.963111 kv-api-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.963111 kv-api-0.1.3/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.973111 kv-api-0.1.3/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-04-05 12:42:30.000000 kv-api-0.1.3/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2250 2024-04-06 08:38:45.000000 kv-api-0.1.3/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.973111 kv-api-0.1.3/src/kv/api/asyncify/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-05 12:42:30.000000 kv-api-0.1.3/src/kv/api/asyncify/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1395 2024-04-06 08:38:48.000000 kv-api-0.1.3/src/kv/api/asyncify/asyncify.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.973111 kv-api-0.1.3/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       70 2024-04-05 12:42:30.000000 kv-api-0.1.3/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      613 2024-04-05 12:42:30.000000 kv-api-0.1.3/src/kv/api/errors/errors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 08:39:05.973111 kv-api-0.1.3/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-06 08:39:05.000000 kv-api-0.1.3/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      356 2024-04-06 08:39:05.000000 kv-api-0.1.3/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 08:39:05.000000 kv-api-0.1.3/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-06 08:39:05.000000 kv-api-0.1.3/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-06 08:39:05.000000 kv-api-0.1.3/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-18 07:01:32.716112 kv_api-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      603 2024-04-18 07:01:28.000000 kv_api-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 07:01:32.716112 kv_api-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.706112 kv_api-0.1.4/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-18 06:51:44.000000 kv_api-0.1.4/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1327 2024-04-18 06:51:39.000000 kv_api-0.1.4/src/kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       45 2024-04-15 16:52:22.000000 kv_api-0.1.4/src/kv/api/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      762 2024-04-18 06:52:15.000000 kv_api-0.1.4/src/kv/api/append/append.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv/api/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.4/src/kv/api/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      679 2024-04-10 09:04:29.000000 kv_api-0.1.4/src/kv/api/errors/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-04-15 16:21:13.000000 kv_api-0.1.4/src/kv/api/locatable.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:32.716112 kv_api-0.1.4/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-18 07:01:32.000000 kv_api-0.1.4/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv-api-0.1.3/pyproject.toml` & `kv_api-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-api"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API spec for an async Key-Value DB"
 dependencies = [
   "haskellian-either"
 ]
```

### Comparing `kv-api-0.1.3/src/kv/api/errors/errors.py` & `kv_api-0.1.4/src/kv/api/errors/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Any
 from dataclasses import dataclass
 
 @dataclass(eq=False)
 class InexistentItem(BaseException):
-  key: str
+  key: str | None = None
   detail: Any | None = None
   reason: Literal['inexistent-item'] = 'inexistent-item'
 
 @dataclass(eq=False)
 class ExistentItem(BaseException):
   key: str
   detail: Any | None = None
@@ -17,8 +17,10 @@
 class DBError(BaseException):
   detail: Any = None
   reason: Literal['db-error'] = 'db-error'
 
 @dataclass(eq=False)
 class InvalidData(BaseException):
   detail: Any = None
-  reason: Literal['invalid-data'] = 'invalid-data'
+  reason: Literal['invalid-data'] = 'invalid-data'
+
+ReadError = DBError | InvalidData | InexistentItem
```

