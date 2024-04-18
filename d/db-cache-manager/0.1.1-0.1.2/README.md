# Comparing `tmp/db_cache_manager-0.1.1.tar.gz` & `tmp/db_cache_manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_cache_manager-0.1.1.tar", last modified: Mon Apr 15 08:45:13 2024, max compression
+gzip compressed data, was "db_cache_manager-0.1.2.tar", last modified: Thu Apr 18 10:42:15 2024, max compression
```

## Comparing `db_cache_manager-0.1.1.tar` & `db_cache_manager-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.926033 db_cache_manager-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.926033 db_cache_manager-0.1.1/src/db_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/src/db_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/src/db_cache_manager/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 08:45:13.000000 db_cache_manager-0.1.1/src/db_cache_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:13.930033 db_cache_manager-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-15 08:45:09.000000 db_cache_manager-0.1.1/tests/test_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.176619 db_cache_manager-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/src/db_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/src/db_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32586 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/src/db_cache_manager/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/tests/test_cache_manager.py
```

### Comparing `db_cache_manager-0.1.1/LICENSE` & `db_cache_manager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.1/PKG-INFO` & `db_cache_manager-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.1/README.md` & `db_cache_manager-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.1/pyproject.toml` & `db_cache_manager-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "db_cache_manager"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" },
   { name="Aitor Pérez", email="aitor.perez@epfl.ch" }
 ]
 description = "Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `db_cache_manager-0.1.1/src/db_cache_manager/db.py` & `db_cache_manager-0.1.2/src/db_cache_manager/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,27 +276,29 @@
     """
     return " AND ".join([col + " IS NOT NULL" for col in cols])
 
 
 class DBCachingManagerBase(abc.ABC):
     def __init__(self, db_config, cache_table, most_similar_table, schema='cache_graphai',
                  cache_date_added_col='date_added',
-                 cache_date_modified_col='date_added'):
+                 cache_date_modified_col='date_added',
+                 initialize_database=False):
         # Only three values are hardcoded into this class and need to be respected by its child classes:
         # 1. The name of the id column for both the main and the most-similar tables is 'id_token'
         # 2. The cache tables must have a "date_added" column of the data type DATETIME,
         #    which has the following format: YYYY-MM-DD hh:mm:ss
         # 3. The name of the second column in the most-similar table is 'most_similar_token'
         self.schema = schema
         self.cache_table = cache_table
         self.most_similar_table = most_similar_table
         self.cache_date_added_col = cache_date_added_col
         self.cache_date_modified_col = cache_date_modified_col
         self.db = DB(db_config)
-        self.init_db()
+        if initialize_database:
+            self.init_db()
 
     @abc.abstractmethod
     def init_db(self):
         pass
 
     def _resolve_most_similar_chain(self, token):
         """
```

### Comparing `db_cache_manager-0.1.1/src/db_cache_manager.egg-info/PKG-INFO` & `db_cache_manager-0.1.2/src/db_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.1/tests/test_cache_manager.py` & `db_cache_manager-0.1.2/tests/test_cache_manager.py`

 * *Files identical despite different names*

