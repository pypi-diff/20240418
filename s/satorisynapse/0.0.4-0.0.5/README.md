# Comparing `tmp/satorisynapse-0.0.4.tar.gz` & `tmp/satorisynapse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.0.4.tar", last modified: Wed Apr 17 21:10:01 2024, max compression
+gzip compressed data, was "satorisynapse-0.0.5.tar", last modified: Wed Apr 17 21:27:30 2024, max compression
```

## Comparing `satorisynapse-0.0.4.tar` & `satorisynapse-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:10:01.081031 satorisynapse-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:10:01.081031 satorisynapse-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:10:01.077031 satorisynapse-0.0.4/satorisynapse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:10:01.077031 satorisynapse-0.0.4/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:10:01.077031 satorisynapse-0.0.4/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:10:01.081031 satorisynapse-0.0.4/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:10:01.000000 satorisynapse-0.0.4/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 21:10:01.000000 satorisynapse-0.0.4/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 21:10:01.000000 satorisynapse-0.0.4/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:10:01.000000 satorisynapse-0.0.4/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 21:10:01.000000 satorisynapse-0.0.4/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:10:01.081031 satorisynapse-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 21:09:55.000000 satorisynapse-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.348275 satorisynapse-0.0.5/satorisynapse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 21:27:30.000000 satorisynapse-0.0.5/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:27:30.352275 satorisynapse-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 21:27:25.000000 satorisynapse-0.0.5/setup.py
```

### Comparing `satorisynapse-0.0.4/LICENSE` & `satorisynapse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.4/PKG-INFO` & `satorisynapse-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.4
+Version: 0.0.5
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.4/satorisynapse/lib/domain.py` & `satorisynapse-0.0.5/satorisynapse/lib/domain.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.4/satorisynapse/lib/requests.py` & `satorisynapse-0.0.5/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.4/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.0.5/satorisynapse/synapse/asynchronous.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.4/satorisynapse/synapse/threaded.py` & `satorisynapse-0.0.5/satorisynapse/synapse/threaded.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.4/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.0.5/satorisynapse.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.4
+Version: 0.0.5
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.4/setup.py` & `satorisynapse-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.4'
+    return '0.0.5'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
```

