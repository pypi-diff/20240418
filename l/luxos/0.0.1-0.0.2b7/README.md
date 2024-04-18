# Comparing `tmp/luxos-0.0.1.tar.gz` & `tmp/luxos-0.0.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.1.tar", last modified: Wed Apr 10 23:11:04 2024, max compression
+gzip compressed data, was "luxos-0.0.2b7.tar", last modified: Thu Apr 18 13:06:01 2024, max compression
```

## Comparing `luxos-0.0.1.tar` & `luxos-0.0.2b7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/
--rw-r--r--   0 antonio   (1000) antonio   (1000)     3628 2024-04-10 23:11:04.270379 luxos-0.0.1/PKG-INFO
--rw-r--r--   0 antonio   (1000) antonio   (1000)     2799 2024-04-10 16:28:21.000000 luxos-0.0.1/README.md
--rw-r--r--   0 antonio   (1000) antonio   (1000)     1724 2024-04-10 23:11:02.000000 luxos-0.0.1/pyproject.toml
--rw-r--r--   0 antonio   (1000) antonio   (1000)       38 2024-04-10 23:11:04.270379 luxos-0.0.1/setup.cfg
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.267045 luxos-0.0.1/src/
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/
--rw-r--r--   0 antonio   (1000) antonio   (1000)       75 2024-04-10 23:11:02.000000 luxos-0.0.1/src/luxos/__init__.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)       75 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/__main__.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)     3501 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/api.json
--rw-r--r--   0 antonio   (1000) antonio   (1000)      803 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/api.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)     9601 2024-04-10 23:06:11.000000 luxos-0.0.1/src/luxos/asyncops.py
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/cli/
--rw-r--r--   0 antonio   (1000) antonio   (1000)        0 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/cli/__init__.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)     4546 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/cli/v1.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)      645 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/exceptions.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)      755 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/misc.py
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/scripts/
--rw-r--r--   0 antonio   (1000) antonio   (1000)        0 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/__init__.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)     1639 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)    30158 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/health_checker.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)    12195 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/luxos.py
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos.egg-info/
--rw-r--r--   0 antonio   (1000) antonio   (1000)     3628 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 antonio   (1000) antonio   (1000)      632 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 antonio   (1000) antonio   (1000)        1 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 antonio   (1000) antonio   (1000)      102 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 antonio   (1000) antonio   (1000)       33 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/requires.txt
--rw-r--r--   0 antonio   (1000) antonio   (1000)        6 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/tests/
--rw-r--r--   0 antonio   (1000) antonio   (1000)      555 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_cli.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)      478 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_luxos.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)     5796 2024-04-10 23:06:11.000000 luxos-0.0.1/tests/test_luxos_asyncops.py
--rw-r--r--   0 antonio   (1000) antonio   (1000)      558 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 13:06:01.162823 luxos-0.0.2b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-18 13:05:28.000000 luxos-0.0.2b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-18 13:05:59.000000 luxos-0.0.2b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:06:01.162823 luxos-0.0.2b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.158823 luxos-0.0.2b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 13:05:59.000000 luxos-0.0.2b7/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-18 13:05:28.000000 luxos-0.0.2b7/src/luxos/scripts/luxos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 13:06:01.000000 luxos-0.0.2b7/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:06:01.162823 luxos-0.0.2b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 13:05:28.000000 luxos-0.0.2b7/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.1/PKG-INFO` & `luxos-0.0.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.1
+Version: 0.0.2b7
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.1/README.md` & `luxos-0.0.2b7/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/pyproject.toml` & `luxos-0.0.2b7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.1"
+version = "0.0.2b7"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
@@ -39,15 +39,15 @@
 Issues = "https://github.com/LuxorLabs/firmware-biz-tools/issues"
 
 [project.scripts]
 luxos = "luxos.scripts.luxos:main"
 health-checker = "luxos.scripts.health_checker:main"
 
 [tool.setuptools.package-data]
-'luxos' = ['*.json']
+'luxos' = ['*.json', 'py.typed']
 
 
 [tool.ruff]
 target-version = "py39"
 line-length = 88
```

### Comparing `luxos-0.0.1/src/luxos/api.json` & `luxos-0.0.2b7/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/api.py` & `luxos-0.0.2b7/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/asyncops.py` & `luxos-0.0.2b7/src/luxos/asyncops.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,18 +237,19 @@
     timeout: float | None = None,
     retry: int | None = None,
     retry_delay: float | None = None,
 ) -> dict[str, Any] | None:
     from . import api
 
     parameters = ([parameters] if isinstance(parameters, str) else parameters) or []
+    parameters = [str(param) for param in parameters]
 
     timeout = TIMEOUT if timeout is None else timeout
     retry = RETRY if retry is None else retry
-    retry_delay = RETRY_DELAY if retry_delay else retry_delay
+    retry_delay = RETRY_DELAY if retry_delay is None else retry_delay
 
     # if cmd is logon/logoff we dealt with it differently
     if cmd in {"logon", "logoff"}:
         failure = None
         for i in range(retry or 1):
             try:
                 if cmd == "logon":
```

### Comparing `luxos-0.0.1/src/luxos/exceptions.py` & `luxos-0.0.2b7/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/misc.py` & `luxos-0.0.2b7/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/scripts/async_luxos.py` & `luxos-0.0.2b7/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/scripts/health_checker.py` & `luxos-0.0.2b7/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos/scripts/luxos.py` & `luxos-0.0.2b7/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.2b7/src/luxos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.1
+Version: 0.0.2b7
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.1/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.2b7/src/luxos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/luxos/__init__.py
 src/luxos/__main__.py
 src/luxos/api.json
 src/luxos/api.py
 src/luxos/asyncops.py
 src/luxos/exceptions.py
 src/luxos/misc.py
+src/luxos/py.typed
 src/luxos.egg-info/PKG-INFO
 src/luxos.egg-info/SOURCES.txt
 src/luxos.egg-info/dependency_links.txt
 src/luxos.egg-info/entry_points.txt
 src/luxos.egg-info/requires.txt
 src/luxos.egg-info/top_level.txt
 src/luxos/cli/__init__.py
```

### Comparing `luxos-0.0.1/tests/test_cli.py` & `luxos-0.0.2b7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/tests/test_luxos_asyncops.py` & `luxos-0.0.2b7/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.1/tests/test_luxos_misc.py` & `luxos-0.0.2b7/tests/test_luxos_misc.py`

 * *Files identical despite different names*

