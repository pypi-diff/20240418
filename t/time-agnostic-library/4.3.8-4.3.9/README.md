# Comparing `tmp/time_agnostic_library-4.3.8.tar.gz` & `tmp/time_agnostic_library-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_agnostic_library-4.3.8.tar", max compression
+gzip compressed data, was "time_agnostic_library-4.3.9.tar", max compression
```

## Comparing `time_agnostic_library-4.3.8.tar` & `time_agnostic_library-4.3.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      786 2023-06-20 12:43:34.241515 time_agnostic_library-4.3.8/LICENSE.md
--rw-r--r--   0        0        0     1638 2023-09-26 13:37:51.247970 time_agnostic_library-4.3.8/pyproject.toml
--rw-r--r--   0        0        0    18918 2023-06-20 12:43:34.245516 time_agnostic_library-4.3.8/README.md
--rw-r--r--   0        0        0      831 2023-06-20 12:43:12.793829 time_agnostic_library-4.3.8/src/time_agnostic_library/__init__.py
--rw-r--r--   0        0        0    21850 2023-09-26 13:37:38.272054 time_agnostic_library-4.3.8/src/time_agnostic_library/agnostic_entity.py
--rw-r--r--   0        0        0    43077 2023-09-11 12:32:21.441261 time_agnostic_library-4.3.8/src/time_agnostic_library/agnostic_query.py
--rw-r--r--   0        0        0     2430 2023-06-20 12:43:12.828518 time_agnostic_library-4.3.8/src/time_agnostic_library/prov_entity.py
--rw-r--r--   0        0        0     9881 2023-09-11 12:18:46.493179 time_agnostic_library-4.3.8/src/time_agnostic_library/sparql.py
--rw-r--r--   0        0        0     1830 2023-06-20 12:43:12.848466 time_agnostic_library-4.3.8/src/time_agnostic_library/statistics.py
--rw-r--r--   0        0        0     8299 2023-09-03 13:52:12.654732 time_agnostic_library-4.3.8/src/time_agnostic_library/support.py
--rw-r--r--   0        0        0    20582 1970-01-01 00:00:00.000000 time_agnostic_library-4.3.8/setup.py
--rw-r--r--   0        0        0    20572 1970-01-01 00:00:00.000000 time_agnostic_library-4.3.8/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-06-20 12:43:34.241515 time_agnostic_library-4.3.9/LICENSE.md
+-rw-r--r--   0        0        0     1638 2023-10-05 13:52:01.642933 time_agnostic_library-4.3.9/pyproject.toml
+-rw-r--r--   0        0        0    18918 2023-06-20 12:43:34.245516 time_agnostic_library-4.3.9/README.md
+-rw-r--r--   0        0        0      831 2023-06-20 12:43:12.793829 time_agnostic_library-4.3.9/src/time_agnostic_library/__init__.py
+-rw-r--r--   0        0        0    21850 2023-10-05 13:51:07.795956 time_agnostic_library-4.3.9/src/time_agnostic_library/agnostic_entity.py
+-rw-r--r--   0        0        0    43077 2023-09-11 12:32:21.441261 time_agnostic_library-4.3.9/src/time_agnostic_library/agnostic_query.py
+-rw-r--r--   0        0        0     2430 2023-06-20 12:43:12.828518 time_agnostic_library-4.3.9/src/time_agnostic_library/prov_entity.py
+-rw-r--r--   0        0        0    10102 2023-10-05 13:51:34.716778 time_agnostic_library-4.3.9/src/time_agnostic_library/sparql.py
+-rw-r--r--   0        0        0     1830 2023-06-20 12:43:12.848466 time_agnostic_library-4.3.9/src/time_agnostic_library/statistics.py
+-rw-r--r--   0        0        0     8299 2023-09-03 13:52:12.654732 time_agnostic_library-4.3.9/src/time_agnostic_library/support.py
+-rw-r--r--   0        0        0    20524 1970-01-01 00:00:00.000000 time_agnostic_library-4.3.9/PKG-INFO
```

### Comparing `time_agnostic_library-4.3.8/LICENSE.md` & `time_agnostic_library-4.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/pyproject.toml` & `time_agnostic_library-4.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "time-agnostic-library"
-version = "4.3.8"
+version = "4.3.9"
 description = "time-agnostic-library is a Python ≥3.7 library that allows performing time-travel queries on RDF datasets compliant with the OCDM v2.0.1 provenance specification."
 authors = ["Arcangelo Massari <arcangelo.massari@unibo.it>"]
 readme = "README.md"
 license = "ISC"
 homepage = "https://github.com/opencitations/time-agnostic-library"
 repository = "https://github.com/opencitations/time-agnostic-library"
 documentation = "https://time-agnostic-library.readthedocs.io"
```

### Comparing `time_agnostic_library-4.3.8/README.md` & `time_agnostic_library-4.3.9/README.md`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/__init__.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/__init__.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/agnostic_entity.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/agnostic_entity.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/agnostic_query.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/agnostic_query.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/prov_entity.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/prov_entity.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/sparql.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/sparql.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,18 @@
                 results = sparql.queryAndConvert()
                 for quad in results["results"]["bindings"]:
                     quad_to_add = list()
                     for var in results["head"]["vars"]:
                         if quad[var]["type"] == "uri":
                             quad_to_add.append(URIRef(quad[var]["value"]))
                         elif quad[var]["type"] == "literal":
-                            quad_to_add.append(Literal(quad[var]["value"]))
+                            if 'datatype' in quad[var]:
+                                quad_to_add.append(Literal(quad[var]["value"], datatype=quad[var]['datatype']))
+                            else:
+                                quad_to_add.append(Literal(quad[var]["value"], datatype=XSD.string))
                     cg.add(tuple(quad_to_add))
             elif algebra.name == "ConstructQuery":
                 sparql.setReturnFormat(RDFXML)
                 sparql.setOnlyConneg(True)
                 cg += sparql.queryAndConvert()            
         return cg        
     
@@ -212,9 +215,8 @@
     def _cut_by_limit(self, input):
         lock.acquire()
         algebra:CompValue = prepareQuery(self.query).algebra
         lock.release()
         if "length" in algebra["p"]:
             limit = int(algebra["p"]["length"])
             input = input[:limit]
-        return input
-    
+        return input
```

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/statistics.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/statistics.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/src/time_agnostic_library/support.py` & `time_agnostic_library-4.3.9/src/time_agnostic_library/support.py`

 * *Files identical despite different names*

### Comparing `time_agnostic_library-4.3.8/setup.py` & `time_agnostic_library-4.3.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,448 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: time-agnostic-library
+Version: 4.3.9
+Summary: time-agnostic-library is a Python ≥3.7 library that allows performing time-travel queries on RDF datasets compliant with the OCDM v2.0.1 provenance specification.
+Home-page: https://github.com/opencitations/time-agnostic-library
+License: ISC
+Keywords: rdf,provenance,opencitations,change-tracking,time-traversal query
+Author: Arcangelo Massari
+Author-email: arcangelo.massari@unibo.it
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: SPARQLWrapper (==2.0.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: python_dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: rdflib (==6.3.2)
+Requires-Dist: rdflib-ocdm (==0.3.6)
+Requires-Dist: setuptools (>=68.2.2,<69.0.0)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Project-URL: Documentation, https://time-agnostic-library.readthedocs.io
+Project-URL: Repository, https://github.com/opencitations/time-agnostic-library
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)
+[![run_tests](https://github.com/opencitations/time-agnostic-library/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/time-agnostic-library/actions/workflows/run_tests.yml)
+![Coverage](https://raw.githubusercontent.com/opencitations/time-agnostic-library/main/tests/coverage/coverage.svg)
+![PyPI](https://img.shields.io/pypi/pyversions/time-agnostic-library)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/time-agnostic-library)
 
-packages = \
-['time_agnostic_library']
+# time-agnostic-library
+
+**time-agnostic-library** is a Python &ge;3.7 library that allows performing time-travel queries on RDF datasets compliant with the [OCDM v2.0.1](https://figshare.com/articles/Metadata_for_the_OpenCitations_Corpus/3443876) provenance specification.
+
+The package was tested on **Blazegraph**, **GraphDB**, **Apache Jena Fuseki**, and **OpenLink Virtuoso**, and it is fully compatible with these triplestores. 
+
+Documentation can be found here: [https://time-agnostic-library.readthedocs.io](https://time-agnostic-library.readthedocs.io).
+
+## Table of Contents
+
+- [User's guide](#users-guide)
+  * [Version materialization](#version-materialization)
+  * [Single-version structured query](#single-version-structured-query)
+  * [Cross-version structured query](#cross-version-structured-query)
+  * [Single-delta structured query](#single-delta-structured-query)
+  * [Cross-delta structured query](#cross-delta-structured-query)
+  * [Configuration file](#configuration-file)
+- [Developer's guide](#developers-guide)
+  * [First steps](#first-steps)
+  * [How to run the tests](#how-to-run-the-tests)
+  * [How to build the documentation](#how-to-build-the-documentation)
+  * [How to benchmark](#how-to-benchmark)
+
+## User's guide
+
+This package can be installed with **pip**:
+
+``` bash
+  pip install time-agnostic-library
+```
+
+The library allows five types of queries: versions materializations, single-version structured queries, cross-version structured queries, single-delta structured queries and cross-delta structured queries.
+
+### Version materialization
+
+Obtaining a version materialization means returning an entity version at a given time. Time can be an interval, an instant, a before or an after.
+
+To do so, create an instance of the **AgnosticEntity** class, passing as an argument the entity URI (RES_URI) and the configuration file path (CONFIG_PATH). For more information about the configuration file, see [Configuration file](#configuration-file). Finally, run the **get_state_at_time method**, passing the time of interest as an argument and, if provenance metadata are needed, True to the **include_prov_metadata** field. 
+
+The specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.
+
+``` python
+  agnostic_entity = AgnosticEntity(res=RES_URI, config_path=CONFIG_PATH)
+  agnostic_entity.get_state_at_time(time=(START, END), include_prov_metadata=True)
+```
+
+The output is always a tuple of three elements: the first is a dictionary that associates graphs and timestamps within the specified interval; the second contains the snapshots metadata of which the states has been returned, the third is a dictionary including the other snapshots' provenance metadata if **include_prov_metadata** is True, None if False.
+
+``` python
+  (
+      {
+          TIME_1: ENTITY_GRAPH_AT_TIME_1, 
+          TIME_2: ENTITY_GRAPH_AT_TIME_2
+      },
+      {
+          SNAPSHOT_URI_AT_TIME_1: {
+              'generatedAtTime': TIME_1, 
+              'wasAttributedTo': ATTRIBUTION, 
+              'hadPrimarySource': PRIMARY_SOURCE
+          },
+          SNAPSHOT_URI_AT_TIME_2: {
+              'generatedAtTime': TIME_2, 
+              'wasAttributedTo': ATTRIBUTION, 
+              'hadPrimarySource': PRIMARY_SOURCE
+          }
+      }, 
+      {
+          OTHER_SNAPSHOT_URI_1: {
+              'generatedAtTime': GENERATION_TIME, 
+              'wasAttributedTo': ATTRIBUTION, 
+              'hadPrimarySource': PRIMARY_SOURCE
+          }, 
+          OTHER_SNAPSHOT_URI_2: {
+              'generatedAtTime': GENERATION_TIME, 
+              'wasAttributedTo': ATTRIBUTION, 
+              'hadPrimarySource': PRIMARY_SOURCE
+          }
+      }
+  )
+```
+
+On the other hand, if the whole entity's history is required, use the **get_history** method.
+
+``` python
+  agnostic_entity = AgnosticEntity(res=RES_URI, config_path=CONFIG_PATH)
+  agnostic_entity.get_history(include_prov_metadata=True)
+```
+
+In this case, the output is always a two-element tuple. The first is a dictionary containing all the versions of a given resource. The second is a dictionary containing all the provenance metadata linked to that resource if **include_prov_metadata** is True, None if False.
+
+``` python
+  (
+    {
+       RES_URI: {
+            TIME_1: ENTITY_GRAPH_AT_TIME_1, 
+            TIME_2: ENTITY_GRAPH_AT_TIME_2
+        }
+    },
+    {
+      RES_URI: {
+        SNAPSHOT_URI_AT_TIME_1': {
+            'generatedAtTime': GENERATION_TIME, 
+            'wasAttributedTo': ATTRIBUTION, 
+            'hadPrimarySource': PRIMARY_SOURCE
+        }, 
+        SNAPSHOT_URI_AT_TIME_2: {
+            'generatedAtTime': GENERATION_TIME, 
+            'wasAttributedTo': ATTRIBUTION, 
+            'hadPrimarySource': PRIMARY_SOURCE
+        }
+    } 
+  )
+```
+
+Finally, the history of an entity and all related entities, along with their provenance metadata, can be obtained by switching to True the **related_entities_history** argument.
+
+``` python
+  agnostic_entity = AgnosticEntity(res=RES_URI, related_entities_history=True, config_path=CONFIG_PATH)
+  agnostic_entity.get_history(include_prov_metadata=True)
+```
+
+### Single-version structured query
+
+Performing a single-version structured query means running a SPARQL query on a specified version. A version can be a time interval, an instant, a before or an after.
+
+To obtain this result, instantiate the **VersionQuery** class, passing as an argument the SPARQL query string (QUERY_STRING), the time of interest and the configuration file's path (CONFIG_PATH). Finally, execute the **run_agnostic_query** method.
+
+The specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.
+
+For more information about the configuration file, see [Configuration file](#configuration-file). 
+
+**Please note**: only SELECT queries are allowed. 
+
+``` python
+  agnostic_query = VersionQuery(query=QUERY_STRING, on_time=(START, END), config_path=CONFIG_PATH)
+  agnostic_query.run_agnostic_query()
+```
+
+The output is a dictionary in which the keys are the snapshots relevant to that query. The values correspond to sets of tuples containing the query results at the time specified by the key. The positional value of the elements in the tuples is equivalent to the variables indicated in the query.
+
+``` python
+  {
+    TIME: {
+      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),
+      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),
+      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)
+    }
+  }
+```
+
+### Cross-version structured query
+
+Performing a cross-version structured query means running a SPARQL query on all the dataset's versions.
+
+To obtain this result, instantiate the **VersionQuery** class, passing as an argument the SPARQL query string (QUERY_STRING) and the configuration file's path (CONFIG_PATH). Finally, execute **the run_agnostic_query** method.
+
+For more information about the configuration file, see [Configuration file](#configuration-file). 
+
+**Please note**: only SELECT queries are allowed. 
+
+``` python
+  agnostic_query = VersionQuery(query=QUERY_STRING, config_path=CONFIG_PATH)
+  agnostic_query.run_agnostic_query()
+```
+
+The output is a dictionary in which the keys are the snapshots relevant to that query. The values correspond to sets of tuples containing the query results at the time specified by the key. The positional value of the elements in the tuples is equivalent to the variables indicated in the query.
+
+``` python
+  {
+    TIME_1: {
+      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),
+      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),
+      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)
+    },
+    TIME_2: {
+      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),
+      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),
+      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)
+    },
+    TIME_N: {
+      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),
+      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),
+      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)
+    }
+  }
+```
+
+### Single-delta structured query
+
+Performing a single-delta query means that a structured queries must be satisfied on a specific change instance of the dataset. This information demand particularly focuses on the differences between two versions, which are typically but not always consecutive.
+
+To obtain this result, instantiate the **DeltaQuery** class, passing as an argument the SPARQL query string, the time of interest, a set of properties, and the configuration file's path. Finally, execute the **run_agnostic_query** method.
+
+The query string (QUERY_STRING) is useful to identify the entities whose change you want to investigate.
+
+The specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.
+
+The set of properties (PROPERTIES_SET) narrows the field to those entities where the properties specified in the set have changed. If no property was indicated, any changes are considered.
+
+For more information about the configuration file (CONFIG_PATH), see [Configuration file](#configuration-file). 
+
+**Please note**: only SELECT queries are allowed. 
+
+``` python
+  agnostic_entity = DeltaQuery(query=QUERY_STRING, on_time=(START, END), changed_properties=PROPERTIES_SET, config_path=CONFIG_PATH)
+  agnostic_entity.run_agnostic_query()
+```
+
+The output is a dictionary that reports the modified entities, when they were created, modified, and deleted. Moreover, changes are reported as SPARQL UPDATE queries.
+
+``` python
+  {
+      RES_URI_1: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },
+      RES_URI_2: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },
+      RES_URI_N: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },		
+  }    
+```
+
+### Cross-delta structured query
+
+Performing a cross-delta query means that a structured queries must be satisfied across the differences of the dataset, thus allowing for fully fledged evolution studies.
+
+To obtain this result, instantiate the **DeltaQuery** class, passing as an argument the SPARQL query string, a set of properties, and the configuration file's path. Finally, execute the **run_agnostic_query** method.
+
+The query string (QUERY_STRING) is useful to identify the entities whose change you want to investigate.
+
+The set of properties (PROPERTIES_SET) narrows the field to those entities where the properties specified in the set have changed. If no property was indicated, any changes are considered.
+
+For more information about the configuration file (CONFIG_PATH), see [Configuration file](#configuration-file). 
+
+**Please note**: only SELECT queries are allowed. 
+
+``` python
+  agnostic_entity = DeltaQuery(query=QUERY_STRING, changed_properties=PROPERTIES_SET, config_path=CONFIG_PATH)
+  agnostic_entity.run_agnostic_query()
+```
+
+The output is a dictionary that reports the modified entities, when they were created, modified, and deleted. Changes are reported as SPARQL UPDATE queries. If the entity was not created or deleted within the indicated range, the "created" or "deleted" value is None. On the other hand, if the entity does not exist within the input interval, the "modified" value is an empty dictionary.
+
+``` python
+  {
+      RES_URI_1: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },
+      RES_URI_2: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },
+      RES_URI_N: {
+          "created": TIMESTAMP_CREATION,
+          "modified": {
+              TIMESTAMP_1: UPDATE_QUERY_1,
+              TIMESTAMP_2: UPDATE_QUERY_2,
+              TIMESTAMP_N: UPDATE_QUERY_N
+          },
+          "deleted": TIMESTAMP_DELETION
+      },		
+  }    
+```
+
+### Configuration file
+
+The configuration file is mainly used to indicate to the library where to search for data and provenance. In addition, some optional values can be set to make executions faster and more efficient.
+
+- **dataset** (required)
+  - **triplestore_urls**: Specify a list of triplestore URLs containing data.  
+  - **file_paths**: Specify a list of paths of files containing data.   
+- **provenance** (required)
+  - **triplestore_urls**: Specify a list of triplestore URLs containing provenance metadata.    
+  - **file_paths** Specify a list of paths of files containing provenance metadata.      
+- **blazegraph_full_text_search**, **fuseki_full_text_search**, **virtuoso_full_text_search** (optional): Specify an affirmative Boolean value if Blazegraph, Fuseki or Virtuoso was used as a triplestore, and a textual index was built to speed up queries. The allowed values are "true", "1", 1, "t", "y", "yes", "ok", or "false", "0", 0, "n", "f", "no".
+- **graphdb_connector_name** (optional): Specify the name of the Lucene connector if GraphDB was used as a triplestore and a textual index was built to speed up queries. For more information, see [https://graphdb.ontotext.com/documentation/free/general-full-text-search-with-connectors.html](https://graphdb.ontotext.com/documentation/free/general-full-text-search-with-connectors.html).
+- **cache_triplestore_url** (optional): Specifies the triplestore URL to use as a cache to make queries faster. If your triplestore uses different endpoints for reading and writing (e.g. GraphDB), specify the endpoint for reading in the "endpoint" field and the endpoint for writing in the "update_endpoint" field. If there is only one endpoint (e.g. Blazegraph), specify it in both fields.
+
+``` json
+  {
+      "dataset": {
+          "triplestore_urls": ["TRIPLESTORE_URL_1", "TRIPLESTORE_URL_2", "TRIPLESTORE_URL_N"],
+          "file_paths": ["PATH_1", "PATH_2", "PATH_N"]
+      },
+      "provenance": {
+          "triplestore_urls": ["TRIPLESTORE_URL_1", "TRIPLESTORE_URL_2", "TRIPLESTORE_URL_N"],
+          "file_paths": ["PATH_1", "PATH_2", "PATH_N"]
+      },
+      "blazegraph_full_text_search": "no",
+      "fuseki_full_text_search": "no",
+      "virtuoso_full_text_search": "no",
+      "graphdb_connector_name": "CONNECTOR_NAME",
+      "cache_triplestore_url": {
+        "endpoint": "READ_ENDPOINT",
+        "update_endpoint": "UPDATE_ENDPOINT"
+    }
+  }
+```
+
+## Developer's guide
+
+### First steps
+  1. Install Poetry:
+``` bash
+    pip install poetry
+```
+  2. Clone this repository:
+``` bash
+    git clone https://github.com/opencitations/time-agnostic-library
+    cd ./time-agnostic-library
+```
+  3. Install all the dependencies:
+``` bash
+    poetry install
+```
+  4. Build the package (_output dir:_ `dist`):
+``` bash
+    poetry build
+```
+  5. Globally install the package:
+``` bash
+    pip install ./dist/time-agnostic-library-<VERSION>.tar.gz
+```
+  6. If everything went the right way, than you should be able to use `time_agnostic_library` in your Python modules as follows:
+``` python
+    from time_agnostic_library.agnostic_entity import AgnosticEntity
+    from time_agnostic_library.agnostic_query import AgnosticQuery
+    # ...
+```
+
+### How to run the tests
+
+ 1. Make sure that Java is installed on your computer.
+ 2. Simply launch the following command from the root folder:
+
+``` bash
+  poetry run test
+```
+
+### How to build the documentation
+
+  1. Move inside the `docs` folder:
+``` bash
+  cd docs
+```
+  2. Use the Makefile provided to build the docs:
+      + _on Windows_
+        ```
+          ./make.bat html
+        ```
+      + _on Linux and MacOs_
+        ```
+          make html
+        ```
+  3. Open the `_build/html/index.html` file with a web browser of your choice!
+
+### How to benchmark
+
+Two benchmarks were designed, one on the execution times and the other on the RAM. Moreover, all benchmarks are performed on four different triplestores: Blazegraph, GraphDB Free Edition, Apache Jena Fuseki, and OpenLink Virtuoso.
+
+The dataset used for the benchmarks contains bibliographical information about scholarly works in the journal Scientometrics only if the DOI is known. The data was extracted via Crossref. It is a temporal dataset in which provenance information and change-tracking have been managed by adopting the OpenCitations Data Model. Moreover, the dataset contains information on all the cited academic works. Journals, bibliographic resources, and authors always appear unambiguously, without duplicates. Finally, heuristics have been applied to recover the DOI of the cited works in case Crossref did not provide such information.
+
+In order to run the benchmark, do the following steps:
+1. Download the dataset from [10.5281/zenodo.7105258](https://doi.org/10.5281/zenodo.7105258). 
+2. Extract `reproduce_results.zip`. 
+    + _on Windows_
+      
+      Execute `run_banchmarks.bat`
+    + _on Linux and MacOs_
+      
+      Execute `run_banchmarks.sh`
+3. As the results become available, they can be read by opening `json_to_table.html` via a local server.
+
+In the event that the execution should stop due to unforeseen causes, it will resume from where it was interrupted.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['SPARQLWrapper==2.0.0',
- 'psycopg2>=2.9.6,<3.0.0',
- 'python_dateutil>=2.8.2,<3.0.0',
- 'rdflib-ocdm==0.3.6',
- 'rdflib==6.3.2',
- 'setuptools>=68.2.2,<69.0.0',
- 'tqdm>=4.62.3,<5.0.0',
- 'validators>=0.20.0,<0.21.0']
-
-entry_points = \
-{'console_scripts': ['test = tests.run_all_tests:main']}
-
-setup_kwargs = {
-    'name': 'time-agnostic-library',
-    'version': '4.3.8',
-    'description': 'time-agnostic-library is a Python ≥3.7 library that allows performing time-travel queries on RDF datasets compliant with the OCDM v2.0.1 provenance specification.',
-    'long_description': '[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![run_tests](https://github.com/opencitations/time-agnostic-library/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/time-agnostic-library/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/time-agnostic-library/main/tests/coverage/coverage.svg)\n![PyPI](https://img.shields.io/pypi/pyversions/time-agnostic-library)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/opencitations/time-agnostic-library)\n\n# time-agnostic-library\n\n**time-agnostic-library** is a Python &ge;3.7 library that allows performing time-travel queries on RDF datasets compliant with the [OCDM v2.0.1](https://figshare.com/articles/Metadata_for_the_OpenCitations_Corpus/3443876) provenance specification.\n\nThe package was tested on **Blazegraph**, **GraphDB**, **Apache Jena Fuseki**, and **OpenLink Virtuoso**, and it is fully compatible with these triplestores. \n\nDocumentation can be found here: [https://time-agnostic-library.readthedocs.io](https://time-agnostic-library.readthedocs.io).\n\n## Table of Contents\n\n- [User\'s guide](#users-guide)\n  * [Version materialization](#version-materialization)\n  * [Single-version structured query](#single-version-structured-query)\n  * [Cross-version structured query](#cross-version-structured-query)\n  * [Single-delta structured query](#single-delta-structured-query)\n  * [Cross-delta structured query](#cross-delta-structured-query)\n  * [Configuration file](#configuration-file)\n- [Developer\'s guide](#developers-guide)\n  * [First steps](#first-steps)\n  * [How to run the tests](#how-to-run-the-tests)\n  * [How to build the documentation](#how-to-build-the-documentation)\n  * [How to benchmark](#how-to-benchmark)\n\n## User\'s guide\n\nThis package can be installed with **pip**:\n\n``` bash\n  pip install time-agnostic-library\n```\n\nThe library allows five types of queries: versions materializations, single-version structured queries, cross-version structured queries, single-delta structured queries and cross-delta structured queries.\n\n### Version materialization\n\nObtaining a version materialization means returning an entity version at a given time. Time can be an interval, an instant, a before or an after.\n\nTo do so, create an instance of the **AgnosticEntity** class, passing as an argument the entity URI (RES_URI) and the configuration file path (CONFIG_PATH). For more information about the configuration file, see [Configuration file](#configuration-file). Finally, run the **get_state_at_time method**, passing the time of interest as an argument and, if provenance metadata are needed, True to the **include_prov_metadata** field. \n\nThe specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.\n\n``` python\n  agnostic_entity = AgnosticEntity(res=RES_URI, config_path=CONFIG_PATH)\n  agnostic_entity.get_state_at_time(time=(START, END), include_prov_metadata=True)\n```\n\nThe output is always a tuple of three elements: the first is a dictionary that associates graphs and timestamps within the specified interval; the second contains the snapshots metadata of which the states has been returned, the third is a dictionary including the other snapshots\' provenance metadata if **include_prov_metadata** is True, None if False.\n\n``` python\n  (\n      {\n          TIME_1: ENTITY_GRAPH_AT_TIME_1, \n          TIME_2: ENTITY_GRAPH_AT_TIME_2\n      },\n      {\n          SNAPSHOT_URI_AT_TIME_1: {\n              \'generatedAtTime\': TIME_1, \n              \'wasAttributedTo\': ATTRIBUTION, \n              \'hadPrimarySource\': PRIMARY_SOURCE\n          },\n          SNAPSHOT_URI_AT_TIME_2: {\n              \'generatedAtTime\': TIME_2, \n              \'wasAttributedTo\': ATTRIBUTION, \n              \'hadPrimarySource\': PRIMARY_SOURCE\n          }\n      }, \n      {\n          OTHER_SNAPSHOT_URI_1: {\n              \'generatedAtTime\': GENERATION_TIME, \n              \'wasAttributedTo\': ATTRIBUTION, \n              \'hadPrimarySource\': PRIMARY_SOURCE\n          }, \n          OTHER_SNAPSHOT_URI_2: {\n              \'generatedAtTime\': GENERATION_TIME, \n              \'wasAttributedTo\': ATTRIBUTION, \n              \'hadPrimarySource\': PRIMARY_SOURCE\n          }\n      }\n  )\n```\n\nOn the other hand, if the whole entity\'s history is required, use the **get_history** method.\n\n``` python\n  agnostic_entity = AgnosticEntity(res=RES_URI, config_path=CONFIG_PATH)\n  agnostic_entity.get_history(include_prov_metadata=True)\n```\n\nIn this case, the output is always a two-element tuple. The first is a dictionary containing all the versions of a given resource. The second is a dictionary containing all the provenance metadata linked to that resource if **include_prov_metadata** is True, None if False.\n\n``` python\n  (\n    {\n       RES_URI: {\n            TIME_1: ENTITY_GRAPH_AT_TIME_1, \n            TIME_2: ENTITY_GRAPH_AT_TIME_2\n        }\n    },\n    {\n      RES_URI: {\n        SNAPSHOT_URI_AT_TIME_1\': {\n            \'generatedAtTime\': GENERATION_TIME, \n            \'wasAttributedTo\': ATTRIBUTION, \n            \'hadPrimarySource\': PRIMARY_SOURCE\n        }, \n        SNAPSHOT_URI_AT_TIME_2: {\n            \'generatedAtTime\': GENERATION_TIME, \n            \'wasAttributedTo\': ATTRIBUTION, \n            \'hadPrimarySource\': PRIMARY_SOURCE\n        }\n    } \n  )\n```\n\nFinally, the history of an entity and all related entities, along with their provenance metadata, can be obtained by switching to True the **related_entities_history** argument.\n\n``` python\n  agnostic_entity = AgnosticEntity(res=RES_URI, related_entities_history=True, config_path=CONFIG_PATH)\n  agnostic_entity.get_history(include_prov_metadata=True)\n```\n\n### Single-version structured query\n\nPerforming a single-version structured query means running a SPARQL query on a specified version. A version can be a time interval, an instant, a before or an after.\n\nTo obtain this result, instantiate the **VersionQuery** class, passing as an argument the SPARQL query string (QUERY_STRING), the time of interest and the configuration file\'s path (CONFIG_PATH). Finally, execute the **run_agnostic_query** method.\n\nThe specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.\n\nFor more information about the configuration file, see [Configuration file](#configuration-file). \n\n**Please note**: only SELECT queries are allowed. \n\n``` python\n  agnostic_query = VersionQuery(query=QUERY_STRING, on_time=(START, END), config_path=CONFIG_PATH)\n  agnostic_query.run_agnostic_query()\n```\n\nThe output is a dictionary in which the keys are the snapshots relevant to that query. The values correspond to sets of tuples containing the query results at the time specified by the key. The positional value of the elements in the tuples is equivalent to the variables indicated in the query.\n\n``` python\n  {\n    TIME: {\n      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),\n      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),\n      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)\n    }\n  }\n```\n\n### Cross-version structured query\n\nPerforming a cross-version structured query means running a SPARQL query on all the dataset\'s versions.\n\nTo obtain this result, instantiate the **VersionQuery** class, passing as an argument the SPARQL query string (QUERY_STRING) and the configuration file\'s path (CONFIG_PATH). Finally, execute **the run_agnostic_query** method.\n\nFor more information about the configuration file, see [Configuration file](#configuration-file). \n\n**Please note**: only SELECT queries are allowed. \n\n``` python\n  agnostic_query = VersionQuery(query=QUERY_STRING, config_path=CONFIG_PATH)\n  agnostic_query.run_agnostic_query()\n```\n\nThe output is a dictionary in which the keys are the snapshots relevant to that query. The values correspond to sets of tuples containing the query results at the time specified by the key. The positional value of the elements in the tuples is equivalent to the variables indicated in the query.\n\n``` python\n  {\n    TIME_1: {\n      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),\n      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),\n      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)\n    },\n    TIME_2: {\n      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),\n      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),\n      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)\n    },\n    TIME_N: {\n      (VALUE_1_OF_VARIABLE_1, VALUE_1_OF_VARIABLE_2, VALUE_1_OF_VARIABLE_N),\n      (VALUE_2_OF_VARIABLE_1, VALUE_2_OF_VARIABLE_2, VALUE_2_OF_VARIABLE_N),\n      (VALUE_N_OF_VARIABLE_1, VALUE_N_OF_VARIABLE_2, VALUE_N_OF_VARIABLE_N)\n    }\n  }\n```\n\n### Single-delta structured query\n\nPerforming a single-delta query means that a structured queries must be satisfied on a specific change instance of the dataset. This information demand particularly focuses on the differences between two versions, which are typically but not always consecutive.\n\nTo obtain this result, instantiate the **DeltaQuery** class, passing as an argument the SPARQL query string, the time of interest, a set of properties, and the configuration file\'s path. Finally, execute the **run_agnostic_query** method.\n\nThe query string (QUERY_STRING) is useful to identify the entities whose change you want to investigate.\n\nThe specified time is a tuple, in the form (START, END). If one of the two values is None, only the other is considered. The time can be specified using any existing standard.\n\nThe set of properties (PROPERTIES_SET) narrows the field to those entities where the properties specified in the set have changed. If no property was indicated, any changes are considered.\n\nFor more information about the configuration file (CONFIG_PATH), see [Configuration file](#configuration-file). \n\n**Please note**: only SELECT queries are allowed. \n\n``` python\n  agnostic_entity = DeltaQuery(query=QUERY_STRING, on_time=(START, END), changed_properties=PROPERTIES_SET, config_path=CONFIG_PATH)\n  agnostic_entity.run_agnostic_query()\n```\n\nThe output is a dictionary that reports the modified entities, when they were created, modified, and deleted. Moreover, changes are reported as SPARQL UPDATE queries.\n\n``` python\n  {\n      RES_URI_1: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\n      RES_URI_2: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\n      RES_URI_N: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\t\t\n  }    \n```\n\n### Cross-delta structured query\n\nPerforming a cross-delta query means that a structured queries must be satisfied across the differences of the dataset, thus allowing for fully fledged evolution studies.\n\nTo obtain this result, instantiate the **DeltaQuery** class, passing as an argument the SPARQL query string, a set of properties, and the configuration file\'s path. Finally, execute the **run_agnostic_query** method.\n\nThe query string (QUERY_STRING) is useful to identify the entities whose change you want to investigate.\n\nThe set of properties (PROPERTIES_SET) narrows the field to those entities where the properties specified in the set have changed. If no property was indicated, any changes are considered.\n\nFor more information about the configuration file (CONFIG_PATH), see [Configuration file](#configuration-file). \n\n**Please note**: only SELECT queries are allowed. \n\n``` python\n  agnostic_entity = DeltaQuery(query=QUERY_STRING, changed_properties=PROPERTIES_SET, config_path=CONFIG_PATH)\n  agnostic_entity.run_agnostic_query()\n```\n\nThe output is a dictionary that reports the modified entities, when they were created, modified, and deleted. Changes are reported as SPARQL UPDATE queries. If the entity was not created or deleted within the indicated range, the "created" or "deleted" value is None. On the other hand, if the entity does not exist within the input interval, the "modified" value is an empty dictionary.\n\n``` python\n  {\n      RES_URI_1: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\n      RES_URI_2: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\n      RES_URI_N: {\n          "created": TIMESTAMP_CREATION,\n          "modified": {\n              TIMESTAMP_1: UPDATE_QUERY_1,\n              TIMESTAMP_2: UPDATE_QUERY_2,\n              TIMESTAMP_N: UPDATE_QUERY_N\n          },\n          "deleted": TIMESTAMP_DELETION\n      },\t\t\n  }    \n```\n\n### Configuration file\n\nThe configuration file is mainly used to indicate to the library where to search for data and provenance. In addition, some optional values can be set to make executions faster and more efficient.\n\n- **dataset** (required)\n  - **triplestore_urls**: Specify a list of triplestore URLs containing data.  \n  - **file_paths**: Specify a list of paths of files containing data.   \n- **provenance** (required)\n  - **triplestore_urls**: Specify a list of triplestore URLs containing provenance metadata.    \n  - **file_paths** Specify a list of paths of files containing provenance metadata.      \n- **blazegraph_full_text_search**, **fuseki_full_text_search**, **virtuoso_full_text_search** (optional): Specify an affirmative Boolean value if Blazegraph, Fuseki or Virtuoso was used as a triplestore, and a textual index was built to speed up queries. The allowed values are "true", "1", 1, "t", "y", "yes", "ok", or "false", "0", 0, "n", "f", "no".\n- **graphdb_connector_name** (optional): Specify the name of the Lucene connector if GraphDB was used as a triplestore and a textual index was built to speed up queries. For more information, see [https://graphdb.ontotext.com/documentation/free/general-full-text-search-with-connectors.html](https://graphdb.ontotext.com/documentation/free/general-full-text-search-with-connectors.html).\n- **cache_triplestore_url** (optional): Specifies the triplestore URL to use as a cache to make queries faster. If your triplestore uses different endpoints for reading and writing (e.g. GraphDB), specify the endpoint for reading in the "endpoint" field and the endpoint for writing in the "update_endpoint" field. If there is only one endpoint (e.g. Blazegraph), specify it in both fields.\n\n``` json\n  {\n      "dataset": {\n          "triplestore_urls": ["TRIPLESTORE_URL_1", "TRIPLESTORE_URL_2", "TRIPLESTORE_URL_N"],\n          "file_paths": ["PATH_1", "PATH_2", "PATH_N"]\n      },\n      "provenance": {\n          "triplestore_urls": ["TRIPLESTORE_URL_1", "TRIPLESTORE_URL_2", "TRIPLESTORE_URL_N"],\n          "file_paths": ["PATH_1", "PATH_2", "PATH_N"]\n      },\n      "blazegraph_full_text_search": "no",\n      "fuseki_full_text_search": "no",\n      "virtuoso_full_text_search": "no",\n      "graphdb_connector_name": "CONNECTOR_NAME",\n      "cache_triplestore_url": {\n        "endpoint": "READ_ENDPOINT",\n        "update_endpoint": "UPDATE_ENDPOINT"\n    }\n  }\n```\n\n## Developer\'s guide\n\n### First steps\n  1. Install Poetry:\n``` bash\n    pip install poetry\n```\n  2. Clone this repository:\n``` bash\n    git clone https://github.com/opencitations/time-agnostic-library\n    cd ./time-agnostic-library\n```\n  3. Install all the dependencies:\n``` bash\n    poetry install\n```\n  4. Build the package (_output dir:_ `dist`):\n``` bash\n    poetry build\n```\n  5. Globally install the package:\n``` bash\n    pip install ./dist/time-agnostic-library-<VERSION>.tar.gz\n```\n  6. If everything went the right way, than you should be able to use `time_agnostic_library` in your Python modules as follows:\n``` python\n    from time_agnostic_library.agnostic_entity import AgnosticEntity\n    from time_agnostic_library.agnostic_query import AgnosticQuery\n    # ...\n```\n\n### How to run the tests\n\n 1. Make sure that Java is installed on your computer.\n 2. Simply launch the following command from the root folder:\n\n``` bash\n  poetry run test\n```\n\n### How to build the documentation\n\n  1. Move inside the `docs` folder:\n``` bash\n  cd docs\n```\n  2. Use the Makefile provided to build the docs:\n      + _on Windows_\n        ```\n          ./make.bat html\n        ```\n      + _on Linux and MacOs_\n        ```\n          make html\n        ```\n  3. Open the `_build/html/index.html` file with a web browser of your choice!\n\n### How to benchmark\n\nTwo benchmarks were designed, one on the execution times and the other on the RAM. Moreover, all benchmarks are performed on four different triplestores: Blazegraph, GraphDB Free Edition, Apache Jena Fuseki, and OpenLink Virtuoso.\n\nThe dataset used for the benchmarks contains bibliographical information about scholarly works in the journal Scientometrics only if the DOI is known. The data was extracted via Crossref. It is a temporal dataset in which provenance information and change-tracking have been managed by adopting the OpenCitations Data Model. Moreover, the dataset contains information on all the cited academic works. Journals, bibliographic resources, and authors always appear unambiguously, without duplicates. Finally, heuristics have been applied to recover the DOI of the cited works in case Crossref did not provide such information.\n\nIn order to run the benchmark, do the following steps:\n1. Download the dataset from [10.5281/zenodo.7105258](https://doi.org/10.5281/zenodo.7105258). \n2. Extract `reproduce_results.zip`. \n    + _on Windows_\n      \n      Execute `run_banchmarks.bat`\n    + _on Linux and MacOs_\n      \n      Execute `run_banchmarks.sh`\n3. As the results become available, they can be read by opening `json_to_table.html` via a local server.\n\nIn the event that the execution should stop due to unforeseen causes, it will resume from where it was interrupted.\n\n\n',
-    'author': 'Arcangelo Massari',
-    'author_email': 'arcangelo.massari@unibo.it',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/opencitations/time-agnostic-library',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

