# Comparing `tmp/llama_index_cli-0.1.8.tar.gz` & `tmp/llama_index_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_cli-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_cli-0.1.9.tar", max compression
```

## Comparing `llama_index_cli-0.1.8.tar` & `llama_index_cli-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      816 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/__init__.py
--rw-r--r--   0        0        0     8798 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/command_line.py
--rw-r--r--   0        0        0      111 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/__init__.py
--rw-r--r--   0        0        0     3527 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/base.py
--rw-r--r--   0        0        0     2002 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/common/.gitignore
--rw-r--r--   0        0        0      676 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/common/Makefile
--rw-r--r--   0        0        0       17 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/common/_build
--rw-r--r--   0        0        0      320 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/templates/__init__.py
--rw-r--r--   0        0        0      204 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/templates/init.py
--rw-r--r--   0        0        0     1572 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/templates/pyproject.py
--rw-r--r--   0        0        0       60 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/new_package/templates/readme.py
--rw-r--r--   0        0        0      125 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/rag/__init__.py
--rw-r--r--   0        0        0    15136 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/rag/base.py
--rw-r--r--   0        0        0      111 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/upgrade/__init__.py
--rw-r--r--   0        0        0     9644 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/upgrade/base.py
--rw-r--r--   0        0        0    50986 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/llama_index/cli/upgrade/mappings.json
--rw-r--r--   0        0        0     1860 2024-03-06 23:59:45.398217 llama_index_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 llama_index_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      816 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/__init__.py
+-rw-r--r--   0        0        0     9070 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/command_line.py
+-rw-r--r--   0        0        0      111 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/__init__.py
+-rw-r--r--   0        0        0     3527 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/base.py
+-rw-r--r--   0        0        0     2002 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/common/.gitignore
+-rw-r--r--   0        0        0      676 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/common/Makefile
+-rw-r--r--   0        0        0       17 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/common/_build
+-rw-r--r--   0        0        0      320 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/templates/__init__.py
+-rw-r--r--   0        0        0      204 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/templates/init.py
+-rw-r--r--   0        0        0     1572 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/templates/pyproject.py
+-rw-r--r--   0        0        0       60 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/new_package/templates/readme.py
+-rw-r--r--   0        0        0      125 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/rag/__init__.py
+-rw-r--r--   0        0        0    15136 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/rag/base.py
+-rw-r--r--   0        0        0      111 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/upgrade/__init__.py
+-rw-r--r--   0        0        0     9644 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/upgrade/base.py
+-rw-r--r--   0        0        0    51047 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/llama_index/cli/upgrade/mappings.json
+-rw-r--r--   0        0        0     1816 2024-03-12 22:45:13.217973 llama_index_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 llama_index_cli-0.1.9/PKG-INFO
```

### Comparing `llama_index_cli-0.1.8/README.md` & `llama_index_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/command_line.py` & `llama_index_cli-0.1.9/llama_index/cli/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,27 @@
         load_documents=False,
     )
 
     print(f"Successfully downloaded {llama_dataset_class} to {download_dir}")
 
 
 def default_rag_cli() -> RagCLI:
-    import chromadb  # pants: no-infer-dep
     from llama_index.embeddings.openai import OpenAIEmbedding  # pants: no-infer-dep
-    from llama_index.vector_stores.chroma import (
-        ChromaVectorStore,
-    )  # pants: no-infer-dep
+
+    try:
+        import chromadb  # pants: no-infer-dep
+        from llama_index.vector_stores.chroma import (
+            ChromaVectorStore,
+        )  # pants: no-infer-dep
+    except ImportError:
+        raise ImportError(
+            "Default RAG pipeline uses chromadb. "
+            "Install with `pip install llama-index-vector-stores-chroma "
+            "or customize to use a different vector store."
+        )
 
     persist_dir = default_ragcli_persist_dir()
     chroma_client = chromadb.PersistentClient(path=persist_dir)
     chroma_collection = chroma_client.create_collection("default", get_or_create=True)
     vector_store = ChromaVectorStore(
         chroma_collection=chroma_collection, persist_dir=persist_dir
     )
```

### Comparing `llama_index_cli-0.1.8/llama_index/cli/new_package/base.py` & `llama_index_cli-0.1.9/llama_index/cli/new_package/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/new_package/common/.gitignore` & `llama_index_cli-0.1.9/llama_index/cli/new_package/common/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/new_package/common/Makefile` & `llama_index_cli-0.1.9/llama_index/cli/new_package/common/Makefile`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/new_package/templates/pyproject.py` & `llama_index_cli-0.1.9/llama_index/cli/new_package/templates/pyproject.py`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/rag/base.py` & `llama_index_cli-0.1.9/llama_index/cli/rag/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/upgrade/base.py` & `llama_index_cli-0.1.9/llama_index/cli/upgrade/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_cli-0.1.8/llama_index/cli/upgrade/mappings.json` & `llama_index_cli-0.1.9/llama_index/cli/upgrade/mappings.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988950276243094%*

 * *Differences: {"'TiDBVectorStore'": "'llama_index.vector_stores.tidbvector'"}*

```diff
@@ -758,14 +758,15 @@
     "TavilyToolSpec": "llama_index.tools.tavily_research",
     "TelegramReader": "llama_index.readers.telegram",
     "TencentVectorDB": "llama_index.vector_stores.tencentvectordb",
     "TextEmbeddingsInference": "llama_index.embeddings.text_embeddings_inference",
     "TextNode": "llama_index.core.schema",
     "TextSplitter": "llama_index.core.node_parser",
     "TextToImageToolSpec": "llama_index.tools.text_to_image",
+    "TiDBVectorStore": "llama_index.vector_stores.tidbvector",
     "TimeWeightedPostprocessor": "llama_index.core.postprocessor",
     "TimescaleVectorAutoretrievalPack": "llama_index.packs.timescale_vector_autoretrieval",
     "TimescaleVectorStore": "llama_index.vector_stores.timescalevector",
     "TitleExtractor": "llama_index.core.extractors",
     "TogetherEmbedding": "llama_index.embeddings.together",
     "TogetherLLM": "llama_index.llms.together",
     "TokenCountingHandler": "llama_index.core.callbacks",
```

### Comparing `llama_index_cli-0.1.8/pyproject.toml` & `llama_index_cli-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -28,20 +28,19 @@
     "Logan Markewich <logan@llamaindex.ai>",
     "Simon Suo <simon@llamaindex.ai>",
     "Sourabh Desai <sourabh@llamaindex.ai>",
 ]
 name = "llama-index-cli"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
-llama-index-vector-stores-chroma = "^0.1.1"
 llama-index-embeddings-openai = "^0.1.1"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
```

### Comparing `llama_index_cli-0.1.8/PKG-INFO` & `llama_index_cli-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: llama-index-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index cli
 License: MIT
 Author: llamaindex
 Maintainer: Andrei Fajardo
 Maintainer-email: andrei@runllama.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: llama-index-embeddings-openai (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
-Requires-Dist: llama-index-vector-stores-chroma (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex CLI
 
 ## Installation
 
 ```sh
```

