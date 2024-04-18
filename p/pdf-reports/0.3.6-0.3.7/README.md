# Comparing `tmp/pdf_reports-0.3.6.tar.gz` & `tmp/pdf_reports-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_reports-0.3.6.tar", last modified: Wed Apr 17 11:06:16 2024, max compression
+gzip compressed data, was "pdf_reports-0.3.7.tar", last modified: Thu Apr 18 13:46:05 2024, max compression
```

## Comparing `pdf_reports-0.3.6.tar` & `pdf_reports-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.018083 pdf_reports-0.3.6/
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/LICENCE.txt
--rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7294 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/README.rst
--rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/ez_setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:15.994084 pdf_reports-0.3.6/pdf_reports/
--rw-rw-r--   0 peter     (1000) peter     (1000)      239 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/pdf_reports/css/
--rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/egf-logo.svg
--rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/semantic.min.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/pdf_reports/css/style.css
--rw-rw-r--   0 peter     (1000) peter     (1000)     6797 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/pdf_reports.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5656 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/tools.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/pdf_reports/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/pdf_reports.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      469 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       87 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2024-04-17 11:06:12.000000 pdf_reports-0.3.6/pdf_reports.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1590 2023-07-21 22:25:15.000000 pdf_reports-0.3.6/pypi-readme.rst
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2024-04-17 11:06:16.018083 pdf_reports-0.3.6/setup.cfg
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1326 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-17 11:06:16.014083 pdf_reports-0.3.6/tests/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2272 2024-04-17 11:05:59.000000 pdf_reports-0.3.6/tests/test_basics.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2022-05-05 10:51:32.000000 pdf_reports-0.3.6/tests/test_tools.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 13:46:05.490506 pdf_reports-0.3.7/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1081 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/LICENCE.txt
+-rwxrwxr-x   0 peter     (1000) peter     (1000)       84 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-18 13:46:05.490506 pdf_reports-0.3.7/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7294 2024-04-18 13:45:18.000000 pdf_reports-0.3.7/README.rst
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     8512 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/ez_setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 13:46:05.486506 pdf_reports-0.3.7/pdf_reports/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      239 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/pdf_reports/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 13:46:05.486506 pdf_reports-0.3.7/pdf_reports/css/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)    19352 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/pdf_reports/css/egf-logo.svg
+-rw-rw-r--   0 peter     (1000) peter     (1000)   618735 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/pdf_reports/css/semantic.min.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1502 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/pdf_reports/css/style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6797 2024-04-18 13:45:18.000000 pdf_reports-0.3.7/pdf_reports/pdf_reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5623 2024-04-18 13:45:20.000000 pdf_reports-0.3.7/pdf_reports/tools.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2024-04-18 13:45:20.000000 pdf_reports-0.3.7/pdf_reports/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 13:46:05.486506 pdf_reports-0.3.7/pdf_reports.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2060 2024-04-18 13:46:05.000000 pdf_reports-0.3.7/pdf_reports.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      469 2024-04-18 13:46:05.000000 pdf_reports-0.3.7/pdf_reports.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2024-04-18 13:46:05.000000 pdf_reports-0.3.7/pdf_reports.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       87 2024-04-18 13:46:05.000000 pdf_reports-0.3.7/pdf_reports.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2024-04-18 13:46:05.000000 pdf_reports-0.3.7/pdf_reports.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1590 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/pypi-readme.rst
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2024-04-18 13:46:05.490506 pdf_reports-0.3.7/setup.cfg
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1326 2024-04-18 13:45:18.000000 pdf_reports-0.3.7/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-18 13:46:05.486506 pdf_reports-0.3.7/tests/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2272 2024-04-18 13:45:18.000000 pdf_reports-0.3.7/tests/test_basics.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2024-03-26 14:05:16.000000 pdf_reports-0.3.7/tests/test_tools.py
```

### Comparing `pdf_reports-0.3.6/LICENCE.txt` & `pdf_reports-0.3.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/PKG-INFO` & `pdf_reports-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_reports
-Version: 0.3.6
+Version: 0.3.7
 Summary: Create nice-looking PDF reports from HTML content.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
 Author: Zulko
 License: MIT
 Keywords: PDF report web jinja weasyprint
 License-File: LICENCE.txt
 Requires-Dist: pypugjs
```

### Comparing `pdf_reports-0.3.6/README.rst` & `pdf_reports-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/ez_setup.py` & `pdf_reports-0.3.7/ez_setup.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/pdf_reports/css/egf-logo.svg` & `pdf_reports-0.3.7/pdf_reports/css/egf-logo.svg`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/pdf_reports/css/semantic.min.css` & `pdf_reports-0.3.7/pdf_reports/css/semantic.min.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/pdf_reports/css/style.css` & `pdf_reports-0.3.7/pdf_reports/css/style.css`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/pdf_reports/pdf_reports.py` & `pdf_reports-0.3.7/pdf_reports/pdf_reports.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/pdf_reports/tools.py` & `pdf_reports-0.3.7/pdf_reports/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Utilities for report generation.
 
 The module contains in particular routines the creation of tables, plots, etc.
 inside the templates. Functions in this module are available from inside the
 templates under the domain name ``pdf_tools``. For instance
 ``pdf_tools.dataframe_to_html()``.
 """
+
 from bs4 import BeautifulSoup
 import base64
 import pandas
 from io import BytesIO
 import datetime
 import textwrap
 
-from matplotlib.axes import Axes
-
 
 def dataframe_to_html(
     dataframe,
     extra_classes=(),
     index=False,
     header=True,
     use_default_classes=True,
```

### Comparing `pdf_reports-0.3.6/pdf_reports.egg-info/PKG-INFO` & `pdf_reports-0.3.7/pdf_reports.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf_reports
-Version: 0.3.6
+Version: 0.3.7
 Summary: Create nice-looking PDF reports from HTML content.
 Home-page: https://github.com/Edinburgh-Genome-Foundry/pdf_reports
 Author: Zulko
 License: MIT
 Keywords: PDF report web jinja weasyprint
 License-File: LICENCE.txt
 Requires-Dist: pypugjs
```

### Comparing `pdf_reports-0.3.6/pypi-readme.rst` & `pdf_reports-0.3.7/pypi-readme.rst`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/setup.py` & `pdf_reports-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/tests/test_basics.py` & `pdf_reports-0.3.7/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pdf_reports-0.3.6/tests/test_tools.py` & `pdf_reports-0.3.7/tests/test_tools.py`

 * *Files identical despite different names*

