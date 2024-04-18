# Comparing `tmp/alibabacloud_aligenieiap_1_0-1.2.0.tar.gz` & `tmp/alibabacloud_aligenieiap_1_0-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.2.0.tar", last modified: Tue Apr 16 17:16:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.2.1.tar", last modified: Wed Apr 17 17:10:51 2024, max compression
```

## Comparing `alibabacloud_aligenieiap_1_0-1.2.0.tar` & `alibabacloud_aligenieiap_1_0-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93586 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   183098 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93586 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   183098 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:10:51.000000 alibabacloud_aligenieiap_1_0-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-17 17:10:50.000000 alibabacloud_aligenieiap_1_0-1.2.1/setup.py
```

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/LICENSE` & `alibabacloud_aligenieiap_1_0-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieiap_1_0
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/README-CN.md` & `alibabacloud_aligenieiap_1_0-1.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/README.md` & `alibabacloud_aligenieiap_1_0-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/client.py` & `alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/models.py` & `alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.2.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieiap-1-0
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.2.0/setup.py` & `alibabacloud_aligenieiap_1_0-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieiap_1_0.
 
-Created on 16/04/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieiap_1_0"
 NAME = "alibabacloud_aligenieiap_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python"
```

