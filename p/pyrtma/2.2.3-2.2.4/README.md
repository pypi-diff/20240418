# Comparing `tmp/pyrtma-2.2.3.tar.gz` & `tmp/pyrtma-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtma-2.2.3.tar", last modified: Wed Apr 17 19:50:05 2024, max compression
+gzip compressed data, was "pyrtma-2.2.4.tar", last modified: Thu Apr 18 15:52:10 2024, max compression
```

## Comparing `pyrtma-2.2.3.tar` & `pyrtma-2.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.270963 pyrtma-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 19:50:01.000000 pyrtma-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 19:50:01.000000 pyrtma-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-17 19:50:05.270963 pyrtma-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-17 19:50:01.000000 pyrtma-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-17 19:50:01.000000 pyrtma-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:50:05.270963 pyrtma-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.262963 pyrtma-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27808 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/c99.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/matlab.py
--rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/python_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/core_defs/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/core_defs/core_defs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/core_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    47924 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/generate_test_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/quicklogger_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/random_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/web_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.683206 pyrtma-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 15:52:04.000000 pyrtma-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 15:52:04.000000 pyrtma-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-18 15:52:10.683206 pyrtma-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-18 15:52:04.000000 pyrtma-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 15:52:04.000000 pyrtma-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:52:10.683206 pyrtma-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.671206 pyrtma-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.675206 pyrtma-2.2.4/src/pyrtma/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27808 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.679206 pyrtma-2.2.4/src/pyrtma/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/c99.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/matlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/python_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/compilers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.679206 pyrtma-2.2.4/src/pyrtma/core_defs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/core_defs/core_defs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/core_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/message_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/message_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47924 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.679206 pyrtma-2.2.4/src/pyrtma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/utils/generate_test_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/utils/quicklogger_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/utils/random_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-18 15:52:04.000000 pyrtma-2.2.4/src/pyrtma/web_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.679206 pyrtma-2.2.4/src/pyrtma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 15:52:10.000000 pyrtma-2.2.4/src/pyrtma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:52:10.679206 pyrtma-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-18 15:52:04.000000 pyrtma-2.2.4/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-18 15:52:04.000000 pyrtma-2.2.4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-18 15:52:04.000000 pyrtma-2.2.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-18 15:52:04.000000 pyrtma-2.2.4/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-04-18 15:52:04.000000 pyrtma-2.2.4/tests/test_validators.py
```

### Comparing `pyrtma-2.2.3/LICENSE` & `pyrtma-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/PKG-INFO` & `pyrtma-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 2.2.3
+Version: 2.2.4
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-2.2.3/README.md` & `pyrtma-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/pyproject.toml` & `pyrtma-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/__version__.py` & `pyrtma-2.2.4/src/pyrtma/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __title__ = "pyrtma"
 __description__ = "A Python compiler and client for RTMA/Dragonfly messaging system"
 __url__ = "https://github.com/pitt-rnel/pyrtma"
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "RNEL"
 __author_email__ = ""
 __license__ = "MIT"
 __copyright__ = "University of Pittsburgh Rehab Neural Engineering Labs, 2024"
 
 
 def check_compiled_version(compiled_version: str):
```

### Comparing `pyrtma-2.2.3/src/pyrtma/client.py` & `pyrtma-2.2.4/src/pyrtma/client.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compile.py` & `pyrtma-2.2.4/src/pyrtma/compile.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/c99.py` & `pyrtma-2.2.4/src/pyrtma/compilers/c99.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/info.py` & `pyrtma-2.2.4/src/pyrtma/compilers/info.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/javascript.py` & `pyrtma-2.2.4/src/pyrtma/compilers/javascript.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/matlab.py` & `pyrtma-2.2.4/src/pyrtma/compilers/matlab.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/python.py` & `pyrtma-2.2.4/src/pyrtma/compilers/python.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/python_v1.py` & `pyrtma-2.2.4/src/pyrtma/compilers/python_v1.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/compilers/yaml.py` & `pyrtma-2.2.4/src/pyrtma/compilers/yaml.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/constants.py` & `pyrtma-2.2.4/src/pyrtma/constants.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/core_defs/core_defs.yaml` & `pyrtma-2.2.4/src/pyrtma/core_defs/core_defs.yaml`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/core_defs.py` & `pyrtma-2.2.4/src/pyrtma/core_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This message def file was auto-generated by pyrtma.compile version 2.2.2"""
+"""This message def file was auto-generated by pyrtma.compile version 2.2.4"""
 
 import ctypes
 
 import pyrtma
 from pyrtma.__version__ import check_compiled_version
 from typing import ClassVar, Dict, Any
 
@@ -26,15 +26,15 @@
     Char,
     String,
     Byte,
     ByteArray,
 )
 
 
-COMPILED_PYRTMA_VERSION: str = "2.2.2"
+COMPILED_PYRTMA_VERSION: str = "2.2.4"
 check_compiled_version(COMPILED_PYRTMA_VERSION)
 
 # Constants
 MAX_MODULES: int = 200
 DYN_MOD_ID_START: int = 100
 MAX_HOSTS: int = 5
 MAX_MESSAGE_TYPES: int = 10000
```

### Comparing `pyrtma-2.2.3/src/pyrtma/exceptions.py` & `pyrtma-2.2.4/src/pyrtma/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/header.py` & `pyrtma-2.2.4/src/pyrtma/header.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/manager.py` & `pyrtma-2.2.4/src/pyrtma/manager.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/message.py` & `pyrtma-2.2.4/src/pyrtma/message.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/message_base.py` & `pyrtma-2.2.4/src/pyrtma/message_base.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/parser.py` & `pyrtma-2.2.4/src/pyrtma/parser.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/utils/generate_test_defs.py` & `pyrtma-2.2.4/src/pyrtma/utils/generate_test_defs.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/utils/print.py` & `pyrtma-2.2.4/src/pyrtma/utils/print.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/utils/quicklogger_reader.py` & `pyrtma-2.2.4/src/pyrtma/utils/quicklogger_reader.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/utils/random_fields.py` & `pyrtma-2.2.4/src/pyrtma/utils/random_fields.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/validators.py` & `pyrtma-2.2.4/src/pyrtma/validators.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma/web_manager.py` & `pyrtma-2.2.4/src/pyrtma/web_manager.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/src/pyrtma.egg-info/PKG-INFO` & `pyrtma-2.2.4/src/pyrtma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 2.2.3
+Version: 2.2.4
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-2.2.3/src/pyrtma.egg-info/SOURCES.txt` & `pyrtma-2.2.4/src/pyrtma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/tests/test_encoding.py` & `pyrtma-2.2.4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/tests/test_json.py` & `pyrtma-2.2.4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/tests/test_parser.py` & `pyrtma-2.2.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/tests/test_sync.py` & `pyrtma-2.2.4/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.3/tests/test_validators.py` & `pyrtma-2.2.4/tests/test_validators.py`

 * *Files identical despite different names*

