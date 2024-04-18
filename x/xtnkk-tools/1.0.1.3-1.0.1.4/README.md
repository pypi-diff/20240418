# Comparing `tmp/xtnkk-tools-1.0.1.3.tar.gz` & `tmp/xtnkk-tools-1.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.1.3.tar", last modified: Thu Apr 18 04:34:58 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.1.4.tar", last modified: Thu Apr 18 05:04:59 2024, max compression
```

## Comparing `xtnkk-tools-1.0.1.3.tar` & `xtnkk-tools-1.0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.3/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-18 04:34:50.000000 xtnkk-tools-1.0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/
--rw-rw-rw-   0        0        0     5489 2024-04-18 04:22:33.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-18 04:15:31.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     6241 2024-04-18 04:34:37.000000 xtnkk-tools-1.0.1.3/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 04:34:58.000000 xtnkk-tools-1.0.1.3/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-18 05:04:49.000000 xtnkk-tools-1.0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/xtnkk_tools/
+-rw-rw-rw-   0        0        0     5495 2024-04-18 04:57:03.000000 xtnkk-tools-1.0.1.4/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-18 04:15:31.000000 xtnkk-tools-1.0.1.4/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     2626 2024-04-18 04:57:03.000000 xtnkk-tools-1.0.1.4/xtnkk_tools/tools.py
+-rw-rw-rw-   0        0        0     4877 2024-04-18 05:04:49.000000 xtnkk-tools-1.0.1.4/xtnkk_tools/tools_time.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-18 05:04:58.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-18 05:04:59.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:04:58.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 05:04:58.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 05:04:58.000000 xtnkk-tools-1.0.1.4/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.1.3/setup.py` & `xtnkk-tools-1.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.1.3",  # 版本
+    version="1.0.1.4",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.1.3/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.1.4/xtnkk_tools/MongoDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 说明：
 #    MongoDBPro
 # History:
 # Date          Author    Version       Modification
 # --------------------------------------------------------------------------------------------------
 # 2024/4/17    xiatn     V00.01.000    新建
 # --------------------------------------------------------------------------------------------------
-from xtnkk_tools.tools import *
+from xtnkk_tools.tools_time import *
 from urllib import parse
 from typing import List, Dict, Optional
 from pymongo import MongoClient
 from pymongo.database import Database
 from pymongo.collection import Collection
 from pymongo.errors import DuplicateKeyError, BulkWriteError
 
@@ -103,15 +103,15 @@
             data: 单条数据
             insert_ignore: 索引冲突是否忽略 默认False
             is_add_create_time: 是否在数据中添加一个创建数据10时间戳字段 默认False不创建
             is_add_create_time_field_name: 自定义创建数据时间戳字段名：默认：create_dt
         Returns: 插入成功的行数
         """
         if is_add_create_time:
-            data[is_add_create_time_field_name] = get_now_timestamp_int(is_time_10=True)
+            data[is_add_create_time_field_name] = get_time_now_timestamp(is_time_10=True)
         collection = self.get_collection(coll_name)
         try:
             collection.insert_one(data)
         except DuplicateKeyError as e:
             if not insert_ignore:
                 raise e
             return 0
```

