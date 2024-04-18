# Comparing `tmp/ai_microcore-3.1.0.tar.gz` & `tmp/ai_microcore-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.1.0.tar` & `ai_microcore-3.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.1.0/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.1.0/README.md
--rwxr-xr-x   0        0        0     3708 2024-04-17 18:06:43.438164 ai_microcore-3.1.0/microcore/__init__.py
--rwxr-xr-x   0        0        0     5172 2024-04-16 13:59:44.280985 ai_microcore-3.1.0/microcore/_env.py
--rwxr-xr-x   0        0        0     2984 2023-11-06 21:28:53.896764 ai_microcore-3.1.0/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.1.0/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.1.0/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.1.0/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.1.0/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11345 2024-04-16 14:19:14.188938 ai_microcore-3.1.0/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.1.0/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.1.0/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.1.0/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4732 2024-04-17 18:01:14.743261 ai_microcore-3.1.0/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.1.0/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.1.0/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5078 2024-04-16 09:40:54.280341 ai_microcore-3.1.0/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.1.0/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.1.0/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5773 2024-04-16 09:04:29.140424 ai_microcore-3.1.0/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.1.0/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     2966 2024-04-17 13:18:17.371824 ai_microcore-3.1.0/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.1.0/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.1.0/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.1.0/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.1.0/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.1.0/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.1.0/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.1.0/microcore/types.py
--rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.1.0/microcore/ui.py
--rwxr-xr-x   0        0        0     6834 2024-04-16 23:16:06.885847 ai_microcore-3.1.0/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.1.0/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1167 2024-04-17 17:16:01.701580 ai_microcore-3.1.0/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.1.0/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1287 2023-11-26 19:05:20.640308 ai_microcore-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.2.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.2.0/README.md
+-rwxr-xr-x   0        0        0     3708 2024-04-18 16:18:40.147620 ai_microcore-3.2.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6065 2024-04-18 16:11:44.822923 ai_microcore-3.2.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.2.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.2.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.2.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.2.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.2.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11441 2024-04-18 16:14:59.191428 ai_microcore-3.2.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.2.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.2.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.2.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4743 2024-04-18 13:05:21.878253 ai_microcore-3.2.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.2.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.2.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5086 2024-04-18 13:44:01.397853 ai_microcore-3.2.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.2.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.2.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.2.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.2.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     3052 2024-04-18 13:05:21.887990 ai_microcore-3.2.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.2.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.2.0/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.2.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.2.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.2.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.2.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.2.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.2.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     8169 2024-04-18 13:44:01.426469 ai_microcore-3.2.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.2.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.2.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.2.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.2.0/PKG-INFO
```

### Comparing `ai_microcore-3.1.0/LICENSE` & `ai_microcore-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/README.md` & `ai_microcore-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/__init__.py` & `ai_microcore-3.2.0/microcore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,8 @@
     "utils",
     "configuration",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
```

### Comparing `ai_microcore-3.1.0/microcore/_env.py` & `ai_microcore-3.2.0/microcore/_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, asdict
 from importlib.util import find_spec
 import jinja2
 
 from .configuration import Config, ApiType
 from . import AbstractEmbeddingDB
 from .types import TplFunctionType, LLMAsyncFunctionType, LLMFunctionType
 from .templating.jinja2 import make_jinja2_env, make_tpl_function
@@ -33,31 +33,32 @@
         self.init_similarity_search()
 
     def init_templating(self):
         self.jinja_env = make_jinja2_env(self)
         self.tpl_function = make_tpl_function(self)
 
     def init_llm(self):
-        if self.config.LLM_API_TYPE == ApiType.LOCAL_FUNC:
+        if self.config.LLM_API_TYPE == ApiType.FUNCTION:
             self.llm_function, self.llm_async_function = make_local_llm_functions(
                 self.config
             )
-        elif self.config.LLM_API_TYPE == ApiType.LOCAL_TRANSFORMERS:
+        elif self.config.LLM_API_TYPE == ApiType.TRANSFORMERS:
             try:
                 from .llm.local_transformers import (
                     make_llm_functions as make_transformers_llm_functions,
                 )
             except ModuleNotFoundError as e:
                 raise ModuleNotFoundError(
                     "To use local Transformers language models, "
                     "you need to install the `transformers`, `pytorch` and `accelerate` packages. "
                 ) from e
-            (self.llm_function, self.llm_async_function) = (
-                make_transformers_llm_functions(self.config, self)
-            )
+            (
+                self.llm_function,
+                self.llm_async_function,
+            ) = make_transformers_llm_functions(self.config, self)
         elif self.config.LLM_API_TYPE == ApiType.ANTHROPIC:
             try:
                 from .llm.anthropic import (
                     make_llm_functions as make_anthropic_llm_functions,
                 )
             except ModuleNotFoundError as e:
                 raise ModuleNotFoundError(
@@ -119,14 +120,34 @@
         super().__post_init__()
         Env(self)
 
 
 configure: callable = _Configure
 """Applies configuration to MicroCore environment"""
 
+if True:  # pylint: disable=W0125
+    # This block is inside a condition to avoid breaking IDE autocompletion
+    def _config_builder_wrapper(cfg: Config | dict = None, **kwargs):
+        """
+        - Convert configuration keys to uppercase
+        - Add LLM_ prefix to keys if necessary
+        - Allow to configure from Config instance or dictionary
+        """
+        if cfg:
+            assert not kwargs, "Cannot pass both cfg and kwargs"
+        if isinstance(cfg, dict):
+            return _config_builder_wrapper(**cfg)
+        kwargs = {str(k).upper(): v for k, v in kwargs.items()}
+        for k in list(kwargs.keys()):
+            if not hasattr(Config, k) and hasattr(Config, f"LLM_{k}"):
+                kwargs[f"LLM_{k}"] = kwargs.pop(k)
+        return _Configure(**(cfg and asdict(cfg) or kwargs))
+
+    configure = _config_builder_wrapper
+
 _env: Env | None = None
 
 
 def env() -> Env:
     """Returns the current MicroCore environment"""
     return _env or Env()
```

### Comparing `ai_microcore-3.1.0/microcore/_llm_functions.py` & `ai_microcore-3.2.0/microcore/_llm_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import datetime
+
 from .message_types import Msg
 from .wrappers.llm_response_wrapper import LLMResponse
 from ._env import env
 
 
 def llm(prompt: str | Msg | list[str] | list[Msg], **kwargs) -> str | LLMResponse:
     """
@@ -32,15 +34,20 @@
 
         See fields returned by the OpenAI:
 
         - https://platform.openai.com/docs/api-reference/completions/object
         - https://platform.openai.com/docs/api-reference/chat/object
     """
     [h(prompt, **kwargs) for h in env().llm_before_handlers]
+    start = datetime.now()
     response = env().llm_function(prompt, **kwargs)
+    try:
+        response.gen_duration = (datetime.now() - start).total_seconds()
+    except AttributeError:
+        ...
     [h(response) for h in env().llm_after_handlers]
     return response
 
 
 async def allm(
     prompt: str | Msg | list[str] | list[Msg], **kwargs
 ) -> str | LLMResponse:
@@ -74,10 +81,15 @@
 
         See fields returned by the OpenAI:
 
         - https://platform.openai.com/docs/api-reference/completions/object
         - https://platform.openai.com/docs/api-reference/chat/object
     """
     [h(prompt, **kwargs) for h in env().llm_before_handlers]
+    start = datetime.now()
     response = await env().llm_async_function(prompt, **kwargs)
+    try:
+        response.gen_duration = (datetime.now() - start).total_seconds()
+    except AttributeError:
+        ...
     [h(response) for h in env().llm_after_handlers]
     return response
```

### Comparing `ai_microcore-3.1.0/microcore/_prepare_llm_args.py` & `ai_microcore-3.2.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/ai_func/__init__.py` & `ai_microcore-3.2.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/ai_modules.py` & `ai_microcore-3.2.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/configuration.py` & `ai_microcore-3.2.0/microcore/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,24 +27,30 @@
 
 class ApiType:
     """LLM API types"""
 
     OPEN_AI = "open_ai"
     AZURE = "azure"
     """See https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models"""
-    LOCAL_FUNC = "local"
-    LOCAL_TRANSFORMERS = "local_transformers"
     ANYSCALE = "anyscale"
     """See https://www.anyscale.com/endpoints"""
     DEEP_INFRA = "deep_infra"
     """List of text generation models: https://deepinfra.com/models?type=text-generation"""
     ANTHROPIC = "anthropic"
     GOOGLE_VERTEX_AI = "google_vertex_ai"
     GOOGLE_AI_STUDIO = "google_ai_studio"
 
+    # Local models
+    FUNCTION = "function"
+    TRANSFORMERS = "transformers"
+
+    @staticmethod
+    def is_local(api_type: str) -> bool:
+        return api_type in (ApiType.FUNCTION, ApiType.TRANSFORMERS)
+
 
 _default_dotenv_loaded = False
 
 
 @dataclass
 class BaseConfig:
     """Base class for configuration dataclasses"""
@@ -143,22 +149,22 @@
     """Custom initialization parameters for the model"""
 
     def __post_init__(self):
         super().__post_init__()
         self._init_llm_options()
         self.validate()
 
-    def is_local_llm_used(self) -> bool:
-        return self.LLM_API_TYPE in (ApiType.LOCAL_FUNC, ApiType.LOCAL_TRANSFORMERS)
+    def uses_local_model(self) -> bool:
+        return ApiType.is_local(self.LLM_API_TYPE)
 
     def _init_llm_options(self):
         if self.INFERENCE_FUNC:
             if not self.LLM_API_TYPE:
-                self.LLM_API_TYPE = ApiType.LOCAL_FUNC
-        if self.is_local_llm_used():
+                self.LLM_API_TYPE = ApiType.FUNCTION
+        if self.uses_local_model():
             return
 
         # Use defaults from ENV variables expected by OpenAI API
         self.LLM_API_TYPE = self.LLM_API_TYPE or self.OPENAI_API_TYPE
         if self.GOOGLE_VERTEX_RESPONSE_VALIDATION is None:
             self.GOOGLE_VERTEX_RESPONSE_VALIDATION = get_bool_from_env(
                 "GOOGLE_VERTEX_RESPONSE_VALIDATION", False
@@ -197,42 +203,42 @@
 
     def _validate_local_llm(self):
         if self.CHAT_MODE is None:
             logging.warning(
                 "When using local models, "
                 "(bool)CHAT_MODE configuration option should be explicitly set"
             )
-        if self.LLM_API_TYPE == ApiType.LOCAL_FUNC:
+        if self.LLM_API_TYPE == ApiType.FUNCTION:
             if not self.INFERENCE_FUNC:
                 raise LLMConfigError(
                     "LLM configuration error: "
                     "INFERENCE_FUNC should be provided for local models"
                 )
             if (
                 isinstance(self.INFERENCE_FUNC, str)
                 and self.INFERENCE_FUNC not in globals()
             ):
                 raise LLMConfigError(
                     f"LLM configuration error: inference function '{self.INFERENCE_FUNC}' not found"
                 )
-        elif self.LLM_API_TYPE == ApiType.LOCAL_TRANSFORMERS:
+        elif self.LLM_API_TYPE == ApiType.TRANSFORMERS:
             if not self.MODEL:
                 raise LLMConfigError(
                     "LLM configuration error: "
                     "MODEL should be provided for local transformers models"
                 )
 
     def validate(self):
         """
         Validate LLM configuration
 
         Raises:
             LLMConfigError
         """
-        if self.is_local_llm_used():
+        if self.uses_local_model():
             self._validate_local_llm()
             return
         if self.INFERENCE_FUNC:
             raise LLMConfigError(
                 "LLM configuration error: INFERENCE_FUNC should be provided only for local models"
             )
         if self.LLM_API_TYPE == ApiType.GOOGLE_VERTEX_AI:
```

### Comparing `ai_microcore-3.1.0/microcore/embedding_db/__init__.py` & `ai_microcore-3.2.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/embedding_db/chromadb.py` & `ai_microcore-3.2.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/file_storage.py` & `ai_microcore-3.2.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/json_parsing.py` & `ai_microcore-3.2.0/microcore/json_parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 
 from .types import BadAIJsonAnswer
 
 
 def unwrap_json_substring(
-        input_string: str, allow_in_text: bool = True, return_original_on_fail: bool = True
+    input_string: str, allow_in_text: bool = True, return_original_on_fail: bool = True
 ) -> str:
     input_string = str(input_string).strip()
     if input_string.endswith("```"):
         if input_string.startswith("```json"):
             return input_string[7:-3].strip()
         if input_string.startswith("```"):
             return input_string[3:-3].strip()
@@ -38,17 +38,19 @@
             start = s_start
             end = s_end
             brace = "["
     except ValueError:
         ...
 
     return (
-        input_string[start: end + 1]
+        input_string[start : end + 1]
         if brace
-        else input_string if return_original_on_fail else ""
+        else input_string
+        if return_original_on_fail
+        else ""
     )
 
 
 def fix_json(s: str) -> str:
     """
     Fix internal JSON content
     """
@@ -111,24 +113,24 @@
         s = re.sub(r"\'\s*\:\s*(?=[\'\"])", '": ', s)
         s = re.sub(r"(?<=[\'\"])\s*\:\s*\'", ': "', s)
         return json.dumps(json.loads(s), indent=4)
     except json.JSONDecodeError:
         ...
 
     # incomplete JSON
-    if s.startswith('{') and not s.endswith('}'):
+    if s.startswith("{") and not s.endswith("}"):
         # count number of "
         if s.count('"') % 2 == 1:
             s += '"'
-        s += '}'
+        s += "}"
     return s
 
 
 def parse_json(
-        input_string: str, raise_errors: bool = True, required_fields: list[str] = None
+    input_string: str, raise_errors: bool = True, required_fields: list[str] = None
 ) -> list | dict | float | int | str:
     assert isinstance(required_fields, list) or required_fields is None
     try:
         s = unwrap_json_substring(input_string)
         try:
             res = json.loads(s)
         except json.JSONDecodeError:
```

### Comparing `ai_microcore-3.1.0/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.2.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.2.0/microcore/llm/_openai_llm_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 
 def _prepare_llm_arguments(config: Config, kwargs: dict):
     args = {**config.LLM_DEFAULT_ARGS, **kwargs}
     args["model"] = args.get(
         "model",
         args.get("deployment_id", config.LLM_DEPLOYMENT_ID or config.MODEL)
         if config.LLM_API_TYPE == ApiType.AZURE
-        else config.MODEL
+        else config.MODEL,
     )
     callbacks: list[callable] = args.pop("callbacks", [])
     if "callback" in args:
         cb = args.pop("callback")
         if cb:
             callbacks.append(cb)
     args["stream"] = bool(callbacks)
     return args, {"callbacks": callbacks}
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     if config.LLM_API_TYPE == ApiType.AZURE:
         connection_type = openai.AzureOpenAI
         async_connection_type = openai.AsyncAzureOpenAI
-        params = dict(
-            api_key=config.LLM_API_KEY,
-            azure_endpoint=config.LLM_API_BASE,
-            api_version=config.LLM_API_VERSION,
-            **config.INIT_PARAMS
-        )
+        params = {
+            "api_key": config.LLM_API_KEY,
+            "azure_endpoint": config.LLM_API_BASE,
+            "api_version": config.LLM_API_VERSION,
+            **config.INIT_PARAMS,
+        }
     else:
         connection_type = openai.OpenAI
         async_connection_type = openai.AsyncOpenAI
-        params = dict(
-            api_key=config.LLM_API_KEY,
-            base_url=config.LLM_API_BASE,
-            # **config.INIT_PARAMS
-        )
+        params = {
+            "api_key": config.LLM_API_KEY,
+            "base_url": config.LLM_API_BASE,
+            **config.INIT_PARAMS,
+        }
 
     _connection = connection_type(**params)
     _async_connection = async_connection_type(**params)
 
     async def allm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
         if is_chat_model(args["model"], config):
```

### Comparing `ai_microcore-3.1.0/microcore/llm/anthropic.py` & `ai_microcore-3.2.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/llm/google_genai.py` & `ai_microcore-3.2.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.2.0/microcore/llm/google_vertex_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,21 +55,21 @@
             raise ValueError(
                 "Failed to authenticate with Google Cloud. "
                 "Please make sure you have gcloud installed and configured "
                 "(try `gcloud auth application-default login`; "
                 "`gcloud auth application-default print-access-token`)."
             )
     credentials = Credentials(token=config.GOOGLE_VERTEX_ACCESS_TOKEN)
-    vertexai.init(
+    defaults = dict(
         credentials=credentials,
         project=config.GOOGLE_VERTEX_PROJECT_ID,
         location=config.GOOGLE_VERTEX_LOCATION or None,
         api_endpoint=config.LLM_API_BASE or None,
-        **config.INIT_PARAMS,
     )
+    vertexai.init(**{**defaults, **config.INIT_PARAMS})
 
 
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     init_vertex_ai(config)
     if config.GOOGLE_GEMINI_SAFETY_SETTINGS is None:
         config.GOOGLE_GEMINI_SAFETY_SETTINGS = {
             HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_NONE,
```

### Comparing `ai_microcore-3.1.0/microcore/llm/local_llm.py` & `ai_microcore-3.2.0/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/llm/local_transformers.py` & `ai_microcore-3.2.0/microcore/llm/local_transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,25 +30,28 @@
         gc.collect()
         torch.cuda.empty_cache()
         model_config = transformers.AutoConfig.from_pretrained(
             config.MODEL,
             trust_remote_code=True,
         )
         mc_param_names = ["model", "tokenizer", "device", "quantize_4bit", "inference"]
-        model_init_params = dict(
+        model_init_params = {
             **dict(
                 trust_remote_code=True,
                 torch_dtype="auto",
                 config=model_config,
                 device_map="auto",
                 offload_folder=config.STORAGE_PATH,
             ),
             **{k: v for k, v in params.items() if k not in mc_param_names},
-        )
-        if params.get("quantize_4bit"):
+        }
+        if (
+            params.get("quantize_4bit")
+            and "quantization_config" not in model_init_params
+        ):
             model_init_params["quantization_config"] = transformers.BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_quant_type="nf4",
                 bnb_4bit_compute_dtype=torch.bfloat16,
                 bnb_4bit_use_double_quant=True,
             )
```

### Comparing `ai_microcore-3.1.0/microcore/logging.py` & `ai_microcore-3.2.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/message_types.py` & `ai_microcore-3.2.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/templating/jinja2.py` & `ai_microcore-3.2.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.2.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/types.py` & `ai_microcore-3.2.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/ui.py` & `ai_microcore-3.2.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.1.0/microcore/utils.py` & `ai_microcore-3.2.0/microcore/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import os
 import sys
 import re
 import subprocess
 from dataclasses import dataclass
 from fnmatch import fnmatch
 from pathlib import Path
+from typing import Any
+
 from colorama import Fore
 
 from .configuration import Config
 from .types import BadAIAnswer
 from .message_types import UserMsg, SysMsg, AssistantMsg
 
 
@@ -210,7 +212,49 @@
     except subprocess.CalledProcessError:
         msg = "No GPU found or nvidia-smi is not installed"
         return f"{Fore.RED}{msg}{Fore.RESET}" if as_string else None
 
 
 def show_vram_usage():
     print(get_vram_usage(as_string=True))
+
+
+def return_default(default, *args):
+    if isinstance(default, type) and issubclass(default, BaseException):
+        raise default()
+    if isinstance(default, BaseException):
+        raise default
+    if inspect.isbuiltin(default):
+        return default(*args)
+    if inspect.isfunction(default):
+        arg_count = default.__code__.co_argcount
+        if inspect.ismethod(default):
+            arg_count -= 1
+        return default(*args) if arg_count >= len(args) else default()
+
+    return default
+
+
+def extract_number(
+    text: str,
+    default=None,
+    position="last",
+    dtype: type | str = float,
+    rounding: bool = False,
+) -> int | float | Any:
+    assert position in ["last", "first"], f"Invalid position: {position}"
+    idx = {"last": -1, "first": 0}[position]
+
+    dtype = {"int": int, "float": float}.get(dtype, dtype)
+    assert dtype in [int, float], f"Invalid dtype: {dtype}"
+    if rounding:
+        dtype = float
+    regex = {int: r"[-+]?\d+", float: r"[-+]?\d*\.?\d+"}[dtype]
+
+    numbers = re.findall(regex, str(text))
+    if numbers:
+        try:
+            value = dtype(numbers[idx].strip())
+            return round(value) if rounding else value
+        except ValueError:
+            ...
+    return return_default(default, text)
```

### Comparing `ai_microcore-3.1.0/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.2.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Any
+
+from ..types import BadAIAnswer
 from ..json_parsing import parse_json
-from ..utils import ExtendedString, ConvertableToMessage
+from ..utils import ExtendedString, ConvertableToMessage, extract_number
 from ..message_types import Role, AssistantMsg
 
 
 class LLMResponse(ExtendedString, ConvertableToMessage):
     """
     Response from the Large Language Model.
 
@@ -14,20 +17,32 @@
     See fields returned by the OpenAI:
 
     - https://platform.openai.com/docs/api-reference/completions/object
     - https://platform.openai.com/docs/api-reference/chat/object
     """
 
     def __new__(cls, string: str, attrs: dict = None):
+        attrs = {
+            "role": Role.ASSISTANT,
+            "content": str(string),
+            "gen_duration": None,
+            **(attrs or {}),
+        }
         obj = ExtendedString.__new__(cls, string, attrs)
-        # Same fields like in Msg
-        setattr(obj, "role", Role.ASSISTANT)
-        setattr(obj, "content", str(string))
         return obj
 
     def parse_json(
         self, raise_errors: bool = True, required_fields: list[str] = None
     ) -> list | dict | float | int | str:
         return parse_json(self.content, raise_errors, required_fields)
 
+    def parse_number(
+        self,
+        default=BadAIAnswer,
+        position="last",
+        dtype: type | str = float,
+        rounding: bool = False,
+    ) -> int | float | Any:
+        return extract_number(self.content, default, position, dtype, rounding)
+
     def as_message(self) -> AssistantMsg:
         return self.as_assistant
```

### Comparing `ai_microcore-3.1.0/pyproject.toml` & `ai_microcore-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -42,8 +42,12 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 #addopts = "--cov=microcore --cov-report=xml:coverage.xml --cov-report=term"
 addopts = "-vv --capture=no --log-cli-level=INFO"
 testpaths = [
     "tests/basic",
+]
+filterwarnings = [
+    "ignore:Deprecated call to `pkg_resources\\.declare_namespace\\('.*'\\):DeprecationWarning",
+    "ignore::DeprecationWarning:google.rpc",
 ]
```

### Comparing `ai_microcore-3.1.0/PKG-INFO` & `ai_microcore-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.1.0
+Version: 3.2.0
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.1.0 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.2.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

