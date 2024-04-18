# Comparing `tmp/curl_cffi-0.6.3b1.tar.gz` & `tmp/curl_cffi-0.7.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.6.3b1.tar", last modified: Wed Mar  6 09:22:33 2024, max compression
+gzip compressed data, was "curl_cffi-0.7.0b4.tar", last modified: Thu Apr 18 04:57:50 2024, max compression
```

## Comparing `curl_cffi-0.6.3b1.tar` & `curl_cffi-0.7.0b4.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.965129 curl_cffi-0.6.3b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-03-06 09:22:33.965129 curl_cffi-0.6.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.953129 curl_cffi-0.6.3b1/curl_cffi/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12975 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/_asyncio_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/curl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.957129 curl_cffi-0.6.3b1/curl_cffi/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    39942 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/curl_cffi/requests/websockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.961129 curl_cffi-0.6.3b1/curl_cffi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-03-06 09:22:33.000000 curl_cffi-0.6.3b1/curl_cffi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-06 09:22:33.000000 curl_cffi-0.6.3b1/curl_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 09:22:33.000000 curl_cffi-0.6.3b1/curl_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-06 09:22:33.000000 curl_cffi-0.6.3b1/curl_cffi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 09:22:33.000000 curl_cffi-0.6.3b1/curl_cffi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.957129 curl_cffi-0.6.3b1/ffi/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/ffi/cdef.c
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/ffi/shim.c
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/ffi/shim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.949129 curl_cffi-0.6.3b1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.957129 curl_cffi-0.6.3b1/include/curl/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    22254 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)   130315 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/curl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/curlver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/easy.h
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/header.h
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/mprintf.h
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/multi.h
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/options.h
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/stdcheaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/system.h
--rw-r--r--   0 runner    (1001) docker     (127)    43548 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/typecheck-gcc.h
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/urlapi.h
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-06 09:22:28.000000 curl_cffi-0.6.3b1/include/curl/websockets.h
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/libs.json
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.957129 curl_cffi-0.6.3b1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/scripts/build.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 09:22:33.965129 curl_cffi-0.6.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.953129 curl_cffi-0.6.3b1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.961129 curl_cffi-0.6.3b1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/integration/test_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/integration/test_httpbin.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/integration/test_real_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.961129 curl_cffi-0.6.3b1/tests/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/threads/test_eventlet.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/threads/test_gevent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 09:22:33.961129 curl_cffi-0.6.3b1/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_async_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_curl.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)    21686 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-06 09:22:15.000000 curl_cffi-0.6.3b1/tests/unittest/test_websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.166237 curl_cffi-0.7.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-18 04:57:50.166237 curl_cffi-0.7.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.158237 curl_cffi-0.7.0b4/curl_cffi/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/_asyncio_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16273 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18174 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.158237 curl_cffi-0.7.0b4/curl_cffi/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41876 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/curl_cffi/requests/websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/curl_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-18 04:57:50.000000 curl_cffi-0.7.0b4/curl_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 04:57:50.000000 curl_cffi-0.7.0b4/curl_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 04:57:50.000000 curl_cffi-0.7.0b4/curl_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 04:57:50.000000 curl_cffi-0.7.0b4/curl_cffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 04:57:50.000000 curl_cffi-0.7.0b4/curl_cffi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.158237 curl_cffi-0.7.0b4/ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/ffi/cdef.c
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/ffi/shim.c
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/ffi/shim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.154237 curl_cffi-0.7.0b4/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/include/curl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    22183 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)   131362 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/curl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/curlver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/easy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/header.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/mprintf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/multi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/stdcheaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19017 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/system.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43628 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/typecheck-gcc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/urlapi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-18 04:57:43.000000 curl_cffi-0.7.0b4/include/curl/websockets.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/libs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/scripts/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 04:57:50.166237 curl_cffi-0.7.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.154237 curl_cffi-0.7.0b4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/integration/test_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/integration/test_httpbin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/integration/test_real_world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/tests/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/threads/test_eventlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/threads/test_gevent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:57:50.162237 curl_cffi-0.7.0b4/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_async_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24748 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-18 04:57:30.000000 curl_cffi-0.7.0b4/tests/unittest/test_websockets.py
```

### Comparing `curl_cffi-0.6.3b1/LICENSE` & `curl_cffi-0.7.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/Makefile` & `curl_cffi-0.7.0b4/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .ONESHELL:
 SHELL := bash
 
 # this is the upstream libcurl-impersonate version
-VERSION := 0.6.2b2
-CURL_VERSION := curl-8.1.1
+VERSION := 0.7.0b4
+CURL_VERSION := curl-8.5.0
 
 $(CURL_VERSION):
 	curl -L "https://curl.se/download/$(CURL_VERSION).tar.xz" \
 		-o "$(CURL_VERSION).tar.xz"
 	tar -xf $(CURL_VERSION).tar.xz
 
 curl-impersonate-$(VERSION)/chrome/patches: $(CURL_VERSION)
@@ -35,14 +35,23 @@
 	pip install -e .
 
 build: .preprocessed
 	rm -rf dist/
 	pip install build
 	python -m build --wheel
 
+lint:
+	ruff check
+	ruff format --diff
+	mypy --install-types --non-interactive .
+
+format:
+	ruff check --fix
+	ruff format
+
 test:
 	python -bb -m pytest tests/unittest
 
 clean:
 	rm -rf build/ dist/ curl_cffi.egg-info/ $(CURL_VERSION)/ curl-impersonate-$(VERSION)/
 	rm -rf curl_cffi/*.o curl_cffi/*.so curl_cffi/_wrapper.c
 	rm -rf .preprocessed $(CURL_VERSION).tar.xz curl-impersonate-$(VERSION).tar.gz
```

### Comparing `curl_cffi-0.6.3b1/PKG-INFO` & `curl_cffi-0.7.0b4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_cffi
-Version: 0.6.3b1
+Version: 0.7.0b4
 Summary: libcurl ffi bindings for Python, with impersonation support.
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
         
@@ -36,60 +36,56 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.12.0
-Requires-Dist: certifi
+Requires-Dist: certifi>=2024.2.2
 Provides-Extra: dev
-Requires-Dist: autoflake==1.4; extra == "dev"
-Requires-Dist: coverage==6.4.1; extra == "dev"
-Requires-Dist: cryptography==38.0.3; extra == "dev"
-Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear==22.7.1; extra == "dev"
-Requires-Dist: flake8-pie==0.15.0; extra == "dev"
+Requires-Dist: charset_normalizer<4.0,>=3.3.2; extra == "dev"
+Requires-Dist: coverage<7.0,>=6.4.1; extra == "dev"
+Requires-Dist: cryptography<43.0,>=42.0.5; extra == "dev"
 Requires-Dist: httpx==0.23.1; extra == "dev"
-Requires-Dist: mypy==0.971; extra == "dev"
-Requires-Dist: types-certifi==2021.10.8.2; extra == "dev"
-Requires-Dist: pytest==7.1.2; extra == "dev"
-Requires-Dist: pytest-asyncio==0.19.0; extra == "dev"
-Requires-Dist: pytest-trio==0.7.0; extra == "dev"
-Requires-Dist: trio==0.21.0; extra == "dev"
-Requires-Dist: trio-typing==0.7.0; extra == "dev"
-Requires-Dist: trustme==0.9.0; extra == "dev"
-Requires-Dist: uvicorn==0.18.3; extra == "dev"
-Requires-Dist: websockets==11.0.3; extra == "dev"
-Requires-Dist: ruff==0.1.14; extra == "dev"
+Requires-Dist: mypy<2.0,>=1.9.0; extra == "dev"
+Requires-Dist: pytest<9.0,>=8.1.1; extra == "dev"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "dev"
+Requires-Dist: pytest-trio<1.0,>=0.8.0; extra == "dev"
+Requires-Dist: ruff<1.0,>=0.3.5; extra == "dev"
+Requires-Dist: trio<1.0,>=0.25.0; extra == "dev"
+Requires-Dist: trustme<2.0,>=1.1.0; extra == "dev"
+Requires-Dist: uvicorn<1.0,>=0.29.0; extra == "dev"
+Requires-Dist: websockets<13.0,>=12.0; extra == "dev"
 Provides-Extra: build
 Requires-Dist: cibuildwheel; extra == "build"
 Requires-Dist: wheel; extra == "build"
 Provides-Extra: test
-Requires-Dist: cryptography==38.0.3; extra == "test"
+Requires-Dist: charset_normalizer<4.0,>=3.3.2; extra == "test"
+Requires-Dist: cryptography<43.0,>=42.0.5; extra == "test"
+Requires-Dist: fastapi<1.0,==0.110.0; extra == "test"
 Requires-Dist: httpx==0.23.1; extra == "test"
-Requires-Dist: types-certifi==2021.10.8.2; extra == "test"
-Requires-Dist: pytest==7.1.2; extra == "test"
-Requires-Dist: pytest-asyncio==0.19.0; extra == "test"
-Requires-Dist: pytest-trio==0.7.0; extra == "test"
-Requires-Dist: trio==0.21.0; extra == "test"
-Requires-Dist: trio-typing==0.7.0; extra == "test"
-Requires-Dist: trustme==0.9.0; extra == "test"
-Requires-Dist: uvicorn==0.18.3; extra == "test"
-Requires-Dist: proxy.py==2.4.3; extra == "test"
-Requires-Dist: websockets==11.0.3; extra == "test"
-Requires-Dist: python-multipart==0.0.6; extra == "test"
-Requires-Dist: fastapi==0.100.0; extra == "test"
+Requires-Dist: proxy.py<3.0,>=2.4.3; extra == "test"
+Requires-Dist: pytest<9.0,>=8.1.1; extra == "test"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "test"
+Requires-Dist: pytest-trio<1.0,>=0.8.0; extra == "test"
+Requires-Dist: python-multipart<1.0,>=0.0.9; extra == "test"
+Requires-Dist: trio<1.0,>=0.25.0; extra == "test"
+Requires-Dist: trustme<2.0,>=1.1.0; extra == "test"
+Requires-Dist: uvicorn<1.0,>=0.29.0; extra == "test"
+Requires-Dist: websockets<13.0,>=12.0; extra == "test"
 
 # curl_cffi
 
 [![Downloads](https://static.pepy.tech/badge/curl_cffi/week)](https://pepy.tech/project/curl_cffi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/curl_cffi)
 [![PyPI version](https://badge.fury.io/py/curl-cffi.svg)](https://badge.fury.io/py/curl-cffi)
+[![Generic badge](https://img.shields.io/badge/Telegram%20Group-join-blue?logo=telegram)](https://t.me/+lL9n33eZp480MGM1)
+[![Generic badge](https://img.shields.io/badge/微信交流群-加入-brightgreen?logo=wechat)](./assets/wechat.jpg)
 
-[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) | [Discuss on Telegram](https://t.me/+lL9n33eZp480MGM1)
+[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) 
 
 Python binding for [curl-impersonate](https://github.com/lwthiker/curl-impersonate)
 via [cffi](https://cffi.readthedocs.io/en/latest/).
 
 Unlike other pure python http clients like `httpx` or `requests`, `curl_cffi` can
 impersonate browsers' TLS/JA3 and HTTP/2 fingerprints. If you are blocked by some
 website for no obvious reason, you can give `curl_cffi` a try.
@@ -197,34 +193,40 @@
 # {'cookies': {'foo': 'bar'}}
 ```
 
 Supported impersonate versions, as supported by my [fork](https://github.com/yifeikong/curl-impersonate) of [curl-impersonate](https://github.com/lwthiker/curl-impersonate):
 
 However, only Chrome-like browsers are supported. Firefox support is tracked in [#59](https://github.com/yifeikong/curl_cffi/issues/59).
 
+Browser versions will be added **only** when their fingerprints change. If you see a version, e.g.
+chrome122, were skipped, you can simply impersonate it with your own headers and the previous version.
+
 - chrome99
 - chrome100
 - chrome101
 - chrome104
 - chrome107
 - chrome110
 - chrome116 <sup>[1]</sup>
 - chrome119 <sup>[1]</sup>
 - chrome120 <sup>[1]</sup>
+- chrome123 <sup>[3]</sup>
+- chrome124 <sup>[3]</sup>
 - chrome99_android
 - edge99
 - edge101
 - safari15_3 <sup>[2]</sup>
 - safari15_5 <sup>[2]</sup>
 - safari17_0 <sup>[1]</sup>
 - safari17_2_ios <sup>[1]</sup>
 
 Notes:
 1. Added in version `0.6.0`.
 2. Fixed in version `0.6.0`, previous http2 fingerprints were [not correct](https://github.com/lwthiker/curl-impersonate/issues/215).
+3. Added in version `0.7.0`.
 
 ### asyncio
 
 ```python
 from curl_cffi.requests import AsyncSession
 
 async with AsyncSession() as s:
```

### Comparing `curl_cffi-0.6.3b1/README.md` & `curl_cffi-0.7.0b4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # curl_cffi
 
 [![Downloads](https://static.pepy.tech/badge/curl_cffi/week)](https://pepy.tech/project/curl_cffi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/curl_cffi)
 [![PyPI version](https://badge.fury.io/py/curl-cffi.svg)](https://badge.fury.io/py/curl-cffi)
+[![Generic badge](https://img.shields.io/badge/Telegram%20Group-join-blue?logo=telegram)](https://t.me/+lL9n33eZp480MGM1)
+[![Generic badge](https://img.shields.io/badge/微信交流群-加入-brightgreen?logo=wechat)](./assets/wechat.jpg)
 
-[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) | [Discuss on Telegram](https://t.me/+lL9n33eZp480MGM1)
+[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) 
 
 Python binding for [curl-impersonate](https://github.com/lwthiker/curl-impersonate)
 via [cffi](https://cffi.readthedocs.io/en/latest/).
 
 Unlike other pure python http clients like `httpx` or `requests`, `curl_cffi` can
 impersonate browsers' TLS/JA3 and HTTP/2 fingerprints. If you are blocked by some
 website for no obvious reason, you can give `curl_cffi` a try.
@@ -116,34 +118,40 @@
 # {'cookies': {'foo': 'bar'}}
 ```
 
 Supported impersonate versions, as supported by my [fork](https://github.com/yifeikong/curl-impersonate) of [curl-impersonate](https://github.com/lwthiker/curl-impersonate):
 
 However, only Chrome-like browsers are supported. Firefox support is tracked in [#59](https://github.com/yifeikong/curl_cffi/issues/59).
 
+Browser versions will be added **only** when their fingerprints change. If you see a version, e.g.
+chrome122, were skipped, you can simply impersonate it with your own headers and the previous version.
+
 - chrome99
 - chrome100
 - chrome101
 - chrome104
 - chrome107
 - chrome110
 - chrome116 <sup>[1]</sup>
 - chrome119 <sup>[1]</sup>
 - chrome120 <sup>[1]</sup>
+- chrome123 <sup>[3]</sup>
+- chrome124 <sup>[3]</sup>
 - chrome99_android
 - edge99
 - edge101
 - safari15_3 <sup>[2]</sup>
 - safari15_5 <sup>[2]</sup>
 - safari17_0 <sup>[1]</sup>
 - safari17_2_ios <sup>[1]</sup>
 
 Notes:
 1. Added in version `0.6.0`.
 2. Fixed in version `0.6.0`, previous http2 fingerprints were [not correct](https://github.com/lwthiker/curl-impersonate/issues/215).
+3. Added in version `0.7.0`.
 
 ### asyncio
 
 ```python
 from curl_cffi.requests import AsyncSession
 
 async with AsyncSession() as s:
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
 # curl_cffi [![Downloads](https://static.pepy.tech/badge/curl_cffi/week)]
 (https://pepy.tech/project/curl_cffi) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/curl_cffi) [![PyPI version](https://
-badge.fury.io/py/curl-cffi.svg)](https://badge.fury.io/py/curl-cffi)
+badge.fury.io/py/curl-cffi.svg)](https://badge.fury.io/py/curl-cffi) [![Generic
+badge](https://img.shields.io/badge/Telegram%20Group-join-blue?logo=telegram)]
+(https://t.me/+lL9n33eZp480MGM1) [![Generic badge](https://img.shields.io/
+badge/å¾®ä¿¡äº¤æµç¾¤-å å¥-brightgreen?logo=wechat)](./assets/wechat.jpg)
 [Documentation](https://curl-cffi.readthedocs.io) | [ä¸­æ README](https://
-github.com/yifeikong/curl_cffi/blob/main/README-zh.md) | [Discuss on Telegram]
-(https://t.me/+lL9n33eZp480MGM1) Python binding for [curl-impersonate](https://
-github.com/lwthiker/curl-impersonate) via [cffi](https://cffi.readthedocs.io/
-en/latest/). Unlike other pure python http clients like `httpx` or `requests`,
-`curl_cffi` can impersonate browsers' TLS/JA3 and HTTP/2 fingerprints. If you
-are blocked by some website for no obvious reason, you can give `curl_cffi` a
-try. ------ _[_S_c_r_a_p_f_l_y_._i_o_][Scrapfly](https://scrapfly.io/
-?utm_source=github&utm_medium=sponsoring&utm_campaign=curl_cffi) is an
-enterprise-grade solution providing Web Scraping API that aims to simplify the
-scraping process by managing everything: real browser rendering, rotating
+github.com/yifeikong/curl_cffi/blob/main/README-zh.md) Python binding for
+[curl-impersonate](https://github.com/lwthiker/curl-impersonate) via [cffi]
+(https://cffi.readthedocs.io/en/latest/). Unlike other pure python http clients
+like `httpx` or `requests`, `curl_cffi` can impersonate browsers' TLS/JA3 and
+HTTP/2 fingerprints. If you are blocked by some website for no obvious reason,
+you can give `curl_cffi` a try. ------ _[_S_c_r_a_p_f_l_y_._i_o_][Scrapfly](https://
+scrapfly.io/?utm_source=github&utm_medium=sponsoring&utm_campaign=curl_cffi) is
+an enterprise-grade solution providing Web Scraping API that aims to simplify
+the scraping process by managing everything: real browser rendering, rotating
 proxies, and fingerprints (TLS, HTTP, browser) to bypass all major anti-bots.
 Scrapfly also unlocks the observability by providing an analytical dashboard
 and measuring the success rate/block rate in detail. Scrapfly is a good
 solution if you are looking for a cloud-managed solution for `curl_cffi`. If
 you are managing TLS/HTTP fingerprint by yourself with `curl_cffi`, they also
 maintain [this tool](https://scrapfly.io/web-scraping-tools/curl-python/
 curl_cffi) to convert curl command into python curl_cffi code! ------ ##
@@ -55,41 +57,45 @@
 server set cookies s.get("https://httpbin.org/cookies/set/foo/bar") print
 (s.cookies) #
 ]> # retrieve cookies again to verify r = s.get("https://httpbin.org/cookies")
 print(r.json()) # {'cookies': {'foo': 'bar'}} ``` Supported impersonate
 versions, as supported by my [fork](https://github.com/yifeikong/curl-
 impersonate) of [curl-impersonate](https://github.com/lwthiker/curl-
 impersonate): However, only Chrome-like browsers are supported. Firefox support
-is tracked in [#59](https://github.com/yifeikong/curl_cffi/issues/59). -
-chrome99 - chrome100 - chrome101 - chrome104 - chrome107 - chrome110 -
-chrome116 [1] - chrome119 [1] - chrome120 [1] - chrome99_android - edge99 -
-edge101 - safari15_3 [2] - safari15_5 [2] - safari17_0 [1] - safari17_2_ios [1]
-Notes: 1. Added in version `0.6.0`. 2. Fixed in version `0.6.0`, previous http2
+is tracked in [#59](https://github.com/yifeikong/curl_cffi/issues/59). Browser
+versions will be added **only** when their fingerprints change. If you see a
+version, e.g. chrome122, were skipped, you can simply impersonate it with your
+own headers and the previous version. - chrome99 - chrome100 - chrome101 -
+chrome104 - chrome107 - chrome110 - chrome116 [1] - chrome119 [1] - chrome120
+[1] - chrome123 [3] - chrome124 [3] - chrome99_android - edge99 - edge101 -
+safari15_3 [2] - safari15_5 [2] - safari17_0 [1] - safari17_2_ios [1] Notes: 1.
+Added in version `0.6.0`. 2. Fixed in version `0.6.0`, previous http2
 fingerprints were [not correct](https://github.com/lwthiker/curl-impersonate/
-issues/215). ### asyncio ```python from curl_cffi.requests import AsyncSession
-async with AsyncSession() as s: r = await s.get("https://example.com") ``` More
-concurrency: ```python import asyncio from curl_cffi.requests import
-AsyncSession urls = [ "https://google.com/", "https://facebook.com/", "https://
-twitter.com/", ] async with AsyncSession() as s: tasks = [] for url in urls:
-task = s.get(url) tasks.append(task) results = await asyncio.gather(*tasks) ```
-### WebSockets ```python from curl_cffi.requests import Session, WebSocket def
-on_message(ws: WebSocket, message): print(message) with Session() as s: ws =
-s.ws_connect( "wss://api.gemini.com/v1/marketdata/BTCUSD",
-on_message=on_message, ) ws.run_forever() ``` For low-level APIs, Scrapy
-integration and other advanced topics, see the [docs](https://curl-
-cffi.readthedocs.io) for more details. ## Acknowledgement - Originally forked
-from [multippt/python_curl_cffi](https://github.com/multippt/python_curl_cffi),
-which is under the MIT license. - Headers/Cookies files are copied from [httpx]
-(https://github.com/encode/httpx/blob/master/httpx/_models.py), which is under
-the BSD license. - Asyncio support is inspired by Tornado's curl http client. -
-The WebSocket API is inspired by [websocket_client](https://github.com/
-websocket-client/websocket-client). ## [Sponsor] Bypass Cloudflare with API
-_[_Y_e_s_ _C_a_p_t_c_h_a_!_]Yescaptcha is a proxy service that bypasses Cloudflare and uses
-the API interface to obtain verified cookies (e.g. `cf_clearance`). Click
-[here](https://yescaptcha.com/i/stfnIO) to register: https://yescaptcha.com/i/
-stfnIO ## [Sponsor] ScrapeNinja _[_S_c_r_a_p_e_ _N_i_n_j_a_][ScrapeNinja](https://
+issues/215). 3. Added in version `0.7.0`. ### asyncio ```python from
+curl_cffi.requests import AsyncSession async with AsyncSession() as s: r =
+await s.get("https://example.com") ``` More concurrency: ```python import
+asyncio from curl_cffi.requests import AsyncSession urls = [ "https://
+google.com/", "https://facebook.com/", "https://twitter.com/", ] async with
+AsyncSession() as s: tasks = [] for url in urls: task = s.get(url) tasks.append
+(task) results = await asyncio.gather(*tasks) ``` ### WebSockets ```python from
+curl_cffi.requests import Session, WebSocket def on_message(ws: WebSocket,
+message): print(message) with Session() as s: ws = s.ws_connect( "wss://
+api.gemini.com/v1/marketdata/BTCUSD", on_message=on_message, ) ws.run_forever()
+``` For low-level APIs, Scrapy integration and other advanced topics, see the
+[docs](https://curl-cffi.readthedocs.io) for more details. ## Acknowledgement -
+Originally forked from [multippt/python_curl_cffi](https://github.com/multippt/
+python_curl_cffi), which is under the MIT license. - Headers/Cookies files are
+copied from [httpx](https://github.com/encode/httpx/blob/master/httpx/
+_models.py), which is under the BSD license. - Asyncio support is inspired by
+Tornado's curl http client. - The WebSocket API is inspired by
+[websocket_client](https://github.com/websocket-client/websocket-client). ##
+[Sponsor] Bypass Cloudflare with API _[_Y_e_s_ _C_a_p_t_c_h_a_!_]Yescaptcha is a proxy
+service that bypasses Cloudflare and uses the API interface to obtain verified
+cookies (e.g. `cf_clearance`). Click [here](https://yescaptcha.com/i/stfnIO) to
+register: https://yescaptcha.com/i/stfnIO ## [Sponsor] ScrapeNinja _[_S_c_r_a_p_e
+_N_i_n_j_a_][ScrapeNinja](https://
 scrapeninja.net?utm_source=github&utm_medium=banner&utm_campaign=cffi) is a web
 scraping API with two engines: fast, with high performance and TLS fingerprint;
 and slower with a real browser under the hood. ScrapeNinja handles headless
 browsers, proxies, timeouts, retries, and helps with data extraction, so you
 can just get the data in JSON. Rotating proxies are available out of the box on
 all subscription plans. ## Sponsor_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/__init__.py` & `curl_cffi-0.7.0b4/curl_cffi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "CurlHttpVersion",
     "CurlWsFlag",
     "ffi",
     "lib",
 ]
 
 import _cffi_backend  # noqa: F401  # required by _wrapper
-# This line includes _wrapper.so into the wheel
-from ._wrapper import ffi, lib  # type: ignore
 
-from .const import CurlInfo, CurlMOpt, CurlOpt, CurlECode, CurlHttpVersion, CurlWsFlag
-from .curl import Curl, CurlError, CurlMime
-from .aio import AsyncCurl
+from .__version__ import __curl_version__, __description__, __title__, __version__  # noqa: F401
 
-from .__version__ import __title__, __version__, __description__, __curl_version__
+# This line includes _wrapper.so into the wheel
+from ._wrapper import ffi, lib
+from .aio import AsyncCurl
+from .const import CurlECode, CurlHttpVersion, CurlInfo, CurlMOpt, CurlOpt, CurlWsFlag
+from .curl import Curl, CurlError, CurlMime
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/_asyncio_selector.py` & `curl_cffi-0.7.0b4/curl_cffi/_asyncio_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 """Ensure asyncio selector methods (add_reader, etc.) are available
 tornado 6.1 adds AddThreadSelectorEventLoop event loop,
 running select in a thread and defining these methods on the running event loop.
 This factors out the functionality of AddThreadSelectorEventLoop
 into a standalone SelectorThread object which can be attached to any running event loop.
-Vendored from tornado v6.1.0-64-g289c834b (PR #3029)
+Vendored from tornado v6.4.0
 Redistributed under license Apache-2.0
 """
+
 import asyncio
 import atexit
 import errno
 import functools
 import select
 import socket
 import threading
 import typing
+from contextlib import suppress
 from typing import (
     Any,
     Callable,
-    Union,
-    Optional,
+    Dict,
     List,
+    Optional,
+    Protocol,
+    Set,
     Tuple,
-    Dict,
-)  # noqa: F401
-
-from typing import Set  # noqa: F401
+    TypeVar,
+    Union,
+)
 
-from typing import Protocol
+_T = TypeVar("_T")
 
 
 class _HasFileno(Protocol):
     def fileno(self) -> int:
-        pass
+        return 0
 
 
 _FileDescriptorLike = Union[int, _HasFileno]
 
 
 # Collection of selector thread event loops to shut down on exit.
 _selector_loops: Set["SelectorThread"] = set()
 
 
 def _atexit_callback() -> None:
     for loop in _selector_loops:
         with loop._select_cond:
             loop._closing_selector = True
             loop._select_cond.notify()
-        try:
+        with suppress(BlockingIOError):
             loop._waker_w.send(b"a")
-        except BlockingIOError:
-            pass
-        # If we don't join our (daemon) thread here, we may get a deadlock
-        # during interpreter shutdown. I don't really understand why. This
-        # deadlock happens every time in CI (both travis and appveyor) but
-        # I've never been able to reproduce locally.
-        loop._thread.join()
+        if loop._thread is not None:
+            # If we don't join our (daemon) thread here, we may get a deadlock
+            # during interpreter shutdown. I don't really understand why. This
+            # deadlock happens every time in CI (both travis and appveyor) but
+            # I've never been able to reproduce locally.
+            loop._thread.join()
     _selector_loops.clear()
 
 
 atexit.register(_atexit_callback)
 
 
 class SelectorThread:
@@ -74,32 +76,30 @@
 
     _closed = False
 
     def __init__(self, real_loop: asyncio.AbstractEventLoop) -> None:
         self._real_loop = real_loop
 
         self._select_cond = threading.Condition()
-        self._select_args: Optional[
-            Tuple[List[_FileDescriptorLike], List[_FileDescriptorLike]]
-        ] = None
+        self._select_args: Optional[Tuple[List[_FileDescriptorLike], List[_FileDescriptorLike]]] = (
+            None
+        )
         self._closing_selector = False
         self._thread: Optional[threading.Thread] = None
         self._thread_manager_handle = self._thread_manager()
 
         async def thread_manager_anext() -> None:
             # the anext builtin wasn't added until 3.10. We just need to iterate
             # this generator one step.
             await self._thread_manager_handle.__anext__()
 
         # When the loop starts, start the thread. Not too soon because we can't
         # clean up if we get to this point but the event loop is closed without
         # starting.
-        self._real_loop.call_soon(
-            lambda: self._real_loop.create_task(thread_manager_anext())
-        )
+        self._real_loop.call_soon(lambda: self._real_loop.create_task(thread_manager_anext()))
 
         self._readers: Dict[_FileDescriptorLike, Callable] = {}
         self._writers: Dict[_FileDescriptorLike, Callable] = {}
 
         # Writing to _waker_w will wake up the selector thread, which
         # watches for _waker_r to be readable.
         self._waker_r, self._waker_w = socket.socketpair()
@@ -147,24 +147,20 @@
         except GeneratorExit:
             self.close()
             raise
 
     def _wake_selector(self) -> None:
         if self._closed:
             return
-        try:
+        with suppress(BlockingIOError):
             self._waker_w.send(b"a")
-        except BlockingIOError:
-            pass
 
     def _consume_waker(self) -> None:
-        try:
+        with suppress(BlockingIOError):
             self._waker_r.recv(1024)
-        except BlockingIOError:
-            pass
 
     def _start_select(self) -> None:
         # Capture reader and writer sets here in the event loop
         # thread to avoid any problems with concurrent
         # modification while the select loop uses them.
         with self._select_cond:
             assert self._select_args is None
@@ -231,17 +227,15 @@
                 pass
             except AttributeError:
                 # ProactorEventLoop may raise this instead of RuntimeError
                 # if call_soon_threadsafe races with a call to close().
                 # Swallow it too for consistency.
                 pass
 
-    def _handle_select(
-        self, rs: List[_FileDescriptorLike], ws: List[_FileDescriptorLike]
-    ) -> None:
+    def _handle_select(self, rs: List[_FileDescriptorLike], ws: List[_FileDescriptorLike]) -> None:
         for r in rs:
             self._handle_event(r, self._readers)
         for w in ws:
             self._handle_event(w, self._writers)
         self._start_select()
 
     def _handle_event(
@@ -324,21 +318,27 @@
         self._selector = SelectorThread(real_loop)
 
     def close(self) -> None:
         self._selector.close()
         self._real_loop.close()
 
     def add_reader(
-        self, fd: _FileDescriptorLike, callback: Callable[..., None], *args: Any
+        self,
+        fd: "_FileDescriptorLike",
+        callback: Callable[..., None],
+        *args: Any,  # type: ignore
     ) -> None:
         return self._selector.add_reader(fd, callback, *args)
 
     def add_writer(
-        self, fd: _FileDescriptorLike, callback: Callable[..., None], *args: Any
+        self,
+        fd: "_FileDescriptorLike",
+        callback: Callable[..., None],
+        *args: Any,  # type: ignore
     ) -> None:
         return self._selector.add_writer(fd, callback, *args)
 
-    def remove_reader(self, fd: _FileDescriptorLike) -> bool:
+    def remove_reader(self, fd: "_FileDescriptorLike") -> bool:
         return self._selector.remove_reader(fd)
 
-    def remove_writer(self, fd: _FileDescriptorLike) -> bool:
+    def remove_writer(self, fd: "_FileDescriptorLike") -> bool:
         return self._selector.remove_writer(fd)
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/aio.py` & `curl_cffi-0.7.0b4/curl_cffi/aio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 import sys
 import warnings
 from contextlib import suppress
-from typing import Any
-from weakref import WeakSet, WeakKeyDictionary
+from typing import Any, Dict, Set
+from weakref import WeakKeyDictionary, WeakSet
 
-from ._wrapper import ffi, lib  # type: ignore
+from ._wrapper import ffi, lib
 from .const import CurlMOpt
-from .curl import Curl, DEFAULT_CACERT
+from .curl import DEFAULT_CACERT, Curl
 
 __all__ = ["AsyncCurl"]
 
 if sys.platform == "win32":
     # registry of asyncio loop : selector thread
     _selectors: WeakKeyDictionary = WeakKeyDictionary()
     PROACTOR_WARNING = """
@@ -32,15 +32,15 @@
 
         if asyncio_loop in _selectors:
             return _selectors[asyncio_loop]
 
         if not isinstance(asyncio_loop, getattr(asyncio, "ProactorEventLoop", type(None))):
             return asyncio_loop
 
-        warnings.warn(PROACTOR_WARNING, RuntimeWarning)
+        warnings.warn(PROACTOR_WARNING, RuntimeWarning, stacklevel=2)
 
         from ._asyncio_selector import AddThreadSelectorEventLoop
 
         selector_loop = _selectors[asyncio_loop] = AddThreadSelectorEventLoop(asyncio_loop)  # type: ignore
 
         # patch loop.close to also close the selector thread
         loop_close = asyncio_loop.close
@@ -48,18 +48,19 @@
         def _close_selector_and_loop():
             # restore original before calling selector.close,
             # which in turn calls eventloop.close!
             asyncio_loop.close = loop_close
             _selectors.pop(asyncio_loop, None)
             selector_loop.close()
 
-        asyncio_loop.close = _close_selector_and_loop  # type: ignore # mypy bug - assign a function to method
+        asyncio_loop.close = _close_selector_and_loop
         return selector_loop
 
 else:
+
     def _get_selector(loop) -> asyncio.AbstractEventLoop:
         return loop
 
 
 CURL_POLL_NONE = 0
 CURL_POLL_IN = 1
 CURL_POLL_OUT = 2
@@ -73,15 +74,15 @@
 CURL_CSELECT_OUT = 0x02
 CURL_CSELECT_ERR = 0x04
 
 CURLMSG_DONE = 1
 
 
 @ffi.def_extern()
-def timer_function(curlm, timeout_ms: int, clientp: Any):
+def timer_function(curlm, timeout_ms: int, clientp: "AsyncCurl"):
     """
     see: https://curl.se/libcurl/c/CURLMOPT_TIMERFUNCTION.html
     """
     async_curl = ffi.from_handle(clientp)
 
     # A timeout_ms value of -1 means you should delete the timer.
     if timeout_ms == -1:
@@ -94,17 +95,16 @@
             async_curl.process_data,
             CURL_SOCKET_TIMEOUT,  # -1
             CURL_POLL_NONE,  # 0
         )
         async_curl._timers.add(timer)
 
 
-
 @ffi.def_extern()
-def socket_function(curl, sockfd: int, what: int, clientp: Any, data: Any):
+def socket_function(curl, sockfd: int, what: int, clientp: "AsyncCurl", data: Any):
     async_curl = ffi.from_handle(clientp)
     loop = async_curl.loop
 
     # Always remove and readd fd
     if sockfd in async_curl._sockfds:
         loop.remove_reader(sockfd)
         loop.remove_writer(sockfd)
@@ -114,34 +114,33 @@
         async_curl._sockfds.add(sockfd)
     if what & CURL_POLL_OUT:
         loop.add_writer(sockfd, async_curl.process_data, sockfd, CURL_CSELECT_OUT)
         async_curl._sockfds.add(sockfd)
     if what & CURL_POLL_REMOVE:
         async_curl._sockfds.remove(sockfd)
 
+
 class AsyncCurl:
     """Wrapper around curl_multi handle to provide asyncio support. It uses the libcurl
     socket_action APIs."""
 
     def __init__(self, cacert: str = "", loop=None):
         """
         Parameters:
             cacert: CA cert path to use, by default, curl_cffi uses certs from ``certifi``.
             loop: EventLoop to use.
         """
         self._curlm = lib.curl_multi_init()
         self._cacert = cacert or DEFAULT_CACERT
-        self._curl2future = {}  # curl to future map
-        self._curl2curl = {}  # c curl to Curl
-        self._sockfds = set()  # sockfds
-        self.loop = _get_selector(
-            loop if loop is not None else asyncio.get_running_loop()
-        )
+        self._curl2future: Dict[Curl, asyncio.Future] = {}  # curl to future map
+        self._curl2curl: Dict[ffi.CData, Curl] = {}  # c curl to Curl
+        self._sockfds: Set[int] = set()  # sockfds
+        self.loop = _get_selector(loop if loop is not None else asyncio.get_running_loop())
         self._checker = self.loop.create_task(self._force_timeout())
-        self._timers = WeakSet()
+        self._timers: WeakSet[asyncio.TimerHandle] = WeakSet()
         self._setup()
 
     def _setup(self):
         self.setopt(CurlMOpt.TIMERFUNCTION, lib.timer_function)
         self.setopt(CurlMOpt.SOCKETFUNCTION, lib.socket_function)
         self._self_handle = ffi.new_handle(self)
         self.setopt(CurlMOpt.SOCKETDATA, self._self_handle)
@@ -198,15 +197,15 @@
         running_handle = ffi.new("int *")
         lib.curl_multi_socket_action(self._curlm, sockfd, ev_bitmask, running_handle)
         return running_handle[0]
 
     def process_data(self, sockfd: int, ev_bitmask: int):
         """Call curl_multi_info_read to read data for given socket."""
         if not self._curlm:
-            warnings.warn("Curlm alread closed! quitting from process_data")
+            warnings.warn("Curlm alread closed! quitting from process_data", stacklevel=2)
             return
 
         self.socket_action(sockfd, ev_bitmask)
 
         msg_in_queue = ffi.new("int *")
         while True:
             curl_msg = lib.curl_multi_info_read(self._curlm, msg_in_queue)
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/const.py` & `curl_cffi-0.7.0b4/curl_cffi/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,13 +541,13 @@
     V2_PRIOR_KNOWLEDGE = 5  # please use HTTP 2 without HTTP/1.1 Upgrade */
     V3 = 30  # Makes use of explicit HTTP/3 without fallback.
 
 
 class CurlWsFlag(IntEnum):
     """``CURL_WS_FLAG`` constancs extracted from libcurl, see comments for details"""
 
-    TEXT       = (1<<0)
-    BINARY     = (1<<1)
-    CONT       = (1<<2)
-    CLOSE      = (1<<3)
-    PING       = (1<<4)
-    OFFSET     = (1<<5)
+    TEXT = 1 << 0
+    BINARY = 1 << 1
+    CONT = 1 << 2
+    CLOSE = 1 << 3
+    PING = 1 << 4
+    OFFSET = 1 << 5
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/curl.py` & `curl_cffi-0.7.0b4/curl_cffi/curl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 import warnings
 from http.cookies import SimpleCookie
-from typing import Any, List, Tuple, Union, Optional
 from pathlib import Path
+from typing import Any, List, Optional, Tuple, Union
 
 import certifi
 
-from ._wrapper import ffi, lib  # type: ignore
+from ._wrapper import ffi, lib
 from .const import CurlHttpVersion, CurlInfo, CurlOpt, CurlWsFlag
 
 DEFAULT_CACERT = certifi.where()
+REASON_PHRASE_RE = re.compile(rb"HTTP/\d\.\d [0-9]{3} (.*)")
+STATUS_LINE_RE = re.compile(rb"HTTP/(\d\.\d) ([0-9]{3}) (.*)")
 
 
 class CurlError(Exception):
     """Base exception for curl_cffi package"""
 
     def __init__(self, msg, code: int = 0, *args, **kwargs):
         super().__init__(msg, *args, **kwargs)
@@ -63,19 +65,19 @@
 @ffi.def_extern()
 def write_callback(ptr, size, nmemb, userdata):
     """ffi callback for curl write function, calls the callback python function"""
     # although similar enough to the function above, kept here for performance reasons
     callback = ffi.from_handle(userdata)
     wrote = callback(ffi.buffer(ptr, nmemb)[:])
     wrote = ensure_int(wrote)
-    if wrote == CURL_WRITEFUNC_PAUSE or wrote == CURL_WRITEFUNC_ERROR:
+    if wrote == CURL_WRITEFUNC_PAUSE or wrote == CURL_WRITEFUNC_ERROR:  # noqa: SIM109
         return wrote
     # should make this an exception in future versions
     if wrote != nmemb * size:
-        warnings.warn("Wrote bytes != received bytes.", RuntimeWarning)
+        warnings.warn("Wrote bytes != received bytes.", RuntimeWarning, stacklevel=2)
     return nmemb * size
 
 
 # Credits: @alexio777 on https://github.com/yifeikong/curl_cffi/issues/4
 def slist_to_list(head) -> List[bytes]:
     """Converts curl slist to a python list."""
     result = []
@@ -88,57 +90,57 @@
 
 
 class Curl:
     """
     Wrapper for ``curl_easy_*`` functions of libcurl.
     """
 
-    def __init__(self, cacert: str = "", debug: bool = False, handle=None):
+    def __init__(self, cacert: str = "", debug: bool = False, handle=None) -> None:
         """
         Parameters:
             cacert: CA cert path to use, by default, curl_cffi uses certs from ``certifi``.
             debug: whether to show curl debug messages.
             handle: a curl handle instance from ``curl_easy_init``.
         """
-        self._curl = lib.curl_easy_init() if not handle else handle
+        self._curl = handle if handle else lib.curl_easy_init()
         self._headers = ffi.NULL
         self._proxy_headers = ffi.NULL
         self._resolve = ffi.NULL
         self._cacert = cacert or DEFAULT_CACERT
         self._is_cert_set = False
         self._write_handle = None
         self._header_handle = None
         self._body_handle = None
         # TODO: use CURL_ERROR_SIZE
         self._error_buffer = ffi.new("char[]", 256)
         self._debug = debug
         self._set_error_buffer()
 
-    def _set_error_buffer(self):
+    def _set_error_buffer(self) -> None:
         ret = lib._curl_easy_setopt(self._curl, CurlOpt.ERRORBUFFER, self._error_buffer)
         if ret != 0:
-            warnings.warn("Failed to set error buffer")
+            warnings.warn("Failed to set error buffer", stacklevel=2)
         if self._debug:
             self.setopt(CurlOpt.VERBOSE, 1)
             lib._curl_easy_setopt(self._curl, CurlOpt.DEBUGFUNCTION, lib.debug_function)
 
-    def debug(self):
+    def debug(self) -> None:
         """Set debug to True"""
         self.setopt(CurlOpt.VERBOSE, 1)
         lib._curl_easy_setopt(self._curl, CurlOpt.DEBUGFUNCTION, lib.debug_function)
 
-    def __del__(self):
+    def __del__(self) -> None:
         self.close()
 
-    def _check_error(self, errcode: int, *args):
+    def _check_error(self, errcode: int, *args: Any) -> None:
         error = self._get_error(errcode, *args)
         if error is not None:
             raise error
 
-    def _get_error(self, errcode: int, *args):
+    def _get_error(self, errcode: int, *args: Any):
         if errcode != 0:
             errmsg = ffi.string(self._error_buffer).decode()
             action = " ".join([str(a) for a in args])
             return CurlError(
                 f"Failed to {action}, curl: ({errcode}) {errmsg}. "
                 "See https://curl.se/libcurl/c/libcurl-errors.html first for more details.",
                 code=errcode,
@@ -167,38 +169,31 @@
         # Convert value
         value_type = input_option.get(int(option / 10000) * 10000)
         if value_type == "int*":
             c_value = ffi.new("int*", value)
         elif option == CurlOpt.WRITEDATA:
             c_value = ffi.new_handle(value)
             self._write_handle = c_value
-            lib._curl_easy_setopt(
-                self._curl, CurlOpt.WRITEFUNCTION, lib.buffer_callback
-            )
+            lib._curl_easy_setopt(self._curl, CurlOpt.WRITEFUNCTION, lib.buffer_callback)
         elif option == CurlOpt.HEADERDATA:
             c_value = ffi.new_handle(value)
             self._header_handle = c_value
-            lib._curl_easy_setopt(
-                self._curl, CurlOpt.HEADERFUNCTION, lib.buffer_callback
-            )
+            lib._curl_easy_setopt(self._curl, CurlOpt.HEADERFUNCTION, lib.buffer_callback)
         elif option == CurlOpt.WRITEFUNCTION:
             c_value = ffi.new_handle(value)
             self._write_handle = c_value
             lib._curl_easy_setopt(self._curl, CurlOpt.WRITEFUNCTION, lib.write_callback)
             option = CurlOpt.WRITEDATA
         elif option == CurlOpt.HEADERFUNCTION:
             c_value = ffi.new_handle(value)
             self._header_handle = c_value
             lib._curl_easy_setopt(self._curl, CurlOpt.WRITEFUNCTION, lib.write_callback)
             option = CurlOpt.HEADERDATA
         elif value_type == "char*":
-            if isinstance(value, str):
-                c_value = value.encode()
-            else:
-                c_value = value
+            c_value = value.encode() if isinstance(value, str) else value
             # Must keep a reference, otherwise may be GCed.
             if option == CurlOpt.POSTFIELDS:
                 self._body_handle = c_value
         else:
             raise NotImplementedError("Option unsupported: %s" % option)
 
         if option == CurlOpt.HTTPHEADER:
@@ -264,24 +259,24 @@
         Parameters:
             target: browser to impersonate.
             default_headers: whether to add default headers, like User-Agent.
 
         Returns:
             0 if no error.
         """
-        return lib.curl_easy_impersonate(
-            self._curl, target.encode(), int(default_headers)
-        )
+        return lib.curl_easy_impersonate(self._curl, target.encode(), int(default_headers))
 
-    def _ensure_cacert(self):
+    def _ensure_cacert(self) -> None:
         if not self._is_cert_set:
             ret = self.setopt(CurlOpt.CAINFO, self._cacert)
             self._check_error(ret, "set cacert")
+            ret = self.setopt(CurlOpt.PROXY_CAINFO, self._cacert)
+            self._check_error(ret, "set proxy cacert")
 
-    def perform(self, clear_headers: bool = True):
+    def perform(self, clear_headers: bool = True) -> None:
         """Wrapper for ``curl_easy_perform``, performs a curl request.
 
         Parameters:
             clear_headers: clear header slist used in this perform
 
         Raises:
             CurlError: if the perform was not successful.
@@ -294,38 +289,38 @@
 
         try:
             self._check_error(ret, "perform")
         finally:
             # cleaning
             self.clean_after_perform(clear_headers)
 
-    def clean_after_perform(self, clear_headers: bool = True):
+    def clean_after_perform(self, clear_headers: bool = True) -> None:
         """Clean up handles and buffers after perform, called at the end of `perform`."""
         self._write_handle = None
         self._header_handle = None
         self._body_handle = None
         if clear_headers:
             if self._headers != ffi.NULL:
                 lib.curl_slist_free_all(self._headers)
             self._headers = ffi.NULL
 
             if self._proxy_headers != ffi.NULL:
                 lib.curl_slist_free_all(self._proxy_headers)
             self._proxy_headers = ffi.NULL
 
-    def duphandle(self):
+    def duphandle(self) -> "Curl":
         """Wrapper for ``curl_easy_duphandle``.
 
         This is not a full copy of entire curl object in python. For example, headers
         handle is not copied, you have to set them again."""
         new_handle = lib.curl_easy_duphandle(self._curl)
         c = Curl(cacert=self._cacert, debug=self._debug, handle=new_handle)
         return c
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset all curl options, wrapper for ``curl_easy_reset``."""
         self._is_cert_set = False
         if self._curl is not None:
             lib.curl_easy_reset(self._curl)
             self._set_error_buffer()
         self._resolve = ffi.NULL
 
@@ -334,34 +329,34 @@
 
         Parameters:
             headers: list of headers in bytes.
 
         Returns:
             A parsed cookies.SimpleCookie instance.
         """
-        cookie = SimpleCookie()
+        cookie: SimpleCookie = SimpleCookie()
         for header in headers:
             if header.lower().startswith(b"set-cookie: "):
                 cookie.load(header[12:].decode())  # len("set-cookie: ") == 12
         return cookie
 
     @staticmethod
     def get_reason_phrase(status_line: bytes) -> bytes:
         """Extract reason phrase, like ``OK``, ``Not Found`` from response status line."""
-        m = re.match(rb"HTTP/\d\.\d [0-9]{3} (.*)", status_line)
+        m = REASON_PHRASE_RE.match(status_line)
         return m.group(1) if m else b""
 
     @staticmethod
     def parse_status_line(status_line: bytes) -> Tuple[CurlHttpVersion, int, bytes]:
         """Parse status line.
 
         Returns:
             http_version, status_code, and reason phrase
         """
-        m = re.match(rb"HTTP/(\d\.\d) ([0-9]{3}) (.*)", status_line)
+        m = STATUS_LINE_RE.match(status_line)
         if not m:
             return CurlHttpVersion.V1_0, 0, b""
         if m.group(1) == "2.0":
             http_version = CurlHttpVersion.V2_0
         elif m.group(1) == "1.1":
             http_version = CurlHttpVersion.V1_1
         elif m.group(1) == "1.0":
@@ -369,15 +364,15 @@
         else:
             http_version = CurlHttpVersion.NONE
         status_code = int(m.group(2))
         reason = m.group(3)
 
         return http_version, status_code, reason
 
-    def close(self):
+    def close(self) -> None:
         """Close and cleanup curl handle, wrapper for ``curl_easy_cleanup``."""
         if self._curl:
             lib.curl_easy_cleanup(self._curl)
             self._curl = None
         ffi.release(self._error_buffer)
         self._resolve = ffi.NULL
 
@@ -420,15 +415,15 @@
         """
         n_sent = ffi.new("int *")
         buffer = ffi.from_buffer(payload)
         ret = lib.curl_ws_send(self._curl, buffer, len(buffer), n_sent, 0, flags)
         self._check_error(ret, "WS_SEND")
         return n_sent[0]
 
-    def ws_close(self):
+    def ws_close(self) -> None:
         """Send the close frame."""
         self.ws_send(b"", CurlWsFlag.CLOSE)
 
 
 class CurlMime:
     """Wrapper for the ``curl_mime_`` API."""
 
@@ -444,15 +439,15 @@
         self,
         name: str,
         *,
         content_type: Optional[str] = None,
         filename: Optional[str] = None,
         local_path: Optional[Union[str, bytes, Path]] = None,
         data: Optional[bytes] = None,
-    ):
+    ) -> None:
         """Add a mime part for a mutlipart html form.
 
         Note: You can only use either local_path or data, not both.
 
         Args:
             name: name of the field.
             content_type: content_type for the field. for example: ``image/png``.
@@ -479,19 +474,24 @@
                 raise CurlError("Add field failed.")
 
         if local_path and data:
             raise CurlError("Can not use local_path and data at the same time.")
 
         # this is a filename
         if local_path is not None:
-            if not isinstance(local_path, bytes):
-                local_path = str(local_path).encode()
-            if not Path(local_path.decode()).exists():
-                raise FileNotFoundError(f"File not found at {local_path}")
-            ret = lib.curl_mime_filedata(part, local_path)
+            if isinstance(local_path, Path):
+                local_path_str = str(local_path)
+            elif isinstance(local_path, bytes):
+                local_path_str = local_path.decode()
+            else:
+                local_path_str = local_path
+
+            if not Path(local_path_str).exists():
+                raise FileNotFoundError(f"File not found at {local_path_str}")
+            ret = lib.curl_mime_filedata(part, local_path_str.encode())
             if ret != 0:
                 raise CurlError("Add field failed.")
 
         if data is not None:
             if not isinstance(data, bytes):
                 data = str(data).encode()
             ret = lib.curl_mime_data(part, data, len(data))
@@ -500,20 +500,20 @@
     def from_list(cls, files: List[dict]):
         """Create a multipart instance from a list of dict, for keys, see ``addpart``"""
         form = cls()
         for file in files:
             form.addpart(**file)
         return form
 
-    def attach(self, curl: Optional[Curl] = None):
+    def attach(self, curl: Optional[Curl] = None) -> None:
         """Attach the mime instance to a curl instance."""
         c = curl if curl else self._curl
         c.setopt(CurlOpt.MIMEPOST, self._form)
 
-    def close(self):
+    def close(self) -> None:
         """Close the mime instance and underlying files. This method must be called after
         ``perform`` or ``request``."""
         lib.curl_mime_free(self._form)
         self._form = ffi.NULL
 
-    def __del__(self):
+    def __del__(self) -> None:
         self.close()
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/__init__.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,31 @@
     "WebSocket",
     "WebSocketError",
     "WsCloseCode",
 ]
 
 from functools import partial
 from io import BytesIO
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
-
-from ..curl import CurlMime
 from ..const import CurlHttpVersion, CurlWsFlag
+from ..curl import CurlMime
 from .cookies import Cookies, CookieTypes
-from .models import Request, Response
 from .errors import RequestsError
 from .headers import Headers, HeaderTypes
-from .session import AsyncSession, BrowserType, Session, ProxySpec, ThreadType
+from .models import Request, Response
+from .session import AsyncSession, BrowserType, ProxySpec, Session, ThreadType
 from .websockets import WebSocket, WebSocketError, WsCloseCode
 
 
 def request(
     method: str,
     url: str,
-    params: Optional[dict] = None,
-    data: Optional[Union[Dict[str, str], str, BytesIO, bytes]] = None,
+    params: Optional[Union[Dict, List, Tuple]] = None,
+    data: Optional[Union[Dict[str, str], List[Tuple], str, BytesIO, bytes]] = None,
     json: Optional[dict] = None,
     headers: Optional[HeaderTypes] = None,
     cookies: Optional[CookieTypes] = None,
     files: Optional[Dict] = None,
     auth: Optional[Tuple[str, str]] = None,
     timeout: Union[float, Tuple[float, float]] = 30,
     allow_redirects: bool = True,
@@ -55,46 +54,53 @@
     verify: Optional[bool] = None,
     referer: Optional[str] = None,
     accept_encoding: Optional[str] = "gzip, deflate, br",
     content_callback: Optional[Callable] = None,
     impersonate: Optional[Union[str, BrowserType]] = None,
     thread: Optional[ThreadType] = None,
     default_headers: Optional[bool] = None,
+    default_encoding: Union[str, Callable[[bytes], str]] = "utf-8",
     curl_options: Optional[dict] = None,
     http_version: Optional[CurlHttpVersion] = None,
     debug: bool = False,
     interface: Optional[str] = None,
     multipart: Optional[CurlMime] = None,
     cert: Optional[Union[str, Tuple[str, str]]] = None,
 ) -> Response:
     """Send an http request.
 
     Parameters:
         method: http method for the request: GET/POST/PUT/DELETE etc.
         url: url for the requests.
         params: query string for the requests.
-        data: form values or binary data to use in body, ``Content-Type: application/x-www-form-urlencoded`` will be added if a dict is given.
-        json: json values to use in body, `Content-Type: application/json` will be added automatically.
+        data: form values or binary data to use in body,
+            ``Content-Type: application/x-www-form-urlencoded`` will be added if a dict is given.
+        json: json values to use in body, `Content-Type: application/json` will be added
+            automatically.
         headers: headers to send.
         cookies: cookies to use.
         files: not supported, use ``multipart`` instead.
         auth: HTTP basic auth, a tuple of (username, password), only basic auth is supported.
         timeout: how many seconds to wait before giving up.
         allow_redirects: whether to allow redirection.
         max_redirects: max redirect counts, default unlimited(-1).
         proxies: dict of proxies to use, format: ``{"http": proxy_url, "https": proxy_url}``.
-        proxy: proxy to use, format: "http://user@pass:proxy_url". Cannot be used with the above parameter.
+        proxy: proxy to use, format: "http://user@pass:proxy_url".
+            Can't be used with proxy parameter.
         proxy_auth: HTTP basic auth for proxy, a tuple of (username, password).
         verify: whether to verify https certs.
         referer: shortcut for setting referer header.
         accept_encoding: shortcut for setting accept-encoding header.
-        content_callback: a callback function to receive response body. ``def callback(chunk: bytes) -> None:``
+        content_callback: a callback function to receive response body.
+            ``def callback(chunk: bytes) -> None:``
         impersonate: which browser version to impersonate.
         thread: work with other thread implementations. choices: eventlet, gevent.
         default_headers: whether to set default browser headers.
+        default_encoding: encoding for decoding response content if charset is not found in headers.
+                Defaults to "utf-8". Can be set to a callable for automatic detection.
         curl_options: extra curl options to use.
         http_version: limiting http version, http2 will be tries by default.
         debug: print extra curl debug info.
         interface: which interface use in request to server.
         multipart: upload files using the multipart format, see.
 
     Returns:
@@ -119,14 +125,15 @@
             proxy_auth=proxy_auth,
             verify=verify,
             referer=referer,
             accept_encoding=accept_encoding,
             content_callback=content_callback,
             impersonate=impersonate,
             default_headers=default_headers,
+            default_encoding=default_encoding,
             http_version=http_version,
             interface=interface,
             multipart=multipart,
             cert=cert,
         )
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/cookies.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/cookies.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # See https://github.com/encode/httpx/blob/master/LICENSE.md
 
 __all__ = ["Cookies"]
 
 import re
 import time
 import typing
+import warnings
+from dataclasses import dataclass
 from http.cookiejar import Cookie, CookieJar
 from http.cookies import _unquote
 from urllib.parse import urlparse
-from dataclasses import dataclass
-import warnings
 
 from .errors import CookieConflict, RequestsError
 
 CookieTypes = typing.Union[
     "Cookies", CookieJar, typing.Dict[str, str], typing.List[typing.Tuple[str, str]]
 ]
 
@@ -66,17 +66,15 @@
             name=name,
             value=_unquote(value),
             http_only=http_only,
         )
 
     def to_curl_format(self):
         if not self.hostname:
-            raise RequestsError(
-                "Domain not found for cookie {}={}".format(self.name, self.value)
-            )
+            raise RequestsError(f"Domain not found for cookie {self.name}={self.value}")
         return "\t".join(
             [
                 self.hostname,
                 self.dump_bool(self.subdomains),
                 self.path,
                 self.dump_bool(self.secure),
                 str(self.expires),
@@ -112,18 +110,18 @@
             domain_specified=True,
             domain_initial_dot=bool(self.hostname.startswith(".")),
             path=self.path,
             path_specified=bool(self.path),
             secure=self.secure,
             # using if explicitly to make it clear.
             expires=None if self.expires == 0 else self.expires,
-            discard=True if self.expires == 0 else False,
+            discard=self.expires == 0,
             comment=None,
             comment_url=None,
-            rest=dict(http_only=self.http_only),  # type: ignore
+            rest=dict(http_only=f"{self.http_only}"),
             rfc2109=False,
         )
 
 
 cut_port_re = re.compile(r":\d+$", re.ASCII)
 IPV4_RE = re.compile(r"\.\d+$", re.ASCII)
 
@@ -185,28 +183,27 @@
 
     def update_cookies_from_curl(self, morsels: typing.List[CurlMorsel]):
         for morsel in morsels:
             cookie = morsel.to_cookiejar_cookie()
             self.jar.set_cookie(cookie)
         self.jar.clear_expired_cookies()
 
-    def set(
-        self, name: str, value: str, domain: str = "", path: str = "/", secure=False
-    ) -> None:
+    def set(self, name: str, value: str, domain: str = "", path: str = "/", secure=False) -> None:
         """
         Set a cookie value by name. May optionally include domain and path.
         """
         # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie
         if name.startswith("__Secure-") and secure is False:
-            warnings.warn("`secure` changed to True for `__Secure-` prefixed cookies")
+            warnings.warn("`secure` changed to True for `__Secure-` prefixed cookies", stacklevel=2)
             secure = True
         elif name.startswith("__Host-") and (secure is False or domain or path != "/"):
             warnings.warn(
                 "`host` changed to True, `domain` removed, `path` changed to `/` "
-                "for `__Host-` prefixed cookies"
+                "for `__Host-` prefixed cookies",
+                stacklevel=2,
             )
             secure = True
             domain = ""
             path = "/"
         kwargs = {
             "version": 0,
             "name": name,
@@ -222,15 +219,15 @@
             "expires": None,
             "discard": True,
             "comment": None,
             "comment_url": None,
             "rest": {"HttpOnly": None},
             "rfc2109": False,
         }
-        cookie = Cookie(**kwargs)  # type: ignore
+        cookie = Cookie(**kwargs)
         self.jar.set_cookie(cookie)
 
     def get(  # type: ignore
         self,
         name: str,
         default: typing.Optional[str] = None,
         domain: typing.Optional[str] = None,
@@ -239,32 +236,34 @@
         """
         Get a cookie by name. May optionally include domain and path
         in order to specify exactly which cookie to retrieve.
         """
         value = None
         matched_domain = ""
         for cookie in self.jar:
-            if cookie.name == name:
-                if domain is None or cookie.domain == domain:
-                    if path is None or cookie.path == path:
-                        # if cookies on two different domains do not share a same value
-                        if (
-                            value is not None
-                            and not matched_domain.endswith(cookie.domain)
-                            and not str(cookie.domain).endswith(matched_domain)
-                            and value != cookie.value
-                        ):
-                            message = (
-                                f"Multiple cookies exist with name={name} on "
-                                f"{matched_domain} and {cookie.domain}, add domain "
-                                "parameter to suppress this error."
-                            )
-                            raise CookieConflict(message)
-                        value = cookie.value
-                        matched_domain = cookie.domain or ""
+            if (
+                cookie.name == name
+                and (domain is None or cookie.domain == domain)
+                and (path is None or cookie.path == path)
+            ):
+                # if cookies on two different domains do not share a same value
+                if (
+                    value is not None
+                    and not matched_domain.endswith(cookie.domain)
+                    and not str(cookie.domain).endswith(matched_domain)
+                    and value != cookie.value
+                ):
+                    message = (
+                        f"Multiple cookies exist with name={name} on "
+                        f"{matched_domain} and {cookie.domain}, add domain "
+                        "parameter to suppress this error."
+                    )
+                    raise CookieConflict(message)
+                value = cookie.value
+                matched_domain = cookie.domain or ""
 
         if value is None:
             return default
         return value
 
     def delete(
         self,
@@ -286,17 +285,15 @@
             and (domain is None or cookie.domain == domain)
             and (path is None or cookie.path == path)
         ]
 
         for cookie in remove:
             self.jar.clear(cookie.domain, cookie.path, cookie.name)
 
-    def clear(
-        self, domain: typing.Optional[str] = None, path: typing.Optional[str] = None
-    ) -> None:
+    def clear(self, domain: typing.Optional[str] = None, path: typing.Optional[str] = None) -> None:
         """
         Delete all cookies. Optionally include a domain and path in
         order to only delete a subset of all the cookies.
         """
         args = []
         if domain is not None:
             args.append(domain)
@@ -331,14 +328,11 @@
     def __bool__(self) -> bool:
         for _ in self.jar:
             return True
         return False
 
     def __repr__(self) -> str:
         cookies_repr = ", ".join(
-            [
-                f"<Cookie {cookie.name}={cookie.value} for {cookie.domain} />"
-                for cookie in self.jar
-            ]
+            [f"<Cookie {cookie.name}={cookie.value} for {cookie.domain} />" for cookie in self.jar]
         )
 
         return f"<Cookies[{cookies_repr}]>"
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/headers.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/headers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,143 @@
 # Copied from: https://github.com/encode/httpx/blob/master/httpx/_models.py,
 # which is licensed under the BSD License.
 # See https://github.com/encode/httpx/blob/master/LICENSE.md
 
-import typing
-from collections.abc import Mapping
+import sys
 
-HeaderTypes = typing.Union[
+# typing.Mapping is deprecated in favor of abc.Mapping
+# see: https://docs.python.org/3/library/typing.html#typing.Mapping
+if sys.version_info < (3, 9, 0):
+    from collections.abc import Mapping as AbcMapping
+    from typing import (
+        ItemsView,
+        Iterable,
+        Iterator,
+        KeysView,
+        Mapping,
+        MutableMapping,
+        Sequence,
+        ValuesView,
+    )
+else:
+    from collections.abc import (
+        ItemsView,
+        Iterable,
+        Iterator,
+        KeysView,
+        Mapping,
+        MutableMapping,
+        Sequence,
+        ValuesView,
+    )
+
+    AbcMapping = Mapping  # type: ignore[misc]
+
+from typing import (
+    Any,
+    AnyStr,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
+
+HeaderTypes = Union[
     "Headers",
-    typing.Mapping[str, str],
-    typing.Mapping[bytes, bytes],
-    typing.Sequence[typing.Tuple[str, str]],
-    typing.Sequence[typing.Tuple[bytes, bytes]],
-    typing.Sequence[str],
-    typing.Sequence[bytes],
+    Mapping[str, Optional[str]],
+    Mapping[bytes, Optional[bytes]],
+    Sequence[Tuple[str, str]],
+    Sequence[Tuple[bytes, bytes]],
+    Sequence[Union[str, bytes]],
 ]
 
 
-def to_str(value: typing.Union[str, bytes], encoding: str = "utf-8") -> str:
+def to_str(value: Union[str, bytes], encoding: str = "utf-8") -> str:
     return value if isinstance(value, str) else value.decode(encoding)
 
 
-def to_bytes_or_str(value: str, match_type_of: typing.AnyStr) -> typing.AnyStr:
-    return value if isinstance(match_type_of, str) else value.encode()  # type: ignore
+def to_bytes_or_str(value: str, match_type_of: AnyStr) -> AnyStr:
+    return value if isinstance(match_type_of, str) else value.encode()  # pyright: ignore [reportGeneralTypeIssues]
 
 
 SENSITIVE_HEADERS = {"authorization", "proxy-authorization"}
 
 
 def obfuscate_sensitive_headers(
-    items: typing.Iterable[typing.Tuple[typing.AnyStr, typing.AnyStr]]
-) -> typing.Iterator[typing.Tuple[typing.AnyStr, typing.AnyStr]]:
+    items: Iterable[Tuple[AnyStr, AnyStr]],
+) -> Iterator[Tuple[AnyStr, AnyStr]]:
     for k, v in items:
         if to_str(k.lower()) in SENSITIVE_HEADERS:
             v = to_bytes_or_str("[secure]", match_type_of=v)
         yield k, v
 
 
 def normalize_header_key(
-    value: typing.Union[str, bytes],
+    value: Union[str, bytes],
     lower: bool,
-    encoding: typing.Optional[str] = None,
+    encoding: Optional[str] = None,
 ) -> bytes:
     """
     Coerce str/bytes into a strictly byte-wise HTTP header key.
     """
-    if isinstance(value, bytes):
-        bytes_value = value
-    else:
-        bytes_value = value.encode(encoding or "ascii")
+    bytes_value = value if isinstance(value, bytes) else value.encode(encoding or "ascii")
 
     return bytes_value.lower() if lower else bytes_value
 
 
-def normalize_header_value(
-    value: typing.Union[str, bytes], encoding: typing.Optional[str] = None
-) -> bytes:
+def normalize_header_value(value: Union[str, bytes], encoding: Optional[str] = None) -> bytes:
     """
     Coerce str/bytes into a strictly byte-wise HTTP header value.
     """
     if isinstance(value, bytes):
         return value
     return value.encode(encoding or "ascii")
 
 
-class Headers(typing.MutableMapping[str, str]):
+class Headers(MutableMapping[str, str]):
     """
     HTTP headers, as a case-insensitive multi-dict.
     """
 
     def __init__(
         self,
-        headers: typing.Optional[HeaderTypes] = None,
-        encoding: typing.Optional[str] = None,
+        headers: Optional[HeaderTypes] = None,
+        encoding: Optional[str] = None,
     ) -> None:
-        if headers is None or len(headers) == 0:
-            self._list = []  # type: typing.List[typing.Tuple[bytes, bytes, bytes]]
+        if not headers:
+            self._list = []  # type: List[Tuple[bytes, bytes, bytes]]
         elif isinstance(headers, Headers):
             self._list = list(headers._list)
-        elif isinstance(headers, Mapping):
+        elif isinstance(headers, AbcMapping):
             self._list = [
                 (
                     normalize_header_key(k, lower=False, encoding=encoding),
                     normalize_header_key(k, lower=True, encoding=encoding),
                     normalize_header_value(v, encoding),
                 )
                 for k, v in headers.items()
                 if v is not None
             ]
-        else:
+        elif isinstance(headers, list):
             if isinstance(headers[0], (str, bytes)):
                 sep = ":" if isinstance(headers[0], str) else b":"
                 h = []
                 for line in headers:
-                    k, v = line.split(sep, maxsplit=1)  # type: ignore
-                    v = v.lstrip()
-                    h.append((k, v))
-            else:
+                    k, v = line.split(sep, maxsplit=1)  # pyright: ignore
+                    h.append((k, v.strip()))
+            elif isinstance(headers[0], tuple):
                 h = headers
-
             self._list = [
                 (
-                    normalize_header_key(k, lower=False, encoding=encoding),  # type: ignore
-                    normalize_header_key(k, lower=True, encoding=encoding),  # type: ignore
-                    normalize_header_value(v, encoding),  # type: ignore
+                    normalize_header_key(k, lower=False, encoding=encoding),
+                    normalize_header_key(k, lower=True, encoding=encoding),
+                    normalize_header_value(v, encoding),
                 )
-                for k, v in h
+                for k, v in h  # pyright: ignore
             ]
 
         self._encoding = encoding
 
     @property
     def encoding(self) -> str:
         """
@@ -135,71 +164,70 @@
         return self._encoding
 
     @encoding.setter
     def encoding(self, value: str) -> None:
         self._encoding = value
 
     @property
-    def raw(self) -> typing.List[typing.Tuple[bytes, bytes]]:
+    def raw(self) -> List[Tuple[bytes, bytes]]:
         """
         Returns a list of the raw header items, as byte pairs.
         """
         return [(raw_key, value) for raw_key, _, value in self._list]
 
-    def keys(self) -> typing.KeysView[str]:
+    def keys(self) -> KeysView[str]:
         return {key.decode(self.encoding): None for _, key, _ in self._list}.keys()
 
-    def values(self) -> typing.ValuesView[str]:
-        values_dict: typing.Dict[str, str] = {}
+    def values(self) -> ValuesView[str]:
+        values_dict: Dict[str, str] = {}
         for _, key, value in self._list:
             str_key = key.decode(self.encoding)
             str_value = value.decode(self.encoding)
             if str_key in values_dict:
                 values_dict[str_key] += f", {str_value}"
             else:
                 values_dict[str_key] = str_value
         return values_dict.values()
 
-    def items(self) -> typing.ItemsView[str, str]:
+    def items(self) -> ItemsView[str, str]:
         """
         Return `(key, value)` items of headers. Concatenate headers
         into a single comma separated value when a key occurs multiple times.
         """
-        values_dict: typing.Dict[str, str] = {}
+        values_dict: Dict[str, str] = {}
         for _, key, value in self._list:
             str_key = key.decode(self.encoding)
             str_value = value.decode(self.encoding)
             if str_key in values_dict:
                 values_dict[str_key] += f", {str_value}"
             else:
                 values_dict[str_key] = str_value
         return values_dict.items()
 
-    def multi_items(self) -> typing.List[typing.Tuple[str, str]]:
+    def multi_items(self) -> List[Tuple[str, str]]:
         """
         Return a list of `(key, value)` pairs of headers. Allow multiple
         occurrences of the same key without concatenating into a single
         comma separated value.
         """
         return [
-            (key.decode(self.encoding), value.decode(self.encoding))
-            for key, _, value in self._list
+            (key.decode(self.encoding), value.decode(self.encoding)) for key, _, value in self._list
         ]
 
-    def get(self, key: str, default: typing.Any = None) -> typing.Any:
+    def get(self, key: str, default: Any = None) -> Any:
         """
         Return a header value. If multiple occurrences of the header occur
         then concatenate them together with commas.
         """
         try:
             return self[key]
         except KeyError:
             return default
 
-    def get_list(self, key: str, split_commas: bool = False) -> typing.List[str]:
+    def get_list(self, key: str, split_commas: bool = False) -> List[str]:
         """
         Return a list of all header values for a given key.
         If `split_commas=True` is passed, then any comma separated header
         values are split into multiple return strings.
         """
         get_header_key = key.lower().encode(self.encoding)
 
@@ -213,17 +241,17 @@
             return values
 
         split_values = []
         for value in values:
             split_values.extend([item.strip() for item in value.split(",")])
         return split_values
 
-    def update(self, headers: typing.Optional[HeaderTypes] = None) -> None:  # type: ignore
+    def update(self, headers: Optional[HeaderTypes] = None) -> None:  # type: ignore
         headers = Headers(headers)
-        for key in headers.keys():
+        for key in headers:
             if key in self:
                 self.pop(key)
         self._list.extend(headers._list)
 
     def copy(self) -> "Headers":
         return Headers(self, encoding=self.encoding)
 
@@ -252,17 +280,15 @@
         Retains insertion order.
         """
         set_key = key.encode(self._encoding or "utf-8")
         set_value = value.encode(self._encoding or "utf-8")
         lookup_key = set_key.lower()
 
         found_indexes = [
-            idx
-            for idx, (_, item_key, _) in enumerate(self._list)
-            if item_key == lookup_key
+            idx for idx, (_, item_key, _) in enumerate(self._list) if item_key == lookup_key
         ]
 
         for idx in reversed(found_indexes[1:]):
             del self._list[idx]
 
         if found_indexes:
             idx = found_indexes[0]
@@ -273,36 +299,34 @@
     def __delitem__(self, key: str) -> None:
         """
         Remove the header `key`.
         """
         del_key = key.lower().encode(self.encoding)
 
         pop_indexes = [
-            idx
-            for idx, (_, item_key, _) in enumerate(self._list)
-            if item_key.lower() == del_key
+            idx for idx, (_, item_key, _) in enumerate(self._list) if item_key.lower() == del_key
         ]
 
         if not pop_indexes:
             raise KeyError(key)
 
         for idx in reversed(pop_indexes):
             del self._list[idx]
 
-    def __contains__(self, key: typing.Any) -> bool:
+    def __contains__(self, key: Any) -> bool:
         header_key = key.lower().encode(self.encoding)
         return header_key in [key for _, key, _ in self._list]
 
-    def __iter__(self) -> typing.Iterator[typing.Any]:
+    def __iter__(self) -> Iterator[Any]:
         return iter(self.keys())
 
     def __len__(self) -> int:
         return len(self._list)
 
-    def __eq__(self, other: typing.Any) -> bool:
+    def __eq__(self, other: Any) -> bool:
         try:
             other_headers = Headers(other)
         except ValueError:
             return False
 
         self_list = [(key, value) for _, key, value in self._list]
         other_list = [(key, value) for _, key, value in other_headers._list]
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/models.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+import queue
+import re
 import warnings
+from concurrent.futures import Future
 from json import loads
-from typing import Optional
-import queue
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Union
 
 from .. import Curl
-from .headers import Headers
 from .cookies import Cookies
 from .errors import RequestsError
+from .headers import Headers
+
+CHARSET_RE = re.compile(r"charset=([\w-]+)")
 
 
 def clear_queue(q: queue.Queue):
     with q.mutex:
         q.queue.clear()
         q.all_tasks_done.notify_all()
         q.unfinished_tasks = 0
 
 
 class Request:
     """Representing a sent request."""
+
     def __init__(self, url: str, headers: Headers, method: str):
         self.url = url
         self.headers = headers
         self.method = method
 
 
 class Response:
@@ -35,14 +40,17 @@
         reason: http response reason, such as OK, Not Found.
         ok: is status_code in [200, 400)?
         headers: response headers.
         cookies: response cookies.
         elapsed: how many seconds the request cost.
         encoding: http body encoding.
         charset: alias for encoding.
+        charset_encoding: encoding specified by the Content-Type header.
+        default_encoding: encoding for decoding response content if charset is not found in
+                headers. Defaults to "utf-8". Can be set to a callable for automatic detection.
         redirect_count: how many redirects happened.
         redirect_url: the final redirected url.
         http_version: http version used.
         history: history redirections, only headers are available.
     """
 
     def __init__(self, curl: Optional[Curl] = None, request: Optional[Request] = None):
@@ -52,58 +60,99 @@
         self.content = b""
         self.status_code = 200
         self.reason = "OK"
         self.ok = True
         self.headers = Headers()
         self.cookies = Cookies()
         self.elapsed = 0.0
-        self.encoding = "utf-8"
-        self.charset = self.encoding
+        self.default_encoding: Union[str, Callable[[bytes], str]] = "utf-8"
         self.redirect_count = 0
         self.redirect_url = ""
         self.http_version = 0
-        self.history = []
-        self.infos = {}
+        self.history: List[Dict[str, Any]] = []
+        self.infos: Dict[str, Any] = {}
         self.queue: Optional[queue.Queue] = None
-        self.stream_task = None
+        self.stream_task: Optional[Future] = None
+        self.astream_task: Optional[Awaitable] = None
         self.quit_now = None
 
+    @property
+    def charset(self) -> str:
+        """Alias for encoding."""
+        return self.encoding
+
+    @property
+    def encoding(self) -> str:
+        """
+        Determines the encoding to decode byte content into text.
+
+        The method follows a specific priority to decide the encoding:
+        1. If `.encoding` has been explicitly set, it is used.
+        2. The encoding specified by the `charset` parameter in the `Content-Type` header.
+        3. The encoding specified by the `default_encoding` attribute. This can either be
+           a string (e.g., "utf-8") or a callable for charset autodetection.
+        """
+        if not hasattr(self, "_encoding"):
+            encoding = self.charset_encoding
+            if encoding is None:
+                if isinstance(self.default_encoding, str):
+                    encoding = self.default_encoding
+                elif callable(self.default_encoding):
+                    encoding = self.default_encoding(self.content)
+            self._encoding = encoding or "utf-8"
+        return self._encoding
+
+    @encoding.setter
+    def encoding(self, value: str) -> None:
+        if hasattr(self, "_text"):
+            raise ValueError("Cannot set encoding after text has been accessed")
+        self._encoding = value
+
+    @property
+    def charset_encoding(self) -> Optional[str]:
+        """Return the encoding, as specified by the Content-Type header."""
+        content_type = self.headers.get("Content-Type")
+        if content_type:
+            charset_match = CHARSET_RE.search(content_type)
+            return charset_match.group(1) if charset_match else None
+        return None
+
+    @property
+    def text(self) -> str:
+        if not hasattr(self, "_text"):
+            if not self.content:
+                self._text = ""
+            else:
+                self._text = self._decode(self.content)
+        return self._text
+
     def _decode(self, content: bytes) -> str:
         try:
-            return content.decode(self.charset, errors="replace")
+            return content.decode(self.encoding, errors="replace")
         except (UnicodeDecodeError, LookupError):
             return content.decode("utf-8-sig")
 
-    @property
-    def text(self) -> str:
-        return self._decode(self.content)
-
     def raise_for_status(self):
         """Raise an error if status code is not in [200, 400)"""
         if not self.ok:
             raise RequestsError(f"HTTP Error {self.status_code}: {self.reason}")
 
     def iter_lines(self, chunk_size=None, decode_unicode=False, delimiter=None):
         """
         iterate streaming content line by line, separated by ``\\n``.
 
         Copied from: https://requests.readthedocs.io/en/latest/_modules/requests/models/
         which is under the License: Apache 2.0
         """
         pending = None
 
-        for chunk in self.iter_content(
-            chunk_size=chunk_size, decode_unicode=decode_unicode
-        ):
+        for chunk in self.iter_content(chunk_size=chunk_size, decode_unicode=decode_unicode):
             if pending is not None:
                 chunk = pending + chunk
-            if delimiter:
-                lines = chunk.split(delimiter)
-            else:
-                lines = chunk.splitlines()
+            lines = chunk.split(delimiter) if delimiter else chunk.splitlines()
             if lines and lines[-1] and chunk and lines[-1][-1] == chunk[-1]:
                 pending = lines.pop()
             else:
                 pending = None
 
             yield from lines
 
@@ -111,61 +160,60 @@
             yield pending
 
     def iter_content(self, chunk_size=None, decode_unicode=False):
         """
         iterate streaming content chunk by chunk in bytes.
         """
         if chunk_size:
-            warnings.warn("chunk_size is ignored, there is no way to tell curl that.")
+            warnings.warn("chunk_size is ignored, there is no way to tell curl that.", stacklevel=2)
         if decode_unicode:
             raise NotImplementedError()
+
+        assert self.queue and self.curl, "stream mode is not enabled."
+
         while True:
-            chunk = self.queue.get()  # type: ignore
+            chunk = self.queue.get()
 
             # re-raise the exception if something wrong happened.
             if isinstance(chunk, RequestsError):
-                self.curl.reset()  # type: ignore
+                self.curl.reset()
                 raise chunk
 
             # end of stream.
             if chunk is None:
-                self.curl.reset()  # type: ignore
+                self.curl.reset()
                 return
 
             yield chunk
 
     def json(self, **kw):
-        """return a prased json object of the content."""
+        """return a parsed json object of the content."""
         return loads(self.content, **kw)
 
     def close(self):
         """Close the streaming connection, only valid in stream mode."""
+
         if self.quit_now:
             self.quit_now.set()
         if self.stream_task:
             self.stream_task.result()
 
     async def aiter_lines(self, chunk_size=None, decode_unicode=False, delimiter=None):
         """
         iterate streaming content line by line, separated by ``\\n``.
 
         Copied from: https://requests.readthedocs.io/en/latest/_modules/requests/models/
         which is under the License: Apache 2.0
         """
         pending = None
 
-        async for chunk in self.aiter_content(
-            chunk_size=chunk_size, decode_unicode=decode_unicode
-        ):
+        async for chunk in self.aiter_content(chunk_size=chunk_size, decode_unicode=decode_unicode):
             if pending is not None:
                 chunk = pending + chunk
-            if delimiter:
-                lines = chunk.split(delimiter)
-            else:
-                lines = chunk.splitlines()
+            lines = chunk.split(delimiter) if delimiter else chunk.splitlines()
             if lines and lines[-1] and chunk and lines[-1][-1] == chunk[-1]:
                 pending = lines.pop()
             else:
                 pending = None
 
             for line in lines:
                 yield line
@@ -174,20 +222,22 @@
             yield pending
 
     async def aiter_content(self, chunk_size=None, decode_unicode=False):
         """
         iterate streaming content chunk by chunk in bytes.
         """
         if chunk_size:
-            warnings.warn("chunk_size is ignored, there is no way to tell curl that.")
+            warnings.warn("chunk_size is ignored, there is no way to tell curl that.", stacklevel=2)
         if decode_unicode:
             raise NotImplementedError()
 
+        assert self.queue and self.curl, "stream mode is not enabled."
+
         while True:
-            chunk = await self.queue.get()  # type: ignore
+            chunk = await self.queue.get()
 
             # re-raise the exception if something wrong happened.
             if isinstance(chunk, RequestsError):
                 await self.aclose()
                 raise chunk
 
             # end of stream.
@@ -208,15 +258,15 @@
         chunks = []
         async for chunk in self.aiter_content():
             chunks.append(chunk)
         return b"".join(chunks)
 
     async def aclose(self):
         """Close the streaming connection, only valid in stream mode."""
-        if self.stream_task:
-            await self.stream_task  # type: ignore
 
-            
+        if self.astream_task:
+            await self.astream_task
+
     # It prints the status code of the response instead of
     # the object's memory location.
-    def __repr__(self)->str:
-        return f"<Response [{self.status_code}]>"
+    def __repr__(self) -> str:
+        return f"<Response [{self.status_code}]>"
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/session.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,94 @@
 import asyncio
-from contextlib import contextmanager, asynccontextmanager
-import re
+import math
+import queue
 import threading
 import warnings
-import queue
-import math
+from collections import Counter
+from concurrent.futures import ThreadPoolExecutor
+from contextlib import asynccontextmanager, contextmanager, suppress
 from enum import Enum
 from functools import partialmethod
 from io import BytesIO
 from json import dumps
-from typing import Callable, Dict, List, Any, Optional, TypedDict, Tuple, Union, cast, TYPE_CHECKING, Literal
-from urllib.parse import ParseResult, parse_qsl, unquote, urlencode, urlparse
-from concurrent.futures import ThreadPoolExecutor
-
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypedDict,
+    Union,
+    cast,
+)
+from urllib.parse import ParseResult, parse_qsl, unquote, urlencode, urljoin, urlparse
 
-from .. import AsyncCurl, Curl, CurlError, CurlInfo, CurlOpt, CurlHttpVersion
+from .. import AsyncCurl, Curl, CurlError, CurlHttpVersion, CurlInfo, CurlOpt
 from ..curl import CURL_WRITEFUNC_ERROR, CurlMime
 from .cookies import Cookies, CookieTypes, CurlMorsel
 from .errors import RequestsError, SessionClosed
 from .headers import Headers, HeaderTypes
 from .models import Request, Response
 from .websockets import WebSocket
 
-try:
+with suppress(ImportError):
     import gevent
-except ImportError:
-    pass
 
-try:
+with suppress(ImportError):
     import eventlet.tpool
-except ImportError:
-    pass
 
 if TYPE_CHECKING:
 
     class ProxySpec(TypedDict, total=False):
         all: str
         http: str
         https: str
         ws: str
         wss: str
 
 else:
     ProxySpec = Dict[str, str]
 
-CHARSET_RE = re.compile(r"charset=([\w-]+)")
 ThreadType = Literal["eventlet", "gevent"]
 
+
 class BrowserType(str, Enum):
     edge99 = "edge99"
     edge101 = "edge101"
     chrome99 = "chrome99"
     chrome100 = "chrome100"
     chrome101 = "chrome101"
     chrome104 = "chrome104"
     chrome107 = "chrome107"
     chrome110 = "chrome110"
     chrome116 = "chrome116"
     chrome119 = "chrome119"
     chrome120 = "chrome120"
+    chrome123 = "chrome123"
+    chrome124 = "chrome124"
     chrome99_android = "chrome99_android"
     safari15_3 = "safari15_3"
     safari15_5 = "safari15_5"
     safari17_0 = "safari17_0"
     safari17_2_ios = "safari17_2_ios"
 
-    chrome = "chrome120"
+    chrome = "chrome123"
     safari = "safari17_0"
     safari_ios = "safari17_2_ios"
 
     @classmethod
     def has(cls, item):
         return item in cls.__members__
 
     @classmethod
     def normalize(cls, item):
-        if item == "chrome":
+        if item == "chrome":  # noqa: SIM116
             return cls.chrome
         elif item == "safari":
             return cls.safari
         elif item == "safari_ios":
             return cls.safari_ios
         else:
             return item
@@ -87,15 +96,21 @@
 
 class BrowserSpec:
     """A more structured way of selecting browsers"""
 
     # TODO
 
 
-def _update_url_params(url: str, params: Dict) -> str:
+def _is_absolute_url(url: str) -> bool:
+    """Check if the provided url is an absolute url"""
+    parsed_url = urlparse(url)
+    return bool(parsed_url.scheme and parsed_url.hostname)
+
+
+def _update_url_params(url: str, params: Union[Dict, List, Tuple]) -> str:
     """Add GET params to provided URL being aware of existing.
 
     Parameters:
         url: string of target URL
         params: dict containing requested params to be added
 
     Returns:
@@ -104,31 +119,45 @@
     >> url = 'http://stackoverflow.com/test?answers=true'
     >> new_params = {'answers': False, 'data': ['some','values']}
     >> _update_url_params(url, new_params)
     'http://stackoverflow.com/test?data=some&data=values&answers=false'
     """
     # Unquoting URL first so we don't loose existing args
     url = unquote(url)
+
     # Extracting url info
     parsed_url = urlparse(url)
+
     # Extracting URL arguments from parsed URL
     get_args = parsed_url.query
-    # Converting URL arguments to dict
-    parsed_get_args = dict(parse_qsl(get_args))
-    # Merging URL arguments dict with new params
-    parsed_get_args.update(params)
 
-    # Bool and Dict values should be converted to json-friendly values
-    # you may throw this part away if you don't like it :)
-    parsed_get_args.update(
-        {k: dumps(v) for k, v in parsed_get_args.items() if isinstance(v, (bool, dict))}
-    )
+    # Do NOT converting URL arguments to dict
+    parsed_get_args = parse_qsl(get_args)
+
+    # Merging URL arguments dict with new params
+    old_args_counter = Counter(x[0] for x in parsed_get_args)
+    if isinstance(params, dict):
+        params = list(params.items())
+    new_args_counter = Counter(x[0] for x in params)
+
+    for key, value in params:
+        # Bool and Dict values should be converted to json-friendly values
+        # you may throw this part away if you don't like it :)
+        if isinstance(value, (bool, dict)):
+            value = dumps(value)
+
+        # 1 to 1 mapping, we have to search and update it.
+        if old_args_counter.get(key) == 1 and new_args_counter.get(key) == 1:
+            parsed_get_args = [(x if x[0] != key else (key, value)) for x in parsed_get_args]
+        else:
+            parsed_get_args.append((key, value))
 
     # Converting URL argument to proper query string
     encoded_get_args = urlencode(parsed_get_args, doseq=True)
+
     # Creating new parsed result object based on provided with new
     # URL arguments. Same thing happens inside of urlparse.
     new_url = ParseResult(
         parsed_url.scheme,
         parsed_url.netloc,
         parsed_url.path,
         parsed_url.params,
@@ -174,63 +203,70 @@
         *,
         headers: Optional[HeaderTypes] = None,
         cookies: Optional[CookieTypes] = None,
         auth: Optional[Tuple[str, str]] = None,
         proxies: Optional[ProxySpec] = None,
         proxy: Optional[str] = None,
         proxy_auth: Optional[Tuple[str, str]] = None,
+        base_url: Optional[str] = None,
         params: Optional[dict] = None,
         verify: bool = True,
         timeout: Union[float, Tuple[float, float]] = 30,
         trust_env: bool = True,
         allow_redirects: bool = True,
         max_redirects: int = -1,
         impersonate: Optional[Union[str, BrowserType]] = None,
         default_headers: bool = True,
+        default_encoding: Union[str, Callable[[bytes], str]] = "utf-8",
         curl_options: Optional[dict] = None,
         curl_infos: Optional[list] = None,
         http_version: Optional[CurlHttpVersion] = None,
         debug: bool = False,
         interface: Optional[str] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
     ):
         self.headers = Headers(headers)
         self.cookies = Cookies(cookies)
         self.auth = auth
+        self.base_url = base_url
         self.params = params
         self.verify = verify
         self.timeout = timeout
         self.trust_env = trust_env
         self.allow_redirects = allow_redirects
         self.max_redirects = max_redirects
         self.impersonate = impersonate
         self.default_headers = default_headers
+        self.default_encoding = default_encoding
         self.curl_options = curl_options or {}
         self.curl_infos = curl_infos or []
         self.http_version = http_version
         self.debug = debug
         self.interface = interface
         self.cert = cert
 
         if proxy and proxies:
             raise TypeError("Cannot specify both 'proxy' and 'proxies'")
         if proxy:
             proxies = {"all": proxy}
         self.proxies: ProxySpec = proxies or {}
         self.proxy_auth = proxy_auth
 
+        if self.base_url and not _is_absolute_url(self.base_url):
+            raise ValueError("You need to provide an absolute url for 'base_url'")
+
         self._closed = False
 
     def _set_curl_options(
         self,
         curl,
         method: str,
         url: str,
-        params: Optional[dict] = None,
-        data: Optional[Union[Dict[str, str], str, BytesIO, bytes]] = None,
+        params: Optional[Union[Dict, List, Tuple]] = None,
+        data: Optional[Union[Dict[str, str], List[Tuple], str, BytesIO, bytes]] = None,
         json: Optional[dict] = None,
         headers: Optional[HeaderTypes] = None,
         cookies: Optional[CookieTypes] = None,
         files: Optional[Dict] = None,
         auth: Optional[Tuple[str, str]] = None,
         timeout: Optional[Union[float, Tuple[float, float], object]] = not_set,
         allow_redirects: Optional[bool] = None,
@@ -256,24 +292,28 @@
         c = curl
 
         # method
         if method == "POST":
             c.setopt(CurlOpt.POST, 1)
         elif method != "GET":
             c.setopt(CurlOpt.CUSTOMREQUEST, method.encode())
+        if method == "HEAD":
+            c.setopt(CurlOpt.NOBODY, 1)
 
         # url
         if self.params:
             url = _update_url_params(url, self.params)
         if params:
             url = _update_url_params(url, params)
+        if self.base_url:
+            url = urljoin(self.base_url, url)
         c.setopt(CurlOpt.URL, url.encode())
 
         # data/body/json
-        if isinstance(data, dict):
+        if isinstance(data, (dict, list, tuple)):
             body = urlencode(data).encode()
         elif isinstance(data, str):
             body = data.encode()
         elif isinstance(data, BytesIO):
             body = data.read()
         elif isinstance(data, bytes):
             body = data
@@ -282,46 +322,37 @@
         else:
             raise TypeError("data must be dict, str, BytesIO or bytes")
         if json is not None:
             body = dumps(json, separators=(",", ":")).encode()
 
         # Tell libcurl to be aware of bodies and related headers when,
         # 1. POST/PUT/PATCH, even if the body is empty, it's up to curl to decide what to do;
-        # 2. GET/DELETE with body, although it's against the RFC, some applications. e.g. Elasticsearch, use this.
+        # 2. GET/DELETE with body, although it's against the RFC, some applications.
+        #   e.g. Elasticsearch, use this.
         if body or method in ("POST", "PUT", "PATCH"):
             c.setopt(CurlOpt.POSTFIELDS, body)
             # necessary if body contains '\0'
             c.setopt(CurlOpt.POSTFIELDSIZE, len(body))
 
         # headers
         h = Headers(self.headers)
         h.update(headers)
-
         # remove Host header if it's unnecessary, otherwise curl maybe confused.
         # Host header will be automatically added by curl if it's not present.
         # https://github.com/yifeikong/curl_cffi/issues/119
         host_header = h.get("Host")
         if host_header is not None:
             u = urlparse(url)
             if host_header == u.netloc or host_header == u.hostname:
-                try:
-                    del h["Host"]
-                except KeyError:
-                    pass
-
-        header_lines = []
-        for k, v in h.multi_items():
-            header_lines.append(f"{k}: {v}")
+                h.pop("Host", None)
+        header_lines = [f"{k}: {v}" for k, v in h.multi_items()]
         if json is not None:
             _update_header_line(header_lines, "Content-Type", "application/json")
         if isinstance(data, dict) and method != "POST":
-            _update_header_line(
-                header_lines, "Content-Type", "application/x-www-form-urlencoded"
-            )
-        # print("header lines", header_lines)
+            _update_header_line(header_lines, "Content-Type", "application/x-www-form-urlencoded")
         c.setopt(CurlOpt.HTTPHEADER, [h.encode() for h in header_lines])
 
         req = Request(url, h, method)
 
         # cookies
         c.setopt(CurlOpt.COOKIEFILE, b"")  # always enable the curl cookie engine first
         c.setopt(CurlOpt.COOKIELIST, "ALL")  # remove all the old cookies first.
@@ -338,25 +369,25 @@
         if files:
             raise NotImplementedError("files is not supported, use `multipart`.")
 
         # multipart
         if multipart:
             # multipart will overrides postfields
             for k, v in cast(dict, data or {}).items():
-                multipart.addpart(name=k, data=v)
+                multipart.addpart(name=k, data=v.encode() if isinstance(v, str) else v)
             c.setopt(CurlOpt.MIMEPOST, multipart._form)
 
         # auth
         if self.auth or auth:
             if self.auth:
                 username, password = self.auth
             if auth:
                 username, password = auth
-            c.setopt(CurlOpt.USERNAME, username.encode())  # type: ignore
-            c.setopt(CurlOpt.PASSWORD, password.encode())  # type: ignore
+            c.setopt(CurlOpt.USERNAME, username.encode())  # pyright: ignore [reportPossiblyUnboundVariable=none]
+            c.setopt(CurlOpt.PASSWORD, password.encode())  # pyright: ignore [reportPossiblyUnboundVariable=none]
 
         # timeout
         if timeout is not_set:
             timeout = self.timeout
         if timeout is None:
             timeout = 0  # indefinitely
 
@@ -365,23 +396,23 @@
             all_timeout = connect_timeout + read_timeout
             c.setopt(CurlOpt.CONNECTTIMEOUT_MS, int(connect_timeout * 1000))
             if not stream:
                 c.setopt(CurlOpt.TIMEOUT_MS, int(all_timeout * 1000))
             else:
                 # trick from: https://github.com/yifeikong/curl_cffi/issues/156
                 c.setopt(CurlOpt.LOW_SPEED_LIMIT, 1)
-                c.setopt(CurlOpt.LOW_SPEED_TIME, math.ceil(all_timeout))  # type: ignore
+                c.setopt(CurlOpt.LOW_SPEED_TIME, math.ceil(all_timeout))
 
-        else:
+        elif isinstance(timeout, (int, float)):
             if not stream:
-                c.setopt(CurlOpt.TIMEOUT_MS, int(timeout * 1000))  # type: ignore
+                c.setopt(CurlOpt.TIMEOUT_MS, int(timeout * 1000))
             else:
-                c.setopt(CurlOpt.CONNECTTIMEOUT_MS, int(timeout * 1000))  # type: ignore
+                c.setopt(CurlOpt.CONNECTTIMEOUT_MS, int(timeout * 1000))
                 c.setopt(CurlOpt.LOW_SPEED_LIMIT, 1)
-                c.setopt(CurlOpt.LOW_SPEED_TIME, math.ceil(timeout))  # type: ignore
+                c.setopt(CurlOpt.LOW_SPEED_TIME, math.ceil(timeout))
 
         # allow_redirects
         c.setopt(
             CurlOpt.FOLLOWLOCATION,
             int(self.allow_redirects if allow_redirects is None else allow_redirects),
         )
 
@@ -397,20 +428,26 @@
         if proxy:
             proxies = {"all": proxy}
         if proxies is None:
             proxies = self.proxies
 
         if proxies:
             parts = urlparse(url)
-            proxy = proxies.get(parts.scheme, proxies.get("all"))
+            proxy = cast(Optional[str], proxies.get(parts.scheme, proxies.get("all")))
             if parts.hostname:
-                proxy = proxies.get(
-                    f"{parts.scheme}://{parts.hostname}",
-                    proxies.get(f"all://{parts.hostname}"),
-                ) or proxy
+                proxy = (
+                    cast(
+                        Optional[str],
+                        proxies.get(
+                            f"{parts.scheme}://{parts.hostname}",
+                            proxies.get(f"all://{parts.hostname}"),
+                        ),
+                    )
+                    or proxy
+                )
 
             if proxy is not None:
                 if parts.scheme == "https" and proxy.startswith("https://"):
                     warnings.warn(
                         "You may be using http proxy WRONG, the prefix should be 'http://' not 'https://',"
                         "see: https://github.com/yifeikong/curl_cffi/issues/6",
                         RuntimeWarning,
@@ -458,17 +495,15 @@
             else:
                 cert, key = cert
                 c.setopt(CurlOpt.SSLCERT, cert)
                 c.setopt(CurlOpt.SSLKEY, key)
 
         # impersonate
         impersonate = impersonate or self.impersonate
-        default_headers = (
-            self.default_headers if default_headers is None else default_headers
-        )
+        default_headers = self.default_headers if default_headers is None else default_headers
         if impersonate:
             impersonate = BrowserType.normalize(impersonate)
             ret = c.impersonate(impersonate, default_headers=default_headers)
             if ret != 0:
                 raise RequestsError(f"Impersonating {impersonate} is not supported")
 
         # http_version, after impersonate, which will change this to http2
@@ -481,55 +516,52 @@
             c.setopt(k, v)
 
         buffer = None
         q = None
         header_recved = None
         quit_now = None
         if stream:
-            q = queue_class()  # type: ignore
+            q = queue_class()
             header_recved = event_class()
             quit_now = event_class()
 
             def qput(chunk):
                 if not header_recved.is_set():
                     header_recved.set()
                 if quit_now.is_set():
                     return CURL_WRITEFUNC_ERROR
                 q.put_nowait(chunk)
                 return len(chunk)
 
-            c.setopt(CurlOpt.WRITEFUNCTION, qput)  # type: ignore
+            c.setopt(CurlOpt.WRITEFUNCTION, qput)
         elif content_callback is not None:
             c.setopt(CurlOpt.WRITEFUNCTION, content_callback)
         else:
             buffer = BytesIO()
             c.setopt(CurlOpt.WRITEDATA, buffer)
         header_buffer = BytesIO()
         c.setopt(CurlOpt.HEADERDATA, header_buffer)
 
-        if method == "HEAD":
-            c.setopt(CurlOpt.NOBODY, 1)
-
         # interface
         interface = interface or self.interface
         if interface:
             c.setopt(CurlOpt.INTERFACE, interface.encode())
 
         # max_recv_speed
         # do not check, since 0 is a valid value to disable it
         c.setopt(CurlOpt.MAX_RECV_SPEED_LARGE, max_recv_speed)
 
         return req, buffer, header_buffer, q, header_recved, quit_now
 
-    def _parse_response(self, curl, buffer, header_buffer):
+    def _parse_response(self, curl, buffer, header_buffer, default_encoding):
         c = curl
         rsp = Response(c)
         rsp.url = cast(bytes, c.getinfo(CurlInfo.EFFECTIVE_URL)).decode()
         if buffer:
-            rsp.content = buffer.getvalue()  # type: ignore
+            rsp.content = buffer.getvalue()
         rsp.http_version = cast(int, c.getinfo(CurlInfo.HTTP_VERSION))
         rsp.status_code = cast(int, c.getinfo(CurlInfo.RESPONSE_CODE))
         rsp.ok = 200 <= rsp.status_code < 400
         header_lines = header_buffer.getvalue().splitlines()
 
         # TODO history urls
         header_list = []
@@ -544,31 +576,23 @@
                 continue
             if header_line.startswith(b" ") or header_line.startswith(b"\t"):
                 header_list[-1] += header_line
                 continue
             header_list.append(header_line)
         rsp.headers = Headers(header_list)
         # print("Set-cookie", rsp.headers["set-cookie"])
-        morsels = [
-            CurlMorsel.from_curl_format(l) for l in c.getinfo(CurlInfo.COOKIELIST)
-        ]
+        morsels = [CurlMorsel.from_curl_format(c) for c in c.getinfo(CurlInfo.COOKIELIST)]
         # for l in c.getinfo(CurlInfo.COOKIELIST):
         #     print("Curl Cookies", l.decode())
 
         self.cookies.update_cookies_from_curl(morsels)
         rsp.cookies = self.cookies
         # print("Cookies after extraction", self.cookies)
 
-        content_type = rsp.headers.get("Content-Type", default="")
-        charset_match = CHARSET_RE.search(content_type)
-        charset = charset_match.group(1) if charset_match else "utf-8"
-
-        rsp.charset = charset
-        rsp.encoding = charset  # TODO use chardet
-
+        rsp.default_encoding = default_encoding
         rsp.elapsed = cast(float, c.getinfo(CurlInfo.TOTAL_TIME))
         rsp.redirect_count = cast(int, c.getinfo(CurlInfo.REDIRECT_COUNT))
         rsp.redirect_url = cast(bytes, c.getinfo(CurlInfo.REDIRECT_URL)).decode()
 
         for info in self.curl_infos:
             rsp.infos[info] = c.getinfo(info)
 
@@ -599,24 +623,28 @@
                 from another thread.
             thread: thread engine to use for working with other thread implementations.
                 choices: eventlet, gevent., possible values: eventlet, gevent.
             headers: headers to use in the session.
             cookies: cookies to add in the session.
             auth: HTTP basic auth, a tuple of (username, password), only basic auth is supported.
             proxies: dict of proxies to use, format: {"http": proxy_url, "https": proxy_url}.
-            proxy: proxy to use, format: "http://proxy_url". Cannot be used with the above parameter.
+            proxy: proxy to use, format: "http://proxy_url".
+                Cannot be used with the above parameter.
             proxy_auth: HTTP basic auth for proxy, a tuple of (username, password).
+            base_url: absolute url to use for relative urls.
             params: query string for the session.
             verify: whether to verify https certs.
             timeout: how many seconds to wait before giving up.
             trust_env: use http_proxy/https_proxy and other environments, default True.
             allow_redirects: whether to allow redirection.
             max_redirects: max redirect counts, default unlimited(-1).
             impersonate: which browser version to impersonate in the session.
             interface: which interface use in request to server.
+            default_encoding: encoding for decoding response content if charset is not found in
+                headers. Defaults to "utf-8". Can be set to a callable for automatic detection.
 
         Notes:
             This class can be used as a context manager.
 
         .. code-block:: python
 
             from curl_cffi.requests import Session
@@ -640,15 +668,15 @@
         else:
             self._curl = curl if curl else Curl(debug=self.debug)
 
     @property
     def curl(self):
         if self._use_thread_local_curl:
             if self._is_customized_curl:
-                warnings.warn("Creating fresh curl handle in different thread.")
+                warnings.warn("Creating fresh curl handle in different thread.", stacklevel=2)
             if not getattr(self._local, "curl", None):
                 self._local.curl = Curl(debug=self.debug)
             return self._local.curl
         else:
             return self._curl
 
     @property
@@ -677,16 +705,16 @@
         finally:
             rsp.close()
 
     def ws_connect(
         self,
         url,
         *args,
-        on_message: Optional[Callable[[WebSocket, str], None]] = None,
-        on_error: Optional[Callable[[WebSocket, str], None]] = None,
+        on_message: Optional[Callable[[WebSocket, bytes], None]] = None,
+        on_error: Optional[Callable[[WebSocket, CurlError], None]] = None,
         on_open: Optional[Callable] = None,
         on_close: Optional[Callable] = None,
         **kwargs,
     ) -> WebSocket:
         """Connects to a websocket url.
 
         Args:
@@ -718,16 +746,16 @@
             on_close=on_close,
         )
 
     def request(
         self,
         method: str,
         url: str,
-        params: Optional[dict] = None,
-        data: Optional[Union[Dict[str, str], str, BytesIO, bytes]] = None,
+        params: Optional[Union[Dict, List, Tuple]] = None,
+        data: Optional[Union[Dict[str, str], List[Tuple], str, BytesIO, bytes]] = None,
         json: Optional[dict] = None,
         headers: Optional[HeaderTypes] = None,
         cookies: Optional[CookieTypes] = None,
         files: Optional[Dict] = None,
         auth: Optional[Tuple[str, str]] = None,
         timeout: Optional[Union[float, Tuple[float, float], object]] = not_set,
         allow_redirects: Optional[bool] = None,
@@ -737,14 +765,15 @@
         proxy_auth: Optional[Tuple[str, str]] = None,
         verify: Optional[bool] = None,
         referer: Optional[str] = None,
         accept_encoding: Optional[str] = "gzip, deflate, br",
         content_callback: Optional[Callable] = None,
         impersonate: Optional[Union[str, BrowserType]] = None,
         default_headers: Optional[bool] = None,
+        default_encoding: Union[str, Callable[[bytes], str]] = "utf-8",
         http_version: Optional[CurlHttpVersion] = None,
         interface: Optional[str] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
         stream: bool = False,
         max_recv_speed: int = 0,
         multipart: Optional[CurlMime] = None,
     ) -> Response:
@@ -795,62 +824,62 @@
         if stream:
             header_parsed = threading.Event()
 
             def perform():
                 try:
                     c.perform()
                 except CurlError as e:
-                    rsp = self._parse_response(c, buffer, header_buffer)
+                    rsp = self._parse_response(c, buffer, header_buffer, default_encoding)
                     rsp.request = req
-                    q.put_nowait(RequestsError(str(e), e.code, rsp))  # type: ignore
+                    cast(queue.Queue, q).put_nowait(RequestsError(str(e), e.code, rsp))
                 finally:
-                    if not header_recved.is_set():  # type: ignore
-                        header_recved.set()  # type: ignore
+                    if not cast(threading.Event, header_recved).is_set():
+                        cast(threading.Event, header_recved).set()
                     # None acts as a sentinel
-                    q.put(None)  # type: ignore
+                    cast(queue.Queue, q).put(None)
 
             def cleanup(fut):
                 header_parsed.wait()
                 c.reset()
 
             stream_task = self.executor.submit(perform)
             stream_task.add_done_callback(cleanup)
 
             # Wait for the first chunk
-            header_recved.wait()  # type: ignore
-            rsp = self._parse_response(c, buffer, header_buffer)
+            cast(threading.Event, header_recved).wait()
+            rsp = self._parse_response(c, buffer, header_buffer, default_encoding)
             header_parsed.set()
 
             # Raise the exception if something wrong happens when receiving the header.
-            first_element = _peek_queue(q)  # type: ignore
+            first_element = _peek_queue(cast(queue.Queue, q))
             if isinstance(first_element, RequestsError):
                 c.reset()
                 raise first_element
 
             rsp.request = req
-            rsp.stream_task = stream_task  # type: ignore
-            rsp.quit_now = quit_now  # type: ignore
+            rsp.stream_task = stream_task
+            rsp.quit_now = quit_now
             rsp.queue = q
             return rsp
         else:
             try:
                 if self._thread == "eventlet":
                     # see: https://eventlet.net/doc/threading.html
                     eventlet.tpool.execute(c.perform)
                 elif self._thread == "gevent":
                     # see: https://www.gevent.org/api/gevent.threadpool.html
                     gevent.get_hub().threadpool.spawn(c.perform).get()
                 else:
                     c.perform()
             except CurlError as e:
-                rsp = self._parse_response(c, buffer, header_buffer)
+                rsp = self._parse_response(c, buffer, header_buffer, default_encoding)
                 rsp.request = req
                 raise RequestsError(str(e), e.code, rsp) from e
             else:
-                rsp = self._parse_response(c, buffer, header_buffer)
+                rsp = self._parse_response(c, buffer, header_buffer, default_encoding)
                 rsp.request = req
                 return rsp
             finally:
                 c.reset()
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
@@ -874,28 +903,33 @@
     ):
         """
         Parameters set in the init method will be override by the same parameter in request method.
 
         Parameters:
             loop: loop to use, if not provided, the running loop will be used.
             async_curl: [AsyncCurl](/api/curl_cffi#curl_cffi.AsyncCurl) object to use.
-            max_clients: maxmium curl handle to use in the session, this will affect the concurrency ratio.
+            max_clients: maxmium curl handle to use in the session,
+                this will affect the concurrency ratio.
             headers: headers to use in the session.
             cookies: cookies to add in the session.
             auth: HTTP basic auth, a tuple of (username, password), only basic auth is supported.
             proxies: dict of proxies to use, format: {"http": proxy_url, "https": proxy_url}.
-            proxy: proxy to use, format: "http://proxy_url". Cannot be used with the above parameter.
+            proxy: proxy to use, format: "http://proxy_url".
+                Cannot be used with the above parameter.
             proxy_auth: HTTP basic auth for proxy, a tuple of (username, password).
+            base_url: absolute url to use for relative urls.
             params: query string for the session.
             verify: whether to verify https certs.
             timeout: how many seconds to wait before giving up.
             trust_env: use http_proxy/https_proxy and other environments, default True.
             allow_redirects: whether to allow redirection.
             max_redirects: max redirect counts, default unlimited(-1).
             impersonate: which browser version to impersonate in the session.
+            default_encoding: encoding for decoding response content if charset is not found
+                in headers. Defaults to "utf-8". Can be set to a callable for automatic detection.
 
         Notes:
             This class can be used as a context manager, and it's recommended to use via
             ``async with``.
             However, unlike aiohttp, it is not required to use ``with``.
 
         .. code-block:: python
@@ -937,18 +971,16 @@
     async def pop_curl(self):
         curl = await self.pool.get()
         if curl is None:
             curl = Curl(debug=self.debug)
         return curl
 
     def push_curl(self, curl):
-        try:
+        with suppress(asyncio.QueueFull):
             self.pool.put_nowait(curl)
-        except asyncio.QueueFull:
-            pass
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         await self.close()
         return None
@@ -993,16 +1025,16 @@
         await self.loop.run_in_executor(None, curl.perform)
         return WebSocket(self, curl)
 
     async def request(
         self,
         method: str,
         url: str,
-        params: Optional[dict] = None,
-        data: Optional[Union[Dict[str, str], str, BytesIO, bytes]] = None,
+        params: Optional[Union[Dict, List, Tuple]] = None,
+        data: Optional[Union[Dict[str, str], List[Tuple], str, BytesIO, bytes]] = None,
         json: Optional[dict] = None,
         headers: Optional[HeaderTypes] = None,
         cookies: Optional[CookieTypes] = None,
         files: Optional[Dict] = None,
         auth: Optional[Tuple[str, str]] = None,
         timeout: Optional[Union[float, Tuple[float, float], object]] = not_set,
         allow_redirects: Optional[bool] = None,
@@ -1012,14 +1044,15 @@
         proxy_auth: Optional[Tuple[str, str]] = None,
         verify: Optional[bool] = None,
         referer: Optional[str] = None,
         accept_encoding: Optional[str] = "gzip, deflate, br",
         content_callback: Optional[Callable] = None,
         impersonate: Optional[Union[str, BrowserType]] = None,
         default_headers: Optional[bool] = None,
+        default_encoding: Union[str, Callable[[bytes], str]] = "utf-8",
         http_version: Optional[CurlHttpVersion] = None,
         interface: Optional[str] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
         stream: bool = False,
         max_recv_speed: int = 0,
         multipart: Optional[CurlMime] = None,
     ):
@@ -1062,58 +1095,58 @@
         if stream:
             task = self.acurl.add_handle(curl)
 
             async def perform():
                 try:
                     await task
                 except CurlError as e:
-                    rsp = self._parse_response(curl, buffer, header_buffer)
+                    rsp = self._parse_response(curl, buffer, header_buffer, default_encoding)
                     rsp.request = req
-                    q.put_nowait(RequestsError(str(e), e.code, rsp))  # type: ignore
+                    cast(asyncio.Queue, q).put_nowait(RequestsError(str(e), e.code, rsp))
                 finally:
-                    if not header_recved.is_set():  # type: ignore
-                        header_recved.set()  # type: ignore
+                    if not cast(asyncio.Event, header_recved).is_set():
+                        cast(asyncio.Event, header_recved).set()
                     # None acts as a sentinel
-                    await q.put(None)  # type: ignore
+                    await cast(asyncio.Queue, q).put(None)
 
             def cleanup(fut):
                 self.release_curl(curl)
 
             stream_task = asyncio.create_task(perform())
             stream_task.add_done_callback(cleanup)
 
-            await header_recved.wait()  # type: ignore
+            await cast(asyncio.Event, header_recved).wait()
 
             # Unlike threads, coroutines does not use preemptive scheduling.
             # For asyncio, there is no need for a header_parsed event, the
             # _parse_response will execute in the foreground, no background tasks running.
-            rsp = self._parse_response(curl, buffer, header_buffer)
+            rsp = self._parse_response(curl, buffer, header_buffer, default_encoding)
 
-            first_element = _peek_aio_queue(q)  # type: ignore
+            first_element = _peek_aio_queue(cast(asyncio.Queue, q))
             if isinstance(first_element, RequestsError):
                 self.release_curl(curl)
                 raise first_element
 
             rsp.request = req
-            rsp.stream_task = stream_task  # type: ignore
+            rsp.astream_task = stream_task
             rsp.quit_now = quit_now
             rsp.queue = q
             return rsp
         else:
             try:
                 # curl.debug()
                 task = self.acurl.add_handle(curl)
                 await task
                 # print(curl.getinfo(CurlInfo.CAINFO))
             except CurlError as e:
-                rsp = self._parse_response(curl, buffer, header_buffer)
+                rsp = self._parse_response(curl, buffer, header_buffer, default_encoding)
                 rsp.request = req
                 raise RequestsError(str(e), e.code, rsp) from e
             else:
-                rsp = self._parse_response(curl, buffer, header_buffer)
+                rsp = self._parse_response(curl, buffer, header_buffer, default_encoding)
                 rsp.request = req
                 return rsp
             finally:
                 self.release_curl(curl)
 
     head = partialmethod(request, "HEAD")
     get = partialmethod(request, "GET")
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi/requests/websockets.py` & `curl_cffi-0.7.0b4/curl_cffi/requests/websockets.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import struct
 from enum import IntEnum
 from typing import Callable, Optional, Tuple
 
 from curl_cffi.const import CurlECode, CurlWsFlag
 from curl_cffi.curl import CurlError
 
-
 ON_MESSAGE_T = Callable[["WebSocket", bytes], None]
 ON_ERROR_T = Callable[["WebSocket", CurlError], None]
 ON_OPEN_T = Callable[["WebSocket"], None]
 ON_CLOSE_T = Callable[["WebSocket", int, str], None]
 
 
 class WsCloseCode(IntEnum):
@@ -106,21 +105,27 @@
                     if len(msg) < 2:
                         code = WsCloseCode.UNKNOWN
                         reason = ""
                     else:
                         try:
                             code = struct.unpack_from("!H", msg)[0]
                             reason = msg[2:].decode()
-                        except UnicodeDecodeError:
-                            raise WebSocketError("Invalid close message", WsCloseCode.INVALID_DATA)
-                        except Exception:
-                            raise WebSocketError("Invalid close frame", WsCloseCode.PROTOCOL_ERROR)
+                        except UnicodeDecodeError as e:
+                            raise WebSocketError(
+                                "Invalid close message", WsCloseCode.INVALID_DATA
+                            ) from e
+                        except Exception as e:
+                            raise WebSocketError(
+                                "Invalid close frame", WsCloseCode.PROTOCOL_ERROR
+                            ) from e
                         else:
                             if code < 3000 and (code not in WsCloseCode or code == 1005):
-                                raise WebSocketError("Invalid close code", WsCloseCode.PROTOCOL_ERROR)
+                                raise WebSocketError(
+                                    "Invalid close code", WsCloseCode.PROTOCOL_ERROR
+                                )
                     if self.on_close:
                         self.on_close(self, code, reason)
             except WebSocketError as e:
                 # Follow the spec to close the connection
                 # TODO: Consider adding setting to autoclose connection on error-free close
                 self.close(e.code)
                 if self.on_error:
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi.egg-info/PKG-INFO` & `curl_cffi-0.7.0b4/curl_cffi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curl_cffi
-Version: 0.6.3b1
+Version: 0.7.0b4
 Summary: libcurl ffi bindings for Python, with impersonation support.
 Author-email: Yifei Kong <kong@yifei.me>
 License: MIT License
         
         Copyright (c) 2018 multippt
         Copyright (c) 2022 Yifei Kong
         
@@ -36,60 +36,56 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.12.0
-Requires-Dist: certifi
+Requires-Dist: certifi>=2024.2.2
 Provides-Extra: dev
-Requires-Dist: autoflake==1.4; extra == "dev"
-Requires-Dist: coverage==6.4.1; extra == "dev"
-Requires-Dist: cryptography==38.0.3; extra == "dev"
-Requires-Dist: flake8==6.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear==22.7.1; extra == "dev"
-Requires-Dist: flake8-pie==0.15.0; extra == "dev"
+Requires-Dist: charset_normalizer<4.0,>=3.3.2; extra == "dev"
+Requires-Dist: coverage<7.0,>=6.4.1; extra == "dev"
+Requires-Dist: cryptography<43.0,>=42.0.5; extra == "dev"
 Requires-Dist: httpx==0.23.1; extra == "dev"
-Requires-Dist: mypy==0.971; extra == "dev"
-Requires-Dist: types-certifi==2021.10.8.2; extra == "dev"
-Requires-Dist: pytest==7.1.2; extra == "dev"
-Requires-Dist: pytest-asyncio==0.19.0; extra == "dev"
-Requires-Dist: pytest-trio==0.7.0; extra == "dev"
-Requires-Dist: trio==0.21.0; extra == "dev"
-Requires-Dist: trio-typing==0.7.0; extra == "dev"
-Requires-Dist: trustme==0.9.0; extra == "dev"
-Requires-Dist: uvicorn==0.18.3; extra == "dev"
-Requires-Dist: websockets==11.0.3; extra == "dev"
-Requires-Dist: ruff==0.1.14; extra == "dev"
+Requires-Dist: mypy<2.0,>=1.9.0; extra == "dev"
+Requires-Dist: pytest<9.0,>=8.1.1; extra == "dev"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "dev"
+Requires-Dist: pytest-trio<1.0,>=0.8.0; extra == "dev"
+Requires-Dist: ruff<1.0,>=0.3.5; extra == "dev"
+Requires-Dist: trio<1.0,>=0.25.0; extra == "dev"
+Requires-Dist: trustme<2.0,>=1.1.0; extra == "dev"
+Requires-Dist: uvicorn<1.0,>=0.29.0; extra == "dev"
+Requires-Dist: websockets<13.0,>=12.0; extra == "dev"
 Provides-Extra: build
 Requires-Dist: cibuildwheel; extra == "build"
 Requires-Dist: wheel; extra == "build"
 Provides-Extra: test
-Requires-Dist: cryptography==38.0.3; extra == "test"
+Requires-Dist: charset_normalizer<4.0,>=3.3.2; extra == "test"
+Requires-Dist: cryptography<43.0,>=42.0.5; extra == "test"
+Requires-Dist: fastapi<1.0,==0.110.0; extra == "test"
 Requires-Dist: httpx==0.23.1; extra == "test"
-Requires-Dist: types-certifi==2021.10.8.2; extra == "test"
-Requires-Dist: pytest==7.1.2; extra == "test"
-Requires-Dist: pytest-asyncio==0.19.0; extra == "test"
-Requires-Dist: pytest-trio==0.7.0; extra == "test"
-Requires-Dist: trio==0.21.0; extra == "test"
-Requires-Dist: trio-typing==0.7.0; extra == "test"
-Requires-Dist: trustme==0.9.0; extra == "test"
-Requires-Dist: uvicorn==0.18.3; extra == "test"
-Requires-Dist: proxy.py==2.4.3; extra == "test"
-Requires-Dist: websockets==11.0.3; extra == "test"
-Requires-Dist: python-multipart==0.0.6; extra == "test"
-Requires-Dist: fastapi==0.100.0; extra == "test"
+Requires-Dist: proxy.py<3.0,>=2.4.3; extra == "test"
+Requires-Dist: pytest<9.0,>=8.1.1; extra == "test"
+Requires-Dist: pytest-asyncio<1.0,>=0.23.6; extra == "test"
+Requires-Dist: pytest-trio<1.0,>=0.8.0; extra == "test"
+Requires-Dist: python-multipart<1.0,>=0.0.9; extra == "test"
+Requires-Dist: trio<1.0,>=0.25.0; extra == "test"
+Requires-Dist: trustme<2.0,>=1.1.0; extra == "test"
+Requires-Dist: uvicorn<1.0,>=0.29.0; extra == "test"
+Requires-Dist: websockets<13.0,>=12.0; extra == "test"
 
 # curl_cffi
 
 [![Downloads](https://static.pepy.tech/badge/curl_cffi/week)](https://pepy.tech/project/curl_cffi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/curl_cffi)
 [![PyPI version](https://badge.fury.io/py/curl-cffi.svg)](https://badge.fury.io/py/curl-cffi)
+[![Generic badge](https://img.shields.io/badge/Telegram%20Group-join-blue?logo=telegram)](https://t.me/+lL9n33eZp480MGM1)
+[![Generic badge](https://img.shields.io/badge/微信交流群-加入-brightgreen?logo=wechat)](./assets/wechat.jpg)
 
-[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) | [Discuss on Telegram](https://t.me/+lL9n33eZp480MGM1)
+[Documentation](https://curl-cffi.readthedocs.io) | [中文 README](https://github.com/yifeikong/curl_cffi/blob/main/README-zh.md) 
 
 Python binding for [curl-impersonate](https://github.com/lwthiker/curl-impersonate)
 via [cffi](https://cffi.readthedocs.io/en/latest/).
 
 Unlike other pure python http clients like `httpx` or `requests`, `curl_cffi` can
 impersonate browsers' TLS/JA3 and HTTP/2 fingerprints. If you are blocked by some
 website for no obvious reason, you can give `curl_cffi` a try.
@@ -197,34 +193,40 @@
 # {'cookies': {'foo': 'bar'}}
 ```
 
 Supported impersonate versions, as supported by my [fork](https://github.com/yifeikong/curl-impersonate) of [curl-impersonate](https://github.com/lwthiker/curl-impersonate):
 
 However, only Chrome-like browsers are supported. Firefox support is tracked in [#59](https://github.com/yifeikong/curl_cffi/issues/59).
 
+Browser versions will be added **only** when their fingerprints change. If you see a version, e.g.
+chrome122, were skipped, you can simply impersonate it with your own headers and the previous version.
+
 - chrome99
 - chrome100
 - chrome101
 - chrome104
 - chrome107
 - chrome110
 - chrome116 <sup>[1]</sup>
 - chrome119 <sup>[1]</sup>
 - chrome120 <sup>[1]</sup>
+- chrome123 <sup>[3]</sup>
+- chrome124 <sup>[3]</sup>
 - chrome99_android
 - edge99
 - edge101
 - safari15_3 <sup>[2]</sup>
 - safari15_5 <sup>[2]</sup>
 - safari17_0 <sup>[1]</sup>
 - safari17_2_ios <sup>[1]</sup>
 
 Notes:
 1. Added in version `0.6.0`.
 2. Fixed in version `0.6.0`, previous http2 fingerprints were [not correct](https://github.com/lwthiker/curl-impersonate/issues/215).
+3. Added in version `0.7.0`.
 
 ### asyncio
 
 ```python
 from curl_cffi.requests import AsyncSession
 
 async with AsyncSession() as s:
```

### Comparing `curl_cffi-0.6.3b1/curl_cffi.egg-info/SOURCES.txt` & `curl_cffi-0.7.0b4/curl_cffi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 curl_cffi/__init__.py
 curl_cffi/__version__.py
 curl_cffi/_asyncio_selector.py
 curl_cffi/aio.py
 curl_cffi/const.py
 curl_cffi/curl.py
+curl_cffi/py.typed
 curl_cffi.egg-info/PKG-INFO
 curl_cffi.egg-info/SOURCES.txt
 curl_cffi.egg-info/dependency_links.txt
 curl_cffi.egg-info/requires.txt
 curl_cffi.egg-info/top_level.txt
 curl_cffi/requests/__init__.py
 curl_cffi/requests/cookies.py
```

### Comparing `curl_cffi-0.6.3b1/ffi/cdef.c` & `curl_cffi-0.7.0b4/ffi/cdef.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/ffi/shim.c` & `curl_cffi-0.7.0b4/ffi/shim.c`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/Makefile.am` & `curl_cffi-0.7.0b4/include/curl/Makefile.am`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/Makefile.in` & `curl_cffi-0.7.0b4/include/curl/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 ACLOCAL_M4 = $(top_srcdir)/aclocal.m4
 am__aclocal_m4_deps = $(top_srcdir)/m4/curl-amissl.m4 \
 	$(top_srcdir)/m4/curl-bearssl.m4 \
 	$(top_srcdir)/m4/curl-compilers.m4 \
 	$(top_srcdir)/m4/curl-confopts.m4 \
 	$(top_srcdir)/m4/curl-functions.m4 \
 	$(top_srcdir)/m4/curl-gnutls.m4 \
-	$(top_srcdir)/m4/curl-mbedtls.m4 $(top_srcdir)/m4/curl-nss.m4 \
+	$(top_srcdir)/m4/curl-mbedtls.m4 \
 	$(top_srcdir)/m4/curl-openssl.m4 \
 	$(top_srcdir)/m4/curl-override.m4 \
 	$(top_srcdir)/m4/curl-reentrant.m4 \
 	$(top_srcdir)/m4/curl-rustls.m4 \
 	$(top_srcdir)/m4/curl-schannel.m4 \
 	$(top_srcdir)/m4/curl-sectransp.m4 \
 	$(top_srcdir)/m4/curl-sysconfig.m4 \
@@ -290,15 +290,14 @@
 MAKEINFO = @MAKEINFO@
 MANIFEST_TOOL = @MANIFEST_TOOL@
 MANOPT = @MANOPT@
 MKDIR_P = @MKDIR_P@
 NM = @NM@
 NMEDIT = @NMEDIT@
 NROFF = @NROFF@
-NSS_LIBS = @NSS_LIBS@
 OBJDUMP = @OBJDUMP@
 OBJEXT = @OBJEXT@
 OTOOL = @OTOOL@
 OTOOL64 = @OTOOL64@
 PACKAGE = @PACKAGE@
 PACKAGE_BUGREPORT = @PACKAGE_BUGREPORT@
 PACKAGE_NAME = @PACKAGE_NAME@
@@ -335,17 +334,16 @@
 USE_LIBSSH2 = @USE_LIBSSH2@
 USE_MBEDTLS = @USE_MBEDTLS@
 USE_MSH3 = @USE_MSH3@
 USE_NGHTTP2 = @USE_NGHTTP2@
 USE_NGHTTP3 = @USE_NGHTTP3@
 USE_NGTCP2 = @USE_NGTCP2@
 USE_NGTCP2_CRYPTO_GNUTLS = @USE_NGTCP2_CRYPTO_GNUTLS@
-USE_NGTCP2_CRYPTO_OPENSSL = @USE_NGTCP2_CRYPTO_OPENSSL@
+USE_NGTCP2_CRYPTO_QUICTLS = @USE_NGTCP2_CRYPTO_QUICTLS@
 USE_NGTCP2_CRYPTO_WOLFSSL = @USE_NGTCP2_CRYPTO_WOLFSSL@
-USE_NSS = @USE_NSS@
 USE_OPENLDAP = @USE_OPENLDAP@
 USE_QUICHE = @USE_QUICHE@
 USE_RUSTLS = @USE_RUSTLS@
 USE_SCHANNEL = @USE_SCHANNEL@
 USE_SECTRANSP = @USE_SECTRANSP@
 USE_UNIX_SOCKETS = @USE_UNIX_SOCKETS@
 USE_WIN32_CRYPTO = @USE_WIN32_CRYPTO@
```

### Comparing `curl_cffi-0.6.3b1/include/curl/curl.h` & `curl_cffi-0.7.0b4/include/curl/curl.h`

 * *Files 0% similar despite different names*

```diff
@@ -49,63 +49,54 @@
 #define CURL_DEPRECATED(version, message)
 #define CURL_IGNORE_DEPRECATION(statements)     statements
 #endif
 
 #include "curlver.h"         /* libcurl version defines   */
 #include "system.h"          /* determine things run-time */
 
-/*
- * Define CURL_WIN32 when build target is Win32 API
- */
-
-#if (defined(_WIN32) || defined(__WIN32__) || defined(WIN32)) &&        \
-  !defined(__SYMBIAN32__)
-#define CURL_WIN32
-#endif
-
 #include <stdio.h>
 #include <limits.h>
 
-#if (defined(__FreeBSD__) && (__FreeBSD__ >= 2)) || defined(__MidnightBSD__)
+#if defined(__FreeBSD__) || defined(__MidnightBSD__)
 /* Needed for __FreeBSD_version or __MidnightBSD_version symbol definition */
-#include <osreldate.h>
+#include <sys/param.h>
 #endif
 
 /* The include stuff here below is mainly for time_t! */
 #include <sys/types.h>
 #include <time.h>
 
-#if defined(CURL_WIN32) && !defined(_WIN32_WCE) && !defined(__CYGWIN__)
+#if defined(_WIN32) && !defined(_WIN32_WCE) && !defined(__CYGWIN__)
 #if !(defined(_WINSOCKAPI_) || defined(_WINSOCK_H) || \
       defined(__LWIP_OPT_H__) || defined(LWIP_HDR_OPT_H))
 /* The check above prevents the winsock2 inclusion if winsock.h already was
    included, since they can't co-exist without problems */
 #include <winsock2.h>
 #include <ws2tcpip.h>
 #endif
 #endif
 
 /* HP-UX systems version 9, 10 and 11 lack sys/select.h and so does oldish
    libc5-based Linux systems. Only include it on systems that are known to
    require it! */
 #if defined(_AIX) || defined(__NOVELL_LIBC__) || defined(__NetBSD__) || \
-    defined(__minix) || defined(__SYMBIAN32__) || defined(__INTEGRITY) || \
+    defined(__minix) || defined(__INTEGRITY) || \
     defined(ANDROID) || defined(__ANDROID__) || defined(__OpenBSD__) || \
     defined(__CYGWIN__) || defined(AMIGA) || defined(__NuttX__) || \
    (defined(__FreeBSD_version) && (__FreeBSD_version < 800000)) || \
    (defined(__MidnightBSD_version) && (__MidnightBSD_version < 100000)) || \
-    defined(__sun__) || defined(__serenity__)
+    defined(__sun__) || defined(__serenity__) || defined(__vxworks__)
 #include <sys/select.h>
 #endif
 
-#if !defined(CURL_WIN32) && !defined(_WIN32_WCE)
+#if !defined(_WIN32) && !defined(_WIN32_WCE)
 #include <sys/socket.h>
 #endif
 
-#if !defined(CURL_WIN32)
+#if !defined(_WIN32)
 #include <sys/time.h>
 #endif
 
 /* Compatibility for non-Clang compilers */
 #ifndef __has_declspec_attribute
 #  define __has_declspec_attribute(x) 0
 #endif
@@ -124,15 +115,15 @@
 
 /*
  * libcurl external API function linkage decorations.
  */
 
 #ifdef CURL_STATICLIB
 #  define CURL_EXTERN
-#elif defined(CURL_WIN32) || defined(__SYMBIAN32__) || \
+#elif defined(_WIN32) || \
      (__has_declspec_attribute(dllexport) && \
       __has_declspec_attribute(dllimport))
 #  if defined(BUILDING_LIBCURL)
 #    define CURL_EXTERN  __declspec(dllexport)
 #  else
 #    define CURL_EXTERN  __declspec(dllimport)
 #  endif
@@ -140,32 +131,32 @@
 #  define CURL_EXTERN CURL_EXTERN_SYMBOL
 #else
 #  define CURL_EXTERN
 #endif
 
 #ifndef curl_socket_typedef
 /* socket typedef */
-#if defined(CURL_WIN32) && !defined(__LWIP_OPT_H__) && !defined(LWIP_HDR_OPT_H)
+#if defined(_WIN32) && !defined(__LWIP_OPT_H__) && !defined(LWIP_HDR_OPT_H)
 typedef SOCKET curl_socket_t;
 #define CURL_SOCKET_BAD INVALID_SOCKET
 #else
 typedef int curl_socket_t;
 #define CURL_SOCKET_BAD -1
 #endif
 #define curl_socket_typedef
 #endif /* curl_socket_typedef */
 
 /* enum for the different supported SSL backends */
 typedef enum {
   CURLSSLBACKEND_NONE = 0,
   CURLSSLBACKEND_OPENSSL = 1,
   CURLSSLBACKEND_GNUTLS = 2,
-  CURLSSLBACKEND_NSS = 3,
+  CURLSSLBACKEND_NSS                    CURL_DEPRECATED(8.3.0, "") = 3,
   CURLSSLBACKEND_OBSOLETE4 = 4,  /* Was QSOSSL. */
-  CURLSSLBACKEND_GSKIT = 5,
+  CURLSSLBACKEND_GSKIT                  CURL_DEPRECATED(8.3.0, "") = 5,
   CURLSSLBACKEND_POLARSSL               CURL_DEPRECATED(7.69.0, "") = 6,
   CURLSSLBACKEND_WOLFSSL = 7,
   CURLSSLBACKEND_SCHANNEL = 8,
   CURLSSLBACKEND_SECURETRANSPORT = 9,
   CURLSSLBACKEND_AXTLS                  CURL_DEPRECATED(7.61.0, "") = 10,
   CURLSSLBACKEND_MBEDTLS = 11,
   CURLSSLBACKEND_MESALINK               CURL_DEPRECATED(7.82.0, "") = 12,
@@ -643,18 +634,18 @@
   CURLE_ECH_REQUIRED      ,      /* 100 - ECH tried but failed */
   CURL_LAST /* never use! */
 } CURLcode;
 
 #ifndef CURL_NO_OLDIES /* define this to test if your app builds with all
                           the obsolete stuff removed! */
 
-/* Previously obsolete error code re-used in 7.38.0 */
+/* Previously obsolete error code reused in 7.38.0 */
 #define CURLE_OBSOLETE16 CURLE_HTTP2
 
-/* Previously obsolete error codes re-used in 7.24.0 */
+/* Previously obsolete error codes reused in 7.24.0 */
 #define CURLE_OBSOLETE10 CURLE_FTP_ACCEPT_FAILED
 #define CURLE_OBSOLETE12 CURLE_FTP_ACCEPT_TIMEOUT
 
 /*  compatibility with older names */
 #define CURLOPT_ENCODING CURLOPT_ACCEPT_ENCODING
 #define CURLE_FTP_WEIRD_SERVER_REPLY CURLE_WEIRD_SERVER_REPLY
 
@@ -778,15 +769,15 @@
 
 typedef enum {
   CURLPROXY_HTTP = 0,   /* added in 7.10, new in 7.19.4 default is to use
                            CONNECT HTTP/1.1 */
   CURLPROXY_HTTP_1_0 = 1,   /* added in 7.19.4, force to use CONNECT
                                HTTP/1.0  */
   CURLPROXY_HTTPS = 2,  /* HTTPS but stick to HTTP/1 added in 7.52.0 */
-  CURLPROXY_HTTPS2 = 3, /* HTTPS and attempt HTTP/2 added in 8.1.0 */
+  CURLPROXY_HTTPS2 = 3, /* HTTPS and attempt HTTP/2 added in 8.2.0 */
   CURLPROXY_SOCKS4 = 4, /* support added in 7.15.2, enum existed already
                            in 7.10 */
   CURLPROXY_SOCKS5 = 5, /* added in 7.10 */
   CURLPROXY_SOCKS4A = 6, /* added in 7.18.0 */
   CURLPROXY_SOCKS5_HOSTNAME = 7 /* Use the SOCKS5 protocol but pass along the
                                    host name rather than the IP address. added
                                    in 7.18.0 */
@@ -1355,15 +1346,15 @@
   /* 73 = OBSOLETE */
 
   /* Set to explicitly use a new connection for the upcoming transfer.
      Do not use this unless you're absolutely sure of this, as it makes the
      operation slower and is less friendly for the network. */
   CURLOPT(CURLOPT_FRESH_CONNECT, CURLOPTTYPE_LONG, 74),
 
-  /* Set to explicitly forbid the upcoming transfer's connection to be re-used
+  /* Set to explicitly forbid the upcoming transfer's connection to be reused
      when done. Do not use this unless you're absolutely sure of this, as it
      makes the operation slower and is less friendly for the network. */
   CURLOPT(CURLOPT_FORBID_REUSE, CURLOPTTYPE_LONG, 75),
 
   /* Set to a file name that contains random data for libcurl to use to
      seed the random engine when doing SSL connects. */
   CURLOPTDEPRECATED(CURLOPT_RANDOM_FILE, CURLOPTTYPE_STRINGPOINT, 76,
@@ -1649,15 +1640,15 @@
   /* Pointer to command string to send if USER/PASS fails. */
   CURLOPT(CURLOPT_FTP_ALTERNATIVE_TO_USER, CURLOPTTYPE_STRINGPOINT, 147),
 
   /* callback function for setting socket options */
   CURLOPT(CURLOPT_SOCKOPTFUNCTION, CURLOPTTYPE_FUNCTIONPOINT, 148),
   CURLOPT(CURLOPT_SOCKOPTDATA, CURLOPTTYPE_CBPOINT, 149),
 
-  /* set to 0 to disable session ID re-use for this transfer, default is
+  /* set to 0 to disable session ID reuse for this transfer, default is
      enabled (== 1) */
   CURLOPT(CURLOPT_SSL_SESSIONID_CACHE, CURLOPTTYPE_LONG, 150),
 
   /* allowed SSH authentication methods */
   CURLOPT(CURLOPT_SSH_AUTH_TYPES, CURLOPTTYPE_VALUES, 151),
 
   /* Used by scp/sftp to do public/private key authentication */
@@ -2110,15 +2101,15 @@
    * (in seconds) */
   CURLOPT(CURLOPT_MAXAGE_CONN, CURLOPTTYPE_LONG, 288),
 
   /* SASL authorization identity */
   CURLOPT(CURLOPT_SASL_AUTHZID, CURLOPTTYPE_STRINGPOINT, 289),
 
   /* allow RCPT TO command to fail for some recipients */
-  CURLOPT(CURLOPT_MAIL_RCPT_ALLLOWFAILS, CURLOPTTYPE_LONG, 290),
+  CURLOPT(CURLOPT_MAIL_RCPT_ALLOWFAILS, CURLOPTTYPE_LONG, 290),
 
   /* the private SSL-certificate as a "blob" */
   CURLOPT(CURLOPT_SSLCERT_BLOB, CURLOPTTYPE_BLOB, 291),
   CURLOPT(CURLOPT_SSLKEY_BLOB, CURLOPTTYPE_BLOB, 292),
   CURLOPT(CURLOPT_PROXY_SSLCERT_BLOB, CURLOPTTYPE_BLOB, 293),
   CURLOPT(CURLOPT_PROXY_SSLKEY_BLOB, CURLOPTTYPE_BLOB, 294),
   CURLOPT(CURLOPT_ISSUERCERT_BLOB, CURLOPTTYPE_BLOB, 295),
@@ -2204,66 +2195,87 @@
 
   /* CA cache timeout */
   CURLOPT(CURLOPT_CA_CACHE_TIMEOUT, CURLOPTTYPE_LONG, 321),
 
   /* Can leak things, gonna exit() soon */
   CURLOPT(CURLOPT_QUICK_EXIT, CURLOPTTYPE_LONG, 322),
 
+  /* set a specific client IP for HAProxy PROXY protocol header? */
+  CURLOPT(CURLOPT_HAPROXY_CLIENT_IP, CURLOPTTYPE_STRINGPOINT, 323),
+
   /* curl-impersonate: A list of headers used by the impersonated browser.
    * If given, merged with CURLOPT_HTTPHEADER. */
-  CURLOPT(CURLOPT_HTTPBASEHEADER, CURLOPTTYPE_SLISTPOINT, 323),
+  CURLOPT(CURLOPT_HTTPBASEHEADER, CURLOPTTYPE_SLISTPOINT, 324),
 
   /* curl-impersonate: A list of TLS signature hash algorithms.
    * See https://datatracker.ietf.org/doc/html/rfc5246#section-7.4.1.4.1 */
-  CURLOPT(CURLOPT_SSL_SIG_HASH_ALGS, CURLOPTTYPE_STRINGPOINT, 324),
+  CURLOPT(CURLOPT_SSL_SIG_HASH_ALGS, CURLOPTTYPE_STRINGPOINT, 325),
 
   /* curl-impersonate: Whether to enable ALPS in TLS or not.
    * See https://datatracker.ietf.org/doc/html/draft-vvv-tls-alps.
    * Support for ALPS is minimal and is intended only for the TLS client
    * hello to match. */
-  CURLOPT(CURLOPT_SSL_ENABLE_ALPS, CURLOPTTYPE_LONG, 325),
+  CURLOPT(CURLOPT_SSL_ENABLE_ALPS, CURLOPTTYPE_LONG, 326),
 
   /* curl-impersonate: Comma-separated list of certificate compression
    * algorithms to use. These are published in the client hello.
    * Supported algorithms are "zlib" and "brotli".
    * See https://datatracker.ietf.org/doc/html/rfc8879 */
-  CURLOPT(CURLOPT_SSL_CERT_COMPRESSION, CURLOPTTYPE_STRINGPOINT, 326),
+  CURLOPT(CURLOPT_SSL_CERT_COMPRESSION, CURLOPTTYPE_STRINGPOINT, 327),
 
   /* Enable/disable TLS session ticket extension (RFC5077) */
-  CURLOPT(CURLOPT_SSL_ENABLE_TICKET, CURLOPTTYPE_LONG, 327),
+  CURLOPT(CURLOPT_SSL_ENABLE_TICKET, CURLOPTTYPE_LONG, 328),
 
   /*
    * curl-impersonate:
    * Set the order of the HTTP/2 pseudo headers. The value must contain
    * the letters 'm', 'a', 's', 'p' representing the pseudo-headers
    * ":method", ":authority", ":scheme", ":path" in the desired order of
    * appearance in the HTTP/2 HEADERS frame.
    */
-  CURLOPT(CURLOPT_HTTP2_PSEUDO_HEADERS_ORDER, CURLOPTTYPE_STRINGPOINT, 328),
+  CURLOPT(CURLOPT_HTTP2_PSEUDO_HEADERS_ORDER, CURLOPTTYPE_STRINGPOINT, 329),
 
   /*
    * curl-impersonate:
    * HTTP2 settings frame keys and values, format: 1:v;2:v;3:v
    */
-  CURLOPT(CURLOPT_HTTP2_SETTINGS, CURLOPTTYPE_STRINGPOINT, 329),
+  CURLOPT(CURLOPT_HTTP2_SETTINGS, CURLOPTTYPE_STRINGPOINT, 330),
 
   /* 
    * curl-impersonate: Whether to enable Boringssl permute extensions
    * See https://commondatastorage.googleapis.com/chromium-boringssl-docs/ssl.h.html#SSL_set_permute_extensions.
    */
-  CURLOPT(CURLOPT_SSL_PERMUTE_EXTENSIONS, CURLOPTTYPE_LONG, 330),
+  CURLOPT(CURLOPT_SSL_PERMUTE_EXTENSIONS, CURLOPTTYPE_LONG, 331),
 
   /*
    * curl-impersonate:
    * HTTP2 initial window update
    */
-  CURLOPT(CURLOPT_HTTP2_WINDOW_UPDATE, CURLOPTTYPE_LONG, 331),
+  CURLOPT(CURLOPT_HTTP2_WINDOW_UPDATE, CURLOPTTYPE_LONG, 332),
+
+  /* curl-impersonate:
+   * set ECH configuration, XXX, the official one is 324
+   */
+  CURLOPT(CURLOPT_ECH, CURLOPTTYPE_STRINGPOINT, 333),
+
+  /*
+   * curl-impersonate:
+   * Set the initial streams settings for http2.
+   */
+  CURLOPT(CURLOPT_HTTP2_STREAMS, CURLOPTTYPE_STRINGPOINT, 334),
+
+  /* curl-impersonate:
+   * enable tls grease
+   */
+  CURLOPT(CURLOPT_TLS_GREASE, CURLOPTTYPE_LONG, 335),
 
-  /* set ECH configuration, XXX, the official one is 324  */
-  CURLOPT(CURLOPT_ECH, CURLOPTTYPE_STRINGPOINT, 332),
+  /* curl-impersonate:
+   * set tls extension order
+   */
+  CURLOPT(CURLOPT_TLS_EXTENSION_ORDER, CURLOPTTYPE_STRINGPOINT, 336),
 
   CURLOPT_LASTENTRY /* the last unused */
 } CURLoption;
 
 #ifndef CURL_NO_OLDIES /* define this to test if your app builds with all
                           the obsolete stuff removed! */
 
@@ -2285,14 +2297,17 @@
 
 #define CURLOPT_SSLCERTPASSWD CURLOPT_KEYPASSWD
 #define CURLOPT_KRB4LEVEL CURLOPT_KRBLEVEL
 
 /* */
 #define CURLOPT_FTP_RESPONSE_TIMEOUT CURLOPT_SERVER_RESPONSE_TIMEOUT
 
+/* Added in 8.2.0 */
+#define CURLOPT_MAIL_RCPT_ALLLOWFAILS CURLOPT_MAIL_RCPT_ALLOWFAILS
+
 #else
 /* This is set if CURL_NO_OLDIES is defined at compile-time */
 #undef CURLOPT_DNS_USE_GLOBAL_CACHE /* soon obsolete */
 #endif
 
 
   /* Below here follows defines for the CURLOPT_IPRESOLVE option. If a host
@@ -2775,14 +2790,28 @@
  * DESCRIPTION
  *
  * curl_global_cleanup() should be invoked exactly once for each application
  * that uses libcurl
  */
 CURL_EXTERN void curl_global_cleanup(void);
 
+/*
+ * NAME curl_global_trace()
+ *
+ * DESCRIPTION
+ *
+ * curl_global_trace() can be invoked at application start to
+ * configure which components in curl should participate in tracing.
+
+ * This function is thread-safe if CURL_VERSION_THREADSAFE is set in the
+ * curl_version_info_data.features flag (fetch by curl_version_info()).
+
+ */
+CURL_EXTERN CURLcode curl_global_trace(const char *config);
+
 /* linked-list structure for the CURLOPT_QUOTE option (and other) */
 struct curl_slist {
   char *data;
   struct curl_slist *next;
 };
 
 /*
@@ -2854,21 +2883,22 @@
  *
  * Returns the time, in seconds since 1 Jan 1970 of the time string given in
  * the first argument. The time argument in the second parameter is unused
  * and should be set to NULL.
  */
 CURL_EXTERN time_t curl_getdate(const char *p, const time_t *unused);
 
-/* info about the certificate chain, only for OpenSSL, GnuTLS, Schannel, NSS
-   and GSKit builds. Asked for with CURLOPT_CERTINFO / CURLINFO_CERTINFO */
+/* info about the certificate chain, for SSL backends that support it. Asked
+   for with CURLOPT_CERTINFO / CURLINFO_CERTINFO */
 struct curl_certinfo {
   int num_of_certs;             /* number of certificates with information */
   struct curl_slist **certinfo; /* for each index in this array, there's a
-                                   linked list with textual information in the
-                                   format "name: value" */
+                                   linked list with textual information for a
+                                   certificate in the format "name:content".
+                                   eg "Subject:foo", "Issuer:bar", etc. */
 };
 
 /* Information about the SSL library used and the respective internal SSL
    handle, which can be used to obtain further information regarding the
    connection. Asked for with CURLINFO_TLS_SSL_PTR or CURLINFO_TLS_SESSION. */
 struct curl_tlssessioninfo {
   curl_sslbackend backend;
@@ -2968,15 +2998,17 @@
   CURLINFO_APPCONNECT_TIME_T = CURLINFO_OFF_T + 56,
   CURLINFO_RETRY_AFTER      = CURLINFO_OFF_T + 57,
   CURLINFO_EFFECTIVE_METHOD = CURLINFO_STRING + 58,
   CURLINFO_PROXY_ERROR      = CURLINFO_LONG + 59,
   CURLINFO_REFERER          = CURLINFO_STRING + 60,
   CURLINFO_CAINFO           = CURLINFO_STRING + 61,
   CURLINFO_CAPATH           = CURLINFO_STRING + 62,
-  CURLINFO_LASTONE          = 62
+  CURLINFO_XFER_ID          = CURLINFO_OFF_T + 63,
+  CURLINFO_CONN_ID          = CURLINFO_OFF_T + 64,
+  CURLINFO_LASTONE          = 64
 } CURLINFO;
 
 /* CURLINFO_RESPONSE_CODE is the new name for the option previously known as
    CURLINFO_HTTP_CODE */
 #define CURLINFO_HTTP_CODE CURLINFO_RESPONSE_CODE
 
 typedef enum {
@@ -3247,14 +3279,15 @@
   stuff before they can be included! */
 #include "easy.h" /* nothing in curl is fun without the easy stuff */
 #include "multi.h"
 #include "urlapi.h"
 #include "options.h"
 #include "header.h"
 #include "websockets.h"
+#include "mprintf.h"
 
 /* the typechecker doesn't work in C++ (yet) */
 #if defined(__GNUC__) && defined(__GNUC_MINOR__) && \
     ((__GNUC__ > 4) || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3)) && \
     !defined(__cplusplus) && !defined(CURL_DISABLE_TYPECHECK)
 #include "typecheck-gcc.h"
 #else
```

### Comparing `curl_cffi-0.6.3b1/include/curl/curlver.h` & `curl_cffi-0.7.0b4/include/curl/curlver.h`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,21 @@
    a script at release-time. This was made its own header file in 7.11.2 */
 
 /* This is the global package copyright */
 #define LIBCURL_COPYRIGHT "Daniel Stenberg, <daniel@haxx.se>."
 
 /* This is the version number of the libcurl package from which this header
    file origins: */
-#define LIBCURL_VERSION "8.1.1"
+#define LIBCURL_VERSION "8.5.0"
 
 /* The numeric version number is also available "in parts" by using these
    defines: */
 #define LIBCURL_VERSION_MAJOR 8
-#define LIBCURL_VERSION_MINOR 1
-#define LIBCURL_VERSION_PATCH 1
+#define LIBCURL_VERSION_MINOR 5
+#define LIBCURL_VERSION_PATCH 0
 
 /* This is the numeric version of the libcurl version number, meant for easier
    parsing and comparisons by programs. The LIBCURL_VERSION_NUM define will
    always follow this syntax:
 
          0xXXYYZZ
 
@@ -55,25 +55,25 @@
    and it is always a greater number in a more recent release. It makes
    comparisons with greater than and less than work.
 
    Note: This define is the full hex number and _does not_ use the
    CURL_VERSION_BITS() macro since curl's own configure script greps for it
    and needs it to contain the full number.
 */
-#define LIBCURL_VERSION_NUM 0x080101
+#define LIBCURL_VERSION_NUM 0x080500
 
 /*
  * This is the date and time when the full source package was created. The
  * timestamp is not stored in git, as the timestamp is properly set in the
  * tarballs by the maketgz script.
  *
  * The format of the date follows this template:
  *
  * "2007-11-23"
  */
-#define LIBCURL_TIMESTAMP "2023-05-23"
+#define LIBCURL_TIMESTAMP "2023-12-06"
 
 #define CURL_VERSION_BITS(x,y,z) ((x)<<16|(y)<<8|(z))
 #define CURL_AT_LEAST_VERSION(x,y,z) \
   (LIBCURL_VERSION_NUM >= CURL_VERSION_BITS(x, y, z))
 
 #endif /* CURLINC_CURLVER_H */
```

### Comparing `curl_cffi-0.6.3b1/include/curl/easy.h` & `curl_cffi-0.7.0b4/include/curl/easy.h`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/header.h` & `curl_cffi-0.7.0b4/include/curl/header.h`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/multi.h` & `curl_cffi-0.7.0b4/include/curl/multi.h`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 #define CURL_WAIT_POLLIN    0x0001
 #define CURL_WAIT_POLLPRI   0x0002
 #define CURL_WAIT_POLLOUT   0x0004
 
 struct curl_waitfd {
   curl_socket_t fd;
   short events;
-  short revents; /* not supported yet */
+  short revents;
 };
 
 /*
  * Name:    curl_multi_init()
  *
  * Desc:    initialize multi-style curl usage
  *
@@ -422,14 +422,25 @@
  *          (only) useful for curl_multi_socket uses.
  *
  * Returns: CURLM error code.
  */
 CURL_EXTERN CURLMcode curl_multi_assign(CURLM *multi_handle,
                                         curl_socket_t sockfd, void *sockp);
 
+/*
+ * Name:    curl_multi_get_handles()
+ *
+ * Desc:    Returns an allocated array holding all handles currently added to
+ *          the multi handle. Marks the final entry with a NULL pointer. If
+ *          there is no easy handle added to the multi handle, this function
+ *          returns an array with the first entry as a NULL pointer.
+ *
+ * Returns: NULL on failure, otherwise a CURL **array pointer
+ */
+CURL_EXTERN CURL **curl_multi_get_handles(CURLM *multi_handle);
 
 /*
  * Name: curl_push_callback
  *
  * Desc: This callback gets called when a new stream is being pushed by the
  *       server. It approves or denies the new stream. It can also decide
  *       to completely fail the connection.
```

### Comparing `curl_cffi-0.6.3b1/include/curl/options.h` & `curl_cffi-0.7.0b4/include/curl/options.h`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/stdcheaders.h` & `curl_cffi-0.7.0b4/include/curl/stdcheaders.h`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/include/curl/system.h` & `curl_cffi-0.7.0b4/include/curl/system.h`

 * *Files 1% similar despite different names*

```diff
@@ -137,37 +137,14 @@
 #    define CURL_FORMAT_CURL_OFF_T     "ld"
 #    define CURL_FORMAT_CURL_OFF_TU    "lu"
 #    define CURL_SUFFIX_CURL_OFF_T     L
 #    define CURL_SUFFIX_CURL_OFF_TU    UL
 #    define CURL_TYPEOF_CURL_SOCKLEN_T int
 #  endif
 
-#elif defined(__SYMBIAN32__)
-#  if defined(__EABI__) /* Treat all ARM compilers equally */
-#    define CURL_TYPEOF_CURL_OFF_T     long long
-#    define CURL_FORMAT_CURL_OFF_T     "lld"
-#    define CURL_FORMAT_CURL_OFF_TU    "llu"
-#    define CURL_SUFFIX_CURL_OFF_T     LL
-#    define CURL_SUFFIX_CURL_OFF_TU    ULL
-#  elif defined(__CW32__)
-#    pragma longlong on
-#    define CURL_TYPEOF_CURL_OFF_T     long long
-#    define CURL_FORMAT_CURL_OFF_T     "lld"
-#    define CURL_FORMAT_CURL_OFF_TU    "llu"
-#    define CURL_SUFFIX_CURL_OFF_T     LL
-#    define CURL_SUFFIX_CURL_OFF_TU    ULL
-#  elif defined(__VC32__)
-#    define CURL_TYPEOF_CURL_OFF_T     __int64
-#    define CURL_FORMAT_CURL_OFF_T     "lld"
-#    define CURL_FORMAT_CURL_OFF_TU    "llu"
-#    define CURL_SUFFIX_CURL_OFF_T     LL
-#    define CURL_SUFFIX_CURL_OFF_TU    ULL
-#  endif
-#  define CURL_TYPEOF_CURL_SOCKLEN_T unsigned int
-
 #elif defined(macintosh)
 #  include <ConditionalMacros.h>
 #  if TYPE_LONGLONG
 #    define CURL_TYPEOF_CURL_OFF_T     long long
 #    define CURL_FORMAT_CURL_OFF_T     "lld"
 #    define CURL_FORMAT_CURL_OFF_TU    "llu"
 #    define CURL_SUFFIX_CURL_OFF_T     LL
@@ -197,17 +174,18 @@
 #  define CURL_FORMAT_CURL_OFF_T     "I64d"
 #  define CURL_FORMAT_CURL_OFF_TU    "I64u"
 #  define CURL_SUFFIX_CURL_OFF_T     i64
 #  define CURL_SUFFIX_CURL_OFF_TU    ui64
 #  define CURL_TYPEOF_CURL_SOCKLEN_T int
 
 #elif defined(__MINGW32__)
+#  include <inttypes.h>
 #  define CURL_TYPEOF_CURL_OFF_T     long long
-#  define CURL_FORMAT_CURL_OFF_T     "I64d"
-#  define CURL_FORMAT_CURL_OFF_TU    "I64u"
+#  define CURL_FORMAT_CURL_OFF_T     PRId64
+#  define CURL_FORMAT_CURL_OFF_TU    PRIu64
 #  define CURL_SUFFIX_CURL_OFF_T     LL
 #  define CURL_SUFFIX_CURL_OFF_TU    ULL
 #  define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
 #  define CURL_PULL_SYS_TYPES_H      1
 #  define CURL_PULL_WS2TCPIP_H       1
 
 #elif defined(__VMS)
@@ -233,41 +211,36 @@
 #  define CURL_SUFFIX_CURL_OFF_T     LL
 #  define CURL_SUFFIX_CURL_OFF_TU    ULL
 #  define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
 #  define CURL_PULL_SYS_TYPES_H      1
 #  define CURL_PULL_SYS_SOCKET_H     1
 
 #elif defined(__MVS__)
-#  if defined(__IBMC__) || defined(__IBMCPP__)
-#    if defined(_ILP32)
-#    elif defined(_LP64)
-#    endif
-#    if defined(_LONG_LONG)
-#      define CURL_TYPEOF_CURL_OFF_T     long long
-#      define CURL_FORMAT_CURL_OFF_T     "lld"
-#      define CURL_FORMAT_CURL_OFF_TU    "llu"
-#      define CURL_SUFFIX_CURL_OFF_T     LL
-#      define CURL_SUFFIX_CURL_OFF_TU    ULL
-#    elif defined(_LP64)
-#      define CURL_TYPEOF_CURL_OFF_T     long
-#      define CURL_FORMAT_CURL_OFF_T     "ld"
-#      define CURL_FORMAT_CURL_OFF_TU    "lu"
-#      define CURL_SUFFIX_CURL_OFF_T     L
-#      define CURL_SUFFIX_CURL_OFF_TU    UL
-#    else
-#      define CURL_TYPEOF_CURL_OFF_T     long
-#      define CURL_FORMAT_CURL_OFF_T     "ld"
-#      define CURL_FORMAT_CURL_OFF_TU    "lu"
-#      define CURL_SUFFIX_CURL_OFF_T     L
-#      define CURL_SUFFIX_CURL_OFF_TU    UL
-#    endif
-#    define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
-#    define CURL_PULL_SYS_TYPES_H      1
-#    define CURL_PULL_SYS_SOCKET_H     1
+#  if defined(_LONG_LONG)
+#    define CURL_TYPEOF_CURL_OFF_T     long long
+#    define CURL_FORMAT_CURL_OFF_T     "lld"
+#    define CURL_FORMAT_CURL_OFF_TU    "llu"
+#    define CURL_SUFFIX_CURL_OFF_T     LL
+#    define CURL_SUFFIX_CURL_OFF_TU    ULL
+#  elif defined(_LP64)
+#    define CURL_TYPEOF_CURL_OFF_T     long
+#    define CURL_FORMAT_CURL_OFF_T     "ld"
+#    define CURL_FORMAT_CURL_OFF_TU    "lu"
+#    define CURL_SUFFIX_CURL_OFF_T     L
+#    define CURL_SUFFIX_CURL_OFF_TU    UL
+#  else
+#    define CURL_TYPEOF_CURL_OFF_T     long
+#    define CURL_FORMAT_CURL_OFF_T     "ld"
+#    define CURL_FORMAT_CURL_OFF_TU    "lu"
+#    define CURL_SUFFIX_CURL_OFF_T     L
+#    define CURL_SUFFIX_CURL_OFF_TU    UL
 #  endif
+#  define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
+#  define CURL_PULL_SYS_TYPES_H      1
+#  define CURL_PULL_SYS_SOCKET_H     1
 
 #elif defined(__370__)
 #  if defined(__IBMC__) || defined(__IBMCPP__)
 #    if defined(_ILP32)
 #    elif defined(_LP64)
 #    endif
 #    if defined(_LONG_LONG)
@@ -348,20 +321,45 @@
 #    define CURL_SUFFIX_CURL_OFF_T     L
 #    define CURL_SUFFIX_CURL_OFF_TU    UL
 #  endif
 #  define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
 #  define CURL_PULL_SYS_TYPES_H      1
 #  define CURL_PULL_SYS_SOCKET_H     1
 
+#elif defined(__hpux) /* HP aCC compiler */
+#  if !defined(_LP64)
+#    define CURL_TYPEOF_CURL_OFF_T     long long
+#    define CURL_FORMAT_CURL_OFF_T     "lld"
+#    define CURL_FORMAT_CURL_OFF_TU    "llu"
+#    define CURL_SUFFIX_CURL_OFF_T     LL
+#    define CURL_SUFFIX_CURL_OFF_TU    ULL
+#  else
+#    define CURL_TYPEOF_CURL_OFF_T     long
+#    define CURL_FORMAT_CURL_OFF_T     "ld"
+#    define CURL_FORMAT_CURL_OFF_TU    "lu"
+#    define CURL_SUFFIX_CURL_OFF_T     L
+#    define CURL_SUFFIX_CURL_OFF_TU    UL
+#  endif
+#  define CURL_TYPEOF_CURL_SOCKLEN_T socklen_t
+#  define CURL_PULL_SYS_TYPES_H      1
+#  define CURL_PULL_SYS_SOCKET_H     1
+
 /* ===================================== */
 /*    KEEP MSVC THE PENULTIMATE ENTRY    */
 /* ===================================== */
 
 #elif defined(_MSC_VER)
-#  if (_MSC_VER >= 900) && (_INTEGRAL_MAX_BITS >= 64)
+#  if (_MSC_VER >= 1800)
+#    include <inttypes.h>
+#    define CURL_TYPEOF_CURL_OFF_T     __int64
+#    define CURL_FORMAT_CURL_OFF_T     PRId64
+#    define CURL_FORMAT_CURL_OFF_TU    PRIu64
+#    define CURL_SUFFIX_CURL_OFF_T     i64
+#    define CURL_SUFFIX_CURL_OFF_TU    ui64
+#  elif (_MSC_VER >= 900) && (_INTEGRAL_MAX_BITS >= 64)
 #    define CURL_TYPEOF_CURL_OFF_T     __int64
 #    define CURL_FORMAT_CURL_OFF_T     "I64d"
 #    define CURL_FORMAT_CURL_OFF_TU    "I64u"
 #    define CURL_SUFFIX_CURL_OFF_T     i64
 #    define CURL_SUFFIX_CURL_OFF_TU    ui64
 #  else
 #    define CURL_TYPEOF_CURL_OFF_T     long
```

### Comparing `curl_cffi-0.6.3b1/include/curl/typecheck-gcc.h` & `curl_cffi-0.7.0b4/include/curl/typecheck-gcc.h`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
    (option) == CURLOPT_DOH_URL ||                                             \
    (option) == CURLOPT_ECH ||                                                 \
    (option) == CURLOPT_EGDSOCKET ||                                           \
    (option) == CURLOPT_FTP_ACCOUNT ||                                         \
    (option) == CURLOPT_FTP_ALTERNATIVE_TO_USER ||                             \
    (option) == CURLOPT_FTPPORT ||                                             \
    (option) == CURLOPT_HSTS ||                                                \
+   (option) == CURLOPT_HAPROXY_CLIENT_IP ||                                   \
    (option) == CURLOPT_INTERFACE ||                                           \
    (option) == CURLOPT_ISSUERCERT ||                                          \
    (option) == CURLOPT_KEYPASSWD ||                                           \
    (option) == CURLOPT_KRBLEVEL ||                                            \
    (option) == CURLOPT_LOGIN_OPTIONS ||                                       \
    (option) == CURLOPT_MAIL_AUTH ||                                           \
    (option) == CURLOPT_MAIL_FROM ||                                           \
```

### Comparing `curl_cffi-0.6.3b1/include/curl/urlapi.h` & `curl_cffi-0.7.0b4/include/curl/urlapi.h`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,16 @@
 #define CURLU_URLDECODE (1<<6)          /* URL decode on get */
 #define CURLU_URLENCODE (1<<7)          /* URL encode on set */
 #define CURLU_APPENDQUERY (1<<8)        /* append a form style part */
 #define CURLU_GUESS_SCHEME (1<<9)       /* legacy curl-style guessing */
 #define CURLU_NO_AUTHORITY (1<<10)      /* Allow empty authority when the
                                            scheme is unknown. */
 #define CURLU_ALLOW_SPACE (1<<11)       /* Allow spaces in the URL */
-#define CURLU_PUNYCODE (1<<12)          /* get the host name in pynycode */
+#define CURLU_PUNYCODE (1<<12)          /* get the host name in punycode */
+#define CURLU_PUNY2IDN (1<<13)          /* punycode => IDN conversion */
 
 typedef struct Curl_URL CURLU;
 
 /*
  * curl_url() creates a new CURLU handle and returns a pointer to it.
  * Must be freed with curl_url_cleanup().
  */
```

### Comparing `curl_cffi-0.6.3b1/include/curl/websockets.h` & `curl_cffi-0.7.0b4/include/curl/websockets.h`

 * *Files 13% similar despite different names*

```diff
@@ -50,35 +50,35 @@
  * DESCRIPTION
  *
  * Receives data from the websocket connection. Use after successful
  * curl_easy_perform() with CURLOPT_CONNECT_ONLY option.
  */
 CURL_EXTERN CURLcode curl_ws_recv(CURL *curl, void *buffer, size_t buflen,
                                   size_t *recv,
-                                  struct curl_ws_frame **metap);
+                                  const struct curl_ws_frame **metap);
 
-/* sendflags for curl_ws_send() */
+/* flags for curl_ws_send() */
 #define CURLWS_PONG       (1<<6)
 
 /*
- * NAME curl_easy_send()
+ * NAME curl_ws_send()
  *
  * DESCRIPTION
  *
  * Sends data over the websocket connection. Use after successful
  * curl_easy_perform() with CURLOPT_CONNECT_ONLY option.
  */
 CURL_EXTERN CURLcode curl_ws_send(CURL *curl, const void *buffer,
                                   size_t buflen, size_t *sent,
-                                  curl_off_t framesize,
-                                  unsigned int sendflags);
+                                  curl_off_t fragsize,
+                                  unsigned int flags);
 
 /* bits for the CURLOPT_WS_OPTIONS bitmask: */
 #define CURLWS_RAW_MODE (1<<0)
 
-CURL_EXTERN struct curl_ws_frame *curl_ws_meta(CURL *curl);
+CURL_EXTERN const struct curl_ws_frame *curl_ws_meta(CURL *curl);
 
 #ifdef  __cplusplus
 }
 #endif
 
 #endif /* CURLINC_WEBSOCKETS_H */
```

### Comparing `curl_cffi-0.6.3b1/libs.json` & `curl_cffi-0.7.0b4/libs.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9696969696969698%*

 * *Differences: {'10': "{'libdir': ''}",*

 * * '4': "{'libdir': ''}",*

 * * '5': "{'libdir': ''}",*

 * * '6': "{'libdir': ''}",*

 * * '7': "{'libdir': ''}",*

 * * '9': "{'libdir': ''}"}*

```diff
@@ -33,48 +33,48 @@
         "so_arch": "arm64",
         "so_name": "libcurl-impersonate-chrome.4.dylib",
         "sysname": "macos",
         "system": "Darwin"
     },
     {
         "libc": "gnu",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "x86_64",
         "pointer_size": 64,
         "so_arch": "x86_64",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
     },
     {
         "libc": "musl",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "x86_64",
         "pointer_size": 64,
         "so_arch": "x86_64",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
     },
     {
         "libc": "gnu",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "i686",
         "pointer_size": 32,
         "so_arch": "i386",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
     },
     {
         "libc": "gnu",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "aarch64",
         "pointer_size": 64,
         "so_arch": "aarch64",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
@@ -88,26 +88,26 @@
         "so_arch": "aarch64",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
     },
     {
         "libc": "gnueabihf",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "armv6l",
         "pointer_size": 32,
         "so_arch": "arm",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
     },
     {
         "libc": "gnueabihf",
-        "libdir": "~/.local/lib",
+        "libdir": "",
         "link_type": "static",
         "machine": "armv7l",
         "pointer_size": 32,
         "so_arch": "arm",
         "so_name": "libcurl-impersonate-chrome.so",
         "sysname": "linux",
         "system": "Linux"
```

### Comparing `curl_cffi-0.6.3b1/scripts/build.py` & `curl_cffi-0.7.0b4/scripts/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import json
 import os
 import platform
 import shutil
 import struct
+import tempfile
 from pathlib import Path
 from urllib.request import urlretrieve
 
 from cffi import FFI
 
 # this is the upstream libcurl-impersonate version
-__version__ = "0.6.2b2"
+__version__ = "0.7.0b4"
+
+tmpdir = None
 
 
 def detect_arch():
     with open(Path(__file__).parent.parent / "libs.json") as f:
         archs = json.loads(f.read())
 
     libc, _ = platform.libc_ver()
@@ -25,31 +28,36 @@
     for arch in archs:
         if (
             arch["system"] == uname.system
             and arch["machine"] == uname.machine
             and arch["pointer_size"] == pointer_size
             and ("libc" not in arch or arch.get("libc") == libc)
         ):
-            arch["libdir"] = os.path.expanduser(arch["libdir"])
+            if arch["libdir"]:
+                arch["libdir"] = os.path.expanduser(arch["libdir"])
+            else:
+                global tmpdir
+                tmpdir = tempfile.TemporaryDirectory()
+                arch["libdir"] = tmpdir.name
             return arch
     raise Exception(f"Unsupported arch: {uname}")
 
 
 arch = detect_arch()
+print(f"Using {arch['libdir']} to store libcurl-impersonate")
+
 
 def download_libcurl():
     if (Path(arch["libdir"]) / arch["so_name"]).exists():
         print(".so files already downloaded.")
         return
 
     file = "libcurl-impersonate.tar.gz"
-    if arch["system"] == "Linux":
-        sysname = "linux-" + arch["libc"]
-    else:
-        sysname = arch["sysname"]
+    sysname = "linux-" + arch["libc"] if arch["system"] == "Linux" else arch["sysname"]
+
     url = (
         f"https://github.com/yifeikong/curl-impersonate/releases/download/"
         f"v{__version__}/libcurl-impersonate-v{__version__}"
         f".{arch['so_arch']}-{sysname}.tar.gz"
     )
 
     print(f"Downloading libcurl-impersonate-chrome from {url}...")
@@ -58,37 +66,40 @@
     print("Unpacking downloaded files...")
     os.makedirs(arch["libdir"], exist_ok=True)
     shutil.unpack_archive(file, arch["libdir"])
 
     if arch["system"] == "Windows":
         shutil.copy2(f"{arch['libdir']}/libcurl.dll", "curl_cffi")
 
+
 def get_curl_archives():
     if arch["system"] == "Linux" and arch.get("link_type") == "static":
         # note that the order of libraries matters
         # https://stackoverflow.com/a/36581865
         return [
             f"{arch['libdir']}/libcurl-impersonate-chrome.a",
             f"{arch['libdir']}/libssl.a",
             f"{arch['libdir']}/libcrypto.a",
             f"{arch['libdir']}/libz.a",
+            f"{arch['libdir']}/libzstd.a",
             f"{arch['libdir']}/libnghttp2.a",
             f"{arch['libdir']}/libbrotlidec-static.a",
             f"{arch['libdir']}/libbrotlienc-static.a",
             f"{arch['libdir']}/libbrotlicommon-static.a",
         ]
     else:
         return []
 
+
 def get_curl_libraries():
     if arch["system"] == "Windows":
         return ["libcurl"]
-    elif arch["system"] == "Darwin":
-        return ["curl-impersonate-chrome"]
-    elif arch["system"] == "Linux" and arch.get("link_type") == "dynamic":
+    elif arch["system"] == "Darwin" or (
+        arch["system"] == "Linux" and arch.get("link_type") == "dynamic"
+    ):
         return ["curl-impersonate-chrome"]
     else:
         return []
 
 
 ffibuilder = FFI()
 system = platform.system()
@@ -109,17 +120,15 @@
     include_dirs=[
         str(root_dir / "include"),
         str(root_dir / "ffi"),
     ],
     sources=[
         str(root_dir / "ffi/shim.c"),
     ],
-    extra_compile_args=(
-        ["-Wno-implicit-function-declaration"] if system == "Darwin" else []
-    ),
+    extra_compile_args=(["-Wno-implicit-function-declaration"] if system == "Darwin" else []),
 )
 
 with open(root_dir / "ffi/cdef.c") as f:
     cdef_content = f.read()
     ffibuilder.cdef(cdef_content)
```

### Comparing `curl_cffi-0.6.3b1/setup.py` & `curl_cffi-0.7.0b4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,10 +13,10 @@
         return python, abi, plat
 
 
 setup(
     # this option is only valid in setup.py
     cffi_modules=["scripts/build.py:ffibuilder"],
     cmdclass={
-        "bdist_wheel": bdist_wheel_abi3,  # type: ignore
+        "bdist_wheel": bdist_wheel_abi3,
     },
 )
```

### Comparing `curl_cffi-0.6.3b1/tests/integration/test_fingerprints.py` & `curl_cffi-0.7.0b4/tests/integration/test_fingerprints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
-from curl_cffi import requests
 
+from curl_cffi import requests
 
 JA3_URL = "https://tls.browserleaks.com/json"
 # Copied from my browser on macOS
 CHROME_JA3_HASH = "53ff64ddf993ca882b70e1c82af5da49"
 # Edge 101 is the same as Chrome 101
 EDGE_JA3_HASH = "53ff64ddf993ca882b70e1c82af5da49"
 # Same as safari 16.x
@@ -30,9 +30,7 @@
     r = requests.get(JA3_URL, impersonate="safari15_5")
     assert r.json()["ja3_hash"] == SAFARI_JA3_HASH
 
 
 def test_impersonate_unknown():
     with pytest.raises(requests.RequestsError, match="not supported"):
         requests.get(JA3_URL, impersonate="unknown")
-
-
```

### Comparing `curl_cffi-0.6.3b1/tests/integration/test_httpbin.py` & `curl_cffi-0.7.0b4/tests/integration/test_httpbin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
-from curl_cffi import requests, CurlHttpVersion, CurlOpt
 
+from curl_cffi import CurlHttpVersion, CurlOpt, requests
 
 #######################################################################################
 # testing httpbin
 #######################################################################################
 
 
 def test_gzip():
```

### Comparing `curl_cffi-0.6.3b1/tests/threads/test_eventlet.py` & `curl_cffi-0.7.0b4/tests/threads/test_gevent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import eventlet
+from gevent import monkey
 
-eventlet.monkey_patch()
+monkey.patch_all()
 
-import threading
-import time
+import threading  #  noqa: E402
+import time  #  noqa: E402
 
-from curl_cffi import requests
+from curl_cffi import requests  #  noqa: E402
 
 
 def delay():
-    requests.get("http://192.168.64.5:8080/delay/2", thread="eventlet")
+    requests.get("http://192.168.64.5:8080/delay/2", thread="gevent")
 
 
 def delay_not_working():
     requests.get("http://192.168.64.5:8080/delay/2")
 
 
 def test_gevent_parallel(fn):
```

### Comparing `curl_cffi-0.6.3b1/tests/threads/test_gevent.py` & `curl_cffi-0.7.0b4/tests/threads/test_eventlet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from gevent import monkey
+import eventlet
 
-monkey.patch_all()
+eventlet.monkey_patch()
 
-import threading
-import time
+import threading  #  noqa: E402
+import time  #  noqa: E402
 
-from curl_cffi import requests
+from curl_cffi import requests  #  noqa: E402
 
 
 def delay():
-    requests.get("http://192.168.64.5:8080/delay/2", thread="gevent")
+    requests.get("http://192.168.64.5:8080/delay/2", thread="eventlet")
 
 
 def delay_not_working():
     requests.get("http://192.168.64.5:8080/delay/2")
 
 
 def test_gevent_parallel(fn):
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/conftest.py` & `curl_cffi-0.7.0b4/tests/unittest/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.serialization import (
     BestAvailableEncryption,
     Encoding,
     PrivateFormat,
     load_pem_private_key,
 )
-from fastapi import FastAPI, UploadFile, Form
+from fastapi import FastAPI, Form, UploadFile
 from httpx import URL
 from uvicorn.config import Config
 from uvicorn.main import Server
 
 ENVIRONMENT_VARIABLES = {
     "SSL_CERT_FILE",
     "SSL_CERT_DIR",
@@ -120,14 +120,16 @@
         await redirect_then_echo_headers(scope, receive, send)
     elif scope["path"].startswith("/json"):
         await hello_world_json(scope, receive, send)
     elif scope["path"].startswith("/incomplete_read"):
         await incomplete_read(scope, receive, send)
     elif scope["path"].startswith("/gbk"):
         await hello_world_gbk(scope, receive, send)
+    elif scope["path"].startswith("/windows1251"):
+        await hello_world_windows1251(scope, receive, send)
     elif scope["path"].startswith("http://"):
         await http_proxy(scope, receive, send)
     elif scope["method"] == "CONNECT":
         await https_proxy(scope, receive, send)
     else:
         await hello_world(scope, receive, send)
 
@@ -161,14 +163,30 @@
             "status": 200,
             "headers": [[b"content-type", b"text/plain; charset=gbk"]],
         }
     )
     await send({"type": "http.response.body", "body": b"Hello, world!"})
 
 
+async def hello_world_windows1251(scope, receive, send):
+    await send(
+        {
+            "type": "http.response.start",
+            "status": 200,
+            "headers": [[b"content-type", b"text/plain"]],
+        }
+    )
+    await send(
+        {
+            "type": "http.response.body",
+            "body": "Bсеки човек има право на образование.".encode("cp1251"),
+        }
+    )
+
+
 async def http_proxy(scope, receive, send):
     await send(
         {
             "type": "http.response.start",
             "status": 200,
             "headers": [[b"content-type", b"application/json"]],
         }
@@ -413,27 +431,25 @@
             ],
         }
     )
     await send({"type": "http.response.body", "body": b"Hello, world!"})
 
 
 async def redirect_301(scope, receive, send):
-    await send(
-        {"type": "http.response.start", "status": 301, "headers": [[b"location", b"/"]]}
-    )
+    await send({"type": "http.response.start", "status": 301, "headers": [[b"location", b"/"]]})
     await send({"type": "http.response.body", "body": b"Redirecting..."})
 
 
 async def redirect_to(scope, receive, send):
     params = parse_qs(scope["query_string"].decode())
     await send(
         {
             "type": "http.response.start",
             "status": 301,
-            "headers": [[b"location", params["to"][0].encode()]],  # type: ignore
+            "headers": [[b"location", params["to"][0].encode()]],
         }
     )
     await send({"type": "http.response.body", "body": b"Redirecting..."})
 
 
 async def redirect_loop(scope, receive, send):
     await send(
@@ -589,15 +605,15 @@
     def __init__(self, port):
         self.url = f"ws://127.0.0.1:{port}"
         self.port = port
 
     def run(self):
         async def serve(port):
             # GitHub actions only likes 127, not localhost, wtf...
-            async with websockets.serve(echo, "127.0.0.1", port):
+            async with websockets.serve(echo, "127.0.0.1", port):  # pyright: ignore
                 await asyncio.Future()  # run forever
 
         asyncio.run(serve(self.port))
 
 
 def serve_in_thread(server: Server):
     thread = threading.Thread(target=server.run)
@@ -688,23 +704,25 @@
 
 
 @file_app.post("/files")
 def upload_multi_files(images: typing.List[UploadFile]):
     files = []
     for image in images:
         content = image.file.read()
-        files.append({
-            "filename": image.filename,
-            "content_type": image.content_type,
-            "size": len(content),
-
-        })
+        files.append(
+            {
+                "filename": image.filename,
+                "content_type": image.content_type,
+                "size": len(content),
+            }
+        )
 
     return {"files": files}
 
+
 @file_app.post("/two-files")
 def upload_two_files(image1: UploadFile, image2: UploadFile):
     return {
         "size1": len(image1.file.read()),
         "size2": len(image2.file.read()),
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_async.py` & `curl_cffi-0.7.0b4/tests/unittest/test_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from curl_cffi import AsyncCurl, Curl, CurlOpt
 
 
 async def test_init(server):
-    ac = AsyncCurl()
+    ac = AsyncCurl()  # noqa F841
 
 
 async def test_add_handle(server):
     ac = AsyncCurl()
     c = Curl()
     c.setopt(CurlOpt.URL, "http://example.com")
     c.setopt(CurlOpt.WRITEFUNCTION, lambda x: len(x))
@@ -19,13 +19,12 @@
     running = ac.socket_action(-1, 0)
     # assert running == 0
     c = Curl()
     c.setopt(CurlOpt.URL, "http://example.com")
     c.setopt(CurlOpt.WRITEFUNCTION, lambda x: len(x))
     fut = ac.add_handle(c)
     await fut
-    running = ac.socket_action(-1, 0)
+    running = ac.socket_action(-1, 0)  # noqa F841
     # assert running == 1
 
 
-async def test_process_data(server):
-    ...
+async def test_process_data(server): ...
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_async_session.py` & `curl_cffi-0.7.0b4/tests/unittest/test_async_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import base64
 import json
+from contextlib import suppress
+
 import pytest
 
 from curl_cffi.requests import AsyncSession, RequestsError
 from curl_cffi.requests.errors import SessionClosed
 
 
 async def test_get(server):
@@ -21,44 +23,36 @@
         assert r.status_code == 200
 
     asyncio.run(get())
 
 
 async def test_post_dict(server):
     async with AsyncSession() as s:
-        r = await s.post(
-            str(server.url.copy_with(path="/echo_body")), data={"foo": "bar"}
-        )
+        r = await s.post(str(server.url.copy_with(path="/echo_body")), data={"foo": "bar"})
         assert r.status_code == 200
         assert r.content == b"foo=bar"
 
 
 async def test_post_str(server):
     async with AsyncSession() as s:
-        r = await s.post(
-            str(server.url.copy_with(path="/echo_body")), data='{"foo": "bar"}'
-        )
+        r = await s.post(str(server.url.copy_with(path="/echo_body")), data='{"foo": "bar"}')
         assert r.status_code == 200
         assert r.content == b'{"foo": "bar"}'
 
 
 async def test_post_json(server):
     async with AsyncSession() as s:
-        r = await s.post(
-            str(server.url.copy_with(path="/echo_body")), json={"foo": "bar"}
-        )
+        r = await s.post(str(server.url.copy_with(path="/echo_body")), json={"foo": "bar"})
         assert r.status_code == 200
         assert r.content == b'{"foo":"bar"}'
 
 
 async def test_put_json(server):
     async with AsyncSession() as s:
-        r = await s.put(
-            str(server.url.copy_with(path="/echo_body")), json={"foo": "bar"}
-        )
+        r = await s.put(str(server.url.copy_with(path="/echo_body")), json={"foo": "bar"})
         assert r.status_code == 200
         assert r.content == b'{"foo":"bar"}'
 
 
 async def test_delete(server):
     async with AsyncSession() as s:
         r = await s.delete(str(server.url.copy_with(path="/echo_body")))
@@ -67,37 +61,60 @@
 
 async def test_options(server):
     async with AsyncSession() as s:
         r = await s.options(str(server.url.copy_with(path="/echo_body")))
         assert r.status_code == 200
 
 
+async def test_base_url(server):
+    async with AsyncSession(
+        base_url=str(server.url.copy_with(path="/a/b", params={"foo": "bar"}))
+    ) as s:
+        # target path is empty
+        r = await s.get("")
+        assert r.url == s.base_url
+
+        # target path only has params
+        r = await s.get("", params={"hello": "world"})
+        assert r.url == str(server.url.copy_with(path="/a/b", params={"hello": "world"}))
+
+        # target path is a relative path without starting /
+        r = await s.get("x")
+        assert r.url == str(server.url.copy_with(path="/a/x"))
+        r = await s.get("x", params={"hello": "world"})
+        assert r.url == str(server.url.copy_with(path="/a/x", params={"hello": "world"}))
+
+        # target path is a relative path with starting /
+        r = await s.get("/x")
+        assert r.url == str(server.url.copy_with(path="/x"))
+        r = await s.get("/x", params={"hello": "world"})
+        assert r.url == str(server.url.copy_with(path="/x", params={"hello": "world"}))
+
+        # target path is an absolute url
+        r = await s.get(str(server.url.copy_with(path="/x/y")))
+        assert r.url == str(server.url.copy_with(path="/x/y"))
+
+
 async def test_params(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"})
         assert r.status_code == 200
         assert r.content == b'{"params": {"foo": ["bar"]}}'
 
 
 async def test_update_params(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_params?foo=z")), params={"foo": "bar"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_params?foo=z")), params={"foo": "bar"})
         assert r.status_code == 200
         assert r.content == b'{"params": {"foo": ["bar"]}}'
 
 
 async def test_headers(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_headers")), headers={"foo": "bar"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_headers")), headers={"foo": "bar"})
         headers = r.json()
         assert headers["Foo"][0] == "bar"
 
 
 async def test_cookies(server):
     async with AsyncSession() as s:
         r = await s.get(
@@ -106,45 +123,36 @@
         )
         cookies = r.json()
         assert cookies["foo"] == "bar"
 
 
 async def test_auth(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_headers")), auth=("foo", "bar")
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_headers")), auth=("foo", "bar"))
         assert r.status_code == 200
-        assert (
-            r.json()["Authorization"][0]
-            == f"Basic {base64.b64encode(b'foo:bar').decode()}"
-        )
+        assert r.json()["Authorization"][0] == f"Basic {base64.b64encode(b'foo:bar').decode()}"
 
 
 async def test_timeout(server):
     with pytest.raises(RequestsError):
         async with AsyncSession() as s:
             await s.get(str(server.url.copy_with(path="/slow_response")), timeout=0.1)
 
 
 async def test_not_follow_redirects(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/redirect_301")), allow_redirects=False
-        )
+        r = await s.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=False)
         assert r.status_code == 301
         assert r.redirect_count == 0
         assert r.content == b"Redirecting..."
 
 
 async def test_follow_redirects(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-        )
+        r = await s.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
         assert r.status_code == 200
         assert r.redirect_count == 1
 
 
 async def test_verify(https_server):
     async with AsyncSession() as s:
         with pytest.raises(RequestsError, match="SSL certificate problem"):
@@ -170,17 +178,15 @@
 #######################################################################################
 # testing response
 #######################################################################################
 
 
 async def test_redirect_url(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-        )
+        r = await s.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
         assert r.url == str(server.url.copy_with(path="/"))
 
 
 async def test_response_headers(server):
     async with AsyncSession() as s:
         r = await s.get(str(server.url.copy_with(path="/set_headers")))
         assert r.headers.get_list("x-test") == ["test", "test2"]
@@ -197,60 +203,50 @@
     async with AsyncSession() as s:
         r = await s.get(str(server.url.copy_with(path="/slow_response")))
         assert r.elapsed > 0.1
 
 
 async def test_reason(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/redirect_301")), allow_redirects=False
-        )
+        r = await s.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=False)
         assert r.reason == "Moved Permanently"
-        r = await s.get(
-            str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-        )
+        r = await s.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
         assert r.status_code == 200
         assert r.reason == "OK"
 
 
 #######################################################################################
 # testing session
 #######################################################################################
 
 
 async def test_session_update_parms(server):
     async with AsyncSession(params={"old": "day"}) as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"})
         assert r.content == b'{"params": {"old": ["day"], "foo": ["bar"]}}'
 
 
 async def test_session_preset_cookies(server):
     async with AsyncSession(cookies={"foo": "bar"}) as s:
         # send requests with other cookies
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"})
         cookies = r.json()
         # old cookies should be persisted
         assert cookies["foo"] == "bar"
         # new cookies should be added
         assert cookies["hello"] == "world"
 
 
 async def test_session_cookies(server):
     async with AsyncSession() as s:
         # let the server set cookies
         r = await s.get(str(server.url.copy_with(path="/set_cookies")))
         assert s.cookies["foo"] == "bar"
         # send requests with other cookies
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"})
         cookies = r.json()
         # old cookies should be persisted
         assert cookies["foo"] == "bar"
         # new cookies should be added
         assert cookies["hello"] == "world"
 
 
@@ -260,53 +256,49 @@
         r = await s.get(str(server.url), headers={"Foo": "bar"})
         r = await s.get(str(server.url), headers={"Foo": "baz"})
         assert r.status_code == 200
 
 
 async def test_session_too_many_headers(server):
     async with AsyncSession() as s:
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_headers")), headers={"Foo": "1"}
-        )
-        r = await s.get(
-            str(server.url.copy_with(path="/echo_headers")), headers={"Foo": "2"}
-        )
+        r = await s.get(str(server.url.copy_with(path="/echo_headers")), headers={"Foo": "1"})
+        r = await s.get(str(server.url.copy_with(path="/echo_headers")), headers={"Foo": "2"})
         headers = r.json()
         assert len(headers["Foo"]) == 1
         assert headers["Foo"][0] == "2"
 
 
 # https://github.com/yifeikong/curl_cffi/issues/222
 async def test_closed_session_throws_error():
     async with AsyncSession() as s:
         pass
 
     with pytest.raises(SessionClosed):
-        await s.get('https://example.com')
+        await s.get("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.post('https://example.com')
+        await s.post("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.put('https://example.com')
+        await s.put("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.delete('https://example.com')
+        await s.delete("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.options('https://example.com')
+        await s.options("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.head('https://example.com')
+        await s.head("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.patch('https://example.com')
+        await s.patch("https://example.com")
 
     with pytest.raises(SessionClosed):
-        await s.ws_connect('wss://example.com')
+        await s.ws_connect("wss://example.com")
 
 
 # https://github.com/yifeikong/curl_cffi/issues/39
 async def test_post_body_cleaned(server):
     async with AsyncSession() as s:
         # POST with body
         r = await s.post(str(server.url), json={"foo": "bar"})
@@ -315,33 +307,29 @@
         # ensure body is empty
         assert r.content == b""
 
 
 async def test_timers_leak(server):
     async with AsyncSession() as sess:
         for _ in range(3):
-            try:
+            with suppress(Exception):
                 await sess.get(str(server.url.copy_with(path="/slow_response")), timeout=0.1)
-            except Exception:
-                pass
         await asyncio.sleep(0.2)
         assert len(sess.acurl._timers) == 0
 
 
 #######################################################################################
 # async parallel
 #######################################################################################
 
 
 async def test_parallel(server):
     async with AsyncSession() as s:
         rs = [
-            s.get(
-                str(server.url.copy_with(path="/echo_headers")), headers={"Foo": f"{i}"}
-            )
+            s.get(str(server.url.copy_with(path="/echo_headers")), headers={"Foo": f"{i}"})
             for i in range(6)
         ]
         tasks = [asyncio.create_task(r) for r in rs]
         rs = await asyncio.gather(*tasks)
         for idx, r in enumerate(rs):
             assert r.status_code == 200
             assert r.json()["Foo"][0] == str(idx)
@@ -394,9 +382,7 @@
 async def test_stream_atext(server):
     async with AsyncSession() as s:
         url = str(server.url.copy_with(path="/stream"))
         async with s.stream("GET", url, params={"n": "20"}) as r:
             text = await r.atext()
             chunks = text.split("\n")
             assert len(chunks) == 20
-
-
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_cookies.py` & `curl_cffi-0.7.0b4/tests/unittest/test_cookies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
-from curl_cffi.requests.models import Request
+
 from curl_cffi.requests.cookies import Cookies, CurlMorsel
-from curl_cffi.requests.headers import Headers
 from curl_cffi.requests.errors import CookieConflict, RequestsError
 
 
 def test_cookies_conflict():
     c = Cookies()
     c.set("foo", "bar", domain="example.com")
     c.set("foo", "baz", domain="test.local")
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_curl.py` & `curl_cffi-0.7.0b4/tests/unittest/test_curl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import json
 from io import BytesIO
+from typing import cast
 
 import pytest
 
 from curl_cffi import Curl, CurlError, CurlInfo, CurlOpt
 
 #######################################################################################
 # testing setopt
@@ -147,17 +148,15 @@
     c.setopt(CurlOpt.URL, url.encode())
     c.setopt(CurlOpt.USERNAME, b"foo")
     c.setopt(CurlOpt.PASSWORD, b"bar")
     buffer = BytesIO()
     c.setopt(CurlOpt.WRITEDATA, buffer)
     c.perform()
     headers = json.loads(buffer.getvalue().decode())
-    assert (
-        headers["Authorization"][0] == f"Basic {base64.b64encode(b'foo:bar').decode()}"
-    )
+    assert headers["Authorization"][0] == f"Basic {base64.b64encode(b'foo:bar').decode()}"
 
 
 def test_timeout(server):
     c = Curl()
     url = str(server.url.copy_with(path="/slow_response"))
     c.setopt(CurlOpt.URL, url.encode())
     c.setopt(CurlOpt.TIMEOUT_MS, 100)
@@ -307,15 +306,15 @@
 
 
 def test_elapsed(server):
     c = Curl()
     url = str(server.url)
     c.setopt(CurlOpt.URL, url.encode())
     c.perform()
-    assert c.getinfo(CurlInfo.TOTAL_TIME) > 0
+    assert cast(int, c.getinfo(CurlInfo.TOTAL_TIME)) > 0
 
 
 def test_reason(server):
     c = Curl()
     url = str(server.url)
     c.setopt(CurlOpt.URL, url.encode())
     buffer = BytesIO()
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_headers.py` & `curl_cffi-0.7.0b4/tests/unittest/test_headers.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_impersonate.py` & `curl_cffi-0.7.0b4/tests/unittest/test_impersonate.py`

 * *Files identical despite different names*

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_requests.py` & `curl_cffi-0.7.0b4/tests/unittest/test_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import base64
+import json
 import time
 from io import BytesIO
-import json
 
 import pytest
+from charset_normalizer import detect
 
-from curl_cffi import requests, CurlOpt
+from curl_cffi import CurlOpt, requests
 from curl_cffi.const import CurlECode, CurlInfo
 from curl_cffi.requests.errors import SessionClosed
+from curl_cffi.requests.models import Response
 
 
 def test_head(server):
     r = requests.head(str(server.url))
     assert r.status_code == 200
 
 
@@ -41,17 +43,15 @@
     bar = "a" * 100000
     r = requests.post(str(server.url.copy_with(path="/echo_body")), json={"foo": bar})
     assert r.status_code == 200
     assert r.json()["foo"] == bar
 
 
 def test_post_str(server):
-    r = requests.post(
-        str(server.url.copy_with(path="/echo_body")), data='{"foo": "bar"}'
-    )
+    r = requests.post(str(server.url.copy_with(path="/echo_body")), data='{"foo": "bar"}')
     assert r.status_code == 200
     assert r.content == b'{"foo": "bar"}'
 
 
 def test_post_no_body(server):
     r = requests.post(str(server.url), headers={"Content-Type": "application/json"})
     assert r.status_code == 200
@@ -64,14 +64,30 @@
     assert r.status_code == 200
     assert r.content == b'{"foo":"bar"}'
     r = requests.post(str(server.url.copy_with(path="/echo_body")), json={})
     assert r.status_code == 200
     assert r.content == b"{}"
 
 
+def test_post_form(server):
+    r = requests.post(str(server.url.copy_with(path="/echo_body")), data={"foo": "bar"})
+    assert r.status_code == 200
+    assert r.content == b"foo=bar"
+
+    data = [("foo", 7), ("foo", 8), ("bar", 9)]
+    r = requests.post(str(server.url.copy_with(path="/echo_body")), data=data)
+    assert r.status_code == 200
+    assert r.content == b"foo=7&foo=8&bar=9"
+
+    data = [("foo[]", 7), ("foo[]", 8), ("bar", 9)]
+    r = requests.post(str(server.url.copy_with(path="/echo_body")), data=data)
+    assert r.status_code == 200
+    assert r.content == b"foo%5B%5D=7&foo%5B%5D=8&bar=9"
+
+
 def test_post_redirect_to_get(server):
     url = str(server.url.copy_with(path="/redirect_then_echo_headers"))
     r = requests.post(url, data={"foo": "bar"}, allow_redirects=True, debug=True)
     headers = r.json()
     # print(headers)
     assert headers.get("Content-length") is None
 
@@ -89,38 +105,69 @@
 
 def test_options(server):
     r = requests.options(str(server.url.copy_with(path="/echo_body")))
     assert r.status_code == 200
 
 
 def test_params(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"}
-    )
+    r = requests.get(str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"})
     assert r.content == b'{"params": {"foo": ["bar"]}}'
 
 
 def test_update_params(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/echo_params?foo=z")), params={"foo": "bar"}
-    )
+    # The param is new, just append it
+    r = requests.get(str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"})
     assert r.content == b'{"params": {"foo": ["bar"]}}'
 
+    # The old param is already multiple, append it, too
+    r = requests.get(str(server.url.copy_with(path="/echo_params?foo=1&foo=2")), params={"foo": 3})
+    assert r.content == b'{"params": {"foo": ["1", "2", "3"]}}'
+
+    # 1 to 1 mapping, we have to update it.
+    r = requests.get(str(server.url.copy_with(path="/echo_params?foo=z")), params={"foo": "bar"})
+    assert r.content == b'{"params": {"foo": ["bar"]}}'
+
+    # does not break old ones
+    r = requests.get(
+        str(server.url.copy_with(path="/echo_params?a=1&a=2&foo=z")),
+        params={"foo": "bar"},
+    )
+    assert r.content == b'{"params": {"a": ["1", "2"], "foo": ["bar"]}}'
 
-def test_headers(server):
     r = requests.get(
-        str(server.url.copy_with(path="/echo_headers")), headers={"foo": "bar"}
+        str(server.url.copy_with(path="/echo_params?a=1&a=2&foo=z")),
+        params=[("foo", "1"), ("foo", "2")],
     )
+    assert r.content == b'{"params": {"a": ["1", "2"], "foo": ["z", "1", "2"]}}'
+
+
+def test_headers(server):
+    r = requests.get(str(server.url.copy_with(path="/echo_headers")), headers={"foo": "bar"})
     headers = r.json()
     assert headers["Foo"][0] == "bar"
 
 
 def test_charset_parse(server):
-    r = requests.get( str(server.url.copy_with(path="/gbk")))
-    assert r.charset == "gbk"
+    r = requests.get(str(server.url.copy_with(path="/gbk")))
+    assert r.encoding == "gbk"
+
+
+def test_charset_default_encoding(server):
+    r = requests.get(
+        str(server.url.copy_with(path="/windows1251")), default_encoding="windows-1251"
+    )
+    assert r.encoding == "windows-1251"
+
+
+def test_charset_default_encoding_autodetect(server):
+    def autodetect(content):
+        return detect(content).get("encoding")
+
+    r = requests.get(str(server.url.copy_with(path="/windows1251")), default_encoding=autodetect)
+    assert r.encoding == "windows-1251"
 
 
 def test_content_type_header_with_json(server):
     # FIXME: this actually does not work, because the test server uvicorn will merge
     # Content-Type headers, so it always works even if there is duplicate headers.
     r = requests.get(
         str(server.url.copy_with(path="/echo_headers")),
@@ -157,21 +204,17 @@
         )
         cookies = r.json()
         assert cookies["__Secure-foo"] == "bar"
         assert cookies["__Host-hello"] == "world"
 
 
 def test_auth(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/echo_headers")), auth=("foo", "bar")
-    )
+    r = requests.get(str(server.url.copy_with(path="/echo_headers")), auth=("foo", "bar"))
     assert r.status_code == 200
-    assert (
-        r.json()["Authorization"][0] == f"Basic {base64.b64encode(b'foo:bar').decode()}"
-    )
+    assert r.json()["Authorization"][0] == f"Basic {base64.b64encode(b'foo:bar').decode()}"
 
 
 def test_timeout(server):
     with pytest.raises(requests.RequestsError):
         requests.get(str(server.url.copy_with(path="/slow_response")), timeout=0.1)
 
 
@@ -182,64 +225,57 @@
 
 def test_post_timeout(server):
     with pytest.raises(requests.RequestsError):
         requests.post(str(server.url.copy_with(path="/slow_response")), timeout=0.1)
 
 
 def test_not_follow_redirects(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/redirect_301")), allow_redirects=False
-    )
+    r = requests.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=False)
     assert r.status_code == 301
     assert r.redirect_count == 0
     assert r.content == b"Redirecting..."
 
 
 def test_follow_redirects(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-    )
+    r = requests.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
     assert r.status_code == 200
     assert r.redirect_count == 1
 
 
 def test_too_many_redirects(server):
     with pytest.raises(requests.RequestsError) as e:
         requests.get(str(server.url.copy_with(path="/redirect_loop")), max_redirects=2)
     assert e.value.code == CurlECode.TOO_MANY_REDIRECTS
-    assert e.value.response.status_code == 301  # type: ignore
+    assert isinstance(e.value.response, Response)
+    assert e.value.response.status_code == 301
 
 
 def test_verify(https_server):
     with pytest.raises(requests.RequestsError, match="SSL certificate problem"):
         requests.get(str(https_server.url), verify=True)
 
 
 def test_verify_false(https_server):
     r = requests.get(str(https_server.url), verify=False)
     assert r.status_code == 200
 
 
 def test_referer(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/echo_headers")), referer="http://example.com"
-    )
+    r = requests.get(str(server.url.copy_with(path="/echo_headers")), referer="http://example.com")
     headers = r.json()
     assert headers["Referer"][0] == "http://example.com"
 
 
 #######################################################################################
 # testing response
 #######################################################################################
 
 
 def test_redirect_url(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-    )
+    r = requests.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
     assert r.url == str(server.url.copy_with(path="/"))
 
 
 def test_response_headers(server):
     r = requests.get(str(server.url.copy_with(path="/set_headers")))
     assert r.headers.get_list("x-test") == ["test", "test2"]
 
@@ -252,21 +288,17 @@
 
 def test_elapsed(server):
     r = requests.get(str(server.url.copy_with(path="/slow_response")))
     assert r.elapsed > 0.1
 
 
 def test_reason(server):
-    r = requests.get(
-        str(server.url.copy_with(path="/redirect_301")), allow_redirects=False
-    )
+    r = requests.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=False)
     assert r.reason == "Moved Permanently"
-    r = requests.get(
-        str(server.url.copy_with(path="/redirect_301")), allow_redirects=True
-    )
+    r = requests.get(str(server.url.copy_with(path="/redirect_301")), allow_redirects=True)
     assert r.status_code == 200
     assert r.reason == "OK"
 
 
 #######################################################################################
 # testing session
 #######################################################################################
@@ -280,39 +312,63 @@
 
 def test_session_options(server):
     s = requests.Session()
     r = s.options(str(server.url))
     assert r.status_code == 200
 
 
+def test_session_base_url(server):
+    s = requests.Session(base_url=str(server.url.copy_with(path="/a/b", params={"foo": "bar"})))
+
+    # target path is empty
+    r = s.get("")
+    assert r.url == s.base_url
+
+    # target path only has params
+    r = s.get("", params={"hello": "world"})
+    assert r.url == str(server.url.copy_with(path="/a/b", params={"hello": "world"}))
+
+    # target path is a relative path without starting /
+    r = s.get("x")
+    assert r.url == str(server.url.copy_with(path="/a/x"))
+    r = s.get("x", params={"hello": "world"})
+    assert r.url == str(server.url.copy_with(path="/a/x", params={"hello": "world"}))
+
+    # target path is a relative path with starting /
+    r = s.get("/x")
+    assert r.url == str(server.url.copy_with(path="/x"))
+    r = s.get("/x", params={"hello": "world"})
+    assert r.url == str(server.url.copy_with(path="/x", params={"hello": "world"}))
+
+    # target path is an absolute url
+    r = s.get(str(server.url.copy_with(path="/x/y")))
+    assert r.url == str(server.url.copy_with(path="/x/y"))
+
+
 def test_session_update_parms(server):
     s = requests.Session(params={"old": "day"})
     r = s.get(str(server.url.copy_with(path="/echo_params")), params={"foo": "bar"})
     assert r.content == b'{"params": {"old": ["day"], "foo": ["bar"]}}'
 
 
 def test_session_preset_cookies(server):
     s = requests.Session(cookies={"foo": "bar"})
     # send requests with other cookies
-    r = s.get(
-        str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"}
-    )
+    r = s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"})
     cookies = r.json()
     # old cookies should be persisted
     assert cookies["foo"] == "bar"
     # new cookies should be added
     assert cookies["hello"] == "world"
     # XXX request cookies will always be added to the entire session
     # request cookies should not be added to session cookiejar
     # assert s.cookies.get("hello") is None
 
     # but you can override
-    r = s.get(
-        str(server.url.copy_with(path="/echo_cookies")), cookies={"foo": "notbar"}
-    )
+    r = s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"foo": "notbar"})
     cookies = r.json()
     assert cookies["foo"] == "notbar"
 
 
 def test_delete_cookies(server):
     s = requests.Session()
     s.get(str(server.url.copy_with(path="/set_cookies")))
@@ -322,34 +378,30 @@
 
 
 def test_cookie_domains(server):
     s = requests.Session()
     s.cookies.set("foo", "bar", domain="example.com")
     s.cookies.set("foo2", "bar", domain="127.0.0.1")
     # send requests with other cookies
-    r = s.get(
-        str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"}
-    )
+    r = s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"})
     cookies = r.json()
     # only specific domains should be there
     assert "foo" not in cookies
     assert cookies["foo2"] == "bar"
     # new cookies should be added
     assert cookies["hello"] == "world"
 
 
 def test_session_cookies(server):
     s = requests.Session()
     # let the server set cookies
     r = s.get(str(server.url.copy_with(path="/set_cookies")))
     assert s.cookies["foo"] == "bar"
     # send requests with other cookies
-    r = s.get(
-        str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"}
-    )
+    r = s.get(str(server.url.copy_with(path="/echo_cookies")), cookies={"hello": "world"})
     cookies = r.json()
     # old cookies should be persisted
     assert cookies["foo"] == "bar"
     # new cookies should be added
     assert cookies["hello"] == "world"
 
 
@@ -437,72 +489,68 @@
     r = s.get(str(server.url), headers={"Foo": "baz"})
     assert r.status_code == 200
 
 
 # https://github.com/yifeikong/curl_cffi/pull/171
 def test_session_with_hostname_proxies(server, proxy_server):
     proxies = {
-        f'all://{server.url.host}': f'http://{proxy_server.flags.hostname}:{proxy_server.flags.port}'
+        f"all://{server.url.host}": f"http://{proxy_server.flags.hostname}:{proxy_server.flags.port}"
     }
     s = requests.Session(proxies=proxies)
     url = str(server.url.copy_with(path="/echo_headers"))
     r = s.get(url)
-    assert r.text == 'Hello from man in the middle'
+    assert r.text == "Hello from man in the middle"
 
 
 # https://github.com/yifeikong/curl_cffi/pull/171
 def test_session_with_http_proxies(server, proxy_server):
-    proxies = {
-        'http': f'http://{proxy_server.flags.hostname}:{proxy_server.flags.port}'
-    }
+    proxies = {"http": f"http://{proxy_server.flags.hostname}:{proxy_server.flags.port}"}
     s = requests.Session(proxies=proxies)
     url = str(server.url.copy_with(path="/echo_headers"))
     r = s.get(url)
-    assert r.text == 'Hello from man in the middle'
+    assert r.text == "Hello from man in the middle"
 
 
 # https://github.com/yifeikong/curl_cffi/pull/171
 def test_session_with_all_proxies(server, proxy_server):
-    proxies = {
-        'all': f'http://{proxy_server.flags.hostname}:{proxy_server.flags.port}'
-    }
+    proxies = {"all": f"http://{proxy_server.flags.hostname}:{proxy_server.flags.port}"}
     s = requests.Session(proxies=proxies)
     url = str(server.url.copy_with(path="/echo_headers"))
     r = s.get(url)
-    assert r.text == 'Hello from man in the middle'
+    assert r.text == "Hello from man in the middle"
 
 
 # https://github.com/yifeikong/curl_cffi/issues/222
 def test_closed_session_throws_error():
     with requests.Session() as s:
         pass
 
     with pytest.raises(SessionClosed):
-        s.get('https://example.com')
+        s.get("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.post('https://example.com')
+        s.post("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.put('https://example.com')
+        s.put("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.delete('https://example.com')
+        s.delete("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.options('https://example.com')
+        s.options("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.head('https://example.com')
+        s.head("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.patch('https://example.com')
+        s.patch("https://example.com")
 
     with pytest.raises(SessionClosed):
-        s.ws_connect('wss://example.com')
+        s.ws_connect("wss://example.com")
 
 
 def test_stream_iter_content(server):
     with requests.Session() as s:
         url = str(server.url.copy_with(path="/stream"))
         with s.stream("GET", url, params={"n": "20"}) as r:
             for chunk in r.iter_content():
@@ -553,15 +601,15 @@
 #                 # print(data["path"])
 #             assert r.status_code == 200
 
 
 def test_stream_incomplete_read(server):
     with requests.Session() as s:
         url = str(server.url.copy_with(path="/incomplete_read"))
-        with pytest.raises(requests.RequestsError) as e:
+        with pytest.raises(requests.RequestsError) as e:  # noqa: SIM117
             with s.stream("GET", url) as r:
                 for _ in r.iter_content():
                     continue
         assert e.value.code == CurlECode.PARTIAL_FILE
 
 
 def test_stream_incomplete_read_without_close(server):
@@ -576,30 +624,32 @@
 
         assert e.value.code == CurlECode.PARTIAL_FILE
 
 
 def test_stream_redirect_loop(server):
     with requests.Session() as s:
         url = str(server.url.copy_with(path="/redirect_loop"))
-        with pytest.raises(requests.RequestsError) as e:
+        with pytest.raises(requests.RequestsError) as e:  # noqa: SIM117
             with s.stream("GET", url, max_redirects=2):
                 pass
         assert e.value.code == CurlECode.TOO_MANY_REDIRECTS
-        assert e.value.response.status_code == 301  # type: ignore
+        assert isinstance(e.value.response, Response)
+        assert e.value.response.status_code == 301
 
 
 def test_stream_redirect_loop_without_close(server):
     with requests.Session() as s:
         url = str(server.url.copy_with(path="/redirect_loop"))
         with pytest.raises(requests.RequestsError) as e:
             # if the error happens receiving header, it's raised right away
             s.get(url, max_redirects=2, stream=True)
 
         assert e.value.code == CurlECode.TOO_MANY_REDIRECTS
-        assert e.value.response.status_code == 301  # type: ignore
+        assert isinstance(e.value.response, Response)
+        assert e.value.response.status_code == 301
 
 
 def test_stream_auto_close_plain(server):
     s = requests.Session()
     url = str(server.url.copy_with(path="/stream"))
     s.get(url, stream=True)
     url = str(server.url.copy_with(path="/"))
@@ -620,15 +670,16 @@
 def test_stream_auto_close_with_header_errors(server):
     s = requests.Session()
 
     url = str(server.url.copy_with(path="/redirect_loop"))
     with pytest.raises(requests.RequestsError) as e:
         s.get(url, max_redirects=2, stream=True)
     assert e.value.code == CurlECode.TOO_MANY_REDIRECTS
-    assert e.value.response.status_code == 301  # type: ignore
+    assert isinstance(e.value.response, Response)
+    assert e.value.response.status_code == 301
 
     url = str(server.url.copy_with(path="/"))
     s.get(url, stream=True)
 
 
 def test_stream_options_persist(server):
     s = requests.Session()
@@ -648,38 +699,36 @@
 @pytest.mark.skip(reason="External url unstable")
 def test_stream_close_early(server):
     s = requests.Session()
     # url = str(server.url.copy_with(path="/large"))
     # from http://xcal1.vodafone.co.uk/
     url = "http://212.183.159.230/200MB.zip"
     r = s.get(url, max_recv_speed=1024 * 1024, stream=True)
-    counter = 0
     start = time.time()
-    for _ in r.iter_content():
-        counter += 1
-        if counter > 10:
+    for i, _ in enumerate(r.iter_content()):
+        if i > 10:
             break
     r.close()
     end = time.time()
     assert end - start < 50
 
 
 @pytest.mark.skip(reason="External url unstable")
 def test_max_recv_speed(server):
     s = requests.Session()
     s.curl.setopt(CurlOpt.BUFFERSIZE, 1024 * 1024)
     url = str(server.url.copy_with(path="/large"))
     # from http://xcal1.vodafone.co.uk/
     url = "http://212.183.159.230/200MB.zip"
     start = time.time()
-    r = s.get(url, max_recv_speed=10 * 1024 * 1024)
+    r = s.get(url, max_recv_speed=10 * 1024 * 1024)  # noqa F841
     end = time.time()
     # assert len(r.content) == 20 * 1024 * 1024
     assert end - start > 10
 
 
 def test_curl_infos(server):
     s = requests.Session(curl_infos=[CurlInfo.PRIMARY_IP])
 
     r = s.get(str(server.url))
 
-    assert r.infos[CurlInfo.PRIMARY_IP] == b"127.0.0.1"
+    assert r.infos[CurlInfo.PRIMARY_IP] == b"127.0.0.1"  # pyright: ignore
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_smoke.py` & `curl_cffi-0.7.0b4/tests/unittest/test_smoke.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Simple smoke test to real world websites
 from curl_cffi import requests
 
-
 URLS = [
     "https://www.baidu.com",
     "https://www.qq.com",
 ]
 
 
 def test_without_impersonate():
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_upload.py` & `curl_cffi-0.7.0b4/tests/unittest/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 from pathlib import Path
 
-import pytest
-
 from curl_cffi import CurlMime, requests
 
 ASSET_FOLDER = Path(__file__).parent.parent.parent / "assets"
 
 
 def test_upload_single_file(file_server):
     multipart = CurlMime.from_list(
@@ -37,17 +35,15 @@
                 "filename": "alipay.jpg",
                 "local_path": str(ASSET_FOLDER / "alipay.jpg"),
             },
             {"name": "foo", "data": b"bar"},
         ]
     )
 
-    r = requests.post(
-        file_server.url + "/file", data={"foo": "bar"}, multipart=multipart
-    )
+    r = requests.post(file_server.url + "/file", data={"foo": "bar"}, multipart=multipart)
     data = r.json()
     assert data["filename"] == "alipay.jpg"
     assert data["content_type"] == "image/jpg"
     assert data["size"] == os.path.getsize(ASSET_FOLDER / "alipay.jpg")
     assert data["foo"] == "bar"
     multipart.close()
 
@@ -66,15 +62,15 @@
                 "content_type": "image/jpg",
                 "filename": "wechat.jpg",
                 "local_path": str(ASSET_FOLDER / "wechat.jpg"),
             },
         ]
     )
 
-    r = requests.post( file_server.url + "/files", multipart=multipart)
+    r = requests.post(file_server.url + "/files", multipart=multipart)
     data = r.json()
     assert len(data["files"]) == 2
     assert data["files"][0]["filename"] == "alipay.jpg"
     assert data["files"][0]["content_type"] == "image/jpg"
     assert data["files"][0]["size"] == os.path.getsize(ASSET_FOLDER / "alipay.jpg")
     multipart.close()
 
@@ -93,12 +89,12 @@
                 "content_type": "image/jpg",
                 "filename": "wechat.jpg",
                 "local_path": str(ASSET_FOLDER / "wechat.jpg"),
             },
         ]
     )
 
-    r = requests.post(file_server.url + "/two-files" , multipart=multipart)
+    r = requests.post(file_server.url + "/two-files", multipart=multipart)
     data = r.json()
     assert data["size1"] == os.path.getsize(ASSET_FOLDER / "alipay.jpg")
     assert data["size2"] == os.path.getsize(ASSET_FOLDER / "wechat.jpg")
     multipart.close()
```

### Comparing `curl_cffi-0.6.3b1/tests/unittest/test_websockets.py` & `curl_cffi-0.7.0b4/tests/unittest/test_websockets.py`

 * *Files identical despite different names*

