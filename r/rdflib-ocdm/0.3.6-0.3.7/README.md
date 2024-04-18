# Comparing `tmp/rdflib_ocdm-0.3.6.tar.gz` & `tmp/rdflib_ocdm-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdflib_ocdm-0.3.6.tar", max compression
+gzip compressed data, was "rdflib_ocdm-0.3.7.tar", max compression
```

## Comparing `rdflib_ocdm-0.3.6.tar` & `rdflib_ocdm-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      515 2023-09-10 17:29:02.695640 rdflib_ocdm-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      840 2023-06-10 14:49:29.039605 rdflib_ocdm-0.3.6/rdflib_ocdm/__init__.py
--rw-r--r--   0        0        0     6176 2023-06-10 14:49:29.040616 rdflib_ocdm-0.3.6/rdflib_ocdm/abstract_entity.py
--rw-r--r--   0        0        0      839 2023-06-10 14:49:29.042607 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     2444 2023-06-10 14:49:29.043617 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0     5348 2023-06-10 14:49:29.044751 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0     3119 2023-06-10 14:49:29.045767 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     2144 2023-06-10 14:58:08.663200 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/redis_counter_handler.py
--rw-r--r--   0        0        0     3554 2023-09-09 20:17:16.731982 rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     4869 2023-09-10 17:28:15.351714 rdflib_ocdm-0.3.6/rdflib_ocdm/ocdm_graph.py
--rw-r--r--   0        0        0      839 2023-06-10 14:49:29.050418 rdflib_ocdm-0.3.6/rdflib_ocdm/prov/__init__.py
--rw-r--r--   0        0        0     2948 2023-09-09 20:16:44.998894 rdflib_ocdm-0.3.6/rdflib_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0     8507 2023-09-10 17:28:46.732045 rdflib_ocdm-0.3.6/rdflib_ocdm/prov/provenance.py
--rw-r--r--   0        0        0    13514 2023-06-10 14:49:29.053989 rdflib_ocdm-0.3.6/rdflib_ocdm/prov/snapshot_entity.py
--rw-r--r--   0        0        0     4448 2023-09-09 20:16:52.411791 rdflib_ocdm-0.3.6/rdflib_ocdm/query_utils.py
--rw-r--r--   0        0        0     2259 2023-06-10 14:49:29.055534 rdflib_ocdm-0.3.6/rdflib_ocdm/reader.py
--rw-r--r--   0        0        0     8993 2023-09-09 20:16:57.159094 rdflib_ocdm-0.3.6/rdflib_ocdm/storer.py
--rw-r--r--   0        0        0     2570 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.6/rdflib_ocdm/support.py
--rw-r--r--   0        0        0      600 2023-06-10 14:49:29.035949 rdflib_ocdm-0.3.6/README.md
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.6/setup.py
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      513 2024-04-18 12:41:20.727127 rdflib_ocdm-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      840 2023-06-10 14:49:29.039605 rdflib_ocdm-0.3.7/rdflib_ocdm/__init__.py
+-rw-r--r--   0        0        0     6176 2023-06-10 14:49:29.040616 rdflib_ocdm-0.3.7/rdflib_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0      839 2023-06-10 14:49:29.042607 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-10 14:49:29.043617 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0     5348 2023-06-10 14:49:29.044751 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0     3119 2023-06-10 14:49:29.045767 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     2144 2023-06-10 14:58:08.663200 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/redis_counter_handler.py
+-rw-r--r--   0        0        0     3554 2023-09-09 20:17:16.731982 rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     4869 2023-09-10 17:28:15.351714 rdflib_ocdm-0.3.7/rdflib_ocdm/ocdm_graph.py
+-rw-r--r--   0        0        0      839 2023-06-10 14:49:29.050418 rdflib_ocdm-0.3.7/rdflib_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0     2948 2023-09-09 20:16:44.998894 rdflib_ocdm-0.3.7/rdflib_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0     8507 2023-09-10 17:28:46.732045 rdflib_ocdm-0.3.7/rdflib_ocdm/prov/provenance.py
+-rw-r--r--   0        0        0    13514 2023-06-10 14:49:29.053989 rdflib_ocdm-0.3.7/rdflib_ocdm/prov/snapshot_entity.py
+-rw-r--r--   0        0        0     4448 2023-09-09 20:16:52.411791 rdflib_ocdm-0.3.7/rdflib_ocdm/query_utils.py
+-rw-r--r--   0        0        0     2259 2023-06-10 14:49:29.055534 rdflib_ocdm-0.3.7/rdflib_ocdm/reader.py
+-rw-r--r--   0        0        0     8993 2023-09-09 20:16:57.159094 rdflib_ocdm-0.3.7/rdflib_ocdm/storer.py
+-rw-r--r--   0        0        0     2570 2023-06-10 14:49:29.057559 rdflib_ocdm-0.3.7/rdflib_ocdm/support.py
+-rw-r--r--   0        0        0      600 2023-06-10 14:49:29.035949 rdflib_ocdm-0.3.7/README.md
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 rdflib_ocdm-0.3.7/PKG-INFO
```

### Comparing `rdflib_ocdm-0.3.6/pyproject.toml` & `rdflib_ocdm-0.3.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rdflib-ocdm"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["arcangelo7 <arcangelomas@gmail.com>"]
 license = "ISC"
 readme = "README.md"
 packages = [{include = "rdflib_ocdm"}]
 
 [tool.poetry.dependencies]
-python = "^3.7.4"
+python = "^3.8"
 rdflib = "^6.2.0"
-oc-ocdm = "^7.1.7"
+oc-ocdm = "^8.0.2"
 sparqlwrapper = "^2.0.0"
 redis = "^4.5.5"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.3"
 coverage-badge = "^1.1.0"
```

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/__init__.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/abstract_entity.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/__init__.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/counter_handler.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/filesystem_counter_handler.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/in_memory_counter_handler.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/redis_counter_handler.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/redis_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/counter_handler/sqlite_counter_handler.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/ocdm_graph.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/ocdm_graph.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/prov/__init__.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/prov/prov_entity.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/prov/provenance.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/prov/provenance.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/prov/snapshot_entity.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/prov/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/query_utils.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/query_utils.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/reader.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/storer.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/rdflib_ocdm/support.py` & `rdflib_ocdm-0.3.7/rdflib_ocdm/support.py`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/README.md` & `rdflib_ocdm-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_ocdm-0.3.6/PKG-INFO` & `rdflib_ocdm-0.3.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rdflib-ocdm
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
-Requires-Python: >=3.7.4,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: oc-ocdm (>=7.1.7,<8.0.0)
+Requires-Dist: oc-ocdm (>=8.0.2,<9.0.0)
 Requires-Dist: rdflib (>=6.2.0,<7.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
 Requires-Dist: sparqlwrapper (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 [<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
 [![Run tests](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/rdflib-ocdm/actions/workflows/run_tests.yml)
```

