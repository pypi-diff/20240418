# Comparing `tmp/bivariate-2.0.1.tar.gz` & `tmp/bivariate-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bivariate-2.0.1.tar", last modified: Tue Apr 16 20:14:25 2024, max compression
+gzip compressed data, was "bivariate-2.0.2.tar", last modified: Thu Apr 18 05:18:58 2024, max compression
```

## Comparing `bivariate-2.0.1.tar` & `bivariate-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.999677 bivariate-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-16 20:14:21.000000 bivariate-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-16 20:14:24.999677 bivariate-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-16 20:14:21.000000 bivariate-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 20:14:21.000000 bivariate-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:14:24.999677 bivariate-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.995677 bivariate-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.995677 bivariate-2.0.1/src/bivariate/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_component_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    29684 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_copula.py
--rw-r--r--   0 runner    (1001) docker     (127)    33386 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_emperical.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_fitresults.py
--rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/bivariate/class_multivar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.999677 bivariate-2.0.1/src/bivariate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-16 20:14:24.000000 bivariate-2.0.1/src/bivariate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-16 20:14:24.000000 bivariate-2.0.1/src/bivariate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:14:24.000000 bivariate-2.0.1/src/bivariate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 20:14:24.000000 bivariate-2.0.1/src/bivariate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 20:14:24.000000 bivariate-2.0.1/src/bivariate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.999677 bivariate-2.0.1/src/component_reliability/
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-04-16 20:14:21.000000 bivariate-2.0.1/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:14:24.999677 bivariate-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-16 20:14:21.000000 bivariate-2.0.1/tests/test_bivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-18 05:18:54.000000 bivariate-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-18 05:18:58.704314 bivariate-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-18 05:18:54.000000 bivariate-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-18 05:18:54.000000 bivariate-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:18:58.704314 bivariate-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.700313 bivariate-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/bivariate/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_component_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29684 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_copula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33386 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_emperical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_fitresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/bivariate/class_multivar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/bivariate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45928 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 05:18:58.000000 bivariate-2.0.2/src/bivariate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/src/component_reliability/
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-04-18 05:18:54.000000 bivariate-2.0.2/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:18:58.704314 bivariate-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-18 05:18:54.000000 bivariate-2.0.2/tests/test_bivariate.py
```

### Comparing `bivariate-2.0.1/LICENSE.txt` & `bivariate-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/PKG-INFO` & `bivariate-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivariate
-Version: 2.0.1
+Version: 2.0.2
 Summary: This package contains methods that assist in performing bivariate analysis of datasets.
 Author: Robert Lanzafame
 Author-email: r.lanzafame@tudelft.nl
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,30 +684,46 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: seaborn
 Requires-Dist: scipy
 Requires-Dist: ipykernel
 Requires-Dist: pyvinecopulib
+Requires-Dist: scikit-learn
 Provides-Extra: test
 Requires-Dist: pytest==7.4.0; extra == "test"
 Requires-Dist: pytest-cov>4.0.0; extra == "test"
 Requires-Dist: mypy==1.5.1; extra == "test"
 
 # Bivariate
 
 This package is meant to make life easier for students and teachers working on probabilistic applications. It was developed initially for MSc education at TU Delft. The focus is on visualizing multivariate distributions in 2D plots (hence the name bivariate) and making this process as easy as possible, as well as definition of the multivariate distribution and common calculations.
 
 Contributors:
 - 2022: Thirza Feenstra, Jelle Knibbe, Irene van der Veer, Caspar Jungbacker
 - 2023: Benjamin Ramousse
 - 2024: Siemen Algra, Max Guichard
 
+Version history:
+- v0.0: never published, originally stored on TU Delft GitLab, only used with students in class
+- v1.0: never published, moved to GitHub, only used with students in class (Q4, Q1 2023) and for book figures
+- v2.0: first release on PyPI for use with students. Wait for v3.0 for better organization and documentation, and for something that begins to approach stability
+
 **License:** _still working out the details, but it will eventually have a permissive license along the lines of GPL 3.0 or CC BY 4.0. Stay tuned..._
 
+## Installation instructions
+
+Using Python virtual environment:
+
+```
+PATH_TO_YOUR/python -m venv .venv
+source .venv/Scripts/activate
+python -m pip install -r requirements.txt
+```
+
 ## Guidelines - 06/10/2023 (written by Benjamin Ramousse)
 
 **NOTE THAT EVERYTHING FROM HERE AND BELOW HAS NOT BEEN UPDATED AFTER OCTOBER 1, 2023.**
 
 - `src/bivariate` contains the source code for the package
 - `tests/test_bivariate.py` is the test file used for automated testing with pytest. In particular, the syntax of the 
 methods defined in the said file relates to that of the `pytest` module.
```

### Comparing `bivariate-2.0.1/README.md` & `bivariate-2.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,31 @@
 This package is meant to make life easier for students and teachers working on probabilistic applications. It was developed initially for MSc education at TU Delft. The focus is on visualizing multivariate distributions in 2D plots (hence the name bivariate) and making this process as easy as possible, as well as definition of the multivariate distribution and common calculations.
 
 Contributors:
 - 2022: Thirza Feenstra, Jelle Knibbe, Irene van der Veer, Caspar Jungbacker
 - 2023: Benjamin Ramousse
 - 2024: Siemen Algra, Max Guichard
 
+Version history:
+- v0.0: never published, originally stored on TU Delft GitLab, only used with students in class
+- v1.0: never published, moved to GitHub, only used with students in class (Q4, Q1 2023) and for book figures
+- v2.0: first release on PyPI for use with students. Wait for v3.0 for better organization and documentation, and for something that begins to approach stability
+
 **License:** _still working out the details, but it will eventually have a permissive license along the lines of GPL 3.0 or CC BY 4.0. Stay tuned..._
 
+## Installation instructions
+
+Using Python virtual environment:
+
+```
+PATH_TO_YOUR/python -m venv .venv
+source .venv/Scripts/activate
+python -m pip install -r requirements.txt
+```
+
 ## Guidelines - 06/10/2023 (written by Benjamin Ramousse)
 
 **NOTE THAT EVERYTHING FROM HERE AND BELOW HAS NOT BEEN UPDATED AFTER OCTOBER 1, 2023.**
 
 - `src/bivariate` contains the source code for the package
 - `tests/test_bivariate.py` is the test file used for automated testing with pytest. In particular, the syntax of the 
 methods defined in the said file relates to that of the `pytest` module.
```

### Comparing `bivariate-2.0.1/pyproject.toml` & `bivariate-2.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name='bivariate'
-version='2.0.1'
+version='2.0.2'
 description='This package contains methods that assist in performing bivariate analysis of datasets.'
 license = {file = "LICENSE.txt"}
 authors = [
   {email = "r.lanzafame@tudelft.nl"},
   {name = "Robert Lanzafame"}
 ]
 readme = "README.md"
@@ -18,14 +18,15 @@
     'numpy',
     'pandas',
     'matplotlib >= 3.5.0',
     'seaborn',
     'scipy',
     'ipykernel',
     'pyvinecopulib',
+    'scikit-learn'
 ]
 
 [project.urls]
 Repository = 'https://github.com/prob-design/bivariate.git'
 
 [project.optional-dependencies]
 test = [
```

### Comparing `bivariate-2.0.1/src/bivariate/class_component_analysis.py` & `bivariate-2.0.2/src/bivariate/class_component_analysis.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate/class_copula.py` & `bivariate-2.0.2/src/bivariate/class_copula.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate/class_dataset.py` & `bivariate-2.0.2/src/bivariate/class_dataset.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate/class_emperical.py` & `bivariate-2.0.2/src/bivariate/class_emperical.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate/class_fitresults.py` & `bivariate-2.0.2/src/bivariate/class_fitresults.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate/class_multivar.py` & `bivariate-2.0.2/src/bivariate/class_multivar.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/bivariate.egg-info/PKG-INFO` & `bivariate-2.0.2/src/bivariate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bivariate
-Version: 2.0.1
+Version: 2.0.2
 Summary: This package contains methods that assist in performing bivariate analysis of datasets.
 Author: Robert Lanzafame
 Author-email: r.lanzafame@tudelft.nl
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,30 +684,46 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib>=3.5.0
 Requires-Dist: seaborn
 Requires-Dist: scipy
 Requires-Dist: ipykernel
 Requires-Dist: pyvinecopulib
+Requires-Dist: scikit-learn
 Provides-Extra: test
 Requires-Dist: pytest==7.4.0; extra == "test"
 Requires-Dist: pytest-cov>4.0.0; extra == "test"
 Requires-Dist: mypy==1.5.1; extra == "test"
 
 # Bivariate
 
 This package is meant to make life easier for students and teachers working on probabilistic applications. It was developed initially for MSc education at TU Delft. The focus is on visualizing multivariate distributions in 2D plots (hence the name bivariate) and making this process as easy as possible, as well as definition of the multivariate distribution and common calculations.
 
 Contributors:
 - 2022: Thirza Feenstra, Jelle Knibbe, Irene van der Veer, Caspar Jungbacker
 - 2023: Benjamin Ramousse
 - 2024: Siemen Algra, Max Guichard
 
+Version history:
+- v0.0: never published, originally stored on TU Delft GitLab, only used with students in class
+- v1.0: never published, moved to GitHub, only used with students in class (Q4, Q1 2023) and for book figures
+- v2.0: first release on PyPI for use with students. Wait for v3.0 for better organization and documentation, and for something that begins to approach stability
+
 **License:** _still working out the details, but it will eventually have a permissive license along the lines of GPL 3.0 or CC BY 4.0. Stay tuned..._
 
+## Installation instructions
+
+Using Python virtual environment:
+
+```
+PATH_TO_YOUR/python -m venv .venv
+source .venv/Scripts/activate
+python -m pip install -r requirements.txt
+```
+
 ## Guidelines - 06/10/2023 (written by Benjamin Ramousse)
 
 **NOTE THAT EVERYTHING FROM HERE AND BELOW HAS NOT BEEN UPDATED AFTER OCTOBER 1, 2023.**
 
 - `src/bivariate` contains the source code for the package
 - `tests/test_bivariate.py` is the test file used for automated testing with pytest. In particular, the syntax of the 
 methods defined in the said file relates to that of the `pytest` module.
```

### Comparing `bivariate-2.0.1/src/bivariate.egg-info/SOURCES.txt` & `bivariate-2.0.2/src/bivariate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py` & `bivariate-2.0.2/src/component_reliability/Case_Study_Compontent_Reliability_Tools.py`

 * *Files identical despite different names*

### Comparing `bivariate-2.0.1/tests/test_bivariate.py` & `bivariate-2.0.2/tests/test_bivariate.py`

 * *Files identical despite different names*

