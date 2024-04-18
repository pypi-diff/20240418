# Comparing `tmp/jy_lib-0.6.1.tar.gz` & `tmp/jy_lib-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.6.1.tar` & `jy_lib-0.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.6.1/.gitignore
--rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.6.1/.pypirc
--rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.6.1/.vscode/launch.json
--rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.6.1/.vscode/settings.json
--rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.6.1/LICENSE
--rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.6.1/Pipfile
--rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.6.1/Pipfile.lock
--rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.6.1/README.md
--rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.6.1/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-17 00:51:39.198589 jy_lib-0.6.1/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.6.1/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.6.1/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.6.1/jy_lib/base.py
--rw-r--r--   0        0        0     2758 2024-03-29 02:02:03.064817 jy_lib-0.6.1/jy_lib/cache.py
--rw-r--r--   0        0        0     3356 2024-04-15 08:39:28.625202 jy_lib-0.6.1/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.6.1/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.6.1/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.6.1/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.6.1/jy_lib/date.py
--rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.6.1/jy_lib/decorator.py
--rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.6.1/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.6.1/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.6.1/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.6.1/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.6.1/jy_lib/nav.py
--rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.6.1/jy_lib/smb_client.py
--rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.6.1/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.6.1/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.6.1/jy_lib/time.py
--rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.6.1/publish-jypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.6.1/publish-pypi.sh
--rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.6.1/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.6.1/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.6.2/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.6.2/.pypirc
+-rw-r--r--   0        0        0      466 2023-10-19 02:20:46.582059 jy_lib-0.6.2/.vscode/launch.json
+-rw-r--r--   0        0        0     1615 2023-10-19 02:20:46.582499 jy_lib-0.6.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.6.2/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.6.2/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.6.2/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.6.2/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.6.2/README_Project.md
+-rw-r--r--   0        0        0      518 2024-04-18 00:57:34.004921 jy_lib-0.6.2/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.6.2/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.6.2/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.6.2/jy_lib/base.py
+-rw-r--r--   0        0        0     2972 2024-04-18 00:57:02.602284 jy_lib-0.6.2/jy_lib/cache.py
+-rw-r--r--   0        0        0     3356 2024-04-15 08:39:28.625202 jy_lib-0.6.2/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.6.2/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.6.2/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.6.2/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.6.2/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.6.2/jy_lib/decorator.py
+-rw-r--r--   0        0        0     4230 2023-10-25 08:34:10.094139 jy_lib-0.6.2/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.6.2/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.6.2/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.6.2/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.6.2/jy_lib/nav.py
+-rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.6.2/jy_lib/smb_client.py
+-rw-r--r--   0        0        0     4385 2024-01-16 08:18:48.686163 jy_lib-0.6.2/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.6.2/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.6.2/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.6.2/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.6.2/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.6.2/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.6.2/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.6.2/PKG-INFO
```

### Comparing `jy_lib-0.6.1/.gitignore` & `jy_lib-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/.vscode/settings.json` & `jy_lib-0.6.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/LICENSE` & `jy_lib-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/Pipfile` & `jy_lib-0.6.2/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/Pipfile.lock` & `jy_lib-0.6.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/__init__.py` & `jy_lib-0.6.2/jy_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     WarrantsType,
     BlockType,
     SpotType,
     SymbolType,
     SymbolFlag,
 )
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
```

### Comparing `jy_lib-0.6.1/jy_lib/auth_client.py` & `jy_lib-0.6.2/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/bank.py` & `jy_lib-0.6.2/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/base.py` & `jy_lib-0.6.2/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/cache.py` & `jy_lib-0.6.2/jy_lib/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # -*- coding: utf-8 -*-
+import inspect
 import lz4.frame
 import math
+import os
 import pickle
 import re
 import sqlite3
 import time
 from typing import Any, Set, List
 
 
 class Cache:
     """持久化TTL缓存"""
 
     def __init__(self, path: str):
-        self.path: str = path
+        current_frame = inspect.currentframe()
+        caller_frame = current_frame.f_back
+        caller_file = caller_frame.f_code.co_filename
+        self.path: str = os.path.join(os.path.dirname(caller_file), path)
         self.conn = sqlite3.connect(self.path)
         self.datasets: Set[str] = self.get_tables()
 
     def get_tables(self) -> Set[str]:
         cursor = self.conn.cursor()
         r = cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
         return {row[0] for row in r.fetchall()}
```

### Comparing `jy_lib-0.6.1/jy_lib/clickhouse.py` & `jy_lib-0.6.2/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/compressor.py` & `jy_lib-0.6.2/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/country.py` & `jy_lib-0.6.2/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/currency.py` & `jy_lib-0.6.2/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/date.py` & `jy_lib-0.6.2/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/decorator.py` & `jy_lib-0.6.2/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/exchange.py` & `jy_lib-0.6.2/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/interrupt_protect.py` & `jy_lib-0.6.2/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/lock.py` & `jy_lib-0.6.2/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/math.py` & `jy_lib-0.6.2/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/nav.py` & `jy_lib-0.6.2/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/smb_client.py` & `jy_lib-0.6.2/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/symbol.py` & `jy_lib-0.6.2/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/symbol_em.py` & `jy_lib-0.6.2/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/jy_lib/time.py` & `jy_lib-0.6.2/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.6.1/pyproject.toml` & `jy_lib-0.6.2/pyproject.toml`

 * *Files identical despite different names*

