# Comparing `tmp/pyrpabrowserdemo-0.0.2.tar.gz` & `tmp/pyrpabrowserdemo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrpabrowserdemo-0.0.2.tar", last modified: Tue Apr 16 19:22:37 2024, max compression
+gzip compressed data, was "pyrpabrowserdemo-0.0.3.tar", last modified: Thu Apr 18 20:17:37 2024, max compression
```

## Comparing `pyrpabrowserdemo-0.0.2.tar` & `pyrpabrowserdemo-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-16 19:22:37.440176 pyrpabrowserdemo-0.0.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 pyrpabrowserdemo-0.0.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-16 19:22:37.440176 pyrpabrowserdemo-0.0.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1419 2024-04-16 19:14:12.000000 pyrpabrowserdemo-0.0.2/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-16 19:22:37.440176 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2024-04-16 19:10:47.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2546 2024-04-16 19:21:48.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo/browser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      489 2024-04-08 12:26:11.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo/definition.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      127 2024-04-15 21:20:15.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo/test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-16 19:22:37.440176 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-16 19:22:37.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      338 2024-04-16 19:22:37.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-16 19:22:37.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-04-16 19:22:37.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2024-04-16 19:22:37.000000 pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-16 19:22:37.440176 pyrpabrowserdemo-0.0.2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1124 2024-04-16 19:22:32.000000 pyrpabrowserdemo-0.0.2/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 20:17:37.811544 pyrpabrowserdemo-0.0.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1066 2024-04-07 19:59:28.000000 pyrpabrowserdemo-0.0.3/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-18 20:17:37.811544 pyrpabrowserdemo-0.0.3/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1419 2024-04-16 19:14:12.000000 pyrpabrowserdemo-0.0.3/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 20:17:37.811544 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2024-04-16 19:10:47.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5257 2024-04-18 17:58:24.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo/browser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      766 2024-04-18 18:14:31.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo/definition.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1385 2024-04-18 18:16:24.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo/test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-18 20:17:37.811544 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1985 2024-04-18 20:17:37.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      338 2024-04-18 20:17:37.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-18 20:17:37.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       28 2024-04-18 20:17:37.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2024-04-18 20:17:37.000000 pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-18 20:17:37.811544 pyrpabrowserdemo-0.0.3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1124 2024-04-18 20:17:27.000000 pyrpabrowserdemo-0.0.3/setup.py
```

### Comparing `pyrpabrowserdemo-0.0.2/LICENSE` & `pyrpabrowserdemo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrpabrowserdemo-0.0.2/PKG-INFO` & `pyrpabrowserdemo-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrpabrowserdemo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simplify RPA activities with a browser.
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrpabrowserdemo-0.0.2/README.md` & `pyrpabrowserdemo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrpabrowserdemo-0.0.2/pyrpabrowserdemo.egg-info/PKG-INFO` & `pyrpabrowserdemo-0.0.3/pyrpabrowserdemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrpabrowserdemo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simplify RPA activities with a browser.
 Author: Daniel Rubens
 Author-email: danielrubensdaniel@gmail.com
 Keywords: python,rpa,robocorp,pdf,html,conversor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrpabrowserdemo-0.0.2/setup.py` & `pyrpabrowserdemo-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Simplify RPA activities with a browser.'
 LONG_DESCRIPTION = 'A package that allows to execute RPA activities without configuration'
 
 # Setting up
 setup(
     name="pyrpabrowserdemo",
     version=VERSION,
```

