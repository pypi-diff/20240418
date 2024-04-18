# Comparing `tmp/cloudkitect.patterns-1.3.4.tar.gz` & `tmp/cloudkitect.patterns-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudkitect.patterns-1.3.4.tar", last modified: Thu Apr 18 05:11:53 2024, max compression
+gzip compressed data, was "cloudkitect.patterns-1.4.0.tar", last modified: Thu Apr 18 15:26:48 2024, max compression
```

## Comparing `cloudkitect.patterns-1.3.4.tar` & `cloudkitect.patterns-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/src/cloudkitect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)    56454 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48182 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/_jsii/patterns@1.3.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:11:42.000000 cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:11:53.200968 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-18 05:11:53.000000 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 05:11:53.000000 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:11:53.000000 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 05:11:53.000000 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 05:11:53.000000 cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/src/cloudkitect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)    56454 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48182 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/_jsii/patterns@1.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:26:38.000000 cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:26:48.738435 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-18 15:26:48.000000 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 15:26:48.000000 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:26:48.000000 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 15:26:48.000000 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 15:26:48.000000 cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/top_level.txt
```

### Comparing `cloudkitect.patterns-1.3.4/LICENSE` & `cloudkitect.patterns-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudkitect.patterns-1.3.4/PKG-INFO` & `cloudkitect.patterns-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudkitect.patterns
-Version: 1.3.4
+Version: 1.4.0
 Summary: CloudKitect freemium patterns are built on top of CloudKitect freemium components which comply to various standards. Using these patterns you can host your website, or run your containerized app using ECS Fargate within a couple hours
 Home-page: https://github.com/cloudkitect/freemium
 Author: CloudKitect Inc<support@cloudkitect.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cloudkitect/freemium
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudkitect.patterns-1.3.4/README.md` & `cloudkitect.patterns-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudkitect.patterns-1.3.4/setup.py` & `cloudkitect.patterns-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudkitect.patterns",
-    "version": "1.3.4",
+    "version": "1.4.0",
     "description": "CloudKitect freemium patterns are built on top of CloudKitect freemium components which comply to various standards. Using these patterns you can host your website, or run your containerized app using ECS Fargate within a couple hours",
     "license": "Apache-2.0",
     "url": "https://github.com/cloudkitect/freemium",
     "long_description_content_type": "text/markdown",
     "author": "CloudKitect Inc<support@cloudkitect.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudkitect.patterns",
         "cloudkitect.patterns._jsii"
     ],
     "package_data": {
         "cloudkitect.patterns._jsii": [
-            "patterns@1.3.4.jsii.tgz"
+            "patterns@1.4.0.jsii.tgz"
         ],
         "cloudkitect.patterns": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudkitect.patterns-1.3.4/src/cloudkitect/patterns/__init__.py` & `cloudkitect.patterns-1.4.0/src/cloudkitect/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitect.patterns-1.3.4/src/cloudkitect.patterns.egg-info/PKG-INFO` & `cloudkitect.patterns-1.4.0/src/cloudkitect.patterns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudkitect.patterns
-Version: 1.3.4
+Version: 1.4.0
 Summary: CloudKitect freemium patterns are built on top of CloudKitect freemium components which comply to various standards. Using these patterns you can host your website, or run your containerized app using ECS Fargate within a couple hours
 Home-page: https://github.com/cloudkitect/freemium
 Author: CloudKitect Inc<support@cloudkitect.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cloudkitect/freemium
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

