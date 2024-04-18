# Comparing `tmp/xtnkk-tools-1.0.1.0.tar.gz` & `tmp/xtnkk-tools-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.1.0.tar", last modified: Wed Apr 17 16:36:17 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.1.1.tar", last modified: Thu Apr 18 02:29:26 2024, max compression
```

## Comparing `xtnkk-tools-1.0.1.0.tar` & `xtnkk-tools-1.0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.0/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 16:36:05.000000 xtnkk-tools-1.0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools/
--rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.1.0/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.1.0/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     5586 2024-04-17 16:35:57.000000 xtnkk-tools-1.0.1.0/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 16:36:17.000000 xtnkk-tools-1.0.1.0/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-18 02:29:12.000000 xtnkk-tools-1.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools/
+-rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.1.1/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      460 2024-04-18 02:29:04.000000 xtnkk-tools-1.0.1.1/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     5586 2024-04-17 16:35:57.000000 xtnkk-tools-1.0.1.1/xtnkk_tools/tools.py
+-rw-rw-rw-   0        0        0      869 2024-04-18 02:28:49.000000 xtnkk-tools-1.0.1.1/xtnkk_tools/update.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 02:29:26.000000 xtnkk-tools-1.0.1.1/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.1.0/setup.py` & `xtnkk-tools-1.0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.1.0",  # 版本
+    version="1.0.1.1",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.1.0/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.1.1/xtnkk_tools/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtnkk-tools-1.0.1.0/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.1.1/xtnkk_tools/tools.py`

 * *Files identical despite different names*

