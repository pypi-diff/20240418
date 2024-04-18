# Comparing `tmp/ksqldb_client-0.28.2a1.tar.gz` & `tmp/ksqldb_client-0.28.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksqldb_client-0.28.2a1.tar", max compression
+gzip compressed data, was "ksqldb_client-0.28.2a2.tar", max compression
```

## Comparing `ksqldb_client-0.28.2a1.tar` & `ksqldb_client-0.28.2a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-03-09 20:43:55.773215 ksqldb_client-0.28.2a1/LICENSE
--rw-r--r--   0        0        0      127 2024-03-09 20:40:28.140661 ksqldb_client-0.28.2a1/README.md
--rw-r--r--   0        0        0    10693 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a1/ksqldb_client/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a1/ksqldb_client/decorators.py
--rw-r--r--   0        0        0      502 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a1/ksqldb_client/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a1/ksqldb_client/models/__init__.py
--rw-r--r--   0        0        0      151 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a1/ksqldb_client/models/base.py
--rw-r--r--   0        0        0      426 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a1/ksqldb_client/models/info_response.py
--rw-r--r--   0        0        0     1689 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a1/ksqldb_client/models/ksql_response.py
--rw-r--r--   0        0        0      999 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a1/ksqldb_client/models/query_response.py
--rw-r--r--   0        0        0      212 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a1/ksqldb_client/models/status_response.py
--rw-r--r--   0        0        0        0 2024-03-11 10:14:39.276743 ksqldb_client-0.28.2a1/ksqldb_client/testing/__init__.py
--rw-r--r--   0        0        0     3802 2024-03-11 10:14:39.284743 ksqldb_client-0.28.2a1/ksqldb_client/testing/parse.py
--rw-r--r--   0        0        0      235 2024-03-11 10:14:39.284743 ksqldb_client-0.28.2a1/ksqldb_client/testing/to_timestamp.py
--rw-r--r--   0        0        0     1199 2024-03-11 10:24:49.865971 ksqldb_client-0.28.2a1/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 ksqldb_client-0.28.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-03-09 20:43:55.773215 ksqldb_client-0.28.2a2/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-17 13:08:56.813676 ksqldb_client-0.28.2a2/README.md
+-rw-r--r--   0        0        0    10693 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a2/ksqldb_client/__init__.py
+-rw-r--r--   0        0        0     1311 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a2/ksqldb_client/decorators.py
+-rw-r--r--   0        0        0      502 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a2/ksqldb_client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a2/ksqldb_client/models/__init__.py
+-rw-r--r--   0        0        0      151 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a2/ksqldb_client/models/base.py
+-rw-r--r--   0        0        0      426 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a2/ksqldb_client/models/info_response.py
+-rw-r--r--   0        0        0     1689 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a2/ksqldb_client/models/ksql_response.py
+-rw-r--r--   0        0        0      999 2024-03-09 20:25:41.201261 ksqldb_client-0.28.2a2/ksqldb_client/models/query_response.py
+-rw-r--r--   0        0        0      212 2024-03-03 09:00:44.964706 ksqldb_client-0.28.2a2/ksqldb_client/models/status_response.py
+-rw-r--r--   0        0        0        0 2024-03-11 10:14:39.276743 ksqldb_client-0.28.2a2/ksqldb_client/testing/__init__.py
+-rw-r--r--   0        0        0     3979 2024-04-18 06:27:54.208006 ksqldb_client-0.28.2a2/ksqldb_client/testing/parse.py
+-rw-r--r--   0        0        0      235 2024-03-11 10:14:39.284743 ksqldb_client-0.28.2a2/ksqldb_client/testing/to_timestamp.py
+-rw-r--r--   0        0        0     1199 2024-04-18 06:47:23.078167 ksqldb_client-0.28.2a2/pyproject.toml
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 ksqldb_client-0.28.2a2/PKG-INFO
```

### Comparing `ksqldb_client-0.28.2a1/LICENSE` & `ksqldb_client-0.28.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ksqldb_client-0.28.2a1/ksqldb_client/__init__.py` & `ksqldb_client-0.28.2a2/ksqldb_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ksqldb_client-0.28.2a1/ksqldb_client/decorators.py` & `ksqldb_client-0.28.2a2/ksqldb_client/decorators.py`

 * *Files identical despite different names*

### Comparing `ksqldb_client-0.28.2a1/ksqldb_client/models/ksql_response.py` & `ksqldb_client-0.28.2a2/ksqldb_client/models/ksql_response.py`

 * *Files identical despite different names*

### Comparing `ksqldb_client-0.28.2a1/ksqldb_client/models/query_response.py` & `ksqldb_client-0.28.2a2/ksqldb_client/models/query_response.py`

 * *Files identical despite different names*

### Comparing `ksqldb_client-0.28.2a1/ksqldb_client/testing/parse.py` & `ksqldb_client-0.28.2a2/ksqldb_client/testing/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 def extract_columns_from_ksql_schema(schema: str) -> dict[str, str]:
     parts = re.split(r",(?![^<]*>)", schema)
 
     result: dict[str, str] = {}
     for part in parts:
         part_stripped = part.strip()
-        if re.search(r"STRUCT<.*>", part_stripped):
-            if match := re.search(r"`([^`]+)`\s+(STRUCT)<", part_stripped):
+        if re.search(r"(STRUCT|ARRAY)<.*>", part_stripped):
+            if match := re.search(r"`([^`]+)`\s+(STRUCT|ARRAY)<", part_stripped):
                 result.update({match.group(1): match.group(2)})
         elif match := re.search(r"`([^`]+)`\s+([A-Z]+)", part_stripped):
             result.update({match.group(1): match.group(2)})
 
     return result
 
 
@@ -47,14 +47,15 @@
 KSQL_TO_PANDAS_TYPES = {
     "STRING": pd.StringDtype(),
     "BOOLEAN": pd.BooleanDtype(),
     "INTEGER": pd.Int64Dtype(),
     "BIGINT": pd.Int64Dtype(),
     "DOUBLE": pd.Float64Dtype(),
     "DECIMAL": pd.Float64Dtype(),
+    "DATE": pd.DatetimeTZDtype(tz="utc"),
     "TIMESTAMP": pd.DatetimeTZDtype(tz="utc"),
     "ARRAY": "object",
     "MAP": "object",
     "STRUCT": "object",
 }
 
 
@@ -62,41 +63,42 @@
     """Convert a ksql query response to a pandas DataFrame.
 
     Note: Column names are converted to lowercase.
     """
     header = extract_header_from_query_response(query_response)
     rows = extract_rows_from_query_response(query_response)
 
-    columns = extract_columns_from_ksql_schema(header.header.schema_)
 
-    column_names = tuple(column_name.lower() for column_name in columns)
-    pandas_column_types = tuple(KSQL_TO_PANDAS_TYPES[ksql_column_type] for ksql_column_type in columns.values())
 
     data = tuple(row.row.columns for row in rows)
 
+    column_name_to_ksqldb_type_dict = extract_columns_from_ksql_schema(header.header.schema_)
+    column_names = tuple(column_name.lower() for column_name in column_name_to_ksqldb_type_dict)
+    pandas_column_types = tuple(KSQL_TO_PANDAS_TYPES[ksql_column_type] for ksql_column_type in column_name_to_ksqldb_type_dict.values())
+
     return pd.DataFrame(
-        dictionary_keys_to_lowercase(data),
+        dictionary_keys_to_lowercase_recursively(data),
         columns=column_names,
     ).astype(
         dict(
             zip(
                 column_names,
                 pandas_column_types,
                 strict=True,
             ),
         ),
     )
 
 
-def dictionary_keys_to_lowercase(dict_: dict[str, Any] | tuple[Any, ...]) -> dict[str, Any] | tuple[Any, ...]:
+def dictionary_keys_to_lowercase_recursively(dict_: dict[str, Any] | tuple[Any, ...]) -> dict[str, Any] | tuple[Any, ...]:
     """Convert all dictionary keys to lowercase, including nested dictionaries and lists of dictionaries."""
     if isinstance(dict_, dict):
-        return {k.lower(): dictionary_keys_to_lowercase(v) for k, v in dict_.items()}
+        return {k.lower(): dictionary_keys_to_lowercase_recursively(v) for k, v in dict_.items()}
     if isinstance(dict_, tuple):
-        return tuple(dictionary_keys_to_lowercase(v) for v in dict_)
+        return tuple(dictionary_keys_to_lowercase_recursively(v) for v in dict_)
 
     return dict_
 
 
 KSQLDB_TO_REDSHIFT_TYPES = {
     "BOOLEAN": "BOOLEAN",
     "INTEGER": "INTEGER",
```

### Comparing `ksqldb_client-0.28.2a1/pyproject.toml` & `ksqldb_client-0.28.2a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "ksqldb-client"
 version = "0.28.2a1"
 requires-python = ">=3.10"
 
 [tool.poetry]
 name = "ksqldb-client"
-version = "0.28.2a1"
+version = "0.28.2a2"
 description = ""
 authors = ["Ander Aramburu <ander.aranfdz@gmail.com>"]
 readme = "README.md"
 packages = []
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `ksqldb_client-0.28.2a1/PKG-INFO` & `ksqldb_client-0.28.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksqldb-client
-Version: 0.28.2a1
+Version: 0.28.2a2
 Summary: 
 Author: Ander Aramburu
 Author-email: ander.aranfdz@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,7 +13,8 @@
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # KSqlDB Client
 
 A Python client to interact with the [KSqlDB REST API](https://docs.ksqldb.io/en/latest/developer-guide/api/).
+
```

