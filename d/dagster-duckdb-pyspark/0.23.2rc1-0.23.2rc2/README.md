# Comparing `tmp/dagster-duckdb-pyspark-0.23.2rc1.tar.gz` & `tmp/dagster-duckdb-pyspark-0.23.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.23.2rc1.tar", last modified: Tue Apr 16 17:58:36 2024, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.23.2rc2.tar", last modified: Tue Apr 16 20:39:20 2024, max compression
```

## Comparing `dagster-duckdb-pyspark-0.23.2rc1.tar` & `dagster-duckdb-pyspark-0.23.2rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:36.212087 dagster-duckdb-pyspark-0.23.2rc1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      626 2024-04-16 17:58:36.212087 dagster-duckdb-pyspark-0.23.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:36.208087 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9588 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:36.212087 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      626 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 17:58:36.000000 dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2024-04-16 17:58:36.212087 dagster-duckdb-pyspark-0.23.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2024-04-16 17:50:34.000000 dagster-duckdb-pyspark-0.23.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:20.844442 dagster-duckdb-pyspark-0.23.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      626 2024-04-16 20:39:20.844442 dagster-duckdb-pyspark-0.23.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:20.840442 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:20.844442 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 20:39:20.000000 dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-16 20:39:20.844442 dagster-duckdb-pyspark-0.23.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1510 2024-04-16 20:26:55.000000 dagster-duckdb-pyspark-0.23.2rc2/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.23.2rc1/LICENSE` & `dagster-duckdb-pyspark-0.23.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.23.2rc1/PKG-INFO` & `dagster-duckdb-pyspark-0.23.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.23.2rc1/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.23.2rc2/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.23.2rc1/setup.py` & `dagster-duckdb-pyspark-0.23.2rc2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc1",
-        "dagster-duckdb==0.23.2rc1",
+        "dagster==1.7.2rc2",
+        "dagster-duckdb==0.23.2rc2",
         "pyspark>=3",
         # Pinned pending duckdb removal of broken pandas import. Pin can be
         # removed as soon as it produces a working build.
         "pandas<2.1",
         "pyarrow",
     ],
     zip_safe=False,
```
