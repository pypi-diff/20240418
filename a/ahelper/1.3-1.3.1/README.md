# Comparing `tmp/ahelper-1.3.tar.gz` & `tmp/ahelper-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahelper-1.3.tar", last modified: Thu Apr 18 15:32:51 2024, max compression
+gzip compressed data, was "ahelper-1.3.1.tar", last modified: Thu Apr 18 15:47:41 2024, max compression
```

## Comparing `ahelper-1.3.tar` & `ahelper-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/
--rw-rw-r--   0 jtli      (1012) jtli      (1013)      934 2024-04-18 15:32:51.972224 ahelper-1.3/PKG-INFO
-drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/ahelper/
--rw-------   0 jtli      (1012) jtli      (1013)      957 2024-04-18 15:06:12.000000 ahelper-1.3/ahelper/__init__.py
--rw-------   0 jtli      (1012) jtli      (1013)     9944 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/deepwalk.py
--rw-------   0 jtli      (1012) jtli      (1013)     4074 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/feature.py
--rw-------   0 jtli      (1012) jtli      (1013)    15521 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/layers.py
--rw-------   0 jtli      (1012) jtli      (1013)      839 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/links.py
--rw-rw-r--   0 jtli      (1012) jtli      (1013)    18348 2024-04-18 15:01:07.000000 ahelper-1.3/ahelper/nlu_lora.py
--rw-------   0 jtli      (1012) jtli      (1013)    12614 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/snn.py
--rw-------   0 jtli      (1012) jtli      (1013)    14793 2024-04-18 14:56:41.000000 ahelper-1.3/ahelper/utils.py
-drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:32:51.972224 ahelper-1.3/ahelper.egg-info/
--rw-rw-r--   0 jtli      (1012) jtli      (1013)      934 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/PKG-INFO
--rw-rw-r--   0 jtli      (1012) jtli      (1013)      278 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/SOURCES.txt
--rw-rw-r--   0 jtli      (1012) jtli      (1013)        1 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/dependency_links.txt
--rw-rw-r--   0 jtli      (1012) jtli      (1013)        8 2024-04-18 15:32:51.000000 ahelper-1.3/ahelper.egg-info/top_level.txt
--rw-rw-r--   0 jtli      (1012) jtli      (1013)       38 2024-04-18 15:32:51.972224 ahelper-1.3/setup.cfg
--rw-------   0 jtli      (1012) jtli      (1013)     1241 2024-04-18 15:32:49.000000 ahelper-1.3/setup.py
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:47:41.730457 ahelper-1.3.1/
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      936 2024-04-18 15:47:41.730457 ahelper-1.3.1/PKG-INFO
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:47:41.726456 ahelper-1.3.1/ahelper/
+-rw-------   0 jtli      (1012) jtli      (1013)      957 2024-04-18 15:06:12.000000 ahelper-1.3.1/ahelper/__init__.py
+-rw-------   0 jtli      (1012) jtli      (1013)     9944 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/deepwalk.py
+-rw-------   0 jtli      (1012) jtli      (1013)     4074 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/feature.py
+-rw-------   0 jtli      (1012) jtli      (1013)    15521 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/layers.py
+-rw-------   0 jtli      (1012) jtli      (1013)      839 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/links.py
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)    18348 2024-04-18 15:01:07.000000 ahelper-1.3.1/ahelper/nlu_lora.py
+-rw-------   0 jtli      (1012) jtli      (1013)    12614 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/snn.py
+-rw-------   0 jtli      (1012) jtli      (1013)    14793 2024-04-18 14:56:41.000000 ahelper-1.3.1/ahelper/utils.py
+drwxrwxr-x   0 jtli      (1012) jtli      (1013)        0 2024-04-18 15:47:41.730457 ahelper-1.3.1/ahelper.egg-info/
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      936 2024-04-18 15:47:41.000000 ahelper-1.3.1/ahelper.egg-info/PKG-INFO
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)      278 2024-04-18 15:47:41.000000 ahelper-1.3.1/ahelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)        1 2024-04-18 15:47:41.000000 ahelper-1.3.1/ahelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)        8 2024-04-18 15:47:41.000000 ahelper-1.3.1/ahelper.egg-info/top_level.txt
+-rw-rw-r--   0 jtli      (1012) jtli      (1013)       38 2024-04-18 15:47:41.730457 ahelper-1.3.1/setup.cfg
+-rw-------   0 jtli      (1012) jtli      (1013)     1245 2024-04-18 15:47:39.000000 ahelper-1.3.1/setup.py
```

### Comparing `ahelper-1.3/PKG-INFO` & `ahelper-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahelper
-Version: 1.3
+Version: 1.3.1
 Summary: A helper.
 Home-page: https://gitee.com/EdisonLeeeee/ahelper
 Author: Jintang Li
 Author-email: cnljt@outlook.com
 License: MIT LICENSE
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ahelper-1.3/ahelper/__init__.py` & `ahelper-1.3.1/ahelper/__init__.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/deepwalk.py` & `ahelper-1.3.1/ahelper/deepwalk.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/feature.py` & `ahelper-1.3.1/ahelper/feature.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/layers.py` & `ahelper-1.3.1/ahelper/layers.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/links.py` & `ahelper-1.3.1/ahelper/links.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/nlu_lora.py` & `ahelper-1.3.1/ahelper/nlu_lora.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/snn.py` & `ahelper-1.3.1/ahelper/snn.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper/utils.py` & `ahelper-1.3.1/ahelper/utils.py`

 * *Files identical despite different names*

### Comparing `ahelper-1.3/ahelper.egg-info/PKG-INFO` & `ahelper-1.3.1/ahelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahelper
-Version: 1.3
+Version: 1.3.1
 Summary: A helper.
 Home-page: https://gitee.com/EdisonLeeeee/ahelper
 Author: Jintang Li
 Author-email: cnljt@outlook.com
 License: MIT LICENSE
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ahelper-1.3/setup.py` & `ahelper-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 url='https://gitee.com/EdisonLeeeee/ahelper'
-VERSION = 1.3
+VERSION = '1.3.1'
 
 setup(
     name='ahelper',
     version=VERSION,
     description='A helper.',
     python_requires='>=3.6',
     license="MIT LICENSE",
```

