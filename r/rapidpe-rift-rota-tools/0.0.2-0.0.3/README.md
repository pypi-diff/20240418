# Comparing `tmp/rapidpe_rift_rota_tools-0.0.2.tar.gz` & `tmp/rapidpe_rift_rota_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_rota_tools-0.0.2.tar", last modified: Mon Mar 11 21:16:42 2024, max compression
+gzip compressed data, was "rapidpe_rift_rota_tools-0.0.3.tar", last modified: Tue Apr 16 19:28:33 2024, max compression
```

## Comparing `rapidpe_rift_rota_tools-0.0.2.tar` & `rapidpe_rift_rota_tools-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.064595 rapidpe_rift_rota_tools-0.0.2/
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)    18038 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/COPYING
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       69 2024-03-11 00:09:53.000000 rapidpe_rift_rota_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1015 2024-03-11 21:16:42.064595 rapidpe_rift_rota_tools-0.0.2/PKG-INFO
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)      282 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/README.md
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1170 2024-03-11 21:16:42.066594 rapidpe_rift_rota_tools-0.0.2/setup.cfg
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       38 2024-03-11 00:09:53.000000 rapidpe_rift_rota_tools-0.0.2/setup.py
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.024594 rapidpe_rift_rota_tools-0.0.2/src/
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.042594 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       22 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/__init__.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1496 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/auto_generate_status_page.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     2207 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/condor.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     5821 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/create_status_page.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)      499 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/results.py
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.054594 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/static/
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/static/__init__.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)      214 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/static/gracedb_dir.json
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     2889 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/status_summary.py
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.060594 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/__init__.py
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     2842 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/status.jinja2
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1524 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/status_style.css
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)      382 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/status_style.js
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       73 2024-03-11 18:54:23.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/test_statuspage.py
-drwxrwxr-x   0 vinaya.valsan (45215) vinaya.valsan (45215)        0 2024-03-11 21:16:42.062595 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/
--rw-r--r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1015 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/PKG-INFO
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)     1003 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)        1 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)      187 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/entry_points.txt
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       25 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/requires.txt
--rw-rw-r--   0 vinaya.valsan (45215) vinaya.valsan (45215)       24 2024-03-11 21:16:42.000000 rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.598755 rapidpe_rift_rota_tools-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)    18038 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-16 19:28:33.598755 rapidpe_rift_rota_tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2024-04-16 19:28:33.598755 rapidpe_rift_rota_tools-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.594755 rapidpe_rift_rota_tools-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.595755 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/auto_generate_status_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/condor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/create_status_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.597756 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 19:28:26.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/static/gracedb_dir.json
+-rw-rw-rw-   0 root         (0) root         (0)     2889 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/status_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.597756 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 19:28:26.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/status.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/status_style.css
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/status_style.js
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-16 00:49:40.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/test_statuspage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 19:28:33.597756 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-16 19:28:33.000000 rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/top_level.txt
```

### Comparing `rapidpe_rift_rota_tools-0.0.2/COPYING` & `rapidpe_rift_rota_tools-0.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/PKG-INFO` & `rapidpe_rift_rota_tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_rota_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Rota tools for  RapidPE-RIFT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `rapidpe_rift_rota_tools-0.0.2/setup.cfg` & `rapidpe_rift_rota_tools-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/auto_generate_status_page.py` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/auto_generate_status_page.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/condor.py` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/condor.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/create_status_page.py` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/create_status_page.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/status_summary.py` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/status_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/status.jinja2` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/status.jinja2`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools/template_files/status_style.css` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools/template_files/status_style.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/PKG-INFO` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_rota_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Rota tools for  RapidPE-RIFT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `rapidpe_rift_rota_tools-0.0.2/src/rapidpe_rift_rota_tools.egg-info/SOURCES.txt` & `rapidpe_rift_rota_tools-0.0.3/src/rapidpe_rift_rota_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

