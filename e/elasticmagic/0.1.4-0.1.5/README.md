# Comparing `tmp/elasticmagic-0.1.4.tar.gz` & `tmp/elasticmagic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticmagic-0.1.4.tar", last modified: Thu Feb  9 14:25:36 2023, max compression
+gzip compressed data, was "elasticmagic-0.1.5.tar", last modified: Thu Apr 18 10:04:07 2024, max compression
```

## Comparing `elasticmagic-0.1.4.tar` & `elasticmagic-0.1.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    65633 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/document.py
--rw-r--r--   0 runner    (1001) docker     (123)    24240 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/expression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic/ext/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic/ext/asyncio/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/pagination/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/asyncio/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic/ext/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/pagination/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/elasticmagic/ext/queryfilter/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/queryfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/queryfilter/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/ext/queryfilter/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    35968 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/elasticmagic/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 14:25:33.000000 elasticmagic-0.1.4/elasticmagic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.096127 elasticmagic-0.1.4/elasticmagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-09 14:25:36.000000 elasticmagic-0.1.4/elasticmagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-09 14:25:36.000000 elasticmagic-0.1.4/elasticmagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 14:25:36.000000 elasticmagic-0.1.4/elasticmagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-09 14:25:36.000000 elasticmagic-0.1.4/elasticmagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-09 14:25:36.000000 elasticmagic-0.1.4/elasticmagic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/requirements_geo.txt
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-09 14:25:33.000000 elasticmagic-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.092127 elasticmagic-0.1.4/tests_integ/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/tests_integ/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/test_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    25291 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/test_parent_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/asyncio/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:36.100127 elasticmagic-0.1.4/tests_integ/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/general/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-09 14:25:21.000000 elasticmagic-0.1.4/tests_integ/general/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.332306 elasticmagic-0.1.5/elasticmagic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31794 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65571 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/expression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.332306 elasticmagic-0.1.5/elasticmagic/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/elasticmagic/ext/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/elasticmagic/ext/asyncio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/pagination/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/asyncio/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/elasticmagic/ext/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/pagination/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/elasticmagic/ext/queryfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/queryfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/queryfilter/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46209 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/ext/queryfilter/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35909 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/elasticmagic/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 10:04:05.000000 elasticmagic-0.1.5/elasticmagic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.332306 elasticmagic-0.1.5/elasticmagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-18 10:04:07.000000 elasticmagic-0.1.5/elasticmagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-18 10:04:07.000000 elasticmagic-0.1.5/elasticmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:04:07.000000 elasticmagic-0.1.5/elasticmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 10:04:07.000000 elasticmagic-0.1.5/elasticmagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 10:04:07.000000 elasticmagic-0.1.5/elasticmagic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/requirements_geo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-18 10:04:05.000000 elasticmagic-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.328306 elasticmagic-0.1.5/tests_integ/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/tests_integ/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/test_parent_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/asyncio/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:04:07.336306 elasticmagic-0.1.5/tests_integ/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/general/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 10:03:52.000000 elasticmagic-0.1.5/tests_integ/general/test_indexing.py
```

### Comparing `elasticmagic-0.1.4/LICENSE` & `elasticmagic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/PKG-INFO` & `elasticmagic-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticmagic
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python orm for elasticsearch.
 Home-page: https://github.com/anti-social/elasticmagic
 Author: Alexander Koval
 Author-email: kovalidis@gmail.com
 License: Apache License 2.0
 Keywords: elasticsearch dsl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elasticmagic-0.1.4/README.md` & `elasticmagic-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/__init__.py` & `elasticmagic-0.1.5/elasticmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/actions.py` & `elasticmagic-0.1.5/elasticmagic/actions.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/agg.py` & `elasticmagic-0.1.5/elasticmagic/agg.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/attribute.py` & `elasticmagic-0.1.5/elasticmagic/attribute.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/cluster.py` & `elasticmagic-0.1.5/elasticmagic/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABCMeta
 
-from .compat import with_metaclass
 from .compiler import (
     ESVersion,
     get_compiler_by_es_version,
 )
 from .index import Index
 from .result import (
     ClearScrollResult,
@@ -13,15 +12,15 @@
 )
 from .search import SearchQuery
 from .util import clean_params
 
 MAX_RESULT_WINDOW = 10000
 
 
-class BaseCluster(with_metaclass(ABCMeta)):
+class BaseCluster(metaclass=ABCMeta):
     _index_cls = None
     _search_query_cls = None
 
     def __init__(
             self, client, index_cls=None,
             multi_search_raise_on_error=True,
             autodetect_es_version=True, compiler=None,
```

### Comparing `elasticmagic-0.1.4/elasticmagic/compiler.py` & `elasticmagic-0.1.5/elasticmagic/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import operator
 from collections import OrderedDict
 from collections import namedtuple
+from collections.abc import Iterable, Mapping
 from functools import partial
 
 from elasticsearch import ElasticsearchException
 
 from elasticmagic.attribute import AttributedField
-from .compat import Iterable
-from .compat import Mapping
-from .compat import string_types
 from .document import DOC_TYPE_JOIN_FIELD
 from .document import DOC_TYPE_FIELD
 from .document import DOC_TYPE_NAME_FIELD
 from .document import DOC_TYPE_PARENT_FIELD
 from .document import Document
 from .document import DynamicDocument
 from .document import get_doc_type_for_hit
@@ -103,27 +101,27 @@
 ):
     extra_stored_fields = []
     if add_source:
         extra_stored_fields.append('_source')
     extra_stored_fields.extend([DOC_TYPE_NAME_FIELD, DOC_TYPE_PARENT_FIELD])
     if not stored_fields:
         return extra_stored_fields
-    elif isinstance(stored_fields, string_types):
+    elif isinstance(stored_fields, str):
         return [stored_fields] + extra_stored_fields
     elif isinstance(stored_fields, list):
         return stored_fields + extra_stored_fields
     raise ValueError(
         'Unsupported stored_fields type: {}'.format(type(stored_fields))
     )
 
 
 def _patch_stored_fields_in_params(features, params, add_source_field):
     stored_fields_param = features.stored_fields_param
     stored_fields = params.get(stored_fields_param)
-    if isinstance(stored_fields, string_types):
+    if isinstance(stored_fields, str):
         stored_fields = stored_fields.split(',')
     stored_fields = _add_doc_type_fields_into_stored_fields(
         stored_fields, add_source_field
     )
     params[stored_fields_param] = ','.join(stored_fields)
     return params
```

### Comparing `elasticmagic-0.1.4/elasticmagic/datastructures.py` & `elasticmagic-0.1.5/elasticmagic/datastructures.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/document.py` & `elasticmagic-0.1.5/elasticmagic/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from .types import Type, String, Integer, Float, Date
 from .attribute import AttributedField, DynamicAttributedField
 from .attribute import _attributed_field_factory
 from .expression import Field, MappingField
 from .datastructures import OrderedAttributes
 from .util import cached_property
-from .compat import with_metaclass
 
 
 DOC_TYPE_FIELD = '_doc_type'
 DOC_TYPE_NAME_FIELD = '{}.name'.format(DOC_TYPE_FIELD)
 DOC_TYPE_PARENT_FIELD = '{}.parent'.format(DOC_TYPE_FIELD)
 DOC_TYPE_JOIN_FIELD = '_doc_type_join'
 DOC_TYPE_ID_DELIMITER = '~'
@@ -124,15 +123,15 @@
     def wildcard(cls, name):
         return DynamicAttributedField(cls, name, Field(name))
 
     def __getattr__(cls, name):
         return getattr(cls.fields, name)
 
 
-class Document(with_metaclass(DocumentMeta)):
+class Document(metaclass=DocumentMeta):
     __visit_name__ = 'document'
 
     _uid = MappingField(String)
     _id = MappingField(String)
     _type = MappingField(String)
     _source = MappingField(String)
     _all = MappingField(String)
@@ -323,15 +322,15 @@
                 "'{}' class has no attribute '{}'".format(cls, name)
             )
         if name.startswith('_'):
             return super(DynamicDocumentMeta, cls).__getattr__(name)
         return cls.fields[name]
 
 
-class DynamicDocument(with_metaclass(DynamicDocumentMeta, Document)):
+class DynamicDocument(Document, metaclass=DynamicDocumentMeta):
     def _process_source_key_value(self, key, value):
         key, value = (
             super(DynamicDocument, self)._process_source_key_value(key, value)
         )
         if isinstance(value, dict):
             return key, DynamicDocument(**value)
         return key, value
```

### Comparing `elasticmagic-0.1.4/elasticmagic/expression.py` & `elasticmagic-0.1.5/elasticmagic/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 import inspect
 import operator
+from collections.abc import Mapping
 from itertools import count
 
 from .util import clean_params, collect_doc_classes
 from .types import instantiate, Type
-from .compat import string_types, Mapping
 
 
 class Expression(object):
     def _collect_doc_classes(self):
         return set()
 
     def compile(self, compiler):
@@ -598,15 +598,15 @@
 
     _counter = count()
 
     def __init__(self, *args, **kwargs):
         self._name = None
         self._type = None
         if len(args) == 1:
-            if isinstance(args[0], string_types):
+            if isinstance(args[0], str):
                 self._name = args[0]
             elif (
                     isinstance(args[0], Type) or (
                         inspect.isclass(args[0]) and issubclass(args[0], Type)
                     )
             ):
                 self._type = args[0]
```

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/asyncio/cluster.py` & `elasticmagic-0.1.5/elasticmagic/ext/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/asyncio/index.py` & `elasticmagic-0.1.5/elasticmagic/ext/asyncio/index.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/asyncio/pagination/__init__.py` & `elasticmagic-0.1.5/elasticmagic/ext/asyncio/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/asyncio/pagination/flask.py` & `elasticmagic-0.1.5/elasticmagic/ext/asyncio/pagination/flask.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/asyncio/search.py` & `elasticmagic-0.1.5/elasticmagic/ext/asyncio/search.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/pagination/__init__.py` & `elasticmagic-0.1.5/elasticmagic/ext/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/pagination/flask.py` & `elasticmagic-0.1.5/elasticmagic/ext/pagination/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from __future__ import unicode_literals
 
 from abc import ABCMeta
 from math import ceil
 
 from . import SearchQueryWrapper
 from ...cluster import MAX_RESULT_WINDOW
-from ...compat import with_metaclass
 
 
-class BasePagination(with_metaclass(ABCMeta)):
+class BasePagination(metaclass=ABCMeta):
     def _prev_page_params(self):
         return {
             'page': self.prev_num,
             'per_page': self.per_page,
             'max_items': self.max_items,
         }
```

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/queryfilter/__init__.py` & `elasticmagic-0.1.5/elasticmagic/ext/queryfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/queryfilter/codec.py` & `elasticmagic-0.1.5/elasticmagic/ext/queryfilter/codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from collections import defaultdict
 
 import dateutil.parser
 
 from elasticmagic.types import instantiate
 from elasticmagic.types import Type
 from elasticmagic.compat import force_unicode
-from elasticmagic.compat import int_types
 
 
 TIME_ATTRS = {'hour', 'minute', 'second', 'microsecond', 'tzinfo'}
 
 
 class TypeCodec(object):
     def decode(self, value, es_type=None):
@@ -38,15 +37,15 @@
 
     def encode(self, value, es_type=None):
         return value
 
 
 class IntCodec(TypeCodec):
     def encode(self, value, es_type=None):
-        if isinstance(value, int_types):
+        if isinstance(value, int):
             return force_unicode(value)
         return force_unicode(int(value))
 
     def decode(self, value, es_type=None):
         v = int(value)
         if (
                 es_type is not None and
```

### Comparing `elasticmagic-0.1.4/elasticmagic/ext/queryfilter/queryfilter.py` & `elasticmagic-0.1.5/elasticmagic/ext/queryfilter/queryfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import operator
 from math import ceil
 from itertools import chain
 
 from elasticmagic import agg
 from elasticmagic.cluster import MAX_RESULT_WINDOW
-from elasticmagic.compat import text_type, string_types, with_metaclass
 from elasticmagic.expression import Bool, MatchAll, Nested
 from elasticmagic.types import Integer, instantiate
 
 from .codec import SimpleCodec
 
 
 log = logging.getLogger(__name__)
@@ -47,15 +46,15 @@
     def __setattr__(cls, name, value):
         if isinstance(value, UnboundFilter):
             cls._unbound_filters.append((name, value))
         else:
             type.__setattr__(cls, name, value)
 
 
-class QueryFilter(with_metaclass(QueryFilterMeta)):
+class QueryFilter(metaclass=QueryFilterMeta):
     NAME = 'qf'
 
     CONJ_OR = 'CONJ_OR'
     CONJ_AND = 'CONJ_AND'
 
     def __init__(self, name=None, codec=None):
         self._name = name or self.NAME
@@ -164,15 +163,15 @@
     def __init__(self, name, alias):
         self.name = name
         self.alias = alias
 
 
 class BaseFilter(object):
     def __new__(cls, *args, **kwargs):
-        if not args or not isinstance(args[0], string_types):
+        if not args or not isinstance(args[0], str):
             return UnboundFilter(cls, args, kwargs)
         return super(BaseFilter, cls).__new__(cls)
 
     def __init__(self, name, alias=None):
         self.name = name
         self.alias = alias or self.name
         self.qf = None
@@ -443,19 +442,19 @@
         return self.filter.qf._codec.encode_value(self.value)
 
     @property
     def title(self):
         if self._get_title:
             return self._get_title(self)
         if self.instance:
-            return text_type(self.instance)
-        return text_type(self.value)
+            return str(self.instance)
+        return str(self.value)
 
     def __str__(self):
-        return text_type(self.title)
+        return str(self.title)
 
     __unicode__ = __str__
 
 
 class BinaryFilter(BaseFilter):
     def __init__(self, name, condition, p_key=None, p_value=None, alias=None):
         super(BinaryFilter, self).__init__(name, alias=alias)
@@ -549,19 +548,19 @@
         return self.filter.qf._codec.encode_value(self.value)
 
     @property
     def title(self):
         if self.filter._get_title:
             return self.filter._get_title(self)
         if self.instance:
-            return text_type(self.instance)
-        return text_type(self.value)
+            return str(self.instance)
+        return str(self.value)
 
     def __str__(self):
-        return text_type(self.title)
+        return str(self.title)
 
     __unicode__ = __str__
 
 
 class RangeFilter(FieldFilter):
 
     def __init__(
@@ -797,18 +796,18 @@
 
     @property
     def is_default(self):
         return self.value == self.filter.default
 
     @property
     def title(self):
-        return text_type(self.opts.get('title', self.value))
+        return str(self.opts.get('title', self.value))
 
     def __str__(self):
-        return text_type(self.title)
+        return str(self.title)
 
     __unicode__ = __str__
 
 
 class FacetQueryFilter(SimpleQueryFilter):
     def __init__(self, name, *values, **kwargs):
         super(FacetQueryFilter, self).__init__(name, *values, **kwargs)
@@ -951,18 +950,18 @@
 
     @property
     def is_default(self):
         return self.value == self.filter.default
 
     @property
     def title(self):
-        return text_type(self.opts.get('title', self.value))
+        return str(self.opts.get('title', self.value))
 
     def __str__(self):
-        return text_type(self.title)
+        return str(self.title)
 
     __unicode__ = __str__
 
 
 class OrderingValue(BaseFilterValue):
     def __init__(self, value, orderings, _filter=None, **kwargs):
         super(OrderingValue, self).__init__(value, _filter=_filter)
@@ -971,15 +970,15 @@
 
     def bind(self, filter):
         return self.__class__(
             self.value, self.orderings, _filter=filter, **self.opts
         )
 
     def __str__(self):
-        return text_type(self.opts.get('title', self.value))
+        return str(self.opts.get('title', self.value))
 
     __unicode__ = __str__
 
     def _apply(self, query):
         return query.order_by(*self.orderings)
 
 
@@ -1059,15 +1058,15 @@
     def __init__(self, value, selected, is_default, title=None):
         self.value = value
         self.selected = selected
         self.is_default = is_default
         self.title = title
 
     def __str__(self):
-        return text_type(self.title)
+        return str(self.title)
 
     __unicode__ = __str__
 
 
 class PageFilter(BaseFilter):
     DEFAULT_PER_PAGE_PARAM = 'per_page'
     DEFAULT_PER_PAGE = 10
```

### Comparing `elasticmagic-0.1.4/elasticmagic/function.py` & `elasticmagic-0.1.5/elasticmagic/function.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/elasticmagic/index.py` & `elasticmagic-0.1.5/elasticmagic/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import absolute_import
 
 from abc import ABCMeta
 
-from .compat import with_metaclass
 from .document import DynamicDocument
 from .util import to_camel_case
 
 
-class BaseIndex(with_metaclass(ABCMeta)):
+class BaseIndex(metaclass=ABCMeta):
     def __init__(self, cluster, name):
         self._cluster = cluster
         self._name = name
 
         self._doc_cls_cache = {}
 
     def __getitem__(self, doc_type):
```

### Comparing `elasticmagic-0.1.4/elasticmagic/result.py` & `elasticmagic-0.1.5/elasticmagic/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .compat import string_types
 from .document import DynamicDocument
 from .document import get_doc_type_for_hit
 
 
 class Result(object):
     def __init__(self, raw_result):
         self.raw = raw_result
@@ -118,15 +117,15 @@
         super(ActionResult, self).__init__(raw_result)
         self.name = next(iter(raw_result.keys()))
         data = next(iter(raw_result.values()))
         self.status = data['status']
         self.found = data.get('found')
         raw_error = data.get('error')
         if raw_error:
-            if isinstance(raw_error, string_types):
+            if isinstance(raw_error, str):
                 self.error = raw_error
             else:
                 self.error = ErrorReason(raw_error)
         else:
             self.error = None
         self._index = data['_index']
         self._type = data['_type']
```

### Comparing `elasticmagic-0.1.4/elasticmagic/search.py` & `elasticmagic-0.1.5/elasticmagic/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
    from elasticmagic.compiler import Compiler_5_0
    from elasticmagic.compiler import Compiler_7_0
 """
 import warnings
 from abc import ABCMeta
 from collections import namedtuple, OrderedDict
+from collections.abc import Iterable
 
-from .compat import zip, with_metaclass, string_types
-from .compat import Iterable
 from .util import _with_clone
 from .util import merge_params, collect_doc_classes
 from .expression import Params, Source, Highlight, Rescore, Script
 
 __all__ = [
     'BaseSearchQuery', 'SearchQuery', 'SearchQueryContext',
     'FunctionScoreSettings', 'GENERAL_FUNCTION_SCORE', 'BOOST_FUNCTION_SCORE'
@@ -42,15 +41,15 @@
 )
 
 BOOST_FUNCTION_SCORE = FunctionScoreSettings(
     'BOOST', score_mode='sum', boost_mode='sum'
 )
 
 
-class BaseSearchQuery(with_metaclass(ABCMeta)):
+class BaseSearchQuery(metaclass=ABCMeta):
     _q = None
     _source = None
     _fields = None
     _filters = ()
     _filters_meta = ()
     _post_filters = ()
     _post_filters_meta = ()
@@ -466,16 +465,16 @@
     def function_score_settings(self, *function_score_settings):
         """Adds or updates function score level.
         Levels will be inserted before existing.
         """
         function_scores = OrderedDict()
         for fs_settings in function_score_settings:
             if fs_settings.name in self._function_scores:
-                fs = self._function_score[fs_settings.name]
-                self._function_score[fs_settings.name] = _FunctionScore(
+                fs = self._function_scores[fs_settings.name]
+                self._function_scores[fs_settings.name] = _FunctionScore(
                     fs.functions, fs_settings.settings
                 )
             else:
                 function_scores[fs_settings.name] = _FunctionScore(
                     (), fs_settings.settings
                 )
         function_scores.update(self._function_scores)
@@ -974,15 +973,15 @@
             doc_classes = [doc_cls]
         else:
             doc_classes = doc_cls
         self.doc_classes = tuple(doc_classes)
 
         if not search_query._doc_type:
             doc_types = []
-        elif isinstance(search_query._doc_type, string_types):
+        elif isinstance(search_query._doc_type, str):
             doc_types = [
                 t.strip() for t in search_query._doc_type.split(',')
             ]
         else:
             doc_types = list(search_query._doc_type)
         self.doc_types = self._get_unique_doc_types(
             doc_types, self.doc_classes
```

### Comparing `elasticmagic-0.1.4/elasticmagic/types.py` & `elasticmagic-0.1.5/elasticmagic/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 try:
     import geohash
     GEOHASH_IMPORTED = True
 except ImportError:
     GEOHASH_IMPORTED = False
 
-from .compat import binary_type, text_type, string_types
-
 
 def instantiate(typeobj, *args, **kwargs):
     if inspect.isclass(typeobj):
         return typeobj(*args, **kwargs)
     return typeobj
 
 
@@ -45,18 +43,18 @@
     def from_python(self, value, compiler, validate=False):
         return value
 
 
 class String(Type):
     __visit_name__ = 'string'
 
-    python_type = text_type
+    python_type = str
 
     def from_python(self, value, compiler, validate=False):
-        return text_type(value)
+        return str(value)
 
 
 class Keyword(String):
     __visit_name__ = 'keyword'
 
 
 class Text(String):
@@ -172,15 +170,15 @@
     def from_python(self, value, compiler, validate=True):
         return bool(value)
 
 
 class Binary(Type):
     __visit_name__ = 'binary'
 
-    python_type = binary_type
+    python_type = str
 
     def to_python(self, value):
         if value is None:
             return None
         return base64.b64decode(value)
 
     def from_python(self, value, compiler, validate=False):
@@ -199,15 +197,15 @@
     __visit_name__ = 'ip'
 
     IPV4_REGEXP = re.compile(
         r'^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}'
         r'(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$'
     )
 
-    python_type = text_type
+    python_type = str
 
     def from_python(self, value, compiler, validate=False):
         if validate:
             try:
                 if not self.IPV4_REGEXP.match(value):
                     raise ValidationError(
                         'Not valid IPv4 address: {}'.format(value))
@@ -286,15 +284,15 @@
     python_type = dict
 
     def to_python(self, value):
         if value is None:
             return None
         if isinstance(value, (list, tuple)):
             value = list(reversed(value))
-        if isinstance(value, string_types):
+        if isinstance(value, str):
             if self.LAT_LON_SEPARATOR in value:
                 value = list(value.split(self.LAT_LON_SEPARATOR))
             elif GEOHASH_IMPORTED:
                 value = list(geohash.decode(value))
         elif isinstance(value, dict):
             value = [value.get('lat'), value.get('lon')]
         return {'lat': float(value[0]), 'lon': float(value[1])}
```

### Comparing `elasticmagic-0.1.4/elasticmagic/util.py` & `elasticmagic-0.1.5/elasticmagic/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from collections.abc import Iterable, Mapping
 from functools import wraps
 from itertools import chain
 
-from .compat import Iterable, Mapping
-
 
 def _with_clone(fn):
     @wraps(fn)
     def wrapper(self, *args, **kwargs):
         clone = self.clone()
         res = fn(clone, *args, **kwargs)
         if res is not None:
```

### Comparing `elasticmagic-0.1.4/elasticmagic.egg-info/PKG-INFO` & `elasticmagic-0.1.5/elasticmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticmagic
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python orm for elasticsearch.
 Home-page: https://github.com/anti-social/elasticmagic
 Author: Alexander Koval
 Author-email: kovalidis@gmail.com
 License: Apache License 2.0
 Keywords: elasticsearch dsl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elasticmagic-0.1.4/elasticmagic.egg-info/SOURCES.txt` & `elasticmagic-0.1.5/elasticmagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/setup.py` & `elasticmagic-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="elasticmagic",
-    version="0.1.4",
+    version="0.1.5",
     author="Alexander Koval",
     author_email="kovalidis@gmail.com",
     description=("Python orm for elasticsearch."),
     license="Apache License 2.0",
     keywords="elasticsearch dsl",
     url="https://github.com/anti-social/elasticmagic",
     packages=find_packages(exclude=["tests", "tests_integ"]),
```

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/conftest.py` & `elasticmagic-0.1.5/tests_integ/asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/test_bulk.py` & `elasticmagic-0.1.5/tests_integ/asyncio/test_bulk.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/test_index.py` & `elasticmagic-0.1.5/tests_integ/asyncio/test_index.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/test_pagination.py` & `elasticmagic-0.1.5/tests_integ/asyncio/test_pagination.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/test_parent_child.py` & `elasticmagic-0.1.5/tests_integ/asyncio/test_parent_child.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/asyncio/test_search.py` & `elasticmagic-0.1.5/tests_integ/asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/general/conftest.py` & `elasticmagic-0.1.5/tests_integ/general/conftest.py`

 * *Files identical despite different names*

### Comparing `elasticmagic-0.1.4/tests_integ/general/test_indexing.py` & `elasticmagic-0.1.5/tests_integ/general/test_indexing.py`

 * *Files identical despite different names*

