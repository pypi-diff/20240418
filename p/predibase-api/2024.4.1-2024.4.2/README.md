# Comparing `tmp/predibase-api-2024.4.1.tar.gz` & `tmp/predibase-api-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2024.4.1.tar", last modified: Thu Apr 18 20:03:44 2024, max compression
+gzip compressed data, was "predibase-api-2024.4.2.tar", last modified: Thu Apr 18 20:31:15 2024, max compression
```

## Comparing `predibase-api-2024.4.1.tar` & `predibase-api-2024.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.613184 predibase-api-2024.4.1/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:03:44.000000 predibase-api-2024.4.1/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 20:03:44.000000 predibase-api-2024.4.1/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:03:44.000000 predibase-api-2024.4.1/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:02:53.000000 predibase-api-2024.4.1/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:03:44.000000 predibase-api-2024.4.1/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:03:44.000000 predibase-api-2024.4.1/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:03:44.617184 predibase-api-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 20:01:44.000000 predibase-api-2024.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:03:39.000000 predibase-api-2024.4.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.446135 predibase-api-2024.4.2/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 20:31:15.000000 predibase-api-2024.4.2/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-18 20:31:15.000000 predibase-api-2024.4.2/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:15.000000 predibase-api-2024.4.2/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:30:23.000000 predibase-api-2024.4.2/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:31:15.000000 predibase-api-2024.4.2/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:31:15.000000 predibase-api-2024.4.2/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:31:15.450135 predibase-api-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 20:29:15.000000 predibase-api-2024.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 20:31:10.000000 predibase-api-2024.4.2/version.txt
```

### Comparing `predibase-api-2024.4.1/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2024.4.2/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2024.4.2/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2024.4.2/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2024.4.2/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2024.4.2/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2024.4.2/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2024.4.2/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.1/setup.py` & `predibase-api-2024.4.2/setup.py`

 * *Files identical despite different names*

