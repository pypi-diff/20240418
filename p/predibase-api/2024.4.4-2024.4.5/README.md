# Comparing `tmp/predibase-api-2024.4.4.tar.gz` & `tmp/predibase-api-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2024.4.4.tar", last modified: Thu Apr 18 20:38:32 2024, max compression
+gzip compressed data, was "predibase-api-2024.4.5.tar", last modified: Thu Apr 18 20:47:08 2024, max compression
```

## Comparing `predibase-api-2024.4.4.tar` & `predibase-api-2024.4.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.657450 predibase-api-2024.4.4/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.657450 predibase-api-2024.4.4/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.657450 predibase-api-2024.4.4/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:38:32.657450 predibase-api-2024.4.4/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:38:32.000000 predibase-api-2024.4.4/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 20:38:32.000000 predibase-api-2024.4.4/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:38:32.000000 predibase-api-2024.4.4/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:37:44.000000 predibase-api-2024.4.4/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:38:32.000000 predibase-api-2024.4.4/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:38:32.000000 predibase-api-2024.4.4/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:38:32.661450 predibase-api-2024.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 20:36:39.000000 predibase-api-2024.4.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:38:28.000000 predibase-api-2024.4.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.039773 predibase-api-2024.4.5/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:47:07.000000 predibase-api-2024.4.5/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 20:47:08.000000 predibase-api-2024.4.5/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:47:07.000000 predibase-api-2024.4.5/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:46:19.000000 predibase-api-2024.4.5/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:47:07.000000 predibase-api-2024.4.5/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:47:07.000000 predibase-api-2024.4.5/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:47:08.043773 predibase-api-2024.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 20:45:02.000000 predibase-api-2024.4.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:47:02.000000 predibase-api-2024.4.5/version.txt
```

### Comparing `predibase-api-2024.4.4/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2024.4.5/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2024.4.5/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2024.4.5/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2024.4.5/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2024.4.5/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2024.4.5/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2024.4.5/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.4/setup.py` & `predibase-api-2024.4.5/setup.py`

 * *Files identical despite different names*

