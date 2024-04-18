# Comparing `tmp/stDCL-1.0.0.tar.gz` & `tmp/stDCL-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stDCL-1.0.0.tar", last modified: Sun Apr 14 16:12:10 2024, max compression
+gzip compressed data, was "dist/stDCL-1.0.1.tar", last modified: Thu Apr 18 07:09:18 2024, max compression
```

## Comparing `stDCL-1.0.0.tar` & `stDCL-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-14 16:12:10.000000 stDCL-1.0.0/
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)       38 2024-04-14 16:12:10.000000 stDCL-1.0.0/setup.cfg
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)      820 2024-04-14 16:11:36.000000 stDCL-1.0.0/setup.py
-drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL/
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-14 13:53:23.000000 stDCL-1.0.0/stDCL/_init_.py
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     6010 2024-04-13 16:31:45.000000 stDCL-1.0.0/stDCL/stDCL.py
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     2833 2024-04-13 16:29:52.000000 stDCL-1.0.0/stDCL/model.py
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     3958 2024-04-13 16:31:49.000000 stDCL-1.0.0/stDCL/preprocess.py
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     6467 2024-04-13 16:31:59.000000 stDCL-1.0.0/stDCL/utils.py
-drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL.egg-info/
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        1 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL.egg-info/dependency_links.txt
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        6 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL.egg-info/top_level.txt
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)      223 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL.egg-info/SOURCES.txt
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     3210 2024-04-14 16:12:10.000000 stDCL-1.0.0/stDCL.egg-info/PKG-INFO
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     3210 2024-04-14 16:12:10.000000 stDCL-1.0.0/PKG-INFO
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     1071 2024-04-14 13:56:06.000000 stDCL-1.0.0/LICENSE
--rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     2682 2024-04-14 13:55:43.000000 stDCL-1.0.0/README.md
+drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-18 07:09:18.000000 stDCL-1.0.1/
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)       38 2024-04-18 07:09:18.000000 stDCL-1.0.1/setup.cfg
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)      820 2024-04-18 07:08:06.000000 stDCL-1.0.1/setup.py
+drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL/
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-14 13:53:23.000000 stDCL-1.0.1/stDCL/_init_.py
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     6010 2024-04-13 16:31:45.000000 stDCL-1.0.1/stDCL/stDCL.py
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     2833 2024-04-13 16:29:52.000000 stDCL-1.0.1/stDCL/model.py
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     3958 2024-04-13 16:31:49.000000 stDCL-1.0.1/stDCL/preprocess.py
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     6467 2024-04-13 16:31:59.000000 stDCL-1.0.1/stDCL/utils.py
+drwxrwxr-x   0 yuzhuohan  (1013) yuzhuohan  (1013)        0 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL.egg-info/
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        1 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)        6 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL.egg-info/top_level.txt
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)      223 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     4369 2024-04-18 07:09:18.000000 stDCL-1.0.1/stDCL.egg-info/PKG-INFO
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     4369 2024-04-18 07:09:18.000000 stDCL-1.0.1/PKG-INFO
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     1071 2024-04-14 13:56:06.000000 stDCL-1.0.1/LICENSE
+-rw-rw-r--   0 yuzhuohan  (1013) yuzhuohan  (1013)     3841 2024-04-18 07:08:00.000000 stDCL-1.0.1/README.md
```

### Comparing `stDCL-1.0.0/setup.py` & `stDCL-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # @Software: PyCharm
 # @Description:
 
 from setuptools import setup
 
 setup(
     name='stDCL',
-    version='1.0.0',
+    version='1.0.1',
     description='Spatial Transcriptome Heterogeneity Dissection of Brain Regions with Dual Graph Contrastive Learning',
     author='Zhuohan Yu',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author_email="zhuohan20@mails.jlu.edu.cn",
     packages=['stDCL'],
     url='https://github.com/Philyzh8/stDCL',
```

### Comparing `stDCL-1.0.0/stDCL/stDCL.py` & `stDCL-1.0.1/stDCL/stDCL.py`

 * *Files identical despite different names*

### Comparing `stDCL-1.0.0/stDCL/model.py` & `stDCL-1.0.1/stDCL/model.py`

 * *Files identical despite different names*

### Comparing `stDCL-1.0.0/stDCL/preprocess.py` & `stDCL-1.0.1/stDCL/preprocess.py`

 * *Files identical despite different names*

### Comparing `stDCL-1.0.0/stDCL/utils.py` & `stDCL-1.0.1/stDCL/utils.py`

 * *Files identical despite different names*

### Comparing `stDCL-1.0.0/LICENSE` & `stDCL-1.0.1/LICENSE`

 * *Files identical despite different names*

