# Comparing `tmp/a3mongo-0.1.1.tar.gz` & `tmp/a3mongo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3mongo-0.1.1.tar", last modified: Mon Mar 11 08:44:29 2024, max compression
+gzip compressed data, was "a3mongo-0.1.2.tar", last modified: Thu Apr 18 05:10:27 2024, max compression
```

## Comparing `a3mongo-0.1.1.tar` & `a3mongo-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-11 08:44:29.517004 a3mongo-0.1.1/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3mongo-0.1.1/LICENSE
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       65 2024-03-10 12:10:19.000000 a3mongo-0.1.1/MANIFEST.in
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1214 2024-03-11 08:44:29.517004 a3mongo-0.1.1/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      127 2024-03-10 12:10:44.000000 a3mongo-0.1.1/README.md
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-11 08:44:29.513004 a3mongo-0.1.1/a3mongo/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      150 2024-03-11 08:43:24.000000 a3mongo-0.1.1/a3mongo/__init__.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      773 2024-03-11 08:43:24.000000 a3mongo-0.1.1/a3mongo/mongo_client_factory.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     5231 2024-03-10 13:24:28.000000 a3mongo-0.1.1/a3mongo/mongo_table.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-03-11 08:44:29.517004 a3mongo-0.1.1/a3mongo.egg-info/
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1214 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      307 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/SOURCES.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/dependency_links.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/not-zip-safe
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       15 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/requires.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        8 2024-03-11 08:44:29.000000 a3mongo-0.1.1/a3mongo.egg-info/top_level.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1119 2024-03-11 08:44:29.517004 a3mongo-0.1.1/setup.cfg
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3mongo-0.1.1/setup.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 05:10:27.440394 a3mongo-0.1.2/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3mongo-0.1.2/LICENSE
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       65 2024-03-10 12:10:19.000000 a3mongo-0.1.2/MANIFEST.in
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1214 2024-04-18 05:10:27.440394 a3mongo-0.1.2/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      127 2024-03-10 12:10:44.000000 a3mongo-0.1.2/README.md
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 05:10:27.440394 a3mongo-0.1.2/a3mongo/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      150 2024-04-18 03:35:49.000000 a3mongo-0.1.2/a3mongo/__init__.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      773 2024-03-11 08:43:24.000000 a3mongo-0.1.2/a3mongo/mongo_client_factory.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     6354 2024-04-18 05:08:44.000000 a3mongo-0.1.2/a3mongo/mongo_table.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 05:10:27.440394 a3mongo-0.1.2/a3mongo.egg-info/
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1214 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      307 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/not-zip-safe
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       15 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/requires.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        8 2024-04-18 05:10:27.000000 a3mongo-0.1.2/a3mongo.egg-info/top_level.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1119 2024-04-18 05:10:27.440394 a3mongo-0.1.2/setup.cfg
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3mongo-0.1.2/setup.py
```

### Comparing `a3mongo-0.1.1/LICENSE` & `a3mongo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `a3mongo-0.1.1/PKG-INFO` & `a3mongo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3mongo
-Version: 0.1.1
+Version: 0.1.2
 Summary: It is just a thin wrapper of pymongo.
 Home-page: https://github.com/three-kinds/a3mongo
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3mongo
 Project-URL: Source, https://github.com/three-kinds/a3mongo
```

### Comparing `a3mongo-0.1.1/a3mongo/mongo_client_factory.py` & `a3mongo-0.1.2/a3mongo/mongo_client_factory.py`

 * *Files identical despite different names*

### Comparing `a3mongo-0.1.1/a3mongo/mongo_table.py` & `a3mongo-0.1.2/a3mongo/mongo_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 import math
 from typing import List, Iterable, Dict
-from pymongo.operations import ReplaceOne
+from pymongo.operations import ReplaceOne, UpdateOne
 from pymongo.collection import Collection
 from pymongo.database import Database
 from pymongo.cursor import Cursor
 from pymongo.errors import BulkWriteError, WriteError
 from pymongo.results import UpdateResult, BulkWriteResult
 
 from .mongo_client_factory import MongoClientFactory
 
 
 class MongoTable:
     table_name: str = None
     db_conf_name: str = None
 
     def __init__(self, db: Database = None, table_name: str = None):
-        self.db = db or MongoClientFactory.get_db(self.db_conf_name)
+        if db is None:
+            db = MongoClientFactory.get_db(self.db_conf_name)
+
+        self.db = db
         self.table_name = table_name or self.table_name
         self._table = self.db.get_collection(self.table_name)
 
     def get_raw_collection(self) -> Collection:
         return self._table
 
     def is_table_exists(self) -> bool:
@@ -71,28 +74,59 @@
         unique_field = unique_field or '_id'
         try:
             update_result = self._table.replace_one({unique_field: entry[unique_field]}, entry, upsert=True)
             return True, update_result
         except WriteError as e:
             return False, str(e)
 
+    # insert or update
     def upsert_many(self, entry_list: list, unique_field: str = None) -> (int, BulkWriteResult):
         unique_field = unique_field or '_id'
         request_list = list()
 
         for entry in entry_list:
             request_list.append(
                 ReplaceOne({unique_field: entry[unique_field]}, entry, upsert=True)
             )
 
         error_count = 0
         while True:
             try:
                 write_result = self._table.bulk_write(request_list)
                 return error_count, write_result
+            except BulkWriteError as e:
+                error_index_list = list()
+                for error in e.details['writeErrors']:
+                    error_index_list.append(error['index'])
+
+                error_count += len(error_index_list)
+                for index in sorted(error_index_list, reverse=True):
+                    del request_list[index]
+
+    # only insert not update
+    def insert_many(self, entry_list: list, unique_field: str = None) -> (int, BulkWriteResult):
+        unique_field = unique_field or '_id'
+        request_list = list()
+
+        for entry in entry_list:
+            request_list.append(
+                UpdateOne(
+                    {unique_field: entry[unique_field]},
+                    {
+                        "$setOnInsert": entry
+                    },
+                    upsert=True
+                )
+            )
+
+        error_count = 0
+        while True:
+            try:
+                write_result = self._table.bulk_write(request_list)
+                return error_count, write_result
             except BulkWriteError as e:
                 error_index_list = list()
                 for error in e.details['writeErrors']:
                     error_index_list.append(error['index'])
 
                 error_count += len(error_index_list)
                 for index in sorted(error_index_list, reverse=True):
```

### Comparing `a3mongo-0.1.1/a3mongo.egg-info/PKG-INFO` & `a3mongo-0.1.2/a3mongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3mongo
-Version: 0.1.1
+Version: 0.1.2
 Summary: It is just a thin wrapper of pymongo.
 Home-page: https://github.com/three-kinds/a3mongo
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3mongo
 Project-URL: Source, https://github.com/three-kinds/a3mongo
```

### Comparing `a3mongo-0.1.1/setup.cfg` & `a3mongo-0.1.2/setup.cfg`

 * *Files identical despite different names*

