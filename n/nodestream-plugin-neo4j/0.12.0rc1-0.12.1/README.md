# Comparing `tmp/nodestream_plugin_neo4j-0.12.0rc1.tar.gz` & `tmp/nodestream_plugin_neo4j-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_neo4j-0.12.0rc1.tar", max compression
+gzip compressed data, was "nodestream_plugin_neo4j-0.12.1.tar", max compression
```

## Comparing `nodestream_plugin_neo4j-0.12.0rc1.tar` & `nodestream_plugin_neo4j-0.12.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2547 2024-01-18 16:53:12.239701 nodestream_plugin_neo4j-0.12.0rc1/README.md
--rw-r--r--   0        0        0       94 2024-03-08 15:43:02.882311 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/__init__.py
--rw-r--r--   0        0        0     2703 2024-03-08 17:46:33.350050 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/database_connector.py
--rw-r--r--   0        0        0     1744 2024-03-08 15:43:02.886882 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/extractor.py
--rw-r--r--   0        0        0     9475 2024-03-08 17:46:33.351553 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/ingest_query_builder.py
--rw-r--r--   0        0        0    16927 2024-03-20 18:23:46.523855 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/migrator.py
--rw-r--r--   0        0        0     1807 2024-04-03 14:25:34.326336 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/neo4j_database.py
--rw-r--r--   0        0        0     2195 2024-03-08 17:46:33.352799 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query.py
--rw-r--r--   0        0        0     2821 2024-03-08 17:46:33.354141 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query_executor.py
--rw-r--r--   0        0        0     2762 2024-03-08 15:43:02.896795 nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/type_retriever.py
--rw-r--r--   0        0        0     1012 2024-04-03 14:28:10.722380 nodestream_plugin_neo4j-0.12.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 nodestream_plugin_neo4j-0.12.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2496 2024-04-18 17:27:20.243143 nodestream_plugin_neo4j-0.12.1/README.md
+-rw-r--r--   0        0        0       94 2024-03-08 15:43:02.882311 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/__init__.py
+-rw-r--r--   0        0        0     2703 2024-03-08 17:46:33.350050 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/database_connector.py
+-rw-r--r--   0        0        0     1744 2024-03-08 15:43:02.886882 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/extractor.py
+-rw-r--r--   0        0        0     9717 2024-04-18 17:27:20.243898 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0    16927 2024-03-20 18:23:46.523855 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/migrator.py
+-rw-r--r--   0        0        0     1807 2024-04-03 14:25:34.326336 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/neo4j_database.py
+-rw-r--r--   0        0        0     2507 2024-04-18 17:27:20.244610 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/query.py
+-rw-r--r--   0        0        0     2898 2024-04-18 17:27:20.245183 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/query_executor.py
+-rw-r--r--   0        0        0     2762 2024-03-08 15:43:02.896795 nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/type_retriever.py
+-rw-r--r--   0        0        0      967 2024-04-18 17:27:45.340384 nodestream_plugin_neo4j-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 nodestream_plugin_neo4j-0.12.1/PKG-INFO
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/README.md` & `nodestream_plugin_neo4j-0.12.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Neo4j Nodestream Plugin for Nodestream
 
 This plugin provides a [Nodestream](https://github.com/nodestream-proj/nodestream) interface to Neo4j. 
 
-**THIS PLUGIN IS IN BETA. USE AT YOUR OWN RISK.**
-
 ## Installation
 
 ```bash
 pip install nodestream-plugin-neo4j
 ```
 
 ## Usage
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/database_connector.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/database_connector.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/extractor.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/extractor.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/ingest_query_builder.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/ingest_query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,16 +250,23 @@
         query_builder = query_builder.where_literal(
             f"{ref_name}.last_ingested_at <= $earliest_allowed_time"
         ).return_literal(f"id({ref_name}) as id")
 
         return Query(str(query_builder), params)
 
     def generate_ttl_query_from_configuration(
-        self, config: TimeToLiveConfiguration
+        self,
+        config: TimeToLiveConfiguration,
+        retries_per_chunk,
     ) -> Query:
         ttl_match_query = self.generate_ttl_match_query(config)
+        execute_chunks_in_parallel = (
+            config.graph_object_type == GraphObjectType.RELATIONSHIP
+        )
         operation = (
             DELETE_NODE_QUERY
             if config.graph_object_type == GraphObjectType.NODE
             else DELETE_REL_QUERY
         )
-        return ttl_match_query.feed_batched_query(operation)
+        return ttl_match_query.feed_batched_query(
+            operation, config.batch_size, execute_chunks_in_parallel, retries_per_chunk
+        )
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/migrator.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/migrator.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/neo4j_database.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/neo4j_database.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,22 +25,31 @@
     query_statement: str
     parameters: Dict[str, Any]
 
     @classmethod
     def from_statement(cls, query_statement: str, **parameters: Any) -> "Query":
         return cls(query_statement, parameters)
 
-    def feed_batched_query(self, batched_query: str) -> "Query":
+    def feed_batched_query(
+        self,
+        batched_query: str,
+        chunk_size: int = 1000,
+        execute_chunks_in_parallel: bool = True,
+        retries_per_chunk: int = 3,
+    ) -> "Query":
         """Feed the results of the the query into another query that will be executed in batches."""
         return Query(
             COMMIT_QUERY,
             {
                 "iterate_params": self.parameters,
                 "batched_query": batched_query,
                 "iterable_query": self.query_statement,
+                "execute_chunks_in_parallel": execute_chunks_in_parallel,
+                "chunk_size": chunk_size,
+                "retries_per_chunk": retries_per_chunk,
             },
         )
 
 
 @dataclass(slots=True, frozen=True)
 class QueryBatch:
     query_statement: str
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/query_executor.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/query_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,13 +67,16 @@
         )
         await self.database_connection.execute(
             batched_query.as_query(self.ingest_query_builder.apoc_iterate),
             log_result=True,
         )
 
     async def perform_ttl_op(self, config: TimeToLiveConfiguration):
-        query = self.ingest_query_builder.generate_ttl_query_from_configuration(config)
+        query = self.ingest_query_builder.generate_ttl_query_from_configuration(
+            config,
+            retries_per_chunk=self.retries_per_chunk,
+        )
         await self.database_connection.execute(query)
 
     async def execute_hook(self, hook: IngestionHook):
         query_string, params = hook.as_cypher_query_and_parameters()
         await self.database_connection.execute(Query(query_string, params))
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/nodestream_plugin_neo4j/type_retriever.py` & `nodestream_plugin_neo4j-0.12.1/nodestream_plugin_neo4j/type_retriever.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/pyproject.toml` & `nodestream_plugin_neo4j-0.12.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nodestream-plugin-neo4j"
-version = "0.12.0rc1"
+version = "0.12.1"
 description = ""
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 neo4j = "^5.16.0"
-nodestream = { version = "0.12.0rc2", allow-prereleases = true} 
+nodestream = "^0.12.0"
 cymple = "^0.11.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 pyhamcrest = "^2.1.0"
 freezegun = "^1.4.0"
 pytest = "^7.4.4"
```

### Comparing `nodestream_plugin_neo4j-0.12.0rc1/PKG-INFO` & `nodestream_plugin_neo4j-0.12.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-neo4j
-Version: 0.12.0rc1
+Version: 0.12.1
 Summary: 
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cymple (>=0.11.0,<0.12.0)
 Requires-Dist: neo4j (>=5.16.0,<6.0.0)
-Requires-Dist: nodestream (==0.12.0rc2)
+Requires-Dist: nodestream (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Neo4j Nodestream Plugin for Nodestream
 
 This plugin provides a [Nodestream](https://github.com/nodestream-proj/nodestream) interface to Neo4j. 
 
-**THIS PLUGIN IS IN BETA. USE AT YOUR OWN RISK.**
-
 ## Installation
 
 ```bash
 pip install nodestream-plugin-neo4j
 ```
 
 ## Usage
```

