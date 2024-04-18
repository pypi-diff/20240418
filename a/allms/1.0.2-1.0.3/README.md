# Comparing `tmp/allms-1.0.2.tar.gz` & `tmp/allms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allms-1.0.2.tar", max compression
+gzip compressed data, was "allms-1.0.3.tar", max compression
```

## Comparing `allms-1.0.2.tar` & `allms-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2024-03-22 14:30:46.478972 allms-1.0.2/LICENSE
--rw-r--r--   0        0        0     8996 2024-03-22 14:30:46.478972 allms-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/chains/__init__.py
--rw-r--r--   0        0        0     4864 2024-03-22 14:30:46.478972 allms-1.0.2/allms/chains/long_text_processing_chain.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/constants/__init__.py
--rw-r--r--   0        0        0      575 2024-03-22 14:30:46.478972 allms-1.0.2/allms/constants/azure.py
--rw-r--r--   0        0        0      877 2024-03-22 14:30:46.478972 allms-1.0.2/allms/constants/input_data.py
--rw-r--r--   0        0        0      258 2024-03-22 14:30:46.478972 allms-1.0.2/allms/constants/prompt.py
--rw-r--r--   0        0        0      270 2024-03-22 14:30:46.478972 allms-1.0.2/allms/constants/vertex_ai.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/defaults/__init__.py
--rw-r--r--   0        0        0      666 2024-03-22 14:30:46.478972 allms-1.0.2/allms/defaults/azure_defaults.py
--rw-r--r--   0        0        0      117 2024-03-22 14:30:46.478972 allms-1.0.2/allms/defaults/general_defaults.py
--rw-r--r--   0        0        0      469 2024-03-22 14:30:46.478972 allms-1.0.2/allms/defaults/long_text_chain.py
--rw-r--r--   0        0        0      676 2024-03-22 14:30:46.478972 allms-1.0.2/allms/defaults/vertex_ai.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/__init__.py
--rw-r--r--   0        0        0      471 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/configuration.py
--rw-r--r--   0        0        0      777 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/enumerables.py
--rw-r--r--   0        0        0      229 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/input_data.py
--rw-r--r--   0        0        0      444 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/prompt_dto.py
--rw-r--r--   0        0        0      726 2024-03-22 14:30:46.478972 allms-1.0.2/allms/domain/response.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/exceptions/__init__.py
--rw-r--r--   0        0        0     1548 2024-03-22 14:30:46.478972 allms-1.0.2/allms/exceptions/validation_input_data_exceptions.py
--rw-r--r--   0        0        0     1134 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/__init__.py
--rw-r--r--   0        0        0    16372 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/abstract.py
--rw-r--r--   0        0        0      935 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/azure_base.py
--rw-r--r--   0        0        0     2247 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/azure_llama2.py
--rw-r--r--   0        0        0     2170 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/azure_mistral.py
--rw-r--r--   0        0        0     1840 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/azure_openai.py
--rw-r--r--   0        0        0     3894 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/vertexai_base.py
--rw-r--r--   0        0        0     1965 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/vertexai_gemini.py
--rw-r--r--   0        0        0     2128 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/vertexai_gemma.py
--rw-r--r--   0        0        0     1947 2024-03-22 14:30:46.478972 allms-1.0.2/allms/models/vertexai_palm.py
--rw-r--r--   0        0        0        0 2024-03-22 14:30:46.478972 allms-1.0.2/allms/utils/__init__.py
--rw-r--r--   0        0        0     1256 2024-03-22 14:30:46.478972 allms-1.0.2/allms/utils/io_utils.py
--rw-r--r--   0        0        0      291 2024-03-22 14:30:46.478972 allms-1.0.2/allms/utils/logger_utils.py
--rw-r--r--   0        0        0     4839 2024-03-22 14:30:46.478972 allms-1.0.2/allms/utils/long_text_processing_utils.py
--rw-r--r--   0        0        0     2607 2024-03-22 14:30:46.478972 allms-1.0.2/allms/utils/response_parsing_utils.py
--rw-r--r--   0        0        0      663 2024-03-22 14:30:46.482972 allms-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9825 1970-01-01 00:00:00.000000 allms-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 13:17:53.931928 allms-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8996 2024-04-18 13:17:53.931928 allms-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/chains/__init__.py
+-rw-r--r--   0        0        0     4864 2024-04-18 13:17:53.931928 allms-1.0.3/allms/chains/long_text_processing_chain.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/azure.py
+-rw-r--r--   0        0        0      877 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/input_data.py
+-rw-r--r--   0        0        0      258 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/prompt.py
+-rw-r--r--   0        0        0      270 2024-04-18 13:17:53.931928 allms-1.0.3/allms/constants/vertex_ai.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/azure_defaults.py
+-rw-r--r--   0        0        0      117 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/general_defaults.py
+-rw-r--r--   0        0        0      469 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/long_text_chain.py
+-rw-r--r--   0        0        0      676 2024-04-18 13:17:53.931928 allms-1.0.3/allms/defaults/vertex_ai.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/configuration.py
+-rw-r--r--   0        0        0      777 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/enumerables.py
+-rw-r--r--   0        0        0      229 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/input_data.py
+-rw-r--r--   0        0        0      444 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/prompt_dto.py
+-rw-r--r--   0        0        0      726 2024-04-18 13:17:53.931928 allms-1.0.3/allms/domain/response.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/exceptions/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-18 13:17:53.931928 allms-1.0.3/allms/exceptions/validation_input_data_exceptions.py
+-rw-r--r--   0        0        0     1134 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/__init__.py
+-rw-r--r--   0        0        0    16564 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/abstract.py
+-rw-r--r--   0        0        0      935 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_base.py
+-rw-r--r--   0        0        0     2247 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_llama2.py
+-rw-r--r--   0        0        0     2170 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_mistral.py
+-rw-r--r--   0        0        0     1840 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/azure_openai.py
+-rw-r--r--   0        0        0     3894 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_base.py
+-rw-r--r--   0        0        0     1965 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_gemini.py
+-rw-r--r--   0        0        0     2128 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_gemma.py
+-rw-r--r--   0        0        0     1947 2024-04-18 13:17:53.931928 allms-1.0.3/allms/models/vertexai_palm.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/io_utils.py
+-rw-r--r--   0        0        0      291 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/logger_utils.py
+-rw-r--r--   0        0        0     4839 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/long_text_processing_utils.py
+-rw-r--r--   0        0        0     2607 2024-04-18 13:17:53.931928 allms-1.0.3/allms/utils/response_parsing_utils.py
+-rw-r--r--   0        0        0      663 2024-04-18 13:17:53.935928 allms-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9825 1970-01-01 00:00:00.000000 allms-1.0.3/PKG-INFO
```

### Comparing `allms-1.0.2/LICENSE` & `allms-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/README.md` & `allms-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/chains/long_text_processing_chain.py` & `allms-1.0.3/allms/chains/long_text_processing_chain.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/constants/azure.py` & `allms-1.0.3/allms/constants/azure.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/constants/input_data.py` & `allms-1.0.3/allms/constants/input_data.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/defaults/azure_defaults.py` & `allms-1.0.3/allms/defaults/azure_defaults.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/defaults/vertex_ai.py` & `allms-1.0.3/allms/defaults/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/domain/enumerables.py` & `allms-1.0.3/allms/domain/enumerables.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/domain/response.py` & `allms-1.0.3/allms/domain/response.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/exceptions/validation_input_data_exceptions.py` & `allms-1.0.3/allms/exceptions/validation_input_data_exceptions.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/__init__.py` & `allms-1.0.3/allms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/abstract.py` & `allms-1.0.3/allms/models/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,22 @@
         self._json_pattern = re.compile(r"{.*?}", re.DOTALL)
         self._is_json_format_injected_into_prompt: bool = True
 
         if max_output_tokens >= model_total_max_tokens:
             raise ValueError("max_output_tokens has to be lower than model_total_max_tokens")
 
         self._llm = self._create_llm()
-        self._event_loop = event_loop if event_loop is not None else asyncio.get_event_loop()
+
+        if not event_loop:
+            try:
+                event_loop = asyncio.get_running_loop()
+            except RuntimeError as error:
+                event_loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(event_loop)
+        self._event_loop = event_loop
 
         self._predict_example = create_base_retry_decorator(
             error_types=[
                 openai.error.RateLimitError, openai.error.APIError, openai.error.Timeout,
                 openai.error.APIConnectionError, openai.error.ServiceUnavailableError,
                 google.api_core.exceptions.ResourceExhausted, urllib.error.HTTPError
             ],
```

### Comparing `allms-1.0.2/allms/models/azure_base.py` & `allms-1.0.3/allms/models/azure_base.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/azure_llama2.py` & `allms-1.0.3/allms/models/azure_llama2.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/azure_mistral.py` & `allms-1.0.3/allms/models/azure_mistral.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/azure_openai.py` & `allms-1.0.3/allms/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/vertexai_base.py` & `allms-1.0.3/allms/models/vertexai_base.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/vertexai_gemini.py` & `allms-1.0.3/allms/models/vertexai_gemini.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/vertexai_gemma.py` & `allms-1.0.3/allms/models/vertexai_gemma.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/models/vertexai_palm.py` & `allms-1.0.3/allms/models/vertexai_palm.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/utils/io_utils.py` & `allms-1.0.3/allms/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/utils/long_text_processing_utils.py` & `allms-1.0.3/allms/utils/long_text_processing_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/allms/utils/response_parsing_utils.py` & `allms-1.0.3/allms/utils/response_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `allms-1.0.2/PKG-INFO` & `allms-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allms
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Allegro Opensource
 Author-email: opensource@allegro.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

