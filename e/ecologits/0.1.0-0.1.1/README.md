# Comparing `tmp/ecologits-0.1.0.tar.gz` & `tmp/ecologits-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecologits-0.1.0.tar", max compression
+gzip compressed data, was "ecologits-0.1.1.tar", max compression
```

## Comparing `ecologits-0.1.0.tar` & `ecologits-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16725 2024-04-18 17:18:16.224451 ecologits-0.1.0/LICENSE
--rw-r--r--   0        0        0     1312 2024-04-18 17:18:16.224451 ecologits-0.1.0/README.md
--rw-r--r--   0        0        0       58 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/__init__.py
--rw-r--r--   0        0        0     5763 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/data/models.csv
--rw-r--r--   0        0        0     1806 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/ecologits.py
--rw-r--r--   0        0        0      140 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/exceptions.py
--rw-r--r--   0        0        0      121 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/impacts/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-18 17:18:16.224451 ecologits-0.1.0/ecologits/impacts/dag.py
--rw-r--r--   0        0        0     7605 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/impacts/llm.py
--rw-r--r--   0        0        0     1458 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/impacts/models.py
--rw-r--r--   0        0        0     2992 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/model_repository.py
--rw-r--r--   0        0        0        0 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/__init__.py
--rw-r--r--   0        0        0     7848 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/anthropic_tracer.py
--rw-r--r--   0        0        0     5094 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/cohere_tracer.py
--rw-r--r--   0        0        0     5504 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/huggingface_tracer.py
--rw-r--r--   0        0        0     5065 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/mistralai_tracer.py
--rw-r--r--   0        0        0     5313 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/openai_tracer.py
--rw-r--r--   0        0        0     1139 2024-04-18 17:18:16.228451 ecologits-0.1.0/ecologits/tracers/utils.py
--rw-r--r--   0        0        0     3381 2024-04-18 17:18:16.228451 ecologits-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 ecologits-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-18 17:48:51.396998 ecologits-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1312 2024-04-18 17:48:51.396998 ecologits-0.1.1/README.md
+-rw-r--r--   0        0        0       58 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/__init__.py
+-rw-r--r--   0        0        0     5763 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/data/models.csv
+-rw-r--r--   0        0        0     1712 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/ecologits.py
+-rw-r--r--   0        0        0      140 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/exceptions.py
+-rw-r--r--   0        0        0      121 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/impacts/__init__.py
+-rw-r--r--   0        0        0     1468 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/impacts/dag.py
+-rw-r--r--   0        0        0     7605 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/impacts/llm.py
+-rw-r--r--   0        0        0     1458 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/impacts/models.py
+-rw-r--r--   0        0        0     2992 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/model_repository.py
+-rw-r--r--   0        0        0        0 2024-04-18 17:48:51.396998 ecologits-0.1.1/ecologits/tracers/__init__.py
+-rw-r--r--   0        0        0     7848 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/anthropic_tracer.py
+-rw-r--r--   0        0        0     5094 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/cohere_tracer.py
+-rw-r--r--   0        0        0     5554 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/huggingface_tracer.py
+-rw-r--r--   0        0        0     5065 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/mistralai_tracer.py
+-rw-r--r--   0        0        0     5313 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/openai_tracer.py
+-rw-r--r--   0        0        0     1139 2024-04-18 17:48:51.400998 ecologits-0.1.1/ecologits/tracers/utils.py
+-rw-r--r--   0        0        0     3381 2024-04-18 17:48:51.400998 ecologits-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 ecologits-0.1.1/PKG-INFO
```

### Comparing `ecologits-0.1.0/LICENSE` & `ecologits-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/README.md` & `ecologits-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/data/models.csv` & `ecologits-0.1.1/ecologits/data/models.csv`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/ecologits.py` & `ecologits-0.1.1/ecologits/ecologits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import importlib.util
 
-from ecologits.exceptions import TracerInitializationError
-
 
 class EcoLogits:
     initialized = False
 
     @staticmethod
     def init() -> None:
-        if EcoLogits.initialized:
-            raise TracerInitializationError()
-        init_instruments()
-        EcoLogits.initialized = True
+        if not EcoLogits.initialized:
+            init_instruments()
+            EcoLogits.initialized = True
 
 
 def init_instruments() -> None:
     init_openai_instrumentor()
     init_anthropic_instrumentor()
     init_mistralai_instrumentor()
     init_huggingface_instrumentor()
```

### Comparing `ecologits-0.1.0/ecologits/impacts/dag.py` & `ecologits-0.1.1/ecologits/impacts/dag.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/impacts/llm.py` & `ecologits-0.1.1/ecologits/impacts/llm.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/impacts/models.py` & `ecologits-0.1.1/ecologits/impacts/models.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/model_repository.py` & `ecologits-0.1.1/ecologits/model_repository.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/tracers/anthropic_tracer.py` & `ecologits-0.1.1/ecologits/tracers/anthropic_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/tracers/cohere_tracer.py` & `ecologits-0.1.1/ecologits/tracers/cohere_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/tracers/huggingface_tracer.py` & `ecologits-0.1.1/ecologits/tracers/huggingface_tracer.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,22 @@
     import tiktoken
     from huggingface_hub import AsyncInferenceClient, InferenceClient
     from huggingface_hub import ChatCompletionOutput as _ChatCompletionOutput
     from huggingface_hub import ChatCompletionStreamOutput as _ChatCompletionStreamOutput
 except ImportError:
     InferenceClient = object()
     AsyncInferenceClient = object()
-    _ChatCompletionOutput = object()
-    _ChatCompletionStreamOutput = object()
+
+    @dataclass
+    class _ChatCompletionOutput:
+        pass
+
+    @dataclass
+    class _ChatCompletionStreamOutput:
+        pass
 
 
 PROVIDER = "huggingface_hub"
 
 
 @dataclass
 class ChatCompletionOutput(_ChatCompletionOutput):
```

### Comparing `ecologits-0.1.0/ecologits/tracers/mistralai_tracer.py` & `ecologits-0.1.1/ecologits/tracers/mistralai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/tracers/openai_tracer.py` & `ecologits-0.1.1/ecologits/tracers/openai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/ecologits/tracers/utils.py` & `ecologits-0.1.1/ecologits/tracers/utils.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.0/pyproject.toml` & `ecologits-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecologits"
-version = "0.1.0"
+version = "0.1.1"
 description = "EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs."
 authors = [
     "GenAI Impact",
     "Data For Good"
 ]
 maintainers = [
     "GenAI Impact"
```

### Comparing `ecologits-0.1.0/PKG-INFO` & `ecologits-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecologits
-Version: 0.1.0
+Version: 0.1.1
 Summary: EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs.
 Home-page: https://github.com/genai-impact/ecologits
 License: MPL-2.0
 Author: GenAI Impact
 Maintainer: GenAI Impact
 Requires-Python: >=3.9,<4
 Classifier: Intended Audience :: Developers
```

