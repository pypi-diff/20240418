# Comparing `tmp/mlpro-int-openml-0.1.0.tar.gz` & `tmp/mlpro_int_openml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-openml-0.1.0.tar", last modified: Tue Feb 20 05:32:42 2024, max compression
+gzip compressed data, was "mlpro_int_openml-1.0.0.tar", last modified: Thu Apr 18 17:21:58 2024, max compression
```

## Comparing `mlpro-int-openml-0.1.0.tar` & `mlpro_int_openml-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-20 05:32:42.656874 mlpro-int-openml-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/src/mlpro_int_openml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/src/mlpro_int_openml/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml/wrappers/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-20 05:32:42.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-20 05:32:42.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 05:32:42.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-20 05:32:42.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-20 05:32:42.000000 mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 05:32:42.652874 mlpro-int-openml-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-02-20 05:32:35.000000 mlpro-int-openml-0.1.0/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.070409 mlpro_int_openml-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/src/mlpro_int_openml/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/src/mlpro_int_openml/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml/wrappers/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 17:21:58.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-18 17:21:58.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:21:58.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 17:21:58.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 17:21:58.000000 mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:21:58.074410 mlpro_int_openml-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-18 17:21:54.000000 mlpro_int_openml-1.0.0/test/test_examples.py
```

### Comparing `mlpro-int-openml-0.1.0/LICENSE` & `mlpro_int_openml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-openml-0.1.0/PKG-INFO` & `mlpro_int_openml-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-openml
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration OpenML
 Home-page: https://mlpro-int-openml.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-openml.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-openml-0.1.0/README.md` & `mlpro_int_openml-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-openml-0.1.0/setup.cfg` & `mlpro_int_openml-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-openml
-version = 0.1.0
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration OpenML
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-openml.readthedocs.io
 project_urls =
```

### Comparing `mlpro-int-openml-0.1.0/src/mlpro_int_openml/wrappers/streams.py` & `mlpro_int_openml-1.0.0/src/mlpro_int_openml/wrappers/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 ## -- 2022-11-12  1.5.2     DA       Correction in method WrStreamOpenML._download()
 ## -- 2022-11-19  1.6.0     DA       Class WrStreamOpenML: 
 ## --                                - changes due to stream options
 ## --                                - method _get_string(): new parameter p_name
 ## -- 2022-12-09  1.6.1     DA       Bugfix: features/labels need to be added under their full name
 ## -- 2024-02-17  1.7.0     DA       Refactoring
 ## -- 2024-02-19  1.8.0     DA       Adaptation to new API >= v0.14.2
+## -- 2024-04-18  1.9.0     DA       Alignment with MLPro 1.4.0
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 1.8.0 (2024-02-19)
+Ver. 1.9.0 (2024-04-18)
 
 This module provides wrapper functionalities to incorporate public data sets of the OpenML ecosystem.
 
 Learn more: 
 
 https://docs.openml.org/APIs/
 
 """
 
 from mlpro.bf.various import ScientificObject, Log
 from mlpro.bf.ops import Mode
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 from mlpro.bf.streams import Feature, Label, Instance, StreamProvider, Stream
 from mlpro.bf.math import Element, MSpace
 
 import openml
```

### Comparing `mlpro-int-openml-0.1.0/src/mlpro_int_openml.egg-info/PKG-INFO` & `mlpro_int_openml-1.0.0/src/mlpro_int_openml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-openml
-Version: 0.1.0
+Version: 1.0.0
 Summary: MLPro: Integration OpenML
 Home-page: https://mlpro-int-openml.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-openml.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-openml-0.1.0/test/test_examples.py` & `mlpro_int_openml-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

