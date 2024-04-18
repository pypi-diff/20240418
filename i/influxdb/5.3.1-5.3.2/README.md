# Comparing `tmp/influxdb-5.3.1.tar.gz` & `tmp/influxdb-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/influxdb-5.3.1.tar", last modified: Wed Nov 11 21:23:18 2020, max compression
+gzip compressed data, was "influxdb-5.3.2.tar", last modified: Thu Apr 18 21:45:02 2024, max compression
```

## Comparing `influxdb-5.3.1.tar` & `influxdb-5.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     1075 2020-04-10 19:37:09.000000 influxdb-5.3.1/LICENSE
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      119 2019-07-16 20:12:00.000000 influxdb-5.3.1/MANIFEST.in
--rw-r--r--   0 sborza    (1000) sborza    (1000)     7150 2020-11-11 21:23:18.000000 influxdb-5.3.1/PKG-INFO
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     4899 2020-04-08 16:30:41.000000 influxdb-5.3.1/README.rst
--rw-rw-r--   0 sborza    (1000) sborza    (1000)       85 2019-07-16 20:12:00.000000 influxdb-5.3.1/dev-requirements.txt
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      433 2020-11-11 21:02:54.000000 influxdb-5.3.1/influxdb/__init__.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)    19398 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/_dataframe_client.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      644 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/chunked_json.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)    45143 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/client.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      831 2020-04-08 16:30:41.000000 influxdb-5.3.1/influxdb/dataframe_client.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     1012 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/exceptions.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)     7846 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/helper.py
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb/influxdb08/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      407 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/influxdb08/__init__.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      659 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/influxdb08/chunked_json.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)    25916 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/influxdb08/client.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     7291 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/influxdb08/dataframe_client.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     5564 2020-04-10 17:33:28.000000 influxdb-5.3.1/influxdb/influxdb08/helper.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     5225 2020-04-10 17:30:12.000000 influxdb-5.3.1/influxdb/line_protocol.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     6756 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/resultset.py
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb/tests/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      608 2020-04-08 16:30:41.000000 influxdb-5.3.1/influxdb/tests/__init__.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     1700 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/chunked_json_test.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)    55698 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/tests/client_test.py
--rw-r--r--   0 sborza    (1000) sborza    (1000)    52326 2020-11-11 19:10:37.000000 influxdb-5.3.1/influxdb/tests/dataframe_client_test.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)    16657 2020-04-10 17:33:28.000000 influxdb-5.3.1/influxdb/tests/helper_test.py
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb/tests/influxdb08/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)       66 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/influxdb08/__init__.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)    32277 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/influxdb08/client_test.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)    13289 2020-04-08 16:30:41.000000 influxdb-5.3.1/influxdb/tests/influxdb08/dataframe_client_test.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     9237 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/influxdb08/helper_test.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     1557 2019-07-16 20:12:00.000000 influxdb-5.3.1/influxdb/tests/misc.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     6868 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/resultset_test.py
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb/tests/server_tests/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)       39 2020-04-06 23:24:00.000000 influxdb-5.3.1/influxdb/tests/server_tests/__init__.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     4244 2020-04-10 16:49:57.000000 influxdb-5.3.1/influxdb/tests/server_tests/base.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)    33279 2020-04-10 16:58:43.000000 influxdb-5.3.1/influxdb/tests/server_tests/client_test_with_server.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     7121 2020-04-09 22:34:53.000000 influxdb-5.3.1/influxdb/tests/server_tests/influxdb_instance.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     6349 2020-04-10 17:30:12.000000 influxdb-5.3.1/influxdb/tests/test_line_protocol.py
-drwxr-xr-x   0 sborza    (1000) sborza    (1000)        0 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     7150 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/PKG-INFO
--rw-rw-r--   0 sborza    (1000) sborza    (1000)     1257 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/SOURCES.txt
--rw-rw-r--   0 sborza    (1000) sborza    (1000)        1 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/dependency_links.txt
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      106 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/requires.txt
--rw-rw-r--   0 sborza    (1000) sborza    (1000)        9 2020-11-11 21:23:18.000000 influxdb-5.3.1/influxdb.egg-info/top_level.txt
--rw-rw-r--   0 sborza    (1000) sborza    (1000)       65 2020-04-11 23:50:47.000000 influxdb-5.3.1/requirements.txt
--rw-rw-r--   0 sborza    (1000) sborza    (1000)      101 2020-11-11 21:23:18.000000 influxdb-5.3.1/setup.cfg
--rwxrwxr-x   0 sborza    (1000) sborza    (1000)     1705 2020-04-08 16:30:41.000000 influxdb-5.3.1/setup.py
--rw-rw-r--   0 sborza    (1000) sborza    (1000)       33 2019-07-16 20:12:00.000000 influxdb-5.3.1/test-requirements.txt
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.637745 influxdb-5.3.2/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1075 2024-04-16 14:22:32.000000 influxdb-5.3.2/LICENSE
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      119 2024-04-16 14:22:32.000000 influxdb-5.3.2/MANIFEST.in
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6848 2024-04-18 21:45:02.637745 influxdb-5.3.2/PKG-INFO
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     5745 2024-04-17 13:12:44.000000 influxdb-5.3.2/README.rst
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       85 2024-04-16 14:22:32.000000 influxdb-5.3.2/dev-requirements.txt
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.634411 influxdb-5.3.2/influxdb/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      433 2024-04-17 13:13:37.000000 influxdb-5.3.2/influxdb/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    19400 2024-04-17 13:12:44.000000 influxdb-5.3.2/influxdb/_dataframe_client.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      644 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/chunked_json.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    46092 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/client.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      831 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/dataframe_client.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1012 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/exceptions.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     7846 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/helper.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.634411 influxdb-5.3.2/influxdb/influxdb08/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      407 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/influxdb08/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      659 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/influxdb08/chunked_json.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    25916 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/influxdb08/client.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     7291 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/influxdb08/dataframe_client.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     5564 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/influxdb08/helper.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     5225 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/line_protocol.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6756 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/resultset.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.634411 influxdb-5.3.2/influxdb/tests/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      608 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1700 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/chunked_json_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    57388 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/client_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    55247 2024-04-17 13:12:44.000000 influxdb-5.3.2/influxdb/tests/dataframe_client_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    16657 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/helper_test.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.634411 influxdb-5.3.2/influxdb/tests/influxdb08/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       66 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/influxdb08/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    32277 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/influxdb08/client_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    13289 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/influxdb08/dataframe_client_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     9237 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/influxdb08/helper_test.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1557 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/misc.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6868 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/resultset_test.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.637745 influxdb-5.3.2/influxdb/tests/server_tests/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       39 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/server_tests/__init__.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     4244 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/server_tests/base.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)    33279 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/server_tests/client_test_with_server.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     7121 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/server_tests/influxdb_instance.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6349 2024-04-16 14:22:32.000000 influxdb-5.3.2/influxdb/tests/test_line_protocol.py
+drwxr-xr-x   0 powersj   (1000) powersj   (1000)        0 2024-04-18 21:45:02.637745 influxdb-5.3.2/influxdb.egg-info/
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     6848 2024-04-18 21:45:02.000000 influxdb-5.3.2/influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 powersj   (1000) powersj   (1000)     1257 2024-04-18 21:45:02.000000 influxdb-5.3.2/influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)        1 2024-04-18 21:45:02.000000 influxdb-5.3.2/influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      106 2024-04-18 21:45:02.000000 influxdb-5.3.2/influxdb.egg-info/requires.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)        9 2024-04-18 21:45:02.000000 influxdb-5.3.2/influxdb.egg-info/top_level.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       65 2024-04-16 14:22:32.000000 influxdb-5.3.2/requirements.txt
+-rw-r--r--   0 powersj   (1000) powersj   (1000)      101 2024-04-18 21:45:02.637745 influxdb-5.3.2/setup.cfg
+-rwxr-xr-x   0 powersj   (1000) powersj   (1000)     1705 2024-04-16 14:22:32.000000 influxdb-5.3.2/setup.py
+-rw-r--r--   0 powersj   (1000) powersj   (1000)       33 2024-04-16 14:22:32.000000 influxdb-5.3.2/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `influxdb-5.3.1/LICENSE` & `influxdb-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/PKG-INFO` & `influxdb-5.3.2/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,201 +1,193 @@
-Metadata-Version: 2.1
-Name: influxdb
-Version: 5.3.1
-Summary: InfluxDB client
-Home-page: https://github.com/influxdb/influxdb-python
-License: MIT License
-Description: InfluxDB-Python
-        ===============
-        
-        .. image:: https://travis-ci.org/influxdata/influxdb-python.svg?branch=master
-            :target: https://travis-ci.org/influxdata/influxdb-python
-        .. image:: https://readthedocs.org/projects/influxdb-python/badge/?version=latest&style
-            :target: http://influxdb-python.readthedocs.org/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/coveralls/influxdata/influxdb-python.svg
-          :target: https://coveralls.io/r/influxdata/influxdb-python
-          :alt: Coverage
-        
-        .. image:: https://img.shields.io/pypi/v/influxdb.svg
-           :target: https://pypi.python.org/pypi/influxdb
-           :alt: PyPI Status
-        
-        InfluxDB-Python is a client for interacting with InfluxDB_.
-        
-        Development of this library is maintained by:
-        
-        +-----------+-------------------------------+
-        | Github ID | URL                           |
-        +===========+===============================+
-        | @aviau    | (https://github.com/aviau)    |
-        +-----------+-------------------------------+
-        | @xginn8   | (https://github.com/xginn8)   |
-        +-----------+-------------------------------+
-        | @sebito91 | (https://github.com/sebito91) |
-        +-----------+-------------------------------+
-        
-        .. _readme-about:
-        
-        InfluxDB is an open-source distributed time series database, find more about InfluxDB_ at https://docs.influxdata.com/influxdb/latest
-        
-        
-        .. _installation:
-        
-        InfluxDB pre v1.1.0 users
-        -------------------------
-        
-        This module is tested with InfluxDB versions: v1.2.4, v1.3.9, v1.4.3, v1.5.4, v1.6.4, and 1.7.4.
-        
-        Those users still on InfluxDB v0.8.x users may still use the legacy client by importing ``from influxdb.influxdb08 import InfluxDBClient``.
-        
-        Installation
-        ------------
-        
-        Install, upgrade and uninstall influxdb-python with these commands::
-        
-            $ pip install influxdb
-            $ pip install --upgrade influxdb
-            $ pip uninstall influxdb
-        
-        On Debian/Ubuntu, you can install it with this command::
-        
-            $ sudo apt-get install python-influxdb
-        
-        Dependencies
-        ------------
-        
-        The influxdb-python distribution is supported and tested on Python 2.7, 3.5, 3.6, 3.7, PyPy and PyPy3.
-        
-        **Note:** Python <3.5 are currently untested. See ``.travis.yml``.
-        
-        Main dependency is:
-        
-        - Requests: HTTP library for human beings (http://docs.python-requests.org/)
-        
-        
-        Additional dependencies are:
-        
-        - pandas: for writing from and reading to DataFrames (http://pandas.pydata.org/)
-        - Sphinx: Tool to create and manage the documentation (http://sphinx-doc.org/)
-        - Nose: to auto-discover tests (http://nose.readthedocs.org/en/latest/)
-        - Mock: to mock tests (https://pypi.python.org/pypi/mock)
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available at https://influxdb-python.readthedocs.io/en/latest/.
-        
-        You will need Sphinx_ installed to generate the documentation.
-        
-        The documentation can be generated by running::
-        
-            $ tox -e docs
-        
-        
-        Generated documentation can be found in the *docs/build/html/* directory.
-        
-        
-        Examples
-        --------
-        
-        Here's a basic example (for more see the examples directory)::
-        
-            $ python
-        
-            >>> from influxdb import InfluxDBClient
-        
-            >>> json_body = [
-                {
-                    "measurement": "cpu_load_short",
-                    "tags": {
-                        "host": "server01",
-                        "region": "us-west"
-                    },
-                    "time": "2009-11-10T23:00:00Z",
-                    "fields": {
-                        "value": 0.64
-                    }
-                }
-            ]
-        
-            >>> client = InfluxDBClient('localhost', 8086, 'root', 'root', 'example')
-        
-            >>> client.create_database('example')
-        
-            >>> client.write_points(json_body)
-        
-            >>> result = client.query('select value from cpu_load_short;')
-        
-            >>> print("Result: {0}".format(result))
-        
-        
-        Testing
-        -------
-        
-        Make sure you have tox by running the following::
-        
-            $ pip install tox
-        
-        To test influxdb-python with multiple version of Python, you can use Tox_::
-        
-            $ tox
-        
-        
-        Support
-        -------
-        
-        For issues with, questions about, or feedback for InfluxDB_, please look into
-        our community page: http://influxdb.com/community/.
-        
-        We are also lurking on the following:
-        
-        - #influxdb on irc.freenode.net
-        - #influxdb on gophers.slack.com
-        
-        
-        Development
-        -----------
-        
-        All development is done on Github_. Use Issues_ to report
-        problems or submit contributions.
-        
-        .. _Github: https://github.com/influxdb/influxdb-python/
-        .. _Issues: https://github.com/influxdb/influxdb-python/issues
-        
-        Please note that we WILL get to your questions/issues/concerns as quickly as possible. We maintain many
-        software repositories and sometimes things may get pushed to the backburner. Please don't take offense,
-        we will do our best to reply as soon as possible!
-        
-        
-        Source code
-        -----------
-        
-        The source code is currently available on Github: https://github.com/influxdata/influxdb-python
-        
-        
-        TODO
-        ----
-        
-        The TODO/Roadmap can be found in Github bug tracker: https://github.com/influxdata/influxdb-python/issues
-        
-        
-        .. _InfluxDB: https://influxdata.com/time-series-platform/influxdb/
-        .. _Sphinx: http://sphinx.pocoo.org/
-        .. _Tox: https://tox.readthedocs.org
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: test
+The v1 client libraries for InfluxDB were typically developed and maintained by
+community members. For InfluxDB 3.0 users, this library is succeeded by the
+lightweight `v3 client library <https://github.com/InfluxCommunity/influxdb3-python>`_.
+For InfluxDB 2.0 users, look at the `v2 client library
+<https://github.com/influxdata/influxdb-client-python>`_.
+
+If there are still users of this v1 client library, and they or somebody else
+are willing to keep them updated with security fixes at a minimum please reach
+out on the `Community Forums <https://community.influxdata.com/>`_ or
+`InfluxData Slack <https://influxdata.com/slack>`_.
+
+InfluxDB-Python
+===============
+
+.. image:: https://travis-ci.org/influxdata/influxdb-python.svg?branch=master
+    :target: https://travis-ci.org/influxdata/influxdb-python
+.. image:: https://readthedocs.org/projects/influxdb-python/badge/?version=latest&style
+    :target: http://influxdb-python.readthedocs.org/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/coveralls/influxdata/influxdb-python.svg
+  :target: https://coveralls.io/r/influxdata/influxdb-python
+  :alt: Coverage
+
+.. image:: https://img.shields.io/pypi/v/influxdb.svg
+   :target: https://pypi.python.org/pypi/influxdb
+   :alt: PyPI Status
+
+InfluxDB-Python is a client for interacting with InfluxDB_.
+
+**Note: This library is for use with InfluxDB 1.x. For connecting to InfluxDB 2.x instances, please use the the** `influxdb-client-python <https://github.com/influxdata/influxdb-client-python>`_ **client.**
+
+Development of this library is maintained by:
+
++-----------+-------------------------------+
+| Github ID | URL                           |
++===========+===============================+
+| @aviau    | (https://github.com/aviau)    |
++-----------+-------------------------------+
+| @xginn8   | (https://github.com/xginn8)   |
++-----------+-------------------------------+
+| @sebito91 | (https://github.com/sebito91) |
++-----------+-------------------------------+
+
+.. _readme-about:
+
+InfluxDB is an open-source distributed time series database, find more about InfluxDB_ at https://docs.influxdata.com/influxdb/latest
+
+
+.. _installation:
+
+InfluxDB pre v1.1.0 users
+-------------------------
+
+This module is tested with InfluxDB versions: v1.2.4, v1.3.9, v1.4.3, v1.5.4, v1.6.4, and 1.7.4.
+
+Those users still on InfluxDB v0.8.x users may still use the legacy client by importing ``from influxdb.influxdb08 import InfluxDBClient``.
+
+Installation
+------------
+
+Install, upgrade and uninstall influxdb-python with these commands::
+
+    $ pip install influxdb
+    $ pip install --upgrade influxdb
+    $ pip uninstall influxdb
+
+On Debian/Ubuntu, you can install it with this command::
+
+    $ sudo apt-get install python-influxdb
+
+Dependencies
+------------
+
+The influxdb-python distribution is supported and tested on Python 2.7, 3.5, 3.6, 3.7, PyPy and PyPy3.
+
+**Note:** Python <3.5 are currently untested. See ``.travis.yml``.
+
+Main dependency is:
+
+- Requests: HTTP library for human beings (http://docs.python-requests.org/)
+
+
+Additional dependencies are:
+
+- pandas: for writing from and reading to DataFrames (http://pandas.pydata.org/)
+- Sphinx: Tool to create and manage the documentation (http://sphinx-doc.org/)
+- Nose: to auto-discover tests (http://nose.readthedocs.org/en/latest/)
+- Mock: to mock tests (https://pypi.python.org/pypi/mock)
+
+
+Documentation
+-------------
+
+Documentation is available at https://influxdb-python.readthedocs.io/en/latest/.
+
+You will need Sphinx_ installed to generate the documentation.
+
+The documentation can be generated by running::
+
+    $ tox -e docs
+
+
+Generated documentation can be found in the *docs/build/html/* directory.
+
+
+Examples
+--------
+
+Here's a basic example (for more see the examples directory)::
+
+    $ python
+
+    >>> from influxdb import InfluxDBClient
+
+    >>> json_body = [
+        {
+            "measurement": "cpu_load_short",
+            "tags": {
+                "host": "server01",
+                "region": "us-west"
+            },
+            "time": "2009-11-10T23:00:00Z",
+            "fields": {
+                "value": 0.64
+            }
+        }
+    ]
+
+    >>> client = InfluxDBClient('localhost', 8086, 'root', 'root', 'example')
+
+    >>> client.create_database('example')
+
+    >>> client.write_points(json_body)
+
+    >>> result = client.query('select value from cpu_load_short;')
+
+    >>> print("Result: {0}".format(result))
+
+
+Testing
+-------
+
+Make sure you have tox by running the following::
+
+    $ pip install tox
+
+To test influxdb-python with multiple version of Python, you can use Tox_::
+
+    $ tox
+
+
+Support
+-------
+
+For issues with, questions about, or feedback for InfluxDB_, please look into
+our community page: http://influxdb.com/community/.
+
+We are also lurking on the following:
+
+- #influxdb on irc.freenode.net
+- #influxdb on gophers.slack.com
+
+
+Development
+-----------
+
+All development is done on Github_. Use Issues_ to report
+problems or submit contributions.
+
+.. _Github: https://github.com/influxdb/influxdb-python/
+.. _Issues: https://github.com/influxdb/influxdb-python/issues
+
+Please note that we WILL get to your questions/issues/concerns as quickly as possible. We maintain many
+software repositories and sometimes things may get pushed to the backburner. Please don't take offense,
+we will do our best to reply as soon as possible!
+
+
+Source code
+-----------
+
+The source code is currently available on Github: https://github.com/influxdata/influxdb-python
+
+
+TODO
+----
+
+The TODO/Roadmap can be found in Github bug tracker: https://github.com/influxdata/influxdb-python/issues
+
+
+.. _InfluxDB: https://influxdata.com/time-series-platform/influxdb/
+.. _Sphinx: http://sphinx.pocoo.org/
+.. _Tox: https://tox.readthedocs.org
```

### Comparing `influxdb-5.3.1/influxdb/_dataframe_client.py` & `influxdb-5.3.2/influxdb/_dataframe_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,18 +368,18 @@
             "s": 1e9,
             "m": 1e9 * 60,
             "h": 1e9 * 3600,
         }.get(time_precision, 1)
 
         # Make array of timestamp ints
         if isinstance(dataframe.index, pd.PeriodIndex):
-            time = ((dataframe.index.to_timestamp().values.astype(np.int64) /
+            time = ((dataframe.index.to_timestamp().values.astype(np.int64) //
                      precision_factor).astype(np.int64).astype(str))
         else:
-            time = ((pd.to_datetime(dataframe.index).values.astype(np.int64) /
+            time = ((pd.to_datetime(dataframe.index).values.astype(np.int64) //
                      precision_factor).astype(np.int64).astype(str))
 
         # If tag columns exist, make an array of formatted tag keys and values
         if tag_columns:
 
             # Make global_tags as tag_columns
             if global_tags:
```

### Comparing `influxdb-5.3.1/influxdb/chunked_json.py` & `influxdb-5.3.2/influxdb/chunked_json.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/client.py` & `influxdb-5.3.2/influxdb/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import struct
 import time
 from itertools import chain, islice
 
 import msgpack
 import requests
 import requests.exceptions
+from requests.adapters import HTTPAdapter
 from six.moves.urllib.parse import urlparse
 
 from influxdb.line_protocol import make_lines, quote_ident, quote_literal
 from influxdb.resultset import ResultSet
 from .exceptions import InfluxDBClientError
 from .exceptions import InfluxDBServerError
 
@@ -83,14 +84,19 @@
     :type gzip: bool
     :param session: allow for the new client request to use an existing
         requests Session, defaults to None
     :type session: requests.Session
     :param headers: headers to add to Requests, will add 'Content-Type'
         and 'Accept' unless these are already present, defaults to {}
     :type headers: dict
+    :param socket_options: use custom tcp socket options,
+        If not specified, then defaults are loaded from
+        ``HTTPConnection.default_socket_options``
+    :type socket_options: list
+
     :raises ValueError: if cert is provided but ssl is disabled (set to False)
     """
 
     def __init__(self,
                  host='localhost',
                  port=8086,
                  username='root',
@@ -105,14 +111,15 @@
                  proxies=None,
                  pool_size=10,
                  path='',
                  cert=None,
                  gzip=False,
                  session=None,
                  headers=None,
+                 socket_options=None,
                  ):
         """Construct a new InfluxDBClient object."""
         self.__host = host
         self.__port = int(port)
         self._username = username
         self._password = password
         self._database = database
@@ -124,17 +131,18 @@
         self.__use_udp = use_udp
         self.__udp_port = int(udp_port)
 
         if not session:
             session = requests.Session()
 
         self._session = session
-        adapter = requests.adapters.HTTPAdapter(
+        adapter = _SocketOptionsAdapter(
             pool_connections=int(pool_size),
-            pool_maxsize=int(pool_size)
+            pool_maxsize=int(pool_size),
+            socket_options=socket_options
         )
 
         if use_udp:
             self.udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
         if not path:
             self.__path = ''
@@ -175,15 +183,15 @@
         headers.setdefault('Accept', 'application/x-msgpack')
         self._headers = headers
 
         self._gzip = gzip
 
     def __enter__(self):
         """Enter function as used by context manager."""
-        pass
+        return self
 
     def __exit__(self, _exc_type, _exc_value, _traceback):
         """Exit function as used by context manager."""
         self.close()
 
     @property
     def _baseurl(self):
@@ -324,15 +332,18 @@
                 data = compressed.getvalue()
 
         # Try to send the request more than once by default (see #103)
         retry = True
         _try = 0
         while retry:
             try:
-                auth = (self._username, self._password)
+                if "Authorization" in headers:
+                    auth = (None, None)
+                else:
+                    auth = (self._username, self._password)
                 response = self._session.request(
                     method=method,
                     url=url,
                     auth=auth if None not in auth else None,
                     params=params,
                     data=data,
                     stream=stream,
@@ -622,15 +633,15 @@
 
     @staticmethod
     def _batches(iterable, size):
         # Iterate over an iterable producing iterables of batches. Based on:
         # http://code.activestate.com/recipes/303279-getting-items-in-batches/
         iterator = iter(iterable)
         while True:
-            try:        # Try get the first element in the iterator...
+            try:  # Try get the first element in the iterator...
                 head = (next(iterator),)
             except StopIteration:
                 return  # ...so that we can stop if there isn't one
             # Otherwise, lazily slice the rest of the batch
             rest = islice(iterator, size - 1)
             yield chain(head, rest)
 
@@ -1245,7 +1256,20 @@
 def _msgpack_parse_hook(code, data):
     if code == 5:
         (epoch_s, epoch_ns) = struct.unpack(">QI", data)
         timestamp = datetime.datetime.utcfromtimestamp(epoch_s)
         timestamp += datetime.timedelta(microseconds=(epoch_ns / 1000))
         return timestamp.isoformat() + 'Z'
     return msgpack.ExtType(code, data)
+
+
+class _SocketOptionsAdapter(HTTPAdapter):
+    """_SocketOptionsAdapter injects socket_options into HTTP Adapter."""
+
+    def __init__(self, *args, **kwargs):
+        self.socket_options = kwargs.pop("socket_options", None)
+        super(_SocketOptionsAdapter, self).__init__(*args, **kwargs)
+
+    def init_poolmanager(self, *args, **kwargs):
+        if self.socket_options is not None:
+            kwargs["socket_options"] = self.socket_options
+        super(_SocketOptionsAdapter, self).init_poolmanager(*args, **kwargs)
```

### Comparing `influxdb-5.3.1/influxdb/dataframe_client.py` & `influxdb-5.3.2/influxdb/dataframe_client.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/exceptions.py` & `influxdb-5.3.2/influxdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/helper.py` & `influxdb-5.3.2/influxdb/helper.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/influxdb08/chunked_json.py` & `influxdb-5.3.2/influxdb/influxdb08/chunked_json.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/influxdb08/client.py` & `influxdb-5.3.2/influxdb/influxdb08/client.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/influxdb08/dataframe_client.py` & `influxdb-5.3.2/influxdb/influxdb08/dataframe_client.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/influxdb08/helper.py` & `influxdb-5.3.2/influxdb/influxdb08/helper.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/line_protocol.py` & `influxdb-5.3.2/influxdb/line_protocol.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/resultset.py` & `influxdb-5.3.2/influxdb/resultset.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/__init__.py` & `influxdb-5.3.2/influxdb/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/chunked_json_test.py` & `influxdb-5.3.2/influxdb/tests/chunked_json_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/client_test.py` & `influxdb-5.3.2/influxdb/tests/client_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import json
 import mock
 import requests
 import requests.exceptions
 import requests_mock
 
 from nose.tools import raises
+from urllib3.connection import HTTPConnection
 
 from influxdb import InfluxDBClient
 from influxdb.resultset import ResultSet
 
 
 def _build_response_object(status_code=200, content=""):
     resp = requests.Response()
@@ -1394,15 +1395,15 @@
 
     def test_invalid_port_fails(self):
         """Test invalid port fail for TestInfluxDBClient object."""
         with self.assertRaises(ValueError):
             InfluxDBClient('host', '80/redir', 'username', 'password')
 
     def test_chunked_response(self):
-        """Test chunked reponse for TestInfluxDBClient object."""
+        """Test chunked response for TestInfluxDBClient object."""
         example_response = \
             u'{"results":[{"statement_id":0,"series":[{"columns":["key"],' \
             '"values":[["cpu"],["memory"],["iops"],["network"]],"partial":' \
             'true}],"partial":true}]}\n{"results":[{"statement_id":0,' \
             '"series":[{"columns":["key"],"values":[["qps"],["uptime"],' \
             '["df"],["mount"]]}]}]}\n'
 
@@ -1494,14 +1495,48 @@
 
             cli = InfluxDBClient(username=None, password=None,
                                  headers={"Authorization": "my-token"})
             cli.ping()
             self.assertEqual(m.last_request.headers["Authorization"],
                              "my-token")
 
+    def test_custom_socket_options(self):
+        """Test custom socket options."""
+        test_socket_options = HTTPConnection.default_socket_options + \
+            [(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1),
+             (socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, 60),
+             (socket.IPPROTO_TCP, socket.TCP_KEEPCNT, 15)]
+
+        cli = InfluxDBClient(username=None, password=None,
+                             socket_options=test_socket_options)
+
+        self.assertEquals(cli._session.adapters.get("http://").socket_options,
+                          test_socket_options)
+        self.assertEquals(cli._session.adapters.get("http://").poolmanager.
+                          connection_pool_kw.get("socket_options"),
+                          test_socket_options)
+
+        connection_pool = cli._session.adapters.get("http://").poolmanager \
+            .connection_from_url(
+            url="http://localhost:8086")
+        new_connection = connection_pool._new_conn()
+        self.assertEquals(new_connection.socket_options, test_socket_options)
+
+    def test_none_socket_options(self):
+        """Test default socket options."""
+        cli = InfluxDBClient(username=None, password=None)
+        self.assertEquals(cli._session.adapters.get("http://").socket_options,
+                          None)
+        connection_pool = cli._session.adapters.get("http://").poolmanager \
+            .connection_from_url(
+            url="http://localhost:8086")
+        new_connection = connection_pool._new_conn()
+        self.assertEquals(new_connection.socket_options,
+                          HTTPConnection.default_socket_options)
+
 
 class FakeClient(InfluxDBClient):
     """Set up a fake client instance of InfluxDBClient."""
 
     def __init__(self, *args, **kwargs):
         """Initialize an instance of the FakeClient object."""
         super(FakeClient, self).__init__(*args, **kwargs)
```

### Comparing `influxdb-5.3.1/influxdb/tests/dataframe_client_test.py` & `influxdb-5.3.2/influxdb/tests/dataframe_client_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -873,15 +873,15 @@
         """Test query into df for TestDataFrameClient object."""
         data = {
             "results": [{
                 "series": [
                     {"measurement": "network",
                      "tags": {"direction": ""},
                      "columns": ["time", "value"],
-                     "values":[["2009-11-10T23:00:00Z", 23422]]
+                     "values": [["2009-11-10T23:00:00Z", 23422]]
                      },
                     {"measurement": "network",
                      "tags": {"direction": "in"},
                      "columns": ["time", "value"],
                      "values": [["2009-11-10T23:00:00Z", 23422],
                                 ["2009-11-10T23:00:00Z", 23422],
                                 ["2009-11-10T23:00:00Z", 23422]]
@@ -1270,7 +1270,79 @@
                                data_frame_index=["time", "host"])
 
             _data_frame = result['cpu_load_short']
             print(_data_frame)
 
             self.assertListEqual(["time", "host"],
                                  list(_data_frame.index.names))
+
+    def test_dataframe_nanosecond_precision(self):
+        """Test nanosecond precision."""
+        for_df_dict = {
+            "nanFloats": [1.1, float('nan'), 3.3, 4.4],
+            "onlyFloats": [1.1, 2.2, 3.3, 4.4],
+            "strings": ['one_one', 'two_two', 'three_three', 'four_four']
+        }
+        df = pd.DataFrame.from_dict(for_df_dict)
+        df['time'] = ['2019-10-04 06:27:19.850557111+00:00',
+                      '2019-10-04 06:27:19.850557184+00:00',
+                      '2019-10-04 06:27:42.251396864+00:00',
+                      '2019-10-04 06:27:42.251396974+00:00']
+        df['time'] = pd.to_datetime(df['time'], unit='ns')
+        df = df.set_index('time')
+
+        expected = (
+            b'foo nanFloats=1.1,onlyFloats=1.1,strings="one_one" 1570170439850557111\n'  # noqa E501 line too long
+            b'foo onlyFloats=2.2,strings="two_two" 1570170439850557184\n'  # noqa E501 line too long
+            b'foo nanFloats=3.3,onlyFloats=3.3,strings="three_three" 1570170462251396864\n'  # noqa E501 line too long
+            b'foo nanFloats=4.4,onlyFloats=4.4,strings="four_four" 1570170462251396974\n'  # noqa E501 line too long
+        )
+
+        with requests_mock.Mocker() as m:
+            m.register_uri(
+                requests_mock.POST,
+                "http://localhost:8086/write",
+                status_code=204
+            )
+
+            cli = DataFrameClient(database='db')
+            cli.write_points(df, 'foo', time_precision='n')
+
+            self.assertEqual(m.last_request.body, expected)
+
+    def test_dataframe_nanosecond_precision_one_microsecond(self):
+        """Test nanosecond precision within one microsecond."""
+        # 1 microsecond = 1000 nanoseconds
+        start = np.datetime64('2019-10-04T06:27:19.850557000')
+        end = np.datetime64('2019-10-04T06:27:19.850558000')
+
+        # generate timestamps with nanosecond precision
+        timestamps = np.arange(
+            start,
+            end + np.timedelta64(1, 'ns'),
+            np.timedelta64(1, 'ns')
+        )
+        # generate values
+        values = np.arange(0.0, len(timestamps))
+
+        df = pd.DataFrame({'value': values}, index=timestamps)
+        with requests_mock.Mocker() as m:
+            m.register_uri(
+                requests_mock.POST,
+                "http://localhost:8086/write",
+                status_code=204
+            )
+
+            cli = DataFrameClient(database='db')
+            cli.write_points(df, 'foo', time_precision='n')
+
+            lines = m.last_request.body.decode('utf-8').split('\n')
+            self.assertEqual(len(lines), 1002)
+
+            for index, line in enumerate(lines):
+                if index == 1001:
+                    self.assertEqual(line, '')
+                    continue
+                self.assertEqual(
+                    line,
+                    f"foo value={index}.0 157017043985055{7000 + index:04}"
+                )
```

### Comparing `influxdb-5.3.1/influxdb/tests/helper_test.py` & `influxdb-5.3.2/influxdb/tests/helper_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/influxdb08/client_test.py` & `influxdb-5.3.2/influxdb/tests/influxdb08/client_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/influxdb08/dataframe_client_test.py` & `influxdb-5.3.2/influxdb/tests/influxdb08/dataframe_client_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/influxdb08/helper_test.py` & `influxdb-5.3.2/influxdb/tests/influxdb08/helper_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/misc.py` & `influxdb-5.3.2/influxdb/tests/misc.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/resultset_test.py` & `influxdb-5.3.2/influxdb/tests/resultset_test.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/server_tests/base.py` & `influxdb-5.3.2/influxdb/tests/server_tests/base.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/server_tests/client_test_with_server.py` & `influxdb-5.3.2/influxdb/tests/server_tests/client_test_with_server.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/server_tests/influxdb_instance.py` & `influxdb-5.3.2/influxdb/tests/server_tests/influxdb_instance.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb/tests/test_line_protocol.py` & `influxdb-5.3.2/influxdb/tests/test_line_protocol.py`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/influxdb.egg-info/SOURCES.txt` & `influxdb-5.3.2/influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `influxdb-5.3.1/setup.py` & `influxdb-5.3.2/setup.py`

 * *Files identical despite different names*

