# Comparing `tmp/pydqt-1.4.0.tar.gz` & `tmp/pydqt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydqt-1.4.0.tar", max compression
+gzip compressed data, was "pydqt-1.4.1.tar", max compression
```

## Comparing `pydqt-1.4.0.tar` & `pydqt-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    17606 2024-04-08 13:26:57.983811 pydqt-1.4.0/README.md
--rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.4.0/pydqt/__init__.py
--rw-r--r--   0        0        0    35944 2024-04-08 12:36:00.763438 pydqt-1.4.0/pydqt/pydqt.py
--rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.4.0/pydqt/sql/templates/macros/macros.jinja
--rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.4.0/pydqt/test.csv
--rw-r--r--   0        0        0     6687 2024-04-05 12:42:05.002914 pydqt-1.4.0/pydqt/tests/test_querying.py
--rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.4.0/pydqt/utils/__init__.py
--rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.4.0/pydqt/utils/custom_filters.py
--rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.4.0/pydqt/workspaces/main/templates/base.sql
--rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.4.0/pydqt/workspaces/main/templates/example.sql
--rw-r--r--   0        0        0      684 2024-04-08 13:25:26.257770 pydqt-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    18553 1970-01-01 00:00:00.000000 pydqt-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    17606 2024-04-08 13:26:57.983811 pydqt-1.4.1/README.md
+-rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.4.1/pydqt/__init__.py
+-rw-r--r--   0        0        0    35940 2024-04-18 10:08:48.887612 pydqt-1.4.1/pydqt/pydqt.py
+-rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.4.1/pydqt/sql/templates/macros/macros.jinja
+-rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.4.1/pydqt/test.csv
+-rw-r--r--   0        0        0     6687 2024-04-05 12:42:05.002914 pydqt-1.4.1/pydqt/tests/test_querying.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.4.1/pydqt/utils/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.4.1/pydqt/utils/custom_filters.py
+-rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.4.1/pydqt/workspaces/main/templates/base.sql
+-rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.4.1/pydqt/workspaces/main/templates/example.sql
+-rw-r--r--   0        0        0      684 2024-04-18 10:09:24.699374 pydqt-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    18553 1970-01-01 00:00:00.000000 pydqt-1.4.1/PKG-INFO
```

### Comparing `pydqt-1.4.0/README.md` & `pydqt-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydqt-1.4.0/pydqt/__init__.py` & `pydqt-1.4.1/pydqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.4.0/pydqt/pydqt.py` & `pydqt-1.4.1/pydqt/pydqt.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,16 +349,16 @@
                         )
 
     for var in ["SNOWFLAKE_LOGIN", "SNOWFLAKE_ROLE", "SNOWFLAKE_DEFAULT_DATABASE", "SNOWFLAKE_DEFAULT_SCHEMA"]:
         check_env_var(var)
 
     # Now have default values in function definition, above
     SNOWFLAKE_ROLE = os.getenv("SNOWFLAKE_ROLE")
-    # if not warehouse:
-    #     warehouse=f"{SNOWFLAKE_ROLE}_QUERY_LARGE_WH"
+    if not warehouse:
+        warehouse=f"{SNOWFLAKE_ROLE}_QUERY_LARGE_WH"
     # if not database:
     #     database = os.getenv("SNOWFLAKE_DEFAULT_DATABASE")
     # if not schema:
     #     schema = os.getenv("SNOWFLAKE_DEFAULT_SCHEMA")
 
     password=''
     if "SNOWFLAKE_PASSWORD" in os.environ:
```

### Comparing `pydqt-1.4.0/pydqt/sql/templates/macros/macros.jinja` & `pydqt-1.4.1/pydqt/sql/templates/macros/macros.jinja`

 * *Files identical despite different names*

### Comparing `pydqt-1.4.0/pydqt/test.csv` & `pydqt-1.4.1/pydqt/test.csv`

 * *Files identical despite different names*

### Comparing `pydqt-1.4.0/pydqt/tests/test_querying.py` & `pydqt-1.4.1/pydqt/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.4.0/pyproject.toml` & `pydqt-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydqt"
-version = "1.4.0"
+version = "1.4.1"
 description = "A package to help parameterise and macrofy sql queries"
 authors = ["Mark Ingham <mark.ingham@ly.st>"]
 readme = "README.md"
 repository = "https://github.com/markingham77/dqt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `pydqt-1.4.0/PKG-INFO` & `pydqt-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydqt
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package to help parameterise and macrofy sql queries
 Home-page: https://github.com/markingham77/dqt
 License: MIT
 Author: Mark Ingham
 Author-email: mark.ingham@ly.st
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

