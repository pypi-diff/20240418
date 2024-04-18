# Comparing `tmp/dagster-embedded-elt-0.23.2rc1.tar.gz` & `tmp/dagster-embedded-elt-0.23.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.2rc1.tar", last modified: Tue Apr 16 17:58:50 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.2rc2.tar", last modified: Tue Apr 16 20:38:47 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.2rc1.tar` & `dagster-embedded-elt-0.23.2rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.964118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3681 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7024 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17560 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.964118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-16 17:58:50.972118 dagster-embedded-elt-0.23.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1430 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:46.992371 dagster-embedded-elt-0.23.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 20:38:46.992371 dagster-embedded-elt-0.23.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:46.984371 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:46.988371 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:46.992371 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17560 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:46.984371 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 20:38:46.000000 dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-16 20:38:46.996371 dagster-embedded-elt-0.23.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1430 2024-04-16 20:26:55.000000 dagster-embedded-elt-0.23.2rc2/setup.py
```

### Comparing `dagster-embedded-elt-0.23.2rc1/LICENSE` & `dagster-embedded-elt-0.23.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/PKG-INFO` & `dagster-embedded-elt-0.23.2rc2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.2rc1
+Version: 0.23.2rc2
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.2rc2/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc1/setup.py` & `dagster-embedded-elt-0.23.2rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc1", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.2rc2", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

