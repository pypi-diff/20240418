# Comparing `tmp/codelinker-0.1.3.tar.gz` & `tmp/codelinker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelinker-0.1.3.tar", max compression
+gzip compressed data, was "codelinker-0.1.4.tar", max compression
```

## Comparing `codelinker-0.1.3.tar` & `codelinker-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-17 07:20:29.996021 codelinker-0.1.3/LICENSE
--rw-r--r--   0        0        0     1968 2024-04-17 07:20:29.996021 codelinker-0.1.3/README.md
--rw-r--r--   0        0        0     1584 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/__init__.py
--rw-r--r--   0        0        0     3249 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/config.py
--rw-r--r--   0        0        0     8412 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/linker.py
--rw-r--r--   0        0        0       64 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/__init__.py
--rw-r--r--   0        0        0      273 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/labels.py
--rw-r--r--   0        0        0      308 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/models/structuredRet.py
--rw-r--r--   0        0        0       32 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/__init__.py
--rw-r--r--   0        0        0    11665 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/objGen.py
--rw-r--r--   0        0        0     5086 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/request/openai.py
--rw-r--r--   0        0        0     1510 2024-04-17 07:20:29.996021 codelinker-0.1.3/codelinker/utils.py
--rw-r--r--   0        0        0      359 2024-04-17 07:20:29.996021 codelinker-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 08:28:07.884080 codelinker-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-18 08:28:07.884080 codelinker-0.1.4/README.md
+-rw-r--r--   0        0        0     1584 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/__init__.py
+-rw-r--r--   0        0        0     3392 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/config.py
+-rw-r--r--   0        0        0     8412 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/linker.py
+-rw-r--r--   0        0        0       64 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/labels.py
+-rw-r--r--   0        0        0      308 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/structuredRet.py
+-rw-r--r--   0        0        0       32 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/__init__.py
+-rw-r--r--   0        0        0    12268 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/objGen.py
+-rw-r--r--   0        0        0     5086 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/openai.py
+-rw-r--r--   0        0        0     1510 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/utils.py
+-rw-r--r--   0        0        0      359 2024-04-18 08:28:07.884080 codelinker-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.4/PKG-INFO
```

### Comparing `codelinker-0.1.3/LICENSE` & `codelinker-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/README.md` & `codelinker-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/codelinker/__init__.py` & `codelinker-0.1.4/codelinker/__init__.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/codelinker/config.py` & `codelinker-0.1.4/codelinker/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         req_name_mapping: dict[str, str] = {
             "gpt-4v": "gpt-4-vision",
             "gpt4": "gpt-4",
             "gpt4-32": "gpt-4-32k",
             "gpt-35-16k": "gpt-3.5-turbo-16k",
         }
 
+        save_completion: bool = False
+        # default to save in current working directory 
+        save_completion_path: str = os.getcwd()
+
     request: RequestConfig = RequestConfig()
     
     class ExectionConfig(BaseModel):
         max_ai_functions_tokens: int = 12800
         max_message_tokens: int = 15872
 
     execution: ExectionConfig = ExectionConfig()
```

### Comparing `codelinker-0.1.3/codelinker/linker.py` & `codelinker-0.1.4/codelinker/linker.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/codelinker/request/objGen.py` & `codelinker-0.1.4/codelinker/request/objGen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import os
 import json
+import uuid
+import datetime
 import jsonschema
 import jsonschema.exceptions
 import importlib
 
 from typing import Literal
 from copy import deepcopy
 from tenacity import AsyncRetrying, RetryError, stop_after_attempt
@@ -131,14 +134,23 @@
 
         rets = []
 
         try:
             async for attempt in AsyncRetrying(stop=stop_after_attempt(max_retry_times), reraise=True):
                 with attempt:
                     response = await self._chatcompletion_request(**kwargs)
+                    if self.config.request.save_completion:
+                        with open(os.path.join(self.config.request.save_completion_path,
+                                               datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f")+f"{uuid.uuid4().hex}.json"
+                                               ), 'w') as f:
+                            f.write(json.dumps({
+                                "request": kwargs,
+                                "response": response
+                                }, indent=4))
+                        
                     for choice in response["choices"]:
                         structuredRets = []
                         for tool_call in choice["message"]["tool_calls"]:
                             if tool_call["type"] != "function":
                                 continue
 
                             if schema_validation and self.config.request.schema_validation:
```

### Comparing `codelinker-0.1.3/codelinker/request/openai.py` & `codelinker-0.1.4/codelinker/request/openai.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/codelinker/utils.py` & `codelinker-0.1.4/codelinker/utils.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.3/PKG-INFO` & `codelinker-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelinker
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: luyaxi
 Author-email: luyaxi@live.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

