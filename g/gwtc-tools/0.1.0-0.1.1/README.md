# Comparing `tmp/gwtc_tools-0.1.0.tar.gz` & `tmp/gwtc_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwtc_tools-0.1.0.tar", last modified: Wed Apr 17 17:37:12 2024, max compression
+gzip compressed data, was "gwtc_tools-0.1.1.tar", last modified: Thu Apr 18 13:25:34 2024, max compression
```

## Comparing `gwtc_tools-0.1.0.tar` & `gwtc_tools-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.430825 gwtc_tools-0.1.0/
--rw-r--r--   0 channa     (502) staff       (20)       97 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/.gitignore
--rw-r--r--   0 channa     (502) staff       (20)      865 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/.gitlab-ci.yml
--rw-r--r--   0 channa     (502) staff       (20)      677 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 channa     (502) staff       (20)     1078 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/LICENSE.md
--rw-r--r--   0 channa     (502) staff       (20)     7260 2024-04-17 17:37:12.430692 gwtc_tools-0.1.0/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)     6339 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/README.md
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.418672 gwtc_tools-0.1.0/docs/
--rw-r--r--   0 channa     (502) staff       (20)      638 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/Makefile
--rw-r--r--   0 channa     (502) staff       (20)      804 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/make.bat
--rw-r--r--   0 channa     (502) staff       (20)       59 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.419370 gwtc_tools-0.1.0/docs/source/
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.420069 gwtc_tools-0.1.0/docs/source/_templates/
--rw-r--r--   0 channa     (502) staff       (20)      662 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 channa     (502) staff       (20)     1408 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 channa     (502) staff       (20)     2507 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/source/conf.py
--rw-r--r--   0 channa     (502) staff       (20)      484 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/docs/source/index.rst
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.423321 gwtc_tools-0.1.0/examples/
--rw-r--r--   0 channa     (502) staff       (20)     1415 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)     1440 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)   115407 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)       91 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/H1L1-SPIIR_AllSky_PASTRO-1376883065-0.json
--rw-r--r--   0 channa     (502) staff       (20)     1416 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz
--rw-r--r--   0 channa     (502) staff       (20)       58 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/L1-GSTLAL_AllSky_PASTRO-1368783503-0.json
--rw-r--r--   0 channa     (502) staff       (20)     3460 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/README.md
--rw-r--r--   0 channa     (502) staff       (20)      114 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/gstlalv1.yaml
--rw-r--r--   0 channa     (502) staff       (20)      212 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/examples/gstlalv2.yaml
--rw-r--r--   0 channa     (502) staff       (20)     1623 2024-04-17 17:36:03.000000 gwtc_tools-0.1.0/pyproject.toml
--rw-r--r--   0 channa     (502) staff       (20)      855 2024-04-17 17:37:12.431676 gwtc_tools-0.1.0/setup.cfg
--rw-r--r--   0 channa     (502) staff       (20)       92 2023-11-02 15:10:15.000000 gwtc_tools-0.1.0/setup.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.414025 gwtc_tools-0.1.0/src/
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.423975 gwtc_tools-0.1.0/src/catalog_pipeline/
--rw-r--r--   0 channa     (502) staff       (20)       51 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/catalog_pipeline/__init__.py
--rw-r--r--   0 channa     (502) staff       (20)     5835 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/catalog_pipeline/aggregate_data.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.427514 gwtc_tools-0.1.0/src/gwtc/
--rw-r--r--   0 channa     (502) staff       (20)      324 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/__init__.py
--rw-r--r--   0 channa     (502) staff       (20)      462 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc/_version.py
--rw-r--r--   0 channa     (502) staff       (20)    10091 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc.py
--rwxr-xr-x   0 channa     (502) staff       (20)     1301 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc_create_from_query.py
--rwxr-xr-x   0 channa     (502) staff       (20)     1480 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc_diff.py
--rwxr-xr-x   0 channa     (502) staff       (20)     2516 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc_get_gevent_coinc_files.py
--rw-r--r--   0 channa     (502) staff       (20)     8723 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc_gracedb.py
--rwxr-xr-x   0 channa     (502) staff       (20)     4337 2024-04-17 16:37:35.000000 gwtc_tools-0.1.0/src/gwtc/gwtc_update_pipeline_gevents.py
-drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-17 17:37:12.429862 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/
--rw-r--r--   0 channa     (502) staff       (20)     7260 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 channa     (502) staff       (20)     1174 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 channa     (502) staff       (20)        1 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 channa     (502) staff       (20)      315 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 channa     (502) staff       (20)       13 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/requires.txt
--rw-r--r--   0 channa     (502) staff       (20)       22 2024-04-17 17:37:12.000000 gwtc_tools-0.1.0/src/gwtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.617596 gwtc_tools-0.1.1/
+-rw-r--r--   0 channa     (502) staff       (20)       97 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/.gitignore
+-rw-r--r--   0 channa     (502) staff       (20)      865 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0 channa     (502) staff       (20)      677 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 channa     (502) staff       (20)     1078 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/LICENSE.md
+-rw-r--r--   0 channa     (502) staff       (20)     7280 2024-04-18 13:25:34.617411 gwtc_tools-0.1.1/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)     6339 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/README.md
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.597830 gwtc_tools-0.1.1/docs/
+-rw-r--r--   0 channa     (502) staff       (20)      638 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/Makefile
+-rw-r--r--   0 channa     (502) staff       (20)      804 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/make.bat
+-rw-r--r--   0 channa     (502) staff       (20)       59 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.599116 gwtc_tools-0.1.1/docs/source/
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.600293 gwtc_tools-0.1.1/docs/source/_templates/
+-rw-r--r--   0 channa     (502) staff       (20)      662 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 channa     (502) staff       (20)     1408 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 channa     (502) staff       (20)     2507 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/source/conf.py
+-rw-r--r--   0 channa     (502) staff       (20)      484 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/docs/source/index.rst
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.607015 gwtc_tools-0.1.1/examples/
+-rw-r--r--   0 channa     (502) staff       (20)     1415 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)     1440 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)   115407 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)       91 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/H1L1-SPIIR_AllSky_PASTRO-1376883065-0.json
+-rw-r--r--   0 channa     (502) staff       (20)     1416 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz
+-rw-r--r--   0 channa     (502) staff       (20)       58 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/L1-GSTLAL_AllSky_PASTRO-1368783503-0.json
+-rw-r--r--   0 channa     (502) staff       (20)     3460 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/README.md
+-rw-r--r--   0 channa     (502) staff       (20)      114 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/gstlalv1.yaml
+-rw-r--r--   0 channa     (502) staff       (20)      212 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/examples/gstlalv2.yaml
+-rw-r--r--   0 channa     (502) staff       (20)     1635 2024-04-18 13:23:20.000000 gwtc_tools-0.1.1/pyproject.toml
+-rw-r--r--   0 channa     (502) staff       (20)      855 2024-04-18 13:25:34.618753 gwtc_tools-0.1.1/setup.cfg
+-rw-r--r--   0 channa     (502) staff       (20)       92 2023-11-02 15:10:15.000000 gwtc_tools-0.1.1/setup.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.592819 gwtc_tools-0.1.1/src/
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.608150 gwtc_tools-0.1.1/src/catalog_pipeline/
+-rw-r--r--   0 channa     (502) staff       (20)       51 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/catalog_pipeline/__init__.py
+-rw-r--r--   0 channa     (502) staff       (20)     5835 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/catalog_pipeline/aggregate_data.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.613046 gwtc_tools-0.1.1/src/gwtc/
+-rw-r--r--   0 channa     (502) staff       (20)      324 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/__init__.py
+-rw-r--r--   0 channa     (502) staff       (20)      442 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc/_version.py
+-rw-r--r--   0 channa     (502) staff       (20)    10091 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     1301 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc_create_from_query.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     1480 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc_diff.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     2516 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc_get_gevent_coinc_files.py
+-rw-r--r--   0 channa     (502) staff       (20)     8723 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc_gracedb.py
+-rwxr-xr-x   0 channa     (502) staff       (20)     4337 2024-04-17 16:37:35.000000 gwtc_tools-0.1.1/src/gwtc/gwtc_update_pipeline_gevents.py
+drwxr-xr-x   0 channa     (502) staff       (20)        0 2024-04-18 13:25:34.616525 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/
+-rw-r--r--   0 channa     (502) staff       (20)     7280 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 channa     (502) staff       (20)     1174 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 channa     (502) staff       (20)        1 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 channa     (502) staff       (20)      315 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 channa     (502) staff       (20)       18 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/requires.txt
+-rw-r--r--   0 channa     (502) staff       (20)       22 2024-04-18 13:25:34.000000 gwtc_tools-0.1.1/src/gwtc_tools.egg-info/top_level.txt
```

### Comparing `gwtc_tools-0.1.0/.gitlab-ci.yml` & `gwtc_tools-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/.pre-commit-config.yaml` & `gwtc_tools-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/LICENSE.md` & `gwtc_tools-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/PKG-INFO` & `gwtc_tools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gwtc-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for gwtc operations, including interactions with gracedb
 Home-page: https://git.ligo.org/chad-hanna/gwtc
 Author: Chad Hanna
 Author-email: Chad Hanna <chad.hanna@ligo.org>, Alexander Pace <alexander.pace@ligo.org>, Divya Singh <divya.singh@ligo.org>, Leo Tsukada <leo.tsukada@ligo.org>, Patrick Godwin <patrick.godwin@ligo.org>, Prathamesh Joshi <prathamesh.joshi@ligo.org>, Becca Ewing <rebecca.ewing@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/chad-hanna/gwtc
 Project-URL: Bug Tracker, https://git.ligo.org/chad-hanna/gwtc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ligo-gracedb
+Requires-Dist: yaml
 
 # gwtc
 
 A library for creating and interacting with Gravitational Wave Transient Catalogs in gracedb.
 
 [[_TOC_]]
```

### Comparing `gwtc_tools-0.1.0/README.md` & `gwtc_tools-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/docs/Makefile` & `gwtc_tools-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/docs/make.bat` & `gwtc_tools-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/docs/source/_templates/custom-class-template.rst` & `gwtc_tools-0.1.1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/docs/source/_templates/custom-module-template.rst` & `gwtc_tools-0.1.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/docs/source/conf.py` & `gwtc_tools-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz` & `gwtc_tools-0.1.1/examples/H1-GSTLAL_AllSky-1368009034-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz` & `gwtc_tools-0.1.1/examples/H1L1-GSTLAL_AllSky-1376883065-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz` & `gwtc_tools-0.1.1/examples/H1L1-SPIIR_AllSky-1376883065-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz` & `gwtc_tools-0.1.1/examples/L1-GSTLAL_AllSky-1368783503-0.xml.gz`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/examples/README.md` & `gwtc_tools-0.1.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/pyproject.toml` & `gwtc_tools-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools_scm]
 write_to = "src/gwtc/_version.py"
 
 
 [project]
 name = "gwtc-tools"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Chad Hanna", email="chad.hanna@ligo.org" },
   { name="Alexander Pace", email="alexander.pace@ligo.org" },
   { name="Divya Singh", email="divya.singh@ligo.org" },
   { name="Leo Tsukada", email="leo.tsukada@ligo.org" },
   { name="Patrick Godwin", email="patrick.godwin@ligo.org" },
   { name="Prathamesh Joshi", email="prathamesh.joshi@ligo.org" },
@@ -28,15 +28,16 @@
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "ligo-gracedb"
+    "ligo-gracedb",
+    "yaml"
 ]
 
 [project.scripts]
     gwtc_test = "gwtc:gwtc_test"
     gwtc_update_pipeline_gevents = "gwtc:gwtc_update_pipeline_gevents"
     gwtc_diff = "gwtc:gwtc_diff"
     gwtc_get_gevent_coinc_files = "gwtc:gwtc_get_gevent_coinc_files"
```

### Comparing `gwtc_tools-0.1.0/setup.cfg` & `gwtc_tools-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/catalog_pipeline/aggregate_data.py` & `gwtc_tools-0.1.1/src/catalog_pipeline/aggregate_data.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc_create_from_query.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc_create_from_query.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc_diff.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc_diff.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc_get_gevent_coinc_files.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc_get_gevent_coinc_files.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc_gracedb.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc/gwtc_update_pipeline_gevents.py` & `gwtc_tools-0.1.1/src/gwtc/gwtc_update_pipeline_gevents.py`

 * *Files identical despite different names*

### Comparing `gwtc_tools-0.1.0/src/gwtc_tools.egg-info/PKG-INFO` & `gwtc_tools-0.1.1/src/gwtc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: gwtc-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for gwtc operations, including interactions with gracedb
 Home-page: https://git.ligo.org/chad-hanna/gwtc
 Author: Chad Hanna
 Author-email: Chad Hanna <chad.hanna@ligo.org>, Alexander Pace <alexander.pace@ligo.org>, Divya Singh <divya.singh@ligo.org>, Leo Tsukada <leo.tsukada@ligo.org>, Patrick Godwin <patrick.godwin@ligo.org>, Prathamesh Joshi <prathamesh.joshi@ligo.org>, Becca Ewing <rebecca.ewing@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/chad-hanna/gwtc
 Project-URL: Bug Tracker, https://git.ligo.org/chad-hanna/gwtc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ligo-gracedb
+Requires-Dist: yaml
 
 # gwtc
 
 A library for creating and interacting with Gravitational Wave Transient Catalogs in gracedb.
 
 [[_TOC_]]
```

### Comparing `gwtc_tools-0.1.0/src/gwtc_tools.egg-info/SOURCES.txt` & `gwtc_tools-0.1.1/src/gwtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

