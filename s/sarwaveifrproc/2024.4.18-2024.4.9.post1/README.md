# Comparing `tmp/sarwaveifrproc-2024.4.18.tar.gz` & `tmp/sarwaveifrproc-2024.4.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarwaveifrproc-2024.4.18.tar", last modified: Thu Apr 18 09:35:22 2024, max compression
+gzip compressed data, was "sarwaveifrproc-2024.4.9.post1.tar", last modified: Tue Apr  9 13:39:19 2024, max compression
```

## Comparing `sarwaveifrproc-2024.4.18.tar` & `sarwaveifrproc-2024.4.9.post1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.845837 sarwaveifrproc-2024.4.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.845837 sarwaveifrproc-2024.4.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.849837 sarwaveifrproc-2024.4.18/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.849837 sarwaveifrproc-2024.4.18/sarwaveifrproc/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/l2_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/
--rw-r--r--   0 runner    (1001) docker     (127)   372928 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc
--rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc
--rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/sarwaveifrproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 09:35:22.000000 sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:35:22.853837 sarwaveifrproc-2024.4.18/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-18 09:35:14.000000 sarwaveifrproc-2024.4.18/tests/test_sarwaveifrproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.311471 sarwaveifrproc-2024.4.9.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.311471 sarwaveifrproc-2024.4.9.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.315471 sarwaveifrproc-2024.4.9.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.315471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/l2_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   372928 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/sarwaveifrproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/test_sarwaveifrproc.py
```

### Comparing `sarwaveifrproc-2024.4.18/.github/workflows/publish.yml` & `sarwaveifrproc-2024.4.9.post1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/.gitignore` & `sarwaveifrproc-2024.4.9.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/CONTRIBUTING.rst` & `sarwaveifrproc-2024.4.9.post1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/LICENSE` & `sarwaveifrproc-2024.4.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/Makefile` & `sarwaveifrproc-2024.4.9.post1/Makefile`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/PKG-INFO` & `sarwaveifrproc-2024.4.9.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarwaveifrproc
-Version: 2024.4.18
+Version: 2024.4.9.post1
 Summary: Python library to generate Level-2 WAVE Product starting from Ifremer Level-1B or Level-1C SAR files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wave,reseach,sea-state
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `sarwaveifrproc-2024.4.18/README.rst` & `sarwaveifrproc-2024.4.9.post1/README.rst`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/docs/Makefile` & `sarwaveifrproc-2024.4.9.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/docs/conf.py` & `sarwaveifrproc-2024.4.9.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/docs/installation.rst` & `sarwaveifrproc-2024.4.9.post1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/docs/make.bat` & `sarwaveifrproc-2024.4.9.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/pyproject.toml` & `sarwaveifrproc-2024.4.9.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc/l2_wave.py` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/l2_wave.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc/utils.py` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/utils.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/PKG-INFO` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarwaveifrproc
-Version: 2024.4.18
+Version: 2024.4.9.post1
 Summary: Python library to generate Level-2 WAVE Product starting from Ifremer Level-1B or Level-1C SAR files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wave,reseach,sea-state
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `sarwaveifrproc-2024.4.18/sarwaveifrproc.egg-info/SOURCES.txt` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/tests/test_predict.py` & `sarwaveifrproc-2024.4.9.post1/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.18/tests/test_sarwaveifrproc.py` & `sarwaveifrproc-2024.4.9.post1/tests/test_sarwaveifrproc.py`

 * *Files identical despite different names*

