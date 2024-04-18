# Comparing `tmp/uglyorange-0.0.3.tar.gz` & `tmp/uglyorange-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uglyorange-0.0.3.tar", max compression
+gzip compressed data, was "uglyorange-0.0.4.tar", max compression
```

## Comparing `uglyorange-0.0.3.tar` & `uglyorange-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026996 uglyorange-0.0.3/README.md
--rw-r--r--   0        0        0      496 2024-03-30 06:26:03.615121 uglyorange-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026944 uglyorange-0.0.3/uglyorange/__init__.py
--rw-r--r--   0        0        0     3313 2024-03-30 06:24:14.794624 uglyorange-0.0.3/uglyorange/network.py
--rw-r--r--   0        0        0      313 2024-03-30 03:39:04.125950 uglyorange-0.0.3/uglyorange/utils.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 uglyorange-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026996 uglyorange-0.0.4/README.md
+-rw-r--r--   0        0        0      511 2024-04-18 02:26:36.235538 uglyorange-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-29 06:27:57.026944 uglyorange-0.0.4/uglyorange/__init__.py
+-rw-r--r--   0        0        0     3424 2024-04-18 02:26:24.287567 uglyorange-0.0.4/uglyorange/network.py
+-rw-r--r--   0        0        0      313 2024-03-30 03:39:04.125950 uglyorange-0.0.4/uglyorange/utils.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 uglyorange-0.0.4/PKG-INFO
```

### Comparing `uglyorange-0.0.3/uglyorange/network.py` & `uglyorange-0.0.4/uglyorange/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 import socket
 import httpx
 import codefast as cf
+from codefast.utils import timeout
 import os
 import sys
 import subprocess
 import argparse
 from .utils import get_system_info
 
 
@@ -70,20 +71,25 @@
             sock.close()
 
     def is_socks5_working(self):
         proxies = {
             'http://': 'socks5://{}:{}'.format(self.args.host, self.args.port),
             'https://': 'socks5://{}:{}'.format(self.args.host, self.args.port)
         }
-        with httpx.Client(proxies=proxies) as client:
-            try:
+
+        @timeout(5)
+        def _worker():
+            with httpx.Client(proxies=proxies) as client:
                 response = client.get('http://www.google.com')
                 return response.status_code == 200
-            except:
-                return False
+
+        try:
+            return _worker()
+        except Exception:
+            return False
 
     def is_http_working(self):
         proxies = {'http://': 'http://{}:{}'.format(self.args.host, self.args.port),
                    'https://': 'http://{}:{}'.format(self.args.host, self.args.port)}
         with httpx.Client(proxies=proxies) as client:
             try:
                 response = client.get('http://www.google.com')
```

### Comparing `uglyorange-0.0.3/PKG-INFO` & `uglyorange-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: uglyorange
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: ultrasev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: codefast (>=24.2.24.10,<25.0.0.0)
 Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: httpx[socks] (>=0.27.0,<0.28.0)
+Requires-Dist: lxml (==4.9.4)
 Description-Content-Type: text/markdown
```

