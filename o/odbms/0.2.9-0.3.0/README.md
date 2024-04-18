# Comparing `tmp/odbms-0.2.9.tar.gz` & `tmp/odbms-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbms-0.2.9.tar", last modified: Thu Apr 11 19:08:32 2024, max compression
+gzip compressed data, was "odbms-0.3.0.tar", last modified: Thu Apr 18 18:06:09 2024, max compression
```

## Comparing `odbms-0.2.9.tar` & `odbms-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:08:32.253747 odbms-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-11 19:08:28.000000 odbms-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 19:08:28.000000 odbms-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-11 19:08:32.253747 odbms-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 19:08:28.000000 odbms-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:08:32.253747 odbms-0.2.9/odbms/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/dbms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/postgresqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-11 19:08:28.000000 odbms-0.2.9/odbms/sqlitedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:08:32.253747 odbms-0.2.9/odbms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-11 19:08:32.000000 odbms-0.2.9/odbms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 19:08:32.000000 odbms-0.2.9/odbms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:08:32.000000 odbms-0.2.9/odbms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 19:08:32.000000 odbms-0.2.9/odbms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 19:08:32.000000 odbms-0.2.9/odbms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:08:32.253747 odbms-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-11 19:08:28.000000 odbms-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:06:09.536106 odbms-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 18:05:58.000000 odbms-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 18:05:58.000000 odbms-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 18:06:09.536106 odbms-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-18 18:05:58.000000 odbms-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:06:09.536106 odbms-0.3.0/odbms/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/dbms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:06:09.536106 odbms-0.3.0/odbms/orms/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/postgresqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-18 18:05:58.000000 odbms-0.3.0/odbms/orms/sqlitedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:06:09.536106 odbms-0.3.0/odbms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-18 18:06:09.000000 odbms-0.3.0/odbms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 18:06:09.000000 odbms-0.3.0/odbms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:06:09.000000 odbms-0.3.0/odbms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 18:06:09.000000 odbms-0.3.0/odbms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 18:06:09.000000 odbms-0.3.0/odbms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:06:09.536106 odbms-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-18 18:05:58.000000 odbms-0.3.0/setup.py
```

### Comparing `odbms-0.2.9/LICENSE` & `odbms-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odbms-0.2.9/PKG-INFO` & `odbms-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.9
+Version: 0.3.0
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.2.9/odbms/app.py` & `odbms-0.3.0/odbms/app.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.9/odbms/database.py` & `odbms-0.3.0/odbms/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # -*- coding: utf-8 -*-
 # @Date    : 2022-08-06 17:37:00
 # @Author  : Amos Amissah (theonlyamos@gmail.com)
 # @Link    : link
 # @Version : 1.0.0
 
 from typing import Type, Literal, Optional
-from .mongodb import MongoDB
-from .mysqldb import MysqlDB
-from .sqlitedb import SqliteDB
-from .postgresqldb import PostgresqlDB
+from .orms.mongodb import MongoDB
+from .orms.mysqldb import MysqlDB
+from .orms.sqlitedb import SqliteDB
+from .orms.postgresqldb import PostgresqlDB
 # from .model import Model
 
 
 class Database():
     db: Type[MysqlDB]|Type[MongoDB]|Type[PostgresqlDB]|Type[SqliteDB]|None = None
     dbms: str|None = None
     # models: Type[Models] = Models()
```

### Comparing `odbms-0.2.9/odbms/dbms.py` & `odbms-0.3.0/odbms/dbms.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # -*- coding: utf-8 -*-
 # @Date    : 2022-08-06 17:37:00
 # @Author  : Amos Amissah (theonlyamos@gmail.com)
 # @Link    : link
 # @Version : 1.0.0
 
 from typing import Type, Literal, Union
-from .mongodb import MongoDB
+from .orms.mongodb import MongoDB
 # from .mysqldb import MysqlDB
-from .sqlitedb import SqliteDB
-from .postgresqldb import PostgresqlDB
+from .orms.sqlitedb import SqliteDB
+from .orms.postgresqldb import PostgresqlDB
 
 from bson.objectid import ObjectId
 
 def normalise(content: dict, optype: str = 'dbresult')-> dict:
     '''
     Static method of normalising database results\n
     Converts _id from mongodb to id
```

### Comparing `odbms-0.2.9/odbms/mongodb.py` & `odbms-0.3.0/odbms/orms/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from pymongo import MongoClient
 from pymongo.database import Database
 
 import os
 from typing import Union
 from dotenv import load_dotenv
 
+from .base import ORM
+
 load_dotenv()
 
 
-class MongoDB(object):
+class MongoDB(ORM):
     db: Database
     dbms = 'mongodb'
     
     @staticmethod
     def initialize(host, port, database, user=None, password=None):
         if port:
             client = MongoClient(host, int(port))
```

### Comparing `odbms-0.2.9/odbms/mysqldb.py` & `odbms-0.3.0/odbms/orms/mysqldb.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # @Link    : link
 # @Version : 1.0.0
 
 import os
 from mysql import connector
 from sys import exit
 
-class MysqlDB:
+from .base import ORM
+
+class MysqlDB(ORM):
     db = None
     dbms = 'mysql'
     cursor = None
     database_exists = True
     
     @staticmethod
     def connect(dbsettings: dict):
```

### Comparing `odbms-0.2.9/odbms/postgresqldb.py` & `odbms-0.3.0/odbms/orms/postgresqldb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,152 +1,193 @@
+import logging
 import psycopg2
 from psycopg2 import sql
 from psycopg2.extensions import connection, cursor as Cursor
 from typing import Union, List, Dict
 
-class PostgresqlDB:
+from .base import ORM
+
+class PostgresqlDB(ORM):
     db: connection
     cursor: Cursor
     dbms = 'postgresql'
 
     @staticmethod
-    def initialize(host, port, database, user, password):
+    def initialize(host, port, user, password, database):
         try:
+            # Connect to the PostgreSQL server without specifying a database
+            conn = psycopg2.connect(
+                host=host,
+                port=port,
+                user=user,
+                password=password
+            )
+            conn.autocommit = True
+            cursor = conn.cursor()
+
+            # Check if the database exists
+            cursor.execute(f"SELECT 1 FROM pg_database WHERE datname = '{database}'")
+            exists = cursor.fetchone()
+
+            if not exists:
+                # If the database doesn't exist, create it
+                cursor.execute(sql.SQL("CREATE DATABASE {}").format(sql.Identifier(database)))
+                logging.info(f"Database '{database}' created successfully.")
+
+            cursor.close()
+            conn.close()
+            
+            # Connect to the database
             PostgresqlDB.db = psycopg2.connect(
                 host=host,
                 port=port,
                 database=database,
                 user=user,
                 password=password
             )
             PostgresqlDB.db.set_session(autocommit=False)
             PostgresqlDB.cursor = PostgresqlDB.db.cursor()
+            
         except (Exception, psycopg2.Error) as error:
-            print("Error connecting to PostgreSQL database:", error)
+            logging.error("Error connecting to PostgreSQL database:", error)
 
     @staticmethod
-    def query(sql_query, params=None):
+    def execute(query, params=None):
         try:
             if params:
-                PostgresqlDB.cursor.execute(sql_query, params)
+                PostgresqlDB.cursor.execute(query, params)
             else:
-                PostgresqlDB.cursor.execute(sql_query)
-            result = PostgresqlDB.cursor.fetchall()
-            PostgresqlDB.db.commit()
-            return result
+                PostgresqlDB.cursor.execute(query)
+                PostgresqlDB.db.commit()
+
         except (Exception, psycopg2.Error) as error:
-            print("Error executing SQL:", error)
+            logging.exception(error)
             PostgresqlDB.db.rollback()
 
     @staticmethod
     def insert(table: str, data: Dict):
         columns = sql.SQL(', ').join(sql.Identifier(col) for col in data.keys())
         values = ', '.join(['%s'] * len(data))
-        sql_query = sql.SQL("INSERT INTO {} ({}) VALUES ({})").format(
+        sql_query = sql.SQL("INSERT INTO {} ({}) VALUES ({}) RETURNING id").format(
             sql.Identifier(table),
             columns,
             sql.SQL(values)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(data.values()))
             PostgresqlDB.db.commit()
+            new_inserts = PostgresqlDB.cursor.fetchone()
+            insert_id =   new_inserts[0] if new_inserts else 0
+            return insert_id
         except (Exception, psycopg2.Error) as error:
             print("Error inserting data:", error)
             PostgresqlDB.db.rollback()
+            return 0
 
     @staticmethod
     def insert_many(table: str, data: List[Dict]):
         columns = sql.SQL(', ').join(sql.Identifier(col) for col in data[0].keys())
         values_template = ', '.join(['%s'] * len(data[0]))
         values = ', '.join(['(' + values_template + ')'] * len(data))
         sql_query = sql.SQL("INSERT INTO {} ({}) VALUES {}").format(
             sql.Identifier(table),
             columns,
             sql.SQL(values)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, [value for row in data for value in row.values()])
             PostgresqlDB.db.commit()
+            return True
         except (Exception, psycopg2.Error) as error:
             print("Error inserting data:", error)
             PostgresqlDB.db.rollback()
+            return False
 
     @staticmethod
     def find(table: str, filter: Dict = {}, projection: Union[List, Dict] = []):
-        columns = sql.SQL(', ').join(sql.Identifier(col) for col in projection) if projection else sql.SQL('*')
-        conditions = ' AND '.join(f"{sql.Identifier(key)} = %s" for key in filter.keys())
+        columns = sql.SQL(', ').join(map(sql.Identifier, projection)) if projection else sql.SQL('*')
+        conditions = ' AND '.join(f"{key} = %s" for key in filter.keys())
         sql_query = sql.SQL("SELECT {} FROM {}").format(
             columns,
             sql.Identifier(table),
         )
         if filter:
             sql_query = sql.SQL("{} WHERE {}").format(
                 sql_query,
                 sql.SQL(conditions)
             )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(filter.values()))
-            result = PostgresqlDB.cursor.fetchall()
+            column_names = [desc.name for desc in PostgresqlDB.cursor.description] # type: ignore
+            result = [dict(zip(column_names, row)) for row in PostgresqlDB.cursor.fetchall()]
             PostgresqlDB.db.commit()
             return result
         except (Exception, psycopg2.Error) as error:
-            print("Error executing SQL:", error)
+            logging.error({'status': 'Error', 'message': str(error)})
             PostgresqlDB.db.rollback()
+            return []
 
     @staticmethod
     def find_one(table: str, filter: Dict = {}, projection: Union[List, Dict] = []):
-        columns = sql.SQL(', ').join(sql.Identifier(col) for col in projection) if projection else sql.SQL('*')
-        conditions = ' AND '.join(f"{sql.Identifier(key)} = %s" for key in filter.keys())
+        columns = sql.SQL(', ').join(map(sql.Identifier, projection)) if projection else sql.SQL('*')
+        conditions = ' AND '.join(f"{key} = %s" for key in filter.keys())
         sql_query = sql.SQL("SELECT {} FROM {} WHERE {} LIMIT 1").format(
-            columns, 
+            columns,
             sql.Identifier(table),
             sql.SQL(conditions)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(filter.values()))
-            result = PostgresqlDB.cursor.fetchone()
+            column_names = [desc.name for desc in PostgresqlDB.cursor.description] # type: ignore
+            result = dict(zip(column_names, PostgresqlDB.cursor.fetchone())) if PostgresqlDB.cursor.rowcount > 0 else None # type: ignore
             PostgresqlDB.db.commit()
+            
             return result
         except (Exception, psycopg2.Error) as error:
             print("Error executing SQL:", error)
             PostgresqlDB.db.rollback()
+            return {}
 
     @staticmethod
     def remove(table: str, filter: Dict):
-        conditions = ' AND '.join(f"{sql.Identifier(key)} = %s" for key in filter.keys())
+        conditions = ' AND '.join(f"{key} = %s" for key in filter.keys())
         sql_query = sql.SQL("DELETE FROM {} WHERE {}").format(
             sql.Identifier(table),
             sql.SQL(conditions)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(filter.values()))
             PostgresqlDB.db.commit()
+            return True
         except (Exception, psycopg2.Error) as error:
             print("Error removing data:", error)
             PostgresqlDB.db.rollback()
+            return False
 
     @staticmethod
     def update(table: str, filter: Dict, data: Dict):
-        set_clause = ', '.join(f"{sql.Identifier(key)} = %s" for key in data.keys())
-        conditions = ' AND '.join(f"{sql.Identifier(key)} = %s" for key in filter.keys())
+        set_clause = ', '.join(f"{key} = %s" for key in data.keys())
+        conditions = ' AND '.join(f"{key} = %s" for key in filter.keys())
         sql_query = sql.SQL("UPDATE {} SET {} WHERE {}").format(
             sql.Identifier(table),
             sql.SQL(set_clause),
             sql.SQL(conditions)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(data.values()) + list(filter.values()))
             PostgresqlDB.db.commit()
+            return True
         except (Exception, psycopg2.Error) as error:
             print("Error updating data:", error)
             PostgresqlDB.db.rollback()
+            return False
 
     @staticmethod
     def count(table: str, filter: Dict = {}):
-        conditions = ' AND '.join(f"{sql.Identifier(key)} = %s" for key in filter.keys())
+        conditions = ' AND '.join(f"{key} = %s" for key in filter.keys())
         sql_query = sql.SQL("SELECT COUNT(*) FROM {} WHERE {}").format(
             sql.Identifier(table),
             sql.SQL(conditions)
         )
         try:
             PostgresqlDB.cursor.execute(sql_query, list(filter.values()))
             result = PostgresqlDB.cursor.fetchone()
```

### Comparing `odbms-0.2.9/odbms/sqlitedb.py` & `odbms-0.3.0/odbms/orms/sqlitedb.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 # @Link    : link
 # @Version : 1.0.0
 
 import os
 import logging
 import sqlite3
 from sqlite3 import Connection, Cursor
-from sys import exit
 from typing import Union
 
-class SqliteDB:
+from .base import ORM
+
+class SqliteDB(ORM):
     db: Connection
     cursor: Cursor
     dbms = 'sqlite'
     
     @staticmethod
     def initialize(database):
         db = sqlite3.connect(database)
@@ -24,17 +25,17 @@
         cursor = db.cursor()
         SqliteDB.db = db
         SqliteDB.cursor = cursor
     
     @staticmethod
     def insert(table: str, data: dict):
 
-        query = f'INSERT INTO {table}('
+        query = f'INSERT INTO {table} ('
         query += ', '.join(data.keys())
-        query += ") VALUES('"
+        query += ") VALUES ('"
 
         values = [str(val) for val in data.values()]
         query += "','".join(values)
         query += "')"
         try:
             SqliteDB.cursor.execute(query)
             SqliteDB.db.commit()
@@ -71,31 +72,32 @@
             return SqliteDB.cursor.lastrowid
 
         except Exception as e:
             logging.error(str(e))
             return None
     
     @staticmethod
-    def find(table: str, params: dict = {}):
-        query = f'SELECT * FROM {table}'
+    def find(table: str, params: dict = {}, columns: list = ['*']):
+        query = f'SELECT {', '.join(columns)} FROM {table}'
 
         if len(params.keys()):
             query += ' WHERE '
             for key, value in params.items():
                 query += f"{key} = ?,"
             query = query.rstrip(',')
             
         try:
             SqliteDB.cursor.execute(query, tuple(params.values()))
             SqliteDB.db.commit()
-
-            return [x for x in SqliteDB.cursor.fetchall()]
+            
+            return SqliteDB.cursor.fetchall()
 
         except Exception as e:
-            return {'status': 'Error', 'message': str(e)}
+            logging.error({'status': 'Error', 'message': str(e)})
+            return []
     
     @staticmethod
     def find_one(table: str, params: dict = {}):
         query = f'SELECT * FROM {table}'
         
         if len(params.keys()):
             query += ' WHERE '
@@ -104,18 +106,19 @@
             query = query.rstrip(',')
         
         try:
             SqliteDB.cursor.execute(query, tuple(params.values()))
             SqliteDB.db.commit()
 
             resp = [x for x in SqliteDB.cursor.fetchall()]
-            return resp[0]
+            return resp[0] if len(resp) else resp
 
         except Exception as e:
-            return {'status': 'Error', 'message': str(e)}
+            logging.error({'status': 'Error', 'message': str(e)})
+            return []
     
     @staticmethod
     def count(table: str, params: dict = {})-> int:
         query = f'SELECT * FROM {table}'
 
         if len(params.keys()):
             query += ' WHERE '
@@ -150,15 +153,15 @@
             return SqliteDB.cursor.fetchall()[0]['sum']
 
         except Exception as e:
             logging.error(str(e))
             return 0
     
     @staticmethod
-    def query(query: str):
+    def execute(query: str):
         try:
             SqliteDB.cursor.execute(query)
             SqliteDB.db.commit()
 
             return [x for x in SqliteDB.cursor.fetchall()]
 
         except Exception as e:
@@ -210,13 +213,13 @@
         @param filename Name of file containing commands
         @return Database result
         '''
 
         try:
             result = None
             with open(filename, 'rt') as file:
-                result = SqliteDB.query(file.read())
+                result = SqliteDB.execute(file.read())
                 
             return result
                 
         except Exception as e:
             return {'status': 'Error', 'message': str(e)}
```

### Comparing `odbms-0.2.9/odbms.egg-info/PKG-INFO` & `odbms-0.3.0/odbms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.9
+Version: 0.3.0
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `odbms-0.2.9/setup.py` & `odbms-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.9'
+VERSION = '0.3.0'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='odbms',
     version=VERSION,
```

