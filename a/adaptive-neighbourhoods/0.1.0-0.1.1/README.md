# Comparing `tmp/adaptive_neighbourhoods-0.1.0.tar.gz` & `tmp/adaptive_neighbourhoods-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_neighbourhoods-0.1.0.tar", last modified: Wed Apr 17 15:00:02 2024, max compression
+gzip compressed data, was "adaptive_neighbourhoods-0.1.1.tar", last modified: Wed Apr 17 15:09:04 2024, max compression
```

## Comparing `adaptive_neighbourhoods-0.1.0.tar` & `adaptive_neighbourhoods-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.867542 adaptive_neighbourhoods-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.867542 adaptive_neighbourhoods-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/tests/test_iris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:09:04.000000 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 15:09:04.000000 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:09:04.000000 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 15:09:04.000000 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 15:09:04.000000 adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:09:04.834221 adaptive_neighbourhoods-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 15:08:33.000000 adaptive_neighbourhoods-0.1.1/tests/test_iris.py
```

### Comparing `adaptive_neighbourhoods-0.1.0/LICENSE` & `adaptive_neighbourhoods-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_neighbourhoods-0.1.0/PKG-INFO` & `adaptive_neighbourhoods-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_neighbourhoods
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python API for generating adapted and unique neighbourhoods for searching for adversarial examples.
 Author: Adeline Paiement, Arno Pauly, Monika Seisenberger
 Author-email: Jay Paul Morgan <j.p.morgan@swansea.ac.uk>
 Project-URL: Homepage, https://github.com/jaypmorgan/adaptive-neighbourhoods
 Project-URL: Bug Tracker, https://github.com/jaypmorgan/adaptive-neighbourhoods/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `adaptive_neighbourhoods-0.1.0/README.md` & `adaptive_neighbourhoods-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adaptive_neighbourhoods-0.1.0/pyproject.toml` & `adaptive_neighbourhoods-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive_neighbourhoods"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Jay Paul Morgan", email="j.p.morgan@swansea.ac.uk"},
   {name="Adeline Paiement"},
   {name="Arno Pauly"},
   {name="Monika Seisenberger"},
 ]
 description = "Python API for generating adapted and unique neighbourhoods for searching for adversarial examples."
```

### Comparing `adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/PKG-INFO` & `adaptive_neighbourhoods-0.1.1/src/adaptive_neighbourhoods.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_neighbourhoods
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python API for generating adapted and unique neighbourhoods for searching for adversarial examples.
 Author: Adeline Paiement, Arno Pauly, Monika Seisenberger
 Author-email: Jay Paul Morgan <j.p.morgan@swansea.ac.uk>
 Project-URL: Homepage, https://github.com/jaypmorgan/adaptive-neighbourhoods
 Project-URL: Bug Tracker, https://github.com/jaypmorgan/adaptive-neighbourhoods/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `adaptive_neighbourhoods-0.1.0/src/main.cpp` & `adaptive_neighbourhoods-0.1.1/src/main.cpp`

 * *Files identical despite different names*

### Comparing `adaptive_neighbourhoods-0.1.0/tests/test_iris.py` & `adaptive_neighbourhoods-0.1.1/tests/test_iris.py`

 * *Files identical despite different names*

