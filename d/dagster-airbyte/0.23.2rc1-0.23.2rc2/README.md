# Comparing `tmp/dagster-airbyte-0.23.2rc1.tar.gz` & `tmp/dagster-airbyte-0.23.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.23.2rc1.tar", last modified: Tue Apr 16 17:55:55 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.2rc2.tar", last modified: Tue Apr 16 20:38:04 2024, max compression
```

## Comparing `dagster-airbyte-0.23.2rc1.tar` & `dagster-airbyte-0.23.2rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.543754 dagster-airbyte-0.23.2rc1/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48304 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.547754 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.547754 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34862 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.543754 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1642 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.476281 dagster-airbyte-0.23.2rc2/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48304 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.480281 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.480281 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282784 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.476281 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/setup.py
```

### Comparing `dagster-airbyte-0.23.2rc1/LICENSE` & `dagster-airbyte-0.23.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/PKG-INFO` & `dagster-airbyte-0.23.2rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/types.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.2rc2/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc1/setup.py` & `dagster-airbyte-0.23.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc1",
+        "dagster==1.7.2rc2",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.23.2rc1",
+            "dagster-managed-elements==0.23.2rc2",
         ],
     },
 )
```

