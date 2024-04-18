# Comparing `tmp/pydantic_sql_bridge-0.0.6.tar.gz` & `tmp/pydantic_sql_bridge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_sql_bridge-0.0.6.tar", max compression
+gzip compressed data, was "pydantic_sql_bridge-0.0.7.tar", max compression
```

## Comparing `pydantic_sql_bridge-0.0.6.tar` & `pydantic_sql_bridge-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-10-24 11:21:28.890406 pydantic_sql_bridge-0.0.6/LICENSE
--rw-r--r--   0        0        0        0 2023-11-08 15:53:56.215514 pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/__init__.py
--rw-r--r--   0        0        0     1564 2024-01-11 14:59:29.299558 pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/pydantic_first.py
--rw-r--r--   0        0        0     4045 2023-11-10 11:17:42.655967 pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/read_write.py
--rw-r--r--   0        0        0    12602 2024-03-18 13:18:32.289776 pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/sql_first.py
--rw-r--r--   0        0        0     4531 2023-11-09 12:58:06.620578 pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/utils.py
--rw-r--r--   0        0        0      785 2024-03-18 13:19:50.103551 pydantic_sql_bridge-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7978 2024-01-11 16:21:00.878365 pydantic_sql_bridge-0.0.6/README.md
--rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 pydantic_sql_bridge-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-10-24 11:21:28.890406 pydantic_sql_bridge-0.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-11-08 15:53:56.215514 pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/__init__.py
+-rw-r--r--   0        0        0     1564 2024-01-11 14:59:29.299558 pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/pydantic_first.py
+-rw-r--r--   0        0        0     4045 2023-11-10 11:17:42.655967 pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/read_write.py
+-rw-r--r--   0        0        0    12602 2024-03-18 13:18:32.289776 pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/sql_first.py
+-rw-r--r--   0        0        0     4531 2023-11-09 12:58:06.620578 pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/utils.py
+-rw-r--r--   0        0        0      785 2024-04-18 09:26:25.291364 pydantic_sql_bridge-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7978 2024-01-11 16:21:00.878365 pydantic_sql_bridge-0.0.7/README.md
+-rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 pydantic_sql_bridge-0.0.7/PKG-INFO
```

### Comparing `pydantic_sql_bridge-0.0.6/LICENSE` & `pydantic_sql_bridge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/pydantic_first.py` & `pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/pydantic_first.py`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/read_write.py` & `pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/read_write.py`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/sql_first.py` & `pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/sql_first.py`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/pydantic_sql_bridge/utils.py` & `pydantic_sql_bridge-0.0.7/pydantic_sql_bridge/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/pyproject.toml` & `pydantic_sql_bridge-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pydantic-sql-bridge"
-version = "0.0.6"
+version = "0.0.7"
 description = "A simple bridge between SQL databases and Pydantic"
 authors = ["Rik <rik.de.kort@hey.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_sql_bridge"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.*"
 sqlglot = "^19.1"
-pggm-datalab-utils = "^2.10"
+pggm-datalab-utils = "^2.11"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23"
 
 [[tool.poetry.source]]
 name = "ptho"
```

### Comparing `pydantic_sql_bridge-0.0.6/README.md` & `pydantic_sql_bridge-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_sql_bridge-0.0.6/PKG-INFO` & `pydantic_sql_bridge-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pydantic-sql-bridge
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple bridge between SQL databases and Pydantic
 License: MIT
 Author: Rik
 Author-email: rik.de.kort@hey.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pggm-datalab-utils (>=2.10,<3.0)
+Requires-Dist: pggm-datalab-utils (>=2.11,<3.0)
 Requires-Dist: pydantic (==2.*)
 Requires-Dist: sqlglot (>=19.1,<20.0)
 Description-Content-Type: text/markdown
 
 # Pydantic SQL Bridge 🌉
 
 SQL and Pydantic models, simplified. Get the benefits of developing with Pydantic while harnessing all the power your
```

