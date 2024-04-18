# Comparing `tmp/write-condastat-0.2.3.tar.gz` & `tmp/write_condastat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "write-condastat-0.2.3.tar", last modified: Wed Mar 13 13:16:06 2024, max compression
+gzip compressed data, was "write_condastat-0.3.0.tar", last modified: Thu Apr 18 14:32:05 2024, max compression
```

## Comparing `write-condastat-0.2.3.tar` & `write_condastat-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:16:06.869421 write-condastat-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 13:15:59.000000 write-condastat-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-13 13:15:59.000000 write-condastat-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-13 13:16:06.869421 write-condastat-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-13 13:15:59.000000 write-condastat-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 13:15:59.000000 write-condastat-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 13:16:06.869421 write-condastat-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-13 13:15:59.000000 write-condastat-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:16:06.865421 write-condastat-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:16:06.869421 write-condastat-0.2.3/src/writecondastat/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 13:15:59.000000 write-condastat-0.2.3/src/writecondastat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24720 2024-03-13 13:15:59.000000 write-condastat-0.2.3/src/writecondastat/condastat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:15:59.000000 write-condastat-0.2.3/src/writecondastat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-13 13:15:59.000000 write-condastat-0.2.3/src/writecondastat/statdate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:16:06.869421 write-condastat-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-13 13:15:59.000000 write-condastat-0.2.3/tests/test_actual_condastat.py
--rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-03-13 13:15:59.000000 write-condastat-0.2.3/tests/test_condastat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-03-13 13:15:59.000000 write-condastat-0.2.3/tests/test_statdate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:16:06.869421 write-condastat-0.2.3/write_condastat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-03-13 13:16:06.000000 write-condastat-0.2.3/write_condastat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-13 13:16:06.000000 write-condastat-0.2.3/write_condastat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:16:06.000000 write-condastat-0.2.3/write_condastat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 13:16:06.000000 write-condastat-0.2.3/write_condastat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 13:16:06.000000 write-condastat-0.2.3/write_condastat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:05.906523 write_condastat-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 14:31:56.000000 write_condastat-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 14:31:56.000000 write_condastat-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-18 14:32:05.906523 write_condastat-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 14:31:56.000000 write_condastat-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 14:31:56.000000 write_condastat-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:32:05.906523 write_condastat-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 14:31:56.000000 write_condastat-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:05.902523 write_condastat-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:05.906523 write_condastat-0.3.0/src/writecondastat/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 14:31:56.000000 write_condastat-0.3.0/src/writecondastat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24720 2024-04-18 14:31:56.000000 write_condastat-0.3.0/src/writecondastat/condastat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:56.000000 write_condastat-0.3.0/src/writecondastat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-18 14:31:56.000000 write_condastat-0.3.0/src/writecondastat/statdate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:05.906523 write_condastat-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-18 14:31:56.000000 write_condastat-0.3.0/tests/test_actual_condastat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-04-18 14:31:56.000000 write_condastat-0.3.0/tests/test_condastat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-18 14:31:56.000000 write_condastat-0.3.0/tests/test_statdate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:32:05.906523 write_condastat-0.3.0/write_condastat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-18 14:32:05.000000 write_condastat-0.3.0/write_condastat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-18 14:32:05.000000 write_condastat-0.3.0/write_condastat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:32:05.000000 write_condastat-0.3.0/write_condastat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 14:32:05.000000 write_condastat-0.3.0/write_condastat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 14:32:05.000000 write_condastat-0.3.0/write_condastat.egg-info/top_level.txt
```

### Comparing `write-condastat-0.2.3/LICENSE` & `write_condastat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/PKG-INFO` & `write_condastat-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: write-condastat
-Version: 0.2.3
+Version: 0.3.0
 Summary: write-condastat makes it easy to collect, filter and save conda statistics to csv files.
 Home-page: https://github.com/veghdev/write-condastat
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/veghdev/write-condastat
 Project-URL: Source, https://github.com/veghdev/write-condastat
 Project-URL: Tracker, https://github.com/veghdev/write-condastat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
+Requires-Dist: click==8.1.7
+Requires-Dist: cloudpickle==3.0.0
 Requires-Dist: dask==2024.2.1
+Requires-Dist: fsspec==2024.3.1
+Requires-Dist: importlib-metadata==7.1.0
+Requires-Dist: locket==1.0.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: partd==1.4.1
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: six==1.16.0
+Requires-Dist: toolz==0.12.1
+Requires-Dist: tzdata==2024.1
+Requires-Dist: zipp==3.18.1
 
 [![PyPI version](https://badge.fury.io/py/write-condastat.svg)](https://badge.fury.io/py/write-condastat)
 [![CI-CD](https://github.com/veghdev/write-condastat/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/veghdev/write-condastat/actions/workflows/cicd.yml)
 
 
 # About The Project
```

### Comparing `write-condastat-0.2.3/README.md` & `write_condastat-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/setup.py` & `write_condastat-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = fp.read().splitlines()
 
 with open("README.md", encoding="utf8") as fp:
     long_description = fp.read()
 
 setup(
     name="write-condastat",
-    version="0.2.3",
+    version="0.3.0",
     description=(
         "write-condastat makes it easy to collect, filter and save conda statistics to csv files."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     packages=["writecondastat"],
```

### Comparing `write-condastat-0.2.3/src/writecondastat/condastat.py` & `write_condastat-0.3.0/src/writecondastat/condastat.py`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/src/writecondastat/statdate.py` & `write_condastat-0.3.0/src/writecondastat/statdate.py`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/tests/test_actual_condastat.py` & `write_condastat-0.3.0/tests/test_actual_condastat.py`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/tests/test_condastat.py` & `write_condastat-0.3.0/tests/test_condastat.py`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/tests/test_statdate.py` & `write_condastat-0.3.0/tests/test_statdate.py`

 * *Files identical despite different names*

### Comparing `write-condastat-0.2.3/write_condastat.egg-info/PKG-INFO` & `write_condastat-0.3.0/write_condastat.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: write-condastat
-Version: 0.2.3
+Version: 0.3.0
 Summary: write-condastat makes it easy to collect, filter and save conda statistics to csv files.
 Home-page: https://github.com/veghdev/write-condastat
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/veghdev/write-condastat
 Project-URL: Source, https://github.com/veghdev/write-condastat
 Project-URL: Tracker, https://github.com/veghdev/write-condastat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
+Requires-Dist: click==8.1.7
+Requires-Dist: cloudpickle==3.0.0
 Requires-Dist: dask==2024.2.1
+Requires-Dist: fsspec==2024.3.1
+Requires-Dist: importlib-metadata==7.1.0
+Requires-Dist: locket==1.0.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: packaging==24.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: partd==1.4.1
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: six==1.16.0
+Requires-Dist: toolz==0.12.1
+Requires-Dist: tzdata==2024.1
+Requires-Dist: zipp==3.18.1
 
 [![PyPI version](https://badge.fury.io/py/write-condastat.svg)](https://badge.fury.io/py/write-condastat)
 [![CI-CD](https://github.com/veghdev/write-condastat/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/veghdev/write-condastat/actions/workflows/cicd.yml)
 
 
 # About The Project
```

