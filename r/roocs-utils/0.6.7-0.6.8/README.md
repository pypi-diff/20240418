# Comparing `tmp/roocs_utils-0.6.7.tar.gz` & `tmp/roocs_utils-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roocs_utils-0.6.7.tar", last modified: Mon Feb  5 16:51:21 2024, max compression
+gzip compressed data, was "roocs_utils-0.6.8.tar", last modified: Thu Apr 18 12:00:41 2024, max compression
```

## Comparing `roocs_utils-0.6.7.tar` & `roocs_utils-0.6.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.587850 roocs_utils-0.6.7/
--rw-r--r--   0 pingu      (501) staff       (20)      399 2024-02-05 15:21:28.000000 roocs_utils-0.6.7/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     3579 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/CONTRIBUTING.rst
--rw-r--r--   0 pingu      (501) staff       (20)     9469 2024-02-05 16:50:36.000000 roocs_utils-0.6.7/HISTORY.rst
--rw-r--r--   0 pingu      (501) staff       (20)     1519 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/LICENSE
--rw-r--r--   0 pingu      (501) staff       (20)      180 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     2260 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/MakeFile
--rw-r--r--   0 pingu      (501) staff       (20)     3236 2024-02-05 16:51:21.587581 roocs_utils-0.6.7/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)      928 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/README.rst
--rw-r--r--   0 pingu      (501) staff       (20)      210 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      140 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/requirements_dev.txt
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.558552 roocs_utils-0.6.7/roocs_utils/
--rw-r--r--   0 pingu      (501) staff       (20)      619 2024-02-05 16:50:36.000000 roocs_utils-0.6.7/roocs_utils/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)      679 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/cli.py
--rw-r--r--   0 pingu      (501) staff       (20)     4153 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/config.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.563992 roocs_utils-0.6.7/roocs_utils/etc/
--rw-r--r--   0 pingu      (501) staff       (20)     8437 2024-02-05 15:21:28.000000 roocs_utils-0.6.7/roocs_utils/etc/roocs.ini
--rw-r--r--   0 pingu      (501) staff       (20)      567 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/exceptions.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.577550 roocs_utils-0.6.7/roocs_utils/parameter/
--rw-r--r--   0 pingu      (501) staff       (20)      221 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/parameter/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     1775 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/area_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     2919 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/base_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     1806 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/collection_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     1780 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/dimension_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     2165 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/level_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     5320 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/param_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)     1449 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/parameterise.py
--rw-r--r--   0 pingu      (501) staff       (20)     2297 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/time_components_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)     2871 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/parameter/time_parameter.py
--rw-r--r--   0 pingu      (501) staff       (20)    11011 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/project_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.581422 roocs_utils-0.6.7/roocs_utils/utils/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/utils/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)      516 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/utils/common.py
--rw-r--r--   0 pingu      (501) staff       (20)     2138 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/utils/file_utils.py
--rw-r--r--   0 pingu      (501) staff       (20)     4024 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/utils/time_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.582815 roocs_utils-0.6.7/roocs_utils/xarray_utils/
--rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-07 12:53:44.000000 roocs_utils-0.6.7/roocs_utils/xarray_utils/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)    11518 2024-02-02 15:39:40.000000 roocs_utils-0.6.7/roocs_utils/xarray_utils/xarray_utils.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.585282 roocs_utils-0.6.7/roocs_utils.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     3236 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1169 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)       53 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/entry_points.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2024-01-19 14:08:24.000000 roocs_utils-0.6.7/roocs_utils.egg-info/not-zip-safe
--rw-r--r--   0 pingu      (501) staff       (20)      308 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       12 2024-02-05 16:51:21.000000 roocs_utils-0.6.7/roocs_utils.egg-info/top_level.txt
--rw-r--r--   0 pingu      (501) staff       (20)      952 2024-02-05 16:51:21.589007 roocs_utils-0.6.7/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     3388 2024-02-05 16:50:36.000000 roocs_utils-0.6.7/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-02-05 16:51:21.583884 roocs_utils-0.6.7/tests/
--rw-r--r--   0 pingu      (501) staff       (20)    11703 2024-02-05 15:21:28.000000 roocs_utils-0.6.7/tests/test_project_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.983962 roocs_utils-0.6.8/
+-rw-r--r--   0 pingu      (501) staff       (20)      399 2024-02-05 15:21:28.000000 roocs_utils-0.6.8/AUTHORS.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     3579 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/CONTRIBUTING.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     9586 2024-04-18 11:59:32.000000 roocs_utils-0.6.8/HISTORY.rst
+-rw-r--r--   0 pingu      (501) staff       (20)     1519 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/LICENSE
+-rw-r--r--   0 pingu      (501) staff       (20)      180 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/MANIFEST.in
+-rw-r--r--   0 pingu      (501) staff       (20)     2260 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/MakeFile
+-rw-r--r--   0 pingu      (501) staff       (20)     3236 2024-04-18 12:00:41.983657 roocs_utils-0.6.8/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)      928 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/README.rst
+-rw-r--r--   0 pingu      (501) staff       (20)      210 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/requirements.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      140 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/requirements_dev.txt
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.948968 roocs_utils-0.6.8/roocs_utils/
+-rw-r--r--   0 pingu      (501) staff       (20)      561 2024-04-18 11:59:32.000000 roocs_utils-0.6.8/roocs_utils/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)      679 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/cli.py
+-rw-r--r--   0 pingu      (501) staff       (20)     4153 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/config.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.956028 roocs_utils-0.6.8/roocs_utils/etc/
+-rw-r--r--   0 pingu      (501) staff       (20)     8437 2024-02-05 15:21:28.000000 roocs_utils-0.6.8/roocs_utils/etc/roocs.ini
+-rw-r--r--   0 pingu      (501) staff       (20)      567 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/exceptions.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.972379 roocs_utils-0.6.8/roocs_utils/parameter/
+-rw-r--r--   0 pingu      (501) staff       (20)      221 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/parameter/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1775 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/area_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2919 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/base_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1806 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/collection_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1780 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/dimension_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2165 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/level_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     5320 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/param_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)     1449 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/parameterise.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2297 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/time_components_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2871 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/parameter/time_parameter.py
+-rw-r--r--   0 pingu      (501) staff       (20)    11011 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/project_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.976813 roocs_utils-0.6.8/roocs_utils/utils/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/utils/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)      516 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/utils/common.py
+-rw-r--r--   0 pingu      (501) staff       (20)     2138 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/utils/file_utils.py
+-rw-r--r--   0 pingu      (501) staff       (20)     4024 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/utils/time_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.978770 roocs_utils-0.6.8/roocs_utils/xarray_utils/
+-rw-r--r--   0 pingu      (501) staff       (20)        0 2023-11-07 12:53:44.000000 roocs_utils-0.6.8/roocs_utils/xarray_utils/__init__.py
+-rw-r--r--   0 pingu      (501) staff       (20)    11518 2024-02-02 15:39:40.000000 roocs_utils-0.6.8/roocs_utils/xarray_utils/xarray_utils.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.980920 roocs_utils-0.6.8/roocs_utils.egg-info/
+-rw-r--r--   0 pingu      (501) staff       (20)     3236 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 pingu      (501) staff       (20)     1169 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       53 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/entry_points.txt
+-rw-r--r--   0 pingu      (501) staff       (20)        1 2024-01-19 14:08:24.000000 roocs_utils-0.6.8/roocs_utils.egg-info/not-zip-safe
+-rw-r--r--   0 pingu      (501) staff       (20)      308 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/requires.txt
+-rw-r--r--   0 pingu      (501) staff       (20)       12 2024-04-18 12:00:41.000000 roocs_utils-0.6.8/roocs_utils.egg-info/top_level.txt
+-rw-r--r--   0 pingu      (501) staff       (20)      952 2024-04-18 12:00:41.985048 roocs_utils-0.6.8/setup.cfg
+-rw-r--r--   0 pingu      (501) staff       (20)     3388 2024-04-18 11:59:32.000000 roocs_utils-0.6.8/setup.py
+drwxr-xr-x   0 pingu      (501) staff       (20)        0 2024-04-18 12:00:41.979916 roocs_utils-0.6.8/tests/
+-rw-r--r--   0 pingu      (501) staff       (20)    11703 2024-02-05 15:21:28.000000 roocs_utils-0.6.8/tests/test_project_utils.py
```

### Comparing `roocs_utils-0.6.7/CONTRIBUTING.rst` & `roocs_utils-0.6.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/HISTORY.rst` & `roocs_utils-0.6.8/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 Next
 ----
 
 * ...
 
 
+v0.6.8 (2024.04.17)
+-------------------
+
+Other Changes
+^^^^^^^^^^^^^
+* Fixed logging and updated conda env (#115).
+
+
 v0.6.7 (2024.02.05)
 -------------------
 
 Other Changes
 ^^^^^^^^^^^^^
 * Updated `roocs.ini` default values for atlas datasets for further methods of how to infer the project name (#113).
```

### Comparing `roocs_utils-0.6.7/LICENSE` & `roocs_utils-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/MakeFile` & `roocs_utils-0.6.8/MakeFile`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/PKG-INFO` & `roocs_utils-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roocs_utils
-Version: 0.6.7
+Version: 0.6.8
 Summary: A package containing common components for the roocs project
 Home-page: https://github.com/roocs/roocs-utils
 Author: Elle Smith
 Author-email: eleanor.smith@stfc.ac.uk
 License: BSD - see LICENSE file in top-level package directory
 Keywords: roocs_utils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `roocs_utils-0.6.7/README.rst` & `roocs_utils-0.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/__init__.py` & `roocs_utils-0.6.8/roocs_utils/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """Top-level package for roocs-utils."""
 
 __author__ = """Eleanor Smith"""
 __contact__ = "eleanor.smith@stfc.ac.uk"
 __copyright__ = "Copyright 2018 United Kingdom Research and Innovation"
 __license__ = "BSD - see LICENSE file in top-level package directory"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 
 from roocs_utils.config import get_config
 import roocs_utils
 
 CONFIG = get_config()
 
 from .parameter import *
 from .xarray_utils import *
 from .utils import *
 
 import logging
 import os
 
 
-LOG_LEVEL = "INFO"
-logging.basicConfig(level=LOG_LEVEL)
-
-
 for env_var, value in CONFIG["environment"].items():
     os.environ[env_var.upper()] = value
```

### Comparing `roocs_utils-0.6.7/roocs_utils/cli.py` & `roocs_utils-0.6.8/roocs_utils/cli.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/config.py` & `roocs_utils-0.6.8/roocs_utils/config.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/etc/roocs.ini` & `roocs_utils-0.6.8/roocs_utils/etc/roocs.ini`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/exceptions.py` & `roocs_utils-0.6.8/roocs_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/area_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/area_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/base_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/base_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/collection_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/collection_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/dimension_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/dimension_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/level_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/level_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/param_utils.py` & `roocs_utils-0.6.8/roocs_utils/parameter/param_utils.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/parameterise.py` & `roocs_utils-0.6.8/roocs_utils/parameter/parameterise.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/time_components_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/time_components_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/parameter/time_parameter.py` & `roocs_utils-0.6.8/roocs_utils/parameter/time_parameter.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/project_utils.py` & `roocs_utils-0.6.8/roocs_utils/project_utils.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/utils/common.py` & `roocs_utils-0.6.8/roocs_utils/utils/common.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/utils/file_utils.py` & `roocs_utils-0.6.8/roocs_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/utils/time_utils.py` & `roocs_utils-0.6.8/roocs_utils/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils/xarray_utils/xarray_utils.py` & `roocs_utils-0.6.8/roocs_utils/xarray_utils/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/roocs_utils.egg-info/PKG-INFO` & `roocs_utils-0.6.8/roocs_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roocs_utils
-Version: 0.6.7
+Version: 0.6.8
 Summary: A package containing common components for the roocs project
 Home-page: https://github.com/roocs/roocs-utils
 Author: Elle Smith
 Author-email: eleanor.smith@stfc.ac.uk
 License: BSD - see LICENSE file in top-level package directory
 Keywords: roocs_utils
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `roocs_utils-0.6.7/roocs_utils.egg-info/SOURCES.txt` & `roocs_utils-0.6.8/roocs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roocs_utils-0.6.7/setup.cfg` & `roocs_utils-0.6.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.7
+current_version = 0.6.8
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `roocs_utils-0.6.7/setup.py` & `roocs_utils-0.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """The setup script."""
 
 __author__ = "Elle Smith"
 __contact__ = "eleanor.smith@stfc.ac.uk"
 __copyright__ = "Copyright 2018 United Kingdom Research and Innovation"
 __license__ = "BSD - see LICENSE file in top-level package directory"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 
 from setuptools import find_packages
 from setuptools import setup
 import os
 
 # One strategy for storing the overall version is to put it in the top-level
 # package's __init__ but Nb. __init__.py files are not needed to declare
```

### Comparing `roocs_utils-0.6.7/tests/test_project_utils.py` & `roocs_utils-0.6.8/tests/test_project_utils.py`

 * *Files identical despite different names*

