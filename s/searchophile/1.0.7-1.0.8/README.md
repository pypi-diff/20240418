# Comparing `tmp/searchophile-1.0.7.tar.gz` & `tmp/searchophile-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchophile-1.0.7.tar", last modified: Thu Oct  5 02:06:28 2023, max compression
+gzip compressed data, was "searchophile-1.0.8.tar", last modified: Thu Apr 18 14:39:07 2024, max compression
```

## Comparing `searchophile-1.0.7.tar` & `searchophile-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 02:06:28.620010 searchophile-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-05 02:06:16.000000 searchophile-1.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2023-10-05 02:06:28.620010 searchophile-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2023-10-05 02:06:16.000000 searchophile-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-05 02:06:28.620010 searchophile-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-10-05 02:06:16.000000 searchophile-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 02:06:28.620010 searchophile-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 02:06:28.620010 searchophile-1.0.7/src/searchophile/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-10-05 02:06:16.000000 searchophile-1.0.7/src/searchophile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-05 02:06:16.000000 searchophile-1.0.7/src/searchophile/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17251 2023-10-05 02:06:16.000000 searchophile-1.0.7/src/searchophile/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 02:06:28.620010 searchophile-1.0.7/src/searchophile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-05 02:06:28.000000 searchophile-1.0.7/src/searchophile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:39:07.183548 searchophile-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 14:38:56.000000 searchophile-1.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-18 14:39:07.183548 searchophile-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-18 14:38:56.000000 searchophile-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 14:39:07.183548 searchophile-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-18 14:38:56.000000 searchophile-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:39:07.179548 searchophile-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:39:07.183548 searchophile-1.0.8/src/searchophile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 14:38:56.000000 searchophile-1.0.8/src/searchophile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-18 14:38:56.000000 searchophile-1.0.8/src/searchophile/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17257 2024-04-18 14:38:56.000000 searchophile-1.0.8/src/searchophile/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:39:07.183548 searchophile-1.0.8/src/searchophile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 14:39:07.000000 searchophile-1.0.8/src/searchophile.egg-info/top_level.txt
```

### Comparing `searchophile-1.0.7/LICENSE.md` & `searchophile-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `searchophile-1.0.7/PKG-INFO` & `searchophile-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchophile
-Version: 1.0.7
+Version: 1.0.8
 Summary: Command line file search tools
 Home-page: https://github.com/Tails86/searchophile
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/searchophile
 Project-URL: Bug Reports, https://github.com/Tails86/searchophile/issues
 Project-URL: Source Code, https://github.com/Tails86/searchophile
```

### Comparing `searchophile-1.0.7/README.md` & `searchophile-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `searchophile-1.0.7/setup.py` & `searchophile-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.5',
     install_requires=[
-        'greplica>=1.2.6,<2.0',
-        'sedeuce>=1.0.7,<2.0',
-        'refind>=1.0.6,<2.0'
+        'greplica>=1.2.7,<2.0',
+        'sedeuce>=1.0.8,<2.0',
+        'refind>=1.0.7,<2.0'
     ],
     extras_require={
         'dev': ['check-manifest']
     },
     entry_points={
         'console_scripts': [
             'search=searchophile.__main__:main',
```

### Comparing `searchophile-1.0.7/src/searchophile/__init__.py` & `searchophile-1.0.8/src/searchophile/__init__.py`

 * *Files identical despite different names*

### Comparing `searchophile-1.0.7/src/searchophile/__main__.py` & `searchophile-1.0.8/src/searchophile/__main__.py`

 * *Files identical despite different names*

### Comparing `searchophile-1.0.7/src/searchophile/search.py` & `searchophile-1.0.8/src/searchophile/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 import re
 import string
 import refind
 import greplica
 import sedeuce
 from typing import Any, Union, List, Tuple
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 PACKAGE_NAME = 'searchophile'
 
 FIND_CMD = 'find'
 GREP_CMD = 'grep'
 SED_CMD = 'sed'
 
 def _item_needs_quotes(item):
@@ -254,15 +254,15 @@
     search_string = args.search_string or args.search_string_opt
     if args.whole_word:
         grep_other_options += 'w'
     if regex:
         grep_other_options += 'E' # For grep "extended regex"
     else:
         grep_other_options += 'F' # Default to string search
-    grep_command += [grep_color_option, grep_other_options, search_string]
+    grep_command += [grep_color_option, grep_other_options, '--', search_string]
 
     if args.show_errors:
         err_file = sys.stderr
     else:
         err_file = None
     grep_obj = greplica.Grep(sys.stdout, err_file)
     grep_parser = greplica.GrepArgParser()
```

### Comparing `searchophile-1.0.7/src/searchophile.egg-info/PKG-INFO` & `searchophile-1.0.8/src/searchophile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchophile
-Version: 1.0.7
+Version: 1.0.8
 Summary: Command line file search tools
 Home-page: https://github.com/Tails86/searchophile
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/searchophile
 Project-URL: Bug Reports, https://github.com/Tails86/searchophile/issues
 Project-URL: Source Code, https://github.com/Tails86/searchophile
```

