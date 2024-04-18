# Comparing `tmp/django_loose_fk-1.1.0.tar.gz` & `tmp/django_loose_fk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_loose_fk-1.1.0.tar", last modified: Wed Apr 17 09:57:20 2024, max compression
+gzip compressed data, was "django_loose_fk-1.1.1.tar", last modified: Thu Apr 18 12:10:17 2024, max compression
```

## Comparing `django_loose_fk-1.1.0.tar` & `django_loose_fk-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.541281 django_loose_fk-1.1.0/django_loose_fk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/drf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/django_loose_fk/inspectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/lookups.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/query_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/django_loose_fk/virtual_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/django_loose_fk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 09:57:20.000000 django_loose_fk-1.1.0/django_loose_fk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.545281 django_loose_fk-1.1.0/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0002_auto_20220310_1612.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/0003_auto_20230705_0917.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:20.549281 django_loose_fk-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_chain_loose_fk.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_is_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_model_field_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_model_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_querying.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_querylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_serializer_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 09:57:16.000000 django_loose_fk-1.1.0/tests/test_system_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.212262 django_loose_fk-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-18 12:10:17.212262 django_loose_fk-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.208262 django_loose_fk-1.1.1/django_loose_fk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/drf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.208262 django_loose_fk-1.1.1/django_loose_fk/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/query_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/django_loose_fk/virtual_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.212262 django_loose_fk-1.1.1/django_loose_fk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 12:10:17.000000 django_loose_fk-1.1.1/django_loose_fk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 12:10:17.216262 django_loose_fk-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.208262 django_loose_fk-1.1.1/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.208262 django_loose_fk-1.1.1/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/migrations/0002_auto_20220310_1612.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/migrations/0003_auto_20230705_0917.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/migrations/0004_zaakobjectfk.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:17.212262 django_loose_fk-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_chain_loose_fk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_is_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_model_field_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_model_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_querying.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_querylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_serializer_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 12:10:07.000000 django_loose_fk-1.1.1/tests/test_system_checks.py
```

### Comparing `django_loose_fk-1.1.0/CHANGELOG.rst` & `django_loose_fk-1.1.1/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.1.1 (2024-04-18)
+==================
+
+* Support related fields in the `FkOrUrlFieldFilter` field_name (#37)
+
 1.1.0 (2024-04-15)
 ==================
 
 * Supported Django 4.2
 * Supported python 3.11
 * Dropped support of python 3.7, python 3.8, python 3.9
```

### Comparing `django_loose_fk-1.1.0/LICENSE` & `django_loose_fk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/PKG-INFO` & `django_loose_fk-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,15 +44,15 @@
 Provides-Extra: release
 Requires-Dist: bump2version; extra == "release"
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.1.0
+:Version: 1.1.1
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django_loose_fk-1.1.0/README.rst` & `django_loose_fk-1.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.1.0
+:Version: 1.1.1
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django_loose_fk-1.1.0/django_loose_fk/apps.py` & `django_loose_fk-1.1.1/django_loose_fk/apps.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/checks.py` & `django_loose_fk-1.1.1/django_loose_fk/checks.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/constraints.py` & `django_loose_fk-1.1.1/django_loose_fk/constraints.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/drf.py` & `django_loose_fk-1.1.1/django_loose_fk/drf.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/fields.py` & `django_loose_fk-1.1.1/django_loose_fk/fields.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/filters.py` & `django_loose_fk-1.1.1/django_loose_fk/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,31 +51,47 @@
 
         values = value
         if not isinstance(values, list):
             values = [values]
 
         parsed_values = [urlparse(value) for value in values]
         host = self.parent.request.get_host()
-        model_field = self.model._meta.get_field(self.field_name)
 
-        filters = self.get_filters(model_field, parsed_values, host)
+        model_field_list = self.field_name.split("__")
+        model_field_path = (
+            f"{self.field_name.rsplit('__', 1)[0]}__"
+            if len(model_field_list) > 1
+            else None
+        )
+        model_field = self.model._meta.get_field(model_field_list.pop(0))
+
+        for field_name in model_field_list:
+            model_field = model_field.target_field.model._meta.get_field(field_name)
+
+        filters = self.get_filters(model_field, parsed_values, host, model_field_path)
 
         # In case the query contained both local and remote zaaktypen, then the filters dict will be
         # {'_zaaktype__in': ['url'], 'externe_zaaktype__in': ['url']}. These filters need to be OR'd
         complex_filter = Q()
         for lookup, value in filters.items():
             complex_filter |= Q(**{lookup: value})
 
         qs = self.get_method(qs)(complex_filter)
         return qs.distinct() if self.distinct else qs
 
-    def get_filters(self, model_field, parsed_values, host) -> dict:
+    def get_filters(
+        self, model_field, parsed_values, host, model_field_path=None
+    ) -> dict:
         local_filter_key = f"{model_field.fk_field}__{self.lookup_expr}"
         external_filter_key = f"{model_field.url_field}__{self.lookup_expr}"
 
+        if model_field_path:
+            local_filter_key = model_field_path + local_filter_key
+            external_filter_key = model_field_path + external_filter_key
+
         filters = {}
         for value in parsed_values:
             local = is_local(host, value.geturl())
             if local:
                 local_object = get_resource_for_path(value.path)
                 if self.instance_path:
                     for bit in self.instance_path.split("."):
```

### Comparing `django_loose_fk-1.1.0/django_loose_fk/inspectors/fields.py` & `django_loose_fk-1.1.1/django_loose_fk/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/inspectors/query.py` & `django_loose_fk-1.1.1/django_loose_fk/inspectors/query.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/loaders.py` & `django_loose_fk-1.1.1/django_loose_fk/loaders.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/lookups.py` & `django_loose_fk-1.1.1/django_loose_fk/lookups.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/query_list.py` & `django_loose_fk-1.1.1/django_loose_fk/query_list.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/utils.py` & `django_loose_fk-1.1.1/django_loose_fk/utils.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk/virtual_models.py` & `django_loose_fk-1.1.1/django_loose_fk/virtual_models.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/django_loose_fk.egg-info/PKG-INFO` & `django_loose_fk-1.1.1/django_loose_fk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,15 +44,15 @@
 Provides-Extra: release
 Requires-Dist: bump2version; extra == "release"
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.1.0
+:Version: 1.1.1
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django_loose_fk-1.1.0/django_loose_fk.egg-info/SOURCES.txt` & `django_loose_fk-1.1.1/django_loose_fk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 testapp/loaders.py
 testapp/models.py
 testapp/settings.py
 testapp/urls.py
 testapp/migrations/0001_initial.py
 testapp/migrations/0002_auto_20220310_1612.py
 testapp/migrations/0003_auto_20230705_0917.py
+testapp/migrations/0004_zaakobjectfk.py
 testapp/migrations/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/test_api.py
 tests/test_api_docs.py
 tests/test_chain_loose_fk.py
 tests/test_compare.py
```

### Comparing `django_loose_fk-1.1.0/setup.cfg` & `django_loose_fk-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-loose-fk
-version = 1.1.0
+version = 1.1.1
 description = Django Loose FK handles local or remote "ForeignKey" references.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-loose-fk
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = ForeignKey, URL reference, decentralization, integrity
```

### Comparing `django_loose_fk-1.1.0/testapp/api.py` & `django_loose_fk-1.1.1/testapp/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django_filters.rest_framework.backends import DjangoFilterBackend
 from django_filters.rest_framework.filterset import FilterSet
 from rest_framework import routers, serializers, viewsets
 
 from django_loose_fk.filters import FkOrUrlFieldFilter
 
-from .models import Zaak, ZaakObject, ZaakType
+from .models import Zaak, ZaakObject, ZaakObjectFk, ZaakType
 
 # Serializers
 
 
 class ZaakTypeSerializer(serializers.HyperlinkedModelSerializer):
     class Meta:
         model = ZaakType
@@ -23,14 +23,20 @@
 
 class ZaakObjectSerializer(serializers.HyperlinkedModelSerializer):
     class Meta:
         model = ZaakObject
         fields = ("url", "zaak", "name")
 
 
+class ZaakObjectFkSerializer(serializers.HyperlinkedModelSerializer):
+    class Meta:
+        model = ZaakObjectFk
+        fields = ("zaak_object", "name")
+
+
 # Filters
 
 
 class ZaakFilterSet(FilterSet):
     class Meta:
         model = Zaak
         fields = {
@@ -42,14 +48,25 @@
     zaak = FkOrUrlFieldFilter(queryset=ZaakObject.objects.all())
 
     class Meta:
         model = ZaakObject
         fields = ("zaak",)
 
 
+class ZaakObjectFkFilterset(FilterSet):
+    zaak = FkOrUrlFieldFilter(
+        queryset=ZaakObjectFk.objects.all(),
+        field_name="zaak_object__zaak",
+    )
+
+    class Meta:
+        model = ZaakObjectFk
+        fields = ("zaak",)
+
+
 # Viewsets
 
 
 class NoAuthMixin:
     def perform_authentication(self, request):
         pass
 
@@ -68,13 +85,21 @@
 
 class ZaakObjectViewSet(NoAuthMixin, viewsets.ModelViewSet):
     queryset = ZaakObject.objects.all()
     serializer_class = ZaakObjectSerializer
     filterset_class = ZaakObjectFilterset
 
 
+class ZaakObjectFkViewSet(NoAuthMixin, viewsets.ModelViewSet):
+    queryset = ZaakObjectFk.objects.all()
+    filter_backends = (DjangoFilterBackend,)
+    serializer_class = ZaakObjectFkSerializer
+    filterset_class = ZaakObjectFkFilterset
+
+
 # URL routing
 
 router = routers.DefaultRouter()
 router.register("zaaktypes", ZaakTypeViewSet)
 router.register("zaken", ZaakViewSet)
 router.register("zaakobjecten", ZaakObjectViewSet)
+router.register("zaakobjectfk", ZaakObjectFkViewSet)
```

### Comparing `django_loose_fk-1.1.0/testapp/migrations/0001_initial.py` & `django_loose_fk-1.1.1/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/testapp/migrations/0002_auto_20220310_1612.py` & `django_loose_fk-1.1.1/testapp/migrations/0002_auto_20220310_1612.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/testapp/migrations/0003_auto_20230705_0917.py` & `django_loose_fk-1.1.1/testapp/migrations/0003_auto_20230705_0917.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/testapp/models.py` & `django_loose_fk-1.1.1/testapp/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 
 class ZaakObject2(models.Model):
     _zaak = models.ForeignKey("Zaak", null=True, blank=True, on_delete=models.PROTECT)
     extern_zaak = models.URLField(blank=True)
     zaak = FkOrURLField(fk_field="_zaak", url_field="extern_zaak")
 
 
+class ZaakObjectFk(models.Model):
+    name = models.CharField(max_length=80, null=True, blank=True)
+    zaak_object = models.ForeignKey(
+        "ZaakObject", null=True, blank=True, on_delete=models.PROTECT
+    )
+
+
 class DummyModel(models.Model):
     _zaaktype1 = models.ForeignKey(
         "ZaakType", null=True, blank=True, on_delete=models.PROTECT, related_name="+"
     )
     extern_zaaktype1 = models.URLField(blank=True)
     zaaktype1 = FkOrURLField(fk_field="_zaaktype1", url_field="extern_zaaktype1")
```

### Comparing `django_loose_fk-1.1.0/testapp/settings.py` & `django_loose_fk-1.1.1/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_api.py` & `django_loose_fk-1.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_api_docs.py` & `django_loose_fk-1.1.1/tests/test_api_docs.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_chain_loose_fk.py` & `django_loose_fk-1.1.1/tests/test_chain_loose_fk.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_compare.py` & `django_loose_fk-1.1.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_integrity.py` & `django_loose_fk-1.1.1/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_is_local.py` & `django_loose_fk-1.1.1/tests/test_is_local.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_loaders.py` & `django_loose_fk-1.1.1/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_model_field_interface.py` & `django_loose_fk-1.1.1/tests/test_model_field_interface.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_querying.py` & `django_loose_fk-1.1.1/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_querylist.py` & `django_loose_fk-1.1.1/tests/test_querylist.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_serializer_field.py` & `django_loose_fk-1.1.1/tests/test_serializer_field.py`

 * *Files identical despite different names*

### Comparing `django_loose_fk-1.1.0/tests/test_system_checks.py` & `django_loose_fk-1.1.1/tests/test_system_checks.py`

 * *Files identical despite different names*

