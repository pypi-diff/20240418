# Comparing `tmp/geventhttpclient-2.2.0.tar.gz` & `tmp/geventhttpclient-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.2.0.tar", last modified: Fri Apr 12 15:24:34 2024, max compression
+gzip compressed data, was "geventhttpclient-2.2.1.tar", last modified: Tue Apr 16 16:41:03 2024, max compression
```

## Comparing `geventhttpclient-2.2.0.tar` & `geventhttpclient-2.2.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/ext/Python_compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/ext/_parser.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/LICENSE-MIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/include/
--rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/include/llhttp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/api.c
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/http.c
--rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/llhttp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.086324 geventhttpclient-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/src/geventhttpclient/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/connectionpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/src/geventhttpclient/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/oncert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/server.key
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_http_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_network_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_no_module_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    20093 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/ext/Python_compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/ext/_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/LICENSE-MIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/llhttp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.241198 geventhttpclient-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/src/geventhttpclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/connectionpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/src/geventhttpclient/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/oncert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_network_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_no_module_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/top_level.txt
```

### Comparing `geventhttpclient-2.2.0/LICENSE.txt` & `geventhttpclient-2.2.1/LICENSE-MIT`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-Based on llhttp, copyright Fedor Indutny, 2018.
+This software is licensed under the MIT License.
 
-Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
-licensed under the same terms.
+Copyright Antonin Amand <antonin.amand@gmail.com>, 2018.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to
-deal in the Software without restriction, including without limitation the
-rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-sell copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to permit
+persons to whom the Software is furnished to do so, subject to the
+following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-IN THE SOFTWARE.
-
-Note: Previous versions of gevenhttpclient used http_parser.c, which in turn 
-was based on src/http/ngx_http_parse.c from NGINX, copyright Igor Sysoev, 
-Joyent, Inc. and other Node contributors. See http://github.com/joyent/http-parser 
-for more information
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `geventhttpclient-2.2.0/PKG-INFO` & `geventhttpclient-2.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.2.0
+Version: 2.2.1
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
-License: Based on llhttp, copyright Fedor Indutny, 2018.
+License: This software is licensed under the MIT License.
         
-        Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
-        licensed under the same terms.
+        Copyright Antonin Amand <antonin.amand@gmail.com>, 2018.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to
-        deal in the Software without restriction, including without limitation the
-        rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-        sell copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-        FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-        IN THE SOFTWARE.
-        
-        Note: Previous versions of gevenhttpclient used http_parser.c, which in turn 
-        was based on src/http/ngx_http_parse.c from NGINX, copyright Igor Sysoev, 
-        Joyent, Inc. and other Node contributors. See http://github.com/joyent/http-parser 
-        for more information
+        Permission is hereby granted, free of charge, to any person obtaining a
+        copy of this software and associated documentation files (the
+        "Software"), to deal in the Software without restriction, including
+        without limitation the rights to use, copy, modify, merge, publish,
+        distribute, sublicense, and/or sell copies of the Software, and to permit
+        persons to whom the Software is furnished to do so, subject to the
+        following conditions:
+        
+        The above copyright notice and this permission notice shall be included
+        in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+        OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+        NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+        DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+        OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+        USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: homepage, http://github.com/geventhttpclient/geventhttpclient
 Project-URL: issues, http://github.com/geventhttpclient/geventhttpclient/issues
 Project-URL: download, https://pypi.org/project/geventhttpclient/#files
 Keywords: http,gevent,client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE-MIT
 Requires-Dist: gevent
 Requires-Dist: certifi
 Requires-Dist: brotli
 Requires-Dist: urllib3
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: dpkt; extra == "dev"
@@ -237,7 +233,15 @@
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
+
+## License
+
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
+Previous versions of geventhttpclient used http_parser.c, which in turn 
+was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
+Joyent, Inc., and other Node contributors. For more information, see 
+http://github.com/joyent/http-parser
```

### Comparing `geventhttpclient-2.2.0/README.md` & `geventhttpclient-2.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -170,7 +170,15 @@
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
+
+## License
+
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
+Previous versions of geventhttpclient used http_parser.c, which in turn 
+was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
+Joyent, Inc., and other Node contributors. For more information, see 
+http://github.com/joyent/http-parser
```

### Comparing `geventhttpclient-2.2.0/ext/_parser.c` & `geventhttpclient-2.2.1/ext/_parser.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/llhttp/LICENSE-MIT` & `geventhttpclient-2.2.1/llhttp/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/llhttp/include/llhttp.h` & `geventhttpclient-2.2.1/llhttp/include/llhttp.h`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/llhttp/src/api.c` & `geventhttpclient-2.2.1/llhttp/src/api.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/llhttp/src/http.c` & `geventhttpclient-2.2.1/llhttp/src/http.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/llhttp/src/llhttp.c` & `geventhttpclient-2.2.1/llhttp/src/llhttp.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/pyproject.toml` & `geventhttpclient-2.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "geventhttpclient"
-version = "2.2.0" # dont forget to update version __init__.py as well
+version = "2.2.1" # dont forget to update version __init__.py as well
 description = "HTTP client library for gevent"
 readme = "README.md"
 requires-python = ">=3.9"
-license = {file = "LICENSE.txt"}
+license = {file = "LICENSE-MIT"}
 keywords = ["http", "gevent", "client"]
 authors = [{name = "Antonin Amand", email = "antonin.amand@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/client.py` & `geventhttpclient-2.2.1/src/geventhttpclient/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,22 +142,18 @@
             )
         self.version = version
         self.headers_type = headers_type
         self.default_headers = headers_type()
         self.default_headers.update(self.DEFAULT_HEADERS)
         self.default_headers.update(headers)
         self.block_size = block_size
-        self._base_url_string = str(self.get_base_url())
 
-    def get_base_url(self):
-        url = URL()
-        url.host = self.host
-        url.port = self.port
-        url.scheme = self.ssl and PROTO_HTTPS or PROTO_HTTP
-        return url
+        scheme = PROTO_HTTPS if self.ssl else PROTO_HTTP
+        port_str = f":{port}" if port else ""
+        self._base_url_string = f"{scheme}://{self.host}{port_str}/"
 
     def close(self):
         self._connection_pool.close()
 
     # Like urllib2, try to treat the body as a file if we can't determine the
     # file length with `len()`
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/connectionpool.py` & `geventhttpclient-2.2.1/src/geventhttpclient/connectionpool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from contextlib import contextmanager
 
 import gevent.queue
 import gevent.socket
 from gevent import lock
 
 _CA_CERTS = None
 
@@ -194,20 +193,23 @@
     ssl_context.check_hostname = check_hostname
     if check_hostname:
         ssl_context.verify_mode = gevent.ssl.CERT_REQUIRED
     return ssl_context
 
 
 try:
+    from ssl import PROTOCOL_TLS_CLIENT
+
     import gevent.ssl
 
     try:
         from gevent.ssl import create_default_context
     except ImportError:
         create_default_context = None
+
 except ImportError:
     pass
 else:
 
     class SSLConnectionPool(ConnectionPool):
         """SSLConnectionPool creates connections wrapped with SSL/TLS.
 
@@ -218,14 +220,15 @@
             if provided. It must be a callable that returns a SSLContext.
         """
 
         default_options = {
             "ciphers": _DEFAULT_CIPHERS,
             "ca_certs": _CA_CERTS,
             "cert_reqs": gevent.ssl.CERT_REQUIRED,
+            "ssl_version": PROTOCOL_TLS_CLIENT,
         }
 
         def __init__(
             self,
             connection_host,
             connection_port,
             request_host,
@@ -256,34 +259,7 @@
             sock = super()._connect_socket(sock, address)
 
             if self.ssl_context is None:
                 return gevent.ssl.wrap_socket(sock, **self.ssl_options)
             else:
                 server_hostname = self.ssl_options.get("server_hostname", self._request_host)
                 return self.ssl_context.wrap_socket(sock, server_hostname=server_hostname)
-
-
-class ClientPool:
-    """
-    Pool implementation for HTTP clients, that weren't designed with concurrency in mind.
-    Usage example:
-
-    pool = ClientPool(MyHttpClient)
-    with pool.get() as client:
-        response = client.request("127.0.0.1")
-    """
-
-    def __init__(self, factory, concurrency=5):
-        self.factory = factory
-        self.queue = gevent.queue.Queue(concurrency)
-        for i in range(concurrency):
-            self.queue.put(factory())
-
-    @contextmanager
-    def get(self):
-        client = self.queue.get()
-        yield client
-        self.queue.put(client)
-
-    def close(self):
-        for client in self.queue:
-            client.close()
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/header.py` & `geventhttpclient-2.2.1/src/geventhttpclient/header.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/httplib.py` & `geventhttpclient-2.2.1/src/geventhttpclient/httplib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Provide HTTPConnection, HTTPSConnection and HTTPResponse implementations ready
 to use as drop-in replacements for their counterparts in http.client.
 """
 
-import http.client as httplib
+import http.client
+from contextlib import contextmanager
 
 import gevent.socket
 import gevent.ssl
 
 from geventhttpclient import connectionpool, header, response
 
-_UNKNOWN = getattr(httplib, "_UNKNOWN", "UNKNOWN")
+_UNKNOWN = getattr(http.client, "_UNKNOWN", "UNKNOWN")
 
 
 class HTTPLibHeaders(header.Headers):
     def __getitem__(self, key):
         value = super().__getitem__(key)
         if isinstance(value, (list, tuple)):
             return ", ".join(value)
@@ -116,18 +117,15 @@
     def geturl(self):
         return self.url
 
     def getcode(self):
         return self.status_code
 
 
-HTTPLibConnection = httplib.HTTPConnection
-
-
-class HTTPConnection(httplib.HTTPConnection):
+class HTTPConnection(http.client.HTTPConnection):
     response_class = HTTPResponse
     source_address = None
     _hidden_socket = None
 
     def connect(self):
         self.sock = gevent.socket.create_connection(
             (self.host, self.port), self.timeout, self.source_address
@@ -216,13 +214,39 @@
                 self._tunnel()
             self.sock = gevent.ssl.SSLSocket(
                 sock, _context=self._context, server_hostname=self.host
             )
 
 
 def patch():
-    httplib.HTTPConnection = HTTPConnection
-    httplib.HTTPResponse = HTTPResponse
+    http.client.HTTPConnection = HTTPConnection
+    http.client.HTTPResponse = HTTPResponse
+    try:
+        http.client.HTTPSConnection = HTTPSConnection
+    except NameError:
+        pass
+
+
+@contextmanager
+def patched():
+    """Temporarily patch http.client."""
+    http_client_HTTPConnection = http.client.HTTPConnection
+    http_client_HTTPResponse = http.client.HTTPResponse
     try:
-        httplib.HTTPSConnection = HTTPSConnection
+        http_client_HTTPSConnection = http.client.HTTPSConnection
     except NameError:
         pass
+    try:
+        http.client.HTTPConnection = HTTPConnection
+        http.client.HTTPResponse = HTTPResponse
+        try:
+            http.client.HTTPSConnection = HTTPSConnection
+        except NameError:
+            pass
+        yield
+    finally:
+        http.client.HTTPConnection = http_client_HTTPConnection
+        http.client.HTTPResponse = http_client_HTTPResponse
+        try:
+            http.client.HTTPSConnection = http_client_HTTPSConnection
+        except NameError:
+            pass
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/httplib2.py` & `geventhttpclient-2.2.1/src/geventhttpclient/httplib2.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,30 +8,62 @@
 httplib.patch()
 
 from geventhttpclient import httplib2
 
 http = httplib2.Http(concurrency=5)
 """
 
-from httplib2 import Http as httplib2_Http
+from contextlib import contextmanager
 
-from geventhttpclient.connectionpool import ClientPool
+import gevent.queue
 
+import geventhttpclient.httplib
 
-class Http:
-    """Imitate a httplib2.Http client. Except that it is now run concurrently."""
 
-    def __init__(self, *args, **kw):
-        self.concurrency = max(kw.pop("concurrency", 0), 2)  # never smaller than 2
-        self.args = args
-        self.kw = kw
-        self.pool = ClientPool(self._http_factory, concurrency=self.concurrency)
+class ClientPool:
+    """
+    Pool implementation for HTTP clients, that weren't designed with concurrency in mind.
+    Usage example:
+
+    pool = ClientPool(MyHttpClient)
+    with pool.get() as client:
+        response = client.request("127.0.0.1")
+    """
+
+    def __init__(self, factory, concurrency=5):
+        self.factory = factory
+        self.queue = gevent.queue.Queue(concurrency)
+        for i in range(concurrency):
+            self.queue.put(factory())
+
+    @contextmanager
+    def get(self):
+        client = self.queue.get()
+        yield client
+        self.queue.put(client)
 
-    def _http_factory(self):
-        return httplib2_Http(*self.args, **self.kw)
+    def close(self):
+        for client in self.queue:
+            client.close()
 
-    def request(self, *args, **kw):
-        with self.pool.get() as client:
-            return client.request(*args, **kw)
 
-    def close(self):
-        self.pool.close()
+with geventhttpclient.httplib.patched():
+    import httplib2
+
+    class Http:
+        """Imitate a httplib2.Http client. Except that it is now run concurrently."""
+
+        def __init__(self, *args, **kw):
+            self.concurrency = max(kw.pop("concurrency", 0), 2)  # never smaller than 2
+            self.args = args
+            self.kw = kw
+            self.pool = ClientPool(self._http_factory, concurrency=self.concurrency)
+
+        def _http_factory(self):
+            return httplib2.Http(*self.args, **self.kw)
+
+        def request(self, *args, **kw):
+            with self.pool.get() as client:
+                return client.request(*args, **kw)
+
+        def close(self):
+            self.pool.close()
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/response.py` & `geventhttpclient-2.2.1/src/geventhttpclient/response.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/oncert.pem` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/oncert.pem`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/server.crt` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/server.crt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/server.key` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/server.key`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_client.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,17 @@
 import json
-import os
-from contextlib import contextmanager
 
 import gevent.pool
-import gevent.pywsgi
+import gevent.queue
 import gevent.server
 import pytest
-from gevent.ssl import SSLError
 
-from geventhttpclient import HTTPClient, __version__
-
-LISTENER = "127.0.0.1", 54323
-HTTPBIN_HOST = "httpbingo.org"  # this might be exchanged with a self-hosted version
-
-
-@contextmanager
-def server(handler):
-    server = gevent.server.StreamServer(LISTENER, handle=handler)
-    server.start()
-    try:
-        yield
-    finally:
-        server.stop()
-
-
-@contextmanager
-def wsgiserver(handler):
-    server = gevent.pywsgi.WSGIServer(LISTENER, handler)
-    server.start()
-    try:
-        yield
-    finally:
-        server.stop()
+from geventhttpclient import __version__
+from geventhttpclient.client import METHOD_GET, HTTPClient
+from geventhttpclient.tests.conftest import HTTPBIN_HOST, LISTENER, server, wsgiserver
 
 
 def httpbin_client(
     host=HTTPBIN_HOST,
     port=None,
     headers=None,
     block_size=HTTPClient.BLOCK_SIZE,
@@ -76,20 +52,30 @@
 def httpbin():
     return httpbin_client()
 
 
 @pytest.mark.parametrize("request_uri", ["/tp/", "tp/", f"http://{HTTPBIN_HOST}/tp/"])
 def test_build_request(httpbin, request_uri):
     request_ref = f"GET /tp/ HTTP/1.1\r\nUser-Agent: python/gevent-http-client-{__version__}\r\nHost: {HTTPBIN_HOST}\r\n\r\n"
-    assert httpbin._build_request("GET", request_uri) == request_ref
+    assert httpbin._build_request(METHOD_GET, request_uri) == request_ref
 
 
 def test_build_request_invalid_host(httpbin):
     with pytest.raises(ValueError):
-        httpbin._build_request("GET", "http://someunrelatedhost.com/")
+        httpbin._build_request(METHOD_GET, "http://someunrelatedhost.com/")
+
+
+@pytest.mark.parametrize("port", [None, 1234])
+@pytest.mark.parametrize("host", ["localhost", "127.0.0.1", "::1", "[::1]"])
+def test_build_request_host(host, port):
+    client = HTTPClient(host, port)
+    host_ref = (
+        f"host: {f'[{host}]' if host.startswith(':') else host}{f':{port}' if port else ''}\r\n"
+    )
+    assert host_ref in client._build_request(METHOD_GET, "").lower()
 
 
 test_url_client_args = [
     ("http://python.org", ("python.org", 80)),
     ("http://python.org:333", ("python.org", 333)),
 ]
 
@@ -251,15 +237,15 @@
 def test_bytes_post():
     with wsgiserver(check_upload(b"12345", 5)):
         client = HTTPClient(*LISTENER)
         client.post("/", b"12345")
 
 
 def test_string_post():
-    with wsgiserver(check_upload("12345", 5)):
+    with wsgiserver(check_upload(b"12345", 5)):
         client = HTTPClient(*LISTENER)
         client.post("/", "12345")
 
 
 def test_unicode_post():
     byte_string = b"\xc8\xb9\xc8\xbc\xc9\x85"
     unicode_string = byte_string.decode("utf-8")
@@ -331,34 +317,14 @@
     with httpbin.get("/") as response:
         assert response.status_code == 200
         r = response
     assert r._sock is None  # released
 
 
 @pytest.mark.network
-def test_client_ssl():
-    client = HTTPClient("github.com", ssl=True)
-    assert client.port == 443
-    response = client.get("/")
-    assert response.status_code == 200
-    body = response.read()
-    assert len(body)
-
-
-@pytest.mark.network
-def test_ssl_fail_invalid_certificate():
-    certs = os.path.join(os.path.dirname(os.path.abspath(__file__)), "oncert.pem")
-    client = HTTPClient("github.com", ssl_options={"ca_certs": certs})
-    assert client.port == 443
-    with pytest.raises(SSLError) as e_info:
-        client.get("/")
-    assert e_info.value.reason == "CERTIFICATE_VERIFY_FAILED"
-
-
-@pytest.mark.network
 def test_multi_queries_greenlet_safe():
     httpbin = httpbin_client(concurrency=3)
     group = gevent.pool.Group()
     event = gevent.event.Event()
 
     def run(i):
         event.wait()
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_headers.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_keep_alive.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_network_failures.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_network_failures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-from contextlib import contextmanager
 from http.client import HTTPException
 
 import gevent.server
 import gevent.socket
 import pytest
 
-from geventhttpclient import HTTPClient
-
-CRLF = "\r\n"
-LISTENER = "127.0.0.1", 54323
-
-
-@contextmanager
-def server(handler):
-    server = gevent.server.StreamServer(LISTENER, handle=handler)
-    server.start()
-    try:
-        yield
-    finally:
-        server.stop()
+from geventhttpclient.client import CRLF, HTTPClient
+from geventhttpclient.tests.conftest import LISTENER, server
 
 
 def wrong_response_status_line(sock, addr):
     sock.recv(4096)
     sock.sendall(b"HTTP/1.1 apfais df0 asdf\r\n\r\n")
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_no_module_ssl.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_no_module_ssl.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_parser.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_ssl.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_ssl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 import os
 import ssl
 from contextlib import contextmanager
 from ssl import CertificateError
 from unittest import mock
 
 import dpkt.ssl
+import gevent.queue
 import gevent.server
 import gevent.socket
 import gevent.ssl
 import pytest
 from gevent import joinall
 from gevent.socket import error as socket_error
 
 from geventhttpclient import HTTPClient
-
-LISTENER = "127.0.0.1", 54323
+from geventhttpclient.tests.conftest import LISTENER
 
 BASEDIR = os.path.dirname(__file__)
 KEY = os.path.join(BASEDIR, "server.key")
 CERT = os.path.join(BASEDIR, "server.crt")
 
 
 @contextmanager
-def server(handler, backlog=1):
+def sslserver(handler, backlog=1):
+    exception_queue = gevent.queue.Queue()
+
+    def wrapped_handler(env, start_response):
+        try:
+            return handler(env, start_response)
+        except Exception as e:
+            exception_queue.put(e)
+            raise
+
     server = gevent.server.StreamServer(
         LISTENER,
         backlog=backlog,
-        handle=handler,
+        handle=wrapped_handler,
         keyfile=KEY,
         certfile=CERT,
         ssl_version=ssl.PROTOCOL_TLS_SERVER,
     )
     server.start()
     try:
-        yield (server.server_host, server.server_port)
+        yield server.server_host, server.server_port
+        if not exception_queue.empty():
+            raise exception_queue.get()
     finally:
         server.stop()
 
 
 @contextmanager
 def timeout_connect_server():
     sock = gevent.socket.socket(gevent.socket.AF_INET, gevent.socket.SOCK_STREAM, 0)
@@ -67,17 +78,17 @@
 def simple_ssl_response(sock, addr):
     sock.recv(1024)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nConnection: close\r\n\r\n")
     sock.close()
 
 
 def test_simple_ssl():
-    with server(simple_ssl_response) as listener:
-        http = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
-        response = http.get("/")
+    with sslserver(simple_ssl_response) as listener:
+        client = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
+        response = client.get("/")
         assert response.status_code == 200
         response.read()
 
 
 def timeout_on_connect(sock, addr):
     sock.recv(1024)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n")
@@ -113,15 +124,15 @@
             gevent.socket.SOCK_STREAM,
             gevent.socket.IPPROTO_TCP,
             "localhost",
             ("127.0.0.1", server_port),
         )
         with mock.patch("gevent.socket.getaddrinfo", mock.Mock(return_value=[mock_addrinfo])):
             server_host = "some_foo"
-            http = HTTPClient(
+            client = HTTPClient(
                 server_host,
                 server_port,
                 insecure=True,
                 ssl=True,
                 connection_timeout=0.1,
                 ssl_context_factory=gevent.ssl.create_default_context,
                 **additional_client_args,
@@ -129,15 +140,15 @@
 
             def run(http):
                 try:
                     http.get("/")
                 except socket_error:
                     pass  # handshake will not be completed
 
-            client_greenlet = gevent.spawn(run, http)
+            client_greenlet = gevent.spawn(run, client)
             joinall([client_greenlet, server_greenlet])
 
     return server_host, server_port, server_greenlet.value
 
 
 @contextmanager
 def sni_checker_server():
@@ -185,32 +196,34 @@
                 first_entry, _ = dpkt.ssl.parse_variable_array(sni_list, 2)
 
                 return first_entry.decode()
 
     job = gevent.spawn(run, sock)
     try:
         yield sock, job
+        if job.exception:
+            raise job.exception
         sock.close()
     finally:
         job.kill()
 
 
 def test_timeout_on_connect():
     with timeout_connect_server() as listener:
-        http = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
+        client = HTTPClient(*listener, insecure=True, ssl=True, ssl_options={"ca_certs": CERT})
 
         def run(http, wait_time=100):
             try:
                 response = http.get("/")
                 gevent.sleep(wait_time)
                 response.read()
             except Exception:
                 pass
 
-        gevent.spawn(run, http)
+        gevent.spawn(run, client)
         gevent.sleep(0)
 
         e = None
         try:
             http2 = HTTPClient(
                 *listener,
                 insecure=True,
@@ -234,25 +247,66 @@
 def network_timeout(sock, addr):
     sock.recv(1024)
     gevent.sleep(10)
     sock.sendall(b"HTTP/1.1 200 Ok\r\nContent-Length: 0\r\n\r\n")
 
 
 def test_network_timeout():
-    with server(network_timeout) as listener:
-        http = HTTPClient(
+    with sslserver(network_timeout) as listener:
+        client = HTTPClient(
             *listener,
             ssl=True,
             insecure=True,
             network_timeout=0.1,
             ssl_options={"ca_certs": CERT},
         )
         with pytest.raises(gevent.socket.timeout):
-            response = http.get("/")
-            assert response.status_code == 0, "should have timed out."
+            client.get("/")
 
 
-def test_verify_hostname():
-    with server(simple_ssl_response) as listener:
-        http = HTTPClient(*listener, ssl=True, ssl_options={"ca_certs": CERT})
-        with pytest.raises(CertificateError):
-            http.get("/")
+def check_client_cert_required(client):
+    """Make sure hostnames are checked by default."""
+    ssl_context = client._connection_pool.ssl_context
+    assert ssl_context.check_hostname
+    assert ssl_context.verify_mode == gevent.ssl.CERT_REQUIRED
+    for socket in client._connection_pool._socket_queue.queue:
+        assert socket._context.verify_mode == gevent.ssl.CERT_REQUIRED
+
+
+def test_verify_self_signed_fail(capsys):
+    with sslserver(simple_ssl_response) as listener:
+        client = HTTPClient(*listener, ssl=True)
+        with pytest.raises(CertificateError) as raised:
+            client.get("/")
+        assert "CERTIFICATE_VERIFY_FAILED" in str(raised.value)
+        assert raised.value.verify_message == "self-signed certificate"
+        check_client_cert_required(client)
+        client.close()
+
+    # This tests breaking server side socket confusingly prints its certificate error message delayed
+    # into other tests output, if we don't give it a split second for printing now.
+    gevent.sleep(0.01)
+    captured = capsys.readouterr().err
+    assert "ssl.SSLError" in captured
+    assert "ALERT_UNKNOWN_CA" in captured
+
+
+@pytest.mark.network
+def test_client_ssl():
+    client = HTTPClient("github.com", ssl=True)
+    assert client.port == 443
+    response = client.get("/")
+    assert response.status_code == 200
+    body = response.read()
+    assert len(body)
+    check_client_cert_required(client)
+
+
+@pytest.mark.network
+def test_fail_invalid_ca_certificate():
+    certs = os.path.join(os.path.dirname(os.path.abspath(__file__)), "oncert.pem")
+    client = HTTPClient("github.com", ssl_options={"ca_certs": certs})
+    assert client.port == 443
+    with pytest.raises(gevent.ssl.SSLError) as e_info:
+        client.get("/")
+    assert e_info.value.reason == "CERTIFICATE_VERIFY_FAILED"
+    check_client_cert_required(client)
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_url.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_url.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,86 @@
 import pytest
 
 from geventhttpclient.url import URL
 
-url_full = "http://getgauss.com/subdir/file.py?param=value&other=true#frag"
+url_full = "http://gevent.org/subdir/file.py?param=value&other=true#frag"
 url_path_only = "/path/to/something?param=value&other=true"
 
 
 def test_simple_url():
     url = URL(url_full)
     assert url.path == "/subdir/file.py"
-    assert url.host == "getgauss.com"
+    assert url.host == "gevent.org"
     assert url.port == 80
-    assert url.query_string == "param=value&other=true"
+    assert url.query == "param=value&other=true"
     assert url.fragment == "frag"
 
 
 def test_path_only():
     url = URL(url_path_only)
     assert url.host == ""
     assert url.port is None
     assert url.path == "/path/to/something"
-    assert url.query_string == "param=value&other=true"
+    assert url.query == "param=value&other=true"
 
 
 def test_params():
     url = URL(url_full, params={"pp": "hello"})
     assert url.path == "/subdir/file.py"
-    assert url.host == "getgauss.com"
+    assert url.host == "gevent.org"
     assert url.port == 80
-    assert url.query_string == "param=value&other=true&pp=hello"
+    assert url.query == "param=value&other=true&pp=hello"
     assert url.fragment == "frag"
 
 
 def test_params_urlencoded():
     url = URL(url_full, params={"a/b": "c/d"})
     assert url.path == "/subdir/file.py"
-    assert url.host == "getgauss.com"
+    assert url.host == "gevent.org"
     assert url.port == 80
-    assert url.query_string == "param=value&other=true&a%2Fb=c%2Fd"
+    assert url.query == "param=value&other=true&a%2Fb=c%2Fd"
     assert url.fragment == "frag"
 
 
-def test_query_string_urlencoded():
-    url = URL("http://getgauss.com/?foo=bar with spaces")
-    assert url.query_string == "foo=bar%20with%20spaces"
-    assert url.host == "getgauss.com"
+def test_query_urlencoded():
+    url = URL("http://gevent.org/?foo=bar with spaces")
+    assert url.query == "foo=bar%20with%20spaces"
+    assert url.host == "gevent.org"
     assert url.port == 80
 
 
+def test_tuple_unpack():
+    url = URL("http://gevent.org/somepath?foo=bar#frag")
+    assert len(tuple(url)) == 6
+    scheme, netloc, path, params, query, fragment = url
+    assert scheme == "http"
+    assert netloc == "gevent.org"
+    assert path == "/somepath"
+    assert query == "foo=bar"
+    assert fragment == "frag"
+
+
+def test_tuple_unpack_no_none():
+    url = URL("http://gevent.org/")
+    assert len(tuple(url)) == 6
+    assert not any(val is None for val in tuple(url))
+
+
 def test_empty():
     url = URL()
     assert url.host == ""
-    assert url.port == 80
-    assert url.query_string == ""
+    assert not url.port
+    assert url.query == ""
     assert url.fragment == ""
     assert url.netloc == ""
-    assert str(url) == "http:///"
+    assert str(url) == ""
 
 
 def test_empty_path():
-    assert URL("http://getgauss.com").path == ""
+    assert URL("http://gevent.org").path == ""
 
 
 def test_consistent_reparsing():
     for surl in (url_full, url_path_only):
         url = URL(surl)
         reparsed = URL(str(url))
         for attr in URL.__slots__:
@@ -72,70 +89,76 @@
 
 def test_redirection_abs_path():
     url = URL(url_full)
     updated = url.redirect("/test.html")
     assert updated.host == url.host
     assert updated.port == url.port
     assert updated.path == "/test.html"
-    assert updated.query_string == ""
+    assert updated.query == ""
     assert updated.fragment == ""
 
 
 @pytest.mark.parametrize("redirection", ("test.html?key=val", "folder/test.html?key=val"))
 def test_redirection_rel_path(redirection):
     url = URL(url_full)
     updated = url.redirect(redirection)
     assert updated.host == url.host
     assert updated.port == url.port
     assert updated.path.startswith("/subdir/")
     assert updated.path.endswith(redirection.split("?", 1)[0])
-    assert updated.query_string == "key=val"
+    assert updated.query == "key=val"
     assert updated.fragment == ""
 
 
 def test_redirection_full_path():
     url_full2_plain = "http://google.de/index"
     url = URL(url_full)
     updated = url.redirect(url_full2_plain)
     url_full2 = URL(url_full2_plain)
     for attr in URL.__slots__:
         assert getattr(updated, attr) == getattr(url_full2, attr)
     assert str(url_full2) == url_full2_plain
 
 
-def test_query_string():
-    assert URL("/some/url", params={"a": "b", "c": 2}).query_string == "a=b&c=2"
+def test_query():
+    assert URL("/some/url", params={"a": "b", "c": 2}).query == "a=b&c=2"
 
 
 def test_equality():
     assert URL("https://example.com/") != URL("http://example.com/")
     assert URL("http://example.com/") == URL("http://example.com/")
 
 
+def test_default_port():
+    assert URL("https://python.org").port == 443
+    assert URL("http://gevent.org").port == 80
+    assert URL("example.com").port is None
+
+
 def test_pw():
-    url = URL("http://asdf:dd@heise.de/index.php?aaaa=bbbbb")
-    assert url.host == "heise.de"
+    url = URL("http://asdf:dd@example.com/index.php?aaaa=bbbbb")
+    assert url.host == "example.com"
     assert url.port == 80
     assert url.user == "asdf"
     assert url.password == "dd"
 
 
 def test_pw_with_port():
-    url = URL("http://asdf:dd@heise.de:90/index.php?aaaa=bbbbb")
-    assert url.host == "heise.de"
+    url = URL("http://asdf:dd@example.com:90/index.php?aaaa=bbbbb")
+    assert url.host == "example.com"
     assert url.port == 90
     assert url.user == "asdf"
     assert url.password == "dd"
 
 
 def test_ipv6():
     url = URL("http://[2001:db8:85a3:8d3:1319:8a2e:370:7348]/")
     assert url.host == "2001:db8:85a3:8d3:1319:8a2e:370:7348"
     assert url.port == 80
-    assert url.user is None
+    assert url.user == ""
 
 
 def test_ipv6_with_port():
     url = URL("https://[2001:db8:85a3:8d3:1319:8a2e:370:7348]:8080/")
     assert url.host == "2001:db8:85a3:8d3:1319:8a2e:370:7348"
     assert url.port == 8080
-    assert url.user is None
+    assert url.user == ""
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_useragent.py` & `geventhttpclient-2.2.1/src/geventhttpclient/tests/test_useragent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-from contextlib import contextmanager
 from http.cookiejar import CookieJar
 
-import gevent.pywsgi
 import pytest
 
+from geventhttpclient.tests.conftest import LISTENER_URL, wsgiserver
 from geventhttpclient.useragent import BadStatusCode, UserAgent
 
-LISTENER = "127.0.0.1", 54323
-LISTENER_URL = f"http://{LISTENER[0]}:{LISTENER[1]}/"
-
 
 @pytest.fixture
 def tmp_file(tmp_path):
     fpath = tmp_path / "tmp.bin"
     with open(fpath, "wb") as f:
         f.write(b"123456789")
     return fpath
 
 
-@contextmanager
-def wsgiserver(handler):
-    server = gevent.pywsgi.WSGIServer(LISTENER, handler)
-    server.start()
-    try:
-        yield
-    finally:
-        server.stop()
-
-
 def check_upload(body, headers=None):
     def wsgi_handler(env, start_response):
         assert env["REQUEST_METHOD"] == "POST"
         assert body == env["wsgi.input"].read()
         start_response("200 OK", [])
         return []
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient/useragent.py` & `geventhttpclient-2.2.1/src/geventhttpclient/useragent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from urllib.parse import urlencode
 
 import brotli
 import gevent
 from urllib3 import encode_multipart_formdata
 from urllib3.fields import RequestField
 
-from .client import HTTPClient, HTTPClientPool
-from .url import URL, to_key_val_list
+from geventhttpclient.client import HTTPClient, HTTPClientPool
+from geventhttpclient.url import URL, to_key_val_list
 
 
 class ConnectionError(Exception):
     def __init__(self, url, *args, **kwargs):
         self.url = url
         self.__dict__.update(kwargs)
         if args and isinstance(args[0], str):
@@ -430,19 +430,19 @@
             url,
             method=method,
             headers=headers,
             payload=payload,
             params=params,
             files=files,
         )
-        for retry in range(self.max_retries):
+        for retry in range(self.max_retries + 1):
             if retry > 0 and self.retry_delay:
                 # Don't wait the first time and skip if no delay specified
                 gevent.sleep(self.retry_delay)
-            for _ in range(self.max_redirects):
+            for _ in range(self.max_redirects + 1):
                 if self.cookiejar is not None:
                     self.cookiejar.add_cookie_header(req)
 
                 try:
                     resp = self._urlopen(req)
                 except gevent.GreenletExit:
                     raise
@@ -543,15 +543,15 @@
         headers = kwargs.pop("headers", {})
         headers["Connection"] = "Keep-Alive"
         if resume and os.path.isfile(fpath):
             offset = os.path.getsize(fpath)
         else:
             offset = 0
 
-        for _ in range(self.max_retries):
+        for _ in range(self.max_retries + 1):
             if offset:
                 headers["Range"] = f"bytes={offset}-"
                 resp = self.urlopen(url, headers=headers, **kwargs)
                 cr = resp.headers.get("Content-Range")
                 if (
                     resp.status_code != 206
                     or not cr
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient.egg-info/PKG-INFO` & `geventhttpclient-2.2.1/src/geventhttpclient.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.2.0
+Version: 2.2.1
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
-License: Based on llhttp, copyright Fedor Indutny, 2018.
+License: This software is licensed under the MIT License.
         
-        Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
-        licensed under the same terms.
+        Copyright Antonin Amand <antonin.amand@gmail.com>, 2018.
         
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to
-        deal in the Software without restriction, including without limitation the
-        rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
-        sell copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-        FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-        IN THE SOFTWARE.
-        
-        Note: Previous versions of gevenhttpclient used http_parser.c, which in turn 
-        was based on src/http/ngx_http_parse.c from NGINX, copyright Igor Sysoev, 
-        Joyent, Inc. and other Node contributors. See http://github.com/joyent/http-parser 
-        for more information
+        Permission is hereby granted, free of charge, to any person obtaining a
+        copy of this software and associated documentation files (the
+        "Software"), to deal in the Software without restriction, including
+        without limitation the rights to use, copy, modify, merge, publish,
+        distribute, sublicense, and/or sell copies of the Software, and to permit
+        persons to whom the Software is furnished to do so, subject to the
+        following conditions:
+        
+        The above copyright notice and this permission notice shall be included
+        in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+        OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN
+        NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+        DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+        OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
+        USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: homepage, http://github.com/geventhttpclient/geventhttpclient
 Project-URL: issues, http://github.com/geventhttpclient/geventhttpclient/issues
 Project-URL: download, https://pypi.org/project/geventhttpclient/#files
 Keywords: http,gevent,client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE-MIT
 Requires-Dist: gevent
 Requires-Dist: certifi
 Requires-Dist: brotli
 Requires-Dist: urllib3
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: dpkt; extra == "dev"
@@ -237,7 +233,15 @@
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
+
+## License
+
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
+Previous versions of geventhttpclient used http_parser.c, which in turn 
+was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
+Joyent, Inc., and other Node contributors. For more information, see 
+http://github.com/joyent/http-parser
```

### Comparing `geventhttpclient-2.2.0/src/geventhttpclient.egg-info/SOURCES.txt` & `geventhttpclient-2.2.1/src/geventhttpclient.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.txt
+LICENSE-MIT
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 ext/Python_compat.h
 ext/_parser.c
 llhttp/LICENSE-MIT
@@ -26,15 +26,14 @@
 src/geventhttpclient.egg-info/top_level.txt
 src/geventhttpclient/tests/conftest.py
 src/geventhttpclient/tests/oncert.pem
 src/geventhttpclient/tests/server.crt
 src/geventhttpclient/tests/server.key
 src/geventhttpclient/tests/test_client.py
 src/geventhttpclient/tests/test_headers.py
-src/geventhttpclient/tests/test_http_host.py
 src/geventhttpclient/tests/test_httplib.py
 src/geventhttpclient/tests/test_httplib2.py
 src/geventhttpclient/tests/test_keep_alive.py
 src/geventhttpclient/tests/test_network_failures.py
 src/geventhttpclient/tests/test_no_module_ssl.py
 src/geventhttpclient/tests/test_parser.py
 src/geventhttpclient/tests/test_ssl.py
```

