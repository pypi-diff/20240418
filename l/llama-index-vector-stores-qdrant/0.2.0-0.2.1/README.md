# Comparing `tmp/llama_index_vector_stores_qdrant-0.2.0.tar.gz` & `tmp/llama_index_vector_stores_qdrant-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_qdrant-0.2.1.tar", max compression
```

## Comparing `llama_index_vector_stores_qdrant-0.2.0.tar` & `llama_index_vector_stores_qdrant-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/README.md
--rw-r--r--   0        0        0      101 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/__init__.py
--rw-r--r--   0        0        0    33618 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/base.py
--rw-r--r--   0        0        0     6897 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/utils.py
--rw-r--r--   0        0        0     1600 2024-04-10 15:16:06.411105 llama_index_vector_stores_qdrant-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-18 21:29:04.575369 llama_index_vector_stores_qdrant-0.2.1/README.md
+-rw-r--r--   0        0        0      101 2024-04-18 21:29:04.575369 llama_index_vector_stores_qdrant-0.2.1/llama_index/vector_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0    33728 2024-04-18 21:29:04.575369 llama_index_vector_stores_qdrant-0.2.1/llama_index/vector_stores/qdrant/base.py
+-rw-r--r--   0        0        0     6897 2024-04-18 21:29:04.575369 llama_index_vector_stores_qdrant-0.2.1/llama_index/vector_stores/qdrant/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-18 21:29:04.575369 llama_index_vector_stores_qdrant-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.2.1/PKG-INFO
```

### Comparing `llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/base.py` & `llama_index_vector_stores_qdrant-0.2.1/llama_index/vector_stores/qdrant/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,18 +867,19 @@
                         match=MatchAny(any=str(subfilter.value).split(",")),
                     )
                 )
 
         return Filter(must=must_conditions)
 
     def use_old_sparse_encoder(self, collection_name: str) -> bool:
+        collection_info = self.client.get_collection(collection_name)
         return (
             self._collection_exists(collection_name)
-            and SPARSE_VECTOR_NAME_OLD
-            in self.client.get_collection(collection_name).config.params.vectors
+            and collection_info.config.params.sparse_vectors is not None
+            and SPARSE_VECTOR_NAME_OLD in collection_info.config.params.sparse_vectors
         )
 
     @property
     def sparse_vector_name(self) -> str:
         return (
             SPARSE_VECTOR_NAME_OLD
             if self.use_old_sparse_encoder(self.collection_name)
```

### Comparing `llama_index_vector_stores_qdrant-0.2.0/llama_index/vector_stores/qdrant/utils.py` & `llama_index_vector_stores_qdrant-0.2.1/llama_index/vector_stores/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_qdrant-0.2.0/pyproject.toml` & `llama_index_vector_stores_qdrant-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores qdrant integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-qdrant"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 llama-index-core = "^0.10.1"
 qdrant-client = "^1.7.1"
 grpcio = "^1.60.0"
```

### Comparing `llama_index_vector_stores_qdrant-0.2.0/PKG-INFO` & `llama_index_vector_stores_qdrant-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-qdrant
-Version: 0.2.0
+Version: 0.2.1
 Summary: llama-index vector_stores qdrant integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

