# Comparing `tmp/chat_rag-0.1.65.tar.gz` & `tmp/chat_rag-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_rag-0.1.65.tar", max compression
+gzip compressed data, was "chat_rag-0.1.66.tar", max compression
```

## Comparing `chat_rag-0.1.65.tar` & `chat_rag-0.1.66.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1083 2024-02-07 09:34:49.972743 chat_rag-0.1.65/LICENSE
--rw-r--r--   0        0        0     1666 2023-12-13 14:55:14.591003 chat_rag-0.1.65/README.md
--rw-r--r--   0        0        0       68 2024-04-02 12:17:40.982534 chat_rag-0.1.65/chat_rag/__init__.py
--rw-r--r--   0        0        0     3295 2024-04-02 12:17:40.982534 chat_rag-0.1.65/chat_rag/async_rag.py
--rw-r--r--   0        0        0        0 2023-12-13 14:55:14.591003 chat_rag-0.1.65/chat_rag/data/__init__.py
--rw-r--r--   0        0        0      788 2024-01-31 17:51:45.327655 chat_rag-0.1.65/chat_rag/data/models.py
--rw-r--r--   0        0        0    10492 2024-04-02 12:17:40.982534 chat_rag-0.1.65/chat_rag/data/parsers.py
--rw-r--r--   0        0        0    13027 2024-03-06 13:48:08.349750 chat_rag-0.1.65/chat_rag/data/splitters.py
--rw-r--r--   0        0        0      897 2024-02-26 17:12:56.927011 chat_rag-0.1.65/chat_rag/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/inf_retrieval/__init__.py
--rw-r--r--   0        0        0     3924 2024-01-22 11:13:32.756810 chat_rag-0.1.65/chat_rag/inf_retrieval/check_answ_questions.py
--rw-r--r--   0        0        0     2450 2024-02-07 09:34:49.972743 chat_rag-0.1.65/chat_rag/inf_retrieval/cross_encoder.py
--rw-r--r--   0        0        0      141 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/inf_retrieval/embedding_models/__init__.py
--rw-r--r--   0        0        0     4617 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/inf_retrieval/embedding_models/base_model.py
--rw-r--r--   0        0        0     1494 2024-01-18 15:08:39.142423 chat_rag-0.1.65/chat_rag/inf_retrieval/embedding_models/e5_model.py
--rw-r--r--   0        0        0     4693 2024-01-22 11:13:32.756810 chat_rag-0.1.65/chat_rag/inf_retrieval/query_generator.py
--rw-r--r--   0        0        0     3886 2024-02-07 09:34:49.972743 chat_rag-0.1.65/chat_rag/inf_retrieval/reference_checker.py
--rw-r--r--   0        0        0      240 2024-04-02 12:17:40.982534 chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/__init__.py
--rw-r--r--   0        0        0      856 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
--rw-r--r--   0        0        0      503 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/retriever_client.py
--rw-r--r--   0        0        0     7447 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
--rw-r--r--   0        0        0      135 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/intent_detection/__init__.py
--rw-r--r--   0        0        0     1527 2024-01-22 11:13:32.756810 chat_rag-0.1.65/chat_rag/intent_detection/clusterize_text.py
--rw-r--r--   0        0        0     1419 2024-01-22 11:13:32.760810 chat_rag-0.1.65/chat_rag/intent_detection/gen_intent.py
--rw-r--r--   0        0        0      445 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/llms/__init__.py
--rw-r--r--   0        0        0     6995 2024-02-26 17:12:56.927011 chat_rag-0.1.65/chat_rag/llms/base_llm.py
--rw-r--r--   0        0        0     9040 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/llms/claude_client.py
--rw-r--r--   0        0        0     5219 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/llms/ggml_llm.py
--rw-r--r--   0        0        0     9255 2023-12-13 14:55:14.595003 chat_rag-0.1.65/chat_rag/llms/hf_llm.py
--rw-r--r--   0        0        0    10715 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/llms/mistral_client.py
--rw-r--r--   0        0        0    10629 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/llms/openai_client.py
--rw-r--r--   0        0        0    25992 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/llms/vllm_client.py
--rw-r--r--   0        0        0     3578 2024-04-02 12:17:40.986534 chat_rag-0.1.65/chat_rag/rag.py
--rw-r--r--   0        0        0      932 2024-04-05 13:05:12.543836 chat_rag-0.1.65/pyproject.toml
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 chat_rag-0.1.65/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.66/LICENSE
+-rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.66/README.md
+-rw-r--r--   0        0        0       68 2024-04-16 07:55:27.403398 chat_rag-0.1.66/chat_rag/__init__.py
+-rw-r--r--   0        0        0     3295 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/async_rag.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/data/__init__.py
+-rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/data/models.py
+-rw-r--r--   0        0        0    10492 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/data/parsers.py
+-rw-r--r--   0        0        0    13027 2024-03-06 16:38:44.353919 chat_rag-0.1.66/chat_rag/data/splitters.py
+-rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.66/chat_rag/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/__init__.py
+-rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/check_answ_questions.py
+-rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/cross_encoder.py
+-rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/embedding_models/__init__.py
+-rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/embedding_models/base_model.py
+-rw-r--r--   0        0        0     1494 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/embedding_models/e5_model.py
+-rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/query_generator.py
+-rw-r--r--   0        0        0     3886 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/reference_checker.py
+-rw-r--r--   0        0        0      240 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
+-rw-r--r--   0        0        0      503 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/retriever_client.py
+-rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
+-rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/intent_detection/__init__.py
+-rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/intent_detection/clusterize_text.py
+-rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/intent_detection/gen_intent.py
+-rw-r--r--   0        0        0      445 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/llms/__init__.py
+-rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.66/chat_rag/llms/base_llm.py
+-rw-r--r--   0        0        0     9040 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/llms/claude_client.py
+-rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/llms/ggml_llm.py
+-rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.66/chat_rag/llms/hf_llm.py
+-rw-r--r--   0        0        0    10715 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/llms/mistral_client.py
+-rw-r--r--   0        0        0    10629 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/llms/openai_client.py
+-rw-r--r--   0        0        0    25992 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/llms/vllm_client.py
+-rw-r--r--   0        0        0     3578 2024-04-16 07:55:27.407398 chat_rag-0.1.66/chat_rag/rag.py
+-rw-r--r--   0        0        0      932 2024-04-18 10:01:19.469159 chat_rag-0.1.66/pyproject.toml
+-rw-r--r--   0        0        0     3166 1970-01-01 00:00:00.000000 chat_rag-0.1.66/PKG-INFO
```

### Comparing `chat_rag-0.1.65/LICENSE` & `chat_rag-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/README.md` & `chat_rag-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/async_rag.py` & `chat_rag-0.1.66/chat_rag/async_rag.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/data/models.py` & `chat_rag-0.1.66/chat_rag/data/models.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/data/parsers.py` & `chat_rag-0.1.66/chat_rag/data/parsers.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/data/splitters.py` & `chat_rag-0.1.66/chat_rag/data/splitters.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/exceptions.py` & `chat_rag-0.1.66/chat_rag/exceptions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/check_answ_questions.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/check_answ_questions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/cross_encoder.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/embedding_models/base_model.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/embedding_models/base_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/embedding_models/e5_model.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/embedding_models/e5_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/query_generator.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/query_generator.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/reference_checker.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/reference_checker.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/rerank_retriever.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/rerank_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/inf_retrieval/retrievers/semantic_retriever.py` & `chat_rag-0.1.66/chat_rag/inf_retrieval/retrievers/semantic_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/intent_detection/clusterize_text.py` & `chat_rag-0.1.66/chat_rag/intent_detection/clusterize_text.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/intent_detection/gen_intent.py` & `chat_rag-0.1.66/chat_rag/intent_detection/gen_intent.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/base_llm.py` & `chat_rag-0.1.66/chat_rag/llms/base_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/claude_client.py` & `chat_rag-0.1.66/chat_rag/llms/claude_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/ggml_llm.py` & `chat_rag-0.1.66/chat_rag/llms/ggml_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/hf_llm.py` & `chat_rag-0.1.66/chat_rag/llms/hf_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/mistral_client.py` & `chat_rag-0.1.66/chat_rag/llms/mistral_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/openai_client.py` & `chat_rag-0.1.66/chat_rag/llms/openai_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/llms/vllm_client.py` & `chat_rag-0.1.66/chat_rag/llms/vllm_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/chat_rag/rag.py` & `chat_rag-0.1.66/chat_rag/rag.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.65/pyproject.toml` & `chat_rag-0.1.66/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-rag"
-version = "0.1.65"
+version = "0.1.66"
 description = ""
 authors = ["Diego Peláez Paquico <diego.pelaez@with-madrid.com>"]
 readme = "README.md"
 packages = [{ include = "chat_rag" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chat_rag-0.1.65/PKG-INFO` & `chat_rag-0.1.66/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: chat-rag
-Version: 0.1.65
+Version: 0.1.66
 Summary: 
 Author: Diego Peláez Paquico
 Author-email: diego.pelaez@with-madrid.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: accelerate (>=0.21.0,<0.22.0)
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: anthropic (==0.18.1)
 Requires-Dist: autoawq (==0.1.7)
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: cryptography (>=41.0.4,<42.0.0)
 Requires-Dist: ctransformers (>=0.2.10,<0.3.0)
```

