# Comparing `tmp/dojo_ds-1.0.9.tar.gz` & `tmp/dojo_ds-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-1.0.9.tar", last modified: Thu Jan 25 23:20:12 2024, max compression
+gzip compressed data, was "dojo_ds-1.1.0.tar", last modified: Thu Apr 18 19:31:10 2024, max compression
```

## Comparing `dojo_ds-1.0.9.tar` & `dojo_ds-1.1.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.484831 dojo_ds-1.0.9/
--rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.0.9/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.0.9/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1634 2024-01-25 23:20:12.484399 dojo_ds-1.0.9/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.0.9/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.468734 dojo_ds-1.0.9/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.0.9/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/docs/authors.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.455106 dojo_ds-1.0.9/docs/build/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.455237 dojo_ds-1.0.9/docs/build/html/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.470534 dojo_ds-1.0.9/docs/build/html/_static/
--rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.0.9/docs/build/html/_static/file.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.0.9/docs/build/html/_static/minus.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.0.9/docs/build/html/_static/plus.png
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.0.9/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.0.9/docs/dojo_ds.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.0.9/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.0.9/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.0.9/docs/modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.0.9/docs/old_modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.0.9/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.478948 dojo_ds-1.0.9/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      828 2024-01-25 23:20:05.000000 dojo_ds-1.0.9/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     2679 2024-01-23 23:41:04.000000 dojo_ds-1.0.9/dojo_ds/_eda_functions_plotly.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.0.9/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4280 2024-01-23 21:15:53.000000 dojo_ds-1.0.9/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     1156 2024-01-23 02:06:05.000000 dojo_ds-1.0.9/dojo_ds/deploy.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    12374 2024-01-25 20:20:52.000000 dojo_ds-1.0.9/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    24120 2024-01-25 23:19:45.000000 dojo_ds-1.0.9/dojo_ds/evaluate.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.0.9/dojo_ds/imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    13820 2024-01-23 23:45:17.000000 dojo_ds-1.0.9/dojo_ds/insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.0.9/dojo_ds/matplotlib_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    49726 2024-01-23 02:08:00.000000 dojo_ds-1.0.9/dojo_ds/nlp.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    18674 2023-11-16 17:38:00.000000 dojo_ds-1.0.9/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.483304 dojo_ds-1.0.9/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1634 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      915 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.0.9/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)       79 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-01-25 23:20:12.000000 dojo_ds-1.0.9/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-01-25 23:20:12.485893 dojo_ds-1.0.9/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     1731 2024-01-25 23:20:05.000000 dojo_ds-1.0.9/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-01-25 23:20:12.482843 dojo_ds-1.0.9/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.0.9/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.0.9/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.167366 dojo_ds-1.1.0/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.0/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.0/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:31:10.167244 dojo_ds-1.1.0/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.0/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.137885 dojo_ds-1.1.0/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.0/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/authors.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.117506 dojo_ds-1.1.0/docs/build/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.117615 dojo_ds-1.1.0/docs/build/html/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.139650 dojo_ds-1.1.0/docs/build/html/_static/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/file.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/plus.png
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.0/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.0/docs/dojo_ds.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.0/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.0/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.0/docs/modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.0/docs/old_modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.0/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.157917 dojo_ds-1.1.0/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 19:24:42.000000 dojo_ds-1.1.0/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.0/dojo_ds/_eda_functions_plotly.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.0/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.0/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.0/dojo_ds/deploy.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.0/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.0/dojo_ds/evaluate.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.0/dojo_ds/imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.0/dojo_ds/insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.0/dojo_ds/matplotlib_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.0/dojo_ds/nlp.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     8861 2024-04-18 19:20:54.000000 dojo_ds-1.1.0/dojo_ds/time_series.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.0/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.166797 dojo_ds-1.1.0/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)      104 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 19:31:10.167792 dojo_ds-1.1.0/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 19:30:18.000000 dojo_ds-1.1.0/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.166427 dojo_ds-1.1.0/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.0/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-1.0.9/CONTRIBUTING.rst` & `dojo_ds-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/LICENSE` & `dojo_ds-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/PKG-INFO` & `dojo_ds-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.0.9
+Version: 1.1.0
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Click>=7.0
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
+Requires-Dist: statsmodels>=0.13.5
+Requires-Dist: pmdarima==2.0.4
 
 =======
 dojo-ds
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/dojo_ds.svg
```

### Comparing `dojo_ds-1.0.9/README.rst` & `dojo_ds-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/docs/Makefile` & `dojo_ds-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/docs/conf.py` & `dojo_ds-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/docs/dojo_ds.rst` & `dojo_ds-1.1.0/docs/dojo_ds.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/docs/installation.rst` & `dojo_ds-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/docs/make.bat` & `dojo_ds-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.0.9/dojo_ds/__init__.py` & `dojo_ds-1.1.0/dojo_ds/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 """
 Custom Functions the Data Science Program
 __author__ = James Irving, Brenda Hungerford
 """
 __author__ = """James Irving"""
 __email__ = 'james.irving.phd@gmail.com'
-__version__ = '1.0.9'
+__version__ = '1.1.0'
 from . import data_enrichment as data
 from . import eda 
 from . import evaluate
 from . import insights 
 from . import nlp
+from . import time_series
 
 # from . import deployment_functions as deploy
 
 from . import utils as utils
 
 
 # from . import _eda_functions_plotly as eda_plotly
 
 def show_code(function):
-	"""Uses inspect modulem to retrieve source code for function.
-	Displays as pthon-syntax Markdown code.
-	
-	Note: Python highlighting doesn't work correctly on VS Code or Google Colab
+	"""
+	Uses the inspect module to retrieve the source code for a function.
+	Displays the code as Python-syntax Markdown code.
+
+	Note: Python highlighting may not work correctly on some editors.
+
+	Parameters:
+	function (callable): The function for which to display the source code.
+
+	Returns:
+	None
 	"""
 	import inspect
 	from IPython.display import display, Markdown
+
 	code = inspect.getsource(function)
 	md = "```python" +'\n' + code + "\n" + '```' 
 	display(Markdown(md))
```

### Comparing `dojo_ds-1.0.9/dojo_ds/data_enrichment.py` & `dojo_ds-1.1.0/dojo_ds/data_enrichment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .evaluate import evaluate_ols, plot_residuals
 def find_outliers_Z(data, verbose=True):
-    """Find outliers based on Z-score rule (outliers have an absolute z-score that is >3)
+    """
+    Find outliers based on Z-score rule (outliers have an absolute z-score that is >3)
 
     Args:
         data (Series): Pandas Series
         verbose (bool, optional): Print summary info about outliers. Defaults to True.
 
     Returns:
         Series: Boolean index for input data, where True = Outlier
@@ -20,109 +21,116 @@
         print(f"- {outliers.sum():,} outliers found in {data.name} out of {n:,} rows ({outliers.sum()/n*100:.2f}%) using Z-scores.")
 
     outliers = pd.Series(outliers, index=data.index, name=data.name)
     return outliers
 
 
 def find_outliers_IQR(data, verbose=True):
-    """Find outliers based on IQR-rule (outliers are either 1.5 x IQR below 25% quantile and 1.5xIQR above 75% quantile.
-    
-    # Calculate q1 and q3 quantiles
-    q3 = np.quantile(data,.75)
-    q1 = np.quantile(data,.25)
-    # Calculate IQR 
-    IQR = q3 - q1
-    
-    # Set thresholds more than 1.5x IQR above Q3/below Q1
-    upper_threshold = q3 + 1.5*IQR
-    lower_threshold = q1 - 1.5*IQR
+    """
+    Find outliers based on IQR-rule (outliers are either 1.5 x IQR below 25% quantile and 1.5xIQR above 75% quantile).
     
     Args:
-        data (Series): Pandas Series
-        verbose (bool, optional): Print summary info about outliers. Defaults to True.
-
+        data (Series): Pandas Series containing the data.
+        verbose (bool, optional): If True, print summary information about outliers. Defaults to True.
+    
     Returns:
-        Series: Boolean index for input data, where True = Outlier
+        Series: Boolean index for input data, where True indicates an outlier.
     """
     import pandas as pd
     import numpy as np
-    q3 = np.quantile(data,.75)
-    q1 = np.quantile(data,.25)
-
+    
+    # Calculate q1 and q3 quantiles
+    q3 = np.quantile(data, .75)
+    q1 = np.quantile(data, .25)
+    
+    # Calculate IQR 
     IQR = q3 - q1
-    upper_threshold = q3 + 1.5*IQR
-    lower_threshold = q1 - 1.5*IQR
     
-    outliers = (data<lower_threshold) | (data>upper_threshold)
+    # Set thresholds more than 1.5x IQR above Q3/below Q1
+    upper_threshold = q3 + 1.5 * IQR
+    lower_threshold = q1 - 1.5 * IQR
+    
+    # Identify outliers
+    outliers = (data < lower_threshold) | (data > upper_threshold)
+    
     if verbose:
         n = len(outliers)
+        print(f"- {outliers.sum():,} outliers found in {data.name} out of {n:,} rows ({outliers.sum() / n * 100:.2f}%) using IQR.")
     
-    
-        print(f"- {outliers.sum():,} outliers found in {data.name} out of {n:,} rows ({outliers.sum()/n*100:.2f}%) using IQR.")
-        
     outliers = pd.Series(outliers, index=data.index, name=data.name)
     return outliers
 
 
 
 
-def remove_outliers(df_,method='iqr', subset=None, verbose=2):
-    """Returns a copy of the input df with outleirs removed from all
-    columns using the selected method (either 'iqr' or 'z'/'zscore')
-    
-    Arguments:
-        df_ (Frame): Dataframe to copy and remove outleirs from
-        method (str): Method of outlier removal. Options are 'iqr' or 'z' (default is 'iqr')
-        subset (list or None): List of column names to remove outliers from. If None, uses all numeric columns.
-        verbose (bool, int): If verbose==1, print only overall summary. If verbose==2, print detailed summary"""
+def remove_outliers(df_, method='iqr', subset=None, verbose=2):
+    """Returns a copy of the input dataframe with outliers removed from selected columns using the specified method.
+
+    Args:
+        df_ (DataFrame): The input dataframe to copy and remove outliers from.
+        method (str): The method of outlier removal. Options are 'iqr' or 'z'/'zscore'. Default is 'iqr'.
+        subset (list or None): A list of column names to remove outliers from. If None, all numeric columns are used. Default is None.
+        verbose (bool, int): If verbose==1, print only the overall summary. If verbose==2, print the detailed summary. Default is 2.
+
+    Returns:
+        DataFrame: A copy of the input dataframe with outliers removed.
+
+    Raises:
+        Exception: If the method is not 'iqr' or 'z'.
+
+    Examples:
+        >>> df = pd.DataFrame({'A': [1, 2, 3, 4, 5], 'B': [10, 20, 30, 40, 50]})
+        >>> remove_outliers(df, method='iqr', subset=['A'], verbose=2)
+        Returns a dataframe with outliers removed from column 'A' using the IQR rule.
+    """
     import pandas as pd
-    ## Make a cope of input dataframe  
+    ## Make a copy of the input dataframe  
     df = df_.copy()
     
-    ## Set verbose_func for calls to outleir funcs
-    if verbose==2:
+    ## Set verbose_func for calls to outlier funcs
+    if verbose == 2:
         verbose_func = True
     else:
-        verbose_func=False
+        verbose_func = False
         
     ## Set outlier removal function and name
-    if method.lower()=='iqr':
+    if method.lower() == 'iqr':
         find_outlier_func = find_outliers_IQR
         method_name = "IQR rule"
     elif 'z' in method.lower():
         find_outlier_func = find_outliers_Z
-        method_name = 'Z_score rule'
+        method_name = 'Z-score rule'
     else:
         raise Exception('[!] Method must be either "iqr" or "z".')
         
-    ## Set list of cols to remove outliers from
+    ## Set list of columns to remove outliers from
     if subset is None:
         col_list = df.select_dtypes('number').columns
-    elif isinstance(subset,str):
+    elif isinstance(subset, str):
         col_list = [subset]
     elif isinstance(subset, list):
         col_list = subset
     else:
         raise Exception("[!] subset must be None, a single string, or a list of strings.")
 
     
-    ## Empty dict for both types of outliers
+    ## Empty dictionary for both types of outliers
     outliers = {}
 
-    ## Use both functions to see the comparison for # of outliers
+    ## Use both functions to see the comparison for the number of outliers
     for col in col_list:
-        idx_outliers = find_outlier_func(df[col],verbose=verbose_func)
+        idx_outliers = find_outlier_func(df[col], verbose=verbose_func)
         outliers[col] = idx_outliers
 
     
-    ## Getting final df of all outliers to get 1 final T/F index
+    ## Getting final dataframe of all outliers to get 1 final T/F index
     outliers_combined = pd.DataFrame(outliers).any(axis=1)
     
     if verbose:
         n = len(outliers_combined)
-        print(f"\n[i] Overall, {outliers_combined.sum():,} rows out of {n:,}({outliers_combined.sum()/n*100:.2f}%) were removed as outliers using {method_name}.")
+        print(f"\n[i] Overall, {outliers_combined.sum():,} rows out of {n:,} ({outliers_combined.sum()/n*100:.2f}%) were removed as outliers using {method_name}.")
     
     
-    # remove_outliers 
+    # remove outliers 
     df_clean = df[~outliers_combined].copy()
     return df_clean
```

### Comparing `dojo_ds-1.0.9/dojo_ds/eda.py` & `dojo_ds-1.1.0/dojo_ds/eda.py`

 * *Files 5% similar despite different names*

```diff
@@ -299,33 +299,51 @@
       plt.show()
   return fig, axes
 
 
 
 ######### NEW
 def plot_correlation(df, cmap='coolwarm', cols=None):
-    if cols == None:
-        cols = df.columns
-    corr = df[cols].corr(numeric_only=True)
-
-    fig, ax = plt.subplots(figsize=(8,6))
-    sns.heatmap(corr, cmap=cmap, ax=ax, annot=True, center=0)
-    ax.set_title("Correlation Matrix")
-    return fig
+  """
+  Plots a correlation matrix heatmap for the given DataFrame.
+
+  Parameters:
+  df (DataFrame): The input DataFrame.
+  cmap (str, optional): The color map to use for the heatmap. Defaults to 'coolwarm'.
+  cols (list, optional): The columns to include in the correlation matrix. If None, all columns are included.
+
+  Returns:
+  fig (Figure): The matplotlib Figure object containing the correlation matrix heatmap.
+  """
+  if cols == None:
+    cols = df.columns
+  corr = df[cols].corr(numeric_only=True)
+
+  fig, ax = plt.subplots(figsize=(8,6))
+  sns.heatmap(corr, cmap=cmap, ax=ax, annot=True, center=0)
+  ax.set_title("Correlation Matrix")
+  return fig
 
 
 from ._eda_functions_plotly import *
 
 
 
 def annotate_regplot_equation(ax):
-  """Adapted from Source: https://www.statology.org/seaborn-regplot-equation/
+  """
+  Annotates a regression plot with the equation of the regression line.
+
+  Parameters:
+  ax (matplotlib.axes.Axes): The axes object containing the regression plot.
+
+  Adapted from Source: https://www.statology.org/seaborn-regplot-equation/
+
   Example Use:
   >> fig, ax = plot_numeric_vs_target(df, x="Living Area Sqft")
   >> annotate_regplot_equation(ax)
   """
   import scipy
   #calculate slope and intercept of regression equation
   slope, intercept, r, p, sterr = scipy.stats.linregress(x=ax.get_lines()[0].get_xdata(),
-                                                        y=ax.get_lines()[0].get_ydata())
+                            y=ax.get_lines()[0].get_ydata())
   eqn = f'y = {slope:,.2f} * X + {intercept:,.2f}'
   ax.legend(handles=[ax.get_lines()[0]], labels=[eqn])
```

### Comparing `dojo_ds-1.0.9/dojo_ds/evaluate.py` & `dojo_ds-1.1.0/dojo_ds/evaluate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 ## PREVIOUS CLASSIFICATION_METRICS FUNCTION FROM INTRO TO ML
-
 def classification_metrics(y_true, y_pred, label='',
                            output_dict=False, figsize=(8,4),
                            normalize='true', cmap='Blues',
                            colorbar=False, values_format=".2f",
                            target_names = None, return_fig=True):
-    """Calculate classification metrics from preditions and display Confusion matrix.
+    """
+    Calculate classification metrics from predictions and display Confusion matrix.
 
     Args:
         y_true (Series/array): True target values.
-        y_pred (Series/array): Predicted targe values.
-        label (str, optional): Label For Printed Header. Defaults to ''.
+        y_pred (Series/array): Predicted target values.
+        label (str, optional): Label for printed header. Defaults to ''.
         output_dict (bool, optional): Return the results of classification_report as a dict. Defaults to False.
         figsize (tuple, optional): figsize for confusion matrix subplots. Defaults to (8,4).
-        normalize (str, optional): arg for sklearn's ConfusionMatrixDisplay. Defaults to 'true' (conf mat values normalized to true class).
+        normalize (str, optional): Arg for sklearn's ConfusionMatrixDisplay. Defaults to 'true' (conf mat values normalized to true class).
         cmap (str, optional): Colormap for the ConfusionMatrixDisplay. Defaults to 'Blues'.
-        colorbar (bool, optional): Arg for ConfusionMatrixDispaly: include colorbar or not. Defaults to False.
+        colorbar (bool, optional): Arg for ConfusionMatrixDisplay: include colorbar or not. Defaults to False.
         values_format (str, optional): Format values on confusion matrix. Defaults to ".2f".
-        target_names (array, optional): Text labels for the integer-encoded target. Passed in numeric order [label for "0", label for "1", etc.]
-        return_fig (bool, optional): To get matplotlib figure for confusion matrix, set outout_dict to False and set return_fig to True.
+        target_names (array, optional): Text labels for the integer-encoded target. Passed in numeric order [label for "0", label for "1", etc.].
+        return_fig (bool, optional): To get matplotlib figure for confusion matrix, set output_dict to False and set return_fig to True.
 
-    Returns (Only 1 value is returned):
+    Returns:
         dict: Dictionary from classification_report. Only returned if output_dict=True.
-        fig: Matplotlib figure with confusion matrix. Only returned if output_dict=False and return_fig=True
-        
-            
+        fig: Matplotlib figure with confusion matrix. Only returned if output_dict=False and return_fig=True.
+
     Note: 
-        This is a modified version of classification metrics function from Intro to Machine Learning.
+        This is a modified version of the classification metrics function from Intro to Machine Learning.
         Updates:
-          - Reversed raw counts confusion matrix cmap  (so darker==more).
-          - Added arg for normalized confusion matrix values_format
-    
+          - Reversed raw counts confusion matrix cmap (so darker==more).
+          - Added arg for normalized confusion matrix values_format.
     """
     from sklearn.metrics import classification_report, ConfusionMatrixDisplay
     import matplotlib.pyplot as plt
     import numpy as np
     # Get the classification report
     report = classification_report(y_true, y_pred,target_names=target_names)
     
@@ -42,15 +40,15 @@
     header = "-"*70
     print(header, f" Classification Metrics: {label}", header, sep='\n')
     print(report)
     
     ## CONFUSION MATRICES SUBPLOTS
     fig, axes = plt.subplots(ncols=2, figsize=figsize)
     
-    # Create a confusion matrix  of raw counts (left subplot)
+    # Create a confusion matrix of raw counts (left subplot)
     ConfusionMatrixDisplay.from_predictions(y_true, y_pred,
                                             normalize=None, 
                                             cmap='gist_gray_r',# Updated cmap
                                             values_format="d", 
                                             colorbar=colorbar,
                                             ax = axes[0], 
                                             display_labels=target_names);
@@ -75,14 +73,15 @@
         report_dict = classification_report(y_true, y_pred,target_names=target_names, output_dict=True)
         return report_dict
 
     elif return_fig == True:
         return fig
     
     
+    
 def evaluate_classification(model, X_train=None, y_train=None, X_test=None, y_test=None,
                             figsize=(6,4), normalize='true', output_dict = False,
                             cmap_train='Blues', cmap_test="Reds",colorbar=False,
                             values_format='.2f',
                             target_names=None, return_fig=False):
     """Evalutes an sklearn-compatible classification model on training and test data. 
     For each data split, return the classification report and confusion matrix display. 
@@ -99,22 +98,19 @@
         cmap_train (str, optional): Colormap for the ConfusionMatrixDisplay for training data. Defaults to 'Blues'.
         cmap_test (str, optional): Colormap for the ConfusionMatrixDisplay for test data.  Defaults to "Reds".
         colorbar (bool, optional): Arg for ConfusionMatrixDispaly: include colorbar or not. Defaults to False.
         values_format (str, optional): Format values on confusion matrix. Defaults to ".2f".
         target_names (array, optional): Text labels for the integer-encoded target. Passed in numeric order [label for "0", label for "1", etc.]
         return_fig (bool, optional): Whether the matplotlib figure for confusion matrix is returned. Defaults to False.
                                           Note: Must set outout_dict to False and set return_fig to True to get figure returned.
-
-
      Returns (Only 1 value is returned, but contents vary):
         dict: Dictionary that contains results for "train" and "test. 
               Contents of dictionary depending on output_dict and return_fig:
               - if output_dict==True and return_fig==False: returns dictionary of classification report results
             - if output_dict==False and return_fig==True: returns dictionary of confusion matrix displays.
-
     """
     # Combining arguments used for both training and test results
     shared_kwargs = dict(output_dict=output_dict,  # output_dict: Changed from hard-coded True
                     #   figsize=figsize, 
                       colorbar=colorbar, 
                       target_names=target_names,
                       values_format=values_format,
@@ -261,21 +257,24 @@
         results_dict = {'train':results_train,
                         'test': results_test}
         return results_dict
 
 
 
 
-def plot_history(history,figsize=(6,8), return_fig=False):
+def plot_history(history, figsize=(6,8), return_fig=False):
     """Plots the training and validation curves for all metrics in a Tensorflow History object.
 
     Args:
         history (Tensorflow History): History output from training a neural network.
-        figsize (tuple, optional): Total fdigure size. Defaults to (6,8).
+        figsize (tuple, optional): Total figure size. Defaults to (6,8).
         return_fig (boolean, optional): If true, return figure instead of displaying it with plt.show()
+
+    Returns:
+        None or matplotlib.figure.Figure: If return_fig is True, returns the figure object. Otherwise, displays the figure using plt.show().
     """
     import matplotlib.pyplot as plt
     import numpy as np
     # Get a unique list of metrics 
     all_metrics = np.unique([k.replace('val_','') for k in history.history.keys()])
     # Plot each metric
     n_plots = len(all_metrics)
@@ -302,178 +301,176 @@
     fig.tight_layout()
  
     if return_fig:
         return fig
     else:
         plt.show()
 
+
 def convert_y_to_sklearn_classes(y, verbose=False):
-    """Helper function to convert neural network outputs to class labels.
-    if ndim ==1, use as-is.
-    
+    """
+    Helper function to convert neural network outputs to class labels.
 
     Args:
-        y (array/Series): preditions to convert to classes.
+        y (array/Series): Predictions to convert to classes.
         verbose (bool, optional): Print which preprocessing approach is used. Defaults to False.
 
     Returns:
         array: Target as 1D class labels
     """
     import numpy as np
+
     # If already one-dimension
-    if np.ndim(y)==1:
+    if np.ndim(y) == 1:
         if verbose:
             print("- y is 1D, using it as-is.")
         return y
-        
+
     # If 2 dimensions with more than 1 column:
-    elif y.shape[1]>1:
+    elif y.shape[1] > 1:
         if verbose:
-            print("- y is 2D with >1 column. Using argmax for metrics.")   
+            print("- y is 2D with >1 column. Using argmax for metrics.")
         return np.argmax(y, axis=1)
-    
+
     else:
         if verbose:
             print("y is 2D with 1 column. Using round for metrics.")
         return np.round(y).flatten().astype(int)
 
 
-def get_true_pred_labels(model,ds):
-    """	Gets the labels and predicted probabilities from a Tensorflow model and Dataset object.
-    Adapted from source: https://stackoverflow.com/questions/66386561/keras-classification-report-accuracy-is-different-between-model-predict-accurac
-    
+def get_true_pred_labels(model, ds):
+    """Gets the true labels and predicted probabilities from a Tensorflow model and Dataset object.
 
     Args:
-        model (Tensorflow/Keras model): Model to get predictions from.
-        ds (tensorflow.data.Dataset): dataset to iterate through as a numpy iterator.
+        model (Tensorflow/Keras model): The model to get predictions from.
+        ds (tensorflow.data.Dataset): The dataset to iterate through.
 
     Returns:
-        _type_: _description_
+        tuple: A tuple containing the true labels and predicted probabilities.
     """
     import numpy as np
 
     y_true = []
     y_pred_probs = []
-    
+
     # Loop through the dataset as a numpy iterator
     for images, labels in ds.as_numpy_iterator():
-        
+
         # Get prediction with batch_size=1
         y_probs = model.predict(images, batch_size=1, verbose=0)
         # Combine previous labels/preds with new labels/preds
         y_true.extend(labels)
         y_pred_probs.extend(y_probs)
     ## Convert the lists to arrays
     y_true = np.array(y_true)
     y_pred_probs = np.array(y_pred_probs)
-    
+
     return y_true, y_pred_probs
 
 
 
 # #### Regression
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
-def regression_metrics(y_true, y_pred, label='', verbose = True, output_dict=False):
-    """Calculate MEA, MSE, RMSE, R-Squared and MAPE using the true and predicted labels.
+def regression_metrics(y_true, y_pred, label='', verbose=True, output_dict=False):
+    """
+    Calculate MEA, MSE, RMSE, R-Squared and MAPE using the true and predicted labels.
 
     Args:
         y_true (Series/array): True target values.
-        y_pred (Series/array): Predicted targe values.
+        y_pred (Series/array): Predicted target values.
         label (str, optional): Label to display in results header. Defaults to ''.
-        verbose (bool, optional): Controls printing of results. Defaults to True. 
-        output_dict (bool, optional): Return results in a dictionary. Defaults to False. (Note one of either verbose or output_dict should be set to True)
+        verbose (bool, optional): Controls printing of results. Defaults to True.
+        output_dict (bool, optional): Return results in a dictionary. Defaults to False.
+            (Note one of either verbose or output_dict should be set to True)
 
     Returns:
-        dict: Dictionary of reuslts with keys: 'Label','MAE','MSE', 'RMSE', 'MAPE','R^2'. Only returned if out_dict==True.
+        dict: Dictionary of results with keys: 'Label', 'MAE', 'MSE', 'RMSE', 'MAPE', 'R^2'.
+            Only returned if output_dict is True.
     """
     import numpy as np
     # Get metrics
     mae = mean_absolute_error(y_true, y_pred)
     mse = mean_squared_error(y_true, y_pred)
     rmse = mean_squared_error(y_true, y_pred, squared=False)
     r_squared = r2_score(y_true, y_pred)
     mape = mean_absolute_percentage_error(y_true, y_pred)
-    if (verbose==False) & (output_dict==False):
-     raise Exception("At least one of the following arguments must be set to True: output_dict, verbose.")
+    if (verbose == False) & (output_dict == False):
+        raise Exception("At least one of the following arguments must be set to True: output_dict, verbose.")
 
     if verbose == True:
         # Print Result with Label and Header
-        header = "-"*60
+        header = "-" * 60
         print(header, f"Regression Metrics: {label}", header, sep='\n')
         print("Relative Comparison Metrics:")
         print(f"- MAE = {mae:,.3f}")
         print(f"- MSE = {mse:,.3f}")
         print(f"- RMSE = {rmse:,.3f}")
         # print('\n')
         print("\nAbsolute Metrics")
         print(f"- MAPE = {mape:,.3f}")
         print(f"- R^2 = {r_squared:,.3f}")
-  
     if output_dict == True:
         metrics = {'Label':label, 'MAE':mae,
                     'MSE':mse, 'RMSE':rmse, 'MAPE':mape,
                     'R^2':r_squared}
         return metrics
 
 
 
-def evaluate_regression(reg, X_train, y_train, X_test, y_test, verbose = True,
-                        output_frame=False):
+def evaluate_regression(reg, X_train, y_train, X_test, y_test, verbose=True, output_frame=False):
     """Evalutes an sklearn-compatible regression model on training and test data. 
     For each data split, return the classification report and confusion matrix display. 
 
     Args:
         reg (sklearn estimator): Regression model to evaluate.
         X_train (Frame/Array, optional): Training data. Defaults to None.
         y_train (Series/Array, optional): Training labels. Defaults to None.
         X_test (Frame/Array, optional): Test data. Defaults to None.
         y_test (Series/Array, optional): Test labels. Defaults to None.
         verbose (bool, optional): Controls printing of results. Defaults to True. 
         output_dict (bool, optional): Return results in a dictionary. Defaults to False. (Note one of either verbose or output_dict should be set to True)
 
     Returns:
-        dict: Dictionary of reuslts with keys: 'Label','MAE','MSE', 'RMSE', 'MAPE','R^2'. Only returned if out_dict==True.
+        dict: Dictionary of results with keys: 'Label','MAE','MSE', 'RMSE', 'MAPE','R^2'. Only returned if output_dict==True.
     """
     # Get predictions for training data
     y_train_pred = reg.predict(X_train)
 
     # Call the helper function to obtain regression metrics for training data
-    results_train = regression_metrics(y_train, y_train_pred, verbose = verbose,
-                                        output_dict=output_frame,
-                                        label='Training Data')
+    results_train = regression_metrics(y_train, y_train_pred, verbose=verbose, output_dict=output_frame, label='Training Data')
     print()
+
     # Get predictions for test data
     y_test_pred = reg.predict(X_test)
+
     # Call the helper function to obtain regression metrics for test data
-    results_test = regression_metrics(y_test, y_test_pred, verbose = verbose,
-                                    output_dict=output_frame,
-                                        label='Test Data' )
+    results_test = regression_metrics(y_test, y_test_pred, verbose=verbose, output_dict=output_frame, label='Test Data')
 
-  # Store results in a dataframe if ouput_frame is True
+    # Store results in a dataframe if output_frame is True
     if output_frame:
         import pandas as pd
-        results_df = pd.DataFrame([results_train,results_test])
+        results_df = pd.DataFrame([results_train, results_test])
         # Set the label as the index
         results_df = results_df.set_index('Label')
         # Set index.name to none to get a cleaner looking result
-        results_df.index.name=None
+        results_df.index.name = None
         # Return the dataframe
         return results_df.round(3)
 
 
 
     
 def evaluate_ols(result,X_train_df, y_train, show_summary=True):
     """Plots a Q-Q Plot and residual plot for a statsmodels OLS regression, with option to display summary.
 
     Args:
-        model (statsmodels OLS): statsmodels regression model.
-        X_test_df (array/Frame): Test Data
-        y_test (array/Series): Test Labels
-        figsize (tuple, optional): Figsize for regression plots. Defaults to (12,5).
+        result (statsmodels RegressionResultsWrapper): The result object obtained from fitting the OLS model.
+        X_train_df (pandas DataFrame): The training data features.
+        y_train (pandas Series): The training data labels.
+        show_summary (bool, optional): Whether to display the summary of the regression model. Defaults to True.
     """
     import matplotlib.pyplot as plt
     import statsmodels.api as sm
     try:
         from IPython.display import display
         display(result.summary())
     except:
@@ -497,18 +494,18 @@
     
     
     
 def plot_residuals(model,X_test_df, y_test,figsize=(12,5)):
     """Plots a Q-Q Plot and residual plot for a regression model.
 
     Args:
-        model (regression model): regression model that supports .predict
-        X_test_df (_type_): Test Data
-        y_test (_type_): Test Labels
-        figsize (tuple, optional): Figsize for regression plots. Defaults to (12,5).
+        model (regression model): The regression model that supports .predict.
+        X_test_df (DataFrame): The test data.
+        y_test (array-like): The test labels.
+        figsize (tuple, optional): The figsize for the regression plots. Defaults to (12,5).
     """
 
     import matplotlib.pyplot as plt
     import statsmodels.api as sm
     ## Make predictions and calculate residuals
     y_pred = model.predict(X_test_df)
     resid = y_test - y_pred
```

### Comparing `dojo_ds-1.0.9/dojo_ds/utils.py` & `dojo_ds-1.1.0/dojo_ds/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -393,27 +393,26 @@
 
 
 
 def column_report(df,index_col=None, sort_column='iloc', ascending=True,
                   interactive=False, return_df=False):
     """
     Displays a DataFrame summary of each column's: 
-    - name, iloc, dtypes, null value count & %, # of 0's, min, max,med,mean, etc
+    - name, iloc, dtypes, null value count & %, # of 0's, min, max, med, mean, etc
     
     Args:
-        df (DataFrame): df to report 
-        index_col (column to set as index, str): Defaults to None.
-        sort_column (str, optional): [description]. Defaults to 'iloc'.
-        ascending (bool, optional): [description]. Defaults to True.
-        as_df (bool, optional): [description]. Defaults to False.
-        interactive (bool, optional): [description]. Defaults to False.
-        return_df (bool, optional): [description]. Defaults to False.
+        df (DataFrame): The DataFrame to report on.
+        index_col (str, optional): The column to set as the index. Defaults to None.
+        sort_column (str, optional): The column to sort the report by. Defaults to 'iloc'.
+        ascending (bool, optional): Whether to sort the report in ascending order. Defaults to True.
+        interactive (bool, optional): Whether to enable interactive sorting. Defaults to False.
+        return_df (bool, optional): Whether to return the non-styled version of the report DataFrame. Defaults to False.
 
     Returns:
-        column_report (df): Non-styled version of displayed df report
+        column_report (DataFrame): The non-styled version of the displayed report DataFrame.
     """
     from ipywidgets import interact
     import pandas as pd
     from IPython.display import display
 
     def count_col_zeros(df, columns=None):
         import pandas as pd
@@ -425,16 +424,14 @@
             columns=df.columns
 
         # get sum of zero values for each column
         for col in columns:
             zeros[col] = np.sum( df[col].values == 0)
         return zeros
 
-
-    ##
     df_report = pd.DataFrame({'.iloc[:,i]': range(len(df.columns)),
                             'column name':df.columns,
                             'dtypes':df.dtypes.astype('str'),
                             '.isna()': df.isna().sum().round(),
                             '% na':df.isna().sum().divide(df.shape[0]).mul(100).round(2),
                             '# zeros': count_col_zeros(df),
                             '# unique':df.nunique(),
@@ -497,90 +494,118 @@
             print(f'del {me} failed')
             continue
         """
     print(del_me)
 
 
 
-def get_methods(obj,private=False):
+def get_methods(obj, private=False):
     """
     Retrieves a list of all non-private methods (default) from inside of obj.
-    - If private==False: only returns methods whose names do NOT start with a '_'
     
     Args:
         obj (object): Object to retrieve methods from.
-        private (bool): Whether to retrieve private methods or public.
+        private (bool, optional): Whether to retrieve private methods or public. 
+            Defaults to False, which retrieves only public methods.
 
     Returns:
-        list: the names of all of the retrieved methods.
+        list: The names of all the retrieved methods.
+
+    Examples:
+        >>> class MyClass:
+        ...     def public_method(self):
+        ...         pass
+        ...     def _private_method(self):
+        ...         pass
+        ...
+        >>> obj = MyClass()
+        >>> get_methods(obj)
+        ['public_method']
+        >>> get_methods(obj, private=True)
+        ['public_method', '_private_method']
     """
     method_list = [func for func in dir(obj) if callable(getattr(obj, func))]
     if private:
-        filt_methods = list(filter(lambda x: '_' in x[0] ,method_list))
+        filt_methods = list(filter(lambda x: '_' in x[0], method_list))
     else:
-        filt_methods = list(filter(lambda x: '_' not in x[0] ,method_list))
-    return  filt_methods
+        filt_methods = list(filter(lambda x: '_' not in x[0], method_list))
+    return filt_methods
 
 
 def get_attributes(obj,private=False):
     """
     Retrieves a list of all non-private attributes (default) from inside of obj.
     - If private==False: only returns methods whose names do NOT start with a '_'
     
     Args:
         obj (object): Object to retrieve attributes from.
-        private (bool): Whether to retrieve private attributes or public.
+        private (bool, optional): Whether to retrieve private attributes or public. Defaults to False.
     
     Returns:
-        list: the names of all of the retrieved attributes.
+        list: The names of all the retrieved attributes.
     """
     method_list = [func for func in dir(obj) if not callable(getattr(obj, func))]
     if private:
         filt_methods = list(filter(lambda x: '_' in x[0] ,method_list))
     else:
         filt_methods = list(filter(lambda x: '_' not in x[0] ,method_list))
     return  filt_methods
     
     
     
-def clickable_link(path,label=None):
-    """Adapted from: https://www.geeksforgeeks.org/how-to-create-a-table-with-clickable-hyperlink-to-a-local-file-in-pandas/"""
-    # returns the final component of a url
-    # f_url = os.path.basename(path)
+def clickable_link(path, label=None):
+    """
+    Converts a file path into a clickable hyperlink.
+
+    Parameters:
+    path (str): The file path to be converted.
+    label (str, optional): The label to be displayed for the hyperlink. If not provided, the file path will be used as the label.
+
+    Returns:
+    str: The clickable hyperlink.
+
+    Adapted from: https://www.geeksforgeeks.org/how-to-create-a-table-with-clickable-hyperlink-to-a-local-file-in-pandas/
+    """
     if label is None:
-    # convert the url into link
         return '<a href="{}">{}</a>'.format(path, path)
     else: 
-        return '<a href="{}">{}</a>'.format(path, label)  
+        return '<a href="{}">{}</a>'.format(path, label)
         
         
         
         
 
-def get_or_print_filesize(fpath, unit ="MB", print_or_return='print'):
+def get_or_print_filesize(fpath, unit="MB", print_or_return='print'):
     """Get the file size as a string, converted to the requested unit(B,KB, MB, GB)
 
     Args:
         fpath (string): file to analyze
         unit (str, optional): unit for conversion. Defaults to "MB".
         print_or_return (str, optional): Controls if string is returned or printed. Defaults to 'print'.
 
     Returns:
         string: file size + units
+
+    Raises:
+        FileNotFoundError: If the specified file does not exist.
     """
     import os
+
+    if not os.path.exists(fpath):
+        raise FileNotFoundError(f"File '{fpath}' does not exist.")
+
     size = os.path.getsize(fpath)
+
     if unit == 'KB':
         size /= 1024
     elif unit == 'MB':
-        size /= (1024**2)
+        size /= (1024 ** 2)
     elif unit == 'GB':
-        size /= (1024**3)
-    # else:
-        # print(f"{size:.3f} B")
+        size /= (1024 ** 3)
+
     formatted_size = f"{size:.3f} {unit}"
-    
+
     if print_or_return == 'print':
         print(formatted_size)
-    else: 
+    else:
         return formatted_size
```

### Comparing `dojo_ds-1.0.9/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-1.1.0/dojo_ds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.0.9
+Version: 1.1.0
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: Click>=7.0
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: seaborn>=0.12.2
+Requires-Dist: statsmodels>=0.13.5
+Requires-Dist: pmdarima==2.0.4
 
 =======
 dojo-ds
 =======
 
 
 .. image:: https://img.shields.io/pypi/v/dojo_ds.svg
```

### Comparing `dojo_ds-1.0.9/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-1.1.0/dojo_ds.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 dojo_ds/deploy.py
 dojo_ds/eda.py
 dojo_ds/evaluate.py
 dojo_ds/imports.py
 dojo_ds/insights.py
 dojo_ds/matplotlib_style.py
 dojo_ds/nlp.py
+dojo_ds/time_series.py
 dojo_ds/utils.py
 dojo_ds.egg-info/PKG-INFO
 dojo_ds.egg-info/SOURCES.txt
 dojo_ds.egg-info/dependency_links.txt
 dojo_ds.egg-info/entry_points.txt
 dojo_ds.egg-info/not-zip-safe
 dojo_ds.egg-info/requires.txt
```

### Comparing `dojo_ds-1.0.9/setup.py` & `dojo_ds-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,45 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-## Grab requirements form file
-# with open("requirements.txt") as f:
+import setuptools
+
+# Function to load requirements from a file
+def load_requirements(filename):
+    try:
+        with open(filename, 'r') as file:
+            requirements = []
+            for line in file:
+                # Remove whitespace and skip comments and empty lines
+                line = line.strip()
+                if line and not line.startswith('#'):
+                    requirements.append(line)
+            return requirements
+    except FileNotFoundError:
+        print(f"Error: The file {filename} does not exist.")
+        return []
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return []
+
+
+# ## Grab requirements form file
+# with open("./requirements.txt") as f:
 #     req_list = f.readlines()
-#     req_LIST = [str(req) for req in req_list]
-req_list = ['scikit-learn>=1.2.2','pandas>=1.5.3','matplotlib>=3.7.1', 'seaborn>=0.12.2']#, 'plotly>=5.15.0']
-requirements = ['Click>=7.0', *req_list  ]
+#     req_list = [x.strip() for x in req_list if not x.startswith('#') and x.strip() != '']
+#     # req_LIST = [str(req) for req in req_list]
+# # req_list = ['scikit-learn>=1.2.2','pandas>=1.5.3','matplotlib>=3.7.1', 'seaborn>=0.12.2'
+# #             'statsmodels>=0.13.5']#, 'plotly>=5.15.0']
+# requirements = ['Click>=7.0', *req_list  ]
 
-test_requirements = [ ]
+test_requirements = ['sphinx_rtd_theme' ]
 
 setup(
     author="James Irving",
     author_email='jirving@codingdojo.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -36,20 +59,20 @@
     ],
     description="Code from Coding Dojo's Online Part-Time Data Science boot camp",
     entry_points={
         'console_scripts': [
             'dojo_ds=dojo_ds.cli:main',
         ],
     },
-    install_requires=requirements,
+    install_requires=load_requirements("./requirements.txt"),
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='dojo_ds',
     name='dojo_ds',
     packages=find_packages(include=['dojo_ds', 'dojo_ds.*']),
     test_suite='tests',
-    tests_require=test_requirements,
+    tests_require=load_requirements("./requirements.txt") + test_requirements,
     url='https://github.com/coding-dojo-data-science/dojo_ds',
-    version='1.0.9',
+    version='1.1.0',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-1.0.9/tests/test_dojo_ds.py` & `dojo_ds-1.1.0/tests/test_dojo_ds.py`

 * *Files identical despite different names*

