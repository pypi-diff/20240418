# Comparing `tmp/databricks_sql_connector-3.1.1.tar.gz` & `tmp/databricks_sql_connector-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-3.1.1.tar", max compression
+gzip compressed data, was "databricks_sql_connector-3.1.2.tar", max compression
```

## Comparing `databricks_sql_connector-3.1.1.tar` & `databricks_sql_connector-3.1.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     9139 2024-03-19 22:27:50.765360 databricks_sql_connector-3.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2024-03-19 22:27:50.765360 databricks_sql_connector-3.1.1/LICENSE
--rw-r--r--   0        0        0     2928 2024-03-19 22:27:50.765360 databricks_sql_connector-3.1.1/README.md
--rw-r--r--   0        0        0     1822 2024-03-19 22:28:13.333356 databricks_sql_connector-3.1.1/pyproject.toml
--rw-r--r--   0        0        0      537 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/__init__.py
--rw-r--r--   0        0        0     2128 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4409 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6079 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     4697 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9989 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0    17735 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/retry.py
--rw-r--r--   0        0        0     7058 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    49670 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/client.py
--rw-r--r--   0        0        0     6547 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/cloudfetch/download_manager.py
--rw-r--r--   0        0        0     6374 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/cloudfetch/downloader.py
--rw-r--r--   0        0        0     3142 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/experimental/oauth_persistence.py
--rw-r--r--   0        0        0      336 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/parameters/__init__.py
--rw-r--r--   0        0        0    19116 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/parameters/native.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/parameters/py.typed
--rwxr-xr-x   0        0        0     7779 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   130572 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2024-03-19 22:27:50.769360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2199428 2024-03-19 22:27:50.773360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2024-03-19 22:27:50.773360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    44079 2024-03-19 22:27:50.773360 databricks_sql_connector-3.1.1/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6811 2024-03-19 22:27:50.773360 databricks_sql_connector-3.1.1/src/databricks/sql/types.py
--rw-r--r--   0        0        0    20997 2024-03-19 22:27:50.773360 databricks_sql_connector-3.1.1/src/databricks/sql/utils.py
--rw-r--r--   0        0        0    12281 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/README.sqlalchemy.md
--rw-r--r--   0        0        0     4239 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/README.tests.md
--rw-r--r--   0        0        0      185 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3879 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_ddl.py
--rw-r--r--   0        0        0    13048 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_parse.py
--rw-r--r--   0        0        0    11753 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_types.py
--rw-r--r--   0        0        0    15619 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/base.py
--rw-r--r--   0        0        0     9019 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      106 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/setup.cfg
--rw-r--r--   0        0        0     1955 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_extra.py
--rw-r--r--   0        0        0    12658 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_future.py
--rw-r--r--   0        0        0     5412 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_regression.py
--rw-r--r--   0        0        0    16061 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_unsupported.py
--rw-r--r--   0        0        0      597 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/conftest.py
--rw-r--r--   0        0        0     7043 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/overrides/_componentreflectiontest.py
--rw-r--r--   0        0        0     1026 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/overrides/_ctetest.py
--rw-r--r--   0        0        0      492 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/test_suite.py
--rw-r--r--   0        0        0      132 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/__init__.py
--rw-r--r--   0        0        0      951 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/conftest.py
--rw-r--r--   0        0        0    59837 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/e2e/MOCK_DATA.xlsx
--rw-r--r--   0        0        0    16749 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/e2e/test_basic.py
--rw-r--r--   0        0        0     3171 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_ddl.py
--rw-r--r--   0        0        0     5017 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_parsing.py
--rw-r--r--   0        0        0     6749 2024-03-19 22:27:50.777360 databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_types.py
--rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 databricks_sql_connector-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9240 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/LICENSE
+-rw-r--r--   0        0        0     2928 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/README.md
+-rw-r--r--   0        0        0     1822 2024-04-18 17:09:09.157776 databricks_sql_connector-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      537 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/py.typed
+-rw-r--r--   0        0        0     2362 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4409 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6079 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     4697 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9989 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0    17735 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/retry.py
+-rw-r--r--   0        0        0     6883 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    49978 2024-04-18 17:08:45.153551 databricks_sql_connector-3.1.2/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     6547 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/cloudfetch/download_manager.py
+-rw-r--r--   0        0        0     6374 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/cloudfetch/downloader.py
+-rw-r--r--   0        0        0     3142 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/experimental/oauth_persistence.py
+-rw-r--r--   0        0        0      336 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/parameters/__init__.py
+-rw-r--r--   0        0        0    19116 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/parameters/native.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/parameters/py.typed
+-rwxr-xr-x   0        0        0     7779 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   130572 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-18 17:08:45.157552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2199428 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    44079 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6811 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sql/types.py
+-rw-r--r--   0        0        0    20997 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0    12281 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/README.sqlalchemy.md
+-rw-r--r--   0        0        0     4239 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/README.tests.md
+-rw-r--r--   0        0        0      185 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3879 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_ddl.py
+-rw-r--r--   0        0        0    13048 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_parse.py
+-rw-r--r--   0        0        0    11753 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    15619 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/base.py
+-rw-r--r--   0        0        0     9019 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      106 2024-04-18 17:08:45.161552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/setup.cfg
+-rw-r--r--   0        0        0     1955 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_extra.py
+-rw-r--r--   0        0        0    12658 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_future.py
+-rw-r--r--   0        0        0     5412 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_regression.py
+-rw-r--r--   0        0        0    16061 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_unsupported.py
+-rw-r--r--   0        0        0      597 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/conftest.py
+-rw-r--r--   0        0        0     7043 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/overrides/_componentreflectiontest.py
+-rw-r--r--   0        0        0     1026 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/overrides/_ctetest.py
+-rw-r--r--   0        0        0      492 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/test_suite.py
+-rw-r--r--   0        0        0      132 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/conftest.py
+-rw-r--r--   0        0        0    59837 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/e2e/MOCK_DATA.xlsx
+-rw-r--r--   0        0        0    16749 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/e2e/test_basic.py
+-rw-r--r--   0        0        0     3171 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_ddl.py
+-rw-r--r--   0        0        0     5017 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_parsing.py
+-rw-r--r--   0        0        0     6749 2024-04-18 17:08:45.165552 databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_types.py
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 databricks_sql_connector-3.1.2/PKG-INFO
```

### Comparing `databricks_sql_connector-3.1.1/CHANGELOG.md` & `databricks_sql_connector-3.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Release History
 
-# x.x.x (TBD)
+# 3.1.2 (2024-04-18)
+
+- Remove broken cookie code (#379)
+- Small typing fixes (#382, #384 thanks @wyattscarpenter)
 
 # 3.1.1 (2024-03-19)
 
 - Don't retry requests that fail with code 403 (#373)
 - Assume a default retry-after for 429/503 (#371)
 - Fix boolean literals (#357)
```

### Comparing `databricks_sql_connector-3.1.1/LICENSE` & `databricks_sql_connector-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/README.md` & `databricks_sql_connector-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/pyproject.toml` & `databricks_sql_connector-3.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "3.1.1"
+version = "3.1.2"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "databricks", from = "src" }]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-3.1.1/src/databricks/__init__.py` & `databricks_sql_connector-3.1.2/src/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/__init__.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 apilevel = "2.0"
 threadsafety = 1  # Threads may share the module, but not connections.
 
 paramstyle = "named"
 
 import re
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    # Use this import purely for type annotations, a la https://mypy.readthedocs.io/en/latest/runtime_troubles.html#import-cycles
+    from .client import Connection
+
 
 class RedactUrlQueryParamsFilter(logging.Filter):
     pattern = re.compile(r"(\?|&)([\w-]+)=([^&]+)")
     mask = r"\1\2=<REDACTED>"
 
     def __init__(self):
         super().__init__()
@@ -58,15 +64,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "3.1.1"
+__version__ = "3.1.2"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
 
 
@@ -74,11 +80,11 @@
     return Date(*time.localtime(ticks)[:3])
 
 
 def TimestampFromTicks(ticks):
     return Timestamp(*time.localtime(ticks)[:6])
 
 
-def connect(server_hostname, http_path, access_token=None, **kwargs):
+def connect(server_hostname, http_path, access_token=None, **kwargs) -> "Connection":
     from .client import Connection
 
     return Connection(server_hostname, http_path, access_token, **kwargs)
```

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/retry.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/retry.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/auth/thrift_http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,18 +185,14 @@
         )
 
         # Get reply to flush the request
         self.code = self.__resp.status
         self.message = self.__resp.reason
         self.headers = self.__resp.headers
 
-        # Saves the cookie sent by the server response
-        if "Set-Cookie" in self.headers:
-            self.setCustomHeaders(dict("Cookie", self.headers["Set-Cookie"]))
-
     @staticmethod
     def basic_proxy_auth_header(proxy):
         if proxy is None or not proxy.username:
             return None
         ap = "%s:%s" % (
             urllib.parse.unquote(proxy.username),
             urllib.parse.unquote(proxy.password),
```

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/client.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,16 @@
                 "This approach will be deprecated in a future release. Consider using native parameters."
                 "Learn more: https://github.com/databricks/databricks-sql-python/tree/main/docs/parameters.md"
                 'To suppress this warning, set use_inline_params="silent"'
             )
 
         return value
 
-    def __enter__(self):
+    # The ideal return type for this method is perhaps Self, but that was not added until 3.11, and we support pre-3.11 pythons, currently.
+    def __enter__(self) -> "Connection":
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __del__(self):
         if self.open:
@@ -405,15 +406,16 @@
         self.open = True
         self.executing_command_id = None
         self.thrift_backend = thrift_backend
         self.active_op_handle = None
         self.escaper = ParamEscaper()
         self.lastrowid = None
 
-    def __enter__(self):
+    # The ideal return type for this method is perhaps Self, but that was not added until 3.11, and we support pre-3.11 pythons, currently.
+    def __enter__(self) -> "Cursor":
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __iter__(self):
         if self.active_result_set:
```

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/cloudfetch/download_manager.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/cloudfetch/download_manager.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/cloudfetch/downloader.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/cloudfetch/downloader.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/exc.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/parameters/native.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/parameters/native.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/thrift_backend.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/types.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sql/utils.py` & `databricks_sql_connector-3.1.2/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/README.sqlalchemy.md` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/README.sqlalchemy.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/README.tests.md` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/README.tests.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_ddl.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_ddl.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_parse.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_parse.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/_types.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/base.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/requirements.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_extra.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_extra.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_future.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_future.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_regression.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_regression.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/_unsupported.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/_unsupported.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/conftest.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/conftest.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/overrides/_componentreflectiontest.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/overrides/_componentreflectiontest.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test/overrides/_ctetest.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test/overrides/_ctetest.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/conftest.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/conftest.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/e2e/MOCK_DATA.xlsx` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/e2e/MOCK_DATA.xlsx`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/e2e/test_basic.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/e2e/test_basic.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_ddl.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_ddl.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_parsing.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_parsing.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/src/databricks/sqlalchemy/test_local/test_types.py` & `databricks_sql_connector-3.1.2/src/databricks/sqlalchemy/test_local/test_types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-3.1.1/PKG-INFO` & `databricks_sql_connector-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 3.1.1
+Version: 3.1.2
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

