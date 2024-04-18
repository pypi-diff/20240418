# Comparing `tmp/sfmanager-0.0.3.tar.gz` & `tmp/sfmanager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfmanager-0.0.3.tar", last modified: Thu Apr 18 06:44:50 2024, max compression
+gzip compressed data, was "sfmanager-0.0.4.tar", last modified: Thu Apr 18 06:47:14 2024, max compression
```

## Comparing `sfmanager-0.0.3.tar` & `sfmanager-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:44:50.782917 sfmanager-0.0.3/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:44:50.786917 sfmanager-0.0.3/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.3/README.md
--rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 06:44:50.786917 sfmanager-0.0.3/setup.cfg
--rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 06:36:35.000000 sfmanager-0.0.3/setup.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:44:50.782917 sfmanager-0.0.3/sfmanager/
--rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.3/sfmanager/__init__.py
--rw-rw-r--   0 grand     (1000) grand     (1000)      483 2024-04-18 05:44:36.000000 sfmanager-0.0.3/sfmanager/app.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:44:50.782917 sfmanager-0.0.3/sfmanager.egg-info/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:44:50.000000 sfmanager-0.0.3/sfmanager.egg-info/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 06:44:50.000000 sfmanager-0.0.3/sfmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 06:44:50.000000 sfmanager-0.0.3/sfmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 06:44:50.000000 sfmanager-0.0.3/sfmanager.egg-info/requires.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 06:44:50.000000 sfmanager-0.0.3/sfmanager.egg-info/top_level.txt
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.534309 sfmanager-0.0.4/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:47:14.534309 sfmanager-0.0.4/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.4/README.md
+-rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 06:47:14.534309 sfmanager-0.0.4/setup.cfg
+-rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 06:46:35.000000 sfmanager-0.0.4/setup.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.530310 sfmanager-0.0.4/sfmanager/
+-rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.4/sfmanager/__init__.py
+-rw-rw-r--   0 grand     (1000) grand     (1000)      491 2024-04-18 06:46:28.000000 sfmanager-0.0.4/sfmanager/app.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.534309 sfmanager-0.0.4/sfmanager.egg-info/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/requires.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/top_level.txt
```

### Comparing `sfmanager-0.0.3/PKG-INFO` & `sfmanager-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

### Comparing `sfmanager-0.0.3/setup.py` & `sfmanager-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sfmanager',
-    version='0.0.3',
+    version='0.0.4',
     author='GrandTheBest',
     author_email='grandinfo-cm@gmail.com',
     description='Super filemanager for python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/grand_studios',
     packages=find_packages(),
```

### Comparing `sfmanager-0.0.3/sfmanager.egg-info/PKG-INFO` & `sfmanager-0.0.4/sfmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

