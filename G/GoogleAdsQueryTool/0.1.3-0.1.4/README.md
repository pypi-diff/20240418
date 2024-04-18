# Comparing `tmp/GoogleAdsQueryTool-0.1.3.tar.gz` & `tmp/GoogleAdsQueryTool-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleAdsQueryTool-0.1.3.tar", last modified: Thu Apr 18 12:44:54 2024, max compression
+gzip compressed data, was "GoogleAdsQueryTool-0.1.4.tar", last modified: Thu Apr 18 17:25:56 2024, max compression
```

## Comparing `GoogleAdsQueryTool-0.1.3.tar` & `GoogleAdsQueryTool-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 12:44:54.476101 GoogleAdsQueryTool-0.1.3/
-drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 12:44:54.475667 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/
--rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      272 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/SOURCES.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/dependency_links.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       76 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/entry_points.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)       30 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/requires.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 12:44:54.000000 GoogleAdsQueryTool-0.1.3/GoogleAdsQueryTool.egg-info/top_level.txt
--rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 12:44:54.475896 GoogleAdsQueryTool-0.1.3/PKG-INFO
--rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 GoogleAdsQueryTool-0.1.3/README.md
--rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 12:44:54.476148 GoogleAdsQueryTool-0.1.3/setup.cfg
--rw-r--r--   0 caspercrause   (501) staff       (20)      642 2024-04-18 12:43:44.000000 GoogleAdsQueryTool-0.1.3/setup.py
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 17:25:56.980538 GoogleAdsQueryTool-0.1.4/
+drwxr-xr-x   0 caspercrause   (501) staff       (20)        0 2024-04-18 17:25:56.980015 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      272 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/SOURCES.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/dependency_links.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       76 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/entry_points.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)       30 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/requires.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)        1 2024-04-18 17:25:56.000000 GoogleAdsQueryTool-0.1.4/GoogleAdsQueryTool.egg-info/top_level.txt
+-rw-r--r--   0 caspercrause   (501) staff       (20)      480 2024-04-18 17:25:56.980259 GoogleAdsQueryTool-0.1.4/PKG-INFO
+-rw-r--r--   0 caspercrause   (501) staff       (20)      157 2024-04-18 11:02:58.000000 GoogleAdsQueryTool-0.1.4/README.md
+-rw-r--r--   0 caspercrause   (501) staff       (20)       38 2024-04-18 17:25:56.980601 GoogleAdsQueryTool-0.1.4/setup.cfg
+-rw-r--r--   0 caspercrause   (501) staff       (20)      642 2024-04-18 17:24:48.000000 GoogleAdsQueryTool-0.1.4/setup.py
```

### Comparing `GoogleAdsQueryTool-0.1.3/setup.py` & `GoogleAdsQueryTool-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GoogleAdsQueryTool',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'google-ads==22.1.0',
         'pandas>1.4'
     ],
     entry_points={
         'console_scripts': [
```

