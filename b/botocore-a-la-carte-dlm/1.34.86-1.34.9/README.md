# Comparing `tmp/botocore-a-la-carte-dlm-1.34.86.tar.gz` & `tmp/botocore-a-la-carte-dlm-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-dlm-1.34.86.tar", last modified: Thu Apr 18 01:00:18 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-dlm-1.34.9.tar", last modified: Thu Dec 28 01:06:44 2023, max compression
```

## Comparing `botocore-a-la-carte-dlm-1.34.86.tar` & `botocore-a-la-carte-dlm-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.867291 botocore-a-la-carte-dlm-1.34.86/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 01:00:18.867291 botocore-a-la-carte-dlm-1.34.86/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.863291 botocore-a-la-carte-dlm-1.34.86/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.863291 botocore-a-la-carte-dlm-1.34.86/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.863291 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.867291 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-18 01:00:01.000000 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 01:00:01.000000 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 01:00:01.000000 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    76301 2024-04-18 01:00:01.000000 botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:00:18.867291 botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:00:18.867291 botocore-a-la-carte-dlm-1.34.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 01:00:18.000000 botocore-a-la-carte-dlm-1.34.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.130297 botocore-a-la-carte-dlm-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:43.000000 botocore-a-la-carte-dlm-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:44.130297 botocore-a-la-carte-dlm-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.126297 botocore-a-la-carte-dlm-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.126297 botocore-a-la-carte-dlm-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.126297 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.126297 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2023-12-28 01:06:26.000000 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76301 2023-12-28 01:06:26.000000 botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:44.130297 botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:44.000000 botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-28 01:06:44.000000 botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:44.000000 botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:44.000000 botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:44.130297 botocore-a-la-carte-dlm-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:06:43.000000 botocore-a-la-carte-dlm-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-dlm-1.34.86/LICENSE.txt` & `botocore-a-la-carte-dlm-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dlm-1.34.86/PKG-INFO` & `botocore-a-la-carte-dlm-1.34.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dlm
-Version: 1.34.86
+Version: 1.34.9
 Summary: dlm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/endpoint-rule-set-1.json` & `botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dlm-1.34.86/botocore/data/dlm/2018-01-12/service-2.json` & `botocore-a-la-carte-dlm-1.34.9/botocore/data/dlm/2018-01-12/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dlm-1.34.86/botocore_a_la_carte_dlm.egg-info/PKG-INFO` & `botocore-a-la-carte-dlm-1.34.9/botocore_a_la_carte_dlm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dlm
-Version: 1.34.86
+Version: 1.34.9
 Summary: dlm data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dlm-1.34.86/setup.py` & `botocore-a-la-carte-dlm-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-dlm',
-    version="1.34.86",
+    version="1.34.9",
     description='dlm data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/dlm/*/*.json'],
```

