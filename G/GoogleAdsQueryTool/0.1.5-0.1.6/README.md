# Comparing `tmp/GoogleAdsQueryTool-0.1.5.tar.gz` & `tmp/GoogleAdsQueryTool-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleAdsQueryTool-0.1.5.tar", last modified: Thu Apr 18 17:40:16 2024, max compression
+gzip compressed data, was "GoogleAdsQueryTool-0.1.6.tar", last modified: Thu Apr 18 18:32:50 2024, max compression
```

## Comparing `GoogleAdsQueryTool-0.1.5.tar` & `GoogleAdsQueryTool-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 17:40:16.111636 GoogleAdsQueryTool-0.1.5/
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 17:40:16.109958 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool/
--rw-r--r--   0 caspercrause   (501) staff       (20)     3951 2024-04-18 12:38:43.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool/GoogleAdsQueryTool.py
--rw-r--r--   0 caspercrause   (501) staff       (20)       32 2024-04-18 17:22:45.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool/__init__.py
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 17:40:16.111088 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/
--rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      344 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/SOURCES.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/dependency_links.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       76 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/entry_points.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       30 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/requires.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       19 2024-04-18 17:40:16.000000 GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool.egg-info/top_level.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 17:40:16.111369 GoogleAdsQueryTool-0.1.5/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 GoogleAdsQueryTool-0.1.5/README.md
--rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 17:40:16.111695 GoogleAdsQueryTool-0.1.5/setup.cfg
--rw-r--r--   0 caspercrause   (501) staff       (20)      642 2024-04-18 17:39:41.000000 GoogleAdsQueryTool-0.1.5/setup.py
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 18:32:50.531304 GoogleAdsQueryTool-0.1.6/
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 18:32:50.530814 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      322 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/SOURCES.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/dependency_links.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       76 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/entry_points.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       30 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/requires.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        8 2024-04-18 18:32:50.000000 GoogleAdsQueryTool-0.1.6/GoogleAdsQueryTool.egg-info/top_level.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 18:32:50.531061 GoogleAdsQueryTool-0.1.6/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 GoogleAdsQueryTool-0.1.6/README.md
+-rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 18:32:50.531358 GoogleAdsQueryTool-0.1.6/setup.cfg
+-rw-r--r--   0 caspercrause   (501) staff       (20)      642 2024-04-18 18:32:38.000000 GoogleAdsQueryTool-0.1.6/setup.py
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 18:32:50.530640 GoogleAdsQueryTool-0.1.6/toolbox/
+-rw-r--r--   0 caspercrause   (501) staff       (20)     3951 2024-04-18 12:38:43.000000 GoogleAdsQueryTool-0.1.6/toolbox/GoogleAdsQueryTool.py
+-rw-r--r--   0 caspercrause   (501) staff       (20)       21 2024-04-18 18:30:58.000000 GoogleAdsQueryTool-0.1.6/toolbox/__init__.py
```

### Comparing `GoogleAdsQueryTool-0.1.5/GoogleAdsQueryTool/GoogleAdsQueryTool.py` & `GoogleAdsQueryTool-0.1.6/toolbox/GoogleAdsQueryTool.py`

 * *Files identical despite different names*

### Comparing `GoogleAdsQueryTool-0.1.5/setup.py` & `GoogleAdsQueryTool-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GoogleAdsQueryTool',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'google-ads==22.1.0',
         'pandas>1.4'
     ],
     entry_points={
         'console_scripts': [
```

