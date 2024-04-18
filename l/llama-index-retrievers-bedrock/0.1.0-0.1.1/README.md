# Comparing `tmp/llama_index_retrievers_bedrock-0.1.0.tar.gz` & `tmp/llama_index_retrievers_bedrock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_retrievers_bedrock-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_retrievers_bedrock-0.1.1.tar", max compression
```

## Comparing `llama_index_retrievers_bedrock-0.1.0.tar` & `llama_index_retrievers_bedrock-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1249 2024-04-11 21:10:50.111219 llama_index_retrievers_bedrock-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-04-11 21:10:50.111219 llama_index_retrievers_bedrock-0.1.0/llama_index/retrievers/bedrock/BUILD
--rw-r--r--   0        0        0      123 2024-04-11 21:10:50.111219 llama_index_retrievers_bedrock-0.1.0/llama_index/retrievers/bedrock/__init__.py
--rw-r--r--   0        0        0     3839 2024-04-11 21:10:50.111219 llama_index_retrievers_bedrock-0.1.0/llama_index/retrievers/bedrock/base.py
--rw-r--r--   0        0        0     1384 2024-04-11 21:10:50.111219 llama_index_retrievers_bedrock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 llama_index_retrievers_bedrock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1249 2024-04-18 06:28:54.925770 llama_index_retrievers_bedrock-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-04-18 06:28:54.925770 llama_index_retrievers_bedrock-0.1.1/llama_index/retrievers/bedrock/BUILD
+-rw-r--r--   0        0        0      123 2024-04-18 06:28:54.925770 llama_index_retrievers_bedrock-0.1.1/llama_index/retrievers/bedrock/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-18 06:28:54.925770 llama_index_retrievers_bedrock-0.1.1/llama_index/retrievers/bedrock/base.py
+-rw-r--r--   0        0        0     1396 2024-04-18 06:28:54.925770 llama_index_retrievers_bedrock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 llama_index_retrievers_bedrock-0.1.1/PKG-INFO
```

### Comparing `llama_index_retrievers_bedrock-0.1.0/README.md` & `llama_index_retrievers_bedrock-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_retrievers_bedrock-0.1.0/llama_index/retrievers/bedrock/base.py` & `llama_index_retrievers_bedrock-0.1.1/llama_index/retrievers/bedrock/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Bedrock Retriever."""
 from typing import List, Optional, Dict, Any
 
 from llama_index.core.base.base_retriever import BaseRetriever
 from llama_index.core.callbacks.base import CallbackManager
-from llama_index.core.schema import NodeWithScore, TextNode
+from llama_index.core.schema import NodeWithScore, QueryBundle, TextNode
 from llama_index.core.utilities.aws_utils import get_aws_service_client
 
 
 class AmazonKnowledgeBasesRetriever(BaseRetriever):
     """`Amazon Bedrock Knowledge Bases` retrieval.
 
     See https://aws.amazon.com/bedrock/knowledge-bases for more info.
@@ -67,15 +67,17 @@
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
         )
         self.knowledge_base_id = knowledge_base_id
         self.retrieval_config = retrieval_config
         super().__init__(callback_manager)
 
-    def _retrieve(self, query: str) -> List[NodeWithScore]:
+    def _retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
+        query = query_bundle.query_str
+
         response = self._client.retrieve(
             retrievalQuery={"text": query.strip()},
             knowledgeBaseId=self.knowledge_base_id,
             retrievalConfiguration=self.retrieval_config,
         )
         results = response["retrievalResults"]
         node_with_score = []
```

### Comparing `llama_index_retrievers_bedrock-0.1.0/pyproject.toml` & `llama_index_retrievers_bedrock-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
-contains_example = true
+contains_example = false
 import_path = "llama_index.retrievers.bedrock"
 
 [tool.llamahub.class_authors]
-BedrockRetriever = "AmazonBedrock"
+AmazonKnowledgeBasesRetriever = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index retrievers bedrock integration"
 license = "MIT"
 name = "llama-index-retrievers-bedrock"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
```

### Comparing `llama_index_retrievers_bedrock-0.1.0/PKG-INFO` & `llama_index_retrievers_bedrock-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-retrievers-bedrock
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index retrievers bedrock integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

