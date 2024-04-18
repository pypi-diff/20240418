# Comparing `tmp/algoseek_connector-2.1.2.tar.gz` & `tmp/algoseek_connector-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algoseek_connector-2.1.2.tar", max compression
+gzip compressed data, was "algoseek_connector-2.1.3.tar", max compression
```

## Comparing `algoseek_connector-2.1.2.tar` & `algoseek_connector-2.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     9770 2023-10-31 13:58:49.434087 algoseek_connector-2.1.2/LICENSE
--rw-r--r--   0        0        0       48 2023-10-31 13:58:49.434087 algoseek_connector-2.1.2/NOTICE
--rw-r--r--   0        0        0     2241 2023-10-31 13:58:49.434087 algoseek_connector-2.1.2/README.md
--rw-r--r--   0        0        0     1798 2023-10-31 13:58:49.442087 algoseek_connector-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      517 2023-10-31 13:58:49.442087 algoseek_connector-2.1.2/src/algoseek_connector/__init__.py
--rw-r--r--   0        0        0    30999 2023-10-31 13:58:49.442087 algoseek_connector-2.1.2/src/algoseek_connector/base.py
--rw-r--r--   0        0        0      255 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/__init__.py
--rw-r--r--   0        0        0     1858 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/alias.json
--rw-r--r--   0        0        0     3716 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/case_insensitive.json
--rw-r--r--   0        0        0    18207 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/client.py
--rw-r--r--   0        0        0     8434 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/sqla_table.py
--rw-r--r--   0        0        0    13653 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/config.py
--rw-r--r--   0        0        0     1515 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/constants.py
--rw-r--r--   0        0        0      790 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/default-config.toml
--rw-r--r--   0        0        0     3253 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/manager.py
--rw-r--r--   0        0        0    12114 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/metadata_api.py
--rw-r--r--   0        0        0      287 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/s3/__init__.py
--rw-r--r--   0        0        0    15544 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/s3/client.py
--rw-r--r--   0        0        0    21430 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/s3/downloader.py
--rw-r--r--   0        0        0     2250 2023-10-31 13:58:49.446087 algoseek_connector-2.1.2/src/algoseek_connector/utils.py
--rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 algoseek_connector-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9770 2024-04-18 14:00:00.155136 algoseek_connector-2.1.3/LICENSE
+-rw-r--r--   0        0        0       48 2024-04-18 14:00:00.155136 algoseek_connector-2.1.3/NOTICE
+-rw-r--r--   0        0        0     2241 2024-04-18 14:00:00.155136 algoseek_connector-2.1.3/README.md
+-rw-r--r--   0        0        0     1945 2024-04-18 14:00:00.163136 algoseek_connector-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      517 2024-04-18 14:00:00.163136 algoseek_connector-2.1.3/src/algoseek_connector/__init__.py
+-rw-r--r--   0        0        0    30999 2024-04-18 14:00:00.163136 algoseek_connector-2.1.3/src/algoseek_connector/base.py
+-rw-r--r--   0        0        0      255 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1858 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/alias.json
+-rw-r--r--   0        0        0     3716 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/case_insensitive.json
+-rw-r--r--   0        0        0    18207 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/client.py
+-rw-r--r--   0        0        0     8434 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/sqla_table.py
+-rw-r--r--   0        0        0    13653 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/config.py
+-rw-r--r--   0        0        0     1515 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/constants.py
+-rw-r--r--   0        0        0      790 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/default-config.toml
+-rw-r--r--   0        0        0     3253 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/manager.py
+-rw-r--r--   0        0        0    12114 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/metadata_api.py
+-rw-r--r--   0        0        0      287 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/s3/__init__.py
+-rw-r--r--   0        0        0    15544 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/s3/client.py
+-rw-r--r--   0        0        0    21430 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/s3/downloader.py
+-rw-r--r--   0        0        0     2250 2024-04-18 14:00:00.167136 algoseek_connector-2.1.3/src/algoseek_connector/utils.py
+-rw-r--r--   0        0        0     3821 1970-01-01 00:00:00.000000 algoseek_connector-2.1.3/PKG-INFO
```

### Comparing `algoseek_connector-2.1.2/LICENSE` & `algoseek_connector-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/README.md` & `algoseek_connector-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/pyproject.toml` & `algoseek_connector-2.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "algoseek-connector"
-version = "2.1.2"
+version = "2.1.3"
 description = "A wrapper library for ORM-like SQL builder and executor"
 authors = [
     "Taras Kuzyo <taras@algoseek.com>",
     "Gabriel Riquelme <gabrielr@algoseek.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
@@ -22,22 +22,26 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Database",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
+[tool.poetry.urls]
+"GitHub" = "https://github.com/algoseekgit/algoseek-connector/"
+"Documentation" = "https://algoseek-connector.readthedocs.io/"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 pandas = "^2.0.2"
 clickhouse-sqlalchemy = "^0.2.4"
 sqlalchemy = "^1.4"
 clickhouse-connect = "^0.6.6"
-sqlparse = "^0.4.4"
+sqlparse = "^0.5.0"
 boto3 = "^1.28.11"
 botocore = "^1.31.12"
 tomli = "^2.0.1"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/__init__.py` & `algoseek_connector-2.1.3/src/algoseek_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/base.py` & `algoseek_connector-2.1.3/src/algoseek_connector/base.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/alias.json` & `algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/alias.json`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/case_insensitive.json` & `algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/case_insensitive.json`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/client.py` & `algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/client.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/clickhouse/sqla_table.py` & `algoseek_connector-2.1.3/src/algoseek_connector/clickhouse/sqla_table.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/config.py` & `algoseek_connector-2.1.3/src/algoseek_connector/config.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/constants.py` & `algoseek_connector-2.1.3/src/algoseek_connector/constants.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/default-config.toml` & `algoseek_connector-2.1.3/src/algoseek_connector/default-config.toml`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/manager.py` & `algoseek_connector-2.1.3/src/algoseek_connector/manager.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/metadata_api.py` & `algoseek_connector-2.1.3/src/algoseek_connector/metadata_api.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/s3/client.py` & `algoseek_connector-2.1.3/src/algoseek_connector/s3/client.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/s3/downloader.py` & `algoseek_connector-2.1.3/src/algoseek_connector/s3/downloader.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/src/algoseek_connector/utils.py` & `algoseek_connector-2.1.3/src/algoseek_connector/utils.py`

 * *Files identical despite different names*

### Comparing `algoseek_connector-2.1.2/PKG-INFO` & `algoseek_connector-2.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
 Name: algoseek-connector
-Version: 2.1.2
+Version: 2.1.3
 Summary: A wrapper library for ORM-like SQL builder and executor
 License: Apache-2.0
 Author: Taras Kuzyo
 Author-email: taras@algoseek.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: boto3 (>=1.28.11,<2.0.0)
 Requires-Dist: botocore (>=1.31.12,<2.0.0)
 Requires-Dist: clickhouse-connect (>=0.6.6,<0.7.0)
 Requires-Dist: clickhouse-sqlalchemy (>=0.2.4,<0.3.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
-Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
+Requires-Dist: sqlparse (>=0.5.0,<0.6.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Project-URL: Documentation, https://algoseek-connector.readthedocs.io/
+Project-URL: GitHub, https://github.com/algoseekgit/algoseek-connector/
 Description-Content-Type: text/markdown
 
 Algoseek Connector
 ==================
 
 [![Documentation Status](https://readthedocs.org/projects/algoseek-connector/badge/?version=latest)](https://algoseek-connector.readthedocs.io/en/latest/?badge=latest) ![example workflow](https://github.com/algoseekgit/algoseek-connector/actions/workflows/unit-tests.yml/badge.svg)
```

