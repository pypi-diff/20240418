# Comparing `tmp/financefunctions-0.0.1.tar.gz` & `tmp/financefunctions-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financefunctions-0.0.1.tar", last modified: Wed Apr  3 19:14:20 2024, max compression
+gzip compressed data, was "financefunctions-0.0.2.tar", last modified: Thu Apr 18 17:59:49 2024, max compression
```

## Comparing `financefunctions-0.0.1.tar` & `financefunctions-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:14:20.322926 financefunctions-0.0.1/
--rw-r--r--   0 neutro2    (501) staff       (20)     8036 2024-04-03 19:14:20.322447 financefunctions-0.0.1/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-04-03 17:30:22.000000 financefunctions-0.0.1/license
--rw-r--r--   0 neutro2    (501) staff       (20)     1021 2024-04-03 17:37:32.000000 financefunctions-0.0.1/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     6052 2024-04-03 19:12:55.000000 financefunctions-0.0.1/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-03 19:14:20.323027 financefunctions-0.0.1/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:14:20.315007 financefunctions-0.0.1/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:14:20.318315 financefunctions-0.0.1/src/financefunctions/
--rw-r--r--   0 neutro2    (501) staff       (20)      655 2024-04-03 18:01:53.000000 financefunctions-0.0.1/src/financefunctions/__init__.py
--rw-r--r--   0 neutro2    (501) staff       (20)     6070 2024-04-03 19:00:01.000000 financefunctions-0.0.1/src/financefunctions/dataframes.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-03 19:14:20.321603 financefunctions-0.0.1/src/financefunctions.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     8036 2024-04-03 19:14:20.000000 financefunctions-0.0.1/src/financefunctions.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      337 2024-04-03 19:14:20.000000 financefunctions-0.0.1/src/financefunctions.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-03 19:14:20.000000 financefunctions-0.0.1/src/financefunctions.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       60 2024-04-03 19:14:20.000000 financefunctions-0.0.1/src/financefunctions.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       17 2024-04-03 19:14:20.000000 financefunctions-0.0.1/src/financefunctions.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-18 17:59:49.408745 financefunctions-0.0.2/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8036 2024-04-18 17:59:49.408110 financefunctions-0.0.2/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-04-03 17:30:22.000000 financefunctions-0.0.2/license
+-rw-r--r--   0 neutro2    (501) staff       (20)     1021 2024-04-18 17:18:12.000000 financefunctions-0.0.2/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     6052 2024-04-03 19:12:55.000000 financefunctions-0.0.2/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-18 17:59:49.408881 financefunctions-0.0.2/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-18 17:59:49.401061 financefunctions-0.0.2/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-18 17:59:49.404597 financefunctions-0.0.2/src/financefunctions/
+-rw-r--r--   0 neutro2    (501) staff       (20)      856 2024-04-18 17:38:37.000000 financefunctions-0.0.2/src/financefunctions/__init__.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     6187 2024-04-18 17:50:52.000000 financefunctions-0.0.2/src/financefunctions/dataframes.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     2541 2024-04-18 17:37:25.000000 financefunctions-0.0.2/src/financefunctions/functions.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     6887 2024-04-18 17:41:33.000000 financefunctions-0.0.2/src/financefunctions/series.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-18 17:59:49.407138 financefunctions-0.0.2/src/financefunctions.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     8036 2024-04-18 17:59:49.000000 financefunctions-0.0.2/src/financefunctions.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      402 2024-04-18 17:59:49.000000 financefunctions-0.0.2/src/financefunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-18 17:59:49.000000 financefunctions-0.0.2/src/financefunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       60 2024-04-18 17:59:49.000000 financefunctions-0.0.2/src/financefunctions.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       17 2024-04-18 17:59:49.000000 financefunctions-0.0.2/src/financefunctions.egg-info/top_level.txt
```

### Comparing `financefunctions-0.0.1/PKG-INFO` & `financefunctions-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financefunctions
-Version: 0.0.1
+Version: 0.0.2
 Summary: a simple package that creates some convenience functions for financial data
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basefunctions>=0.3.5
+Requires-Dist: basefunctions>=0.3.8
 Requires-Dist: pandas>=2.0
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest>=7.4; extra == "test"
 
 # Introduction
```

### Comparing `financefunctions-0.0.1/license` & `financefunctions-0.0.2/license`

 * *Files identical despite different names*

### Comparing `financefunctions-0.0.1/pyproject.toml` & `financefunctions-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "financefunctions"
-version = "0.0.1"
+version = "0.0.2"
 
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "a simple package that creates some convenience functions for financial data"
 
 readme = "readme.md"
 license = { file = "license" }
 requires-python = ">=3.10"
@@ -18,15 +18,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-  "basefunctions >= 0.3.5",
+  "basefunctions >= 0.3.8",
   "pandas >= 2.0",
 ]
 
 [project.optional-dependencies]
 dev = [
 ]
 test = [
```

### Comparing `financefunctions-0.0.1/readme.md` & `financefunctions-0.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `financefunctions-0.0.1/src/financefunctions/dataframes.py` & `financefunctions-0.0.2/src/financefunctions/dataframes.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,8 +202,11 @@
         Returns
         -------
         pandas dataframe
             subcolumns of dataframe
         """
         if isinstance(cols, str):
             cols = [cols]
-        return self._obj.loc[:, (slice(None), cols)]
+        if isinstance(self._obj.columns, pd.MultiIndex):
+            return self._obj.loc[:, (slice(None), cols)]
+        else:
+            return self._obj.loc[:, cols]
```

### Comparing `financefunctions-0.0.1/src/financefunctions.egg-info/PKG-INFO` & `financefunctions-0.0.2/src/financefunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financefunctions
-Version: 0.0.1
+Version: 0.0.2
 Summary: a simple package that creates some convenience functions for financial data
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basefunctions>=0.3.5
+Requires-Dist: basefunctions>=0.3.8
 Requires-Dist: pandas>=2.0
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: pytest>=7.4; extra == "test"
 
 # Introduction
```

