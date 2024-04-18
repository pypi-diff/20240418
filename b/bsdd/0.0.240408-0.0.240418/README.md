# Comparing `tmp/bsdd-0.0.240408.tar.gz` & `tmp/bsdd-0.0.240418.tar.gz`

## Comparing `bsdd-0.0.240408.tar` & `bsdd-0.0.240418.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bsdd-0.0.240408/CITATION.cff
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bsdd-0.0.240408/Makefile
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bsdd-0.0.240408/__init__.py
--rw-r--r--   0        0        0    25316 2020-02-02 00:00:00.000000 bsdd-0.0.240408/bsdd.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bsdd-0.0.240408/tests/test_bsdd.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bsdd-0.0.240408/.gitignore
--rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 bsdd-0.0.240408/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 bsdd-0.0.240408/COPYING.LESSER
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 bsdd-0.0.240408/README.md
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 bsdd-0.0.240408/pyproject.toml
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bsdd-0.0.240408/PKG-INFO
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bsdd-0.0.240418/CITATION.cff
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 bsdd-0.0.240418/Makefile
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bsdd-0.0.240418/__init__.py
+-rw-r--r--   0        0        0    25316 2020-02-02 00:00:00.000000 bsdd-0.0.240418/bsdd.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bsdd-0.0.240418/tests/test_bsdd.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bsdd-0.0.240418/.gitignore
+-rw-r--r--   0        0        0    32473 2020-02-02 00:00:00.000000 bsdd-0.0.240418/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 bsdd-0.0.240418/COPYING.LESSER
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 bsdd-0.0.240418/README.md
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 bsdd-0.0.240418/pyproject.toml
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bsdd-0.0.240418/PKG-INFO
```

### Comparing `bsdd-0.0.240408/bsdd.py` & `bsdd-0.0.240418/bsdd.py`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/tests/test_bsdd.py` & `bsdd-0.0.240418/tests/test_bsdd.py`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/.gitignore` & `bsdd-0.0.240418/.gitignore`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/COPYING` & `bsdd-0.0.240418/COPYING`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/COPYING.LESSER` & `bsdd-0.0.240418/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/README.md` & `bsdd-0.0.240418/README.md`

 * *Files identical despite different names*

### Comparing `bsdd-0.0.240408/pyproject.toml` & `bsdd-0.0.240418/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bsdd"
-version = "0.0.240408"
+version = "0.0.240418"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "Library to interact with the buildingSMART Data Dictionary"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["IFC", "bSDD", "BIM"]
```

### Comparing `bsdd-0.0.240408/PKG-INFO` & `bsdd-0.0.240418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bsdd
-Version: 0.0.240408
+Version: 0.0.240418
 Summary: Library to interact with the buildingSMART Data Dictionary
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Author-email: Dion Moult <dion@thinkmoult.com>
 License-File: COPYING
 License-File: COPYING.LESSER
```

