# Comparing `tmp/hydamo_validation-1.3.0b1.tar.gz` & `tmp/hydamo_validation-1.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydamo_validation-1.3.0b1.tar", last modified: Tue Apr 16 10:33:46 2024, max compression
+gzip compressed data, was "hydamo_validation-1.3.0b2.tar", last modified: Thu Apr 18 14:05:44 2024, max compression
```

## Comparing `hydamo_validation-1.3.0b1.tar` & `hydamo_validation-1.3.0b2.tar`

### file list

```diff
@@ -1,40 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 10:33:46.545471 hydamo_validation-1.3.0b1/
--rw-rw-rw-   0        0        0     1098 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b1/LICENSE
--rw-rw-rw-   0        0        0     1808 2024-04-16 10:33:46.544474 hydamo_validation-1.3.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-04-16 10:17:00.000000 hydamo_validation-1.3.0b1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 10:33:46.493201 hydamo_validation-1.3.0b1/hydamo_validation/
--rw-rw-rw-   0        0        0      491 2024-04-16 09:58:27.000000 hydamo_validation-1.3.0b1/hydamo_validation/__init__.py
--rw-rw-rw-   0        0        0    15508 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b1/hydamo_validation/datamodel.py
--rw-rw-rw-   0        0        0     3846 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b1/hydamo_validation/datasets.py
--rw-rw-rw-   0        0        0     5682 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b1/hydamo_validation/geometry.py
--rw-rw-rw-   0        0        0    14791 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b1/hydamo_validation/logical_validation.py
--rw-rw-rw-   0        0        0     2980 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/hydamo_validation/styles.py
--rw-rw-rw-   0        0        0     8330 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/hydamo_validation/summaries.py
--rw-rw-rw-   0        0        0    10757 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/hydamo_validation/syntax_validation.py
--rw-rw-rw-   0        0        0     2170 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/hydamo_validation/utils.py
--rw-rw-rw-   0        0        0    12709 2024-04-16 10:18:20.000000 hydamo_validation-1.3.0b1/hydamo_validation/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:33:46.543477 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/
--rw-rw-rw-   0        0        0     1808 2024-04-16 10:33:46.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2024-04-16 10:33:46.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 10:33:46.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-16 10:33:46.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 10:33:46.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 10:11:43.000000 hydamo_validation-1.3.0b1/hydamo_validation.egg-info/zip-safe
--rw-rw-rw-   0        0        0      847 2024-04-16 09:40:42.000000 hydamo_validation-1.3.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 10:33:46.546467 hydamo_validation-1.3.0b1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-09 11:35:36.000000 hydamo_validation-1.3.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:33:46.542482 hydamo_validation-1.3.0b1/tests/
--rw-rw-rw-   0        0        0     1069 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b1/tests/test_datasets.py
--rw-rw-rw-   0        0        0      970 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b1/tests/test_dommelerwaard.py
--rw-rw-rw-   0        0        0     4812 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_general_functions.py
--rw-rw-rw-   0        0        0     3468 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_hydamo_2_2.py
--rw-rw-rw-   0        0        0      823 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b1/tests/test_init.py
--rw-rw-rw-   0        0        0     2638 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b1/tests/test_logic_functions.py
--rw-rw-rw-   0        0        0     3205 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b1/tests/test_not_overlapping.py
--rw-rw-rw-   0        0        0     2572 2024-04-16 10:23:56.000000 hydamo_validation-1.3.0b1/tests/test_productie.py
--rw-rw-rw-   0        0        0      991 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_structures_at_interersections.py
--rw-rw-rw-   0        0        0     3003 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_summaries.py
--rw-rw-rw-   0        0        0     4660 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_topologic_functions.py
--rw-rw-rw-   0        0        0     1592 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b1/tests/test_validationrules.py
--rw-rw-rw-   0        0        0     4597 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b1/tests/test_wrij.py
--rw-rw-rw-   0        0        0      761 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b1/tests/test_wrij_profielen.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.206495 hydamo_validation-1.3.0b2/
+-rw-rw-rw-   0        0        0     1098 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/LICENSE
+-rw-rw-rw-   0        0        0     1808 2024-04-18 14:05:44.204638 hydamo_validation-1.3.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-04-16 10:17:00.000000 hydamo_validation-1.3.0b2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.012695 hydamo_validation-1.3.0b2/hydamo_validation/
+-rw-rw-rw-   0        0        0      559 2024-04-18 14:01:29.000000 hydamo_validation-1.3.0b2/hydamo_validation/__init__.py
+-rw-rw-rw-   0        0        0    15508 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b2/hydamo_validation/datamodel.py
+-rw-rw-rw-   0        0        0     3846 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/datasets.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.083827 hydamo_validation-1.3.0b2/hydamo_validation/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/functions/__init__.py
+-rw-rw-rw-   0        0        0     9408 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/functions/general.py
+-rw-rw-rw-   0        0        0     8811 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b2/hydamo_validation/functions/logic.py
+-rw-rw-rw-   0        0        0    21123 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/functions/topologic.py
+-rw-rw-rw-   0        0        0     5682 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b2/hydamo_validation/geometry.py
+-rw-rw-rw-   0        0        0    14791 2024-04-16 09:43:08.000000 hydamo_validation-1.3.0b2/hydamo_validation/logical_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:43.989321 hydamo_validation-1.3.0b2/hydamo_validation/schemas/
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.089128 hydamo_validation-1.3.0b2/hydamo_validation/schemas/hydamo/
+-rw-rw-rw-   0        0        0   137034 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/hydamo/HyDAMO_2.2.json
+-rw-rw-rw-   0        0        0   148047 2024-04-11 08:31:48.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/hydamo/HyDAMO_2.3.json
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.097540 hydamo_validation-1.3.0b2/hydamo_validation/schemas/rules/
+-rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/rules/rules_1.0.json
+-rw-rw-rw-   0        0        0    19418 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/rules/rules_1.1.json
+-rw-rw-rw-   0        0        0    19314 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/rules/rules_1.2.json
+-rw-rw-rw-   0        0        0    19321 2024-04-11 08:40:23.000000 hydamo_validation-1.3.0b2/hydamo_validation/schemas/rules/rules_1.3.json
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.139160 hydamo_validation-1.3.0b2/hydamo_validation/styles/
+-rw-rw-rw-   0        0        0    25514 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/styles/hydroobject.qml
+-rw-rw-rw-   0        0        0      772 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/styles/hydroobject.sld
+-rw-rw-rw-   0        0        0     2980 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/styles.py
+-rw-rw-rw-   0        0        0     8330 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/summaries.py
+-rw-rw-rw-   0        0        0    10757 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/syntax_validation.py
+-rw-rw-rw-   0        0        0     2170 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/hydamo_validation/utils.py
+-rw-rw-rw-   0        0        0    12709 2024-04-16 10:18:20.000000 hydamo_validation-1.3.0b2/hydamo_validation/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.183055 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/
+-rw-rw-rw-   0        0        0     1808 2024-04-18 14:05:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1514 2024-04-18 14:05:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:05:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-18 14:05:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 14:05:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 10:11:43.000000 hydamo_validation-1.3.0b2/hydamo_validation.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      985 2024-04-18 14:05:36.000000 hydamo_validation-1.3.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:05:44.206892 hydamo_validation-1.3.0b2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-09 11:35:36.000000 hydamo_validation-1.3.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:05:44.179977 hydamo_validation-1.3.0b2/tests/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b2/tests/test_datasets.py
+-rw-rw-rw-   0        0        0      970 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b2/tests/test_dommelerwaard.py
+-rw-rw-rw-   0        0        0     4812 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_general_functions.py
+-rw-rw-rw-   0        0        0     3468 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_hydamo_2_2.py
+-rw-rw-rw-   0        0        0      823 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b2/tests/test_init.py
+-rw-rw-rw-   0        0        0     2638 2024-04-16 09:33:08.000000 hydamo_validation-1.3.0b2/tests/test_logic_functions.py
+-rw-rw-rw-   0        0        0     3205 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/tests/test_not_overlapping.py
+-rw-rw-rw-   0        0        0     2572 2024-04-16 10:23:56.000000 hydamo_validation-1.3.0b2/tests/test_productie.py
+-rw-rw-rw-   0        0        0      991 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_structures_at_interersections.py
+-rw-rw-rw-   0        0        0     3003 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_summaries.py
+-rw-rw-rw-   0        0        0     4660 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_topologic_functions.py
+-rw-rw-rw-   0        0        0     1592 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/tests/test_validationrules.py
+-rw-rw-rw-   0        0        0     4597 2024-04-05 13:12:41.000000 hydamo_validation-1.3.0b2/tests/test_wrij.py
+-rw-rw-rw-   0        0        0      761 2024-04-05 13:12:36.000000 hydamo_validation-1.3.0b2/tests/test_wrij_profielen.py
```

### Comparing `hydamo_validation-1.3.0b1/LICENSE` & `hydamo_validation-1.3.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/PKG-INFO` & `hydamo_validation-1.3.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydamo_validation
-Version: 1.3.0b1
+Version: 1.3.0b2
 Summary: Validation module for HyDAMO data
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>
 License: MIT
 Project-URL: Source, https://github.com/HetWaterschapshuis/HyDAMOValidatieModule
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydamo_validation-1.3.0b1/README.md` & `hydamo_validation-1.3.0b2/README.md`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/datamodel.py` & `hydamo_validation-1.3.0b2/hydamo_validation/datamodel.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/datasets.py` & `hydamo_validation-1.3.0b2/hydamo_validation/datasets.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/geometry.py` & `hydamo_validation-1.3.0b2/hydamo_validation/geometry.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/logical_validation.py` & `hydamo_validation-1.3.0b2/hydamo_validation/logical_validation.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/styles.py` & `hydamo_validation-1.3.0b2/hydamo_validation/styles.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/summaries.py` & `hydamo_validation-1.3.0b2/hydamo_validation/summaries.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/syntax_validation.py` & `hydamo_validation-1.3.0b2/hydamo_validation/syntax_validation.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/utils.py` & `hydamo_validation-1.3.0b2/hydamo_validation/utils.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation/validator.py` & `hydamo_validation-1.3.0b2/hydamo_validation/validator.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation.egg-info/PKG-INFO` & `hydamo_validation-1.3.0b2/hydamo_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydamo_validation
-Version: 1.3.0b1
+Version: 1.3.0b2
 Summary: Validation module for HyDAMO data
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>
 License: MIT
 Project-URL: Source, https://github.com/HetWaterschapshuis/HyDAMOValidatieModule
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydamo_validation-1.3.0b1/hydamo_validation.egg-info/SOURCES.txt` & `hydamo_validation-1.3.0b2/hydamo_validation.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 hydamo_validation/validator.py
 hydamo_validation.egg-info/PKG-INFO
 hydamo_validation.egg-info/SOURCES.txt
 hydamo_validation.egg-info/dependency_links.txt
 hydamo_validation.egg-info/requires.txt
 hydamo_validation.egg-info/top_level.txt
 hydamo_validation.egg-info/zip-safe
+hydamo_validation/functions/__init__.py
+hydamo_validation/functions/general.py
+hydamo_validation/functions/logic.py
+hydamo_validation/functions/topologic.py
+hydamo_validation/schemas/hydamo/HyDAMO_2.2.json
+hydamo_validation/schemas/hydamo/HyDAMO_2.3.json
+hydamo_validation/schemas/rules/rules_1.0.json
+hydamo_validation/schemas/rules/rules_1.1.json
+hydamo_validation/schemas/rules/rules_1.2.json
+hydamo_validation/schemas/rules/rules_1.3.json
+hydamo_validation/styles/hydroobject.qml
+hydamo_validation/styles/hydroobject.sld
 tests/test_datasets.py
 tests/test_dommelerwaard.py
 tests/test_general_functions.py
 tests/test_hydamo_2_2.py
 tests/test_init.py
 tests/test_logic_functions.py
 tests/test_not_overlapping.py
```

### Comparing `hydamo_validation-1.3.0b1/pyproject.toml` & `hydamo_validation-1.3.0b2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -33,11 +33,14 @@
 [tool.setuptools]
 zip-safe = true
 
 [tool.setuptools.dynamic]
 version = { attr = "hydamo_validation.__version__" }
 
 [tool.setuptools.packages.find]
-include = ["hydamo_validation"]
+include = ["hydamo_validation", "hydamo_validation.*"]
+
+[tool.setuptools.package-data]
+hydamo_validation = ["schemas/hydamo/*.json","schemas/rules/*.json", "styles/*.*"]
 
 [project.urls]
 Source = "https://github.com/HetWaterschapshuis/HyDAMOValidatieModule"
```

### Comparing `hydamo_validation-1.3.0b1/tests/test_datasets.py` & `hydamo_validation-1.3.0b2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_dommelerwaard.py` & `hydamo_validation-1.3.0b2/tests/test_dommelerwaard.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_general_functions.py` & `hydamo_validation-1.3.0b2/tests/test_general_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_hydamo_2_2.py` & `hydamo_validation-1.3.0b2/tests/test_hydamo_2_2.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_init.py` & `hydamo_validation-1.3.0b2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_logic_functions.py` & `hydamo_validation-1.3.0b2/tests/test_logic_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_not_overlapping.py` & `hydamo_validation-1.3.0b2/tests/test_not_overlapping.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_productie.py` & `hydamo_validation-1.3.0b2/tests/test_productie.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_structures_at_interersections.py` & `hydamo_validation-1.3.0b2/tests/test_structures_at_interersections.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_summaries.py` & `hydamo_validation-1.3.0b2/tests/test_summaries.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_topologic_functions.py` & `hydamo_validation-1.3.0b2/tests/test_topologic_functions.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_validationrules.py` & `hydamo_validation-1.3.0b2/tests/test_validationrules.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_wrij.py` & `hydamo_validation-1.3.0b2/tests/test_wrij.py`

 * *Files identical despite different names*

### Comparing `hydamo_validation-1.3.0b1/tests/test_wrij_profielen.py` & `hydamo_validation-1.3.0b2/tests/test_wrij_profielen.py`

 * *Files identical despite different names*

