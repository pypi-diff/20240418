# Comparing `tmp/itemdb-1.1.2.tar.gz` & `tmp/itemdb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemdb-1.1.2.tar", last modified: Thu Apr 20 23:34:14 2023, max compression
+gzip compressed data, was "itemdb-1.2.0.tar", last modified: Thu Apr 18 14:29:19 2024, max compression
```

## Comparing `itemdb-1.1.2.tar` & `itemdb-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-20 23:34:14.249249 itemdb-1.1.2/
--rw-r--r--   0 almar      (501) staff       (20)     1073 2023-04-20 21:02:09.000000 itemdb-1.1.2/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)     1337 2023-04-20 23:34:14.247783 itemdb-1.1.2/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     2356 2023-04-20 23:33:04.000000 itemdb-1.1.2/README.md
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-04-20 23:34:14.247108 itemdb-1.1.2/itemdb.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)     1337 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)      181 2023-04-20 23:34:14.000000 itemdb-1.1.2/itemdb.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        7 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-20 23:34:13.000000 itemdb-1.1.2/itemdb.egg-info/zip-safe
--rw-r--r--   0 almar      (501) staff       (20)    26808 2023-04-20 23:33:22.000000 itemdb-1.1.2/itemdb.py
--rw-r--r--   0 almar      (501) staff       (20)       38 2023-04-20 23:34:14.249368 itemdb-1.1.2/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2118 2023-04-20 21:02:09.000000 itemdb-1.1.2/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-04-18 14:29:19.230172 itemdb-1.2.0/
+-rw-r--r--   0 almar      (501) staff       (20)     1073 2024-04-18 14:25:07.000000 itemdb-1.2.0/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)     1389 2024-04-18 14:29:19.230048 itemdb-1.2.0/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     2356 2023-04-20 23:33:04.000000 itemdb-1.2.0/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-04-18 14:29:19.229742 itemdb-1.2.0/itemdb.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)     1389 2024-04-18 14:29:19.000000 itemdb-1.2.0/itemdb.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      181 2024-04-18 14:29:19.000000 itemdb-1.2.0/itemdb.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-04-18 14:29:19.000000 itemdb-1.2.0/itemdb.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        7 2024-04-18 14:29:19.000000 itemdb-1.2.0/itemdb.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-04-20 23:34:13.000000 itemdb-1.2.0/itemdb.egg-info/zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)    26710 2024-04-18 14:28:31.000000 itemdb-1.2.0/itemdb.py
+-rw-r--r--   0 almar      (501) staff       (20)       38 2024-04-18 14:29:19.230226 itemdb-1.2.0/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2169 2024-04-18 14:21:25.000000 itemdb-1.2.0/setup.py
```

### Comparing `itemdb-1.1.2/LICENSE` & `itemdb-1.2.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2021 Almar Klein
+Copyright (c) 2018-2024 Almar Klein
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `itemdb-1.1.2/PKG-INFO` & `itemdb-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemdb
-Version: 1.1.2
+Version: 1.2.0
 Summary: Easy transactional database for Python dicts, backed by SQLite
 Home-page: https://github.com/almarklein/itemdb
 Author: Almar Klein
 Author-email: 
 License: MIT
 Keywords: database,sqlite,no-sql
 Platform: any
@@ -13,19 +13,20 @@
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 
 
 The itemdb library allows you to store and retrieve Python dicts in a
 database on the local filesystem, in an easy, fast, and reliable way.
 
 Based on the rock-solid and ACID compliant SQLite, but with easy and
```

### Comparing `itemdb-1.1.2/README.md` & `itemdb-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `itemdb-1.1.2/itemdb.egg-info/PKG-INFO` & `itemdb-1.2.0/itemdb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemdb
-Version: 1.1.2
+Version: 1.2.0
 Summary: Easy transactional database for Python dicts, backed by SQLite
 Home-page: https://github.com/almarklein/itemdb
 Author: Almar Klein
 Author-email: 
 License: MIT
 Keywords: database,sqlite,no-sql
 Platform: any
@@ -13,19 +13,20 @@
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 
 
 The itemdb library allows you to store and retrieve Python dicts in a
 database on the local filesystem, in an easy, fast, and reliable way.
 
 Based on the rock-solid and ACID compliant SQLite, but with easy and
```

### Comparing `itemdb-1.1.2/itemdb.py` & `itemdb-1.2.0/itemdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,29 @@
 Based on the rock-solid and ACID compliant SQLite, but with easy and
 explicit transactions using a ``with`` statement. It provides a simple
 object-based API, with the flexibility to store (JSON-compatible) items
 with arbitrary fields, and add indices when needed.
 """
 
 import os
-import sys
 import json
 import queue
 import asyncio
 import sqlite3
 import threading
 
 
-__version__ = "1.1.2"
+__version__ = "1.2.0"
 version_info = tuple(map(int, __version__.split(".")))
 
 __all__ = ["ItemDB", "AsyncItemDB", "asyncify"]
 
 json_encode = json.JSONEncoder(ensure_ascii=True).encode
 json_decode = json.JSONDecoder().decode
 
-is_py36 = sys.version_info < (3, 7)
-
 
 # Notes:
 #
 # * Setting isolation_level to None turns on autocommit mode. We need to do
 #   this to prevent Python from issuing BEGIN before DML statements.
 # * Using a connection object as a context manager auto-commits/rollbacks a
 #   transaction.
@@ -60,15 +57,15 @@
             result = func(*args, **kwargs)
         except BaseException as e:
             loop.call_soon_threadsafe(future.set_exception, e)
         else:
             loop.call_soon_threadsafe(future.set_result, result)
 
     async def asyncified_func(*args, **kwargs):
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         future = loop.create_future()
         threading.Thread(
             name="asyncify " + func.__name__,
             target=threaded_func,
             args=(loop, future, args, kwargs),
         ).start()
         return await future
@@ -601,42 +598,43 @@
     """An async version of ItemDB. The API is exactly the same, except
     that all methods are async, and one must use `async with` instead
     of the normal `with`.
     """
 
     async def __new__(cls, filename):
         self = super().__new__(cls)
+        self._loop = asyncio.get_running_loop()
         self._queue = queue.Queue()
         self._thread = Thread4AsyncItemDB(self._queue)
         self._thread.start()
         self.db = self._thread.db = await self._handle(ItemDB, filename)
         return self
 
     @property
     def mtime(self):
         return self.db.mtime
 
     async def _handle(self, function, *args, **kwargs):
-        future = asyncio.get_event_loop().create_future()
+        future = self._loop.create_future()
         self._queue.put_nowait((future, function, args, kwargs))
         return await future
 
     async def __aenter__(self):
         return await self._handle(self.db.__enter__)
 
     async def __aexit__(self, type, value, traceback):
         return await self._handle(self.db.__exit__, type, value, traceback)
 
     def __del__(self):
-        future = asyncio.get_event_loop().create_future()
+        future = self._loop.create_future()
         self._queue.put_nowait((future, self.db.close, (), {}))
         self._queue.put_nowait((None, None, None, None))
 
     async def close(self):
-        future = asyncio.get_event_loop().create_future()
+        future = self._loop.create_future()
         self._queue.put_nowait((future, self.db.close, (), {}))
         self._queue.put_nowait((None, None, None, None))
         return await future
 
     async def get_table_names(self, *args, **kwargs):
         return await self._handle(self.db.get_table_names, *args, **kwargs)
 
@@ -700,18 +698,18 @@
             try:
                 result = function(*args, **kwargs)
 
                 def set_result(fut, result):
                     if not fut.done():
                         fut.set_result(result)
 
-                loop = future._loop if is_py36 else future.get_loop()
+                loop = future.get_loop()
                 loop.call_soon_threadsafe(set_result, future, result)
 
             except BaseException as e:
 
                 def set_exception(fut, e):
                     if not fut.done():
                         fut.set_exception(e)
 
-                loop = future._loop if is_py36 else future.get_loop()
+                loop = future.get_loop()
                 loop.call_soon_threadsafe(set_exception, future, e)
```

### Comparing `itemdb-1.1.2/setup.py` & `itemdb-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,27 +42,28 @@
     author_email="",
     license="MIT",
     url="https://github.com/almarklein/itemdb",
     keywords="database, sqlite, no-sql",
     description="Easy transactional database for Python dicts, backed by SQLite",
     long_description=doc,
     platforms="any",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[],
     py_modules=["itemdb"],
     zip_safe=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Database",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

