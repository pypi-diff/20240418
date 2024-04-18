# Comparing `tmp/elbowplot-0.1.tar.gz` & `tmp/elbowplot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elbowplot-0.1.tar", last modified: Thu Apr 18 17:02:51 2024, max compression
+gzip compressed data, was "elbowplot-0.1.1.tar", last modified: Thu Apr 18 17:25:38 2024, max compression
```

## Comparing `elbowplot-0.1.tar` & `elbowplot-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:02:51.341688 elbowplot-0.1/
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)     1088 2024-04-18 17:01:35.000000 elbowplot-0.1/LICENSE
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      924 2024-04-18 17:02:51.341688 elbowplot-0.1/PKG-INFO
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      391 2024-04-18 17:02:20.000000 elbowplot-0.1/README.md
-drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:02:51.341688 elbowplot-0.1/elbowplot/
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:56:28.000000 elbowplot-0.1/elbowplot/__init__.py
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      553 2024-04-18 16:57:59.000000 elbowplot-0.1/elbowplot/core.py
-drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:02:51.341688 elbowplot-0.1/elbowplot.egg-info/
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      924 2024-04-18 17:02:51.000000 elbowplot-0.1/elbowplot.egg-info/PKG-INFO
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      267 2024-04-18 17:02:51.000000 elbowplot-0.1/elbowplot.egg-info/SOURCES.txt
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        1 2024-04-18 17:02:51.000000 elbowplot-0.1/elbowplot.egg-info/dependency_links.txt
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       30 2024-04-18 17:02:51.000000 elbowplot-0.1/elbowplot.egg-info/requires.txt
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       16 2024-04-18 17:02:51.000000 elbowplot-0.1/elbowplot.egg-info/top_level.txt
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       38 2024-04-18 17:02:51.341688 elbowplot-0.1/setup.cfg
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      775 2024-04-18 16:58:19.000000 elbowplot-0.1/setup.py
-drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:02:51.341688 elbowplot-0.1/tests/
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:56:57.000000 elbowplot-0.1/tests/__init__.py
--rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:57:04.000000 elbowplot-0.1/tests/test_core.py
+drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:25:38.985742 elbowplot-0.1.1/
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)     1088 2024-04-18 17:01:35.000000 elbowplot-0.1.1/LICENSE
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)     4669 2024-04-18 17:25:38.985742 elbowplot-0.1.1/PKG-INFO
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)     4135 2024-04-18 17:20:45.000000 elbowplot-0.1.1/README.md
+drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:25:38.985742 elbowplot-0.1.1/elbowplot/
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:56:28.000000 elbowplot-0.1.1/elbowplot/__init__.py
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      553 2024-04-18 16:57:59.000000 elbowplot-0.1.1/elbowplot/core.py
+drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:25:38.985742 elbowplot-0.1.1/elbowplot.egg-info/
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)     4669 2024-04-18 17:25:38.000000 elbowplot-0.1.1/elbowplot.egg-info/PKG-INFO
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      267 2024-04-18 17:25:38.000000 elbowplot-0.1.1/elbowplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        1 2024-04-18 17:25:38.000000 elbowplot-0.1.1/elbowplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       30 2024-04-18 17:25:38.000000 elbowplot-0.1.1/elbowplot.egg-info/requires.txt
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       16 2024-04-18 17:25:38.000000 elbowplot-0.1.1/elbowplot.egg-info/top_level.txt
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)       38 2024-04-18 17:25:38.985742 elbowplot-0.1.1/setup.cfg
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)      777 2024-04-18 17:25:26.000000 elbowplot-0.1.1/setup.py
+drwxrwxr-x   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 17:25:38.985742 elbowplot-0.1.1/tests/
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:56:57.000000 elbowplot-0.1.1/tests/__init__.py
+-rw-rw-r--   0 subaashnair  (1000) subaashnair  (1000)        0 2024-04-18 16:57:04.000000 elbowplot-0.1.1/tests/test_core.py
```

### Comparing `elbowplot-0.1/LICENSE` & `elbowplot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elbowplot-0.1/elbowplot/core.py` & `elbowplot-0.1.1/elbowplot/core.py`

 * *Files identical despite different names*

### Comparing `elbowplot-0.1/setup.py` & `elbowplot-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elbowplot',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description='A simple library to plot the elbow plot for K-means clustering.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/yourusername/elbowplot',
```

