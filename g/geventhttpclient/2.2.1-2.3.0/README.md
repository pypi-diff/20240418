# Comparing `tmp/geventhttpclient-2.2.1.tar.gz` & `tmp/geventhttpclient-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.2.1.tar", last modified: Tue Apr 16 16:41:03 2024, max compression
+gzip compressed data, was "geventhttpclient-2.3.0.tar", last modified: Thu Apr 18 13:28:16 2024, max compression
```

## Comparing `geventhttpclient-2.2.1.tar` & `geventhttpclient-2.3.0.tar`

### file list

```diff
@@ -1,52 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/ext/Python_compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/ext/_parser.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/LICENSE-MIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/include/
--rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/include/llhttp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/llhttp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/api.c
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/http.c
--rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/llhttp/src/llhttp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.241198 geventhttpclient-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.245198 geventhttpclient-2.2.1/src/geventhttpclient/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/connectionpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/src/geventhttpclient/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/oncert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/server.key
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_network_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_no_module_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-16 16:40:59.000000 geventhttpclient-2.2.1/src/geventhttpclient/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:41:03.249198 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 16:41:03.000000 geventhttpclient-2.2.1/src/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.020818 geventhttpclient-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-18 13:28:16.020818 geventhttpclient-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/ext/Python_compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/ext/_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/geventhttpclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/connectionpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10184 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21629 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/geventhttpclient/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/geventhttpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-18 13:28:16.000000 geventhttpclient-2.3.0/geventhttpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 13:28:16.000000 geventhttpclient-2.3.0/geventhttpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:28:16.000000 geventhttpclient-2.3.0/geventhttpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 13:28:16.000000 geventhttpclient-2.3.0/geventhttpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 13:28:16.000000 geventhttpclient-2.3.0/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/llhttp/LICENSE-MIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:28:16.016818 geventhttpclient-2.3.0/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/llhttp/src/llhttp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:28:16.020818 geventhttpclient-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 13:28:09.000000 geventhttpclient-2.3.0/setup.py
```

### Comparing `geventhttpclient-2.2.1/LICENSE-MIT` & `geventhttpclient-2.3.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/PKG-INFO` & `geventhttpclient-2.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.2.1
+Version: 2.3.0
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: This software is licensed under the MIT License.
         
         Copyright Antonin Amand <antonin.amand@gmail.com>, 2018.
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -64,184 +64,185 @@
 [![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
 [![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
 # geventhttpclient
 
-A high performance, concurrent HTTP client library for python using 
+A [high performance](https://github.com/geventhttpclient/geventhttpclient/blob/master/README.md#Benchmarks),
+concurrent HTTP client library for python using
 [gevent](http://gevent.org).
 
-`gevent.httplib` support was removed in [gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6
-), **geventhttpclient** now provides that missing functionality.
+`gevent.httplib` support for patching `http.client` was removed in
+[gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6),
+`geventhttpclient` now provides that missing functionality.
 
-**geventhttpclient** uses a fast [http parser](https://github.com/nodejs/llhttp),
+`geventhttpclient` uses a fast [http parser](https://github.com/nodejs/llhttp),
 written in C.
 
-**geventhttpclient** has been specifically designed for high concurrency,
+`geventhttpclient` has been specifically designed for high concurrency,
 streaming and support HTTP 1.1 persistent connections. More generally it is
 designed for efficiently pulling from REST APIs and streaming APIs
 like Twitter's.
 
-Safe SSL support is provided by default. **geventhttpclient** depends on
+Safe SSL support is provided by default. `geventhttpclient` depends on
 the certifi CA Bundle. This is the same CA Bundle which ships with the
 Requests codebase, and is derived from Mozilla Firefox's canonical set.
 
-As of version 2.1, only Python 3.9+ is fully supported (with prebuilt wheels).
-
-A simple example:
+Since version 2.3, `geventhttpclient` features a largely `requests`
+compatible interface. It covers basic HTTP usage including cookie
+management, form data encoding or decoding of compressed data,
+but otherwise isn't as feature rich as the original `requests`. For
+simple use-cases, it can serve as a drop-in replacement.
 
 ```python
-#!/usr/bin/python
+import geventhttpclient as requests
+requests.get("https://github.com").text
+requests.post("http://httpbingo.org/post", data="asdfasd").json()
+
+from geventhttpclient import Session
+s = Session()
+s.get("http://httpbingo.org/headers").json()
+s.get("https://github.com").content
+```
+
+This interface builds on top of the lower level `HTTPClient`.
 
+```python
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
-url = URL('http://gevent.org/')
-
-http = HTTPClient(url.host)
-
-# issue a get request
-response = http.get(url.request_uri)
-
-# read status_code
+url = URL("http://gevent.org/")
+client = HTTPClient(url.host)
+response = client.get(url.request_uri)
 response.status_code
-
-# read response body
 body = response.read()
-
-# close connections
-http.close()
+client.close()
 ```
 
 ## httplib compatibility and monkey patch
 
-**geventhttpclient.httplib** module contains classes for drop in
-replacement of httplib connection and response objects.
-If you use httplib directly you can replace the **httplib** imports
-by **geventhttpclient.httplib**.
+`geventhttpclient.httplib` module contains classes for drop in
+replacement of `http.client` connection and response objects.
+If you use http.client directly you can replace the `httplib` imports
+by `geventhttpclient.httplib`.
 
 ```python
-# from httplib import HTTPConnection
+# from http.client import HTTPConnection
 from geventhttpclient.httplib import HTTPConnection
 ```
 
-If you use **httplib2**, **urllib** or **urllib2**; you can patch **httplib** to
-use the wrappers from **geventhttpclient**.
-For **httplib2**, make sure you patch before you import or the *super*
-calls will fail.
+If you use `httplib2`, `urllib` or `urllib2`; you can patch `httplib` to
+use the wrappers from `geventhttpclient`. For `httplib2`, make sure you
+patch before you import or the `super()` calls will fail.
 
 ```python
 import geventhttpclient.httplib
 geventhttpclient.httplib.patch()
 
 import httplib2
 ```
 
 ## High Concurrency
 
-HTTPClient has connection pool built in and is greenlet safe by design.
-You can use the same instance among several greenlets.
+`HTTPClient` has a connection pool built in and is greenlet safe by design.
+You can use the same instance among several greenlets. It is the low
+level building block of this library.
 
 ```python
-#!/usr/bin/env python
-
 import gevent.pool
 import json
 
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
 
 # go to http://developers.facebook.com/tools/explorer and copy the access token
-TOKEN = '<go to http://developers.facebook.com/tools/explorer and copy the access token>'
+TOKEN = "<MY_DEV_TOKEN>"
 
-url = URL('https://graph.facebook.com/me/friends')
-url['access_token'] = TOKEN
+url = URL("https://graph.facebook.com/me/friends", params={"access_token": TOKEN})
 
 # setting the concurrency to 10 allow to create 10 connections and
 # reuse them.
-http = HTTPClient.from_url(url, concurrency=10)
+client = HTTPClient.from_url(url, concurrency=10)
 
-response = http.get(url.request_uri)
+response = client.get(url.request_uri)
 assert response.status_code == 200
 
 # response comply to the read protocol. It passes the stream to
 # the json parser as it's being read.
-data = json.load(response)['data']
+data = json.load(response)["data"]
 
-def print_friend_username(http, friend_id):
-    friend_url = URL('/' + str(friend_id))
-    friend_url['access_token'] = TOKEN
+def print_friend_username(client, friend_id):
+    friend_url = URL(f"/{friend_id}", params={"access_token": TOKEN})
     # the greenlet will block until a connection is available
-    response = http.get(friend_url.request_uri)
+    response = client.get(friend_url.request_uri)
     assert response.status_code == 200
     friend = json.load(response)
-    if 'username' in friend:
-        print('%s: %s' % (friend['username'], friend['name']))
+    if "username" in friend:
+        print(f"{friend['username']}: {friend['name']}")
     else:
-        print('%s has no username.' % friend['name'])
+        print(f"{friend['name']} has no username.")
 
 # allow to run 20 greenlet at a time, this is more than concurrency
 # of the http client but isn't a problem since the client has its own
 # connection pool.
 pool = gevent.pool.Pool(20)
 for item in data:
-    friend_id = item['id']
-    pool.spawn(print_friend_username, http, friend_id)
+    friend_id = item["id"]
+    pool.spawn(print_friend_username, client, friend_id)
 
 pool.join()
-http.close()
+client.close()
 ```
 
 ## Streaming
 
-**geventhttpclient** supports streaming.
-Response objects have a read(N) and readline() method that read the stream
-incrementally.
-See *src/examples/twitter_streaming.py* for pulling twitter stream API.
+`geventhttpclient` supports streaming. Response objects have a `read(n)` and
+`readline()` method that read the stream incrementally.
+See [examples/twitter_streaming.py](https://github.com/geventhttpclient/geventhttpclient/blob/master/examples/twitter_streaming.py)
+for pulling twitter stream API.
 
 Here is an example on how to download a big file chunk by chunk to save memory:
 
 ```python
-#!/usr/bin/env python
-
 from geventhttpclient import HTTPClient, URL
 
-url = URL('http://127.0.0.1:80/100.dat')
-http = HTTPClient.from_url(url)
-response = http.get(url.query_string)
+url = URL("http://127.0.0.1:80/100.dat")
+client = HTTPClient.from_url(url)
+response = client.get(url.query_string)
 assert response.status_code == 200
 
 CHUNK_SIZE = 1024 * 16 # 16KB
-with open('/tmp/100.dat', 'w') as f:
+with open("/tmp/100.dat", "w") as f:
     data = response.read(CHUNK_SIZE)
     while data:
         f.write(data)
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
-The benchmark does 10000 get requests against a local nginx server in the default 
+The benchmark runs 10000 `GET` requests against a local nginx server in the default
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
 second for a couple of popular clients is given in the table below. Please read
 [benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
-for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
+for more details. Also note, [HTTPX](https://www.python-httpx.org/) is better be
+used with `asyncio`, not `gevent`.
 
 | HTTP Client        | RPS    |
 |--------------------|--------|
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
 
 ## License
 
-This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
-Previous versions of geventhttpclient used http_parser.c, which in turn 
-was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
-Joyent, Inc., and other Node contributors. For more information, see 
-http://github.com/joyent/http-parser 
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT).
+Previous versions of geventhttpclient used `http_parser.c`, which in turn was
+based on `http/ngx_http_parse.c` from [NGINX](https://nginx.org), copyright Igor
+Sysoev, Joyent, Inc., and other Node contributors. For more information, see
+http://github.com/joyent/http-parser
```

### Comparing `geventhttpclient-2.2.1/README.md` & `geventhttpclient-2.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,185 @@
 [![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
 [![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
 # geventhttpclient
 
-A high performance, concurrent HTTP client library for python using 
+A [high performance](https://github.com/geventhttpclient/geventhttpclient/blob/master/README.md#Benchmarks),
+concurrent HTTP client library for python using
 [gevent](http://gevent.org).
 
-`gevent.httplib` support was removed in [gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6
-), **geventhttpclient** now provides that missing functionality.
+`gevent.httplib` support for patching `http.client` was removed in
+[gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6),
+`geventhttpclient` now provides that missing functionality.
 
-**geventhttpclient** uses a fast [http parser](https://github.com/nodejs/llhttp),
+`geventhttpclient` uses a fast [http parser](https://github.com/nodejs/llhttp),
 written in C.
 
-**geventhttpclient** has been specifically designed for high concurrency,
+`geventhttpclient` has been specifically designed for high concurrency,
 streaming and support HTTP 1.1 persistent connections. More generally it is
 designed for efficiently pulling from REST APIs and streaming APIs
 like Twitter's.
 
-Safe SSL support is provided by default. **geventhttpclient** depends on
+Safe SSL support is provided by default. `geventhttpclient` depends on
 the certifi CA Bundle. This is the same CA Bundle which ships with the
 Requests codebase, and is derived from Mozilla Firefox's canonical set.
 
-As of version 2.1, only Python 3.9+ is fully supported (with prebuilt wheels).
-
-A simple example:
+Since version 2.3, `geventhttpclient` features a largely `requests`
+compatible interface. It covers basic HTTP usage including cookie
+management, form data encoding or decoding of compressed data,
+but otherwise isn't as feature rich as the original `requests`. For
+simple use-cases, it can serve as a drop-in replacement.
 
 ```python
-#!/usr/bin/python
+import geventhttpclient as requests
+requests.get("https://github.com").text
+requests.post("http://httpbingo.org/post", data="asdfasd").json()
+
+from geventhttpclient import Session
+s = Session()
+s.get("http://httpbingo.org/headers").json()
+s.get("https://github.com").content
+```
+
+This interface builds on top of the lower level `HTTPClient`.
 
+```python
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
-url = URL('http://gevent.org/')
-
-http = HTTPClient(url.host)
-
-# issue a get request
-response = http.get(url.request_uri)
-
-# read status_code
+url = URL("http://gevent.org/")
+client = HTTPClient(url.host)
+response = client.get(url.request_uri)
 response.status_code
-
-# read response body
 body = response.read()
-
-# close connections
-http.close()
+client.close()
 ```
 
 ## httplib compatibility and monkey patch
 
-**geventhttpclient.httplib** module contains classes for drop in
-replacement of httplib connection and response objects.
-If you use httplib directly you can replace the **httplib** imports
-by **geventhttpclient.httplib**.
+`geventhttpclient.httplib` module contains classes for drop in
+replacement of `http.client` connection and response objects.
+If you use http.client directly you can replace the `httplib` imports
+by `geventhttpclient.httplib`.
 
 ```python
-# from httplib import HTTPConnection
+# from http.client import HTTPConnection
 from geventhttpclient.httplib import HTTPConnection
 ```
 
-If you use **httplib2**, **urllib** or **urllib2**; you can patch **httplib** to
-use the wrappers from **geventhttpclient**.
-For **httplib2**, make sure you patch before you import or the *super*
-calls will fail.
+If you use `httplib2`, `urllib` or `urllib2`; you can patch `httplib` to
+use the wrappers from `geventhttpclient`. For `httplib2`, make sure you
+patch before you import or the `super()` calls will fail.
 
 ```python
 import geventhttpclient.httplib
 geventhttpclient.httplib.patch()
 
 import httplib2
 ```
 
 ## High Concurrency
 
-HTTPClient has connection pool built in and is greenlet safe by design.
-You can use the same instance among several greenlets.
+`HTTPClient` has a connection pool built in and is greenlet safe by design.
+You can use the same instance among several greenlets. It is the low
+level building block of this library.
 
 ```python
-#!/usr/bin/env python
-
 import gevent.pool
 import json
 
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
 
 # go to http://developers.facebook.com/tools/explorer and copy the access token
-TOKEN = '<go to http://developers.facebook.com/tools/explorer and copy the access token>'
+TOKEN = "<MY_DEV_TOKEN>"
 
-url = URL('https://graph.facebook.com/me/friends')
-url['access_token'] = TOKEN
+url = URL("https://graph.facebook.com/me/friends", params={"access_token": TOKEN})
 
 # setting the concurrency to 10 allow to create 10 connections and
 # reuse them.
-http = HTTPClient.from_url(url, concurrency=10)
+client = HTTPClient.from_url(url, concurrency=10)
 
-response = http.get(url.request_uri)
+response = client.get(url.request_uri)
 assert response.status_code == 200
 
 # response comply to the read protocol. It passes the stream to
 # the json parser as it's being read.
-data = json.load(response)['data']
+data = json.load(response)["data"]
 
-def print_friend_username(http, friend_id):
-    friend_url = URL('/' + str(friend_id))
-    friend_url['access_token'] = TOKEN
+def print_friend_username(client, friend_id):
+    friend_url = URL(f"/{friend_id}", params={"access_token": TOKEN})
     # the greenlet will block until a connection is available
-    response = http.get(friend_url.request_uri)
+    response = client.get(friend_url.request_uri)
     assert response.status_code == 200
     friend = json.load(response)
-    if 'username' in friend:
-        print('%s: %s' % (friend['username'], friend['name']))
+    if "username" in friend:
+        print(f"{friend['username']}: {friend['name']}")
     else:
-        print('%s has no username.' % friend['name'])
+        print(f"{friend['name']} has no username.")
 
 # allow to run 20 greenlet at a time, this is more than concurrency
 # of the http client but isn't a problem since the client has its own
 # connection pool.
 pool = gevent.pool.Pool(20)
 for item in data:
-    friend_id = item['id']
-    pool.spawn(print_friend_username, http, friend_id)
+    friend_id = item["id"]
+    pool.spawn(print_friend_username, client, friend_id)
 
 pool.join()
-http.close()
+client.close()
 ```
 
 ## Streaming
 
-**geventhttpclient** supports streaming.
-Response objects have a read(N) and readline() method that read the stream
-incrementally.
-See *src/examples/twitter_streaming.py* for pulling twitter stream API.
+`geventhttpclient` supports streaming. Response objects have a `read(n)` and
+`readline()` method that read the stream incrementally.
+See [examples/twitter_streaming.py](https://github.com/geventhttpclient/geventhttpclient/blob/master/examples/twitter_streaming.py)
+for pulling twitter stream API.
 
 Here is an example on how to download a big file chunk by chunk to save memory:
 
 ```python
-#!/usr/bin/env python
-
 from geventhttpclient import HTTPClient, URL
 
-url = URL('http://127.0.0.1:80/100.dat')
-http = HTTPClient.from_url(url)
-response = http.get(url.query_string)
+url = URL("http://127.0.0.1:80/100.dat")
+client = HTTPClient.from_url(url)
+response = client.get(url.query_string)
 assert response.status_code == 200
 
 CHUNK_SIZE = 1024 * 16 # 16KB
-with open('/tmp/100.dat', 'w') as f:
+with open("/tmp/100.dat", "w") as f:
     data = response.read(CHUNK_SIZE)
     while data:
         f.write(data)
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
-The benchmark does 10000 get requests against a local nginx server in the default 
+The benchmark runs 10000 `GET` requests against a local nginx server in the default
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
 second for a couple of popular clients is given in the table below. Please read
 [benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
-for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
+for more details. Also note, [HTTPX](https://www.python-httpx.org/) is better be
+used with `asyncio`, not `gevent`.
 
 | HTTP Client        | RPS    |
 |--------------------|--------|
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
 
 ## License
 
-This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
-Previous versions of geventhttpclient used http_parser.c, which in turn 
-was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
-Joyent, Inc., and other Node contributors. For more information, see 
-http://github.com/joyent/http-parser 
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT).
+Previous versions of geventhttpclient used `http_parser.c`, which in turn was
+based on `http/ngx_http_parse.c` from [NGINX](https://nginx.org), copyright Igor
+Sysoev, Joyent, Inc., and other Node contributors. For more information, see
+http://github.com/joyent/http-parser
```

### Comparing `geventhttpclient-2.2.1/ext/_parser.c` & `geventhttpclient-2.3.0/ext/_parser.c`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     const char* reason;
     enum py_parser_should_keep_alive should_keep_alive;
 } PyHTTPResponseParser;
 
 static int on_message_begin(llhttp_t* parser)
 {
     int fail = 0;
-    PyObject* self = (PyObject*)parser->data;
-    if (PyObject_HasAttrString(self, "_on_message_begin")) {
-        PyObject* callable = PyObject_GetAttrString(self, "_on_message_begin");
+    PyHTTPResponseParser *self = (PyHTTPResponseParser*) parser->data;
+    PyObject* callable = PyObject_GetAttrString((PyObject*)self, "_on_message_begin");
+    if (callable) {
         PyObject* result = PyObject_CallObject(callable, NULL);
         PyObject* exception = PyErr_Occurred();
         if (exception != NULL) {
             fail = -1;
         } else {
             if (PyObject_IsTrue(result))
                 fail = -1;
@@ -41,16 +41,16 @@
 }
 
 static int on_message_complete(llhttp_t* parser)
 {
     int fail = 0;
     PyHTTPResponseParser *self = (PyHTTPResponseParser*) parser->data;
     self->should_keep_alive = llhttp_should_keep_alive(parser) ? KA_TRUE : KA_FALSE;
-    if (PyObject_HasAttrString(self, "_on_message_complete")) {
-        PyObject* callable = PyObject_GetAttrString(self, "_on_message_complete");
+    PyObject* callable = PyObject_GetAttrString((PyObject*)self, "_on_message_complete");
+    if (callable) {
         PyObject* result = PyObject_CallObject(callable, NULL);
         PyObject* exception = PyErr_Occurred();
         if (exception != NULL) {
             fail = -1;
         } else {
             if (PyObject_IsTrue(result))
                 fail = -1;
@@ -61,17 +61,17 @@
     return fail;
 }
 
 static int on_headers_complete(llhttp_t* parser)
 {
     /* 1 => skip body, 2 => upgrade, 0 => continue, -1 => error */
     int skip_body = 0;
-    PyObject* self = (PyObject*)parser->data;
-    if (PyObject_HasAttrString(self, "_on_headers_complete")) {
-        PyObject* callable = PyObject_GetAttrString(self, "_on_headers_complete");
+    PyHTTPResponseParser *self = (PyHTTPResponseParser*) parser->data;
+    PyObject* callable = PyObject_GetAttrString((PyObject*)self, "_on_headers_complete");
+    if (callable) {
         PyObject* result = PyObject_CallObject(callable, NULL);
         PyObject* exception = PyErr_Occurred();
         if (exception != NULL) {
             skip_body = -1;
         } else if (PyObject_IsTrue(result)) {
             skip_body = 1;
         }
@@ -80,31 +80,31 @@
     }
     return skip_body;
 }
 
 static int on_http_data_cb(llhttp_t* parser, const char *at, size_t length, const char * python_cb)
 {
     int fail = 0;
-    PyObject* self = (PyObject*)parser->data;
-    if (PyObject_HasAttrString(self, python_cb)) {
-        PyObject* callable = PyObject_GetAttrString(self, python_cb);
+    PyHTTPResponseParser *self = (PyHTTPResponseParser*) parser->data;
+    PyObject* callable = PyObject_GetAttrString((PyObject*)self, python_cb);
+    if (callable) {
         PyObject* args = Py_BuildValue("(s#)", at, length);
         PyObject* result = PyObject_CallObject(callable, args);
         PyObject* exception = PyErr_Occurred();
         if (exception != NULL) {
             fail = -1;
         } else {
             if (PyObject_IsTrue(result))
                 fail = -1;
         }
         Py_XDECREF(result);
         Py_DECREF(callable);
         Py_DECREF(args);
     }
-    return fail;    
+    return fail;
 }
 
 static int on_status(llhttp_t* parser, const char *at, size_t length)
 {
     return on_http_data_cb(parser, at, length, "_on_status");
 }
 
@@ -117,17 +117,17 @@
 {
     return on_http_data_cb(parser, at, length, "_on_header_value");
 }
 
 static int on_body(llhttp_t* parser, const char *at, size_t length)
 {
     int fail = 0;
-    PyObject* self = (PyObject*)parser->data;
-    if (PyObject_HasAttrString(self, "_on_body")) {
-        PyObject* callable = PyObject_GetAttrString(self, "_on_body");
+    PyHTTPResponseParser *self = (PyHTTPResponseParser*) parser->data;
+    PyObject* callable = PyObject_GetAttrString((PyObject*)self, "_on_body");
+    if (callable) {
         PyObject* bytearray = PyByteArray_FromStringAndSize(at, length);
         PyObject* result = PyObject_CallFunctionObjArgs(
             callable, bytearray, NULL);
         PyObject* exception = PyErr_Occurred();
         if (exception != NULL) {
             fail = -1;
         } else {
@@ -265,15 +265,15 @@
 
 static PyObject*
 PyHTTPResponseParser_should_keep_alive(PyHTTPResponseParser* self)
 {
     if (self->error != HPE_OK) {
         Py_RETURN_FALSE;
     }
-    int should_keep_alive;
+    int should_keep_alive = 0;
     switch (self->should_keep_alive) {
         case KA_INCOMPLETE:
             should_keep_alive = llhttp_should_keep_alive(self->parser);
             break;
         case KA_FALSE:
             should_keep_alive = 0;
             break;
@@ -301,15 +301,15 @@
         "Get http version"},
     {"get_remaining_content_length",
         (PyCFunction)PyHTTPResponseParser_get_remaining_content_length,
         METH_NOARGS,
         "Get remaining content length to read"},
     {"should_keep_alive", (PyCFunction)PyHTTPResponseParser_should_keep_alive,
         METH_NOARGS,
-        "Tell wether the connection should stay connected (HTTP 1.1)"},
+        "Tell whether the connection should stay connected (HTTP 1.1)"},
     {"parser_failed", (PyCFunction)PyHTTPResponseParser_parser_failed,
         METH_NOARGS,
         "Tell if parser have failed."},
     {NULL}  /* Sentinel */
 };
 
 static PyTypeObject HTTPParserType = {
```

### Comparing `geventhttpclient-2.2.1/llhttp/LICENSE-MIT` & `geventhttpclient-2.3.0/llhttp/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/llhttp/include/llhttp.h` & `geventhttpclient-2.3.0/llhttp/include/llhttp.h`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/llhttp/src/api.c` & `geventhttpclient-2.3.0/llhttp/src/api.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/llhttp/src/http.c` & `geventhttpclient-2.3.0/llhttp/src/http.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/llhttp/src/llhttp.c` & `geventhttpclient-2.3.0/llhttp/src/llhttp.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/pyproject.toml` & `geventhttpclient-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "geventhttpclient"
-version = "2.2.1" # dont forget to update version __init__.py as well
+version = "2.3.0" # dont forget to update version __init__.py as well
 description = "HTTP client library for gevent"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE-MIT"}
 keywords = ["http", "gevent", "client"]
 authors = [{name = "Antonin Amand", email = "antonin.amand@gmail.com"}]
 classifiers = [
@@ -54,55 +54,64 @@
 download = "https://pypi.org/project/geventhttpclient/#files"
 
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["src"]
-exclude = ["geventhttpclient.tests*"]
+where = [""]
+include = ["geventhttpclient"]
+exclude = ["*.tests", "*.tests.*", "tests.*", "tests"]
 
 [tool.setuptools.package-data]
-"*" = ["LICENSE.txt", "README.md", "release.md", "LICENSE-MIT"]
+"*" = ["README.md", "release.md", "LICENSE-MIT"]
 
 [tool.setuptools.exclude-package-data]
 "*" = ["__pycache__", "*.pyc", "*.pyo"]
 
 
 [tool.pytest.ini_options]
 markers = [
     "network: tests which require internet access"
 ]
 
 
 [tool.tox]
-envlist = "py{39,310,311,312}"
-
-[tool.tox.testenv]
-allowlist_externals = [
-    "rm",
-    "find",
-    "pytest"
-]
-commands = [
-    "rm -rf build",
-    "find . -name '*.pyc' -delete",
-    "python setup.py clean",
-    "python setup.py build_ext --inplace",
-    "pip install -r requirements-dev.txt",
-    "pytest --fulltrace src/geventhttpclient/tests"
-]
+legacy_tox_ini = """
+[tox]
+envlist = py{39,310,311,312}
+
+[testenv]
+deps =
+    pip
+    pytest
+    build
+allowlist_externals =
+    rm
+    find
+commands =
+    rm -rf build
+    # find errors for windows
+    # find . -name '*.pyc' -delete
+    python -m build
+    pip install -r requirements-dev.txt
+    pip install -e.
+    pytest tests
+"""
 
 
 [tool.ruff]
 fix = false
 line-length = 100
 target-version = "py311"
 lint.extend-select = ["UP"]
 lint.ignore = ["F821", "UP038", "E402"]
 
 [tool.ruff.lint.isort]
-known-first-party = ["geventhttpclient"]
+known-first-party = ["geventhttpclient", "tests"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "test_no_module_ssl.py" = ["F401"]
+
+[tool.codespell]
+ignore-regex = ".*codespell-ignore$"
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/client.py` & `geventhttpclient-2.3.0/geventhttpclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,17 +293,17 @@
 
 
 class HTTPClientPool:
     """Factory for maintaining a bunch of clients, one per host:port"""
 
     # TODO: Add some housekeeping and cleanup logic
 
-    def __init__(self, **kwargs):
-        self.clients = dict()
-        self.client_args = kwargs
+    def __init__(self, **kw):
+        self.clients = {}
+        self.client_args = kw
 
     def get_client(self, url):
         if not isinstance(url, URL):
             url = URL(url)
         client_key = url.host, url.port
         try:
             return self.clients[client_key]
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/connectionpool.py` & `geventhttpclient-2.3.0/geventhttpclient/connectionpool.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     import certifi
 
     _CA_CERTS = certifi.where()
 
 _DEFAULT_CIPHERS = (
     "ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:ECDH+HIGH:"
     "DH+HIGH:ECDH+3DES:DH+3DES:RSA+AESGCM:RSA+AES:RSA+HIGH:RSA+3DES:ECDH+RC4:"
-    "DH+RC4:RSA+RC4:!aNULL:!eNULL:!MD5"
+    "DH+RC4:RSA+RC4:!aNULL:!eNULL:!MD5"  # codespell-ignore
 )
 
 
 DEFAULT_CONNECTION_TIMEOUT = 5.0
 DEFAULT_NETWORK_TIMEOUT = 5.0
 
 IGNORED = object()
@@ -59,15 +59,15 @@
 
         self.connection_timeout = connection_timeout
         self.network_timeout = network_timeout
         self.size = size
         self.disable_ipv6 = disable_ipv6
 
     def _resolve(self):
-        """resolve (dns) socket informations needed to connect it."""
+        """resolve (dns) socket information needed to connect it."""
         family = 0
         if self.disable_ipv6:
             family = gevent.socket.AF_INET
         info = gevent.socket.getaddrinfo(
             self._connection_host,
             self._connection_port,
             family,
@@ -80,15 +80,15 @@
     def close(self):
         self._closed = True
         while not self._socket_queue.empty():
             try:
                 sock = self._socket_queue.get(block=False)
                 try:
                     sock.close()
-                except:
+                except:  # noqa
                     pass
             except gevent.queue.Empty:
                 pass
 
     def _create_tcp_socket(self, family, socktype, protocol):
         """tcp socket factory."""
         sock = gevent.socket.socket(family, socktype, protocol)
@@ -114,15 +114,15 @@
                 self.after_connect(sock)
                 sock.settimeout(self.network_timeout)
                 return sock
             except OSError as e:
                 sock.close()
                 if not first_error:
                     first_error = e
-            except:
+            except:  # noqa
                 sock.close()
                 raise
 
         if first_error:
             raise first_error
         else:
             raise RuntimeError(f"Cannot resolve {self._host}:{self._port}")
@@ -155,34 +155,34 @@
         if self._closed:
             raise RuntimeError("connection pool closed")
         try:
             return self._socket_queue.get(block=False)
         except gevent.queue.Empty:
             try:
                 return self._create_socket()
-            except:
+            except:  # noqa
                 self._semaphore.release()
                 raise
 
     def return_socket(self, sock):
         """return a socket to the pool."""
         if self._closed:
             try:
                 sock.close()
-            except:
+            except:  # noqa
                 pass
             return
         self._socket_queue.put(sock)
         self._semaphore.release()
 
     def release_socket(self, sock):
         """call when the socket is no more usable."""
         try:
             sock.close()
-        except:
+        except:  # noqa
             pass
         if not self._closed:
             self._semaphore.release()
 
 
 def init_ssl_context(ssl_context_factory, ca_certs, check_hostname=True):
     try:
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/header.py` & `geventhttpclient-2.3.0/geventhttpclient/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,32 @@
         """Iterate over all header lines, including duplicate ones."""
         for field, vals in _dict_items(self):
             if isinstance(vals, tuple):
                 yield vals
             else:
                 yield from vals
 
-    # Backwards compatibility for httplib
+    # Compatibility with http.client
     getheaders = getlist
     getallmatchingheaders = getlist
-    iget = getlist
 
-    # deprecated
-    iteroriginal = items
+    def iteroriginal(self):
+        import warnings
+
+        warnings.warn(
+            "This is deprecated and will be removed in version v2.3.0. "
+            "Use Headers.items() instead.",
+            DeprecationWarning,
+            2,
+        )
+        return self.items()
+
+    def iget(self, field):
+        import warnings
+
+        warnings.warn(
+            "This is deprecated and will be removed in version v2.3.0. "
+            "Use Headers.getlist() instead.",
+            DeprecationWarning,
+            2,
+        )
+        return self.getlist(field)
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/httplib.py` & `geventhttpclient-2.3.0/geventhttpclient/httplib.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/httplib2.py` & `geventhttpclient-2.3.0/geventhttpclient/httplib2.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/response.py` & `geventhttpclient-2.3.0/geventhttpclient/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     def items(self):
         return self._headers_index.items()
 
     headers = property(items)
 
     def info(self):
+        # compatibility with http.client
         return self._headers_index
 
     def __contains__(self, key):
         return key in self._headers_index
 
     def should_close(self):
         """return if we should close the connection.
@@ -145,15 +146,15 @@
         self._read_headers()
 
     def release(self):
         try:
             if self._sock is not None and self.should_close():
                 try:
                     self._sock.close()
-                except:
+                except:  # noqa
                     pass
         finally:
             self._sock = None
 
     def __del__(self):
         self.release()
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/url.py` & `geventhttpclient-2.3.0/geventhttpclient/url.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient/useragent.py` & `geventhttpclient-2.3.0/geventhttpclient/useragent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import errno
+import json as jsonlib
 import os
 import socket
 import ssl
 import sys
 import zlib
 from urllib.parse import urlencode
 
@@ -12,38 +13,38 @@
 from urllib3.fields import RequestField
 
 from geventhttpclient.client import HTTPClient, HTTPClientPool
 from geventhttpclient.url import URL, to_key_val_list
 
 
 class ConnectionError(Exception):
-    def __init__(self, url, *args, **kwargs):
+    def __init__(self, url, *args, **kw):
         self.url = url
-        self.__dict__.update(kwargs)
+        self.__dict__.update(kw)
         if args and isinstance(args[0], str):
             self.text = args[0] + ": " + str(args[1:])
         else:
             self.text = str(args[0]) if len(args) == 1 else ""
-        if kwargs:
+        if kw:
             self.text += ", " if self.text else ""
-            self.kwargs_text = ", ".join(f"{key}={val}" for key, val in kwargs.items())
-            self.text += self.kwargs_text
+            self.kw_text = ", ".join(f"{key}={val}" for key, val in kw.items())
+            self.text += self.kw_text
         else:
             self.text = ""
 
     def __str__(self):
         if self.text:
             return f"URL {self.url}: {self.text}"
         else:
             return f"URL {self.url}"
 
     def __repr__(self):
         repr_str = super().__repr__()
-        if self.kwargs_text:
-            return repr_str.replace(")", "".join([", ", self.kwargs_text, ")"]))
+        if self.kw_text:
+            return repr_str.replace(")", "".join([", ", self.kw_text, ")"]))
         return repr_str
 
 
 class RetriesExceeded(ConnectionError):
     pass
 
 
@@ -52,33 +53,41 @@
 
 
 class EmptyResponse(ConnectionError):
     pass
 
 
 class CompatRequest:
-    """urllib / cookielib compatible request class.
+    """urllib.request.Request compatible request class.
     See also: http://docs.python.org/library/cookielib.html
     """
 
+    # TODO: Since we dropped all py2 dependencies, we could derive directly from
+    #       urllib.request.Request and only deviate when required. Not rebuild
+    #       the whole thing.
+
     def __init__(self, url, method="GET", headers=None, payload=None, params=None):
-        self.params = params
-        self.set_url(url)
+        self.set_url(url, params=params)
         self.original_host = self.url_split.host
-        self.method = method
+        self.method = method.upper()
         self.headers = headers
         self.payload = payload
 
-    def set_url(self, url):
+    @property
+    def full_url(self):
+        # new in python3.x
+        return self.url
+
+    def set_url(self, url, params=None):
         if isinstance(url, URL):
             self.url = str(url)
             self.url_split = url
         else:
             self.url = url
-            self.url_split = URL(self.url, params=self.params)
+            self.url_split = URL(self.url, params=params)
 
     def get_full_url(self):
         return self.url
 
     def get_host(self):
         return self.url_split.host
 
@@ -123,38 +132,49 @@
         self.set_url(self.url_split.redirect(location))
         if code in (302, 303):
             self._drop_payload()
         self._drop_cookies()
 
 
 class CompatResponse:
-    """Adapter for urllib responses with some extensions"""
+    """Adapter for urllib3-style responses."""
 
     __slots__ = "headers", "_response", "_request", "_sent_request", "_cached_content"
 
     def __init__(self, ghc_response, request=None, sent_request=None):
         self._response = ghc_response
         self._request = request
         self._sent_request = sent_request
         self.headers = self._response._headers_index
 
-    @property
-    def status(self):
-        """The returned http status"""
-        # TODO: Should be a readable string
-        return str(self.status_code)
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args):
+        self.release()
 
     @property
     def status_code(self):
-        """The http status code as plain integer"""
+        """HTTP status code as plain integer"""
         return self._response.get_code()
 
-    @property
-    def stream(self):
-        return self._response
+    def __len__(self):
+        """The content lengths as declared from the headers"""
+        return self._response.length
+
+    def info(self):
+        """Adaption to http.client."""
+        return self.headers
+
+    def __nonzero__(self):
+        """If we have an empty response body, we still don't want to evaluate as false"""
+        return True
+
+    def __iter__(self):
+        return iter(self._response)
 
     def read(self, n=None):
         """Read n bytes from the response body"""
         return self._response.read(n)
 
     def readline(self):
         return self._response.readline()
@@ -183,55 +203,79 @@
             return self._cached_content
         except AttributeError:
             self._cached_content = self._content()
             return self._cached_content
 
     def _content(self):
         try:
-            content_type = self.headers.getheaders("content-encoding")[0].lower()
+            content_encoding = self.headers.getheaders("content-encoding")[0].lower()
         except IndexError:
             # No content-encoding header set
-            content_type = "identity"
+            content_encoding = "identity"
 
-        if content_type == "gzip":
+        if content_encoding == "gzip":
             ret = self.unzipped(gzip=True)
-        elif content_type == "deflate":
+        elif content_encoding == "deflate":
             ret = self.unzipped(gzip=False)
-        elif content_type == "identity":
+        elif content_encoding == "identity":
             ret = self._response.read()
-        elif content_type == "br":
+        elif content_encoding == "br":
             ret = self.unzipped(gzip=False, br=True)
-        elif content_type == "compress":
-            raise ValueError(f"Compression type not supported: {content_type}")
+        elif content_encoding == "compress":
+            raise ValueError(f"Compression type not supported: {content_encoding}")
         else:
-            raise ValueError(f"Unknown content encoding: {content_type}")
+            raise ValueError(f"Unknown content encoding: {content_encoding}")
 
         self.release()
         return ret
 
-    def __len__(self):
-        """The content lengths as should be returned from the headers"""
+    @property
+    def text(self):
+        if not self.content:
+            return ""
+
         try:
-            return int(self.headers.getheaders("content-length")[0])
-        except (IndexError, ValueError):
-            return len(self.content)
+            content_type = self.headers.getheaders("content-type")[0].lower()
+        except IndexError:
+            # No content-encoding header set, let's hope for the best
+            return self.content.decode()
 
-    def __nonzero__(self):
-        """If we have an empty response body, we still don't want to evaluate as false"""
-        return True
+        if content_type.startswith("text"):
+            codec = "utf-8"  # default
+            if "charset" in content_type:
+                try:
+                    codec = content_type.split("charset=", 1)[1][:10]
+                except IndexError:
+                    pass
+            return self.content.decode(codec)
+        return self.content
 
-    def info(self):
-        """Adaption to cookielib: Alias for headers"""
-        return self.headers
+    def json(self):
+        return jsonlib.load(self)
 
-    def __enter__(self):
-        return self
+    # the stuff only for urllib3
 
-    def __exit__(self, *args):
-        self.release()
+    @property
+    def status(self):
+        """HTTP status for urllib3"""
+        return str(self.status_code)
+
+    @property
+    def data(self):
+        """Content for urllib3"""
+        return self.content
+
+    @property
+    def stream(self):
+        """Readable stream for urllib3"""
+        return self._response
+
+    def isclosed(self):
+        """Closed status for urllib3"""
+        return self._response.message_complete
 
 
 class UserAgent:
     response_type = CompatResponse
     request_type = CompatRequest
     valid_response_codes = frozenset([200, 206, 301, 302, 303, 307])
     redirect_resonse_codes = frozenset([301, 302, 303, 307])
@@ -239,150 +283,39 @@
     def __init__(
         self,
         max_redirects=3,
         max_retries=3,
         retry_delay=0,
         cookiejar=None,
         headers=None,
-        **kwargs,
+        **kw,
     ):
         self.max_redirects = int(max_redirects)
         self.max_retries = int(max_retries)
         self.retry_delay = retry_delay
         self.default_headers = HTTPClient.DEFAULT_HEADERS.copy()
         if headers:
             self.default_headers.update(headers)
         self.cookiejar = cookiejar
-        self.clientpool = HTTPClientPool(**kwargs)
+        self.clientpool = HTTPClientPool(**kw)
 
     def close(self):
         self.clientpool.close()
 
-    def __del__(self):
-        self.close()
-
-    def _make_request(self, url, method="GET", headers=None, payload=None, params=None, files=None):
-        req_headers = self.default_headers.copy()
-        if headers:
-            req_headers.update(headers)
-        if payload or files:
-            # Adjust headers depending on payload content
-            content_type = req_headers.get("content-type", None)
-            if files:
-                (body, content_type) = self._encode_files(files, payload)
-                payload = body
-                req_headers["content-type"] = content_type
-            if isinstance(payload, dict):
-                if not content_type:
-                    req_headers["content-type"] = "application/x-www-form-urlencoded; charset=utf-8"
-                payload = urlencode(payload)
-            elif not content_type and isinstance(payload, str):
-                req_headers["content-type"] = "text/plain; charset=utf-8"
-            elif not content_type:
-                req_headers["content-type"] = "application/octet-stream"
-        return self.request_type(
-            url, method=method, headers=req_headers, payload=payload, params=params
-        )
+    def __enter__(self):
+        return self
 
-    def _urlopen(self, request):
-        client = self.clientpool.get_client(request.url_split)
-        resp = client.request(
-            request.method,
-            request.url_split.request_uri,
-            body=request.payload,
-            headers=request.headers,
-        )
-        return self.response_type(resp, request=request, sent_request=resp._sent_request)
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
     def _verify_status(self, status_code, url=None):
         """Hook for subclassing"""
         if status_code not in self.valid_response_codes:
             raise BadStatusCode(url, code=status_code)
 
-    def _encode_files(self, files, data):
-        """
-        Method taken from models in requests library , usage is the same. Only difference is that you can add custom
-        boundary in 5-tuple version.
-
-        Build the body for a multipart/form-data request.
-
-        Will successfully encode files when passed as a dict or a list of
-        tuples. Order is retained if data is a list of tuples but arbitrary
-        if parameters are supplied as a dict.
-
-        The tuples may be
-        2-tuples (filename, fileobj),
-        3-tuples (filename, fileobj, contentype),
-        4-tuples (filename, fileobj, contentype, custom_headers) or
-        5-tuples (filename, fileobj, contentype, custom_headers, custom boundary).
-
-        example:
-        files = {'file': ('report.xls', body, 'application/vnd.ms-excel', {'Expires': '0'}, 'custom_boundary')}
-
-        """
-
-        if not files:
-            raise ValueError("Files must be provided.")
-        elif isinstance(data, (str, bytes)):
-            raise ValueError("Data must not be a string.")
-
-        new_fields = []
-        fields = to_key_val_list(data or {})
-        files = to_key_val_list(files or {})
-
-        for field, val in fields:
-            if isinstance(val, (str, bytes)) or not hasattr(val, "__iter__"):
-                val = [val]
-            for v in val:
-                if v is not None:
-                    if not isinstance(v, bytes):
-                        v = str(v)
-
-                    new_fields.append(
-                        (
-                            field.decode("utf-8") if isinstance(field, bytes) else field,
-                            v.encode("utf-8") if isinstance(v, str) else v,
-                        )
-                    )
-
-        for k, v in files:
-            # support for explicit filename
-            ft = None
-            fh = None
-            boundary = None
-            if isinstance(v, (tuple, list)):
-                if len(v) == 2:
-                    fn, fp = v
-                elif len(v) == 3:
-                    fn, fp, ft = v
-                elif len(v) == 4:
-                    fn, fp, ft, fh = v
-                else:
-                    fn, fp, ft, fh, boundary = v
-            else:
-                fn = self.guess_filename(v) or k
-                fp = v
-
-            if isinstance(fp, (str, bytes, bytearray)):
-                fdata = fp
-            elif hasattr(fp, "read"):
-                fdata = fp.read()
-            elif fp is None:
-                continue
-            else:
-                fdata = fp
-
-            rf = RequestField(name=k, data=fdata, filename=fn, headers=fh)
-            rf.make_multipart(content_type=ft)
-            new_fields.append(rf)
-
-        body, content_type = encode_multipart_formdata(new_fields, boundary)
-
-        return body, content_type
-
     def _handle_error(self, e, url=None):
         """Hook for subclassing. Raise the error to interrupt further retrying,
         return it to continue retries and save the error, when retries
         exceed the limit.
         Temporary errors should be swallowed here for automatic retries.
         """
         if isinstance(e, (socket.timeout, gevent.Timeout)):
@@ -410,39 +343,52 @@
         method="GET",
         response_codes=valid_response_codes,
         headers=None,
         payload=None,
         to_string=False,
         debug_stream=None,
         params=None,
-        **kwargs,
+        max_retries=None,
+        max_redirects=None,
+        files=None,
+        **kw,
     ):
-        """Open an URL, do retries and redirects and verify the status code"""
-        # POST or GET parameters can be passed in **kwargs
-        if kwargs:
-            if not payload:
-                payload = kwargs
-            elif isinstance(payload, dict):
-                payload.update(kwargs)
-            files = kwargs.get("files", None)
-        else:
-            files = None
-        req = self._make_request(
+        """Open a URL, do retries and redirects and verify the status code"""
+        # POST or GET parameters can be passed in **kw
+        req_headers = self.default_headers.copy()
+        if headers:
+            req_headers.update(headers)
+        if kw:
+            if method.upper() == "POST":
+                if payload is None:
+                    payload = kw
+                elif isinstance(payload, dict):
+                    payload.update(kw)
+            else:
+                if params is None:
+                    params = kw
+                elif isinstance(params, dict):
+                    params.update(kw)
+        req = _make_request(
             url,
-            method=method,
-            headers=headers,
+            method,
+            headers=req_headers,
             payload=payload,
             params=params,
             files=files,
+            request_type=self.request_type,
         )
-        for retry in range(self.max_retries + 1):
+        max_retries = int(max_retries) if max_retries is not None else self.max_retries
+        max_redirects = int(max_redirects) if max_redirects is not None else self.max_redirects
+
+        for retry in range(max_retries + 1):
             if retry > 0 and self.retry_delay:
                 # Don't wait the first time and skip if no delay specified
                 gevent.sleep(self.retry_delay)
-            for _ in range(self.max_redirects + 1):
+            for _ in range(max_redirects + 1):
                 if self.cookiejar is not None:
                     self.cookiejar.add_cookie_header(req)
 
                 try:
                     resp = self._urlopen(req)
                 except gevent.GreenletExit:
                     raise
@@ -503,70 +449,73 @@
                             return ret
             else:
                 e = RetriesExceeded(url, f"Redirection limit reached ({self.max_redirects})")
                 last_error = self._handle_error(e, url=url)
         else:
             return self._handle_retries_exceeded(url, last_error=last_error)
 
+    def _urlopen(self, request):
+        client = self.clientpool.get_client(request.url_split)
+        resp = client.request(
+            request.method,
+            request.url_split.request_uri,
+            body=request.payload,
+            headers=request.headers,
+        )
+        return self.response_type(resp, request=request, sent_request=resp._sent_request)
+
     @classmethod
-    def _conversation_str(cls, url, resp, payload=None):
+    def _conversation_str(cls, url, resp, payload=None, encoding="utf-8"):
         header_str = "\n".join(f"{key}: {val}" for key, val in resp.headers.items())
         ret = "REQUEST: " + url + "\n" + resp._sent_request
         if payload:
             if isinstance(payload, bytes):
                 try:
-                    ret += payload.decode("utf-8") + "\n\n"
+                    ret += payload.decode(encoding) + "\n\n"
                 except UnicodeDecodeError:
                     ret += "UnicodeDecodeError" + "\n\n"
             elif isinstance(payload, str):
                 ret += payload + "\n\n"
         ret += (
             "RESPONSE: "
             + resp._response.version
             + " "
             + str(resp.status_code)
             + "\n"
             + header_str
             + "\n\n"
-            + resp.content[:].decode("utf-8")
+            + resp.content.decode(encoding)
         )
         return ret
 
-    @classmethod
-    def guess_filename(cls, file):
-        """Tries to guess the filename of the given object."""
-        name = getattr(file, "name", None)
-        if name and isinstance(name, (str, bytes)) and name[0] != "<" and name[-1] != ">":
-            return os.path.basename(name)
-
-    def download(self, url, fpath, chunk_size=16 * 1024, resume=False, **kwargs):
-        kwargs.pop("to_string", None)
-        headers = kwargs.pop("headers", {})
+    def download(self, url, fpath, chunk_size=16 * 1024, resume=False, **kw):
+        kw.pop("to_string", None)
+        headers = kw.pop("headers", {})
         headers["Connection"] = "Keep-Alive"
         if resume and os.path.isfile(fpath):
             offset = os.path.getsize(fpath)
         else:
             offset = 0
 
         for _ in range(self.max_retries + 1):
             if offset:
                 headers["Range"] = f"bytes={offset}-"
-                resp = self.urlopen(url, headers=headers, **kwargs)
+                resp = self.urlopen(url, headers=headers, **kw)
                 cr = resp.headers.get("Content-Range")
                 if (
                     resp.status_code != 206
                     or not cr
                     or not cr.startswith("bytes")
                     or not cr.split(None, 1)[1].startswith(str(offset))
                 ):
                     resp.release()
                     offset = 0
             if not offset:
                 headers.pop("Range", None)
-                resp = self.urlopen(url, headers=headers, **kwargs)
+                resp = self.urlopen(url, headers=headers, **kw)
 
             with open(fpath, "ab" if offset else "wb") as f:
                 if offset:
                     f.seek(offset, os.SEEK_SET)
                 try:
                     data = resp.read(chunk_size)
                     with resp:
@@ -580,7 +529,125 @@
                         offset = f.tell()
                     continue
             # All done, break outer loop
             break
         else:
             self._handle_retries_exceeded(url, last_error=e)
         return resp
+
+
+def _make_request(
+    url, method, headers, payload=None, params=None, files=None, request_type=CompatRequest
+):
+    # Adjust headers depending on payload content
+    content_type = headers.get("content-type", None)
+    if files:
+        payload, content_type = _encode_multipart_formdata(files, payload)
+        headers["content-type"] = content_type
+        headers["content-length"] = len(payload)
+    elif payload:
+        if isinstance(payload, dict):
+            if not content_type:
+                headers["content-type"] = "application/x-www-form-urlencoded; charset=utf-8"
+            payload = urlencode(payload).encode()
+            headers["content-length"] = len(payload)
+        elif not content_type and isinstance(payload, str):
+            headers["content-type"] = "text/plain; charset=utf-8"
+            payload = payload.encode()
+            headers["content-length"] = len(payload)
+        elif not content_type:
+            headers["content-type"] = "application/octet-stream"
+
+    return request_type(url, method=method, headers=headers, payload=payload, params=params)
+
+
+def _guess_filename(file):
+    """Tries to guess the filename of the given object."""
+    name = getattr(file, "name", None)
+    if not name or not isinstance(name, (str, bytes)):
+        return
+    if isinstance(name, bytes):
+        name = name.decode()
+    if name[0] != "<" and name[-1] != ">":
+        return os.path.basename(name)
+
+
+def _encode_multipart_formdata(files, data):
+    """
+    Method taken from models in requests library , usage is the same. The only difference is that
+    you can add custom boundary in 5-tuple version.
+
+    Build the body for a multipart/form-data request.
+
+    Will successfully encode files when passed as a dict or a list of
+    tuples. Order is retained if data is a list of tuples but arbitrary
+    if parameters are supplied as a dict.
+
+    The tuples may be
+    2-tuples (filename, fileobj),
+    3-tuples (filename, fileobj, contentype),
+    4-tuples (filename, fileobj, contentype, custom_headers) or
+    5-tuples (filename, fileobj, contentype, custom_headers, custom boundary).
+
+    example:
+    files = {'file': ('report.xls', body, 'application/vnd.ms-excel', {'Expires': '0'}, 'custom_boundary')}
+
+    """
+
+    if not files:
+        raise ValueError("Files must be provided.")
+    elif isinstance(data, (str, bytes)):
+        raise ValueError("Data must not be a string.")
+
+    new_fields = []
+    fields = to_key_val_list(data or {})
+    files = to_key_val_list(files or {})
+
+    for field, val in fields:
+        if isinstance(val, (str, bytes)) or not hasattr(val, "__iter__"):
+            val = [val]
+        for v in val:
+            if v is not None:
+                if not isinstance(v, bytes):
+                    v = str(v)
+
+                new_fields.append(
+                    (
+                        field.decode("utf-8") if isinstance(field, bytes) else field,
+                        v.encode("utf-8") if isinstance(v, str) else v,
+                    )
+                )
+
+    for k, v in files:
+        # support for explicit filename
+        ft = None
+        fh = None
+        boundary = None
+        if isinstance(v, (tuple, list)):
+            if len(v) == 2:
+                fn, fp = v
+            elif len(v) == 3:
+                fn, fp, ft = v
+            elif len(v) == 4:
+                fn, fp, ft, fh = v
+            else:
+                fn, fp, ft, fh, boundary = v
+        else:
+            fn = _guess_filename(v) or k
+            fp = v
+
+        if isinstance(fp, (str, bytes, bytearray)):
+            fdata = fp
+        elif hasattr(fp, "read"):
+            fdata = fp.read()
+        elif fp is None:
+            continue
+        else:
+            fdata = fp
+
+        rf = RequestField(name=k, data=fdata, filename=fn, headers=fh)
+        rf.make_multipart(content_type=ft)
+        new_fields.append(rf)
+
+    body, content_type = encode_multipart_formdata(new_fields, boundary)
+
+    return body, content_type
```

### Comparing `geventhttpclient-2.2.1/src/geventhttpclient.egg-info/PKG-INFO` & `geventhttpclient-2.3.0/geventhttpclient.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.2.1
+Version: 2.3.0
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: This software is licensed under the MIT License.
         
         Copyright Antonin Amand <antonin.amand@gmail.com>, 2018.
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -64,184 +64,185 @@
 [![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
 [![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
 # geventhttpclient
 
-A high performance, concurrent HTTP client library for python using 
+A [high performance](https://github.com/geventhttpclient/geventhttpclient/blob/master/README.md#Benchmarks),
+concurrent HTTP client library for python using
 [gevent](http://gevent.org).
 
-`gevent.httplib` support was removed in [gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6
-), **geventhttpclient** now provides that missing functionality.
+`gevent.httplib` support for patching `http.client` was removed in
+[gevent 1.0](https://github.com/surfly/gevent/commit/b45b83b1bc4de14e3c4859362825044b8e3df7d6),
+`geventhttpclient` now provides that missing functionality.
 
-**geventhttpclient** uses a fast [http parser](https://github.com/nodejs/llhttp),
+`geventhttpclient` uses a fast [http parser](https://github.com/nodejs/llhttp),
 written in C.
 
-**geventhttpclient** has been specifically designed for high concurrency,
+`geventhttpclient` has been specifically designed for high concurrency,
 streaming and support HTTP 1.1 persistent connections. More generally it is
 designed for efficiently pulling from REST APIs and streaming APIs
 like Twitter's.
 
-Safe SSL support is provided by default. **geventhttpclient** depends on
+Safe SSL support is provided by default. `geventhttpclient` depends on
 the certifi CA Bundle. This is the same CA Bundle which ships with the
 Requests codebase, and is derived from Mozilla Firefox's canonical set.
 
-As of version 2.1, only Python 3.9+ is fully supported (with prebuilt wheels).
-
-A simple example:
+Since version 2.3, `geventhttpclient` features a largely `requests`
+compatible interface. It covers basic HTTP usage including cookie
+management, form data encoding or decoding of compressed data,
+but otherwise isn't as feature rich as the original `requests`. For
+simple use-cases, it can serve as a drop-in replacement.
 
 ```python
-#!/usr/bin/python
+import geventhttpclient as requests
+requests.get("https://github.com").text
+requests.post("http://httpbingo.org/post", data="asdfasd").json()
+
+from geventhttpclient import Session
+s = Session()
+s.get("http://httpbingo.org/headers").json()
+s.get("https://github.com").content
+```
+
+This interface builds on top of the lower level `HTTPClient`.
 
+```python
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
-url = URL('http://gevent.org/')
-
-http = HTTPClient(url.host)
-
-# issue a get request
-response = http.get(url.request_uri)
-
-# read status_code
+url = URL("http://gevent.org/")
+client = HTTPClient(url.host)
+response = client.get(url.request_uri)
 response.status_code
-
-# read response body
 body = response.read()
-
-# close connections
-http.close()
+client.close()
 ```
 
 ## httplib compatibility and monkey patch
 
-**geventhttpclient.httplib** module contains classes for drop in
-replacement of httplib connection and response objects.
-If you use httplib directly you can replace the **httplib** imports
-by **geventhttpclient.httplib**.
+`geventhttpclient.httplib` module contains classes for drop in
+replacement of `http.client` connection and response objects.
+If you use http.client directly you can replace the `httplib` imports
+by `geventhttpclient.httplib`.
 
 ```python
-# from httplib import HTTPConnection
+# from http.client import HTTPConnection
 from geventhttpclient.httplib import HTTPConnection
 ```
 
-If you use **httplib2**, **urllib** or **urllib2**; you can patch **httplib** to
-use the wrappers from **geventhttpclient**.
-For **httplib2**, make sure you patch before you import or the *super*
-calls will fail.
+If you use `httplib2`, `urllib` or `urllib2`; you can patch `httplib` to
+use the wrappers from `geventhttpclient`. For `httplib2`, make sure you
+patch before you import or the `super()` calls will fail.
 
 ```python
 import geventhttpclient.httplib
 geventhttpclient.httplib.patch()
 
 import httplib2
 ```
 
 ## High Concurrency
 
-HTTPClient has connection pool built in and is greenlet safe by design.
-You can use the same instance among several greenlets.
+`HTTPClient` has a connection pool built in and is greenlet safe by design.
+You can use the same instance among several greenlets. It is the low
+level building block of this library.
 
 ```python
-#!/usr/bin/env python
-
 import gevent.pool
 import json
 
 from geventhttpclient import HTTPClient
 from geventhttpclient.url import URL
 
 
 # go to http://developers.facebook.com/tools/explorer and copy the access token
-TOKEN = '<go to http://developers.facebook.com/tools/explorer and copy the access token>'
+TOKEN = "<MY_DEV_TOKEN>"
 
-url = URL('https://graph.facebook.com/me/friends')
-url['access_token'] = TOKEN
+url = URL("https://graph.facebook.com/me/friends", params={"access_token": TOKEN})
 
 # setting the concurrency to 10 allow to create 10 connections and
 # reuse them.
-http = HTTPClient.from_url(url, concurrency=10)
+client = HTTPClient.from_url(url, concurrency=10)
 
-response = http.get(url.request_uri)
+response = client.get(url.request_uri)
 assert response.status_code == 200
 
 # response comply to the read protocol. It passes the stream to
 # the json parser as it's being read.
-data = json.load(response)['data']
+data = json.load(response)["data"]
 
-def print_friend_username(http, friend_id):
-    friend_url = URL('/' + str(friend_id))
-    friend_url['access_token'] = TOKEN
+def print_friend_username(client, friend_id):
+    friend_url = URL(f"/{friend_id}", params={"access_token": TOKEN})
     # the greenlet will block until a connection is available
-    response = http.get(friend_url.request_uri)
+    response = client.get(friend_url.request_uri)
     assert response.status_code == 200
     friend = json.load(response)
-    if 'username' in friend:
-        print('%s: %s' % (friend['username'], friend['name']))
+    if "username" in friend:
+        print(f"{friend['username']}: {friend['name']}")
     else:
-        print('%s has no username.' % friend['name'])
+        print(f"{friend['name']} has no username.")
 
 # allow to run 20 greenlet at a time, this is more than concurrency
 # of the http client but isn't a problem since the client has its own
 # connection pool.
 pool = gevent.pool.Pool(20)
 for item in data:
-    friend_id = item['id']
-    pool.spawn(print_friend_username, http, friend_id)
+    friend_id = item["id"]
+    pool.spawn(print_friend_username, client, friend_id)
 
 pool.join()
-http.close()
+client.close()
 ```
 
 ## Streaming
 
-**geventhttpclient** supports streaming.
-Response objects have a read(N) and readline() method that read the stream
-incrementally.
-See *src/examples/twitter_streaming.py* for pulling twitter stream API.
+`geventhttpclient` supports streaming. Response objects have a `read(n)` and
+`readline()` method that read the stream incrementally.
+See [examples/twitter_streaming.py](https://github.com/geventhttpclient/geventhttpclient/blob/master/examples/twitter_streaming.py)
+for pulling twitter stream API.
 
 Here is an example on how to download a big file chunk by chunk to save memory:
 
 ```python
-#!/usr/bin/env python
-
 from geventhttpclient import HTTPClient, URL
 
-url = URL('http://127.0.0.1:80/100.dat')
-http = HTTPClient.from_url(url)
-response = http.get(url.query_string)
+url = URL("http://127.0.0.1:80/100.dat")
+client = HTTPClient.from_url(url)
+response = client.get(url.query_string)
 assert response.status_code == 200
 
 CHUNK_SIZE = 1024 * 16 # 16KB
-with open('/tmp/100.dat', 'w') as f:
+with open("/tmp/100.dat", "w") as f:
     data = response.read(CHUNK_SIZE)
     while data:
         f.write(data)
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
-The benchmark does 10000 get requests against a local nginx server in the default 
+The benchmark runs 10000 `GET` requests against a local nginx server in the default
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
 second for a couple of popular clients is given in the table below. Please read
 [benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
-for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
+for more details. Also note, [HTTPX](https://www.python-httpx.org/) is better be
+used with `asyncio`, not `gevent`.
 
 | HTTP Client        | RPS    |
 |--------------------|--------|
 | GeventHTTPClient   | 7268.9 |
 | Httplib2 (patched) | 2323.9 |
 | Urllib3            | 2242.5 |
 | Requests           | 1046.1 |
 | Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
 
 ## License
 
-This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT). 
-Previous versions of geventhttpclient used http_parser.c, which in turn 
-was based on `src/http/ngx_http_parse.c` from NGINX, copyright Igor Sysoev, 
-Joyent, Inc., and other Node contributors. For more information, see 
-http://github.com/joyent/http-parser 
+This package is distributed under the [MIT license](https://github.com/geventhttpclient/geventhttpclient/blob/master/LICENSE-MIT).
+Previous versions of geventhttpclient used `http_parser.c`, which in turn was
+based on `http/ngx_http_parse.c` from [NGINX](https://nginx.org), copyright Igor
+Sysoev, Joyent, Inc., and other Node contributors. For more information, see
+http://github.com/joyent/http-parser
```

