# Comparing `tmp/mlpro_int_hyperopt-0.1.4.tar.gz` & `tmp/mlpro_int_hyperopt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro_int_hyperopt-0.1.4.tar", last modified: Mon Feb 19 15:50:51 2024, max compression
+gzip compressed data, was "mlpro_int_hyperopt-1.0.0.tar", last modified: Thu Apr 18 15:43:42 2024, max compression
```

## Comparing `mlpro_int_hyperopt-0.1.4.tar` & `mlpro_int_hyperopt-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.463162 mlpro_int_hyperopt-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.463162 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/wrappers/hyperopt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-19 15:50:51.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-19 15:50:51.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:50:51.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-19 15:50:51.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-19 15:50:51.000000 mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:50:51.467162 mlpro_int_hyperopt-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-02-19 15:50:44.000000 mlpro_int_hyperopt-0.1.4/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.879159 mlpro_int_hyperopt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 15:43:42.879159 mlpro_int_hyperopt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-18 15:43:42.879159 mlpro_int_hyperopt-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.875159 mlpro_int_hyperopt-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.875159 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.875159 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/wrappers/hyperopt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.879159 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 15:43:42.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 15:43:42.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:43:42.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 15:43:42.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 15:43:42.000000 mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:43:42.875159 mlpro_int_hyperopt-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-18 15:43:34.000000 mlpro_int_hyperopt-1.0.0/test/test_examples.py
```

### Comparing `mlpro_int_hyperopt-0.1.4/LICENSE` & `mlpro_int_hyperopt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro_int_hyperopt-0.1.4/PKG-INFO` & `mlpro_int_hyperopt-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: mlpro_int_hyperopt
-Version: 0.1.4
+Version: 1.0.0
 Summary: MLPro: Integration Hyperopt
 Home-page: https://mlpro-int-hyperopt.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-hyperopt.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: dill>=0.3.6; extra == "full"
-Requires-Dist: numpy>=1.24.2; extra == "full"
-Requires-Dist: matplotlib>=3.7.1; extra == "full"
-Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: mlpro[full]>=1.3.0; extra == "full"
-Requires-Dist: optuna>=3.1.1; extra == "full"
-Requires-Dist: pandas; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: hyperopt>=0.2.7; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Hyperopt/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Hyperopt/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-hyperopt/badge/?version=latest)](https://mlpro-int-hyperopt.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-hyperopt.svg)](https://badge.fury.io/py/mlpro-int-hyperopt)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-hyperopt/mlpro-int-hyperopt/badges/version.svg)](https://anaconda.org/mlpro-int-hyperopt/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-hyperopt/mlpro-int-hyperopt?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-river/mlpro-int-hyperopt)
@@ -38,8 +33,8 @@
 Welcome to MLPro-Int-Hyperopt, an extension to MLPro to integrate the Hyperopt package. MLPro is a middleware framework for standardized machine learning in Python. It is developed by the South Westphalia University of Applied Sciences, Germany, and provides standards, templates, and processes for hybrid machine learning applications. Hyperopt, in turn, provides state-of-the-art algorithms for hyperparameter search and optimization.
 
 MLPro-Int-Hyperopt provides wrapper classes that enable the use of selected Hyperopt functionalities in your MLPro applications. The use of these wrappers is illustrated in numerous example programs.
 
 ### Learn more
 [MLPro - Machine Learning Professional](https://mlpro.readthedocs.io)   
 [MLPro-Int-Hyperopt - Integration of Hyperopt into MLPro](https://mlpro-int-hyperopt.readthedocs.io)   
-[Hyperopt: Distributed Asynchronous Hyper-parameter Optimization](https://hyperopt.github.io/hyperopt/)   
+[Hyperopt: Distributed Asynchronous Hyperparameter Optimization](https://hyperopt.github.io/hyperopt/)
```

### Comparing `mlpro_int_hyperopt-0.1.4/README.md` & `mlpro_int_hyperopt-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 Welcome to MLPro-Int-Hyperopt, an extension to MLPro to integrate the Hyperopt package. MLPro is a middleware framework for standardized machine learning in Python. It is developed by the South Westphalia University of Applied Sciences, Germany, and provides standards, templates, and processes for hybrid machine learning applications. Hyperopt, in turn, provides state-of-the-art algorithms for hyperparameter search and optimization.
 
 MLPro-Int-Hyperopt provides wrapper classes that enable the use of selected Hyperopt functionalities in your MLPro applications. The use of these wrappers is illustrated in numerous example programs.
 
 ### Learn more
 [MLPro - Machine Learning Professional](https://mlpro.readthedocs.io)   
 [MLPro-Int-Hyperopt - Integration of Hyperopt into MLPro](https://mlpro-int-hyperopt.readthedocs.io)   
-[Hyperopt: Distributed Asynchronous Hyper-parameter Optimization](https://hyperopt.github.io/hyperopt/)   
+[Hyperopt: Distributed Asynchronous Hyperparameter Optimization](https://hyperopt.github.io/hyperopt/)
```

### Comparing `mlpro_int_hyperopt-0.1.4/setup.cfg` & `mlpro_int_hyperopt-1.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro_int_hyperopt
-version = 0.1.4
+version = 1.0.0
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration Hyperopt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-hyperopt.readthedocs.io
 project_urls = 
@@ -22,19 +22,14 @@
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
-	dill >= 0.3.6
-	numpy >= 1.24.2
-	matplotlib >= 3.7.1
-	multiprocess >= 0.70.14
-	mlpro[full] >= 1.3.0
-	optuna >= 3.1.1
-	pandas
+	mlpro[full] >= 1.4.0
+	hyperopt >= 0.2.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt/wrappers/hyperopt.py` & `mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt/wrappers/hyperopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 ## -- 2022-03-02  1.0.5     SY       Refactoring
 ## -- 2022-03-24  1.0.6     SY       Refactoring
 ## -- 2022-03-25  1.0.7     SY       Change methods names (SetupSpaces to setup_spaces)
 ## -- 2022-08-14  1.1.0     DA       Introduction of root class Wrapper
 ## -- 2022-10-17  1.1.1     SY       Refactoring due to unit test
 ## -- 2023-04-12  1.1.2     SY       Refactoring
 ## -- 2024-02-01  2.0.0     LSB      Migrated to the new repository
+## -- 2024-04-18  2.1.0     DA       Assignment with MLPro v1.4.0
 ## -------------------------------------------------------------------------------------------------
 
 """
-Ver. 2.0.0 (2024-02-01)
+Ver. 2.1.0 (2024-04-18)
 
 This module provides a wrapper class for hyperparameter tuning by reusing the Hyperopt framework.
 
 See also: https://pypi.org/project/hyperopt/
 
 """
 
 from hyperopt import *
-from mlpro.wrappers.models import Wrapper
+from mlpro.wrappers import Wrapper
 from mlpro.bf.ml import *
 from mlpro.bf.math import *
 from mlpro.bf.various import *
 from mlpro.rl.models import *
 from mlpro.gt.dynamicgames import *
 import os
```

### Comparing `mlpro_int_hyperopt-0.1.4/src/mlpro_int_hyperopt.egg-info/PKG-INFO` & `mlpro_int_hyperopt-1.0.0/src/mlpro_int_hyperopt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: mlpro_int_hyperopt
-Version: 0.1.4
+Version: 1.0.0
 Summary: MLPro: Integration Hyperopt
 Home-page: https://mlpro-int-hyperopt.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-hyperopt.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: full
-Requires-Dist: dill>=0.3.6; extra == "full"
-Requires-Dist: numpy>=1.24.2; extra == "full"
-Requires-Dist: matplotlib>=3.7.1; extra == "full"
-Requires-Dist: multiprocess>=0.70.14; extra == "full"
-Requires-Dist: mlpro[full]>=1.3.0; extra == "full"
-Requires-Dist: optuna>=3.1.1; extra == "full"
-Requires-Dist: pandas; extra == "full"
+Requires-Dist: mlpro[full]>=1.4.0; extra == "full"
+Requires-Dist: hyperopt>=0.2.7; extra == "full"
 
 [![CI](https://github.com/fhswf/MLPro-Int-Hyperopt/actions/workflows/ci.yml/badge.svg)](https://github.com/fhswf/MLPro-Int-Hyperopt/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/mlpro-int-hyperopt/badge/?version=latest)](https://mlpro-int-hyperopt.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/mlpro-int-hyperopt.svg)](https://badge.fury.io/py/mlpro-int-hyperopt)
 <!---
 [![Anaconda-Version Badge](https://anaconda.org/mlpro-int-hyperopt/mlpro-int-hyperopt/badges/version.svg)](https://anaconda.org/mlpro-int-hyperopt/mlpro)
 [![Anaconda-Downloads Badge](https://img.shields.io/conda/dn/mlpro-int-hyperopt/mlpro-int-hyperopt?color=green&label=Anaconda.org%20Total%20downloads&style=flat-square)](https://anaconda.org/mlpro-int-river/mlpro-int-hyperopt)
@@ -38,8 +33,8 @@
 Welcome to MLPro-Int-Hyperopt, an extension to MLPro to integrate the Hyperopt package. MLPro is a middleware framework for standardized machine learning in Python. It is developed by the South Westphalia University of Applied Sciences, Germany, and provides standards, templates, and processes for hybrid machine learning applications. Hyperopt, in turn, provides state-of-the-art algorithms for hyperparameter search and optimization.
 
 MLPro-Int-Hyperopt provides wrapper classes that enable the use of selected Hyperopt functionalities in your MLPro applications. The use of these wrappers is illustrated in numerous example programs.
 
 ### Learn more
 [MLPro - Machine Learning Professional](https://mlpro.readthedocs.io)   
 [MLPro-Int-Hyperopt - Integration of Hyperopt into MLPro](https://mlpro-int-hyperopt.readthedocs.io)   
-[Hyperopt: Distributed Asynchronous Hyper-parameter Optimization](https://hyperopt.github.io/hyperopt/)   
+[Hyperopt: Distributed Asynchronous Hyperparameter Optimization](https://hyperopt.github.io/hyperopt/)
```

### Comparing `mlpro_int_hyperopt-0.1.4/test/test_examples.py` & `mlpro_int_hyperopt-1.0.0/test/test_examples.py`

 * *Files identical despite different names*

