# Comparing `tmp/shipyard_motherduck-0.1.0a2.tar.gz` & `tmp/shipyard_motherduck-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_motherduck-0.1.0a2.tar", max compression
+gzip compressed data, was "shipyard_motherduck-0.1.0a3.tar", max compression
```

## Comparing `shipyard_motherduck-0.1.0a2.tar` & `shipyard_motherduck-0.1.0a3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-11 02:41:42.600015 shipyard_motherduck-0.1.0a2/README.md
--rw-r--r--   0        0        0      618 2024-04-17 01:51:07.343057 shipyard_motherduck-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-11 13:59:39.563880 shipyard_motherduck-0.1.0a2/shipyard_motherduck/__init__.py
--rw-r--r--   0        0        0      547 2024-04-17 00:40:23.894354 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/authtest.py
--rw-r--r--   0        0        0     1090 2024-04-17 01:50:41.897777 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/execute.py
--rw-r--r--   0        0        0     1880 2024-04-17 01:39:58.136436 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/fetch.py
--rw-r--r--   0        0        0     2817 2024-04-17 00:40:23.938301 shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/upload.py
--rw-r--r--   0        0        0      865 2024-04-17 00:40:23.907409 shipyard_motherduck-0.1.0a2/shipyard_motherduck/errors.py
--rw-r--r--   0        0        0     6433 2024-04-17 00:40:23.959410 shipyard_motherduck-0.1.0a2/shipyard_motherduck/motherduck.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 02:41:42.600015 shipyard_motherduck-0.1.0a3/README.md
+-rw-r--r--   0        0        0      618 2024-04-17 16:58:13.635062 shipyard_motherduck-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-11 13:59:39.563880 shipyard_motherduck-0.1.0a3/shipyard_motherduck/__init__.py
+-rw-r--r--   0        0        0      547 2024-04-17 00:40:23.894354 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/authtest.py
+-rw-r--r--   0        0        0     1088 2024-04-17 01:51:26.107771 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/execute.py
+-rw-r--r--   0        0        0     1880 2024-04-17 01:39:58.136436 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/fetch.py
+-rw-r--r--   0        0        0     3061 2024-04-17 16:58:08.969443 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/upload.py
+-rw-r--r--   0        0        0      865 2024-04-17 00:40:23.907409 shipyard_motherduck-0.1.0a3/shipyard_motherduck/exceptions.py
+-rw-r--r--   0        0        0     7097 2024-04-17 16:58:08.988425 shipyard_motherduck-0.1.0a3/shipyard_motherduck/motherduck.py
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.0a3/PKG-INFO
```

### Comparing `shipyard_motherduck-0.1.0a2/pyproject.toml` & `shipyard_motherduck-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-motherduck"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "A local client for working with Python and MotherDuck"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.2"
```

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/authtest.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/execute.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/execute.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def main():
     try:
         args = get_args()
         query = args.query
         database = args.database if args.database != "" else None
-        client = MotherDuckClient(args.token, database = database)
+        client = MotherDuckClient(args.token, database=database)
         client.execute_query(query)
 
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(
```

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/fetch.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/cli/upload.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,16 +58,21 @@
             logger.info(f"Found {n_matches} file matches, preparing to upload...")
             for file in file_matches:
                 logger.debug(f"Uploading {file}")
                 client.upload(table_name, file, insert_method=insert_method)
                 if insert_method == "replace":
                     insert_method = "append"
             logger.info("Successfully uploaded all files")
-        else:
+        elif args.match_type == "exact_match":
             client.upload(table_name, file_path, insert_method=insert_method)
+        else:
+            logger.error(
+                "Invalid match type, select either 'glob_match', 'exact_match', or 'regex_match'"
+            )
+            sys.exit(Database.EXIT_CODE_INVALID_ARGUMENTS)
     except FileNotFoundError:
         logger.error(f"File {file_path} not found")
         sys.exit(Database.EXIT_CODE_FILE_NOT_FOUND)
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
```

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/errors.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a2/shipyard_motherduck/motherduck.py` & `shipyard_motherduck-0.1.0a3/shipyard_motherduck/motherduck.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from shipyard_templates import ShipyardLogger, Database, ExitCodeException
 from shipyard_templates.database import (
     FetchError,
     UploadError,
     ConnectionError,
     QueryError,
 )
-from shipyard_motherduck.errors import (
+from shipyard_motherduck.exceptions import (
     TempTableCreationFailed,
     TempTableInsertFailed,
     TempTableDropFailed,
 )
 from typing import Optional
 
 logger = ShipyardLogger().get_logger()
@@ -176,16 +176,20 @@
             src_table (str): The name of the source table.
             target_table (str): The name of the target table.
 
         Returns:
             None
         """
         try:
-            cmd = f"INSERT INTO {target_table} SELECT * FROM '{src_table}'"
-            self.conn.sql(cmd)
+            if not self._exists(target_table):
+                cmd = f"CREATE TABLE {target_table} AS SELECT * FROM '{src_table}'"
+                self.conn.sql(cmd)
+            else:
+                cmd = f"INSERT INTO {target_table} SELECT * FROM '{src_table}'"
+                self.conn.sql(cmd)
         except Exception:
             raise TempTableInsertFailed(src_table, target_table)
 
     def _drop(self, table_name: str):
         """
         Drops a table from the specified database.
 
@@ -196,7 +200,24 @@
             None
         """
         try:
             cmd = f"DROP TABLE {table_name}"
             self.conn.sql(cmd)
         except Exception:
             raise TempTableDropFailed(table_name)
+
+    def _exists(self, table_name: str) -> bool:
+        """
+        Checks if a table exists in the database.
+
+        Args:
+            table_name (str): The name of the table to check for existence.
+
+        Returns:
+            bool: True if the table exists, False otherwise.
+        """
+        try:
+            cmd = f"SELECT * FROM {table_name} LIMIT 1"
+            self.conn.sql(cmd)
+            return True
+        except Exception:
+            return False
```

### Comparing `shipyard_motherduck-0.1.0a2/PKG-INFO` & `shipyard_motherduck-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-motherduck
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A local client for working with Python and MotherDuck
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

