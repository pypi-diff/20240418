# Comparing `tmp/sqlalchemy-bigquery-1.8.0.tar.gz` & `tmp/sqlalchemy-bigquery-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-bigquery-1.8.0.tar", last modified: Tue Aug 15 13:37:25 2023, max compression
+gzip compressed data, was "sqlalchemy-bigquery-1.9.0.tar", last modified: Mon Dec 11 23:09:20 2023, max compression
```

## Comparing `sqlalchemy-bigquery-1.8.0.tar` & `sqlalchemy-bigquery-1.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.114329 sqlalchemy-bigquery-1.8.0/
--rw-rw-r--   0 root         (0)     1003      622 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/AUTHORS
--rw-rw-r--   0 root         (0)     1003     1064 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003    12530 2023-08-15 13:37:25.114329 sqlalchemy-bigquery-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    11372 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/README.rst
--rw-rw-r--   0 root         (0)     1003      300 2023-08-15 13:37:25.114329 sqlalchemy-bigquery-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     4671 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.106328 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/
--rw-rw-r--   0 root         (0)     1003     2258 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/__init__.py
--rw-rw-r--   0 root         (0)     1003     2412 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_helpers.py
--rw-rw-r--   0 root         (0)     1003     4943 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_struct.py
--rw-rw-r--   0 root         (0)     1003     4717 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_types.py
--rw-rw-r--   0 root         (0)     1003    40051 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/base.py
--rw-rw-r--   0 root         (0)     1003     8638 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/geography.py
--rw-rw-r--   0 root         (0)     1003     9854 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/parse_url.py
--rw-rw-r--   0 root         (0)     1003     7361 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/requirements.py
--rw-rw-r--   0 root         (0)     1003     1131 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.106328 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/
--rw-r--r--   0 root         (0)     1003    12530 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1615 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       69 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003      599 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       20 2023-08-15 13:37:25.000000 sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.106328 sqlalchemy-bigquery-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003        0 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1574 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.106328 sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/
--rw-rw-r--   0 root         (0)     1003      600 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/README.rst
--rw-rw-r--   0 root         (0)     1003     3368 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/conftest.py
--rw-rw-r--   0 root         (0)     1003    10371 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.110329 sqlalchemy-bigquery-1.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003     1108 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     5884 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.110329 sqlalchemy-bigquery-1.8.0/tests/system/data/
--rw-rw-r--   0 root         (0)     1003   200036 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/data/sample.json
--rw-rw-r--   0 root         (0)     1003      340 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/data/sample_one_row.json
--rw-rw-r--   0 root         (0)     1003     1481 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/data/schema.json
--rw-rw-r--   0 root         (0)     1003     6219 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/test__struct.py
--rw-rw-r--   0 root         (0)     1003     6542 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/test_alembic.py
--rw-rw-r--   0 root         (0)     1003     8790 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/test_geography.py
--rw-rw-r--   0 root         (0)     1003     3231 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/test_helpers.py
--rw-rw-r--   0 root         (0)     1003    29222 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/system/test_sqlalchemy_bigquery.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-08-15 13:37:25.114329 sqlalchemy-bigquery-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003     3648 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/conftest.py
--rw-rw-r--   0 root         (0)     1003    16729 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/fauxdbi.py
--rw-rw-r--   0 root         (0)     1003     5231 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test__struct.py
--rw-rw-r--   0 root         (0)     1003    10392 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_catalog_functions.py
--rw-rw-r--   0 root         (0)     1003     3578 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_comments.py
--rw-rw-r--   0 root         (0)     1003     4263 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_compiler.py
--rw-rw-r--   0 root         (0)     1003     7047 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_compliance.py
--rw-rw-r--   0 root         (0)     1003     1632 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_dialect_types.py
--rw-rw-r--   0 root         (0)     1003     2815 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_engine.py
--rw-rw-r--   0 root         (0)     1003     5838 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_geography.py
--rw-rw-r--   0 root         (0)     1003     7821 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_helpers.py
--rw-rw-r--   0 root         (0)     1003     1963 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_like_reescape.py
--rw-rw-r--   0 root         (0)     1003     8633 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_parse_url.py
--rw-rw-r--   0 root         (0)     1003    17303 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_select.py
--rw-rw-r--   0 root         (0)     1003     8283 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_sqlalchemy_bigquery.py
--rw-rw-r--   0 root         (0)     1003     1386 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_version.py
--rw-rw-r--   0 root         (0)     1003     1647 2023-08-15 13:34:44.000000 sqlalchemy-bigquery-1.8.0/tests/unit/test_view.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.818292 sqlalchemy-bigquery-1.9.0/
+-rw-rw-r--   0 root         (0)     1003      622 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/AUTHORS
+-rw-rw-r--   0 root         (0)     1003     1064 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003    13742 2023-12-11 23:09:20.818292 sqlalchemy-bigquery-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    11372 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/README.rst
+-rw-rw-r--   0 root         (0)     1003      300 2023-12-11 23:09:20.818292 sqlalchemy-bigquery-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     4672 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.806292 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/
+-rw-rw-r--   0 root         (0)     1003     2258 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2412 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     4943 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_struct.py
+-rw-rw-r--   0 root         (0)     1003     4717 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_types.py
+-rw-rw-r--   0 root         (0)     1003    40048 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/base.py
+-rw-rw-r--   0 root         (0)     1003     8638 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/geography.py
+-rw-rw-r--   0 root         (0)     1003     9854 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/parse_url.py
+-rw-rw-r--   0 root         (0)     1003     7361 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/requirements.py
+-rw-rw-r--   0 root         (0)     1003     1131 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.806292 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/
+-rw-r--r--   0 root         (0)     1003    13742 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1615 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       69 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003      599 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-12-11 23:09:20.000000 sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.806292 sqlalchemy-bigquery-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1574 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.806292 sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/
+-rw-rw-r--   0 root         (0)     1003      600 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/README.rst
+-rw-rw-r--   0 root         (0)     1003     3368 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/conftest.py
+-rw-rw-r--   0 root         (0)     1003    10370 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.810292 sqlalchemy-bigquery-1.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     1108 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5884 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.810292 sqlalchemy-bigquery-1.9.0/tests/system/data/
+-rw-rw-r--   0 root         (0)     1003   200036 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/data/sample.json
+-rw-rw-r--   0 root         (0)     1003      340 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/data/sample_one_row.json
+-rw-rw-r--   0 root         (0)     1003     1481 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/data/schema.json
+-rw-rw-r--   0 root         (0)     1003     6219 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/test__struct.py
+-rw-rw-r--   0 root         (0)     1003     6542 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/test_alembic.py
+-rw-rw-r--   0 root         (0)     1003     8790 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/test_geography.py
+-rw-rw-r--   0 root         (0)     1003     3231 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003    29222 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/system/test_sqlalchemy_bigquery.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-12-11 23:09:20.814292 sqlalchemy-bigquery-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3648 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/conftest.py
+-rw-rw-r--   0 root         (0)     1003    16728 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/fauxdbi.py
+-rw-rw-r--   0 root         (0)     1003     5231 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test__struct.py
+-rw-rw-r--   0 root         (0)     1003    10392 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_catalog_functions.py
+-rw-rw-r--   0 root         (0)     1003     3578 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_comments.py
+-rw-rw-r--   0 root         (0)     1003     4263 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_compiler.py
+-rw-rw-r--   0 root         (0)     1003     7047 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_compliance.py
+-rw-rw-r--   0 root         (0)     1003     1632 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_dialect_types.py
+-rw-rw-r--   0 root         (0)     1003     2815 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_engine.py
+-rw-rw-r--   0 root         (0)     1003     5838 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_geography.py
+-rw-rw-r--   0 root         (0)     1003     7821 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1961 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_like_reescape.py
+-rw-rw-r--   0 root         (0)     1003     8633 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_parse_url.py
+-rw-rw-r--   0 root         (0)     1003    17303 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_select.py
+-rw-rw-r--   0 root         (0)     1003     8283 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_sqlalchemy_bigquery.py
+-rw-rw-r--   0 root         (0)     1003     1386 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_version.py
+-rw-rw-r--   0 root         (0)     1003     1647 2023-12-11 23:06:53.000000 sqlalchemy-bigquery-1.9.0/tests/unit/test_view.py
```

### Comparing `sqlalchemy-bigquery-1.8.0/AUTHORS` & `sqlalchemy-bigquery-1.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/LICENSE` & `sqlalchemy-bigquery-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/MANIFEST.in` & `sqlalchemy-bigquery-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/PKG-INFO` & `sqlalchemy-bigquery-1.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlalchemy-bigquery
-Version: 1.8.0
-Summary: SQLAlchemy dialect for BigQuery
-Home-page: https://github.com/googleapis/python-bigquery-sqlalchemy
-Author: The Sqlalchemy-Bigquery Authors
-Author-email: googleapis-packages@google.com
-Keywords: bigquery,sqlalchemy
-Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Database :: Front-Ends
-Obsoletes: pybigquery
-Requires-Python: >=3.7, <3.12
-Description-Content-Type: text/x-rst
-Provides-Extra: geography
-Provides-Extra: alembic
-Provides-Extra: tests
-Provides-Extra: bqstorage
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS
-
 SQLAlchemy Dialect for BigQuery
 ===============================
 
 |GA| |pypi| |versions|
 
 `SQLALchemy Dialects`_
 
@@ -81,19 +49,19 @@
 dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
-Python >= 3.7
+Python >= 3.8
 
 Unsupported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Python <= 3.6.
+Python <= 3.7.
 
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
```

### Comparing `sqlalchemy-bigquery-1.8.0/setup.py` & `sqlalchemy-bigquery-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,19 +80,19 @@
     keywords=["bigquery", "sqlalchemy"],
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
         "Topic :: Database :: Front-Ends",
     ],
     platforms="Posix; MacOS X; Windows",
     install_requires=[
         "google-api-core >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
         # NOTE: Maintainers, please do not require google-auth>=2.x.x
@@ -100,15 +100,15 @@
         # https://github.com/googleapis/google-cloud-python/issues/10566
         "google-auth>=1.25.0,<3.0.0dev",  # Work around pip wack.
         "google-cloud-bigquery>=2.25.2,<4.0.0dev",
         "packaging",
         "sqlalchemy>=1.2.0,<2.0.0dev",
     ],
     extras_require=extras,
-    python_requires=">=3.7, <3.12",
+    python_requires=">=3.8, <3.13",
     tests_require=["packaging", "pytz"],
     entry_points={
         "sqlalchemy.dialects": ["bigquery = sqlalchemy_bigquery:BigQueryDialect"]
     },
     # Document that this replaces pybigquery, however, this isn't
     # enforced by pip, because doing so would allow rogue packages to
     # obsolete legitimate ones.
```

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/__init__.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_helpers.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_struct.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_struct.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/_types.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/base.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
     def pre_exec(self):
         self.statement = self.__distribute_types_to_expanded_placeholders(
             self.__remove_type_from_empty_in(self.statement)
         )
 
 
 class BigQueryCompiler(_struct.SQLCompiler, SQLCompiler):
-
     compound_keywords = SQLCompiler.compound_keywords.copy()
     compound_keywords[selectable.CompoundSelect.UNION] = "UNION DISTINCT"
     compound_keywords[selectable.CompoundSelect.UNION_ALL] = "UNION ALL"
 
     def __init__(self, dialect, statement, *args, **kwargs):
         if isinstance(statement, Column):
             kwargs["compile_kwargs"] = util.immutabledict({"include_table": False})
@@ -620,15 +619,14 @@
             else "NUMERIC"
         ) + suffix
 
     visit_DECIMAL = visit_NUMERIC
 
 
 class BigQueryDDLCompiler(DDLCompiler):
-
     # BigQuery has no support for foreign keys.
     def visit_foreign_key_constraint(self, constraint):
         return None
 
     # BigQuery has no support for primary keys.
     def visit_primary_key_constraint(self, constraint):
         return None
@@ -719,15 +717,14 @@
 
     def literal_processor(self, dialect):
         return self.process_timestamp_literal
 
 
 class BQArray(sqlalchemy.sql.sqltypes.ARRAY):
     def literal_processor(self, dialect):
-
         item_processor = self.item_type._cached_literal_processor(dialect)
         if not item_processor:
             raise NotImplementedError(
                 f"Don't know how to literal-quote values of type {self.item_type}"
             )
 
         def process_array_literal(value):
```

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/geography.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/geography.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/parse_url.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/parse_url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/requirements.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery/version.py` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
```

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/PKG-INFO` & `sqlalchemy-bigquery-1.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,61 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bigquery
-Version: 1.8.0
+Version: 1.9.0
 Summary: SQLAlchemy dialect for BigQuery
 Home-page: https://github.com/googleapis/python-bigquery-sqlalchemy
 Author: The Sqlalchemy-Bigquery Authors
 Author-email: googleapis-packages@google.com
 Keywords: bigquery,sqlalchemy
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Obsoletes: pybigquery
-Requires-Python: >=3.7, <3.12
+Requires-Python: >=3.8, <3.13
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+Requires-Dist: google-api-core!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0,<3.0.0dev,>=1.31.5
+Requires-Dist: google-auth<3.0.0dev,>=1.25.0
+Requires-Dist: google-cloud-bigquery<4.0.0dev,>=2.25.2
+Requires-Dist: packaging
+Requires-Dist: sqlalchemy<2.0.0dev,>=1.2.0
 Provides-Extra: geography
+Requires-Dist: GeoAlchemy2; extra == "geography"
+Requires-Dist: shapely; extra == "geography"
 Provides-Extra: alembic
+Requires-Dist: alembic; extra == "alembic"
 Provides-Extra: tests
+Requires-Dist: packaging; extra == "tests"
+Requires-Dist: pytz; extra == "tests"
 Provides-Extra: bqstorage
+Requires-Dist: google-cloud-bigquery-storage<3.0.0dev,>=2.0.0; extra == "bqstorage"
+Requires-Dist: grpcio<2.0dev,>=1.47.0; extra == "bqstorage"
+Requires-Dist: grpcio<2.0dev,>=1.49.1; python_version >= "3.11" and extra == "bqstorage"
+Requires-Dist: pyarrow>=3.0.0; extra == "bqstorage"
 Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS
+Requires-Dist: alembic; extra == "all"
+Requires-Dist: GeoAlchemy2; extra == "all"
+Requires-Dist: google-cloud-bigquery-storage<3.0.0dev,>=2.0.0; extra == "all"
+Requires-Dist: grpcio<2.0dev,>=1.47.0; extra == "all"
+Requires-Dist: shapely; extra == "all"
+Requires-Dist: packaging; extra == "all"
+Requires-Dist: pytz; extra == "all"
+Requires-Dist: grpcio<2.0dev,>=1.49.1; python_version >= "3.11" and extra == "all"
+Requires-Dist: pyarrow>=3.0.0; extra == "all"
 
 SQLAlchemy Dialect for BigQuery
 ===============================
 
 |GA| |pypi| |versions|
 
 `SQLALchemy Dialects`_
@@ -81,19 +104,19 @@
 dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
-Python >= 3.7
+Python >= 3.8
 
 Unsupported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
-Python <= 3.6.
+Python <= 3.7.
 
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
```

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/SOURCES.txt` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/sqlalchemy_bigquery.egg-info/requires.txt` & `sqlalchemy-bigquery-1.9.0/sqlalchemy_bigquery.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packaging
 sqlalchemy<2.0.0dev,>=1.2.0
 
 [alembic]
 alembic
 
 [all]
-google-cloud-bigquery-storage<3.0.0dev,>=2.0.0
 alembic
-pytz
+GeoAlchemy2
+google-cloud-bigquery-storage<3.0.0dev,>=2.0.0
 grpcio<2.0dev,>=1.47.0
 shapely
-GeoAlchemy2
 packaging
+pytz
 pyarrow>=3.0.0
 
 [all:python_version >= "3.11"]
 grpcio<2.0dev,>=1.49.1
 
 [bqstorage]
 google-cloud-bigquery-storage<3.0.0dev,>=2.0.0
```

### Comparing `sqlalchemy-bigquery-1.8.0/tests/conftest.py` & `sqlalchemy-bigquery-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/README.rst` & `sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/conftest.py` & `sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py` & `sqlalchemy-bigquery-1.9.0/tests/sqlalchemy_dialect_compliance/test_dialect_compliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         @pytest.mark.skip("BigQuery doesn't allow an offset without a limit.")
         def test_simple_offset(self):
             pass
 
         test_bound_offset = test_simple_offset
 
     class TimestampMicrosecondsTest(_TimestampMicrosecondsTest):
-
         data = datetime.datetime(2012, 10, 15, 12, 57, 18, 396, tzinfo=pytz.UTC)
 
         def test_literal(self):
             # The base tests doesn't set up the literal properly, because
             # it doesn't pass its datatype to `literal`.
 
             def literal(value):
```

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/__init__.py` & `sqlalchemy-bigquery-1.9.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/conftest.py` & `sqlalchemy-bigquery-1.9.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/data/sample.json` & `sqlalchemy-bigquery-1.9.0/tests/system/data/sample.json`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/data/schema.json` & `sqlalchemy-bigquery-1.9.0/tests/system/data/schema.json`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/test__struct.py` & `sqlalchemy-bigquery-1.9.0/tests/system/test__struct.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/test_alembic.py` & `sqlalchemy-bigquery-1.9.0/tests/system/test_alembic.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/test_geography.py` & `sqlalchemy-bigquery-1.9.0/tests/system/test_geography.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/test_helpers.py` & `sqlalchemy-bigquery-1.9.0/tests/system/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/system/test_sqlalchemy_bigquery.py` & `sqlalchemy-bigquery-1.9.0/tests/system/test_sqlalchemy_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/conftest.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/fauxdbi.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/fauxdbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,14 @@
         if name not in self:
             self[name] = attrdict()
         return self[name]
 
 
 class FauxClient:
     def __init__(self, project_id=None, default_query_job_config=None, *args, **kw):
-
         if project_id is None:
             if default_query_job_config is not None:
                 project_id = default_query_job_config.default_dataset.project
             else:
                 project_id = "authproj"  # we would still have gotten it from auth.
 
         self.project = project_id
```

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test__struct.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test__struct.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_catalog_functions.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_catalog_functions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_comments.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_comments.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_compiler.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_compiler.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_compliance.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_compliance.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_dialect_types.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_dialect_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_engine.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_engine.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_geography.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_geography.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_helpers.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_like_reescape.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_like_reescape.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,22 @@
 
 import sqlalchemy.sql.operators
 import sqlalchemy.sql.schema
 import sqlalchemy_bigquery.base
 
 
 def _check(raw, escaped, escape=None, autoescape=True):
-
     col = sqlalchemy.sql.schema.Column()
     op = col.contains(raw, escape=escape, autoescape=autoescape)
     o2 = sqlalchemy_bigquery.base.BigQueryCompiler._maybe_reescape(op)
     assert o2.left.__dict__ == op.left.__dict__
     assert not o2.modifiers.get("escape")
 
     assert o2.right.value == escaped
 
 
 def test_like_autoescape_reescape():
-
     _check("ab%cd", "ab\\%cd")
     _check("ab%c_d", "ab\\%c\\_d")
     _check("ab%cd", "ab%cd", autoescape=False)
     _check("ab%c_d", "ab\\%c\\_d", escape="\\")
     _check("ab/%c/_/d", "ab/\\%c/\\_/d")
```

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_parse_url.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_parse_url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_select.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_select.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_sqlalchemy_bigquery.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_sqlalchemy_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_version.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-bigquery-1.8.0/tests/unit/test_view.py` & `sqlalchemy-bigquery-1.9.0/tests/unit/test_view.py`

 * *Files identical despite different names*

