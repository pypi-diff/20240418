# Comparing `tmp/dojo_ds-1.1.0.tar.gz` & `tmp/dojo_ds-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-1.1.0.tar", last modified: Thu Apr 18 19:31:10 2024, max compression
+gzip compressed data, was "dojo_ds-1.1.1.tar", last modified: Thu Apr 18 19:38:18 2024, max compression
```

## Comparing `dojo_ds-1.1.0.tar` & `dojo_ds-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.167366 dojo_ds-1.1.0/
--rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.0/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.0/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:31:10.167244 dojo_ds-1.1.0/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.0/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.137885 dojo_ds-1.1.0/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.0/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/authors.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.117506 dojo_ds-1.1.0/docs/build/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.117615 dojo_ds-1.1.0/docs/build/html/
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.139650 dojo_ds-1.1.0/docs/build/html/_static/
--rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/file.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/minus.png
--rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.0/docs/build/html/_static/plus.png
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.0/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.0/docs/dojo_ds.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.0/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.0/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.0/docs/modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.0/docs/old_modules.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.0/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.157917 dojo_ds-1.1.0/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 19:24:42.000000 dojo_ds-1.1.0/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.0/dojo_ds/_eda_functions_plotly.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.0/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.0/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.0/dojo_ds/deploy.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.0/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.0/dojo_ds/evaluate.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.0/dojo_ds/imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.0/dojo_ds/insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.0/dojo_ds/matplotlib_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.0/dojo_ds/nlp.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     8861 2024-04-18 19:20:54.000000 dojo_ds-1.1.0/dojo_ds/time_series.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.0/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.166797 dojo_ds-1.1.0/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)      104 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 19:31:10.000000 dojo_ds-1.1.0/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 19:31:10.167792 dojo_ds-1.1.0/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 19:30:18.000000 dojo_ds-1.1.0/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:31:10.166427 dojo_ds-1.1.0/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.0/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.0/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.141604 dojo_ds-1.1.1/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      195 2024-01-24 00:23:27.000000 dojo_ds-1.1.1/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-1.1.1/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:38:18.141423 dojo_ds-1.1.1/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      607 2023-05-19 01:08:02.000000 dojo_ds-1.1.1/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.121416 dojo_ds-1.1.1/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2024-01-24 01:18:29.000000 dojo_ds-1.1.1/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/authors.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.099342 dojo_ds-1.1.1/docs/build/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.100000 dojo_ds-1.1.1/docs/build/html/
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.123353 dojo_ds-1.1.1/docs/build/html/_static/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      286 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/file.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/minus.png
+-rw-r--r--   0 codingdojo   (502) staff       (20)       90 2024-01-23 23:54:56.000000 dojo_ds-1.1.1/docs/build/html/_static/plus.png
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     6020 2024-01-24 01:33:23.000000 dojo_ds-1.1.1/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1512 2024-01-24 01:04:56.000000 dojo_ds-1.1.1/docs/dojo_ds.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      384 2024-01-24 01:32:59.000000 dojo_ds-1.1.1/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      542 2024-01-24 01:23:15.000000 dojo_ds-1.1.1/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 01:14:29.000000 dojo_ds-1.1.1/docs/modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       58 2024-01-24 00:26:33.000000 dojo_ds-1.1.1/docs/old_modules.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       75 2023-05-17 14:09:11.000000 dojo_ds-1.1.1/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.134170 dojo_ds-1.1.1/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      969 2024-04-18 19:38:08.000000 dojo_ds-1.1.1/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     7851 2024-02-23 02:05:37.000000 dojo_ds-1.1.1/dojo_ds/_eda_functions_plotly.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2024-01-23 02:13:03.000000 dojo_ds-1.1.1/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4721 2024-02-23 02:07:09.000000 dojo_ds-1.1.1/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2047 2024-02-23 02:12:32.000000 dojo_ds-1.1.1/dojo_ds/deploy.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    12923 2024-02-23 02:03:18.000000 dojo_ds-1.1.1/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    24080 2024-02-23 02:01:30.000000 dojo_ds-1.1.1/dojo_ds/evaluate.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2024-01-23 02:14:45.000000 dojo_ds-1.1.1/dojo_ds/imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    22135 2024-02-23 01:54:13.000000 dojo_ds-1.1.1/dojo_ds/insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2024-01-23 02:11:38.000000 dojo_ds-1.1.1/dojo_ds/matplotlib_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    13103 2024-02-23 02:09:27.000000 dojo_ds-1.1.1/dojo_ds/nlp.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    10346 2024-04-18 19:37:49.000000 dojo_ds-1.1.1/dojo_ds/time_series.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    19491 2024-02-23 02:13:34.000000 dojo_ds-1.1.1/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.140929 dojo_ds-1.1.1/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1674 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      938 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-1.1.1/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)      104 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2024-04-18 19:38:18.000000 dojo_ds-1.1.1/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2024-04-18 19:38:18.142695 dojo_ds-1.1.1/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     2602 2024-04-18 19:38:08.000000 dojo_ds-1.1.1/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2024-04-18 19:38:18.139759 dojo_ds-1.1.1/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-1.1.1/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      862 2024-01-23 02:15:25.000000 dojo_ds-1.1.1/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-1.1.0/CONTRIBUTING.rst` & `dojo_ds-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/LICENSE` & `dojo_ds-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/PKG-INFO` & `dojo_ds-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.0
+Version: 1.1.1
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.0/README.rst` & `dojo_ds-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/docs/Makefile` & `dojo_ds-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/docs/conf.py` & `dojo_ds-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/docs/dojo_ds.rst` & `dojo_ds-1.1.1/docs/dojo_ds.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/docs/installation.rst` & `dojo_ds-1.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/docs/make.bat` & `dojo_ds-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/__init__.py` & `dojo_ds-1.1.1/dojo_ds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Custom Functions the Data Science Program
 __author__ = James Irving, Brenda Hungerford
 """
 __author__ = """James Irving"""
 __email__ = 'james.irving.phd@gmail.com'
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 from . import data_enrichment as data
 from . import eda 
 from . import evaluate
 from . import insights 
 from . import nlp
 from . import time_series
```

### Comparing `dojo_ds-1.1.0/dojo_ds/_eda_functions_plotly.py` & `dojo_ds-1.1.1/dojo_ds/_eda_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/data_enrichment.py` & `dojo_ds-1.1.1/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/deploy.py` & `dojo_ds-1.1.1/dojo_ds/deploy.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/eda.py` & `dojo_ds-1.1.1/dojo_ds/eda.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/evaluate.py` & `dojo_ds-1.1.1/dojo_ds/evaluate.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/insights.py` & `dojo_ds-1.1.1/dojo_ds/insights.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/nlp.py` & `dojo_ds-1.1.1/dojo_ds/nlp.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds/time_series.py` & `dojo_ds-1.1.1/dojo_ds/time_series.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,55 +127,14 @@
             axes[0].axvline(m * i, **seas_vline_kwargs, label="season")
             axes[1].axvline(m * i, **seas_vline_kwargs, label="season")
 
     fig.tight_layout()
     return fig
 
 
-def regression_metrics_ts(ts_true, ts_pred, label="", verbose=True, output_dict=False):
-    """
-    Calculates regression metrics for comparing true and predicted time series data.
-
-    Parameters:
-    - ts_true (array-like): The true time series data.
-    - ts_pred (array-like): The predicted time series data.
-    - label (str): The label for the metrics. Default is an empty string.
-    - verbose (bool): Whether to print the metrics. Default is True.
-    - output_dict (bool): Whether to return the metrics as a dictionary. Default is False.
-
-    Returns:
-    - metrics (dict): The regression metrics as a dictionary. Only returned if output_dict is True.
-    """
-    mae = mean_absolute_error(ts_true, ts_pred)
-    mse = mean_squared_error(ts_true, ts_pred)
-    rmse = mean_squared_error(ts_true, ts_pred, squared=False)
-    r_squared = r2_score(ts_true, ts_pred)
-    mae_perc = mean_absolute_percentage_error(ts_true, ts_pred) * 100
-
-    if verbose:
-        header = "---" * 20
-        print(header, f"Regression Metrics: {label}", header, sep="\n")
-        print(f"- MAE = {mae:,.3f}")
-        print(f"- MSE = {mse:,.3f}")
-        print(f"- RMSE = {rmse:,.3f}")
-        print(f"- R^2 = {r_squared:,.3f}")
-        print(f"- MAPE = {mae_perc:,.2f}%")
-
-    if output_dict:
-        metrics = {
-            "Label": label,
-            "MAE": mae,
-            "MSE": mse,
-            "RMSE": rmse,
-            "R^2": r_squared,
-            "MAPE(%)": mae_perc,
-        }
-        return metrics
-
-
 def plot_forecast(ts_train, ts_test, forecast_df, n_train_lags=None, 
                   figsize=(10,4), title='Comparing Forecast vs. True Data'):
     """
     Plots the training data, test data, and forecast with confidence intervals.
 
     Parameters:
     ts_train (pandas.Series): Time series data for training.
@@ -211,7 +170,87 @@
 
     # set the title and add legend
     ax.set_title(title)
     ax.legend();
     
     return fig, ax
 
+
+def thiels_U(ts_true, ts_pred):
+    """Calculate's Thiel's U metric for forecasting accuracy.
+    Accepts true values and predicted values.
+    Original Formula Source: https://docs.oracle.com/cd/E57185_01/CBREG/ch06s02s03s04.html
+    Adapted Function from Source: https://github.com/jirvingphd/predicting-the-SP500-using-trumps-tweets_capstone-project/blob/cf11f6ed88721433d2c00cb1f8486206ab179cc0/bsds/my_keras_functions.py#L735
+    Returns: 
+        U (float)
+        
+    Thiel's U Value Interpretation:
+    - <1  = Forecasting is better than guessing 
+    - 1   = Forecasting is about as good as guessing
+    - >1  = Forecasting is worse than guessing 
+    """
+    import numpy as np
+    # sum_list = []
+    num_list=[]
+    denom_list=[]
+    
+    for t in range(len(ts_true)-1):
+        
+        num_exp = (ts_pred[t+1] - ts_true[t+1])/ts_true[t]
+        num_list.append([num_exp**2])
+        
+        denom_exp = (ts_true[t+1] - ts_true[t])/ts_true[t]
+        denom_list.append([denom_exp**2])
+        
+    U = np.sqrt( np.sum(num_list) / np.sum(denom_list))
+    return U
+
+
+def regression_metrics_ts(ts_true, ts_pred, label="", verbose=True, output_dict=False,
+                          thiels_U=False):
+    """
+    Calculates regression metrics for comparing true and predicted time series data.
+
+    Parameters:
+    - ts_true (array-like): The true time series data.
+    - ts_pred (array-like): The predicted time series data.
+    - label (str): The label for the metrics. Default is an empty string.
+    - verbose (bool): Whether to print the metrics. Default is True.
+    - output_dict (bool): Whether to return the metrics as a dictionary. Default is False.
+    - thiels_U (bool): Whether to calculate Thiel's U metric. Default is False.
+                        - See docstring for thiels_U function for interpretation.
+
+    Returns:
+    - metrics (dict): The regression metrics as a dictionary. Only returned if output_dict is True.
+    """
+    mae = mean_absolute_error(ts_true, ts_pred)
+    mse = mean_squared_error(ts_true, ts_pred)
+    rmse = mean_squared_error(ts_true, ts_pred, squared=False)
+    r_squared = r2_score(ts_true, ts_pred)
+    mae_perc = mean_absolute_percentage_error(ts_true, ts_pred) * 100
+    if thiels_U:
+        U = thiels_U(ts_true, ts_pred)
+    if verbose:
+        header = "---" * 20
+        print(header, f"Regression Metrics: {label}", header, sep="\n")
+        print(f"- MAE = {mae:,.3f}")
+        print(f"- MSE = {mse:,.3f}")
+        print(f"- RMSE = {rmse:,.3f}")
+        print(f"- R^2 = {r_squared:,.3f}")
+        print(f"- MAPE = {mae_perc:,.2f}%")
+        
+        if thiels_U:
+            print(f"- Thiel's U = {U:,.2f}")
+            
+    if output_dict:
+        metrics = {
+            "Label": label,
+            "MAE": mae,
+            "MSE": mse,
+            "RMSE": rmse,
+            "R^2": r_squared,
+            "MAPE(%)": mae_perc,
+        }
+        if thiels_U:
+            metrics['Thiel\'s U'] = U
+        return metrics
+
```

### Comparing `dojo_ds-1.1.0/dojo_ds/utils.py` & `dojo_ds-1.1.1/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-1.1.1/dojo_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 1.1.0
+Version: 1.1.1
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/coding-dojo-data-science/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-1.1.0/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-1.1.1/dojo_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dojo_ds-1.1.0/setup.py` & `dojo_ds-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,10 @@
     include_package_data=True,
     keywords='dojo_ds',
     name='dojo_ds',
     packages=find_packages(include=['dojo_ds', 'dojo_ds.*']),
     test_suite='tests',
     tests_require=load_requirements("./requirements.txt") + test_requirements,
     url='https://github.com/coding-dojo-data-science/dojo_ds',
-    version='1.1.0',
+    version='1.1.1',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-1.1.0/tests/test_dojo_ds.py` & `dojo_ds-1.1.1/tests/test_dojo_ds.py`

 * *Files identical despite different names*

