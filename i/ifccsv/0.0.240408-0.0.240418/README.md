# Comparing `tmp/ifccsv-0.0.240408.tar.gz` & `tmp/ifccsv-0.0.240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifccsv-0.0.240408.tar", last modified: Mon Apr  8 00:58:25 2024, max compression
+gzip compressed data, was "ifccsv-0.0.240418.tar", last modified: Thu Apr 18 01:11:53 2024, max compression
```

## Comparing `ifccsv-0.0.240408.tar` & `ifccsv-0.0.240418.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:25.185202 ifccsv-0.0.240408/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-08 00:58:20.000000 ifccsv-0.0.240408/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-08 00:58:20.000000 ifccsv-0.0.240408/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 00:58:25.185202 ifccsv-0.0.240408/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:58:25.185202 ifccsv-0.0.240408/ifccsv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 00:58:25.000000 ifccsv-0.0.240408/ifccsv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 00:58:25.000000 ifccsv-0.0.240408/ifccsv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:58:25.000000 ifccsv-0.0.240408/ifccsv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 00:58:25.000000 ifccsv-0.0.240408/ifccsv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:58:25.000000 ifccsv-0.0.240408/ifccsv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 00:58:23.000000 ifccsv-0.0.240408/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:58:25.185202 ifccsv-0.0.240408/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/ifccsv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:11:53.000000 ifccsv-0.0.240418/ifccsv.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21294 2024-04-18 01:11:49.000000 ifccsv-0.0.240418/ifccsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-18 01:11:51.000000 ifccsv-0.0.240418/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:11:53.745140 ifccsv-0.0.240418/setup.cfg
```

### Comparing `ifccsv-0.0.240408/COPYING` & `ifccsv-0.0.240418/COPYING`

 * *Files identical despite different names*

### Comparing `ifccsv-0.0.240408/COPYING.LESSER` & `ifccsv-0.0.240418/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifccsv-0.0.240408/PKG-INFO` & `ifccsv-0.0.240418/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifccsv
-Version: 0.0.240408
+Version: 0.0.240418
 Summary: IFC import and export from CSV, XLSX, ODS, and Pandas Dataframes
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,CSV,XLS,XLSX,ODS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifccsv-0.0.240408/ifccsv.egg-info/PKG-INFO` & `ifccsv-0.0.240418/ifccsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifccsv
-Version: 0.0.240408
+Version: 0.0.240418
 Summary: IFC import and export from CSV, XLSX, ODS, and Pandas Dataframes
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,CSV,XLS,XLSX,ODS,BIM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ifccsv-0.0.240408/pyproject.toml` & `ifccsv-0.0.240418/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifccsv"
-version = "0.0.240408"
+version = "0.0.240418"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC import and export from CSV, XLSX, ODS, and Pandas Dataframes"
 readme = "README.md"
 keywords = ["IFC", "CSV", "XLS", "XLSX", "ODS", "BIM"]
 classifiers = [
@@ -20,10 +20,9 @@
 ]
 
 [project.urls]
 Homepage = "http://ifcopenshell.org"
 Documentation = "https://docs.ifcopenshell.org"
 Issues = "https://github.com/IfcOpenShell/IfcOpenShell/issues"
 
-[tool.setuptools.packages.find]
-include = ["ifccsv"]
-exclude = ["test*"]
+[tool.setuptools]
+py-modules = ["ifccsv"]
```

