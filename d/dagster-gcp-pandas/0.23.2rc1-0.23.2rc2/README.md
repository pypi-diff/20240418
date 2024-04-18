# Comparing `tmp/dagster-gcp-pandas-0.23.2rc1.tar.gz` & `tmp/dagster-gcp-pandas-0.23.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-gcp-pandas-0.23.2rc1.tar", last modified: Tue Apr 16 17:56:40 2024, max compression
+gzip compressed data, was "dagster-gcp-pandas-0.23.2rc2.tar", last modified: Tue Apr 16 20:39:16 2024, max compression
```

## Comparing `dagster-gcp-pandas-0.23.2rc1.tar` & `dagster-gcp-pandas-0.23.2rc2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:56:40.455847 dagster-gcp-pandas-0.23.2rc1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-16 17:56:40.455847 dagster-gcp-pandas-0.23.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:56:40.455847 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:56:40.455847 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10894 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:56:40.455847 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      487 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-16 17:56:40.000000 dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      165 2024-04-16 17:56:40.459847 dagster-gcp-pandas-0.23.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1454 2024-04-16 17:50:34.000000 dagster-gcp-pandas-0.23.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:16.404433 dagster-gcp-pandas-0.23.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-16 20:39:16.404433 dagster-gcp-pandas-0.23.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:16.404433 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:16.404433 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10894 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:39:16.404433 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      487 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-16 20:39:16.000000 dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2024-04-16 20:39:16.408433 dagster-gcp-pandas-0.23.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-04-16 20:26:55.000000 dagster-gcp-pandas-0.23.2rc2/setup.py
```

### Comparing `dagster-gcp-pandas-0.23.2rc1/LICENSE` & `dagster-gcp-pandas-0.23.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.23.2rc1/PKG-INFO` & `dagster-gcp-pandas-0.23.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py` & `dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas/bigquery/bigquery_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-gcp-pandas-0.23.2rc1/dagster_gcp_pandas.egg-info/PKG-INFO` & `dagster-gcp-pandas-0.23.2rc2/dagster_gcp_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pandas
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for storing Pandas DataFrames in GCP.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-gcp-pandas-0.23.2rc1/setup.py` & `dagster-gcp-pandas-0.23.2rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc1",
-        "dagster-gcp==0.23.2rc1",
+        "dagster==1.7.2rc2",
+        "dagster-gcp==0.23.2rc2",
         "pandas",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

