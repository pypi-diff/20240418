# Comparing `tmp/evmchains-0.0.6.tar.gz` & `tmp/evmchains-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evmchains-0.0.6.tar", last modified: Sat Apr 13 00:27:28 2024, max compression
+gzip compressed data, was "evmchains-0.0.7.tar", last modified: Thu Apr 18 20:26:20 2024, max compression
```

## Comparing `evmchains-0.0.6.tar` & `evmchains-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.871504 evmchains-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.863504 evmchains-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-13 00:27:09.000000 evmchains-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 00:27:09.000000 evmchains-0.0.6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 00:27:09.000000 evmchains-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-13 00:27:09.000000 evmchains-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-13 00:27:09.000000 evmchains-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-13 00:27:28.871504 evmchains-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-13 00:27:09.000000 evmchains-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/evmchains/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.871504 evmchains-0.0.6/evmchains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-13 00:27:09.000000 evmchains-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-13 00:27:09.000000 evmchains-0.0.6/scripts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-13 00:27:28.871504 evmchains-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 00:27:09.000000 evmchains-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-13 00:27:09.000000 evmchains-0.0.6/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.070538 evmchains-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.062538 evmchains-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 20:26:03.000000 evmchains-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-18 20:26:03.000000 evmchains-0.0.7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 20:26:03.000000 evmchains-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-18 20:26:03.000000 evmchains-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-18 20:26:03.000000 evmchains-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-04-18 20:26:20.070538 evmchains-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 20:26:03.000000 evmchains-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/evmchains/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 20:26:19.000000 evmchains-0.0.7/evmchains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-18 20:26:03.000000 evmchains-0.0.7/evmchains/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/evmchains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15775 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 20:26:20.000000 evmchains-0.0.7/evmchains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 20:26:03.000000 evmchains-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-18 20:26:03.000000 evmchains-0.0.7/scripts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 20:26:20.070538 evmchains-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 20:26:03.000000 evmchains-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:26:20.066537 evmchains-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 20:26:03.000000 evmchains-0.0.7/tests/test_func.py
```

### Comparing `evmchains-0.0.6/.github/workflows/release.yaml` & `evmchains-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/.github/workflows/test.yaml` & `evmchains-0.0.7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/.gitignore` & `evmchains-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/CONTRIBUTING.md` & `evmchains-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/LICENSE` & `evmchains-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/PKG-INFO` & `evmchains-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.6
+Version: 0.0.7
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,15 +218,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic~=2.5.3
+Requires-Dist: pydantic<3,>=2.5.3
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pytest~=7.4.4; extra == "dev"
```

### Comparing `evmchains-0.0.6/README.md` & `evmchains-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/evmchains/__init__.py` & `evmchains-0.0.7/evmchains/__init__.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/evmchains/chains.py` & `evmchains-0.0.7/evmchains/chains.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/evmchains.egg-info/PKG-INFO` & `evmchains-0.0.7/evmchains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.6
+Version: 0.0.7
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,15 +218,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic~=2.5.3
+Requires-Dist: pydantic<3,>=2.5.3
 Provides-Extra: dev
 Requires-Dist: black~=23.12.1; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pytest~=7.4.4; extra == "dev"
```

### Comparing `evmchains-0.0.6/pyproject.toml` & `evmchains-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "pydantic~=2.5.3",
+    "pydantic>=2.5.3,<3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "black~=23.12.1",
     "build~=1.0.3",
```

### Comparing `evmchains-0.0.6/scripts/update.py` & `evmchains-0.0.7/scripts/update.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.6/tests/test_func.py` & `evmchains-0.0.7/tests/test_func.py`

 * *Files identical despite different names*

