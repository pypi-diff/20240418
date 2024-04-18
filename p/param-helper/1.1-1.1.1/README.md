# Comparing `tmp/param-helper-1.1.tar.gz` & `tmp/param-helper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "param-helper-1.1.tar", last modified: Fri Mar 22 16:22:44 2024, max compression
+gzip compressed data, was "param-helper-1.1.1.tar", last modified: Thu Apr 18 13:33:33 2024, max compression
```

## Comparing `param-helper-1.1.tar` & `param-helper-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:22:43.999627 param-helper-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-22 16:22:43.999627 param-helper-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 16:22:37.000000 param-helper-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:22:43.995627 param-helper-1.1/param_helper/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-22 16:22:37.000000 param-helper-1.1/param_helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:22:43.999627 param-helper-1.1/param_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-22 16:22:43.000000 param-helper-1.1/param_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-22 16:22:43.000000 param-helper-1.1/param_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:22:43.000000 param-helper-1.1/param_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 16:22:43.000000 param-helper-1.1/param_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-22 16:22:43.000000 param-helper-1.1/param_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-22 16:22:43.999627 param-helper-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-22 16:22:37.000000 param-helper-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:33:33.351547 param-helper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-18 13:33:33.351547 param-helper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 13:33:26.000000 param-helper-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:33:33.347547 param-helper-1.1.1/param_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-18 13:33:26.000000 param-helper-1.1.1/param_helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:33:33.351547 param-helper-1.1.1/param_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-18 13:33:33.000000 param-helper-1.1.1/param_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 13:33:33.000000 param-helper-1.1.1/param_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:33:33.000000 param-helper-1.1.1/param_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 13:33:33.000000 param-helper-1.1.1/param_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 13:33:33.000000 param-helper-1.1.1/param_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 13:33:33.351547 param-helper-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 13:33:26.000000 param-helper-1.1.1/setup.py
```

### Comparing `param-helper-1.1/PKG-INFO` & `param-helper-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: param-helper
-Version: 1.1
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/EvATive7/param-helper
 Author: EvATive7
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # param-helper
-A python library that can easily get parameters from a function, as well as additional features
+A python library that provides an esay way to get parameters in a function, with additional features
 
 ## usage & example
 [code](test.py)  
 
 ## license
 [AGPL3.0](https://www.gnu.org/licenses/agpl.txt)
```

### Comparing `param-helper-1.1/param_helper/__init__.py` & `param-helper-1.1.1/param_helper/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         value = values[arg]
         if value == None:
             continue
         if annotation == inspect._empty:
             default = signature.default
             if default != inspect._empty:
                 default = type(default)
-                previous_function_args[arg] = default(value)
+                if default != type(None):
+                    previous_function_args[arg] = default(value)
+                else:
+                    previous_function_args[arg] = value
             else:
                 previous_function_args[arg] = value
         else:
             previous_function_args[arg] = annotation(value)
 
     previous_function_args.update(kwargs)
     return previous_function_args
```

### Comparing `param-helper-1.1/param_helper.egg-info/PKG-INFO` & `param-helper-1.1.1/param_helper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: param-helper
-Version: 1.1
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/EvATive7/param-helper
 Author: EvATive7
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # param-helper
-A python library that can easily get parameters from a function, as well as additional features
+A python library that provides an esay way to get parameters in a function, with additional features
 
 ## usage & example
 [code](test.py)  
 
 ## license
 [AGPL3.0](https://www.gnu.org/licenses/agpl.txt)
```

### Comparing `param-helper-1.1/setup.py` & `param-helper-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="param-helper",
-    version="1.1",
+    version="1.1.1",
     author="EvATive7",
     author_email="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EvATive7/param-helper",
     packages=setuptools.find_packages(),
     install_requires=[],
```

