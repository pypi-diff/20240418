# Comparing `tmp/cloudkitect.components-1.3.4.tar.gz` & `tmp/cloudkitect.components-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudkitect.components-1.3.4.tar", last modified: Thu Apr 18 05:12:10 2024, max compression
+gzip compressed data, was "cloudkitect.components-1.4.0.tar", last modified: Thu Apr 18 15:27:02 2024, max compression
```

## Comparing `cloudkitect.components-1.3.4.tar` & `cloudkitect.components-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.979851 cloudkitect.components-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-18 05:12:10.979851 cloudkitect.components-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:12:10.979851 cloudkitect.components-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.975851 cloudkitect.components-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.975851 cloudkitect.components-1.3.4/src/cloudkitect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.979851 cloudkitect.components-1.3.4/src/cloudkitect/components/
--rw-r--r--   0 runner    (1001) docker     (127)   370744 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/src/cloudkitect/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.979851 cloudkitect.components-1.3.4/src/cloudkitect/components/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/src/cloudkitect/components/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   124334 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/src/cloudkitect/components/_jsii/components@1.3.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:11:56.000000 cloudkitect.components-1.3.4/src/cloudkitect/components/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:12:10.975851 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-18 05:12:10.000000 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 05:12:10.000000 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:12:10.000000 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 05:12:10.000000 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 05:12:10.000000 cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.051849 cloudkitect.components-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-18 15:27:02.051849 cloudkitect.components-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:27:02.051849 cloudkitect.components-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.047849 cloudkitect.components-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.047849 cloudkitect.components-1.4.0/src/cloudkitect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.051849 cloudkitect.components-1.4.0/src/cloudkitect/components/
+-rw-r--r--   0 runner    (1001) docker     (127)   370744 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/src/cloudkitect/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.051849 cloudkitect.components-1.4.0/src/cloudkitect/components/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/src/cloudkitect/components/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124398 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/src/cloudkitect/components/_jsii/components@1.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:26:50.000000 cloudkitect.components-1.4.0/src/cloudkitect/components/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:27:02.047849 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-18 15:27:02.000000 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 15:27:02.000000 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:27:02.000000 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 15:27:02.000000 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 15:27:02.000000 cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/top_level.txt
```

### Comparing `cloudkitect.components-1.3.4/LICENSE` & `cloudkitect.components-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudkitect.components-1.3.4/PKG-INFO` & `cloudkitect.components-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudkitect.components
-Version: 1.3.4
+Version: 1.4.0
 Summary: CloudKitect freemium components are scaled down versions of CloudKitect enhanced components offered as monthly or yearly subscription. These are well architected components that offer out of the box monitoring, alerting and compliance to various standards.
 Home-page: https://github.com/cloudkitect/freemium
 Author: CloudKitect Inc<support@cloudkitect.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cloudkitect/freemium
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudkitect.components-1.3.4/README.md` & `cloudkitect.components-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudkitect.components-1.3.4/setup.py` & `cloudkitect.components-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudkitect.components",
-    "version": "1.3.4",
+    "version": "1.4.0",
     "description": "CloudKitect freemium components are scaled down versions of CloudKitect enhanced components offered as monthly or yearly subscription. These are well architected components that offer out of the box monitoring, alerting and compliance to various standards.",
     "license": "Apache-2.0",
     "url": "https://github.com/cloudkitect/freemium",
     "long_description_content_type": "text/markdown",
     "author": "CloudKitect Inc<support@cloudkitect.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudkitect.components",
         "cloudkitect.components._jsii"
     ],
     "package_data": {
         "cloudkitect.components._jsii": [
-            "components@1.3.4.jsii.tgz"
+            "components@1.4.0.jsii.tgz"
         ],
         "cloudkitect.components": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudkitect.components-1.3.4/src/cloudkitect/components/__init__.py` & `cloudkitect.components-1.4.0/src/cloudkitect/components/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitect.components-1.3.4/src/cloudkitect.components.egg-info/PKG-INFO` & `cloudkitect.components-1.4.0/src/cloudkitect.components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudkitect.components
-Version: 1.3.4
+Version: 1.4.0
 Summary: CloudKitect freemium components are scaled down versions of CloudKitect enhanced components offered as monthly or yearly subscription. These are well architected components that offer out of the box monitoring, alerting and compliance to various standards.
 Home-page: https://github.com/cloudkitect/freemium
 Author: CloudKitect Inc<support@cloudkitect.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cloudkitect/freemium
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

