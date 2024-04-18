# Comparing `tmp/ifcclash-0.0.240408.tar.gz` & `tmp/ifcclash-0.0.240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifcclash-0.0.240408.tar", last modified: Mon Apr  8 01:20:31 2024, max compression
+gzip compressed data, was "ifcclash-0.0.240418.tar", last modified: Thu Apr 18 01:10:24 2024, max compression
```

## Comparing `ifcclash-0.0.240408.tar` & `ifcclash-0.0.240418.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:20:31.447045 ifcclash-0.0.240408/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-08 01:20:19.000000 ifcclash-0.0.240408/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-08 01:20:19.000000 ifcclash-0.0.240408/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-08 01:20:31.447045 ifcclash-0.0.240408/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:20:31.447045 ifcclash-0.0.240408/ifcclash/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 01:20:19.000000 ifcclash-0.0.240408/ifcclash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11672 2024-04-08 01:20:19.000000 ifcclash-0.0.240408/ifcclash/ifcclash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 01:20:31.447045 ifcclash-0.0.240408/ifcclash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-08 01:20:31.000000 ifcclash-0.0.240408/ifcclash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 01:20:31.000000 ifcclash-0.0.240408/ifcclash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 01:20:31.000000 ifcclash-0.0.240408/ifcclash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 01:20:31.000000 ifcclash-0.0.240408/ifcclash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 01:20:31.000000 ifcclash-0.0.240408/ifcclash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 01:20:29.000000 ifcclash-0.0.240408/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 01:20:31.447045 ifcclash-0.0.240408/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:10:24.189720 ifcclash-0.0.240418/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 01:10:19.000000 ifcclash-0.0.240418/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 01:10:19.000000 ifcclash-0.0.240418/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 01:10:24.189720 ifcclash-0.0.240418/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:10:24.185720 ifcclash-0.0.240418/ifcclash/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-18 01:10:19.000000 ifcclash-0.0.240418/ifcclash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11672 2024-04-18 01:10:19.000000 ifcclash-0.0.240418/ifcclash/ifcclash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:10:24.189720 ifcclash-0.0.240418/ifcclash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-18 01:10:24.000000 ifcclash-0.0.240418/ifcclash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 01:10:24.000000 ifcclash-0.0.240418/ifcclash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:10:24.000000 ifcclash-0.0.240418/ifcclash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 01:10:24.000000 ifcclash-0.0.240418/ifcclash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 01:10:24.000000 ifcclash-0.0.240418/ifcclash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 01:10:21.000000 ifcclash-0.0.240418/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:10:24.189720 ifcclash-0.0.240418/setup.cfg
```

### Comparing `ifcclash-0.0.240408/COPYING` & `ifcclash-0.0.240418/COPYING`

 * *Files identical despite different names*

### Comparing `ifcclash-0.0.240408/COPYING.LESSER` & `ifcclash-0.0.240418/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifcclash-0.0.240408/PKG-INFO` & `ifcclash-0.0.240418/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcclash
-Version: 0.0.240408
+Version: 0.0.240418
 Summary: IFC clash detection library to handle intersections, collisions, and clearance checks
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,clash,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcclash-0.0.240408/ifcclash/__main__.py` & `ifcclash-0.0.240418/ifcclash/__main__.py`

 * *Files identical despite different names*

### Comparing `ifcclash-0.0.240408/ifcclash/ifcclash.py` & `ifcclash-0.0.240418/ifcclash/ifcclash.py`

 * *Files identical despite different names*

### Comparing `ifcclash-0.0.240408/ifcclash.egg-info/PKG-INFO` & `ifcclash-0.0.240418/ifcclash.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifcclash
-Version: 0.0.240408
+Version: 0.0.240418
 Summary: IFC clash detection library to handle intersections, collisions, and clearance checks
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,clash,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifcclash-0.0.240408/pyproject.toml` & `ifcclash-0.0.240418/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifcclash"
-version = "0.0.240408"
+version = "0.0.240418"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC clash detection library to handle intersections, collisions, and clearance checks"
 readme = "README.md"
 keywords = ["IFC", "clash", "BIM"]
 classifiers = [
```
