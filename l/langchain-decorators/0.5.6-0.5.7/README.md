# Comparing `tmp/langchain_decorators-0.5.6.tar.gz` & `tmp/langchain_decorators-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_decorators-0.5.6.tar", last modified: Sun Apr 14 18:33:31 2024, max compression
+gzip compressed data, was "langchain_decorators-0.5.7.tar", last modified: Thu Apr 18 11:55:42 2024, max compression
```

## Comparing `langchain_decorators-0.5.6.tar` & `langchain_decorators-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.356951 langchain_decorators-0.5.6/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain_decorators-0.5.6/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-14 18:33:31.356725 langchain_decorators-0.5.6/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22976 2024-04-14 18:30:54.000000 langchain_decorators-0.5.6/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain_decorators-0.5.6/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-14 18:33:31.356991 langchain_decorators-0.5.6/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain_decorators-0.5.6/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.349706 langchain_decorators-0.5.6/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.354999 langchain_decorators-0.5.6/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-14 18:33:00.000000 langchain_decorators-0.5.6/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    37071 2024-02-14 08:32:56.000000 langchain_decorators-0.5.6/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain_decorators-0.5.6/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21281 2024-04-14 15:47:14.000000 langchain_decorators-0.5.6/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain_decorators-0.5.6/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21900 2024-04-02 10:42:42.000000 langchain_decorators-0.5.6/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain_decorators-0.5.6/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain_decorators-0.5.6/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-01-05 14:48:06.000000 langchain_decorators-0.5.6/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain_decorators-0.5.6/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.356422 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 11:55:42.033919 langchain_decorators-0.5.7/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain_decorators-0.5.7/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-18 11:55:42.033643 langchain_decorators-0.5.7/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22976 2024-04-14 18:30:54.000000 langchain_decorators-0.5.7/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain_decorators-0.5.7/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-18 11:55:42.033967 langchain_decorators-0.5.7/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain_decorators-0.5.7/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 11:55:42.026148 langchain_decorators-0.5.7/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 11:55:42.031437 langchain_decorators-0.5.7/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-18 11:55:13.000000 langchain_decorators-0.5.7/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    40743 2024-04-17 06:59:53.000000 langchain_decorators-0.5.7/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain_decorators-0.5.7/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21281 2024-04-14 15:47:14.000000 langchain_decorators-0.5.7/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain_decorators-0.5.7/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24077 2024-04-18 08:01:29.000000 langchain_decorators-0.5.7/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain_decorators-0.5.7/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain_decorators-0.5.7/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-04-16 20:33:14.000000 langchain_decorators-0.5.7/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain_decorators-0.5.7/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-18 11:55:42.033333 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-18 11:55:42.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-18 11:55:42.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-18 11:55:42.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-18 11:55:42.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-18 11:55:42.000000 langchain_decorators-0.5.7/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain_decorators-0.5.6/LICENSE` & `langchain_decorators-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/PKG-INFO` & `langchain_decorators-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.6
+Version: 0.5.7
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain_decorators-0.5.6/README.md` & `langchain_decorators-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/setup.py` & `langchain_decorators-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/chains.py` & `langchain_decorators-0.5.7/src/langchain_decorators/chains.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,49 @@
+import inspect
 import json
 import logging
-import inspect
-from typing import Any, Callable, Coroutine, Dict, List, Optional,  Union
-from langchain.chains import LLMChain
-from langchain.prompts import  PromptTemplate
-from langchain.schema import LLMResult
-from langchain.callbacks.manager import CallbackManagerForChainRun, AsyncCallbackManagerForChainRun, Callbacks
-from langchain.tools.base import BaseTool
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Union
 
-from langchain.chat_models.base import BaseChatModel
+import pydantic
 from langchain.callbacks.base import BaseCallbackHandler, BaseCallbackManager
-from langchain.schema.output import LLMResult
+from langchain.callbacks.manager import (
+    AsyncCallbackManagerForChainRun,
+    CallbackManagerForChainRun,
+    Callbacks,
+)
+from langchain.chains import LLMChain
+from langchain.chat_models.base import BaseChatModel
+from langchain.prompts import PromptTemplate
 from langchain.prompts.base import StringPromptValue
-from langchain.prompts.chat import  ChatPromptValue
-from langchain.prompts.chat import  ChatPromptValue
-from langchain.schema import ChatGeneration, BaseMessage, HumanMessage, AIMessage
+from langchain.prompts.chat import ChatPromptValue
+from langchain.schema import (
+    AIMessage,
+    BaseMessage,
+    ChatGeneration,
+    HumanMessage,
+    LLMResult,
+)
+from langchain.schema.output import LLMResult
+from langchain.tools.base import BaseTool
 
-from .common import LlmSelector, print_log, LogColors, PromptTypeSettings, PromptTypes
-from .schema import OutputWithFunctionCall
-from .prompt_template import PromptDecoratorTemplate
-from .output_parsers import OpenAIFunctionsPydanticOutputParser, BaseOutputParser, OutputParserExceptionWithOriginal
+from .common import LlmSelector, LogColors, PromptTypes, PromptTypeSettings, print_log
 from .function_decorator import get_function_schema
+from .output_parsers import (
+    BaseOutputParser,
+    OpenAIFunctionsPydanticOutputParser,
+    OutputParserExceptionWithOriginal,
+)
+from .prompt_template import PromptDecoratorTemplate
+from .schema import OutputWithFunctionCall
 
-import pydantic
-
-if pydantic.__version__ <"2.0.0":
+if pydantic.__version__ < "2.0.0":
     from pydantic import PrivateAttr, root_validator
 else:
-    from pydantic.v1.fields import PrivateAttr
     from pydantic.v1.class_validators import root_validator
+    from pydantic.v1.fields import PrivateAttr
 
 CachedChatLLM = None
 register_prompt_template = None
 try:
     from langchain.tools.convert_to_openai import format_tool_to_openai_function
     from promptwatch import CachedChatLLM, register_prompt_template
 except ImportError:
@@ -40,412 +51,548 @@
 
 try:
     from langchain_openai import ChatOpenAI
 except ImportError:
     ChatOpenAI = None
     pass
 
-MODELS_WITH_JSON_FORMAT_SUPPORT=["gpt-3.5-turbo-1106","gpt-4-1106-preview", "gpt-3.5-turbo-0125", "gpt-4-0125-preview"]
+MODELS_WITH_JSON_FORMAT_SUPPORT = [
+    "gpt-3.5-turbo-1106",
+    "gpt-4-1106-preview",
+    "gpt-3.5-turbo-0125",
+    "gpt-4-0125-preview",
+]
 
 
 class FunctionsProvider:
 
-    def __init__(self, functions:Union[List[Union[Callable, BaseTool]], Dict[str,Union[Callable, BaseTool]]]) -> None:
-        """ Initialize FunctionsProvider with list of funcitons of dictionary where key is the unique function name alias"""
-        self.functions=[]
-        self.aliases=[]
-        self.function_schemas=[]
-        self.func_name_map={}
+    def __init__(
+        self,
+        functions: Union[
+            List[Union[Callable, BaseTool]], Dict[str, Union[Callable, BaseTool]]
+        ],
+    ) -> None:
+        """Initialize FunctionsProvider with list of funcitons of dictionary where key is the unique function name alias"""
+        self.functions = []
+        self.aliases = []
+        self.function_schemas = []
+        self.func_name_map = {}
         if not (isinstance(functions, dict) or isinstance(functions, list)):
-            raise ValueError("FunctionsProvider must be initialized with list of functions or dictionary where key is the unique function name alias")
-        
-        for i,f in enumerate(functions):
-            
+            raise ValueError(
+                "FunctionsProvider must be initialized with list of functions or dictionary where key is the unique function name alias"
+            )
+
+        for i, f in enumerate(functions):
+
             if isinstance(f, str):
                 function_alias = f
                 f = functions[f]
             else:
-               function_alias=None
+                function_alias = None
 
             self.add_function(f, function_alias)
-        
-    
-    def add_function(self, function:Union[Callable, BaseTool], alias:str=None):
-        """ Add function to FunctionsProvider. If alias is provided, it will be used as function name in LLM"""
+
+    def add_function(self, function: Union[Callable, BaseTool], alias: str = None):
+        """Add function to FunctionsProvider. If alias is provided, it will be used as function name in LLM"""
         self.functions.append(function)
         self.aliases.append(alias)
         if isinstance(function, BaseTool):
             self.function_schemas.append(format_tool_to_openai_function(function))
             f_name = alias or function.name
-        elif callable(function) and hasattr(function,"get_function_schema"):
-            if hasattr(function,"function_name"):
+        elif callable(function) and hasattr(function, "get_function_schema"):
+            if hasattr(function, "function_name"):
                 f_name = alias or function.function_name
             else:
-                raise Exception(f"Function {function} does not have function_name attribute. All functions must be marked with @llm_function decorator")
-            self.function_schemas.append(lambda kwargs, f=function: get_function_schema(f, kwargs))
+                raise Exception(
+                    f"Function {function} does not have function_name attribute. All functions must be marked with @llm_function decorator"
+                )
+            self.function_schemas.append(
+                lambda kwargs, f=function: get_function_schema(f, kwargs)
+            )
         else:
-            raise ValueError(f"Invalid item value in functions. Only Tools or functions decorated with @llm_function are allowed. Got: {function}")
+            raise ValueError(
+                f"Invalid item value in functions. Only Tools or functions decorated with @llm_function are allowed. Got: {function}"
+            )
         if f_name in self.func_name_map:
             if alias:
                 raise ValueError(f"Invalid alias - duplicate function name: {f_name}.")
             else:
-                raise ValueError(f"Duplicate function name: {f_name}. Use unique function names, or use FunctionsProvider and assign a unique alias to each function.")
-        self.func_name_map[f_name]=function
-        
+                raise ValueError(
+                    f"Duplicate function name: {f_name}. Use unique function names, or use FunctionsProvider and assign a unique alias to each function."
+                )
+        self.func_name_map[f_name] = function
+
     def __contains__(self, function):
         return function in self.functions
 
-    def get_function_schemas(self, inputs, _index:int=None):
+    def get_function_schemas(self, inputs, _index: int = None):
         if self.function_schemas:
             _f_schemas = []
-            for i, (alias, f_schema_builder) in enumerate(zip(self.aliases,self.function_schemas)):
-                if _index is not None and i!=_index:
+            for i, (alias, f_schema_builder) in enumerate(
+                zip(self.aliases, self.function_schemas)
+            ):
+                if _index is not None and i != _index:
                     continue
 
                 if callable(f_schema_builder):
                     _f_schema = f_schema_builder(inputs)
                 else:
                     _f_schema = f_schema_builder
 
                 if alias:
-                    _f_schema["name"]=alias
-                
+                    _f_schema["name"] = alias
+
                 _f_schemas.append(_f_schema)
-                
+
             return _f_schemas
         else:
             None
 
-
-    
-    def get_function_schema(self, function:Union[str, Callable], inputs:dict):
-        index=None
+    def get_function_schema(self, function: Union[str, Callable], inputs: dict):
+        index = None
         if isinstance(function, str):
             func = self.func_name_map[function]
         else:
             func = function
-            
+
         _index = self.functions.index(func)
         return self.get_function_schemas(inputs, _index=_index)[0]
 
-
-
-
-    def get_function(self, function_name:str=None):
+    def get_function(self, function_name: str = None):
         if function_name in self.func_name_map:
             return self.func_name_map[function_name]
         else:
             raise KeyError(f"Invalid function {function_name}")
-        
+
     def __iter__(self):
         return iter(self.functions)
-    
+
     def index(self, function):
         return self.functions.index(function)
 
 
 class LLMDecoratorChain(LLMChain):
-    name:str
-    llm_selector:LlmSelector=None
+    name: str
+    llm_selector: LlmSelector = None
     """ Optional LLM selector to pick the right LLM for the job. """
-    capture_stream:bool=False
-    expected_gen_tokens:Optional[int]=None
-    llm_selector_rule_key:Optional[str]=None
-    allow_retries:bool=True
-    format_instructions_parameter_key:str="FORMAT_INSTRUCTIONS",
-
-    prompt_type:PromptTypeSettings = PromptTypes.UNDEFINED
-    default_call_kwargs:Optional[Dict[str,Any]]
-    _additional_instruction:Optional[str]=PrivateAttr()
-    _is_retry:Optional[str]=PrivateAttr(default=False)
-
-    def __call__(self, 
-                 inputs: Union[Dict[str, Any], Any]=None, 
-                 return_only_outputs: bool = False, 
-                 callbacks: Callbacks = None, 
-                 *, 
-                 tags: Union[List[str], None] = None, 
-                 metadata: Union[Dict[str, Any], None] = None, 
-                 include_run_info: bool = False,
-                 additional_instruction:str=None
-                 ,
-                 **kwargs
-                 ) -> Dict[str, Any]:
+    capture_stream: bool = False
+    expected_gen_tokens: Optional[int] = None
+    llm_selector_rule_key: Optional[str] = None
+    allow_retries: bool = True
+    format_instructions_parameter_key: str = ("FORMAT_INSTRUCTIONS",)
+
+    prompt_type: PromptTypeSettings = PromptTypes.UNDEFINED
+    default_call_kwargs: Optional[Dict[str, Any]]
+    _additional_instruction: Optional[str] = PrivateAttr()
+    _is_retry: Optional[str] = PrivateAttr(default=False)
+
+    def __call__(
+        self,
+        inputs: Union[Dict[str, Any], Any] = None,
+        return_only_outputs: bool = False,
+        callbacks: Callbacks = None,
+        *,
+        tags: Union[List[str], None] = None,
+        metadata: Union[Dict[str, Any], None] = None,
+        include_run_info: bool = False,
+        additional_instruction: str = None,
+        **kwargs,
+    ) -> Dict[str, Any]:
         """Call the chain with inputs."""
 
         # override of __call__ so this can be run preinitialized by the decorator call
-        kwargs["inputs"]=inputs
-        kwargs["return_only_outputs"]=return_only_outputs
-        kwargs["callbacks"]=callbacks
-        kwargs["tags"]=tags
-        kwargs["metadata"]=metadata
-        kwargs["include_run_info"]=include_run_info
-        self._additional_instruction=additional_instruction
+        kwargs["inputs"] = inputs
+        kwargs["return_only_outputs"] = return_only_outputs
+        kwargs["callbacks"] = callbacks
+        kwargs["tags"] = tags
+        kwargs["metadata"] = metadata
+        kwargs["include_run_info"] = include_run_info
+        self._additional_instruction = additional_instruction
         if self.default_call_kwargs:
-            for k,v in self.default_call_kwargs.items():
-                if kwargs.get(k,None) is None and k in self.default_call_kwargs:
-                    kwargs[k]=v
-        print_log(log_object=f"> Entering {self.name} prompt decorator chain", log_level=self.prompt_type.log_level,color=LogColors.WHITE_BOLD)
+            for k, v in self.default_call_kwargs.items() and k != "llm_kwargs":
+                if kwargs.get(k, None) is None and k in self.default_call_kwargs:
+                    kwargs[k] = v
+        print_log(
+            log_object=f"> Entering {self.name} prompt decorator chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
         try:
             result = super().__call__(**kwargs)
         except RequestRetry as e:
-            if self._is_retry==True:
+            if self._is_retry == True:
                 raise Exception(e.feedback)
-            self._is_retry=True
-            self._additional_instruction=e.feedback
+            self._is_retry = True
+            self._additional_instruction = e.feedback
             result = super().__call__(**kwargs)
-        print_log(log_object=f"> Finished chain", log_level=self.prompt_type.log_level,color=LogColors.WHITE_BOLD)
-        self._additional_instruction=None
+        print_log(
+            log_object=f"> Finished chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
+        self._additional_instruction = None
         return result
 
-    async def acall(self, 
-              inputs: Union[Dict[str, Any], Any]=None, 
-              return_only_outputs: bool = False, 
-              callbacks: Callbacks = None, 
-              *, 
-              tags: Union[List[str], None] = None, 
-              metadata: Union[Dict[str, Any], None] = None, 
-              include_run_info: bool = False,
-              additional_instruction:str=None,
-              **kwargs
-              ) -> Coroutine[Any, Any, Dict[str, Any]]:
+    async def acall(
+        self,
+        inputs: Union[Dict[str, Any], Any] = None,
+        return_only_outputs: bool = False,
+        callbacks: Callbacks = None,
+        *,
+        tags: Union[List[str], None] = None,
+        metadata: Union[Dict[str, Any], None] = None,
+        include_run_info: bool = False,
+        additional_instruction: str = None,
+        **kwargs,
+    ) -> Coroutine[Any, Any, Dict[str, Any]]:
         """Asynchronously call the chain with inputs."""
         # override of __call__ so this can be run preinitialized by the decorator call
-        kwargs["inputs"]=inputs 
-        kwargs["return_only_outputs"]=return_only_outputs
-        kwargs["callbacks"]=callbacks
-        kwargs["tags"]=tags
-        kwargs["metadata"]=metadata
-        kwargs["include_run_info"]=include_run_info
-        self._additional_instruction=additional_instruction
+        kwargs["inputs"] = inputs
+        kwargs["return_only_outputs"] = return_only_outputs
+        kwargs["callbacks"] = callbacks
+        kwargs["tags"] = tags
+        kwargs["metadata"] = metadata
+        kwargs["include_run_info"] = include_run_info
+        self._additional_instruction = additional_instruction
         if self.default_call_kwargs:
-            for k,v in self.default_call_kwargs.items():
-                if kwargs.get(k,None) is None and k in self.default_call_kwargs:
-                    kwargs[k]=v
+            for k, v in self.default_call_kwargs.items():
+                if (
+                    k != "llm_kwargs"
+                    and kwargs.get(k, None) is None
+                    and k in self.default_call_kwargs
+                ):
+                    kwargs[k] = v
 
         try:
             result = await super().acall(**kwargs)
         except RequestRetry as e:
-            if self._is_retry==True:
+            if self._is_retry == True:
                 raise Exception(e.feedback)
-            self._is_retry=True
-            self._additional_instruction=e.feedback
+            self._is_retry = True
+            self._additional_instruction = e.feedback
             result = await super().acall(**kwargs)
-        self._additional_instruction=None
+        self._additional_instruction = None
         return result
 
-    def execute(self,**kwargs):
+    def execute(self, **kwargs):
         """Execute the chain and return outputs"""
-        print_log(log_object=f"> Entering {self.name} prompt decorator chain", log_level=self.prompt_type.log_level ,color=LogColors.WHITE_BOLD)
+        print_log(
+            log_object=f"> Entering {self.name} prompt decorator chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
 
         result_data = self.__call__(**kwargs)
 
         result = result_data[self.output_key]
         try:
             result = self.postprocess_outputs(result_data, result)
         except OutputParserExceptionWithOriginal as e:
             if self.allow_retries:
-                _kwargs = {**self.default_call_kwargs} if self.default_call_kwargs else {}
+                _kwargs = (
+                    {**self.default_call_kwargs} if self.default_call_kwargs else {}
+                )
                 _kwargs.update(kwargs)
-                retryChain, call_kwargs = self._get_retry_parse_call_args(self.prompt, e, lambda: self.prompt.format(**_kwargs["inputs"]))
+                retryChain, call_kwargs = self._get_retry_parse_call_args(
+                    self.prompt, e, lambda: self.prompt.format(**_kwargs["inputs"])
+                )
                 result = retryChain.predict(**call_kwargs)
-                print_log(log_object=f"\nResult:\n{result}", log_level=self.prompt_type.log_level if not self.verbose else 100,color=self.prompt_type.color if self.prompt_type else LogColors.BLUE)
+                print_log(
+                    log_object=f"\nResult:\n{result}",
+                    log_level=self.prompt_type.log_level if not self.verbose else 100,
+                    color=(
+                        self.prompt_type.color if self.prompt_type else LogColors.BLUE
+                    ),
+                )
                 return self.postprocess_outputs(result_data, result)
-            else: 
+            else:
                 raise e
 
-        print_log(log_object=f"> Finished chain", log_level=self.prompt_type.log_level,color=LogColors.WHITE_BOLD)
+        print_log(
+            log_object=f"> Finished chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
         return result
 
-    async def aexecute(self,**kwargs):
+    async def aexecute(self, **kwargs):
         """Execute the chain and return outputs"""
-        print_log(log_object=f"> Entering {self.name} prompt decorator chain", log_level=self.prompt_type.log_level ,color=LogColors.WHITE_BOLD)
+        print_log(
+            log_object=f"> Entering {self.name} prompt decorator chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
 
         try:
             result_data = await self.acall(**kwargs)
 
             result = result_data[self.output_key]
 
             result = self.postprocess_outputs(result_data, result)
         except RequestRetry as e:
-            if self._is_retry==True:
+            if self._is_retry == True:
                 raise Exception(e.feedback)
-            self._is_retry=True
+            self._is_retry = True
             result_data = await self.acall(**kwargs, additional_instruction=e.feedback)
 
             result = result_data[self.output_key]
 
             result = self.postprocess_outputs(result_data, result)
         except OutputParserExceptionWithOriginal as e:
             if self.allow_retries:
-                _kwargs = {**self.default_call_kwargs} if self.default_call_kwargs else {}
+                _kwargs = (
+                    {**self.default_call_kwargs} if self.default_call_kwargs else {}
+                )
                 _kwargs.update(kwargs)
-                retryChain, call_kwargs = self._get_retry_parse_call_args(self.prompt, e, lambda: self.prompt.format(**_kwargs["inputs"]))
+                retryChain, call_kwargs = self._get_retry_parse_call_args(
+                    self.prompt, e, lambda: self.prompt.format(**_kwargs["inputs"])
+                )
                 result = await retryChain.apredict(**call_kwargs)
-                print_log(log_object=f"\nResult:\n{result}", log_level=self.prompt_type.log_level if not self.verbose else 100,color=self.prompt_type.color if self.prompt_type else LogColors.BLUE)
+                print_log(
+                    log_object=f"\nResult:\n{result}",
+                    log_level=self.prompt_type.log_level if not self.verbose else 100,
+                    color=(
+                        self.prompt_type.color if self.prompt_type else LogColors.BLUE
+                    ),
+                )
                 return self.postprocess_outputs(result_data, result)
-            else: 
+            else:
                 raise e
 
-        print_log(log_object=f"> Finished chain", log_level=self.prompt_type.log_level,color=LogColors.WHITE_BOLD)
+        print_log(
+            log_object=f"> Finished chain",
+            log_level=self.prompt_type.log_level,
+            color=LogColors.WHITE_BOLD,
+        )
         return result
 
-    def _get_retry_parse_call_args(self,prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal, get_original_prompt:Callable):
-        logging.warning(msg=f"Failed to parse output for {self.name}: {exception}\nRetrying...")
-        if hasattr(self.prompt, "template_string") and self.format_instructions_parameter_key not in self.prompt.template_string:
-            logging.warning(f"Please note that we didn't find a {self.format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions.")    
+    def _get_retry_parse_call_args(
+        self,
+        prompt_template: PromptDecoratorTemplate,
+        exception: OutputParserExceptionWithOriginal,
+        get_original_prompt: Callable,
+    ):
+        logging.warning(
+            msg=f"Failed to parse output for {self.name}: {exception}\nRetrying..."
+        )
+        if (
+            hasattr(self.prompt, "template_string")
+            and self.format_instructions_parameter_key
+            not in self.prompt.template_string
+        ):
+            logging.warning(
+                f"Please note that we didn't find a {self.format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions."
+            )
         if exception.original_prompt_needed_on_retry:
-            original_prompt=get_original_prompt()
+            original_prompt = get_original_prompt()
         else:
-            original_prompt=""
-        retry_parse_template = PromptTemplate.from_template("{original_prompt}This is our original response {original} but it's not in correct format, please convert it into following format:\n{format_instructions}\n\nIf the response doesn't seem to be relevant to the expected format instructions, return 'N/A'")
+            original_prompt = ""
+        retry_parse_template = PromptTemplate.from_template(
+            "{original_prompt}This is our original response {original} but it's not in correct format, please convert it into following format:\n{format_instructions}\n\nIf the response doesn't seem to be relevant to the expected format instructions, return 'N/A'"
+        )
         register_prompt_template("retry_parse_template", retry_parse_template)
 
         retryChain = LLMChain(llm=self.llm, prompt=retry_parse_template)
         format_instructions = prompt_template.output_parser.get_format_instructions()
         if not format_instructions:
-            raise Exception(f"Failed to get format instructions for {self.name} from output parser {prompt_template.output_parser}.")
-        call_kwargs = {"original_prompt":original_prompt, "original":exception.original, "format_instructions":format_instructions}
+            raise Exception(
+                f"Failed to get format instructions for {self.name} from output parser {prompt_template.output_parser}."
+            )
+        call_kwargs = {
+            "original_prompt": original_prompt,
+            "original": exception.original,
+            "format_instructions": format_instructions,
+        }
         return retryChain, call_kwargs
 
     def postprocess_outputs(self, result_data, result):
-        log_results(result_data, result, is_function_call=False, verbose=self.verbose, prompt_type=self.prompt_type)
-        if self.prompt.output_parser:    
+        log_results(
+            result_data,
+            result,
+            is_function_call=False,
+            verbose=self.verbose,
+            prompt_type=self.prompt_type,
+        )
+        if self.prompt.output_parser:
             if result:
                 try:
                     result = self.prompt.output_parser.parse(result)
                 except:
-                    result = False if result and "yes" in result.lower() else False # usually its something like "Im sorry..."
+                    result = (
+                        False if result and "yes" in result.lower() else False
+                    )  # usually its something like "Im sorry..."
         return result
 
     def select_llm(self, prompts, inputs=None):
         if self.llm_selector:
             # we pick the right LLM based on the first prompt
             first_prompt = prompts[0]
             if isinstance(first_prompt, ChatPromptValue):
-                llm = self.llm_selector.get_llm(first_prompt.messages,**self._additional_llm_selector_args(inputs))
+                llm = self.llm_selector.get_llm(
+                    first_prompt.messages, **self._additional_llm_selector_args(inputs)
+                )
             elif isinstance(first_prompt, str):
-                self.llm_selector.get_llm(first_prompt,**self._additional_llm_selector_args(inputs))
+                self.llm_selector.get_llm(
+                    first_prompt, **self._additional_llm_selector_args(inputs)
+                )
             else:
-                llm = self.llm_selector.get_llm(first_prompt.to_string(),**self._additional_llm_selector_args(inputs))
+                llm = self.llm_selector.get_llm(
+                    first_prompt.to_string(),
+                    **self._additional_llm_selector_args(inputs),
+                )
         else:
             llm = self.llm
         return llm
 
     def _additional_llm_selector_args(self, inputs):
         return {
-            "expected_generated_tokens":self.expected_gen_tokens, 
-            "streaming":self.capture_stream,
-            "llm_selector_rule_key":self.llm_selector_rule_key
-            }
-    
+            "expected_generated_tokens": self.expected_gen_tokens,
+            "streaming": self.capture_stream,
+            "llm_selector_rule_key": self.llm_selector_rule_key,
+        }
+
     def __should_use_json_response_format(self, llm):
         if "OpenAI" in type(llm).__name__:
-            if llm.model_name in MODELS_WITH_JSON_FORMAT_SUPPORT and self.prompt.output_parser and (self.prompt.output_parser._type=="json" or self.prompt.output_parser._type=="pydantic"):
+            if (
+                llm.model_name in MODELS_WITH_JSON_FORMAT_SUPPORT
+                and self.prompt.output_parser
+                and (
+                    self.prompt.output_parser._type == "json"
+                    or self.prompt.output_parser._type == "pydantic"
+                )
+            ):
                 return True
-    
 
     def generate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
         prompts, stop = self.prep_prompts(input_list, run_manager=run_manager)
 
         llm = self.select_llm(prompts, input_list[0])
 
-        additional_kwargs=self.llm_kwargs or {}
+        additional_kwargs = self.llm_kwargs or {}
         if self.__should_use_json_response_format(llm):
-            additional_kwargs["response_format"]= { "type": "json_object" }
+            additional_kwargs["response_format"] = {"type": "json_object"}
 
         try:
             return llm.generate_prompt(
-                prompts, stop, callbacks=run_manager.get_child() if run_manager else None
+                prompts,
+                stop,
+                callbacks=run_manager.get_child() if run_manager else None,
+                **additional_kwargs,
             )
         except RequestRetry as e:
-            if not self._is_retry==True:
-                self._is_retry=True
+            if not self._is_retry == True:
+                self._is_retry = True
                 return llm.generate_prompt(
-                    prompts, stop, callbacks=run_manager.get_child() if run_manager else None,
-                    **additional_kwargs
+                    prompts,
+                    stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
+                    **additional_kwargs,
                 )
             else:
                 raise Exception(e.feedback)
 
     async def agenerate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
         prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
         llm = self.select_llm(prompts, input_list[0])
-        additional_kwargs=self.llm_kwargs or {}
+        additional_kwargs = self.llm_kwargs or {}
         if self.__should_use_json_response_format(llm):
-            additional_kwargs["response_format"]= { "type": "json_object" }
+            additional_kwargs["response_format"] = {"type": "json_object"}
+        if self.llm_kwargs:
+            additional_kwargs["llm_kwargs"] = self.llm_kwargs
         try:
             return await llm.agenerate_prompt(
-                prompts, stop, callbacks=run_manager.get_child() if run_manager else None
+                prompts,
+                stop,
+                callbacks=run_manager.get_child() if run_manager else None,
+                **additional_kwargs,
             )
         except RequestRetry as e:
-            if not self._is_retry==True:
-                self._is_retry=True
+            if not self._is_retry == True:
+                self._is_retry = True
                 return await llm.agenerate_prompt(
-                    prompts, stop, callbacks=run_manager.get_child() if run_manager else None,
-                    **additional_kwargs
+                    prompts,
+                    stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
+                    **additional_kwargs,
                 )
             else:
                 raise Exception(e.feedback)
 
+
 class LLMDecoratorChainWithFunctionSupport(LLMDecoratorChain):
 
-    functions:Union[FunctionsProvider,List[Union[Callable, BaseTool]]]
-    func_name_map:dict=None
+    functions: Union[FunctionsProvider, List[Union[Callable, BaseTool]]]
+    func_name_map: dict = None
 
-    function_call_output_key:str="function_call_info"
-    function_output_key:str="function"
-    message_output_key:str="message"
-    _is_retry:Optional[str]=PrivateAttr(default=False)
+    function_call_output_key: str = "function_call_info"
+    function_output_key: str = "function"
+    message_output_key: str = "message"
+    _is_retry: Optional[str] = PrivateAttr(default=False)
 
     @property
     def output_keys(self) -> List[str]:
         """Will always return text key.
 
         :meta private:
         """
-        return [self.output_key, self.function_output_key, self.function_call_output_key]
+        return [
+            self.output_key,
+            self.function_output_key,
+            self.function_call_output_key,
+        ]
 
     def postprocess_outputs(self, result_data, result):
-        log_results(result_data, result, bool(self.functions.functions), self.verbose, self.prompt_type)
-
-        if self.prompt.output_parser:    
-            if isinstance(self.prompt.output_parser, OpenAIFunctionsPydanticOutputParser):
+        log_results(
+            result_data,
+            result,
+            bool(self.functions.functions),
+            self.verbose,
+            self.prompt_type,
+        )
+
+        if self.prompt.output_parser:
+            if isinstance(
+                self.prompt.output_parser, OpenAIFunctionsPydanticOutputParser
+            ):
                 # it the output parser is OpenAIFunctionsPydanticOutputParser, it means we should return the regular result, since we've used functions only for structure calling
                 # there is no result probably, but if there is, we ignore it... we are interested only in tha data in function_call_info
-                result = self.prompt.output_parser.parse(result_data["function_call_info"]["arguments"])
+                result = self.prompt.output_parser.parse(
+                    result_data["function_call_info"]["arguments"]
+                )
                 # we dont want to return  OutputWithFunctionCall in this case
                 # TODO: Hardcoded for now...
                 return result
             else:
                 if result:
                     result = self.prompt.output_parser.parse(result)
 
         return self._generate_output_with_function_call(result, result_data)
 
     @root_validator(pre=True)
     def validate_and_prepare_chain(cls, values):
-        functions = values.get("functions",None)
-        llm = values.get("llm",None)
-        if isinstance(functions,list):
+        functions = values.get("functions", None)
+        llm = values.get("llm", None)
+        if isinstance(functions, list):
             values["functions"] = FunctionsProvider(functions)
-        elif isinstance(functions,FunctionsProvider):
+        elif isinstance(functions, FunctionsProvider):
             values["functions"] = functions
         elif functions:
-            raise ValueError(f"functions must be a List[Callable|BaseTool] or FunctionsProvider instance. Got: {functions.__class__}")
+            raise ValueError(
+                f"functions must be a List[Callable|BaseTool] or FunctionsProvider instance. Got: {functions.__class__}"
+            )
 
         if not llm:
             raise ValueError("llm must be defined")
 
         # if not "OpenAI" in type(llm).__name__ and (
         #     CachedChatLLM and not isinstance(llm, CachedChatLLM)
         # ):
@@ -454,171 +601,222 @@
         return values
 
     def get_final_function_schemas(self, inputs):
         return self.functions.get_function_schemas(inputs)
 
     def _additional_llm_selector_args(self, inputs):
         args = super()._additional_llm_selector_args(inputs)
-        args["function_schemas"]=self.get_final_function_schemas(inputs)
+        args["function_schemas"] = self.get_final_function_schemas(inputs)
         return args
 
     def preprocess_inputs(self, input_list):
         additional_kwargs = self.llm_kwargs or {}
 
-        final_function_schemas=None
+        final_function_schemas = None
         if self.functions:
             if self.memory is not None:
                 # we are sending out more outputs... memory expects only one (AIMessage... so let's set it, becasue user has no way to know these internals)
                 if hasattr(self.memory, "output_key") and not self.memory.output_key:
                     self.memory.output_key = "message"
-            if len(input_list)!=1:
+            if len(input_list) != 1:
                 raise ValueError("Only one input is allowed when using functions")
             if "function_call" in input_list[0]:
                 for input in input_list:
-                    function_call=input.pop("function_call")
+                    function_call = input.pop("function_call")
                 # function call should be only one... and the same for all inputs... there shouldn't be more anyway
-                if not isinstance(function_call,str):
-                    f_name = next((f_name for f_name, func in  self.functions.func_name_map.items() if func == function_call), None)
+                if not isinstance(function_call, str):
+                    f_name = next(
+                        (
+                            f_name
+                            for f_name, func in self.functions.func_name_map.items()
+                            if func == function_call
+                        ),
+                        None,
+                    )
                     if not f_name:
-                        raise ValueError(f"Invalid function call. Function {function_call} is not defined in this chain")
+                        raise ValueError(
+                            f"Invalid function call. Function {function_call} is not defined in this chain"
+                        )
                     function_call = {"name": f_name}
-                elif function_call not in ["none","auto"]:
+                elif function_call not in ["none", "auto"]:
                     # test if it's a valid function name
                     self.get_function(function_call)
 
                     function_call = {"name": function_call}
 
-                additional_kwargs["function_call"]=function_call 
+                additional_kwargs["function_call"] = function_call
             final_function_schemas = self.get_final_function_schemas(input_list[0])
         return additional_kwargs, final_function_schemas
 
     def generate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
 
         additional_kwargs, final_function_schemas = self.preprocess_inputs(input_list)
 
         prompts, stop = self.prep_prompts(input_list, run_manager=run_manager)
-        chat_model:BaseChatModel=self.select_llm(prompts, input_list[0])
+        chat_model: BaseChatModel = self.select_llm(prompts, input_list[0])
+
         def run():
             if self.functions:
                 messages = [prompt.to_messages() for prompt in prompts]
 
-                result =  chat_model.generate(messages=messages, 
-                                            stop=stop, callbacks=run_manager.get_child() if run_manager else None,
-                                            functions=final_function_schemas,
-                                            **additional_kwargs
-                                            )
+                result = chat_model.generate(
+                    messages=messages,
+                    stop=stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
+                    functions=final_function_schemas,
+                    **additional_kwargs,
+                )
                 return result
             else:
                 return chat_model.generate_prompt(
-                    prompts, stop, callbacks=run_manager.get_child() if run_manager else None
+                    prompts,
+                    stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
                 )
+
         try:
             return run()
         except RequestRetry as e:
-            if not self._is_retry==True:
-                self._is_retry=True
+            if not self._is_retry == True:
+                self._is_retry = True
                 return run()
             else:
                 raise Exception(e.feedback)
 
     async def agenerate(
         self,
         input_list: List[Dict[str, Any]],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> LLMResult:
         """Generate LLM result from inputs."""
         additional_kwargs, final_function_schemas = self.preprocess_inputs(input_list)
 
         prompts, stop = await self.aprep_prompts(input_list, run_manager=run_manager)
-        chat_model:BaseChatModel=self.select_llm(prompts, input_list[0])
+        chat_model: BaseChatModel = self.select_llm(prompts, input_list[0])
 
-        async def arun(additional_instruction:str=None):
+        async def arun(additional_instruction: str = None):
             if final_function_schemas:
                 messages = [prompt.to_messages() for prompt in prompts]
                 if additional_instruction:
                     messages[0].append(AIMessage(content=additional_instruction))
-                return  await chat_model.agenerate(messages=messages, 
-                                            stop=stop, callbacks=run_manager.get_child() if run_manager else None,
-                                            functions=final_function_schemas,
-                                            **additional_kwargs
-                                            )
+                return await chat_model.agenerate(
+                    messages=messages,
+                    stop=stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
+                    functions=final_function_schemas,
+                    **additional_kwargs,
+                )
             else:
                 return await chat_model.agenerate_prompt(
-                    prompts, stop, callbacks=run_manager.get_child() if run_manager else None
+                    prompts,
+                    stop,
+                    callbacks=run_manager.get_child() if run_manager else None,
                 )
 
         try:
             return await arun(additional_instruction=self._additional_instruction)
         except RequestRetry as e:
-            if not self._is_retry==True:
-                self._is_retry=True
+            if not self._is_retry == True:
+                self._is_retry = True
                 return await arun(self._additional_instruction)
             else:
                 raise Exception(e.feedback)
 
-    def _create_output(self,generation):
+    def _create_output(self, generation):
         res = {
-                self.output_key: generation.text,
-                self.function_call_output_key: None,
-                self.function_output_key: None,
-             }
+            self.output_key: generation.text,
+            self.function_call_output_key: None,
+            self.function_output_key: None,
+        }
         if isinstance(generation, ChatGeneration):
             res[self.message_output_key] = generation.message
             # let's make a copy of the function call so that we don't modify the original
-            function_call = dict(generation.message.additional_kwargs.get("function_call")) if generation.message.additional_kwargs else {}
+            function_call = (
+                dict(generation.message.additional_kwargs.get("function_call"))
+                if generation.message.additional_kwargs
+                else {}
+            )
             if function_call:
-                if isinstance(function_call["arguments"],str):
+                if isinstance(function_call["arguments"], str):
                     if function_call["name"] not in self.functions.func_name_map:
-                        raise RequestRetry(feedback=f"invalid function '{function_call['name']}', make sure to use only one of these functions: '{', '.join(self.functions.func_name_map.keys())}'")
+                        raise RequestRetry(
+                            feedback=f"invalid function '{function_call['name']}', make sure to use only one of these functions: '{', '.join(self.functions.func_name_map.keys())}'"
+                        )
                     try:
-                        function_call["arguments"]=json.loads(function_call["arguments"])
+                        function_call["arguments"] = json.loads(
+                            function_call["arguments"]
+                        )
                     except json.JSONDecodeError:
-                        raise RequestRetry(feedback="(function arguments  have to be a valid JSON)")
-
-            if generation.message.additional_kwargs and generation.message.additional_kwargs.get("function_call"):
+                        raise RequestRetry(
+                            feedback="(function arguments  have to be a valid JSON)"
+                        )
+
+            if (
+                generation.message.additional_kwargs
+                and generation.message.additional_kwargs.get("function_call")
+            ):
                 res[self.function_call_output_key] = function_call
                 try:
-                    function = self.get_function(function_call["name"]) if function_call else None
+                    function = (
+                        self.get_function(function_call["name"])
+                        if function_call
+                        else None
+                    )
                 except KeyError:
-                    print_log(f"LLM requested function {function_call['name']} which is not defined! Retrying", log_level=logging.WARNING)
+                    print_log(
+                        f"LLM requested function {function_call['name']} which is not defined! Retrying",
+                        log_level=logging.WARNING,
+                    )
                     valid_func_names = ", ".join(self.functions.func_name_map.keys())
-                    raise RequestRetry(feedback=f"(I need to make sure to use only valid functions... from the list: {valid_func_names})")
+                    raise RequestRetry(
+                        feedback=f"(I need to make sure to use only valid functions... from the list: {valid_func_names})"
+                    )
                 res[self.function_output_key] = function
         return res
 
-    def get_function(self,function_name):
+    def get_function(self, function_name):
         return self.functions.get_function(function_name)
 
     def create_outputs(self, response: LLMResult) -> List[Dict[str, str]]:
         """Create outputs from response."""
 
         return [
-            self._create_output(generation[0])
-            for generation in response.generations
+            self._create_output(generation[0]) for generation in response.generations
         ]
 
-    def _generate_output_with_function_call(self,result:Any, result_data:dict):
-        """ get parsed result, function call data from llm and list of functions and build  OutputWithFunctionCall """
+    def _generate_output_with_function_call(self, result: Any, result_data: dict):
+        """get parsed result, function call data from llm and list of functions and build  OutputWithFunctionCall"""
         # find the function first:
 
         _function = result_data["function"]
         if result_data.get("function_call_info"):
             _tool_arguments = result_data["function_call_info"]["arguments"]
             if isinstance(_function, BaseTool):
                 # langchain hack >> "__arg1" as a single argument hack
-                _is_single_arg_hack="__arg1" in _tool_arguments and len(_tool_arguments)==1
-                tool_input= _tool_arguments["__arg1"] if _is_single_arg_hack else _tool_arguments
+                _is_single_arg_hack = (
+                    "__arg1" in _tool_arguments and len(_tool_arguments) == 1
+                )
+                tool_input = (
+                    _tool_arguments["__arg1"]
+                    if _is_single_arg_hack
+                    else _tool_arguments
+                )
                 _tool_arguments = tool_input
+
                 def _sync_function(arguments=tool_input):
-                    return _function.run(tool_input=arguments, verbose=self.verbose, callbacks=self.callbacks)
+                    return _function.run(
+                        tool_input=arguments,
+                        verbose=self.verbose,
+                        callbacks=self.callbacks,
+                    )
 
                 async def _async_function(arguments=tool_input):
                     return await _function.arun(
                         tool_input=arguments,
                         verbose=self.verbose,
                         callbacks=self.callbacks,
                     )
@@ -631,49 +829,51 @@
                 if is_async:
                     _async_function = _function
                     _sync_function = None
                 else:
                     _sync_function = _function
                     _async_function = None
             else:
-                raise TypeError(f"Invalid function type: {_function} of type {type(_function)}")
+                raise TypeError(
+                    f"Invalid function type: {_function} of type {type(_function)}"
+                )
 
             return OutputWithFunctionCall(
-                    output=result,
-                    output_text=result_data["text"],
-                    output_message=result_data["message"],
-                    function=_sync_function,
-                    function_async=_async_function,
-                    function_name=result_data["function_call_info"]["name"],
-                    function_args=result_data["function_call_info"]["arguments"],
-                    function_arguments=_tool_arguments
-                )
+                output=result,
+                output_text=result_data["text"],
+                output_message=result_data["message"],
+                function=_sync_function,
+                function_async=_async_function,
+                function_name=result_data["function_call_info"]["name"],
+                function_args=result_data["function_call_info"]["arguments"],
+                function_arguments=_tool_arguments,
+            )
         else:
             return OutputWithFunctionCall(
-                    output=result,
-                    output_message=result_data["message"],
-                    output_text=result_data["text"],
-                )
+                output=result,
+                output_message=result_data["message"],
+                output_text=result_data["text"],
+            )
 
 
 class FollowupHandle(BaseCallbackHandler):
 
     def __init__(self) -> None:
         self.last_prompts = None
         self.last_messages = None
         self.last_response_generations = None
-        self.last_inputs=None
-        self.chain:LLMDecoratorChain=None
+        self.last_inputs = None
+        self.chain: LLMDecoratorChain = None
 
     def reset(self):
         self.last_prompts = None
         self.last_messages = None
         self.last_response_generations = None
-        self.last_inputs=None
-        self.chain=None
+        self.last_inputs = None
+        self.chain = None
 
     def bind_to_chain(self, chain: LLMDecoratorChain) -> None:
         """Bind callback handler to chain."""
         if self.chain is not None:
             raise Exception("FollowupHandle is already bound to a chain.")
         self.chain = chain
 
@@ -703,111 +903,162 @@
         return True
 
     @property
     def ignore_chat_model(self) -> bool:
         """Whether to ignore chat model callbacks."""
         return False
 
-    def on_chain_start(self, serialized: Dict[str, Any], inputs: Dict[str, Any], *args, **kwargs) -> Any:
-        self.last_inputs=inputs
-
-    def on_chat_model_start(self,serialized:dict, messages: List[List[BaseMessage]], *args, **kwargs):
-        if len(messages)!=1:
-            raise Exception(f"Invalid messages length {len(messages)}. FollowupHandle only supports one prompt at a time.")
+    def on_chain_start(
+        self, serialized: Dict[str, Any], inputs: Dict[str, Any], *args, **kwargs
+    ) -> Any:
+        self.last_inputs = inputs
+
+    def on_chat_model_start(
+        self, serialized: dict, messages: List[List[BaseMessage]], *args, **kwargs
+    ):
+        if len(messages) != 1:
+            raise Exception(
+                f"Invalid messages length {len(messages)}. FollowupHandle only supports one prompt at a time."
+            )
         self.last_messages = messages
-        self.last_prompts=None
+        self.last_prompts = None
 
-    def on_llm_start(self,serialized:dict, prompts: List[str], *args, **kwargs):
-        if len(prompts)!=1:
-            raise Exception(f"Invalid prompts length {len(prompts)}. FollowupHandle only supports one prompt at a time.")
+    def on_llm_start(self, serialized: dict, prompts: List[str], *args, **kwargs):
+        if len(prompts) != 1:
+            raise Exception(
+                f"Invalid prompts length {len(prompts)}. FollowupHandle only supports one prompt at a time."
+            )
         self.last_prompts = prompts
-        self.last_messages=None
+        self.last_messages = None
 
-    def on_llm_end(
-        self,
-        response: LLMResult,
-        *args,
-        **kwargs
-    ) -> None:
+    def on_llm_end(self, response: LLMResult, *args, **kwargs) -> None:
         self.last_response_generations = response.generations
 
-    def _prepare_followup_chain_with_args(self, followup_content:Union[str, BaseMessage],with_functions:bool):
+    def _prepare_followup_chain_with_args(
+        self, followup_content: Union[str, BaseMessage], with_functions: bool
+    ):
         if self.last_response_generations is None:
-            raise Exception("No response from LLM yet. Can't followup before the prompt has been executed")
-        if len(self.last_response_generations)!=1:
-            raise Exception(f"Invalid response generations length {len(self.last_response_generations)}. FollowupHandle only supports one generated response")
+            raise Exception(
+                "No response from LLM yet. Can't followup before the prompt has been executed"
+            )
+        if len(self.last_response_generations) != 1:
+            raise Exception(
+                f"Invalid response generations length {len(self.last_response_generations)}. FollowupHandle only supports one generated response"
+            )
 
-        llm = self.chain.select_llm( self.last_prompts or [ChatPromptValue(messages=self.last_messages[0])], self.last_inputs)
+        llm = self.chain.select_llm(
+            self.last_prompts or [ChatPromptValue(messages=self.last_messages[0])],
+            self.last_inputs,
+        )
 
         if self.last_messages:
             msg_list = self.last_messages[0]
             last_response_msg = self.last_response_generations[0][0].message
             msg_list.append(last_response_msg)
             if isinstance(followup_content, str):
                 followup_content = HumanMessage(content=followup_content)
 
             msg_list.append(followup_content)
             new_prompt = ChatPromptValue(messages=msg_list)
         elif self.last_prompts:
-            new_prompt = StringPromptValue(self.last_prompts[0] + self.last_response_generations[0][0].text + "\n" + followup_content)
+            new_prompt = StringPromptValue(
+                self.last_prompts[0]
+                + self.last_response_generations[0][0].text
+                + "\n"
+                + followup_content
+            )
         else:
             raise Exception("Last generation has not been recorded")
 
-        if with_functions and not isinstance(self.chain,LLMDecoratorChainWithFunctionSupport):
-            raise Exception("followup can only by used with functions if the the original llm_prompt was called with functions")
+        if with_functions and not isinstance(
+            self.chain, LLMDecoratorChainWithFunctionSupport
+        ):
+            raise Exception(
+                "followup can only by used with functions if the the original llm_prompt was called with functions"
+            )
         kwargs = {
-            "prompts":[new_prompt],
-            "stop":None,
-            "callbacks":self.chain.callbacks
+            "prompts": [new_prompt],
+            "stop": None,
+            "callbacks": self.chain.callbacks,
         }
         if with_functions:
-            kwargs["functions"]=self.chain.get_final_function_schemas(self.last_inputs)
+            kwargs["functions"] = self.chain.get_final_function_schemas(
+                self.last_inputs
+            )
 
         return llm, kwargs
 
     def _process_llm_output(self, llm_result, with_functions, with_output_parser):
         generation = llm_result.generations[0][0]
         if with_output_parser:
-            result=with_output_parser.parse(generation.text)
+            result = with_output_parser.parse(generation.text)
         else:
-            result=generation.text
-        if isinstance(generation,ChatGeneration):
+            result = generation.text
+        if isinstance(generation, ChatGeneration):
             if with_functions:
                 results_data = self.chain.create_outputs(llm_result)
 
-                self.chain._generate_output_with_function_call(result, result_data=results_data[0] if results_data else None)
+                self.chain._generate_output_with_function_call(
+                    result, result_data=results_data[0] if results_data else None
+                )
                 return self.chain.postprocess_outputs(result, results_data[0])
         else:
             if with_functions:
                 raise Exception("LLM does not support functions")
 
         return result
 
-    def followup(self, followup_content:Union[str, BaseMessage], with_functions:bool=False, with_output_parser:BaseOutputParser=None) ->Union[str, OutputWithFunctionCall, Any]:
-
-        llm, kwargs = self._prepare_followup_chain_with_args(followup_content, with_functions=with_functions)
+    def followup(
+        self,
+        followup_content: Union[str, BaseMessage],
+        with_functions: bool = False,
+        with_output_parser: BaseOutputParser = None,
+    ) -> Union[str, OutputWithFunctionCall, Any]:
+
+        llm, kwargs = self._prepare_followup_chain_with_args(
+            followup_content, with_functions=with_functions
+        )
 
         result = llm.generate_prompt(**kwargs)
 
-        return self._process_llm_output(result, with_functions,with_output_parser)
+        return self._process_llm_output(result, with_functions, with_output_parser)
 
-    async def afollowup(self, followup_content:Union[str, BaseMessage],  with_functions:bool=False, with_output_parser:BaseOutputParser=None) ->Union[str, OutputWithFunctionCall, Any]:
-        llm, kwargs = self._prepare_followup_chain_with_args(followup_content, with_functions=with_functions)
+    async def afollowup(
+        self,
+        followup_content: Union[str, BaseMessage],
+        with_functions: bool = False,
+        with_output_parser: BaseOutputParser = None,
+    ) -> Union[str, OutputWithFunctionCall, Any]:
+        llm, kwargs = self._prepare_followup_chain_with_args(
+            followup_content, with_functions=with_functions
+        )
         result = await llm.agenerate_prompt(**kwargs)
         return self._process_llm_output(result, with_functions, with_output_parser)
 
 
 class RequestRetry(Exception):
 
-    def __init__(self, feedback:str=None):
+    def __init__(self, feedback: str = None):
         super().__init__()
-        self.feedback=feedback
+        self.feedback = feedback
 
 
-def log_results(result_data, result, is_function_call=False, verbose=False, prompt_type=None):
+def log_results(
+    result_data, result, is_function_call=False, verbose=False, prompt_type=None
+):
     if verbose or prompt_type:
         if not prompt_type:
             prompt_type = PromptTypes.UNDEFINED
-        print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
+        print_log(
+            log_object=f"\nResult:\n{result}",
+            log_level=prompt_type.log_level if not verbose else 100,
+            color=prompt_type.color if prompt_type else LogColors.BLUE,
+        )
         if is_function_call:
-            function_call_info_str = json.dumps(result_data.get('function_call_info'),indent=4)
-            print_log(log_object=f"\nFunction call:\n{function_call_info_str}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
+            function_call_info_str = json.dumps(
+                result_data.get("function_call_info"), indent=4
+            )
+            print_log(
+                log_object=f"\nFunction call:\n{function_call_info_str}",
+                log_level=prompt_type.log_level if not verbose else 100,
+                color=prompt_type.color if prompt_type else LogColors.BLUE,
+            )
```

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/common.py` & `langchain_decorators-0.5.7/src/langchain_decorators/common.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/function_decorator.py` & `langchain_decorators-0.5.7/src/langchain_decorators/function_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/output_parsers.py` & `langchain_decorators-0.5.7/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/prompt_decorator.py` & `langchain_decorators-0.5.7/src/langchain_decorators/prompt_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 import asyncio
-import logging
 import inspect
-
+import logging
 from functools import wraps
 from types import coroutine
-from typing import Any, Callable, Dict, List, Optional,  Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
-
-from langchain.tools.base import BaseTool
-from langchain.schema import BaseOutputParser
 from langchain.llms.base import BaseLanguageModel
+from langchain.schema import BaseOutputParser
+from langchain.tools.base import BaseTool
 
-
-from .chains import LLMDecoratorChainWithFunctionSupport, LLMDecoratorChain, RequestRetry
+from .chains import (
+    LLMDecoratorChain,
+    LLMDecoratorChainWithFunctionSupport,
+    RequestRetry,
+)
 from .common import *
-from .prompt_template import PromptDecoratorTemplate
+from .function_decorator import get_dynamic_function_template_args, is_dynamic_llm_func
 from .output_parsers import *
+from .prompt_template import PromptDecoratorTemplate
 from .schema import OutputWithFunctionCall
 from .streaming_context import StreamingContext
-from .function_decorator import is_dynamic_llm_func, get_dynamic_function_template_args
 
+SPECIAL_KWARGS = [
+    "callbacks",
+    "followup_handle",
+    "llm_selector_rule_key",
+    "memory",
+    "functions",
+    "function_call",
+    "capture_stream",
+    "llm_selector_rule_key",
+    "stop",
+    "output_parser",
+    "llm_kwargs",
+    "llm",
+]
 
-SPECIAL_KWARGS=["callbacks","followup_handle","llm_selector_rule_key","memory","functions","function_call","capture_stream","llm_selector_rule_key", "stop", "output_parser", "llm_kwargs"]
 
 def llm_prompt(
-        prompt_type:PromptTypeSettings=PromptTypes.UNDEFINED, # do not change the order of this first parameter unless you will change also the fist few lines... since we are handling cases when decorator is used with and without arguments too, than this will be the func
-        template_format:str = "f-string-extra",
-        output_parser:Union[str,None, BaseOutputParser]="auto", 
-        stop_tokens:List[str]=None, 
-        template_name:str=None, 
-        template_version:str=None, 
-        capture_stream:bool=None,
-        llm:Optional[BaseLanguageModel]=None,
-        format_instructions_parameter_key:str="FORMAT_INSTRUCTIONS",
-        retry_on_output_parsing_error:bool=True,
-        verbose:bool=None,
-        expected_gen_tokens:Optional[int]=None,
-        llm_selector_rule_key:Optional[str]=None,
-        llm_selector:Optional[LlmSelector]=None,
-        functions_source:str=None,
-        memory_source:str=None,
-        control_kwargs:List[str]=SPECIAL_KWARGS
-        ):
+    prompt_type: PromptTypeSettings = PromptTypes.UNDEFINED,  # do not change the order of this first parameter unless you will change also the fist few lines... since we are handling cases when decorator is used with and without arguments too, than this will be the func
+    template_format: str = "f-string-extra",
+    output_parser: Union[str, None, BaseOutputParser] = "auto",
+    stop_tokens: List[str] = None,
+    template_name: str = None,
+    template_version: str = None,
+    capture_stream: bool = None,
+    llm: Optional[BaseLanguageModel] = None,
+    format_instructions_parameter_key: str = "FORMAT_INSTRUCTIONS",
+    retry_on_output_parsing_error: bool = True,
+    verbose: bool = None,
+    expected_gen_tokens: Optional[int] = None,
+    llm_selector_rule_key: Optional[str] = None,
+    llm_selector: Optional[LlmSelector] = None,
+    functions_source: str = None,
+    memory_source: str = None,
+    control_kwargs: List[str] = SPECIAL_KWARGS,
+):
     """
     Decorator for functions that turns a regular function into a LLM prompt executed with default model and settings.
-    
-    This can be applied on any function that has a docstring with a prompt template. 
+
+    This can be applied on any function that has a docstring with a prompt template.
     If the function is async, the prompt will be executed asynchronously (with all the langchain async infrastructure).
 
-    Note that the code of the function will never be executed... 
+    Note that the code of the function will never be executed...
 
     Args:
         `prompt_type`: (Optional[PromptTypeSettings]) - This allows you mark your prompt with one of the predefined prompt types (see PromptTypes class - but you can subclass it!) to predefine some settings like LLM or style and color of logging into console.
 
         `template_format` (Optional[str]): one of [ `f-string` | `f-string-extra` ] ... f-string-extra is a superset of f-string template formats, enabling for optional sections.
 
-        `output_parser` (Optional[str]): one of [ `auto` | `json` | `str` | `list` ] or `None` or langchain OutputParser object - you can control how will the output be parsed. 
-        
+        `output_parser` (Optional[str]): one of [ `auto` | `json` | `str` | `list` ] or `None` or langchain OutputParser object - you can control how will the output be parsed.
+
             `auto` - default - determine the output type automatically based on output type annotations
 
             `str` or `None` - will return plain string output
 
             `list` - will parse bullet or numbered list (each item on a new line) as a list
 
             `boolean` - will parse the output as boolean. Expects clear Yes/No in the output
@@ -72,112 +86,142 @@
             `markdown` - will parse the output as markdown sections, the name of each section will be returned as a key and the content as a value. For nested sections, the value will be a dict with the same structure.
 
             `pydantic` - will parse the output as json and then convert into a pydantic model
 
 
         `stop_tokens` (Optional[List[str]]): list of stop tokens to instruct the LLM to stop generating text when it encounters any of these tokens. If not provided, the default stop tokens of the LLM will be used.
 
-        `format_instructions_parameter_key` - name of the format instructions parameter - this will enable you to include the instructions on how LLM should format the output, generated by the output_parsers 
-        ... if you include this into your prompt (docs), you don't need to reinvent the formatting instructions. 
+        `format_instructions_parameter_key` - name of the format instructions parameter - this will enable you to include the instructions on how LLM should format the output, generated by the output_parsers
+        ... if you include this into your prompt (docs), you don't need to reinvent the formatting instructions.
         This works pretty well if you have an annotated pydantic model as an function output. If you are expecting a dict, you should probably include your own formatting instructions, since there is not much to infer from a dict structure.
 
         `retry_on_output_parsing_error` - whether to try to re-format the output if the output parser fails to parse the output by another LLM call
 
         `verbose` - whether to print the response from LLM into console
 
         `expected_gen_tokens` - hint for LLM selector ... if not set, default values of the LLM selector will be used (usually 1/3 of the prompt length)
 
-        `llm_selector_rule_key` - key of the LLM selector rule to use ... if set, only LLMs with assigned rule with this key will be considered. You can also use llm_selector_rule_key argument when calling the llm_prompt function to override the default rule key. 
+        `llm_selector_rule_key` - key of the LLM selector rule to use ... if set, only LLMs with assigned rule with this key will be considered. You can also use llm_selector_rule_key argument when calling the llm_prompt function to override the default rule key.
 
         `functions_source` - only for bound functions ... name of a field or property on `self` that should be used as a source of functions for the OpenAI functions. If not set, you still can pass in functions as an argument, which will also override this.
 
         `control_kwargs` - kwargs that only controls other the behavior, and shall not be passed as template arguments. These are: `callbacks`, `followup_handle`, `llm_selector_rule_key`, `memory`, `functions`, `function_call`, `capture_stream`, `llm_selector_rule_key`, `stop`
     """
 
-    if  callable(prompt_type):
+    if callable(prompt_type):
         # this is the case when the decorator is called without arguments
         # we initialize params with default values
         func = prompt_type
         prompt_type = PromptTypes.UNDEFINED
     else:
         func = None
 
     if verbose is None:
         verbose = GlobalSettings.get_current_settings().verbose
 
     if verbose:
         if prompt_type:
             prompt_type = prompt_type.as_verbose()
         else:
-            prompt_type = PromptTypeSettings(color=LogColors.DARK_GRAY,log_level=100, capture_stream=capture_stream)
+            prompt_type = PromptTypeSettings(
+                color=LogColors.DARK_GRAY, log_level=100, capture_stream=capture_stream
+            )
 
     def decorator(func):
-        name=func.__name__
+        name = func.__name__
 
-        full_name=f"{func.__module__}.{name}" if func.__module__!="__main__" else name
+        full_name = (
+            f"{func.__module__}.{name}" if func.__module__ != "__main__" else name
+        )
         is_async = inspect.iscoroutinefunction(func)
 
-        _llm_selector_rule_key=llm_selector_rule_key
+        _llm_selector_rule_key = llm_selector_rule_key
 
         if prompt_type:
-            _capture_stream = prompt_type.capture_stream if capture_stream is None else capture_stream
+            _capture_stream = (
+                prompt_type.capture_stream if capture_stream is None else capture_stream
+            )
         else:
             _capture_stream = capture_stream
         if _capture_stream and not is_async:
-            print_log(f"Warning: capture_stream=True is only supported for async functions. Ignoring capture_stream for {full_name}", logging.WARNING, LogColors.YELLOW)
-            _capture_stream=False
+            print_log(
+                f"Warning: capture_stream=True is only supported for async functions. Ignoring capture_stream for {full_name}",
+                logging.WARNING,
+                LogColors.YELLOW,
+            )
+            _capture_stream = False
 
         @wraps(func)
-        def build_chain(*args, **kwargs)->LLMDecoratorChain:
+        def build_chain(*args, **kwargs) -> LLMDecoratorChain:
             global_settings = GlobalSettings.get_current_settings()
 
-            capture_stream=_capture_stream
+            capture_stream = _capture_stream
 
             if "capture_stream" in kwargs:
-                if not isinstance(capture_stream,bool):
-                    raise ValueError("capture_stream is a reserved kwarg and must be of type bool")
-                capture_stream=kwargs["capture_stream"]
+                if not isinstance(capture_stream, bool):
+                    raise ValueError(
+                        "capture_stream is a reserved kwarg and must be of type bool"
+                    )
+                capture_stream = kwargs["capture_stream"]
                 del kwargs["capture_stream"]
 
             if capture_stream and not StreamingContext.get_context():
-                print_log(f"INFO: Not inside StreamingContext. Ignoring capture_stream for {full_name}", logging.DEBUG, LogColors.WHITE)
-                capture_stream=False
+                print_log(
+                    f"INFO: Not inside StreamingContext. Ignoring capture_stream for {full_name}",
+                    logging.DEBUG,
+                    LogColors.WHITE,
+                )
+                capture_stream = False
 
             if "followup_handle" in kwargs:
-                followup_handle=kwargs["followup_handle"]
+                followup_handle = kwargs["followup_handle"]
                 del kwargs["followup_handle"]
             else:
-                followup_handle=None
+                followup_handle = None
 
-            if not (llm or (prompt_type and prompt_type.llm)):
+            if not (llm or (prompt_type and prompt_type.llm)) and "llm" not in kwargs:
                 if llm_selector:
-                    _llm_selector= llm_selector
+                    _llm_selector = llm_selector
                 elif prompt_type and prompt_type.llm_selector:
-                    _llm_selector= prompt_type.llm_selector
+                    _llm_selector = prompt_type.llm_selector
                 else:
-                    _llm_selector=  global_settings.llm_selector 
+                    _llm_selector = global_settings.llm_selector
 
                 if capture_stream and not _llm_selector:
                     if not global_settings.default_streaming_llm:
-                        print_log(f"Warning: capture_stream on {name} is on, but the default LLM {llm} doesn't seem to be supporting streaming.", logging.WARNING, LogColors.YELLOW)
+                        print_log(
+                            f"Warning: capture_stream on {name} is on, but the default LLM {llm} doesn't seem to be supporting streaming.",
+                            logging.WARNING,
+                            LogColors.YELLOW,
+                        )
 
-                    prompt_llm=global_settings.default_streaming_llm or global_settings.default_llm
+                    prompt_llm = (
+                        global_settings.default_streaming_llm
+                        or global_settings.default_llm
+                    )
                 else:
                     prompt_llm = global_settings.default_llm
 
+                if "llm" in kwargs:
+                    prompt_llm = kwargs["llm"]
                 if "llm_selector_rule_key" in kwargs:
-                    llm_selector_rule_key=kwargs["llm_selector_rule_key"]
+                    llm_selector_rule_key = kwargs["llm_selector_rule_key"]
                     del kwargs["llm_selector_rule_key"]
                 else:
-                    llm_selector_rule_key=_llm_selector_rule_key
+                    llm_selector_rule_key = _llm_selector_rule_key
 
             else:
-                prompt_llm=llm or prompt_type.llm
-                llm_selector_rule_key=None
-                _llm_selector=None # if LLM is explicitly provided, we don't use the selector
+                if "llm" in kwargs:
+                    prompt_llm = kwargs["llm"]
+                else:
+                    prompt_llm = llm or prompt_type.llm
+                # if LLM is explicitly provided, we don't use the selector
+                llm_selector_rule_key = None
+                _llm_selector = None
+
                 if capture_stream:
                     if hasattr(prompt_llm, "streaming"):
                         if not getattr(prompt_llm, "streaming"):
                             print_log(
                                 f"Warning: capture_stream on {name} is on, but the provided LLM {prompt_llm} doesn't have streaming on! Stream wont be captured",
                                 logging.WARNING,
                                 LogColors.YELLOW,
@@ -185,245 +229,330 @@
                     else:
                         print_log(
                             f"Warning: capture_stream on {name} is on, but the provided LLM {prompt_llm} doesn't seem to be supporting streaming.",
                             logging.WARNING,
                             LogColors.YELLOW,
                         )
 
-            _self=None
-            if len(args)==1 and hasattr(args[0],"__dict__"):
+            _self = None
+            if len(args) == 1 and hasattr(args[0], "__dict__"):
                 # is a proper object
                 _self = args[0]
 
-            elif len(args)>1:
-                raise Exception(f"Positional arguments are not supported for prompt functions. Only one positional argument as an object with attributes as a source of inputs is supported. Got: {args}")
-
-            prompt_template = PromptDecoratorTemplate.from_func(func, 
-                                                            template_format=template_format, 
-                                                            output_parser=output_parser, 
-                                                            format_instructions_parameter_key=format_instructions_parameter_key,
-                                                            template_name=template_name,
-                                                            template_version=template_version,
-                                                            prompt_type=prompt_type,
-                                                            original_kwargs=kwargs
-                                                            )
+            elif len(args) > 1:
+                raise Exception(
+                    f"Positional arguments are not supported for prompt functions. Only one positional argument as an object with attributes as a source of inputs is supported. Got: {args}"
+                )
+
+            prompt_template = PromptDecoratorTemplate.from_func(
+                func,
+                template_format=template_format,
+                output_parser=output_parser,
+                format_instructions_parameter_key=format_instructions_parameter_key,
+                template_name=template_name,
+                template_version=template_version,
+                prompt_type=prompt_type,
+                original_kwargs=kwargs,
+            )
 
             if prompt_template.default_values:
                 kwargs = {**prompt_template.default_values, **kwargs}
 
             if "output_parser" in kwargs:
-                callbacks=kwargs.pop("output_parser")
+                callbacks = kwargs.pop("output_parser")
 
             if "callbacks" in kwargs:
-                callbacks=kwargs.pop("callbacks")
+                callbacks = kwargs.pop("callbacks")
             else:
-                callbacks=[]
+                callbacks = []
 
             if capture_stream:
                 callbacks.append(StreamingContext.StreamingContextCallback())
 
             if "memory" in kwargs:
                 memory = kwargs.pop("memory")
             else:
                 if memory_source:
                     if _self:
                         memory = getattr(_self, memory_source)
                     else:
-                        raise Exception(f"memory_source can only be used on bound functions (arg[0] is not set)")
+                        raise Exception(
+                            f"memory_source can only be used on bound functions (arg[0] is not set)"
+                        )
                 else:
-                    memory=None
+                    memory = None
 
             if "functions" in kwargs:
-                functions=kwargs.pop("functions")
+                functions = kwargs.pop("functions")
             else:
                 if functions_source:
                     if _self:
                         functions = getattr(_self, functions_source)
                         if functions is None:
-                            logging.warning(f"{functions_source} didn't return any value. Return an empty array if this is intended scenario and you don't want to provide any functions for this call")
+                            logging.warning(
+                                f"{functions_source} didn't return any value. Return an empty array if this is intended scenario and you don't want to provide any functions for this call"
+                            )
                     else:
-                        raise Exception(f"functions_source can only be used on bound functions (arg[0] is not set)")
+                        raise Exception(
+                            f"functions_source can only be used on bound functions (arg[0] is not set)"
+                        )
                 else:
-                    functions=None
+                    functions = None
 
-            llm_kwargs=None
+            llm_kwargs = None
             if "llm_kwargs" in kwargs:
-                llm_kwargs=kwargs.pop("llm_kwargs")
+                llm_kwargs = kwargs.pop("llm_kwargs")
 
-            func_args=set()
+            func_args = set()
 
-            chain_kwargs={
-                "llm":prompt_llm, 
-                "name":name,
-                "prompt":prompt_template, 
-                "memory":memory, 
-                
-                "llm_selector":_llm_selector, 
-                "llm_selector_rule_key":llm_selector_rule_key,
-                "capture_stream":capture_stream, 
-                "expected_gen_tokens":expected_gen_tokens, 
-                "format_instructions_parameter_key":format_instructions_parameter_key,
+            chain_kwargs = {
+                "llm": prompt_llm,
+                "name": name,
+                "prompt": prompt_template,
+                "memory": memory,
+                "llm_selector": _llm_selector,
+                "llm_selector_rule_key": llm_selector_rule_key,
+                "capture_stream": capture_stream,
+                "expected_gen_tokens": expected_gen_tokens,
+                "format_instructions_parameter_key": format_instructions_parameter_key,
                 "prompt_type": prompt_type or PromptTypes.UNDEFINED,
-                "allow_retries":retry_on_output_parsing_error,
-                "llm_kwargs":llm_kwargs or {}
+                "allow_retries": retry_on_output_parsing_error,
+                "llm_kwargs": llm_kwargs or {},
             }
 
             if functions is not None:
                 for llm_func in functions:
                     if is_dynamic_llm_func(llm_func):
-                        required, optional = get_dynamic_function_template_args(llm_func)
-                        for k,v in inspect.signature(llm_func).parameters.items():
-                            if v.default!=inspect.Parameter.empty:
+                        required, optional = get_dynamic_function_template_args(
+                            llm_func
+                        )
+                        for k, v in inspect.signature(llm_func).parameters.items():
+                            if v.default != inspect.Parameter.empty:
                                 optional.add(k)
                                 if k in required:
                                     required.remove(k)
                         func_args.update(required)
                         func_args.update(optional)
-                        additional_variable_source = getattr(llm_func,"__self__",None)
-                        kwargs = validate_and_enrich_kwargs(kwargs, _self,  memory,required, optional, additional_variable_source)
-
-                llmChain = LLMDecoratorChainWithFunctionSupport(**chain_kwargs,  functions=functions)
+                        additional_variable_source = getattr(llm_func, "__self__", None)
+                        kwargs = validate_and_enrich_kwargs(
+                            kwargs,
+                            _self,
+                            memory,
+                            required,
+                            optional,
+                            additional_variable_source,
+                        )
 
-            elif isinstance(prompt_template.output_parser, OpenAIFunctionsPydanticOutputParser):
-                function=prompt_template.output_parser.build_llm_function()
+                llmChain = LLMDecoratorChainWithFunctionSupport(
+                    **chain_kwargs, functions=functions
+                )
+
+            elif isinstance(
+                prompt_template.output_parser, OpenAIFunctionsPydanticOutputParser
+            ):
+                function = prompt_template.output_parser.build_llm_function()
                 kwargs["function_call"] = function
-                llmChain = LLMDecoratorChainWithFunctionSupport(**chain_kwargs, functions=[function])
+                llmChain = LLMDecoratorChainWithFunctionSupport(
+                    **chain_kwargs, functions=[function]
+                )
             else:
                 llmChain = LLMDecoratorChain(**chain_kwargs)
 
-            reserved_inputs_violations=[key for key in prompt_template.input_variables if key in control_kwargs]
+            reserved_inputs_violations = [
+                key for key in prompt_template.input_variables if key in control_kwargs
+            ]
             if reserved_inputs_violations:
-                raise Exception(f"Invalid prompt template: {reserved_inputs_violations} are reserved prompt arguments and cannot be used in prompt template.")
-
-            unexpected_inputs = [key for key in kwargs if  key not in prompt_template.input_variables and key not in control_kwargs and key not in func_args ]
+                raise Exception(
+                    f"Invalid prompt template: {reserved_inputs_violations} are reserved prompt arguments and cannot be used in prompt template."
+                )
+
+            unexpected_inputs = [
+                key
+                for key in kwargs
+                if key not in prompt_template.input_variables
+                and key not in control_kwargs
+                and key not in func_args
+                and key not in SPECIAL_KWARGS
+            ]
             if unexpected_inputs:
-                raise TypeError(f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}\nHint: Make sure that you've used all the inputs in the template")
-
-            kwargs = validate_and_enrich_kwargs(kwargs, _self,  memory,prompt_template.input_variables)
+                raise TypeError(
+                    f"Unexpected inputs for prompt function {full_name}: {unexpected_inputs}. \nValid inputs are: {prompt_template.input_variables}\nHint: Make sure that you've used all the inputs in the template"
+                )
+
+            kwargs = validate_and_enrich_kwargs(
+                kwargs, _self, memory, prompt_template.input_variables
+            )
 
             if followup_handle:
                 followup_handle.bind_to_chain(llmChain)
                 if callbacks:
                     callbacks.append(followup_handle)
                 else:
-                    callbacks=[followup_handle]
+                    callbacks = [followup_handle]
 
             if stop_tokens:
-                kwargs["stop"]=stop_tokens
-            call_args = {"inputs":kwargs, "return_only_outputs":True, "callbacks":callbacks}
-            if llm_kwargs:
-                call_args["llm_kwargs"]=llm_kwargs
+                kwargs["stop"] = stop_tokens
+            call_args = {
+                "inputs": kwargs,
+                "return_only_outputs": True,
+                "callbacks": callbacks,
+            }
+
             llmChain.default_call_kwargs = call_args
 
             return llmChain
 
-        def validate_and_enrich_kwargs(kwargs, input_variables_source, memory, required_args, optional_args=None, additional_input_variables_source=None):
-            missing_inputs = [ key for key in required_args if key not in kwargs ]
+        def validate_and_enrich_kwargs(
+            kwargs,
+            input_variables_source,
+            memory,
+            required_args,
+            optional_args=None,
+            additional_input_variables_source=None,
+        ):
+            missing_inputs = [key for key in required_args if key not in kwargs]
             if optional_args:
-                missing_inputs.extend([key for key in optional_args if key not in kwargs ])
+                missing_inputs.extend(
+                    [key for key in optional_args if key not in kwargs]
+                )
             if format_instructions_parameter_key in missing_inputs:
                 missing_inputs.remove(format_instructions_parameter_key)
-                kwargs[format_instructions_parameter_key]=None #init the format instructions with None... will be filled later
+                kwargs[format_instructions_parameter_key] = (
+                    None  # init the format instructions with None... will be filled later
+                )
             if memory and memory.memory_key in missing_inputs:
                 missing_inputs.remove(memory.memory_key)
 
-            def get_value_ext(source, key:str, default):
+            def get_value_ext(source, key: str, default):
                 # this doesnśt work since native python Formatter doesn't support "." in keys
                 # if "." in key:
                 #     key, subpath = key.split(".",1)
                 # else:
-                subpath=None
+                subpath = None
 
-                if isinstance(source,dict):
+                if isinstance(source, dict):
                     value = source.get(key, default)
                 else:
                     value = getattr(source, key, default)
 
                 if subpath and value and value != default:
                     return get_value_ext(value, subpath, default)
                 else:
                     return value
 
             if missing_inputs:
-                missing_value={}
+                missing_value = {}
                 for key in missing_inputs:
                     if input_variables_source or additional_input_variables_source:
-                        value= get_value_ext(input_variables_source, key,missing_value)
+                        value = get_value_ext(
+                            input_variables_source, key, missing_value
+                        )
                         if value is missing_value:
-                            value= get_value_ext(additional_input_variables_source, key,missing_value)
+                            value = get_value_ext(
+                                additional_input_variables_source, key, missing_value
+                            )
                     else:
-                        value=missing_value
+                        value = missing_value
 
                     if value is missing_value:
-                        value= get_value_ext(kwargs, key,missing_value)
+                        value = get_value_ext(kwargs, key, missing_value)
                         if value is missing_value:
                             if optional_args and key in optional_args:
                                 continue
 
-                            raise TypeError(f"Missing a input for prompt function {full_name}: {key}.")
+                            raise TypeError(
+                                f"Missing a input for prompt function {full_name}: {key}."
+                            )
 
                     kwargs[key] = value
             return kwargs
 
-        def get_preprocessing_args_by_running_func(*args,**kwargs):
+        def get_preprocessing_args_by_running_func(*args, **kwargs):
             # temporary, we should always declare the args we want to use, but its not backward compatible
-            kwargs_keys =  [*inspect.signature(func).parameters.keys()]
+            kwargs_keys = [*inspect.signature(func).parameters.keys()]
 
             _extra_kwargs = [k for k in kwargs if k not in kwargs_keys]
 
             if _extra_kwargs:
-                logging.warning(f"We should always declare all arguments of @llm_prompt if we are planning to use them. {_extra_kwargs} extra kwargs found...")
-                _result = func(*args,**{k:v for k,v in kwargs.items() if k not in _extra_kwargs})
+                logging.warning(
+                    f"We should always declare all arguments of @llm_prompt if we are planning to use them. {_extra_kwargs} extra kwargs found..."
+                )
+                _result = func(
+                    *args, **{k: v for k, v in kwargs.items() if k not in _extra_kwargs}
+                )
             else:
                 # use only this in the future
-                _result = func(*args,**kwargs)
+                _result = func(*args, **kwargs)
 
             return _result
 
         if not is_async:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
-                _kwargs = get_preprocessing_args_by_running_func(*args,**kwargs)
+                _kwargs = get_preprocessing_args_by_running_func(*args, **kwargs)
 
                 if _kwargs:
-                    if not isinstance(_kwargs,dict):
-                        raise Exception(f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}")
+                    if not isinstance(_kwargs, dict):
+                        raise Exception(
+                            f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}"
+                        )
                     kwargs.update(_kwargs)
 
                 llmChain = build_chain(*args, **kwargs)
                 return llmChain.execute()
-            wrapper.build_chain=build_chain
+
+            wrapper.build_chain = build_chain
 
             if inspect.signature(func).parameters.get("functions"):
-                if not func.__annotations__.get('return') or func.__annotations__.get('return') == OutputWithFunctionCall:
-                    wrapper.__annotations__['return']= OutputWithFunctionCall
+                if (
+                    not func.__annotations__.get("return")
+                    or func.__annotations__.get("return") == OutputWithFunctionCall
+                ):
+                    wrapper.__annotations__["return"] = OutputWithFunctionCall
                 else:
-                    wrapper.__annotations__['return']= OutputWithFunctionCall[func.__annotations__.get('return') ]
+                    wrapper.__annotations__["return"] = OutputWithFunctionCall[
+                        func.__annotations__.get("return")
+                    ]
 
             return wrapper
 
         else:
+
             @wraps(func)
             async def async_wrapper(*args, **kwargs):
 
-                _kwargs = await get_preprocessing_args_by_running_func(*args,**kwargs)
+                _kwargs = await get_preprocessing_args_by_running_func(*args, **kwargs)
                 if _kwargs:
-                    if not isinstance(_kwargs,dict):
-                        raise Exception(f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}")
+                    if not isinstance(_kwargs, dict):
+                        raise Exception(
+                            f"Invalid @llm_prompt implementation: the result of the function call must be a dict, to augment the input args. Got: {_kwargs}"
+                        )
                     kwargs.update(_kwargs)
 
                 llmChain = build_chain(*args, **kwargs)
 
                 return await llmChain.aexecute()
 
-            async_wrapper.build_chain=build_chain
+            async_wrapper.build_chain = build_chain
             if inspect.signature(func).parameters.get("functions"):
-                if not func.__annotations__.get('return') or func.__annotations__.get('return') == OutputWithFunctionCall  or func.__annotations__.get('return') ==  Coroutine[Any,Any,OutputWithFunctionCall]:
-                    async_wrapper.__annotations__['return'] = Coroutine[Any,Any,OutputWithFunctionCall]
+                if (
+                    not func.__annotations__.get("return")
+                    or func.__annotations__.get("return") == OutputWithFunctionCall
+                    or func.__annotations__.get("return")
+                    == Coroutine[Any, Any, OutputWithFunctionCall]
+                ):
+                    async_wrapper.__annotations__["return"] = Coroutine[
+                        Any, Any, OutputWithFunctionCall
+                    ]
                 else:
-                    async_wrapper.__annotations__['return'] = Coroutine[Any,Any,OutputWithFunctionCall[func.__annotations__.get('return') ]]
+                    async_wrapper.__annotations__["return"] = Coroutine[
+                        Any,
+                        Any,
+                        OutputWithFunctionCall[func.__annotations__.get("return")],
+                    ]
             return async_wrapper
+
     if func:
         return decorator(func)
     else:
         return decorator
```

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/prompt_template.py` & `langchain_decorators-0.5.7/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/pydantic_helpers.py` & `langchain_decorators-0.5.7/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/schema.py` & `langchain_decorators-0.5.7/src/langchain_decorators/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators/streaming_context.py` & `langchain_decorators-0.5.7/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators.egg-info/PKG-INFO` & `langchain_decorators-0.5.7/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.6
+Version: 0.5.7
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain_decorators-0.5.6/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain_decorators-0.5.7/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

