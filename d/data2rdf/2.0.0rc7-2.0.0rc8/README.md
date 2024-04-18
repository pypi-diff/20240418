# Comparing `tmp/data2rdf-2.0.0rc7.tar.gz` & `tmp/data2rdf-2.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-2.0.0rc7.tar", last modified: Wed Apr 17 12:33:36 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc8.tar", last modified: Wed Apr 17 20:47:24 2024, max compression
```

## Comparing `data2rdf-2.0.0rc7.tar` & `data2rdf-2.0.0rc8.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.142654 data2rdf-2.0.0rc7/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1732 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/models/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/abox_scaffolding_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5656 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/pipelines/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/data2rdf/qudt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/qudt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/qudt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/data2rdf/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 12:33:36.000000 data2rdf-2.0.0rc7/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1916 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.146654 data2rdf-2.0.0rc7/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:36.150654 data2rdf-2.0.0rc7/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-17 12:33:32.000000 data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.505449 data2rdf-2.0.0rc8/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1732 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/data2rdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/models/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/data2rdf/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/data2rdf/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/pipelines/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5929 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/pipelines/abox_scaffolding_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5741 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/pipelines/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/qudt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/data2rdf/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 20:47:24.000000 data2rdf-2.0.0rc8/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1936 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.509449 data2rdf-2.0.0rc8/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/csv_pipeline_test/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/csv_pipeline_test/test_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/csv_pipeline_test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/tests/json_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/json_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2062 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/json_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/json_pipeline_test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:24.513449 data2rdf-2.0.0rc8/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6450 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/xls_pipeline_test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-17 20:47:21.000000 data2rdf-2.0.0rc8/tests/xls_pipeline_test/test_pipeline.py
```

### Comparing `data2rdf-2.0.0rc7/LICENSE` & `data2rdf-2.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/PKG-INFO` & `data2rdf-2.0.0rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0.0
 Requires-Dist: chowlk-unofficial-fork==0.0.2
+Requires-Dist: jsonpath-ng~=1.6.1
 Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
```

### Comparing `data2rdf-2.0.0rc7/README.md` & `data2rdf-2.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/config.py` & `data2rdf-2.0.0rc8/data2rdf/config.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/models/mapping.py` & `data2rdf-2.0.0rc8/data2rdf/models/mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,7 +217,18 @@
                     str(cls.iri),
                     annotation,
                 ]
             }
         else:
             types = {"@type": str(cls.iri)}
         return types
+
+
+class JsonConceptMapping(ClassConceptMapping):
+    """A special model for mapping from json files to semantic concepts"""
+
+    value_location: str = Field(
+        ..., description="Json path for the value of the quantity or property"
+    )
+    unit_location: Optional[str] = Field(
+        None, description="Json path to the unit of the property"
+    )
```

### Comparing `data2rdf-2.0.0rc7/data2rdf/parsers/base.py` & `data2rdf-2.0.0rc8/data2rdf/parsers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class DataParser(BaseModel):
     """
     generic parser abstract class with common parser attrubutes and functionalities
     """
 
-    raw_data: str = Field(
+    raw_data: Union[str, Dict[str, Any]] = Field(
         ..., description="File path to the data file to be parsed."
     )
     mapping: Union[str, Dict[str, ClassConceptMapping]] = Field(
         ...,
         description="""File path to the mapping file to be parsed or
         a dictionary with the mapping.""",
     )
```

### Comparing `data2rdf-2.0.0rc7/data2rdf/parsers/csv.py` & `data2rdf-2.0.0rc8/data2rdf/parsers/csv.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/parsers/excel.py` & `data2rdf-2.0.0rc8/data2rdf/parsers/excel.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/parsers/utils.py` & `data2rdf-2.0.0rc8/data2rdf/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/pipelines/abox_scaffolding_pipeline.py` & `data2rdf-2.0.0rc8/data2rdf/pipelines/abox_scaffolding_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/pipelines/annotation_pipeline.py` & `data2rdf-2.0.0rc8/data2rdf/pipelines/annotation_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 
 class AnnotationPipeline(BaseModel):
 
     """
     Runs the complete data2rdf pipeline.
     """
 
-    raw_data: str = Field(
-        ..., description="File path to the data file to be parsed."
+    raw_data: Union[str, Dict[str, Any]] = Field(
+        ...,
+        description="File path to the data file to be parsed or in case of a json file: the parsed data as `dict`.",
     )
     mapping: Union[str, Dict[str, Any]] = Field(
         ...,
         description="""File path to the mapping file to be parsed or
         a dictionary with the mapping.""",
     )
```

### Comparing `data2rdf-2.0.0rc7/data2rdf/qudt/utils.py` & `data2rdf-2.0.0rc8/data2rdf/qudt/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf/utils.py` & `data2rdf-2.0.0rc8/data2rdf/utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc8/data2rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
 Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0.0
 Requires-Dist: chowlk-unofficial-fork==0.0.2
+Requires-Dist: jsonpath-ng~=1.6.1
 Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
```

### Comparing `data2rdf-2.0.0rc7/setup.cfg` & `data2rdf-2.0.0rc8/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data2rdf
-version = v2.0.0rc7
+version = v2.0.0rc8
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
 author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
@@ -17,14 +17,15 @@
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
 	beautifulsoup4>=4.0.0
 	chowlk-unofficial-fork==0.0.2
+	jsonpath-ng~=1.6.1
 	lru-cache<1
 	openpyxl>=3,<4
 	pandas>=2,<3
 	pydantic>=2,<3
 	pydantic-settings
 	python-dotenv
 	rdflib>=6,<7
```

### Comparing `data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc8/tests/csv_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/tests/csv_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc8/tests/csv_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/tests/test_models.py` & `data2rdf-2.0.0rc8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/tests/test_utils.py` & `data2rdf-2.0.0rc8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_parser.py` & `data2rdf-2.0.0rc8/tests/xls_pipeline_test/test_parser.py`

 * *Files identical despite different names*

### Comparing `data2rdf-2.0.0rc7/tests/xls_pipeline_test/test_pipeline.py` & `data2rdf-2.0.0rc8/tests/xls_pipeline_test/test_pipeline.py`

 * *Files identical despite different names*

