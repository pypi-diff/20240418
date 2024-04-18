# Comparing `tmp/apollo_orm-2.1.9.tar.gz` & `tmp/apollo_orm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo_orm-2.1.9.tar", last modified: Fri Apr 12 16:49:13 2024, max compression
+gzip compressed data, was "apollo_orm-2.2.0.tar", last modified: Thu Apr 18 14:13:16 2024, max compression
```

## Comparing `apollo_orm-2.1.9.tar` & `apollo_orm-2.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.638353 apollo_orm-2.1.9/
--rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo_orm-2.1.9/LICENSE
--rw-rw-rw-   0        0        0     3273 2024-04-12 16:49:13.637355 apollo_orm-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo_orm-2.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.542818 apollo_orm-2.1.9/apollo_orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo_orm-2.1.9/apollo_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.584836 apollo_orm-2.1.9/apollo_orm/domains/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo_orm-2.1.9/apollo_orm/domains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.586836 apollo_orm-2.1.9/apollo_orm/domains/models/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo_orm-2.1.9/apollo_orm/domains/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.588832 apollo_orm-2.1.9/apollo_orm/domains/models/entities/
--rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.593359 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/__init__.py
--rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/column/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.595357 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/
--rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.597355 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
--rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.602358 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
--rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.605353 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/
--rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
--rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.611356 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/__init__.py
--rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.613355 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/__init__.py
--rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.615356 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/
--rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/__init__.py
--rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo_orm-2.1.9/apollo_orm/domains/models/entities/table_config/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.617357 apollo_orm-2.1.9/apollo_orm/orm/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo_orm-2.1.9/apollo_orm/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.621358 apollo_orm-2.1.9/apollo_orm/orm/abstracts/
--rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/icredential.py
--rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo_orm-2.1.9/apollo_orm/orm/abstracts/idatabase.py
--rw-rw-rw-   0        0        0    22995 2024-04-12 16:48:38.000000 apollo_orm-2.1.9/apollo_orm/orm/core.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.629357 apollo_orm-2.1.9/apollo_orm/orm/credentials/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/__init__.py
--rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/credential_service.py
--rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/json_credential_service.py
--rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo_orm-2.1.9/apollo_orm/orm/credentials/secrets_manager_credential_service.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.630357 apollo_orm-2.1.9/apollo_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo_orm-2.1.9/apollo_orm/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.633355 apollo_orm-2.1.9/apollo_orm/utils/exceptions/
--rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo_orm-2.1.9/apollo_orm/utils/exceptions/CommonBaseException.py
--rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo_orm-2.1.9/apollo_orm/utils/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.634355 apollo_orm-2.1.9/apollo_orm/utils/logger/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo_orm-2.1.9/apollo_orm/utils/logger/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo_orm-2.1.9/apollo_orm/utils/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.636355 apollo_orm-2.1.9/apollo_orm.egg-info/
--rw-rw-rw-   0        0        0     3273 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 16:49:13.000000 apollo_orm-2.1.9/apollo_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      731 2024-04-12 16:48:38.000000 apollo_orm-2.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 16:49:13.639353 apollo_orm-2.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 16:49:13.635355 apollo_orm-2.1.9/tests/
--rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo_orm-2.1.9/tests/test_full_process.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.360204 apollo_orm-2.2.0/
+-rw-rw-rw-   0        0        0     1092 2024-02-28 16:34:21.000000 apollo_orm-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3273 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-03-06 22:36:21.000000 apollo_orm-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.318948 apollo_orm-2.2.0/apollo_orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:26:45.000000 apollo_orm-2.2.0/apollo_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:30:22.000000 apollo_orm-2.2.0/apollo_orm/domains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:26:38.000000 apollo_orm-2.2.0/apollo_orm/domains/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-02-26 14:35:42.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/column/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:06:33.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/column/__init__.py
+-rw-rw-rw-   0        0        0      390 2024-02-26 18:50:38.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/column/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/
+-rw-rw-rw-   0        0        0        0 2024-03-22 22:10:36.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:19:02.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/__init__.py
+-rw-rw-rw-   0        0        0      566 2024-03-24 02:46:24.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_list/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:18:47.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_list/__init__.py
+-rw-rw-rw-   0        0        0      300 2024-03-24 02:54:01.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_list/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_process/
+-rw-rw-rw-   0        0        0        0 2024-03-24 02:27:03.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_process/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-03-24 03:37:47.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/result_process/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/connection_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:14.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/connection_config/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-20 15:01:55.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/connection_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:23.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/credentials/__init__.py
+-rw-rw-rw-   0        0        0      688 2024-03-20 15:01:55.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/credentials/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/domains/models/entities/table_config/
+-rw-rw-rw-   0        0        0        0 2024-02-26 18:07:52.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/table_config/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-02-28 18:35:47.000000 apollo_orm-2.2.0/apollo_orm/domains/models/entities/table_config/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/orm/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:28:09.000000 apollo_orm-2.2.0/apollo_orm/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.334572 apollo_orm-2.2.0/apollo_orm/orm/abstracts/
+-rw-rw-rw-   0        0        0        0 2024-02-27 18:29:25.000000 apollo_orm-2.2.0/apollo_orm/orm/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-28 18:35:47.000000 apollo_orm-2.2.0/apollo_orm/orm/abstracts/icredential.py
+-rw-rw-rw-   0        0        0     2372 2024-03-02 19:23:03.000000 apollo_orm-2.2.0/apollo_orm/orm/abstracts/idatabase.py
+-rw-rw-rw-   0        0        0    23186 2024-04-18 14:13:03.000000 apollo_orm-2.2.0/apollo_orm/orm/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/apollo_orm/orm/credentials/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:44:41.000000 apollo_orm-2.2.0/apollo_orm/orm/credentials/__init__.py
+-rw-rw-rw-   0        0        0      822 2024-03-04 13:10:50.000000 apollo_orm-2.2.0/apollo_orm/orm/credentials/credential_service.py
+-rw-rw-rw-   0        0        0      629 2024-02-28 18:38:15.000000 apollo_orm-2.2.0/apollo_orm/orm/credentials/json_credential_service.py
+-rw-rw-rw-   0        0        0      994 2024-02-28 20:04:09.000000 apollo_orm-2.2.0/apollo_orm/orm/credentials/secrets_manager_credential_service.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/apollo_orm/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:29.000000 apollo_orm-2.2.0/apollo_orm/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/apollo_orm/utils/exceptions/
+-rw-rw-rw-   0        0        0     1028 2024-02-28 18:38:15.000000 apollo_orm-2.2.0/apollo_orm/utils/exceptions/CommonBaseException.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:01:47.000000 apollo_orm-2.2.0/apollo_orm/utils/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/apollo_orm/utils/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-23 16:02:34.000000 apollo_orm-2.2.0/apollo_orm/utils/logger/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-07 13:30:15.000000 apollo_orm-2.2.0/apollo_orm/utils/logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/apollo_orm.egg-info/
+-rw-rw-rw-   0        0        0     3273 2024-04-18 14:13:16.000000 apollo_orm-2.2.0/apollo_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2024-04-18 14:13:16.000000 apollo_orm-2.2.0/apollo_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:13:16.000000 apollo_orm-2.2.0/apollo_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 14:13:16.000000 apollo_orm-2.2.0/apollo_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      731 2024-04-18 14:12:29.000000 apollo_orm-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:13:16.360204 apollo_orm-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 14:13:16.350196 apollo_orm-2.2.0/tests/
+-rw-rw-rw-   0        0        0    13794 2024-04-03 21:42:11.000000 apollo_orm-2.2.0/tests/test_full_process.py
```

### Comparing `apollo_orm-2.1.9/LICENSE` & `apollo_orm-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/PKG-INFO` & `apollo_orm-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.9
+Version: 2.2.0
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo_orm-2.1.9/README.md` & `apollo_orm-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py` & `apollo_orm-2.2.0/apollo_orm/domains/models/entities/concurrent/pre_processed_insert/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/domains/models/entities/connection_config/entity.py` & `apollo_orm-2.2.0/apollo_orm/domains/models/entities/connection_config/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/domains/models/entities/credentials/entity.py` & `apollo_orm-2.2.0/apollo_orm/domains/models/entities/credentials/entity.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/orm/abstracts/idatabase.py` & `apollo_orm-2.2.0/apollo_orm/orm/abstracts/idatabase.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/orm/core.py` & `apollo_orm-2.2.0/apollo_orm/orm/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import uuid
 from datetime import datetime, date
 
 from typing import Dict, Optional, List, Any
 
 from cassandra import ConsistencyLevel
 from cassandra.auth import PlainTextAuthProvider
-from cassandra.cluster import Cluster, Session, NoHostAvailable, ExecutionProfile, ResultSet, ResponseFuture, \
+from cassandra.cluster import Cluster, Session, ExecutionProfile, ResultSet, ResponseFuture, \
     EXEC_PROFILE_DEFAULT
 from cassandra.concurrent import execute_concurrent_with_args
-from cassandra.connection import ConnectionException
 from cassandra.policies import RoundRobinPolicy, DCAwareRoundRobinPolicy, TokenAwarePolicy, RetryPolicy, \
-    ExponentialReconnectionPolicy, ConstantSpeculativeExecutionPolicy
+    ExponentialReconnectionPolicy
 from cassandra.query import PreparedStatement
 from apollo_orm.domains.models.entities.column.entity import Column
 from apollo_orm.domains.models.entities.concurrent.pre_processed_insert.entity import PreProcessedInsertData
 from apollo_orm.domains.models.entities.concurrent.result_list.entity import ResultList
 from apollo_orm.domains.models.entities.concurrent.result_process.entity import ResultProcess
 from apollo_orm.domains.models.entities.connection_config.entity import ConnectionConfig
 from apollo_orm.domains.models.entities.table_config.entity import TableConfig
@@ -120,22 +119,18 @@
         if retry_num < self.MAX_RETRY_ATTEMPTS and (
                 (write_type == "BATCH_LOG" and received_responses >= required_responses) or (
                 write_type != "BATCH_LOG" and received_responses > 0)):
             return self.RETRY, consistency
         return self.RETHROW, None
 
     def on_unavailable(self, query, consistency, required_replicas, alive_replicas, retry_num):
-        if retry_num < self.MAX_RETRY_ATTEMPTS and alive_replicas < required_replicas:
-            return self.RETRY, consistency
-        return self.RETHROW, None
+        return (self.RETRY_NEXT_HOST, None) if retry_num == 0 else (self.RETHROW, None)
 
     def on_request_error(self, query, consistency, error, retry_num):
-        if retry_num < self.MAX_RETRY_ATTEMPTS:
-            return self.RETRY, consistency
-        return self.RETHROW, None
+        return self.RETRY_NEXT_HOST, None
 
 
 def get_consistency_level(consistency: str) -> int:
     ConsistencyLevel.name_to_value = {
         'ANY': ConsistencyLevel.ANY,
         'ONE': ConsistencyLevel.ONE,
         'TWO': ConsistencyLevel.TWO,
@@ -154,62 +149,61 @@
 class ORMInstance(IDatabaseService):
     log = Logger("ORMInstance")
 
     def __init__(self,
                  connection_config: ConnectionConfig,
                  attempts: int = 5,
                  consistency_level: str = "LOCAL_ONE",
-                 client_timeout: int = 20.0
+                 client_timeout: int = 20,
+                 idle_heartbeat_interval: int = 30
                  ):
         self._attempts = attempts
-        self._speculative_execution_policy = ConstantSpeculativeExecutionPolicy(
-            delay=0.1, max_attempts=attempts)
+        self._connect_timeout = client_timeout
+        self._idle_heartbeat_interval = idle_heartbeat_interval
         self._policy = DCAwareRoundRobinPolicy(
             connection_config.credential.datacenter) if connection_config.credential.datacenter else RoundRobinPolicy()
         self._load_balancing_policy = TokenAwarePolicy(self._policy)
         self._execution_profile = ExecutionProfile(load_balancing_policy=self._load_balancing_policy,
                                                    request_timeout=client_timeout,
                                                    consistency_level=get_consistency_level(consistency_level),
-                                                   retry_policy=ORMRetryPolicy(attempts),
-                                                   speculative_execution_policy=self._speculative_execution_policy
+                                                   retry_policy=RetryPolicy()
                                                    )
         self._connection_config = connection_config
         self._table_config: Optional[List[TableConfig]] = None
         self._prepared_statements: Dict[str, PreparedStatement] = {}
         self.cluster: Optional[Cluster] = None
         self.session: Optional[Session] = None
         self.connect()
 
     def connect(self,
                 protocol_version: int = 4) -> None:
         if self._connection_config is None:
             raise ApolloORMException("Connection config is not set")
-        error_message = ""
-        for _ in range(self._attempts):
-            try:
-                auth_provider = PlainTextAuthProvider(
-                    username=self._connection_config.credential.user,
-                    password=self._connection_config.credential.password
-                )
-                self.cluster = Cluster(
-                    contact_points=self._connection_config.credential.hosts,
-                    port=self._connection_config.credential.port,
-                    auth_provider=auth_provider,
-                    protocol_version=protocol_version,
-                    execution_profiles={EXEC_PROFILE_DEFAULT: self._execution_profile},
-                    reconnection_policy=ExponentialReconnectionPolicy(base_delay=1.0, max_delay=60.0,
-                                                                      max_attempts=self._attempts)
-                )
-                self.session = self.cluster.connect()
-                self._scan_tables()
-                self.log.info(f"Connected to {self._connection_config.credential.hosts}")
-                return
-            except ConnectionException as e:
-                error_message = str(e) if str(e) else "Unknown error"
-        raise ApolloORMException(f"Failed to connect after {self._attempts} attempts - {error_message}")
+        try:
+            auth_provider = PlainTextAuthProvider(
+                username=self._connection_config.credential.user,
+                password=self._connection_config.credential.password
+            )
+            self.cluster = Cluster(
+                contact_points=self._connection_config.credential.hosts,
+                port=self._connection_config.credential.port,
+                connect_timeout=self._connect_timeout,
+                auth_provider=auth_provider,
+                protocol_version=protocol_version,
+                idle_heartbeat_interval=self._idle_heartbeat_interval,
+                execution_profiles={EXEC_PROFILE_DEFAULT: self._execution_profile},
+                reconnection_policy=ExponentialReconnectionPolicy(base_delay=1.0, max_delay=10.0, max_attempts=None)
+            )
+            self.session = self.cluster.connect(self._connection_config.credential.keyspace_name)
+            self._scan_tables()
+            self.log.info(f"Connected to {self._connection_config.credential.hosts}")
+            return
+        except Exception as e:
+            error_message = str(e) if str(e) else "Unknown error"
+            raise ApolloORMException(f"Failed to connect after {self._attempts} attempts - {error_message}")
 
     def close(self):
         if self.session is not None:
             self.session.shutdown()
         if self.cluster is not None:
             self.cluster.shutdown()
 
@@ -261,64 +255,64 @@
         non_regular_columns = self._table_config[self._connection_config.tables.index(table_name)].columns
         filtered = _filter_kind(non_regular_columns, "partition_key")
         pendent_columns = [column.__str__() for column in filtered if
                            column.hash_id not in columns and column.kind == "partition_key"]
         if pendent_columns:
             raise ApolloORMException(
                 f"""Column {pendent_columns} is not in the filtered columns.
-                All partition keys columns must be passed as parameter""".rstrip())
+                    All partition keys columns must be passed as parameter""".rstrip())
 
     def _check_clustering_columns(self, columns: Dict[str, Column], table_name: str) -> None:
         non_regular_columns = self._table_config[self._connection_config.tables.index(table_name)].columns
         filtered = _filter_kind(non_regular_columns, "clustering")
         pendent_columns = [column.__str__() for column in filtered if
                            column.hash_id not in columns and column.kind == "clustering"]
         if pendent_columns:
             raise ApolloORMException(
                 f"""Column {pendent_columns} is not in the filtered columns.
-                All clustering columns must be passed as parameter""".rstrip())
+                    All clustering columns must be passed as parameter""".rstrip())
 
     def select_from_json(self, json_input: str, table_name: str) -> ResultSet:
         return self.select(json.loads(json_input), table_name)
 
     def select(self, dictionary_input: Dict[str, Any], table_name: str) -> ResultSet:
         try:
             filtered_columns = self._filter_columns(dictionary_input, table_name, "select")
             partition_and_clustering = [column for column in sorted(filtered_columns.values(), key=lambda x: x.name) if
                                         column.kind == "partition_key" or column.kind == "clustering"]
             prepared_statement = self._prepare_dynamic_statement(filtered_columns, table_name, "select")
             values = [dictionary_input[column.name] for column in partition_and_clustering]
             return self._execute_query(prepared_statement, values)
         except Exception as e:
             self.log.error(f"Failed to select data: {e}, in table {table_name}")
-            raise ApolloORMException(e)
+            raise ApolloORMException(f"Failed to select data: {dictionary_input} in table {table_name} - {e}")
 
     def insert(self, dictionary_input: Dict[str, Any], table_name: str, exec_async: bool = False) \
             -> Optional[ResponseFuture]:
         try:
             filtered_columns = self._filter_columns(dictionary_input, table_name, "insert")
             prepared_statement = self._prepare_dynamic_statement(filtered_columns, table_name, "insert")
             if exec_async:
                 return self._bind_delete_or_insert(filtered_columns, prepared_statement, exec_async)
             self._bind_delete_or_insert(filtered_columns, prepared_statement)
         except Exception as e:
             self.log.error(f"Failed to insert data: {dictionary_input}, in table {table_name}")
-            raise e
+            raise ApolloORMException(f"Failed to insert data: {dictionary_input} in table {table_name} - {e}")
 
     def delete(self, dictionary_input: Dict[str, Any], table_name: str, exec_async: bool = False) \
             -> Optional[ResponseFuture]:
         try:
             filtered_columns = self._filter_columns(dictionary_input, table_name, "delete")
             prepared_statement = self._prepare_dynamic_statement(filtered_columns, table_name, "delete")
             if exec_async:
                 return self._bind_delete_or_insert(filtered_columns, prepared_statement, exec_async)
             self._bind_delete_or_insert(filtered_columns, prepared_statement)
         except Exception as e:
             self.log.error(f"Failed to delete data: {e}, in table {table_name}")
-            raise e
+            raise ApolloORMException(f"Failed to delete data: {dictionary_input} in table {table_name} - {e}")
 
     def pre_process_insert(self, list_of_dict: List[Dict[str, Any]], table_name: str) -> PreProcessedInsertData:
         statements_and_params = {}
         errors: Optional[List[ResultProcess]] = []
         for dictionary_input in list_of_dict:
             try:
                 filtered_columns = self._filter_columns(dictionary_input, table_name, "insert")
@@ -329,36 +323,32 @@
                           sorted(filtered_columns.values(), key=lambda x: x.name)]
                 statements_and_params[prepared_statement].append(tuple(values))
             except Exception as e:
                 errors.append(ResultProcess(str(e), None, dictionary_input))
                 self.log.error(f"Failed to pre process data: {e}, in table {table_name}")
         return PreProcessedInsertData(statements_and_params, errors)
 
-    def insert_concurrent(self, pre_processed_insert: PreProcessedInsertData, workers: int = 10,
-                          retry: int = 3) -> ResultList:
+    def insert_concurrent(self, pre_processed_insert: PreProcessedInsertData, workers: int = 10) -> ResultList:
         errors: List[ResultProcess] = []
         successful: List[ResultProcess] = []
         if pre_processed_insert.errors:
             errors.extend(pre_processed_insert.errors)
         for statement, values in pre_processed_insert.statements_and_params.items():
             try:
                 result = execute_concurrent_with_args(self.session, statement, values, concurrency=workers)
                 for success, failed in result:
                     if failed:
                         errors.append(ResultProcess(str(failed), statement.query_string, values))
                         self.log.error(f"Failed to insert concurrent data: {failed}")
                     else:
                         successful.append(
                             ResultProcess("Data inserted successfully", statement.query_string, values))
-            except (NoHostAvailable, ConnectionException) as e:
+            except Exception as e:
                 self.log.error("Connection error: {e}")
-                if retry == 0:
-                    raise ApolloORMException(f"Failed to insert data: {statement} - {values} - Error Message: {e}")
-                self.reconnect()
-                self.insert_concurrent(pre_processed_insert, workers, retry - 1)
+                raise ApolloORMException(f"Failed to insert data: {statement} - {values} - Error Message: {e}")
         return ResultList(successful, errors)
 
     def _bind_delete_or_insert(self, filtered_columns: Dict[str, Column],
                                prepared_statement: PreparedStatement, exec_async: bool = False) \
             -> Optional[ResponseFuture]:
         values = [filtered_columns[column.hash_id].value for column in
                   sorted(filtered_columns.values(), key=lambda x: x.name)]
@@ -366,66 +356,76 @@
             return self._execute_async_query(prepared_statement, values)
         self._execute_query(prepared_statement, values)
 
     def _execute_async_query(self, statement: PreparedStatement, values: List[Any]) -> ResponseFuture:
         statement.is_idempotent = True
         self.log.info(f"Executing query: {statement.query_string} with values: {values}")
         try:
-            return self.session.execute_async(statement, values)
-        except (NoHostAvailable, ConnectionException) as e:
-            self.log.error(f"Connection error: {e}. Reconnecting...")
-            self.reconnect()
-            return self.session.execute_async(statement, values)
+            return self.session.execute_async(statement, values, )
         except Exception as e:
             self.log.error(f"Failed to execute query: {statement.query_string, values}")
             raise ApolloORMException(f"Failed to execute query: {statement.query_string, values} - {e}")
 
     def _execute_query(self, statement: PreparedStatement, values: List[Any]) -> ResultSet:
         self.log.info(f"Executing query: {statement.query_string} with values: {values}")
         try:
             return self.session.execute(statement, values)
-        except (NoHostAvailable, ConnectionException) as e:
+        except Exception as e:
             self.log.error(f"Connection error: {e}")
-            self.reconnect()
-            return self.session.execute(statement, values)
+            raise ApolloORMException(f"Failed to execute query: {statement.query_string, values} - {e}")
 
     def _prepare_dynamic_statement(self, columns: Dict[str, Column], table_name: str,
                                    query_type: str) -> PreparedStatement:
         keyspace = self._connection_config.credential.keyspace_name
         ordered_columns = sorted(columns.values(), key=lambda x: x.name)
         hashed_name = _text_to_hash(f"{query_type}-{table_name}".join([column.name for column in ordered_columns]))
         if hashed_name not in self._prepared_statements:
             try:
                 if query_type == "select":
                     self._prepare_read(hashed_name, ordered_columns, keyspace, table_name)
                 elif query_type == "insert":
                     self._prepare_insert(hashed_name, ordered_columns, keyspace, table_name, columns)
                 elif query_type == "delete":
                     self._prepare_delete(hashed_name, ordered_columns, keyspace, table_name, columns)
-            except (NoHostAvailable, ConnectionException) as e:
-                self.log.error(f"Connection error: {e}")
-                self.reconnect()
-                self._prepare_dynamic_statement(columns, table_name, query_type)
+            except Exception as e:
+                self.log.error(f"Failed to prepare statement: {e}")
+                raise ApolloORMException(f"Failed to prepare statement: {columns} - {e}")
         return self._prepared_statements[hashed_name]
 
     def _prepare_read(self, hashed_name: str, columns: List[Column], keyspace: str, table_name: str) -> None:
-        values = _generate_pre_statement_labels(columns)
-        statement = f"select * from {keyspace}.{table_name} where {' and '.join(values.values())}"
-        self._prepared_statements[hashed_name] = self.session.prepare(statement)
+        try:
+            values = _generate_pre_statement_labels(columns)
+            statement = f"select * from {keyspace}.{table_name} where {' and '.join(values.values())}"
+            self._prepare_statement(hashed_name, statement)
+        except Exception as e:
+            self.log.error(f"Failed to prepare read statement: {e}")
+            raise ApolloORMException(f"Failed to prepare read statement: {columns} - {e}")
 
     def _prepare_insert(self, hashed_name: str, columns: List[Column], keyspace: str, table_name: str,
                         dict_columns: Optional[Dict[str, Column]] = None) -> None:
         hashed_statement = {}
-        keys = [column.name for column in columns]
-        for column in columns:
-            hashed_statement[column.hash_id] = "?"
-        statement = f"""insert into
-            {keyspace}.{table_name}
-            ({', '.join(keys)})
-            values ({', '.join(hashed_statement.values())})"""
-        self._prepared_statements[hashed_name] = self.session.prepare(statement)
+        try:
+            keys = [column.name for column in columns]
+            for column in columns:
+                hashed_statement[column.hash_id] = "?"
+            statement = f"""insert into
+                    {keyspace}.{table_name}
+                    ({', '.join(keys)})
+                    values ({', '.join(hashed_statement.values())})"""
+            self._prepare_statement(hashed_name, statement)
+        except Exception as e:
+            self.log.error(f"Failed to prepare insert statement: {e}")
+            raise ApolloORMException(f"Failed to prepare insert statement: {columns} - {e}")
 
     def _prepare_delete(self, hashed_name: str, columns: List[Column], keyspace: str, table_name: str,
                         dict_columns: Optional[Dict[str, Column]] = None) -> None:
-        values = _generate_pre_statement_labels(columns)
-        statement = f"delete from {keyspace}.{table_name} where {' and '.join(values.values())}"
+        try:
+            values = _generate_pre_statement_labels(columns)
+            statement = f"delete from {keyspace}.{table_name} where {' and '.join(values.values())}"
+            self._prepare_statement(hashed_name, statement)
+        except Exception as e:
+            self.log.error(f"Failed to prepare delete statement: {e}")
+            raise ApolloORMException(f"Failed to prepare delete statement: {columns} - {e}")
+
+    def _prepare_statement(self, hashed_name: str, statement: str) -> None:
         self._prepared_statements[hashed_name] = self.session.prepare(statement)
+        self._prepared_statements[hashed_name].is_idempotent = True
```

### Comparing `apollo_orm-2.1.9/apollo_orm/orm/credentials/credential_service.py` & `apollo_orm-2.2.0/apollo_orm/orm/credentials/credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/orm/credentials/json_credential_service.py` & `apollo_orm-2.2.0/apollo_orm/orm/credentials/json_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/orm/credentials/secrets_manager_credential_service.py` & `apollo_orm-2.2.0/apollo_orm/orm/credentials/secrets_manager_credential_service.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/utils/exceptions/CommonBaseException.py` & `apollo_orm-2.2.0/apollo_orm/utils/exceptions/CommonBaseException.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm/utils/logger/logger.py` & `apollo_orm-2.2.0/apollo_orm/utils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/apollo_orm.egg-info/PKG-INFO` & `apollo_orm-2.2.0/apollo_orm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-orm
-Version: 2.1.9
+Version: 2.2.0
 Summary: ORM Cassandra/Scylla Stable Version (2.x.x)
 Author-email: Danilo Rodrigues <daniloarodrigues@outlook.com>
 Project-URL: Homepage, https://github.com/daniloarodrigues/apollo-orm
 Project-URL: Issues, https://github.com/daniloarodrigues/apollo-orm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo_orm-2.1.9/apollo_orm.egg-info/SOURCES.txt` & `apollo_orm-2.2.0/apollo_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo_orm-2.1.9/pyproject.toml` & `apollo_orm-2.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apollo-orm"
-version = "2.1.9"
+version = "2.2.0"
 authors = [
     { name="Danilo Rodrigues", email="daniloarodrigues@outlook.com" },
 ]
 description = "ORM Cassandra/Scylla Stable Version (2.x.x)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `apollo_orm-2.1.9/tests/test_full_process.py` & `apollo_orm-2.2.0/tests/test_full_process.py`

 * *Files identical despite different names*

