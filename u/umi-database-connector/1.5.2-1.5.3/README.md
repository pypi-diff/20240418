# Comparing `tmp/umi-database-connector-1.5.2.tar.gz` & `tmp/umi-database-connector-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umi-database-connector-1.5.2.tar", last modified: Wed Mar 13 10:38:15 2024, max compression
+gzip compressed data, was "/home/runner/work/umi-database-connector/umi-database-connector/dist/.tmp-_34z_mxa/umi-database-connector-1.5.3.tar", last modified: Thu Apr 18 15:48:28 2024, max compression
```

## Comparing `umi-database-connector-1.5.2.tar` & `umi-database-connector-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-13 10:38:03.000000 umi-database-connector-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-13 10:38:03.000000 umi-database-connector-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-13 10:38:03.000000 umi-database-connector-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/src/umi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/src/umi/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:03.000000 umi-database-connector-1.5.2/src/umi/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-03-13 10:38:03.000000 umi-database-connector-1.5.2/src/umi/database/database_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:38:15.983945 umi-database-connector-1.5.2/src/umi_database_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-13 10:38:15.000000 umi-database-connector-1.5.2/src/umi_database_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-13 10:38:15.000000 umi-database-connector-1.5.2/src/umi_database_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:38:15.000000 umi-database-connector-1.5.2/src/umi_database_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-13 10:38:15.000000 umi-database-connector-1.5.2/src/umi_database_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 15:48:16.000000 umi-database-connector-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-18 15:48:16.000000 umi-database-connector-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 15:48:16.000000 umi-database-connector-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:16.000000 umi-database-connector-1.5.3/src/umi/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-04-18 15:48:16.000000 umi-database-connector-1.5.3/src/umi/database/database_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi_database_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi_database_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi_database_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi_database_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 15:48:28.000000 umi-database-connector-1.5.3/src/umi_database_connector.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `umi-database-connector-1.5.2/LICENSE` & `umi-database-connector-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `umi-database-connector-1.5.2/PKG-INFO` & `umi-database-connector-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: umi-database-connector
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python wrapper for our python services
 Author-email: Juan David Cruz Gomez <jdcruz-gomez@umi-innovation.com>, Iaphane Mekki-Felix <imfelix@umi.us>
 Project-URL: Homepage, https://github.com/unitedmotionideas/umi-database-connector
 Project-URL: Issues, https://github.com/unitedmotionideas/umi-database-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UMI database connector
 This is a python wrapper for streamlining the querying process for our python services. The idea of this package is for NLP service
 to use different MongoDB databases on one cluster.
```

### Comparing `umi-database-connector-1.5.2/README.md` & `umi-database-connector-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `umi-database-connector-1.5.2/pyproject.toml` & `umi-database-connector-1.5.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "umi-database-connector"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
   { name="Juan David Cruz Gomez", email="jdcruz-gomez@umi-innovation.com" },
   { name="Iaphane Mekki-Felix", email="imfelix@umi.us" },
 ]
 description = "A python wrapper for our python services"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `umi-database-connector-1.5.2/src/umi/database/database_connector.py` & `umi-database-connector-1.5.3/src/umi/database/database_connector.py`

 * *Files identical despite different names*

### Comparing `umi-database-connector-1.5.2/src/umi_database_connector.egg-info/PKG-INFO` & `umi-database-connector-1.5.3/src/umi_database_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: umi-database-connector
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python wrapper for our python services
 Author-email: Juan David Cruz Gomez <jdcruz-gomez@umi-innovation.com>, Iaphane Mekki-Felix <imfelix@umi.us>
 Project-URL: Homepage, https://github.com/unitedmotionideas/umi-database-connector
 Project-URL: Issues, https://github.com/unitedmotionideas/umi-database-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UMI database connector
 This is a python wrapper for streamlining the querying process for our python services. The idea of this package is for NLP service
 to use different MongoDB databases on one cluster.
```

