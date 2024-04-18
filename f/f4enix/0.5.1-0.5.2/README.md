# Comparing `tmp/f4enix-0.5.1.tar.gz` & `tmp/f4enix-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4enix-0.5.1.tar", last modified: Wed Mar  6 09:30:17 2024, max compression
+gzip compressed data, was "f4enix-0.5.2.tar", last modified: Thu Apr 18 07:01:58 2024, max compression
```

## Comparing `f4enix-0.5.1.tar` & `f4enix-0.5.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.323113 f4enix-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-03-06 09:30:10.000000 f4enix-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 09:30:10.000000 f4enix-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-06 09:30:17.323113 f4enix-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-06 09:30:10.000000 f4enix-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.315113 f4enix-0.5.1/f4enix/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.319113 f4enix-0.5.1/f4enix/input/
--rw-r--r--   0 runner    (1001) docker     (127)    51583 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/MCNPinput.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/d1suned.py
--rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/elite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/libmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    46251 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.319113 f4enix-0.5.1/f4enix/input/ww_gvr/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/meshgrids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/ratios_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16082 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/weight_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/ww_gvr/ww_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/input/xsdirpyne.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.319113 f4enix-0.5.1/f4enix/output/
--rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/MCNPoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/cuv_sampling_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/eeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/fispact_legacy_out.py
--rw-r--r--   0 runner    (1001) docker     (127)    51433 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/mctal.py
--rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/meshinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    73563 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/meshtal.py
--rw-r--r--   0 runner    (1001) docker     (127)    33393 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/output/rssa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.323113 f4enix-0.5.1/f4enix/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/resources/Isotopes.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/resources/activation_libs.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)  1119446 2024-03-06 09:30:10.000000 f4enix-0.5.1/f4enix/resources/xsdir.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.323113 f4enix-0.5.1/f4enix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-06 09:30:17.000000 f4enix-0.5.1/f4enix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-06 09:30:17.000000 f4enix-0.5.1/f4enix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 09:30:17.000000 f4enix-0.5.1/f4enix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-06 09:30:17.000000 f4enix-0.5.1/f4enix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 09:30:17.000000 f4enix-0.5.1/f4enix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-06 09:30:10.000000 f4enix-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-06 09:30:17.323113 f4enix-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:30:17.323113 f4enix-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-06 09:30:10.000000 f4enix-0.5.1/tests/test_cuv_sampling_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    13969 2024-04-18 07:01:54.000000 f4enix-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 07:01:54.000000 f4enix-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-18 07:01:58.716752 f4enix-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-18 07:01:54.000000 f4enix-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.708752 f4enix-0.5.2/f4enix/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.712752 f4enix-0.5.2/f4enix/input/
+-rw-r--r--   0 runner    (1001) docker     (127)    51583 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/MCNPinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/d1suned.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/elite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/libmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46251 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.712752 f4enix-0.5.2/f4enix/input/ww_gvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/meshgrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/ratios_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/weight_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/ww_gvr/ww_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/input/xsdirpyne.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    20866 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/MCNPoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/cuv_sampling_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/eeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/fispact_legacy_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51433 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/mctal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18915 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/meshinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73563 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/meshtal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33393 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/output/rssa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/Isotopes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17456 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/activation_libs.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)  1119446 2024-04-18 07:01:54.000000 f4enix-0.5.2/f4enix/resources/xsdir.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/f4enix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 07:01:58.000000 f4enix-0.5.2/f4enix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 07:01:54.000000 f4enix-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 07:01:58.720752 f4enix-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:01:58.716752 f4enix-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 07:01:54.000000 f4enix-0.5.2/tests/test_cuv_sampling_error.py
```

### Comparing `f4enix-0.5.1/LICENSE` & `f4enix-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/PKG-INFO` & `f4enix-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4enix
-Version: 0.5.1
+Version: 0.5.2
 Summary: API for Monte Carlo input and output parsing
 Author: F4E neutronics team
 Author-email: sc-radiationtransport@f4e.europa.eu
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs
```

### Comparing `f4enix-0.5.1/README.md` & `f4enix-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/constants.py` & `f4enix-0.5.2/f4enix/constants.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/MCNPinput.py` & `f4enix-0.5.2/f4enix/input/MCNPinput.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/auxiliary.py` & `f4enix-0.5.2/f4enix/input/auxiliary.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/d1suned.py` & `f4enix-0.5.2/f4enix/input/d1suned.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/elite.py` & `f4enix-0.5.2/f4enix/input/elite.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/libmanager.py` & `f4enix-0.5.2/f4enix/input/libmanager.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/materials.py` & `f4enix-0.5.2/f4enix/input/materials.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/cli.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/cli.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/geometry.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/geometry.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/meshgrids.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/meshgrids.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/models.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/models.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/ratios_calculation.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/ratios_calculation.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/utils.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/utils.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/weight_window.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/weight_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file includes the main class of the ww_gvr package, the WW class.
 """
+# flake8: noqa: PLR2004
 from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
 
 from f4enix.input.ww_gvr import ww_parser
 from f4enix.input.ww_gvr.geometry import Geometry
@@ -69,15 +70,18 @@
         geometry = cls._create_geometry(parse_result)
         values = cls._nested_to_values_by_particle(parse_result)
 
         return WW(file_path, geometry, values)
 
     @classmethod
     def create_gvr_from_meshtally_file(
-        cls, file_path: Pathlike, maximum_splitting_ratio: float = 5.0
+        cls,
+        file_path: Pathlike,
+        maximum_splitting_ratio: float = 5.0,
+        softening_factor: float = 1.0,
     ):
         """
         Create a WW object (a GVR) from a MCNP meshtally file using the Van Vick /
         Andrew Davis / Magic algorithm.
 
         Parameters
         ----------
@@ -93,16 +97,20 @@
         """
         file_path = Path(file_path)
         parse_result = ww_parser.read_meshtally_file(file_path)
 
         geometry = cls._create_geometry(parse_result)
         values = cls._nested_to_values_by_particle(parse_result)
         cls._convert_flux_values_to_gvr(values, maximum_splitting_ratio)
-
-        return WW(file_path, geometry, values)
+        gvr = WW(file_path, geometry, values)
+        
+        if softening_factor != 1.0:
+            gvr.soften(softening_factor)
+        
+        return gvr
 
     @staticmethod
     def _create_geometry(parse_result: ParseResult) -> Geometry:
         coarse_vectors, fine_vectors = decompose_b2_vectors(parse_result.b2_vectors)
         return Geometry(parse_result.header, coarse_vectors, fine_vectors)
 
     @staticmethod
```

### Comparing `f4enix-0.5.1/f4enix/input/ww_gvr/ww_parser.py` & `f4enix-0.5.2/f4enix/input/ww_gvr/ww_parser.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/input/xsdirpyne.py` & `f4enix-0.5.2/f4enix/input/xsdirpyne.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/MCNPoutput.py` & `f4enix-0.5.2/f4enix/output/MCNPoutput.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/cuv_sampling_error.py` & `f4enix-0.5.2/f4enix/output/cuv_sampling_error.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/eeout.py` & `f4enix-0.5.2/f4enix/output/eeout.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/fispact_legacy_out.py` & `f4enix-0.5.2/f4enix/output/fispact_legacy_out.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/mctal.py` & `f4enix-0.5.2/f4enix/output/mctal.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/meshinfo.py` & `f4enix-0.5.2/f4enix/output/meshinfo.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/meshtal.py` & `f4enix-0.5.2/f4enix/output/meshtal.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/plotter.py` & `f4enix-0.5.2/f4enix/output/plotter.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/output/rssa.py` & `f4enix-0.5.2/f4enix/output/rssa.py`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/resources/Isotopes.txt` & `f4enix-0.5.2/f4enix/resources/Isotopes.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/resources/activation_libs.xlsx` & `f4enix-0.5.2/f4enix/resources/activation_libs.xlsx`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix/resources/xsdir.txt` & `f4enix-0.5.2/f4enix/resources/xsdir.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix.egg-info/PKG-INFO` & `f4enix-0.5.2/f4enix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4enix
-Version: 0.5.1
+Version: 0.5.2
 Summary: API for Monte Carlo input and output parsing
 Author: F4E neutronics team
 Author-email: sc-radiationtransport@f4e.europa.eu
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs
```

### Comparing `f4enix-0.5.1/f4enix.egg-info/SOURCES.txt` & `f4enix-0.5.2/f4enix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/f4enix.egg-info/requires.txt` & `f4enix-0.5.2/f4enix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/setup.cfg` & `f4enix-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `f4enix-0.5.1/tests/test_cuv_sampling_error.py` & `f4enix-0.5.2/tests/test_cuv_sampling_error.py`

 * *Files identical despite different names*

