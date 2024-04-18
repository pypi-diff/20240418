# Comparing `tmp/pypentair-0.1.0.tar.gz` & `tmp/pypentair-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypentair-0.1.0.tar", max compression
+gzip compressed data, was "pypentair-0.2.0.tar", max compression
```

## Comparing `pypentair-0.1.0.tar` & `pypentair-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-07-10 19:25:14.870837 pypentair-0.1.0/LICENSE
--rw-r--r--   0        0        0       70 2023-07-10 19:25:14.870837 pypentair-0.1.0/README.md
--rw-r--r--   0        0        0      223 2023-07-10 19:25:32.559131 pypentair-0.1.0/pypentair/__init__.py
--rw-r--r--   0        0        0      324 2023-07-10 19:25:14.870837 pypentair-0.1.0/pypentair/const.py
--rw-r--r--   0        0        0      212 2023-07-10 19:25:14.870837 pypentair-0.1.0/pypentair/exceptions.py
--rw-r--r--   0        0        0     5417 2023-07-10 19:25:14.870837 pypentair-0.1.0/pypentair/pentair.py
--rw-r--r--   0        0        0        0 2023-07-10 19:25:14.870837 pypentair-0.1.0/pypentair/py.typed
--rw-r--r--   0        0        0     1231 2023-07-10 19:25:14.870837 pypentair-0.1.0/pypentair/utils.py
--rw-r--r--   0        0        0     1096 2023-07-10 19:25:32.559131 pypentair-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 pypentair-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 20:53:38.807083 pypentair-0.2.0/LICENSE
+-rw-r--r--   0        0        0       70 2024-04-18 20:53:38.807083 pypentair-0.2.0/README.md
+-rw-r--r--   0        0        0      224 2024-04-18 20:53:51.203212 pypentair-0.2.0/pypentair/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-18 20:53:38.807083 pypentair-0.2.0/pypentair/const.py
+-rw-r--r--   0        0        0      212 2024-04-18 20:53:38.807083 pypentair-0.2.0/pypentair/exceptions.py
+-rw-r--r--   0        0        0     5418 2024-04-18 20:53:38.807083 pypentair-0.2.0/pypentair/pentair.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:53:38.807083 pypentair-0.2.0/pypentair/py.typed
+-rw-r--r--   0        0        0    10477 2024-04-18 20:53:38.807083 pypentair-0.2.0/pypentair/utils.py
+-rw-r--r--   0        0        0     1428 2024-04-18 20:53:51.203212 pypentair-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 pypentair-0.2.0/PKG-INFO
```

### Comparing `pypentair-0.1.0/LICENSE` & `pypentair-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypentair-0.1.0/pypentair/pentair.py` & `pypentair-0.2.0/pypentair/pentair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pentair account."""
+
 from __future__ import annotations
 
 import logging
 from typing import Any, Final
 from urllib.parse import urljoin
 
 import requests
```

### Comparing `pypentair-0.1.0/PKG-INFO` & `pypentair-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pypentair
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for interacting with Pentair Home devices
 Home-page: https://github.com/natekspencer/pypentair
 License: MIT
 Keywords: Pentair,Pentair Home,salt level sensor,python
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.27.1,<2.0.0)
 Requires-Dist: pycognito (>=2023.5.0,<2024.0.0)
 Project-URL: Repository, https://github.com/natekspencer/pypentair
 Description-Content-Type: text/markdown
 
 # pypentair
```

