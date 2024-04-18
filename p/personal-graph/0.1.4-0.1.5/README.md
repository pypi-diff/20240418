# Comparing `tmp/personal_graph-0.1.4.tar.gz` & `tmp/personal_graph-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_graph-0.1.4.tar", max compression
+gzip compressed data, was "personal_graph-0.1.5.tar", max compression
```

## Comparing `personal_graph-0.1.4.tar` & `personal_graph-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.4/LICENSE
--rw-r--r--   0        0        0     8661 2024-03-30 12:39:30.387205 personal_graph-0.1.4/README.md
--rw-r--r--   0        0        0       54 2024-04-08 09:45:51.825318 personal_graph-0.1.4/personal_graph/__init__.py
--rw-r--r--   0        0        0    25303 2024-04-17 11:56:47.270908 personal_graph-0.1.4/personal_graph/database.py
--rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/embeddings.py
--rw-r--r--   0        0        0     6031 2024-04-17 11:56:47.270908 personal_graph-0.1.4/personal_graph/graph.py
--rw-r--r--   0        0        0      142 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/ml.py
--rw-r--r--   0        0        0     1797 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/models.py
--rw-r--r--   0        0        0     4421 2024-04-17 11:56:47.274908 personal_graph-0.1.4/personal_graph/natural.py
--rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.4/personal_graph/retriever.py
--rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/delete-edge-embedding.sql
--rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/delete-edge.sql
--rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/delete-node-embedding.sql
--rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/delete-node.sql
--rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/existing-edge.sql
--rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/existing-node.sql
--rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/insert-edge-embedding.sql
--rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/insert-edge.sql
--rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.4/personal_graph/sql/insert-node-embedding.sql
--rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/insert-node.sql
--rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/schema.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.4/personal_graph/sql/search-edges-inbound.sql
--rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.4/personal_graph/sql/search-edges-outbound.sql
--rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.4/personal_graph/sql/search-edges.sql
--rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/search-node.template
--rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/search-where.template
--rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/traverse.template
--rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.4/personal_graph/sql/update-node.sql
--rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.4/personal_graph/sql/vector-search-edge.sql
--rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.4/personal_graph/sql/vector-search-node.sql
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.742142 personal_graph-0.1.4/personal_graph/tests/__init__.py
--rw-r--r--   0        0        0     2391 2024-04-12 11:09:18.211085 personal_graph-0.1.4/personal_graph/tests/conftest.py
--rw-r--r--   0        0        0     3723 2024-04-08 05:20:20.742142 personal_graph-0.1.4/personal_graph/tests/test_database.py
--rw-r--r--   0        0        0     4551 2024-04-12 11:09:18.211085 personal_graph-0.1.4/personal_graph/tests/test_graph.py
--rw-r--r--   0        0        0        0 2024-04-08 05:20:20.746141 personal_graph-0.1.4/personal_graph/tests/test_ml.py
--rw-r--r--   0        0        0     1405 2024-04-12 11:09:18.211085 personal_graph-0.1.4/personal_graph/tests/test_natural.py
--rw-r--r--   0        0        0     1399 2024-04-08 05:20:20.746141 personal_graph-0.1.4/personal_graph/tests/test_visualizers.py
--rw-r--r--   0        0        0     4011 2024-04-17 11:56:47.274908 personal_graph-0.1.4/personal_graph/visualizers.py
--rw-r--r--   0        0        0      977 2024-04-17 12:06:44.305803 personal_graph-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9824 1970-01-01 00:00:00.000000 personal_graph-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-13 05:55:36.893450 personal_graph-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8661 2024-03-30 12:39:30.387205 personal_graph-0.1.5/README.md
+-rw-r--r--   0        0        0       54 2024-04-08 09:45:51.825318 personal_graph-0.1.5/personal_graph/__init__.py
+-rw-r--r--   0        0        0    25303 2024-04-17 11:56:47.270908 personal_graph-0.1.5/personal_graph/database.py
+-rw-r--r--   0        0        0      903 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/embeddings.py
+-rw-r--r--   0        0        0     6031 2024-04-17 11:56:47.270908 personal_graph-0.1.5/personal_graph/graph.py
+-rw-r--r--   0        0        0      142 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/ml.py
+-rw-r--r--   0        0        0     1797 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/models.py
+-rw-r--r--   0        0        0     4421 2024-04-17 11:56:47.274908 personal_graph-0.1.5/personal_graph/natural.py
+-rw-r--r--   0        0        0     1161 2024-04-17 11:56:47.274908 personal_graph-0.1.5/personal_graph/retriever.py
+-rw-r--r--   0        0        0       52 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/delete-edge-embedding.sql
+-rw-r--r--   0        0        0       48 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/delete-edge.sql
+-rw-r--r--   0        0        0       45 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/delete-node-embedding.sql
+-rw-r--r--   0        0        0       30 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/delete-node.sql
+-rw-r--r--   0        0        0       97 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/existing-edge.sql
+-rw-r--r--   0        0        0       39 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/existing-node.sql
+-rw-r--r--   0        0        0       72 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/insert-edge-embedding.sql
+-rw-r--r--   0        0        0       91 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/insert-edge.sql
+-rw-r--r--   0        0        0       62 2024-04-08 05:20:20.734143 personal_graph-0.1.5/personal_graph/sql/insert-node-embedding.sql
+-rw-r--r--   0        0        0       70 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/insert-node.sql
+-rw-r--r--   0        0        0     1116 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/schema.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.5/personal_graph/sql/search-edges-inbound.sql
+-rw-r--r--   0        0        0       36 2024-04-08 05:20:20.738142 personal_graph-0.1.5/personal_graph/sql/search-edges-outbound.sql
+-rw-r--r--   0        0        0       80 2024-04-08 05:20:20.738142 personal_graph-0.1.5/personal_graph/sql/search-edges.sql
+-rw-r--r--   0        0        0      252 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/search-node.template
+-rw-r--r--   0        0        0      297 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/search-where.template
+-rw-r--r--   0        0        0      609 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/traverse.template
+-rw-r--r--   0        0        0       75 2024-04-12 11:09:18.207085 personal_graph-0.1.5/personal_graph/sql/update-node.sql
+-rw-r--r--   0        0        0      283 2024-04-12 11:09:18.211085 personal_graph-0.1.5/personal_graph/sql/vector-search-edge.sql
+-rw-r--r--   0        0        0      254 2024-04-12 11:09:18.211085 personal_graph-0.1.5/personal_graph/sql/vector-search-node.sql
+-rw-r--r--   0        0        0        0 2024-04-08 05:20:20.742142 personal_graph-0.1.5/personal_graph/tests/__init__.py
+-rw-r--r--   0        0        0     2391 2024-04-12 11:09:18.211085 personal_graph-0.1.5/personal_graph/tests/conftest.py
+-rw-r--r--   0        0        0     3723 2024-04-08 05:20:20.742142 personal_graph-0.1.5/personal_graph/tests/test_database.py
+-rw-r--r--   0        0        0     4551 2024-04-12 11:09:18.211085 personal_graph-0.1.5/personal_graph/tests/test_graph.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:20:20.746141 personal_graph-0.1.5/personal_graph/tests/test_ml.py
+-rw-r--r--   0        0        0     1405 2024-04-12 11:09:18.211085 personal_graph-0.1.5/personal_graph/tests/test_natural.py
+-rw-r--r--   0        0        0     1399 2024-04-08 05:20:20.746141 personal_graph-0.1.5/personal_graph/tests/test_visualizers.py
+-rw-r--r--   0        0        0     4011 2024-04-17 11:56:47.274908 personal_graph-0.1.5/personal_graph/visualizers.py
+-rw-r--r--   0        0        0      996 2024-04-17 13:20:00.974573 personal_graph-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9864 1970-01-01 00:00:00.000000 personal_graph-0.1.5/PKG-INFO
```

### Comparing `personal_graph-0.1.4/LICENSE` & `personal_graph-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/README.md` & `personal_graph-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/database.py` & `personal_graph-0.1.5/personal_graph/database.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/embeddings.py` & `personal_graph-0.1.5/personal_graph/embeddings.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/graph.py` & `personal_graph-0.1.5/personal_graph/graph.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/models.py` & `personal_graph-0.1.5/personal_graph/models.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/natural.py` & `personal_graph-0.1.5/personal_graph/natural.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/retriever.py` & `personal_graph-0.1.5/personal_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/sql/schema.sql` & `personal_graph-0.1.5/personal_graph/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/sql/traverse.template` & `personal_graph-0.1.5/personal_graph/sql/traverse.template`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/tests/conftest.py` & `personal_graph-0.1.5/personal_graph/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/tests/test_database.py` & `personal_graph-0.1.5/personal_graph/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/tests/test_graph.py` & `personal_graph-0.1.5/personal_graph/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/tests/test_natural.py` & `personal_graph-0.1.5/personal_graph/tests/test_natural.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/tests/test_visualizers.py` & `personal_graph-0.1.5/personal_graph/tests/test_visualizers.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/personal_graph/visualizers.py` & `personal_graph-0.1.5/personal_graph/visualizers.py`

 * *Files identical despite different names*

### Comparing `personal_graph-0.1.4/pyproject.toml` & `personal_graph-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "personal-graph"
-version = "0.1.4"
+version = "0.1.5"
 description = "Graph database in LibSQL"
 authors = ["Anubhuti Bhardwaj <anubhutibhardwaj11@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = [
     { path = "examples/personal-graph.ipynb" }
 ]
@@ -22,14 +22,15 @@
 instructor = "^0.6.7"
 fastapi = "^0.110.0"
 uvicorn = "^0.29.0"
 sqlean-py = "^3.45.1"
 streamlit = "^1.33.0"
 types-pygments = "^2.17.0.20240310"
 types-decorator = "^5.1.8.20240310"
+dspy-ai = "^2.4.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 ruff = "^0.3.2"
 mypy = "^1.9.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `personal_graph-0.1.4/PKG-INFO` & `personal_graph-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: personal-graph
-Version: 0.1.4
+Version: 0.1.5
 Summary: Graph database in LibSQL
 License: MIT
 Author: Anubhuti Bhardwaj
 Author-email: anubhutibhardwaj11@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: scrollable-textbox
+Requires-Dist: dspy-ai (>=2.4.5,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: instructor (>=0.6.7,<0.7.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: libsql-experimental (>=0.0.28,<0.0.29)
 Requires-Dist: openai (>=1.14.2,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
```

