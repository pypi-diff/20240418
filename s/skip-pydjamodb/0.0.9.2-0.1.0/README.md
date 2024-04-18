# Comparing `tmp/skip-pydjamodb-0.0.9.2.tar.gz` & `tmp/skip_pydjamodb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-pydjamodb-0.0.9.2.tar", last modified: Mon Jan 16 23:53:27 2023, max compression
+gzip compressed data, was "skip_pydjamodb-0.1.0.tar", last modified: Thu Apr 18 13:57:38 2024, max compression
```

## Comparing `skip-pydjamodb-0.0.9.2.tar` & `skip_pydjamodb-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/pydjamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/pydjamodb/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-16 23:53:18.000000 skip-pydjamodb-0.0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 23:53:27.175710 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 23:53:26.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-16 23:53:27.000000 skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.173944 skip_pydjamodb-0.1.0/pydjamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/top_level.txt
```

### Comparing `skip-pydjamodb-0.0.9.2/LICENSE` & `skip_pydjamodb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.2/PKG-INFO` & `skip_pydjamodb-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.0.9.2
+Version: 0.1.0
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2
```

### Comparing `skip-pydjamodb-0.0.9.2/README.md` & `skip_pydjamodb-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.2/pydjamodb/attributes.py` & `skip_pydjamodb-0.1.0/pydjamodb/attributes.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.2/pydjamodb/models.py` & `skip_pydjamodb-0.1.0/pydjamodb/models.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.2/pydjamodb/queryset.py` & `skip_pydjamodb-0.1.0/pydjamodb/queryset.py`

 * *Files identical despite different names*

### Comparing `skip-pydjamodb-0.0.9.2/pydjamodb/test_runner.py` & `skip_pydjamodb-0.1.0/pydjamodb/test_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import multiprocessing
 import os
 import sys
 
+import django
 from django.db import connections
-from django.test.runner import ParallelTestSuite, DiscoverRunner
+from django.test.runner import ParallelTestSuite, DiscoverRunner, setup_test_environment
 
 from .connection import TestTableConnection
 from .models import dynamodb_model_classes
 
 try:
     from germanium.signals import set_up, tear_down
 
@@ -33,30 +35,53 @@
     remove_pynamodb_table(model_class)
     model_class.create_table(wait=True)
 
 
 _worker_id = 0
 
 
-def _init_worker(counter):
+def _init_worker(
+    counter,
+    initial_settings=None,
+    serialized_contents=None,
+    process_setup=None,
+    process_setup_args=None,
+    debug_mode=None,
+):
+    """
+    Switch to databases dedicated to this worker.
+
+    This helper lives at module-level because of the multiprocessing module's
+    requirements.
+    """
+
     global _worker_id
 
     with counter.get_lock():
         counter.value += 1
         _worker_id = counter.value
 
+    start_method = multiprocessing.get_start_method()
+
+    if start_method == "spawn":
+        if process_setup and callable(process_setup):
+            if process_setup_args is None:
+                process_setup_args = ()
+            process_setup(*process_setup_args)
+        django.setup()
+        setup_test_environment(debug=debug_mode)
+
     for alias in connections:
         connection = connections[alias]
-        settings_dict = connection.creation.get_test_db_clone_settings(str(_worker_id))
-        # connection.settings_dict must be updated in place for changes to be
-        # reflected in django.db.connections. If the following line assigned
-        # connection.settings_dict = settings_dict, new threads would connect
-        # to the default database instead of the appropriate clone.
-        connection.settings_dict.update(settings_dict)
-        connection.close()
+        if start_method == "spawn":
+            # Restore initial settings in spawned processes.
+            connection.settings_dict.update(initial_settings[alias])
+            if value := serialized_contents.get(alias):
+                connection._test_serialized_contents = value
+        connection.creation.setup_worker_connection(_worker_id)
 
     init_pynamodb_test_prefix(_worker_id)
 
 
 class DynamoDBParallelTestSuite(ParallelTestSuite):
 
     init_worker = _init_worker
```

### Comparing `skip-pydjamodb-0.0.9.2/setup.py` & `skip_pydjamodb-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='skip-pydjamodb',
-    version='0.0.9.2',
+    version='0.1.0',
     description="Django interface to PyDjamoDB.",
     keywords='django, DynamoDB, PyDjamoDB',
     author='Lubos Matl',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/pydjamodb',
     license='MIT',
     package_dir={'pydjamodb': 'pydjamodb'},
@@ -23,11 +23,11 @@
         'Natural Language :: Czech',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
     ],
     install_requires=[
-        'django>=2.0, <4.0',
+        'django>=4.2',
     ],
     zip_safe=False
 )
```

### Comparing `skip-pydjamodb-0.0.9.2/skip_pydjamodb.egg-info/PKG-INFO` & `skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.0.9.2
+Version: 0.1.0
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,8 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2
```

