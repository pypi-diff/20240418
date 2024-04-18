# Comparing `tmp/swpclib-4.3.6.tar.gz` & `tmp/swpclib-4.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.3.6.tar", last modified: Mon Apr 15 02:42:28 2024, max compression
+gzip compressed data, was "swpclib-4.3.7.tar", last modified: Thu Apr 18 00:59:41 2024, max compression
```

## Comparing `swpclib-4.3.6.tar` & `swpclib-4.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:42:28.900849 swpclib-4.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-15 02:42:17.000000 swpclib-4.3.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 02:42:17.000000 swpclib-4.3.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 02:42:17.000000 swpclib-4.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 02:42:17.000000 swpclib-4.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 02:42:28.900849 swpclib-4.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-15 02:42:17.000000 swpclib-4.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:42:28.896849 swpclib-4.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 02:42:17.000000 swpclib-4.3.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 02:42:17.000000 swpclib-4.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 02:42:28.900849 swpclib-4.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 02:42:17.000000 swpclib-4.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:42:28.896849 swpclib-4.3.6/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 02:42:17.000000 swpclib-4.3.6/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-15 02:42:17.000000 swpclib-4.3.6/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-15 02:42:17.000000 swpclib-4.3.6/swpclib/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-15 02:42:17.000000 swpclib-4.3.6/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-15 02:42:17.000000 swpclib-4.3.6/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:42:28.900849 swpclib-4.3.6/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 02:42:28.000000 swpclib-4.3.6/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:42:28.900849 swpclib-4.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 02:42:17.000000 swpclib-4.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-15 02:42:17.000000 swpclib-4.3.6/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:59:41.404978 swpclib-4.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-18 00:59:33.000000 swpclib-4.3.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 00:59:33.000000 swpclib-4.3.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 00:59:33.000000 swpclib-4.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 00:59:33.000000 swpclib-4.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 00:59:41.404978 swpclib-4.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-18 00:59:33.000000 swpclib-4.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:59:41.400978 swpclib-4.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 00:59:33.000000 swpclib-4.3.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 00:59:33.000000 swpclib-4.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 00:59:41.404978 swpclib-4.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 00:59:33.000000 swpclib-4.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:59:41.400978 swpclib-4.3.7/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 00:59:33.000000 swpclib-4.3.7/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-18 00:59:33.000000 swpclib-4.3.7/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-18 00:59:33.000000 swpclib-4.3.7/swpclib/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-18 00:59:33.000000 swpclib-4.3.7/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-18 00:59:33.000000 swpclib-4.3.7/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:59:41.404978 swpclib-4.3.7/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 00:59:41.000000 swpclib-4.3.7/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:59:41.404978 swpclib-4.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 00:59:33.000000 swpclib-4.3.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-18 00:59:33.000000 swpclib-4.3.7/tests/test_swpclib.py
```

### Comparing `swpclib-4.3.6/CONTRIBUTING.rst` & `swpclib-4.3.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/LICENSE` & `swpclib-4.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/docs/Makefile` & `swpclib-4.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/docs/conf.py` & `swpclib-4.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/docs/installation.rst` & `swpclib-4.3.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/docs/make.bat` & `swpclib-4.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/setup.cfg` & `swpclib-4.3.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.3.5
+current_version = 4.3.7
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `swpclib-4.3.6/setup.py` & `swpclib-4.3.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 if __name__ == "__main__":
     setup(
         setup_requires=["setuptools-git-versioning"],
         test_suite="test",
         long_description=long_description,
         long_description_content_type="text/markdown",
         tests_require=test_requirements,
-        install_requires=["aiohttp==3.9.3", "pillow==10.2.0", "click==8.1.7"],
+        install_requires=["aiohttp>=3.8", "pillow>=10.1", "click>=8.1.7"],
         name="swpclib",
     )
```

### Comparing `swpclib-4.3.6/swpclib/alerts.py` & `swpclib-4.3.7/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/swpclib/animate.py` & `swpclib-4.3.7/swpclib/animate.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/swpclib/cli.py` & `swpclib-4.3.7/swpclib/cli.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/swpclib/swpclib.py` & `swpclib-4.3.7/swpclib/swpclib.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/swpclib.egg-info/SOURCES.txt` & `swpclib-4.3.7/swpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.6/tests/test_swpclib.py` & `swpclib-4.3.7/tests/test_swpclib.py`

 * *Files identical despite different names*

