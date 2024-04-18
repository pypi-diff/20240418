# Comparing `tmp/kv-fs-0.1.5.tar.gz` & `tmp/kv_fs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-fs-0.1.5.tar", last modified: Tue Apr  9 18:36:00 2024, max compression
+gzip compressed data, was "kv_fs-0.1.6.tar", last modified: Thu Apr 18 07:01:56 2024, max compression
```

## Comparing `kv-fs-0.1.5.tar` & `kv_fs-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 18:36:00.020682 kv-fs-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv-fs-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-09 18:35:57.000000 kv-fs-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 18:36:00.020682 kv-fs-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2660 2024-04-09 18:35:22.000000 kv-fs-0.1.5/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/json/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/json/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/json/json.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2007 2024-04-09 04:44:24.000000 kv-fs-0.1.5/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      354 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.916112 kv_fs-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-18 07:01:56.916112 kv_fs-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv_fs-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-18 07:01:47.000000 kv_fs-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 07:01:56.916112 kv_fs-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.896112 kv_fs-0.1.6/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv_fs-0.1.6/src/kv/fs/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv_fs-0.1.6/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3520 2024-04-18 06:52:28.000000 kv_fs-0.1.6/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 16:51:53.000000 kv_fs-0.1.6/src/kv/fs/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1109 2024-04-15 17:43:37.000000 kv_fs-0.1.6/src/kv/fs/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-15 16:09:48.000000 kv_fs-0.1.6/src/kv/fs/append/ndjson.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       84 2024-04-15 15:13:10.000000 kv_fs-0.1.6/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2274 2024-04-15 15:48:34.000000 kv_fs-0.1.6/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 07:01:56.906112 kv_fs-0.1.6/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      387 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-18 07:01:56.000000 kv_fs-0.1.6/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv-fs-0.1.5/PKG-INFO` & `kv_fs-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.5
+Version: 0.1.6
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv-fs-0.1.5/README.md` & `kv_fs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.5/pyproject.toml` & `kv_fs-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-fs"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value DB API on the filesystem"
 dependencies = [
   "kv-api", "ramda", "haskellian-either"
 ]
```

### Comparing `kv-fs-0.1.5/src/kv/fs/ops/ops.py` & `kv_fs-0.1.6/src/kv/fs/ops/ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 from haskellian.either import Either, Left, Right, safe
 
 def ensure_path(file: str):
   dir = os.path.dirname(file)
   if dir != '':
     os.makedirs(dir, exist_ok=True)
 
+def append(path: str, data: str|bytes) -> Either[OSError, None]:
+  mode = f'ab' if isinstance(data, bytes) else 'a'
+  try:
+    ensure_path(path)
+    with open(path, mode) as f:
+      f.write(data)
+      return Right(None)
+  except OSError as e:
+    return Left(e)
+
 def insert(path: str, data: str|bytes, *, exists_ok: bool = False) -> Either[FileExistsError | OSError, None]:
   access = 'w' if exists_ok else 'x'
   mode = f'{access}b' if isinstance(data, bytes) else access
   try:
     ensure_path(path)
     with open(path, mode) as f:
       f.write(data)
@@ -22,15 +32,15 @@
   mode = 'r+b' if isinstance(data, bytes) else 'r+'
   try:
     with open(path, mode) as f:
       f.write(data)
       return Right(None)
   except (FileNotFoundError, OSError) as e:
     return Left(e)
-
+  
 def read(path: str) -> Either[FileNotFoundError | OSError, bytes]:
   try:
     with open(path, 'rb') as f:
       return Right(f.read())
   except (FileNotFoundError, OSError) as e:
     return Left(e)
```

### Comparing `kv-fs-0.1.5/src/kv_fs.egg-info/PKG-INFO` & `kv_fs-0.1.6/src/kv_fs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.5
+Version: 0.1.6
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

