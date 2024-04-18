# Comparing `tmp/fandango_aria_plugin-1.0.0.tar.gz` & `tmp/fandango_aria_plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fandango_aria_plugin-1.0.0.tar", last modified: Thu Apr 18 15:06:44 2024, max compression
+gzip compressed data, was "fandango_aria_plugin-1.0.1.tar", last modified: Thu Apr 18 15:44:54 2024, max compression
```

## Comparing `fandango_aria_plugin-1.0.0.tar` & `fandango_aria_plugin-1.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:06:44.927023 fandango_aria_plugin-1.0.0/
--rw-r--r--   0 luiholliday   (501) staff       (20)     1070 2024-02-08 14:49:18.000000 fandango_aria_plugin-1.0.0/LICENSE.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)     1349 2024-04-18 15:06:44.926957 fandango_aria_plugin-1.0.0/PKG-INFO
--rw-r--r--   0 luiholliday   (501) staff       (20)      847 2024-04-18 14:00:37.000000 fandango_aria_plugin-1.0.0/README.md
-drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:06:44.923389 fandango_aria_plugin-1.0.0/fandango/
--rw-r--r--   0 luiholliday   (501) staff       (20)      202 2024-04-11 12:49:35.000000 fandango_aria_plugin-1.0.0/fandango/__init__.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      870 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/abstract_bucket.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1032 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/abstract_field.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      596 2024-03-24 21:32:26.000000 fandango_aria_plugin-1.0.0/fandango/abstract_record.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1486 2024-04-18 12:51:12.000000 fandango_aria_plugin-1.0.0/fandango/api_client.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1590 2024-04-10 13:40:01.000000 fandango_aria_plugin-1.0.0/fandango/aria_client.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     2748 2024-04-11 19:52:20.000000 fandango_aria_plugin-1.0.0/fandango/bucket.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     4543 2024-04-18 13:16:14.000000 fandango_aria_plugin-1.0.0/fandango/cli_data_manager.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     2889 2024-04-18 13:17:02.000000 fandango_aria_plugin-1.0.0/fandango/client_data_manager.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1683 2024-04-18 10:53:40.000000 fandango_aria_plugin-1.0.0/fandango/client_entity_manager.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      423 2024-04-11 19:52:20.000000 fandango_aria_plugin-1.0.0/fandango/client_oauth.py
-drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:06:44.925353 fandango_aria_plugin-1.0.0/fandango/commands/
--rw-r--r--   0 luiholliday   (501) staff       (20)        0 2024-04-11 20:04:01.000000 fandango_aria_plugin-1.0.0/fandango/commands/__init__.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1100 2024-03-21 20:46:26.000000 fandango_aria_plugin-1.0.0/fandango/commands/cli.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      357 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/create_bucket.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      367 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/create_field.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      408 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/create_record.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      283 2024-03-13 22:43:35.000000 fandango_aria_plugin-1.0.0/fandango/commands/get_visits.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      586 2024-03-08 13:31:49.000000 fandango_aria_plugin-1.0.0/fandango/commands/help.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      367 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/list_buckets.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      365 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/list_fields.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      377 2024-03-20 11:44:37.000000 fandango_aria_plugin-1.0.0/fandango/commands/list_records.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      913 2024-04-18 12:58:20.000000 fandango_aria_plugin-1.0.0/fandango/commands/login.py
-drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:06:44.925661 fandango_aria_plugin-1.0.0/fandango/config/
--rw-r--r--   0 luiholliday   (501) staff       (20)        0 2024-04-11 19:49:21.000000 fandango_aria_plugin-1.0.0/fandango/config/__init__.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      640 2024-04-18 13:07:58.000000 fandango_aria_plugin-1.0.0/fandango/config/config.yml
--rw-r--r--   0 luiholliday   (501) staff       (20)     3689 2024-04-12 10:11:22.000000 fandango_aria_plugin-1.0.0/fandango/data_manager.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      976 2024-04-18 10:53:05.000000 fandango_aria_plugin-1.0.0/fandango/entity_manager.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     2047 2024-04-11 20:05:20.000000 fandango_aria_plugin-1.0.0/fandango/field.py
--rw-r--r--   0 luiholliday   (501) staff       (20)      211 2024-04-12 10:42:24.000000 fandango_aria_plugin-1.0.0/fandango/imports_config.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     4506 2024-04-18 09:55:58.000000 fandango_aria_plugin-1.0.0/fandango/oauth.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     2042 2024-04-11 19:57:15.000000 fandango_aria_plugin-1.0.0/fandango/record.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     2470 2024-04-12 12:16:14.000000 fandango_aria_plugin-1.0.0/fandango/token.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     4023 2024-04-12 10:20:02.000000 fandango_aria_plugin-1.0.0/fandango/utils.py
--rw-r--r--   0 luiholliday   (501) staff       (20)     1094 2024-04-11 19:52:20.000000 fandango_aria_plugin-1.0.0/fandango/visit.py
-drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:06:44.926730 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/
--rw-r--r--   0 luiholliday   (501) staff       (20)     1349 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/PKG-INFO
--rw-r--r--   0 luiholliday   (501) staff       (20)     1199 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)        1 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)       55 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/entry_points.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)       42 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/requires.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)        9 2024-04-18 15:06:44.000000 fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/top_level.txt
--rw-r--r--   0 luiholliday   (501) staff       (20)       97 2024-04-16 10:31:33.000000 fandango_aria_plugin-1.0.0/pyproject.toml
--rw-r--r--   0 luiholliday   (501) staff       (20)       78 2024-04-18 15:06:44.927286 fandango_aria_plugin-1.0.0/setup.cfg
--rw-r--r--   0 luiholliday   (501) staff       (20)     1021 2024-04-18 15:02:55.000000 fandango_aria_plugin-1.0.0/setup.py
+drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:44:54.241734 fandango_aria_plugin-1.0.1/
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1070 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/LICENSE.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1349 2024-04-18 15:44:54.241658 fandango_aria_plugin-1.0.1/PKG-INFO
+-rw-r--r--   0 luiholliday   (501) staff       (20)      847 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/README.md
+drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:44:54.238453 fandango_aria_plugin-1.0.1/fandango/
+-rw-r--r--   0 luiholliday   (501) staff       (20)      202 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/__init__.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      870 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/abstract_bucket.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1032 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/abstract_field.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      596 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/abstract_record.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1486 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/api_client.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1644 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/aria_client.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     2748 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/bucket.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     4543 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/cli_data_manager.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     2889 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/client_data_manager.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1684 2024-04-18 15:42:05.000000 fandango_aria_plugin-1.0.1/fandango/client_entity_manager.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      423 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/client_oauth.py
+drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:44:54.239895 fandango_aria_plugin-1.0.1/fandango/commands/
+-rw-r--r--   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/__init__.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1100 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/cli.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      357 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/create_bucket.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      367 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/create_field.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      408 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/create_record.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      283 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/get_visits.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      586 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/help.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      367 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/list_buckets.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      365 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/list_fields.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      377 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/list_records.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      913 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/commands/login.py
+drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:44:54.240154 fandango_aria_plugin-1.0.1/fandango/config/
+-rw-r--r--   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/config/__init__.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      640 2024-04-18 15:44:19.000000 fandango_aria_plugin-1.0.1/fandango/config/config.yml
+-rw-r--r--   0 luiholliday   (501) staff       (20)     3689 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/data_manager.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      976 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/entity_manager.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     2047 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/field.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)      211 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/imports_config.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     4506 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/oauth.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     2042 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/record.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     2470 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/token.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     4023 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/utils.py
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1094 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/fandango/visit.py
+drwxr-xr-x   0 luiholliday   (501) staff       (20)        0 2024-04-18 15:44:54.241227 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1349 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1199 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)        1 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)       55 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)       42 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/requires.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)        9 2024-04-18 15:44:54.000000 fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/top_level.txt
+-rw-r--r--   0 luiholliday   (501) staff       (20)       97 2024-04-18 15:35:39.000000 fandango_aria_plugin-1.0.1/pyproject.toml
+-rw-r--r--   0 luiholliday   (501) staff       (20)       78 2024-04-18 15:44:54.241976 fandango_aria_plugin-1.0.1/setup.cfg
+-rw-r--r--   0 luiholliday   (501) staff       (20)     1021 2024-04-18 15:44:06.000000 fandango_aria_plugin-1.0.1/setup.py
```

### Comparing `fandango_aria_plugin-1.0.0/LICENSE.txt` & `fandango_aria_plugin-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/PKG-INFO` & `fandango_aria_plugin-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango-aria-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Public Client library and CLI for interacting with ARIA's Data Deposition Service.
 Home-page: https://github.com/FragmentScreen/fandango-aria-plugin
 Author: Lui Holliday, Instruct-ERIC
 Author-email: lui.holliday@instruct-eric.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `fandango_aria_plugin-1.0.0/README.md` & `fandango_aria_plugin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/abstract_bucket.py` & `fandango_aria_plugin-1.0.1/fandango/abstract_bucket.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/abstract_field.py` & `fandango_aria_plugin-1.0.1/fandango/abstract_field.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/abstract_record.py` & `fandango_aria_plugin-1.0.1/fandango/abstract_record.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/api_client.py` & `fandango_aria_plugin-1.0.1/fandango/api_client.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/aria_client.py` & `fandango_aria_plugin-1.0.1/fandango/aria_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .oauth import OAuth
 from .data_manager import DataManager
 from .bucket import Bucket
 from .visit import Visit
 from .data_manager import DataManager
 from .cli_data_manager import DataManagerCLI
+<<<<<<< HEAD
 from .token import Token
+=======
 from .entity_manager import EntityManager
-
+>>>>>>> b548e25 (entity fetching)
 class AriaClient :
     '''
     Super class. New instances initiated in the `commands`. All functionality will start with one of these methods.
     '''
     def __init__(self, login=False):
         self.oauth = OAuth()
         if not login:
```

### Comparing `fandango_aria_plugin-1.0.0/fandango/bucket.py` & `fandango_aria_plugin-1.0.1/fandango/bucket.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/cli_data_manager.py` & `fandango_aria_plugin-1.0.1/fandango/cli_data_manager.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/client_data_manager.py` & `fandango_aria_plugin-1.0.1/fandango/client_data_manager.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/client_entity_manager.py` & `fandango_aria_plugin-1.0.1/fandango/client_entity_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class EntityManagerClient(APIClient):
     def __init__(self, token):
         super().__init__(token)
         self.token = token
         self.facility = config['FACILITY']['ID']
         self.visits_url = config["ENDPOINTS"]['GET']["VISITS"]
         self.proposal_data_url = config['ENDPOINTS']['GET']['PROPOSAL_DATA']
-        self.proposal_url = config['ENDPOINT']['GET']['PROPOSAL']
+        self.proposal_url = config['ENDPOINTS']['GET']['PROPOSAL']
 
         self.load_url()
 
     def load_url(self) :
         dev = config.get('DEV', 'LOCAL')
         self.base_url = config['API'][dev]['ENTITY_BASE']
```

### Comparing `fandango_aria_plugin-1.0.0/fandango/commands/cli.py` & `fandango_aria_plugin-1.0.1/fandango/commands/cli.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/commands/help.py` & `fandango_aria_plugin-1.0.1/fandango/commands/help.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/commands/login.py` & `fandango_aria_plugin-1.0.1/fandango/commands/login.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/config/config.yml` & `fandango_aria_plugin-1.0.1/fandango/config/config.yml`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/data_manager.py` & `fandango_aria_plugin-1.0.1/fandango/data_manager.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/entity_manager.py` & `fandango_aria_plugin-1.0.1/fandango/entity_manager.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/field.py` & `fandango_aria_plugin-1.0.1/fandango/field.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/oauth.py` & `fandango_aria_plugin-1.0.1/fandango/oauth.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/record.py` & `fandango_aria_plugin-1.0.1/fandango/record.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/token.py` & `fandango_aria_plugin-1.0.1/fandango/token.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/utils.py` & `fandango_aria_plugin-1.0.1/fandango/utils.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango/visit.py` & `fandango_aria_plugin-1.0.1/fandango/visit.py`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/PKG-INFO` & `fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fandango-aria-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Public Client library and CLI for interacting with ARIA's Data Deposition Service.
 Home-page: https://github.com/FragmentScreen/fandango-aria-plugin
 Author: Lui Holliday, Instruct-ERIC
 Author-email: lui.holliday@instruct-eric.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `fandango_aria_plugin-1.0.0/fandango_aria_plugin.egg-info/SOURCES.txt` & `fandango_aria_plugin-1.0.1/fandango_aria_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fandango_aria_plugin-1.0.0/setup.py` & `fandango_aria_plugin-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='fandango-aria-plugin',
-    version='1.0.0',
+    version='1.0.1',
     description="A Public Client library and CLI for interacting with ARIA's Data Deposition Service.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Lui Holliday, Instruct-ERIC",
     author_email="lui.holliday@instruct-eric.org",
     license='MIT',
     package_data={'fandango': ['config/*.yml']},
```

