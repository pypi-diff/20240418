# Comparing `tmp/pykeypass-2024.4.17.tar.gz` & `tmp/pykeypass-2024.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeypass-2024.4.17.tar", last modified: Thu Apr 18 00:13:11 2024, max compression
+gzip compressed data, was "pykeypass-2024.4.18.tar", last modified: Thu Apr 18 00:16:33 2024, max compression
```

## Comparing `pykeypass-2024.4.17.tar` & `pykeypass-2024.4.18.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-18 00:13:04.000000 pykeypass-2024.4.17/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 00:13:04.000000 pykeypass-2024.4.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:13:11.940288 pykeypass-2024.4.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/src/pykeypass/
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-04-18 00:13:04.000000 pykeypass-2024.4.17/src/pykeypass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/src/pykeypass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 00:13:11.000000 pykeypass-2024.4.17/src/pykeypass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:13:11.944288 pykeypass-2024.4.17/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-18 00:13:04.000000 pykeypass-2024.4.17/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-18 00:13:04.000000 pykeypass-2024.4.17/test/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-18 00:16:23.000000 pykeypass-2024.4.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 00:16:23.000000 pykeypass-2024.4.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:16:33.185516 pykeypass-2024.4.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/src/pykeypass/
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-04-18 00:16:23.000000 pykeypass-2024.4.18/src/pykeypass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/src/pykeypass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 00:16:33.000000 pykeypass-2024.4.18/src/pykeypass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:16:33.189516 pykeypass-2024.4.18/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-18 00:16:23.000000 pykeypass-2024.4.18/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-18 00:16:23.000000 pykeypass-2024.4.18/test/test_local.py
```

### Comparing `pykeypass-2024.4.17/PKG-INFO` & `pykeypass-2024.4.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeypass
-Version: 2024.4.17
+Version: 2024.4.18
 Author-email: bh <bhammond@waubonsee.edu>
 Project-URL: Homepage, https://github.com/darrida/pykeypass
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pykeepass==4.0.7.post1
 Requires-Dist: lxml==5.2.1
 Requires-Dist: click==8.1.7
```

### Comparing `pykeypass-2024.4.17/README.md` & `pykeypass-2024.4.18/README.md`

 * *Files identical despite different names*

### Comparing `pykeypass-2024.4.17/pyproject.toml` & `pykeypass-2024.4.18/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pykeypass"
-version = "2024.04.17"
+version = "2024.04.18"
 description = ""
 authors = [
     {name="bh", email="bhammond@waubonsee.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9,<3.13"
 dependencies = [
@@ -12,15 +12,15 @@
     "lxml==5.2.1",
     "click==8.1.7",
     "setuptools==69.5.1",
     'python_version < 3',
 ]
 
 [project.scripts]
-my-client = "pykeypass:cli"
+pykeypass = "pykeypass:cli"
 
 [project.optional-dependencies]
 test = [    
     'pytest',
     'pytest-asyncio',
     'pytest-mock'
 ]
```

### Comparing `pykeypass-2024.4.17/src/pykeypass/__init__.py` & `pykeypass-2024.4.18/src/pykeypass/__init__.py`

 * *Files identical despite different names*

### Comparing `pykeypass-2024.4.17/src/pykeypass.egg-info/PKG-INFO` & `pykeypass-2024.4.18/src/pykeypass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeypass
-Version: 2024.4.17
+Version: 2024.4.18
 Author-email: bh <bhammond@waubonsee.edu>
 Project-URL: Homepage, https://github.com/darrida/pykeypass
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pykeepass==4.0.7.post1
 Requires-Dist: lxml==5.2.1
 Requires-Dist: click==8.1.7
```

### Comparing `pykeypass-2024.4.17/test/test_github.py` & `pykeypass-2024.4.18/test/test_github.py`

 * *Files identical despite different names*

### Comparing `pykeypass-2024.4.17/test/test_local.py` & `pykeypass-2024.4.18/test/test_local.py`

 * *Files identical despite different names*

