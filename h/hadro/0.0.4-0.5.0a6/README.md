# Comparing `tmp/hadro-0.0.4.tar.gz` & `tmp/hadro-0.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hadro-0.0.4.tar", last modified: Wed Jun 21 16:57:09 2023, max compression
+gzip compressed data, was "hadro-0.5.0a6.tar", last modified: Thu Apr 18 20:04:01 2024, max compression
```

## Comparing `hadro-0.0.4.tar` & `hadro-0.5.0a6.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:57:09.585950 hadro-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 16:56:57.000000 hadro-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-21 16:56:57.000000 hadro-0.0.4/NOTICES
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-21 16:57:09.585950 hadro-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-21 16:56:57.000000 hadro-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:57:09.585950 hadro-0.0.4/hadro/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 16:56:57.000000 hadro-0.0.4/hadro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-21 16:56:57.000000 hadro-0.0.4/hadro/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-21 16:56:57.000000 hadro-0.0.4/hadro/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-21 16:56:57.000000 hadro-0.0.4/hadro/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 16:56:57.000000 hadro-0.0.4/hadro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:57:09.585950 hadro-0.0.4/hadro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-21 16:57:09.000000 hadro-0.0.4/hadro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 16:57:09.000000 hadro-0.0.4/hadro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:57:09.000000 hadro-0.0.4/hadro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:57:09.000000 hadro-0.0.4/hadro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 16:57:09.000000 hadro-0.0.4/hadro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-21 16:56:57.000000 hadro-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:57:09.585950 hadro-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-21 16:56:57.000000 hadro-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:57:09.585950 hadro-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-21 16:56:57.000000 hadro-0.0.4/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.373876 hadro-0.5.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 20:03:51.000000 hadro-0.5.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 20:03:51.000000 hadro-0.5.0a6/NOTICES
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-18 20:04:01.373876 hadro-0.5.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-18 20:03:51.000000 hadro-0.5.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.369876 hadro-0.5.0a6/hadro/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.369876 hadro-0.5.0a6/hadro/compiled/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/compiled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   434513 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro/compiled/memtable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.373876 hadro-0.5.0a6/hadro/memtable/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/memtable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/memtable/memtable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.373876 hadro-0.5.0a6/hadro/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-18 20:03:51.000000 hadro-0.5.0a6/hadro/serde/section_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.373876 hadro-0.5.0a6/hadro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 20:04:01.000000 hadro-0.5.0a6/hadro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 20:03:51.000000 hadro-0.5.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:04:01.373876 hadro-0.5.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-18 20:03:51.000000 hadro-0.5.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:04:01.373876 hadro-0.5.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 20:03:51.000000 hadro-0.5.0a6/tests/test_memory_table.py
```

### Comparing `hadro-0.0.4/LICENSE` & `hadro-0.5.0a6/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Justin Joyce
+Copyright (c) 2023-2024 Justin Joyce
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hadro-0.0.4/hadro/engine.py` & `hadro-0.5.0a6/hadro/_engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,81 +4,40 @@
 
     disk: DiskStorage = DiskStore(file_name="books.db")
     disk.set(key="othello", value="shakespeare")
     author: str = disk.get("othello")
     # it also supports dictionary style API too:
     disk["hamlet"] = "shakespeare"
 """
+
 import io
 import os.path
 import struct
 import typing
 from collections import namedtuple
 
-from hadro.config import WRITE_CONSISTENCY
-from hadro.config import ConsistencyMode
 from orso import logging
 from orso.row import Row
 
+from hadro.config import WRITE_CONSISTENCY
+from hadro.config import ConsistencyMode
+
 logging.set_log_name("MESOS")
 logger = logging.get_logger()
 logger.setLevel(5)
 
 DELETED_FLAG: int = 1
+ROW_HEADER_SIZE: int = 5
 
 RecordHeader = namedtuple("RecordHeader", ["flags", "size"])
 
 
-# DiskStorage is a Log-Structured Hash Table as described in the BitCask paper. We
-# keep appending the data to a file, like a log. DiskStorage maintains an in-memory
-# hash table called KeyDir, which keeps the row's location on the disk.
-#
-# The idea is simple yet brilliant:
-#   - Write the record to the disk
-#   - Update the internal hash table to point to that byte offset
-#   - Whenever we get a read request, check the internal hash table for the address,
-#       fetch that and return
-#
-# KeyDir does not store values, only their locations.
-#
-# The above approach solves a lot of problems:
-#   - Writes are insanely fast since you are just appending to the file
-#   - Reads are insanely fast since you do only one disk seek. In B-Tree backed
-#       storage, there could be 2-3 disk seeks
-#
-# However, there are drawbacks too:
-#   - We need to maintain an in-memory hash table KeyDir. A database with a large
-#       number of keys would require more RAM
-#   - Since we need to build the KeyDir at initialisation, it will affect the startup
-#       time too
-#   - Deleted keys need to be purged from the file to reduce the file size
-#
-# Read the paper for more details: https://riak.com/assets/bitcask-intro.pdf
-
-
 class HadroDB:
     """
     Implements the KV store on the disk
-
-    Args:
-        file_name (str): name of the file where all the data will be written. Just
-            passing the file name will save the data in the current directory. You may
-            pass the full file location too.
-
-    Attributes:
-        file_name (str): name of the file where all the data will be written. Just
-            passing the file name will save the data in the current directory. You may
-            pass the full file location too.
-        file (typing.BinaryIO): file object pointing the file_name
-        write_position (int): current cursor position in the file where the data can be
-            written
-        key_dir (dict[str, KeyEntry]): is a map of key and KeyEntry being the value.
-            KeyEntry contains the position of the byte offset in the file where the
-            value exists. key_dir map acts as in-memory index to fetch the values
-            quickly from the disk
     """
 
     def __init__(self, collection: typing.Union[str, None] = None):
         logger.warning("HadroDB is experimental and not recommended for use.")
         self.collection: str = collection
         self.file_name: str = collection + "/00000000.data"
         self._schema_file: str = collection + "/00000000.schema"
@@ -87,22 +46,17 @@
 
         if collection is None:
             raise ValueError("HadroDB requires a collection name")
         # if the collection exists, it must be a folder, not a file
         if os.path.exists(collection):
             if not os.path.isdir(collection):
                 raise ValueError("Collection must be a folder")
-            # if the file exists already, then we will load the key_dir
-        #            self._init_key_dir()
         else:
             os.makedirs(collection, exist_ok=True)
 
-        #        if os.path.exists(self._schema_file):
-        #            load the schema
-
         # we open the file in `a+b` mode:
         # a - says the writes are append only. `a+` means we want append and read
         # b - says that we are operating the file in binary mode (as opposed to the
         #     default string mode)
         self.file: typing.BinaryIO = open(self.file_name, "a+b")
         self.fileno = self.file.fileno()
 
@@ -128,29 +82,27 @@
         record = self.rows(_record)
         # test it matches the schema
 
         bytes_to_write = record.to_bytes()
         self._write(bytes_to_write)
 
         # update indices index
-        #
-
         self.write_position += len(bytes_to_write)
 
     def scan(self, columns=None, predicates=None):
-        block_size: int = 8 * 1024 * 1024  # read 1Mb at a time
+        block_size: int = 8 * 1024 * 1024  # read 8Mb at a time
         self.file.seek(0, 0)
 
         # TODO: read file header
 
         buffer = io.BufferedReader(self.file, block_size)  # type: ignore
 
-        header_bytes = buffer.read(5)
+        header_bytes = buffer.read(ROW_HEADER_SIZE)
         flags, size = struct.unpack(">BI", header_bytes)
-        block_start = 5  # start of the current block
+        block_start = ROW_HEADER_SIZE  # start of the current block
 
         while size > 0:
             if block_start + size > block_size:
                 # The current record spans multiple blocks, so read the rest of it in the next block
                 remaining_size = size - (block_size - block_start)
                 data_bytes = bytearray(
                     buffer.read(block_size - block_start)
@@ -166,19 +118,21 @@
                 data_bytes = bytearray(buffer.read(size))
                 block_start += size
 
             if flags & DELETED_FLAG == 0:
                 yield self.rows.from_bytes(data_bytes)
 
             # Read the size of the next record
-            header_bytes = buffer.read(5)
+            header_bytes = buffer.read(ROW_HEADER_SIZE)
             if len(header_bytes) == 0:
                 break
             flags, size = struct.unpack(">BI", header_bytes)
-            block_start += 5  # add the size of the size field to the start of the next block
+            block_start += (
+                ROW_HEADER_SIZE  # add the size of the size field to the start of the next block
+            )
 
     def _write(self, data: bytes) -> None:
         # saving stuff to a file reliably is hard!
         # if you would like to explore and learn more, then
         # start from here: https://danluu.com/file-consistency/
         # and read this too: https://lwn.net/Articles/457667/
         os.write(self.fileno, data)
```

### Comparing `hadro-0.0.4/setup.py` & `hadro-0.5.0a6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,61 @@
+import platform
+
+import numpy
+from Cython.Build import cythonize
+from setuptools import Extension
 from setuptools import find_packages
 from setuptools import setup
 
 LIBRARY = "hadro"
 
 
+def is_mac():  # pragma: no cover
+    return platform.system().lower() == "darwin"
+
+
+if is_mac():
+    COMPILE_FLAGS = ["-O2"]
+else:
+    COMPILE_FLAGS = ["-O2", "-march=native"]
+
+__author__ = "notset"
 __version__ = "notset"
-with open(f"{LIBRARY}/version.py", mode="r") as v:
+with open(f"{LIBRARY}/__version__.py", mode="r") as v:
     vers = v.read()
 exec(vers)  # nosec
 
 with open("README.md", mode="r", encoding="UTF8") as rm:
     long_description = rm.read()
 
 try:
     with open("requirements.txt", "r") as f:
         required = f.read().splitlines()
 except:
     with open(f"{LIBRARY}.egg-info/requires.txt", "r") as f:
         required = f.read().splitlines()
 
+extensions = [
+    Extension(
+        name="hadro.compiled.memtable",
+        sources=["hadro/compiled/memtable.pyx"],
+        language="c++",
+        extra_compile_args=COMPILE_FLAGS + ["-std=c++11"],
+    )
+]
 
 setup_config = {
     "name": LIBRARY,
     "version": __version__,
     "description": "Storage Engine",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
-    "maintainer": "@joocer",
-    "author": "@joocer",
+    "maintainer": __author__,
+    "author": __author__,
     "author_email": "justin.joyce@joocer.com",
     "packages": find_packages(include=[LIBRARY, f"{LIBRARY}.*"]),
-    "url": "https://github.com/mabel-dev/hadrodb/",
+    "url": "https://github.com/mabel-dev/hadro/",
     "install_requires": required,
+    "ext_modules": cythonize(extensions),
 }
 
 setup(**setup_config)
```

