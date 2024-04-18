# Comparing `tmp/botocore-a-la-carte-comprehendmedical-1.34.85.tar.gz` & `tmp/botocore-a-la-carte-comprehendmedical-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-comprehendmedical-1.34.85.tar", last modified: Wed Apr 17 01:00:50 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-comprehendmedical-1.34.9.tar", last modified: Thu Dec 28 01:06:36 2023, max compression
```

## Comparing `botocore-a-la-carte-comprehendmedical-1.34.85.tar` & `botocore-a-la-carte-comprehendmedical-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.255576 botocore-a-la-carte-comprehendmedical-1.34.85/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 01:00:50.255576 botocore-a-la-carte-comprehendmedical-1.34.85/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.251576 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.251576 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.251576 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.251576 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/
--rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-04-17 01:00:41.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 01:00:41.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 01:00:41.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    92653 2024-04-17 01:00:41.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:50.255576 botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:00:50.255576 botocore-a-la-carte-comprehendmedical-1.34.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-17 01:00:50.000000 botocore-a-la-carte-comprehendmedical-1.34.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.522239 botocore-a-la-carte-comprehendmedical-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2023-12-28 01:06:26.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92653 2023-12-28 01:06:26.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:36.518239 botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:36.522239 botocore-a-la-carte-comprehendmedical-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-28 01:06:36.000000 botocore-a-la-carte-comprehendmedical-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/LICENSE.txt` & `botocore-a-la-carte-comprehendmedical-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/PKG-INFO` & `botocore-a-la-carte-comprehendmedical-1.34.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-comprehendmedical
-Version: 1.34.85
+Version: 1.34.9
 Summary: comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/botocore/data/comprehendmedical/2018-10-30/service-2.json` & `botocore-a-la-carte-comprehendmedical-1.34.9/botocore/data/comprehendmedical/2018-10-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO` & `botocore-a-la-carte-comprehendmedical-1.34.9/botocore_a_la_carte_comprehendmedical.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-comprehendmedical
-Version: 1.34.85
+Version: 1.34.9
 Summary: comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-comprehendmedical-1.34.85/setup.py` & `botocore-a-la-carte-comprehendmedical-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-comprehendmedical',
-    version="1.34.85",
+    version="1.34.9",
     description='comprehendmedical data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/comprehendmedical/*/*.json'],
```

