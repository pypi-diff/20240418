# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.7.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.7.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.8.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.7.tar` & `langchain_nvidia_ai_endpoints-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-04-17 15:51:53.209527 langchain_nvidia_ai_endpoints-0.0.7/LICENSE
--rw-r--r--   0        0        0    10720 2024-04-17 15:51:53.209527 langchain_nvidia_ai_endpoints-0.0.7/README.md
--rw-r--r--   0        0        0     2070 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29740 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     6441 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    16465 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     5442 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0    10047 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2894 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 19:13:25.981102 langchain_nvidia_ai_endpoints-0.0.8/LICENSE
+-rw-r--r--   0        0        0    10720 2024-04-18 19:13:25.981102 langchain_nvidia_ai_endpoints-0.0.8/README.md
+-rw-r--r--   0        0        0     2070 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    29740 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     7056 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    16465 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     5442 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0     5735 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/image_gen.py
+-rw-r--r--   0        0        0     7597 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/llm.py
+-rw-r--r--   0        0        0        0 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0    10047 2024-04-18 19:13:25.985102 langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2894 2024-04-18 19:13:25.989102 langchain_nvidia_ai_endpoints-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.8/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/LICENSE` & `langchain_nvidia_ai_endpoints-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/README.md` & `langchain_nvidia_ai_endpoints-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_common.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_statics.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/_statics.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,14 +114,31 @@
         # 'ai-stable-diffusion-xl-base': {'model_type': 'iamge_out'},
         "ai-codegemma-7b": {"model_type": "chat", "model_name": "google/codegemma-7b"},
         "ai-recurrentgemma-2b": {
             "model_type": "chat",
             "model_name": "google/recurrentgemma-2b",
         },
         "ai-gemma-2b": {"model_type": "chat", "model_name": "google/gemma-2b"},
+        "ai-mistral-large": {
+            "model_type": "chat",
+            "model_name": "mistralai/mistral-large",
+        },
+        "ai-mixtral-8x22b": {
+            "model_type": "completion",
+            "model_name": "mistralai/mixtral-8x22b-v0.1",
+        },
+        "ai-mixtral-8x22b-instruct": {
+            "model_type": "chat",
+            "model_name": "mistralai/mixtral-8x22b-instruct-v0.1",
+        },
+        "ai-llama3-8b": {"model_type": "chat", "model_name": "meta/llama3-8b"},
+        "ai-llama3-70b": {
+            "model_type": "chat",
+            "model_name": "meta/llama3-70b",
+        },
     }
 )
 
 
 MODEL_SPECS.update(
     {
         "babbage-002": {"model_type": "completion"},
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/embeddings.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/image_gen.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/image_gen.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/llm.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/llm.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.0.8/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.7"
+version = "0.0.8"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.7/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.7
+Version: 0.0.8
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

