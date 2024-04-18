# Comparing `tmp/sfmanager-0.0.4.tar.gz` & `tmp/sfmanager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfmanager-0.0.4.tar", last modified: Thu Apr 18 06:47:14 2024, max compression
+gzip compressed data, was "sfmanager-0.0.5.tar", last modified: Thu Apr 18 07:07:12 2024, max compression
```

## Comparing `sfmanager-0.0.4.tar` & `sfmanager-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.534309 sfmanager-0.0.4/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:47:14.534309 sfmanager-0.0.4/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.4/README.md
--rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 06:47:14.534309 sfmanager-0.0.4/setup.cfg
--rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 06:46:35.000000 sfmanager-0.0.4/setup.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.530310 sfmanager-0.0.4/sfmanager/
--rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.4/sfmanager/__init__.py
--rw-rw-r--   0 grand     (1000) grand     (1000)      491 2024-04-18 06:46:28.000000 sfmanager-0.0.4/sfmanager/app.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 06:47:14.534309 sfmanager-0.0.4/sfmanager.egg-info/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/requires.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 06:47:14.000000 sfmanager-0.0.4/sfmanager.egg-info/top_level.txt
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:07:12.776950 sfmanager-0.0.5/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 07:07:12.776950 sfmanager-0.0.5/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.5/README.md
+-rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 07:07:12.780949 sfmanager-0.0.5/setup.cfg
+-rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 07:07:07.000000 sfmanager-0.0.5/setup.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:07:12.772950 sfmanager-0.0.5/sfmanager/
+-rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.5/sfmanager/__init__.py
+-rw-rw-r--   0 grand     (1000) grand     (1000)     1284 2024-04-18 07:05:04.000000 sfmanager-0.0.5/sfmanager/app.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:07:12.776950 sfmanager-0.0.5/sfmanager.egg-info/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 07:07:12.000000 sfmanager-0.0.5/sfmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 07:07:12.000000 sfmanager-0.0.5/sfmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 07:07:12.000000 sfmanager-0.0.5/sfmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 07:07:12.000000 sfmanager-0.0.5/sfmanager.egg-info/requires.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 07:07:12.000000 sfmanager-0.0.5/sfmanager.egg-info/top_level.txt
```

### Comparing `sfmanager-0.0.4/PKG-INFO` & `sfmanager-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

### Comparing `sfmanager-0.0.4/setup.py` & `sfmanager-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sfmanager',
-    version='0.0.4',
+    version='0.0.5',
     author='GrandTheBest',
     author_email='grandinfo-cm@gmail.com',
     description='Super filemanager for python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/grand_studios',
     packages=find_packages(),
```

### Comparing `sfmanager-0.0.4/sfmanager.egg-info/PKG-INFO` & `sfmanager-0.0.5/sfmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

