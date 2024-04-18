# Comparing `tmp/ipytoolbox-0.2.0.tar.gz` & `tmp/ipytoolbox-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipytoolbox-0.2.0.tar", last modified: Sat Dec 16 03:08:47 2023, max compression
+gzip compressed data, was "ipytoolbox-0.3.0.tar", last modified: Thu Apr 18 18:17:34 2024, max compression
```

## Comparing `ipytoolbox-0.2.0.tar` & `ipytoolbox-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.636261 ipytoolbox-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.636261 ipytoolbox-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/.github/workflows/pre-commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41642 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.636261 ipytoolbox-0.2.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   209255 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.636261 ipytoolbox-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/src/ipytoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/src/ipytoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/src/ipytoolbox/magics.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41642 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-16 03:08:47.000000 ipytoolbox-0.2.0/src/ipytoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 03:08:47.640261 ipytoolbox-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-16 03:08:38.000000 ipytoolbox-0.2.0/tests/test_magics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.601309 ipytoolbox-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.597309 ipytoolbox-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.597309 ipytoolbox-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41682 2024-04-18 18:17:34.601309 ipytoolbox-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.597309 ipytoolbox-0.3.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   209255 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:17:34.601309 ipytoolbox-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.597309 ipytoolbox-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.597309 ipytoolbox-0.3.0/src/ipytoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/src/ipytoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/src/ipytoolbox/magics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.601309 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41682 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 18:17:34.000000 ipytoolbox-0.3.0/src/ipytoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:17:34.601309 ipytoolbox-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 18:17:28.000000 ipytoolbox-0.3.0/tests/test_magics.py
```

### Comparing `ipytoolbox-0.2.0/.github/workflows/ci.yaml` & `ipytoolbox-0.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ipytoolbox-0.2.0/.pre-commit-config.yaml` & `ipytoolbox-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ipytoolbox-0.2.0/LICENSE` & `ipytoolbox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipytoolbox-0.2.0/PKG-INFO` & `ipytoolbox-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipytoolbox
-Version: 0.2.0
+Version: 0.3.0
 Summary: A collection of IPython magic commands and other utilities
 Author-email: Carl Thomé <carlthome@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,22 +681,21 @@
 # ipytoolbox
 
 A collection of IPython magic commands and other utilities.
 
 ## Features
 
 ### `%autocuda`
-
-Automatically select the local CUDA device(s) with most free memory.
+- A line magic to automatically select the local CUDA device(s) with the most free memory.
 
 <img width="673" alt="image" src="https://github.com/carlthome/ipytoolbox/assets/1595907/7634b369-1c68-4e69-a2fd-fc938c7a2261">
 
-### `%animate`
+### `%%animate`
 
-Automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
+- A cell magic to automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
 
 [Example notebook](./notebooks/demo.ipynb)
 
 ## Install
 
 First make sure Python is installed, then run:
```

### Comparing `ipytoolbox-0.2.0/README.md` & `ipytoolbox-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # ipytoolbox
 
 A collection of IPython magic commands and other utilities.
 
 ## Features
 
 ### `%autocuda`
-
-Automatically select the local CUDA device(s) with most free memory.
+- A line magic to automatically select the local CUDA device(s) with the most free memory.
 
 <img width="673" alt="image" src="https://github.com/carlthome/ipytoolbox/assets/1595907/7634b369-1c68-4e69-a2fd-fc938c7a2261">
 
-### `%animate`
+### `%%animate`
 
-Automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
+- A cell magic to automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
 
 [Example notebook](./notebooks/demo.ipynb)
 
 ## Install
 
 First make sure Python is installed, then run:
```

### Comparing `ipytoolbox-0.2.0/notebooks/demo.ipynb` & `ipytoolbox-0.3.0/notebooks/demo.ipynb`

 * *Files identical despite different names*

### Comparing `ipytoolbox-0.2.0/pyproject.toml` & `ipytoolbox-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipytoolbox-0.2.0/src/ipytoolbox.egg-info/PKG-INFO` & `ipytoolbox-0.3.0/src/ipytoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipytoolbox
-Version: 0.2.0
+Version: 0.3.0
 Summary: A collection of IPython magic commands and other utilities
 Author-email: Carl Thomé <carlthome@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,22 +681,21 @@
 # ipytoolbox
 
 A collection of IPython magic commands and other utilities.
 
 ## Features
 
 ### `%autocuda`
-
-Automatically select the local CUDA device(s) with most free memory.
+- A line magic to automatically select the local CUDA device(s) with the most free memory.
 
 <img width="673" alt="image" src="https://github.com/carlthome/ipytoolbox/assets/1595907/7634b369-1c68-4e69-a2fd-fc938c7a2261">
 
-### `%animate`
+### `%%animate`
 
-Automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
+- A cell magic to automatically capture `plt.plot(); plt.show()` calls and display them as an animation once the cell has finished executing.
 
 [Example notebook](./notebooks/demo.ipynb)
 
 ## Install
 
 First make sure Python is installed, then run:
```

### Comparing `ipytoolbox-0.2.0/tests/test_magics.py` & `ipytoolbox-0.3.0/tests/test_magics.py`

 * *Files identical despite different names*

