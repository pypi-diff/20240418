# Comparing `tmp/django_blocklist-2.3.1.tar.gz` & `tmp/django_blocklist-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_blocklist-2.3.1.tar", max compression
+gzip compressed data, was "django_blocklist-2.3.2.tar", max compression
```

## Comparing `django_blocklist-2.3.1.tar` & `django_blocklist-2.3.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1511 2022-07-11 13:00:57.903015 django_blocklist-2.3.1/LICENSE.md
--rw-r--r--   0        0        0     3178 2024-02-23 23:22:09.437458 django_blocklist-2.3.1/README.md
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.903572 django_blocklist-2.3.1/django_blocklist/__init__.py
--rw-r--r--   0        0        0     1284 2024-02-17 19:18:50.132949 django_blocklist-2.3.1/django_blocklist/admin.py
--rw-r--r--   0        0        0      378 2023-03-20 01:47:36.202242 django_blocklist-2.3.1/django_blocklist/apps.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904273 django_blocklist-2.3.1/django_blocklist/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904394 django_blocklist-2.3.1/django_blocklist/management/commands/__init__.py
--rw-r--r--   0        0        0     1797 2024-01-31 14:43:32.509451 django_blocklist-2.3.1/django_blocklist/management/commands/clean_blocklist.py
--rw-r--r--   0        0        0     1410 2024-02-23 23:31:48.998450 django_blocklist-2.3.1/django_blocklist/management/commands/fake_blocklist.py
--rw-r--r--   0        0        0     2877 2024-02-17 19:18:50.132981 django_blocklist-2.3.1/django_blocklist/management/commands/import_blocklist.py
--rw-r--r--   0        0        0      646 2022-07-11 13:00:57.905419 django_blocklist-2.3.1/django_blocklist/management/commands/remove_from_blocklist.py
--rw-r--r--   0        0        0     3766 2024-02-17 19:18:50.132870 django_blocklist-2.3.1/django_blocklist/management/commands/report_blocklist.py
--rw-r--r--   0        0        0      947 2023-08-05 01:19:26.095157 django_blocklist-2.3.1/django_blocklist/management/commands/search_blocklist.py
--rw-r--r--   0        0        0     1710 2023-03-18 02:28:13.931382 django_blocklist-2.3.1/django_blocklist/management/commands/update_blocklist.py
--rw-r--r--   0        0        0     1371 2024-03-02 13:48:11.476944 django_blocklist-2.3.1/django_blocklist/middleware.py
--rw-r--r--   0        0        0     1400 2023-12-09 02:29:53.908469 django_blocklist-2.3.1/django_blocklist/migrations/0001_initial.py
--rw-r--r--   0        0        0      486 2023-12-09 02:29:53.908703 django_blocklist-2.3.1/django_blocklist/migrations/0002_alter_blockedip_tally.py
--rw-r--r--   0        0        0      936 2024-02-17 19:13:49.352265 django_blocklist-2.3.1/django_blocklist/migrations/0003_rename_first_seen_to_datetime_added.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.907461 django_blocklist-2.3.1/django_blocklist/migrations/__init__.py
--rw-r--r--   0        0        0     1907 2024-02-17 19:13:19.239120 django_blocklist-2.3.1/django_blocklist/models.py
--rw-r--r--   0        0        0        0 2022-07-11 13:00:57.908111 django_blocklist-2.3.1/django_blocklist/tests/__init__.py
--rw-r--r--   0        0        0     4833 2024-02-17 19:18:50.143591 django_blocklist-2.3.1/django_blocklist/tests/test_management.py
--rw-r--r--   0        0        0     1646 2024-02-23 23:31:05.927821 django_blocklist-2.3.1/django_blocklist/tests/test_middleware.py
--rw-r--r--   0        0        0      646 2023-12-09 02:29:53.909768 django_blocklist-2.3.1/django_blocklist/tests/test_models.py
--rw-r--r--   0        0        0      942 2024-02-23 23:31:05.928839 django_blocklist-2.3.1/django_blocklist/tests/test_settings.py
--rw-r--r--   0        0        0     2417 2024-02-23 23:31:05.928713 django_blocklist-2.3.1/django_blocklist/tests/test_utils.py
--rw-r--r--   0        0        0     2730 2024-02-23 23:24:12.070851 django_blocklist-2.3.1/django_blocklist/utils.py
--rw-r--r--   0        0        0      641 2024-03-03 19:37:34.870322 django_blocklist-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 django_blocklist-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1511 2022-07-11 13:00:57.903015 django_blocklist-2.3.2/LICENSE.md
+-rw-r--r--   0        0        0     3178 2024-04-18 03:34:12.838634 django_blocklist-2.3.2/README.md
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.903572 django_blocklist-2.3.2/django_blocklist/__init__.py
+-rw-r--r--   0        0        0     1284 2024-02-21 00:54:41.212643 django_blocklist-2.3.2/django_blocklist/admin.py
+-rw-r--r--   0        0        0      378 2024-01-31 01:47:35.578149 django_blocklist-2.3.2/django_blocklist/apps.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904273 django_blocklist-2.3.2/django_blocklist/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.904394 django_blocklist-2.3.2/django_blocklist/management/commands/__init__.py
+-rw-r--r--   0        0        0     1797 2024-01-31 01:55:25.976965 django_blocklist-2.3.2/django_blocklist/management/commands/clean_blocklist.py
+-rw-r--r--   0        0        0     1410 2024-04-18 03:34:12.839146 django_blocklist-2.3.2/django_blocklist/management/commands/fake_blocklist.py
+-rw-r--r--   0        0        0     2877 2024-02-21 00:54:41.213790 django_blocklist-2.3.2/django_blocklist/management/commands/import_blocklist.py
+-rw-r--r--   0        0        0      646 2022-07-11 13:00:57.905419 django_blocklist-2.3.2/django_blocklist/management/commands/remove_from_blocklist.py
+-rw-r--r--   0        0        0     3766 2024-02-21 00:54:41.214382 django_blocklist-2.3.2/django_blocklist/management/commands/report_blocklist.py
+-rw-r--r--   0        0        0      947 2024-01-31 01:47:35.581230 django_blocklist-2.3.2/django_blocklist/management/commands/search_blocklist.py
+-rw-r--r--   0        0        0     1710 2023-03-18 19:53:23.007905 django_blocklist-2.3.2/django_blocklist/management/commands/update_blocklist.py
+-rw-r--r--   0        0        0     1371 2024-04-18 03:34:12.839764 django_blocklist-2.3.2/django_blocklist/middleware.py
+-rw-r--r--   0        0        0     1400 2024-01-31 01:47:35.582674 django_blocklist-2.3.2/django_blocklist/migrations/0001_initial.py
+-rw-r--r--   0        0        0      486 2024-01-31 01:47:35.583007 django_blocklist-2.3.2/django_blocklist/migrations/0002_alter_blockedip_tally.py
+-rw-r--r--   0        0        0      936 2024-02-21 00:54:41.214789 django_blocklist-2.3.2/django_blocklist/migrations/0003_rename_first_seen_to_datetime_added.py
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.907461 django_blocklist-2.3.2/django_blocklist/migrations/__init__.py
+-rw-r--r--   0        0        0     1907 2024-02-21 00:54:41.215527 django_blocklist-2.3.2/django_blocklist/models.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:57:11.148725 django_blocklist-2.3.2/django_blocklist/py.typed
+-rw-r--r--   0        0        0        0 2022-07-11 13:00:57.908111 django_blocklist-2.3.2/django_blocklist/tests/__init__.py
+-rw-r--r--   0        0        0     4833 2024-02-21 00:54:41.216548 django_blocklist-2.3.2/django_blocklist/tests/test_management.py
+-rw-r--r--   0        0        0     1646 2024-04-18 03:34:12.840324 django_blocklist-2.3.2/django_blocklist/tests/test_middleware.py
+-rw-r--r--   0        0        0      646 2024-01-31 01:47:35.585819 django_blocklist-2.3.2/django_blocklist/tests/test_models.py
+-rw-r--r--   0        0        0      942 2024-04-18 03:34:12.841398 django_blocklist-2.3.2/django_blocklist/tests/test_settings.py
+-rw-r--r--   0        0        0     2417 2024-04-18 03:34:12.841837 django_blocklist-2.3.2/django_blocklist/tests/test_utils.py
+-rw-r--r--   0        0        0     2730 2024-04-18 03:34:12.842391 django_blocklist-2.3.2/django_blocklist/utils.py
+-rw-r--r--   0        0        0      691 2024-04-18 04:07:08.807677 django_blocklist-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 django_blocklist-2.3.2/PKG-INFO
```

### Comparing `django_blocklist-2.3.1/LICENSE.md` & `django_blocklist-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/README.md` & `django_blocklist-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/admin.py` & `django_blocklist-2.3.2/django_blocklist/admin.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/clean_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/clean_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/fake_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/fake_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/import_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/import_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/remove_from_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/remove_from_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/report_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/report_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/search_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/search_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/management/commands/update_blocklist.py` & `django_blocklist-2.3.2/django_blocklist/management/commands/update_blocklist.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/middleware.py` & `django_blocklist-2.3.2/django_blocklist/middleware.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/migrations/0001_initial.py` & `django_blocklist-2.3.2/django_blocklist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/migrations/0003_rename_first_seen_to_datetime_added.py` & `django_blocklist-2.3.2/django_blocklist/migrations/0003_rename_first_seen_to_datetime_added.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/models.py` & `django_blocklist-2.3.2/django_blocklist/models.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/tests/test_management.py` & `django_blocklist-2.3.2/django_blocklist/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/tests/test_middleware.py` & `django_blocklist-2.3.2/django_blocklist/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/tests/test_models.py` & `django_blocklist-2.3.2/django_blocklist/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/tests/test_settings.py` & `django_blocklist-2.3.2/django_blocklist/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/tests/test_utils.py` & `django_blocklist-2.3.2/django_blocklist/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/django_blocklist/utils.py` & `django_blocklist-2.3.2/django_blocklist/utils.py`

 * *Files identical despite different names*

### Comparing `django_blocklist-2.3.1/PKG-INFO` & `django_blocklist-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-blocklist
-Version: 2.3.1
+Version: 2.3.2
 Summary: A Django app that implements IP-based blocklisting.
 Home-page: https://gitlab.com/paul_bissex/django-blocklist
 License: BSD-3-Clause
 Author: Paul Bissex
 Author-email: paul@bissex.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: BSD License
```

