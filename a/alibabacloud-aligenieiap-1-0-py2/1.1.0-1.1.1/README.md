# Comparing `tmp/alibabacloud_aligenieiap_1_0_py2-1.1.0.tar.gz` & `tmp/alibabacloud_aligenieiap_1_0_py2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0_py2-1.1.0.tar", last modified: Tue Apr 16 17:15:19 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0_py2-1.1.1.tar", last modified: Wed Apr 17 17:10:08 2024, max compression
```

## Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0.tar` & `alibabacloud_aligenieiap_1_0_py2-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41474 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   183861 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2927 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      209 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41474 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   183861 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-04-17 17:10:08.000000 alibabacloud_aligenieiap_1_0_py2-1.1.1/setup.py
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/LICENSE` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/PKG-INFO` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieiap_1_0_py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/README-CN.md` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/README.md` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/client.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/models.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieiap-1-0-py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieiap_1_0_py2.
 
-Created on 16/04/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieiap_1_0"
 NAME = "alibabacloud_aligenieiap_1_0_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2"
```

