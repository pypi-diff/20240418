# Comparing `tmp/satorisynapse-0.0.6.tar.gz` & `tmp/satorisynapse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.0.6.tar", last modified: Thu Apr 18 20:16:13 2024, max compression
+gzip compressed data, was "satorisynapse-0.0.7.tar", last modified: Thu Apr 18 21:17:57 2024, max compression
```

## Comparing `satorisynapse-0.0.6.tar` & `satorisynapse-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.186349 satorisynapse-0.0.6/satorisynapse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 20:16:13.000000 satorisynapse-0.0.6/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:16:13.190350 satorisynapse-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-18 20:16:09.000000 satorisynapse-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:57.339575 satorisynapse-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:17:57.339575 satorisynapse-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:57.335575 satorisynapse-0.0.7/satorisynapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:57.339575 satorisynapse-0.0.7/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:57.339575 satorisynapse-0.0.7/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:17:57.335575 satorisynapse-0.0.7/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:17:57.000000 satorisynapse-0.0.7/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 21:17:57.000000 satorisynapse-0.0.7/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 21:17:57.000000 satorisynapse-0.0.7/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 21:17:57.000000 satorisynapse-0.0.7/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 21:17:57.000000 satorisynapse-0.0.7/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:17:57.339575 satorisynapse-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-18 21:17:49.000000 satorisynapse-0.0.7/setup.py
```

### Comparing `satorisynapse-0.0.6/LICENSE` & `satorisynapse-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.6/PKG-INFO` & `satorisynapse-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.6
+Version: 0.0.7
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.6/satorisynapse/lib/domain.py` & `satorisynapse-0.0.7/satorisynapse/lib/domain.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.6/satorisynapse/lib/requests.py` & `satorisynapse-0.0.7/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.6/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.0.7/satorisynapse/synapse/asynchronous.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.6/satorisynapse/synapse/threaded.py` & `satorisynapse-0.0.7/satorisynapse/synapse/threaded.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.6/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.7/satorisynapse.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.6
+Version: 0.0.7
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.6/setup.py` & `satorisynapse-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 
 def get_here(file: str):
+    # return os.path.abspath(os.path.dirname(__file__))
     return os.path.join(os.path.dirname(os.path.realpath(__file__)), file)
 
 
 def get_long_description():
     readme = get_here('README.md')
     if os.path.isfile(readme):
         with open(readme, 'r') as f:
@@ -15,15 +16,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.6'
+    return '0.0.7'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
@@ -33,16 +34,17 @@
 if __name__ == '__main__':
     setup(
         name=get_name(),
         version=get_version(),
         description='satorisynapse contains domain model and apis for the Satori Network',
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
-        packages=[f'{get_name()}.{p}' for p in find_packages(
-            where=get_name())],
+        #packages=[get_name()] + [f'{get_name()}.{p}' for p in find_packages(
+        #    where=get_name())],
+        packages=find_packages(),
         install_requires=get_requirements(),
         dependency_links=[
             'git+https://github.com/SatoriNetwork/python-evrmorelib.git#egg=python-evrmorelib'
         ],
         python_requires='>=3.7',
         author='Jordan Miller',
         author_email="jordan@satorinet.io",
```

