# Comparing `tmp/codelinker-0.1.5.tar.gz` & `tmp/codelinker-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelinker-0.1.5.tar", max compression
+gzip compressed data, was "codelinker-0.1.6.tar", max compression
```

## Comparing `codelinker-0.1.5.tar` & `codelinker-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-18 08:31:55.590747 codelinker-0.1.5/LICENSE
--rw-r--r--   0        0        0     1968 2024-04-18 08:31:55.590747 codelinker-0.1.5/README.md
--rw-r--r--   0        0        0     1584 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/__init__.py
--rw-r--r--   0        0        0     3430 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/config.py
--rw-r--r--   0        0        0     8412 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/linker.py
--rw-r--r--   0        0        0       64 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/__init__.py
--rw-r--r--   0        0        0      273 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/labels.py
--rw-r--r--   0        0        0      308 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/structuredRet.py
--rw-r--r--   0        0        0       32 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/__init__.py
--rw-r--r--   0        0        0    12364 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/objGen.py
--rw-r--r--   0        0        0     5086 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/openai.py
--rw-r--r--   0        0        0     1510 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/utils.py
--rw-r--r--   0        0        0      359 2024-04-18 08:31:55.594747 codelinker-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 14:31:30.269408 codelinker-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-18 14:31:30.269408 codelinker-0.1.6/README.md
+-rw-r--r--   0        0        0     1584 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/__init__.py
+-rw-r--r--   0        0        0     3430 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/config.py
+-rw-r--r--   0        0        0     8412 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/linker.py
+-rw-r--r--   0        0        0       64 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/models/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/models/labels.py
+-rw-r--r--   0        0        0      308 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/models/structuredRet.py
+-rw-r--r--   0        0        0       32 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/request/__init__.py
+-rw-r--r--   0        0        0    12481 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/request/objGen.py
+-rw-r--r--   0        0        0     5086 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/request/openai.py
+-rw-r--r--   0        0        0     1510 2024-04-18 14:31:30.269408 codelinker-0.1.6/codelinker/utils.py
+-rw-r--r--   0        0        0      359 2024-04-18 14:31:30.269408 codelinker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.6/PKG-INFO
```

### Comparing `codelinker-0.1.5/LICENSE` & `codelinker-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/README.md` & `codelinker-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/codelinker/__init__.py` & `codelinker-0.1.6/codelinker/__init__.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/codelinker/config.py` & `codelinker-0.1.6/codelinker/config.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/codelinker/linker.py` & `codelinker-0.1.6/codelinker/linker.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/codelinker/request/objGen.py` & `codelinker-0.1.6/codelinker/request/objGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Literal
 from copy import deepcopy
 from tenacity import AsyncRetrying, RetryError, stop_after_attempt
 from logging import Logger
 
 from ..models import StructuredRet, StructureSchema
 from ..config import CodeLinkerConfig
-
+from ..utils import clip_text
 
 class OBJGenerator:
     def __init__(self, config: CodeLinkerConfig, logger: Logger):
         self.config = config
         self.logger = logger
         self.chatcompletion_request_funcs = {}
 
@@ -214,15 +214,15 @@
 
         self.logger.log(20,
                    f'Schema Validation on string:\n{s}\nfor schema {schema["name"]} failed, trying to fix it...')
 
         ret = await self.chatcompletion(
             messages=[{
                 "role": "user",
-                "content": f"""Your task is to fix the json string with schema errors. Remember to keep the target schema in mind. \nAvoid adding any information about this fix!\n\n# Error String\n{s}\n\n# Target Schema\n{schema}\n\n# Error Message\n{error_message}"""
+                "content": clip_text(f"""Your task is to fix the json string with schema errors. Remember to keep the target schema in mind. \nAvoid adding any information about this fix!\n\n# Error String\n{s}\n\n# Target Schema\n{schema}\n\n# Error Message\n{error_message[-1024:]}""",max_tokens=self.config.execution.max_message_tokens,clip_end=True)[0]
             }],
             schemas=StructureSchema(
                 name="json_fixes",
                 description="Fix the error in json string",
                 parameters={
                     "type": "object",
                     "properties": {
```

### Comparing `codelinker-0.1.5/codelinker/request/openai.py` & `codelinker-0.1.6/codelinker/request/openai.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/codelinker/utils.py` & `codelinker-0.1.6/codelinker/utils.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.5/PKG-INFO` & `codelinker-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelinker
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: luyaxi
 Author-email: luyaxi@live.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

