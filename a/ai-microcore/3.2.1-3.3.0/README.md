# Comparing `tmp/ai_microcore-3.2.1.tar.gz` & `tmp/ai_microcore-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.2.1.tar` & `ai_microcore-3.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.2.1/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.2.1/README.md
--rwxr-xr-x   0        0        0     3708 2024-04-18 16:31:15.569589 ai_microcore-3.2.1/microcore/__init__.py
--rwxr-xr-x   0        0        0     6065 2024-04-18 16:11:44.822923 ai_microcore-3.2.1/microcore/_env.py
--rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.2.1/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.2.1/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.2.1/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.2.1/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.2.1/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    11541 2024-04-18 16:30:03.398309 ai_microcore-3.2.1/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.2.1/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.2.1/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.2.1/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4743 2024-04-18 13:05:21.878253 ai_microcore-3.2.1/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.2.1/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.2.1/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5086 2024-04-18 13:44:01.397853 ai_microcore-3.2.1/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.2.1/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.2.1/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.2.1/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.2.1/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     3052 2024-04-18 13:05:21.887990 ai_microcore-3.2.1/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.2.1/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.2.1/microcore/logging.py
--rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.2.1/microcore/message_types.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.2.1/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.2.1/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.2.1/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.2.1/microcore/types.py
--rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.2.1/microcore/ui.py
--rwxr-xr-x   0        0        0     8169 2024-04-18 13:44:01.426469 ai_microcore-3.2.1/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.2.1/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.2.1/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.2.1/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.3.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.3.0/README.md
+-rwxr-xr-x   0        0        0     3819 2024-04-18 17:17:10.357827 ai_microcore-3.3.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     6065 2024-04-18 16:11:44.822923 ai_microcore-3.3.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3311 2024-04-18 13:13:30.363208 ai_microcore-3.3.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      770 2024-03-08 01:17:33.018421 ai_microcore-3.3.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.3.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.3.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.3.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    11541 2024-04-18 16:30:03.398309 ai_microcore-3.3.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.3.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.3.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8369 2024-03-08 00:49:49.038994 ai_microcore-3.3.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4743 2024-04-18 13:05:21.878253 ai_microcore-3.3.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.3.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.3.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5086 2024-04-18 13:44:01.397853 ai_microcore-3.3.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.3.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.3.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.3.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3229 2024-04-16 14:08:39.822867 ai_microcore-3.3.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0     3052 2024-04-18 13:05:21.887990 ai_microcore-3.3.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.3.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2466 2024-04-16 08:13:17.036046 ai_microcore-3.3.0/microcore/logging.py
+-rwxr-xr-x   0        0        0      642 2024-03-08 00:49:48.881046 ai_microcore-3.3.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.3.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.3.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.3.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.3.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1535 2024-03-31 01:09:15.567119 ai_microcore-3.3.0/microcore/ui.py
+-rwxr-xr-x   0        0        0     8730 2024-04-18 17:10:16.647260 ai_microcore-3.3.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.3.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.3.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.3.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.3.0/PKG-INFO
```

### Comparing `ai_microcore-3.2.1/LICENSE` & `ai_microcore-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/README.md` & `ai_microcore-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/__init__.py` & `ai_microcore-3.3.0/microcore/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 from .logging import use_logging
 from .message_types import UserMsg, AssistantMsg, SysMsg, Msg
 from .configuration import ApiType, LLMConfigError
 from .types import BadAIJsonAnswer, BadAIAnswer
 from .wrappers.prompt_wrapper import PromptWrapper
 from .wrappers.llm_response_wrapper import LLMResponse
 from ._llm_functions import llm, allm
-from .utils import parse
+from .utils import parse, dedent
 
 
 def tpl(file: os.PathLike[str] | str, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template using the provided parameters."""
     return PromptWrapper(env().tpl_function(file, **kwargs))
 
 
-def prompt(template_str: str, **kwargs) -> str | PromptWrapper:
+def prompt(template_str: str, remove_indent=True, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template from string using the provided parameters."""
+    if remove_indent:
+        template_str = dedent(template_str)
     return PromptWrapper(env().jinja_env.from_string(template_str).render(**kwargs))
 
 
 def use_model(name: str):
     """Switches language model"""
     config().MODEL = name
     config().LLM_DEFAULT_ARGS["model"] = name
@@ -112,19 +114,20 @@
     "ApiType",
     "BadAIJsonAnswer",
     "BadAIAnswer",
     "LLMConfigError",
     "LLMResponse",
     "PromptWrapper",
     "parse",
+    "dedent",
     # submodules
     "embedding_db",
     "file_storage",
     "message_types",
     "utils",
     "configuration",
     "types",
     "ui",
     # "wrappers",
 ]
 
-__version__ = "3.2.1"
+__version__ = "3.3.0"
```

### Comparing `ai_microcore-3.2.1/microcore/_env.py` & `ai_microcore-3.3.0/microcore/_env.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/_llm_functions.py` & `ai_microcore-3.3.0/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/_prepare_llm_args.py` & `ai_microcore-3.3.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/ai_func/__init__.py` & `ai_microcore-3.3.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/ai_modules.py` & `ai_microcore-3.3.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/configuration.py` & `ai_microcore-3.3.0/microcore/configuration.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/embedding_db/__init__.py` & `ai_microcore-3.3.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/embedding_db/chromadb.py` & `ai_microcore-3.3.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/file_storage.py` & `ai_microcore-3.3.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/json_parsing.py` & `ai_microcore-3.3.0/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.3.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.3.0/microcore/llm/_openai_llm_v1.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/anthropic.py` & `ai_microcore-3.3.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/google_genai.py` & `ai_microcore-3.3.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.3.0/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/local_llm.py` & `ai_microcore-3.3.0/microcore/llm/local_llm.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/llm/local_transformers.py` & `ai_microcore-3.3.0/microcore/llm/local_transformers.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/logging.py` & `ai_microcore-3.3.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/message_types.py` & `ai_microcore-3.3.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/templating/jinja2.py` & `ai_microcore-3.3.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.3.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/types.py` & `ai_microcore-3.3.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/ui.py` & `ai_microcore-3.3.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/microcore/utils.py` & `ai_microcore-3.3.0/microcore/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -254,7 +254,22 @@
     if numbers:
         try:
             value = dtype(numbers[idx].strip())
             return round(value) if rounding else value
         except ValueError:
             ...
     return return_default(default, text)
+
+def dedent(text: str):
+    lines = text.splitlines()
+    while lines and lines[0].strip() == '':
+        lines.pop(0)
+    while lines and lines[-1].strip() == '':
+        lines.pop()
+    non_empty_lines = [line for line in lines if line.strip()]
+    if non_empty_lines:
+        min_indent = min((len(line) - len(line.lstrip())) for line in non_empty_lines)
+        dedented_lines = [line[min_indent:] if line and len(line) >= min_indent else line for line in lines]
+    else:
+        dedented_lines = lines
+    return '\n'.join(dedented_lines)
+
```

### Comparing `ai_microcore-3.2.1/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.3.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/pyproject.toml` & `ai_microcore-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.2.1/PKG-INFO` & `ai_microcore-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.2.1
+Version: 3.3.0
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
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.2.1 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.3.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

