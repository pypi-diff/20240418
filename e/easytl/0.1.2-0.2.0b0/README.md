# Comparing `tmp/easytl-0.1.2.tar.gz` & `tmp/easytl-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.1.2.tar", last modified: Mon Apr 15 23:23:12 2024, max compression
+gzip compressed data, was "easytl-0.2.0b0.tar", last modified: Thu Apr 18 11:09:33 2024, max compression
```

## Comparing `easytl-0.1.2.tar` & `easytl-0.2.0b0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.929459 easytl-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.925459 easytl-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.925459 easytl-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-15 23:23:01.000000 easytl-0.1.2/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-15 23:23:01.000000 easytl-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-15 23:23:01.000000 easytl-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-15 23:23:12.929459 easytl-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-15 23:23:01.000000 easytl-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-15 23:23:01.000000 easytl-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 23:23:01.000000 easytl-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:23:12.929459 easytl-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.925459 easytl-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.929459 easytl-0.1.2/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    40712 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 23:23:01.000000 easytl-0.1.2/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:23:12.929459 easytl-0.1.2/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-15 23:23:12.000000 easytl-0.1.2/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-15 23:23:12.000000 easytl-0.1.2/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:23:12.000000 easytl-0.1.2/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 23:23:12.000000 easytl-0.1.2/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 23:23:12.000000 easytl-0.1.2/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.831990 easytl-0.2.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 11:09:20.000000 easytl-0.2.0b0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-18 11:09:20.000000 easytl-0.2.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 11:09:20.000000 easytl-0.2.0b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-18 11:09:33.839990 easytl-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-18 11:09:20.000000 easytl-0.2.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 11:09:20.000000 easytl-0.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:09:33.839990 easytl-0.2.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.835990 easytl-0.2.0b0/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49369 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17868 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 11:09:20.000000 easytl-0.2.0b0/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:09:33.000000 easytl-0.2.0b0/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:09:33.839990 easytl-0.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 11:09:20.000000 easytl-0.2.0b0/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-18 11:09:20.000000 easytl-0.2.0b0/tests/passing.py
```

### Comparing `easytl-0.1.2/.github/workflows/workflow.yml` & `easytl-0.2.0b0/.github/workflows/workflow.yml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     types: [published]
 
 jobs:
   build_and_publish:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', '3.12']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     steps:
       - name: Checkout code
         uses: actions/checkout@v2
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
@@ -25,12 +25,13 @@
           python -m pip install twine build
 
       - name: Build the package
         run: |
           python -m build
 
       - name: Publish the package to PyPI
+        if: matrix.python-version == '3.8'
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
           python -m twine upload dist/*
```

### Comparing `easytl-0.1.2/.gitignore` & `easytl-0.2.0b0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -155,7 +155,12 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 .vscode/settings.json
+
+## test files
+tests/gemini.txt
+tests/openai.txt
+tests/deepl.txt
```

### Comparing `easytl-0.1.2/LICENSE.md` & `easytl-0.2.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.1.2/PKG-INFO` & `easytl-0.2.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.1.2
+Version: 0.2.0b0
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.0
+Requires-Dist: google-generativeai==0.5.1
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
@@ -33,14 +33,17 @@
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
 Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 
+EasyTL has a trello board:
+https://trello.com/b/Td555CoW/easytl
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
@@ -94,15 +97,15 @@
 
 wheel
 
 setuptools_scm>=6.0
 
 tomli
 
-google-generativeai==0.5.0
+google-generativeai==0.5.1
 
 deepl==1.16.1
 
 openai==1.13.3
 
 backoff==2.2.1
```

### Comparing `easytl-0.1.2/README.md` & `easytl-0.2.0b0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
 Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 
+EasyTL has a trello board:
+https://trello.com/b/Td555CoW/easytl
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
@@ -71,15 +74,15 @@
 
 wheel
 
 setuptools_scm>=6.0
 
 tomli
 
-google-generativeai==0.5.0
+google-generativeai==0.5.1
 
 deepl==1.16.1
 
 openai==1.13.3
 
 backoff==2.2.1
```

### Comparing `easytl-0.1.2/pyproject.toml` & `easytl-0.2.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     "tomli"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [
-    "google-generativeai==0.5.0",
+    "google-generativeai==0.5.1",
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0"
 ]
 
 name = "easytl"
-version = "v0.1.2"
+version = "v0.2.0-beta"
 authors = [
   { name="Bikatr7", email="Tetralon07@gmail.com" },
 ]
 description = "Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `easytl-0.1.2/src/easytl/classes.py` & `easytl-0.2.0b0/src/easytl/classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ## Copyright Bikatr7 (https://github.com/Bikatr7)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## deepl api data used by deepl_service to type check
 from deepl.api_data import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 
+## openai api data used by openai_service to type check
+from openai.types.chat.chat_completion import ChatCompletion
+
+## gemini api data used by gemini_service to type check
+from google.generativeai import GenerationConfig
+from google.generativeai.types import GenerateContentResponse, AsyncGenerateContentResponse
+
 ##-------------------start-of-Message--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 class Message:
 
     """
 
     Message is a class that is used to send translation batches to the OpenAI API.
@@ -30,14 +37,17 @@
         return {
             'role': self.role,
             'content': self.content
         }
     
     def __str__(self) -> str:
         return self.content
+    
+    def __repr__(self):
+        return f"<Message role={self.role} content='{self.content}'>"
 
 ##-------------------start-of-SystemTranslationMessage--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 class SystemTranslationMessage(Message):
 
     """
```

### Comparing `easytl-0.1.2/src/easytl/deepl_service.py` & `easytl-0.2.0b0/src/easytl/deepl_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 import asyncio
 
 ## third-party libraries
 from deepl.translator import Translator
 
 from .util import _convert_iterable_to_str
+from .decorators import _async_logging_decorator, _sync_logging_decorator
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 
 class DeepLService:
 
     _api_key:str = ""
     
     _translator:Translator
@@ -28,51 +29,54 @@
     _tag_handling:typing.Literal["xml", "html"] | None = None
     _outline_detection:bool | None = None
     _non_splitting_tags:str | typing.List[str] | None = None
     _splitting_tags:str | typing.List[str] | None = None
     _ignore_tags:str | typing.List[str] | None = None
 
     _semaphore_value:int = 30
-
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
+    _log_directory:str | None = None
+
 ##-------------------start-of-_set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def _set_decorator(decorator:typing.Callable) -> None:
+    def _set_decorator(decorator:typing.Callable | None) -> None:
 
         """
 
-        Sets the decorator to use for the Gemini service. Should be a callable that returns a decorator.
+        Sets the decorator to use for the DeepL service. Should be a callable that returns a decorator or None.
 
         Parameters:
-        decorator (callable) : The decorator to use.
+        decorator (callable or None) : The decorator to use for the DeepL service.
 
         """
 
         DeepLService._decorator_to_use = decorator
 
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     def _set_attributes(target_lang:str | Language = "EN",
                         source_lang:str | Language | None = None,
                         context:str | None = None,
                         split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                         preserve_formatting:bool | None = None,
-                        semaphore:int | None = None,
                         formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                         glossary:str | GlossaryInfo | None = None,
                         tag_handling:typing.Literal["xml", "html"] | None = None,
                         outline_detection:bool | None = None,
                         non_splitting_tags:str | typing.List[str] | None = None,
                         splitting_tags:str | typing.List[str] | None = None,
-                        ignore_tags:str | typing.List[str] | None = None) -> None:
+                        ignore_tags:str | typing.List[str] | None = None,
+                        semaphore:int | None = None,
+                        logging_directory:str | None = None,
+                        ) -> None:
 
         """
 
         Sets the attributes of the DeepL client.
 
         """
 
@@ -89,14 +93,16 @@
         DeepLService._splitting_tags = splitting_tags
         DeepLService._ignore_tags = ignore_tags
 
         if(semaphore is not None):
             DeepLService._semaphore_value = semaphore
             DeepLService._semaphore = asyncio.Semaphore(semaphore)
 
+        DeepLService._log_directory = logging_directory
+
 ##-------------------start-of-_prepare_translation_parameters()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _prepare_translation_parameters(text:str):
 
         """
 
@@ -132,14 +138,15 @@
         }
 
         return params
 
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
+    @_sync_logging_decorator
     def _translate_text(text:str) -> typing.Union[typing.List[TextResult], TextResult]:
 
         """
 
         Translates the given text to the target language.
 
         Parameters:
@@ -163,14 +170,15 @@
             
         except Exception as _e:
             raise _e
         
 ##-------------------start-of-_async_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
+    @_async_logging_decorator
     async def _async_translate_text(text:str) -> typing.Union[typing.List[TextResult], TextResult]:
 
         """
 
         Translates the given text to the target language asynchronously.
 
         Parameters:
@@ -247,15 +255,15 @@
 ##-------------------start-of-_get_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _get_decorator() -> typing.Union[typing.Callable, None]:
 
         """
 
-        Returns the decorator to use for the Gemini service.
+        Returns the decorator to use for the DeepL service.
 
         Returns:
         decorator (callable) : The decorator to use.
 
         """
 
         return DeepLService._decorator_to_use
```

### Comparing `easytl-0.1.2/src/easytl/easytl.py` & `easytl-0.2.0b0/src/easytl/easytl.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 ## third-party libraries
 from .classes import Language, SplitSentences, Formality, GlossaryInfo
 
 ## custom modules
 from .deepl_service import DeepLService
 from .gemini_service import GeminiService
-from .openai_service import OpenAIService, ChatCompletion
+from .openai_service import OpenAIService
 
-from. classes import ModelTranslationMessage, SystemTranslationMessage
+from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion
 from .exceptions import DeepLException, GoogleAPIError,OpenAIError, EasyTLException
 
 from .util import _convert_to_correct_type, _validate_easytl_translation_settings, _is_iterable_of_strings
 
 class EasyTL:
 
     """
@@ -118,37 +118,43 @@
 ##-------------------start-of-deepl_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def deepl_translate(text:typing.Union[str, typing.Iterable[str]],
                         target_lang:str | Language = "EN-US",
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
+                        logging_directory:str | None = None,
+                        response_type:typing.Literal["text", "raw"] | None = "text",
                         source_lang:str | Language | None = None,
                         context:str | None = None,
                         split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                         preserve_formatting:bool | None = None,
                         formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                         glossary:str | GlossaryInfo | None = None,
                         tag_handling:typing.Literal["xml", "html"] | None = None,
                         outline_detection:bool | None = None,
                         non_splitting_tags:str | typing.List[str] | None = None,
                         splitting_tags:str | typing.List[str] | None = None,
-                        ignore_tags:str | typing.List[str] | None = None) -> typing.Union[typing.List[str], str]:
+                        ignore_tags:str | typing.List[str] | None = None) -> typing.Union[typing.List[str], str, typing.List[TextResult], TextResult]:
         
         """
 
         Translates the given text to the target language using DeepL.
 
         This function assumes that the API key has already been set.
 
+        DeepL has backoff retrying implemented by default.
+
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
         source_lang (string or Language or None) : The source language to translate from.
         context (string or None) : Additional information for the translator to be considered when translating. Not translated itself.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
         formality (literal or Formality or None) : The formality level to use.
         glossary (string or GlossaryInfo or None) : The glossary to use.
         tag_handling (literal or None) : How to handle tags.
@@ -158,73 +164,103 @@
         ignore_tags (string or list or None) : Tags that should be ignored.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
+        assert response_type in ["text", "raw"], ValueError("Invalid response type specified. Must be 'text' or 'raw'.")
+
         EasyTL.test_api_key_validity("deepl")
 
-        if(decorator != None):
-            DeepLService._set_decorator(decorator)
+        DeepLService._set_decorator(decorator)
 
         if(override_previous_settings == True):
-            DeepLService._set_attributes(target_lang, 
-                                        source_lang, 
-                                        context, 
-                                        split_sentences,
-                                        preserve_formatting,
-                                        None,
-                                        formality, 
-                                        glossary, tag_handling, outline_detection, non_splitting_tags, splitting_tags, ignore_tags)
+            DeepLService._set_attributes(target_lang = target_lang, 
+                                        source_lang = source_lang, 
+                                        context = context, 
+                                        split_sentences = split_sentences,
+                                        preserve_formatting = preserve_formatting, 
+                                        formality = formality, 
+                                        glossary = glossary, 
+                                        tag_handling = tag_handling, 
+                                        outline_detection = outline_detection, 
+                                        non_splitting_tags = non_splitting_tags, 
+                                        splitting_tags = splitting_tags, 
+                                        ignore_tags = ignore_tags,
+                                        semaphore=None,
+                                        logging_directory=logging_directory)
             
         if(isinstance(text, str)):
-            return DeepLService._translate_text(text).text # type: ignore
+            result = DeepLService._translate_text(text)
+        
+            assert not isinstance(result, list), "Unexpected error occurred. Please try again."
+
+            if(response_type == "text"):
+                return result.text
+            
+            else:
+                return result
         
         elif(_is_iterable_of_strings(text)):
-            return [DeepLService._translate_text(t).text for t in text] # type: ignore
+
+            results = [DeepLService._translate_text(t) for t in text]
+
+            assert isinstance(results, list), "Unexpected error occurred. Please try again."
+
+            if(all(isinstance(_r, TextResult) for _r in results)):
+                if(response_type == "text"):
+                    return [_r.text for _r in results] # type: ignore
+                
+                else:
+                    return results # type: ignore
         
-        else:
-            raise ValueError("text must be a string or an iterable of strings.")
+        raise ValueError("text must be a string or an iterable of strings.")
         
 ##-------------------start-of-deepl_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def deepl_translate_async(text:typing.Union[str, typing.Iterable[str]],
                             target_lang:str | Language = "EN-US",
                             override_previous_settings:bool = True,
                             decorator:typing.Callable | None = None,
+                            logging_directory:str | None = None,
                             semaphore:int | None = None,
+                            response_type:typing.Literal["text", "raw"] | None = "text",
                             source_lang:str | Language | None = None,
                             context:str | None = None,
                             split_sentences:typing.Literal["OFF", "ALL", "NO_NEWLINES"] |  SplitSentences | None = "ALL",
                             preserve_formatting:bool | None = None,
                             formality:typing.Literal["default", "more", "less", "prefer_more", "prefer_less"] | Formality | None = None,
                             glossary:str | GlossaryInfo | None = None,
                             tag_handling:typing.Literal["xml", "html"] | None = None,
                             outline_detection:bool | None = None,
                             non_splitting_tags:str | typing.List[str] | None = None,
                             splitting_tags:str | typing.List[str] | None = None,
-                            ignore_tags:str | typing.List[str] | None = None) -> typing.Union[typing.List[str], str]:
+                            ignore_tags:str | typing.List[str] | None = None) -> typing.Union[typing.List[str], str, typing.List[TextResult], TextResult]:
         
         """
 
         Asynchronous version of deepl_translate().
         
         Translates the given text to the target language using DeepL.
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the API key has already been set.
+
+        DeepL has backoff retrying implemented by default.
         
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         semaphore (int) : The number of concurrent requests to make. Default is 30.
+        response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
         source_lang (string or Language or None) : The source language to translate from.
         context (string or None) : Additional information for the translator to be considered when translating. Not translated itself.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
         formality (literal or Formality or None) : The formality level to use.
         glossary (string or GlossaryInfo or None) : The glossary to use.
         tag_handling (literal or None) : How to handle tags.
@@ -234,473 +270,524 @@
         ignore_tags (string or list or None) : Tags that should be ignored.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
+        assert response_type in ["text", "raw"], ValueError("Invalid response type specified. Must be 'text' or 'raw'.")
+
         EasyTL.test_api_key_validity("deepl")
 
-        if(decorator != None):
-            DeepLService._set_decorator(decorator)
+        DeepLService._set_decorator(decorator)
 
         if(override_previous_settings == True):
-            DeepLService._set_attributes(target_lang, 
-                                        source_lang, 
-                                        context, 
-                                        split_sentences,
-                                        preserve_formatting, 
-                                        semaphore,
-                                        formality, 
-                                        glossary, tag_handling, outline_detection, non_splitting_tags, splitting_tags, ignore_tags)
+            DeepLService._set_attributes(target_lang=target_lang, 
+                                        source_lang=source_lang, 
+                                        context=context, 
+                                        split_sentences=split_sentences,
+                                        preserve_formatting=preserve_formatting, 
+                                        formality=formality, 
+                                        glossary=glossary, 
+                                        tag_handling=tag_handling, 
+                                        outline_detection=outline_detection, 
+                                        non_splitting_tags=non_splitting_tags, 
+                                        splitting_tags=splitting_tags, 
+                                        ignore_tags=ignore_tags,
+                                        semaphore=semaphore,
+                                        logging_directory=logging_directory)
             
         if(isinstance(text, str)):
             _result = await DeepLService._async_translate_text(text)
 
             assert not isinstance(_result, list), "Unexpected error occurred. Please try again."
 
-            if(hasattr(_result, "text")):
-                return _result.text 
+            if(response_type == "text"):
+                return _result.text
             
             else:
-                raise EasyTLException("Result does not have a 'text' attribute due to an unexpected error.")
+                return _result
             
         elif(_is_iterable_of_strings(text)):
             _tasks = [DeepLService._async_translate_text(t) for t in text]
             _results = await asyncio.gather(*_tasks)
             
             assert isinstance(_results, list), "Unexpected error occurred. Please try again."
 
-            if(all(hasattr(_r, "text") for _r in _results)):
-                return [_r.text for _r in _results] # type: ignore
+            if(all(isinstance(_r, TextResult) for _r in _results)):
+                if(response_type == "text"):
+                    return [_r.text for _r in _results] # type: ignore
+                
+                else:
+                    return _results # type: ignore
             
-            else:
-                raise EasyTLException("Result does not have a 'text' attribute due to an unexpected error.")
-            
-        else:
-            raise ValueError("text must be a string or an iterable of strings.")
+        raise ValueError("text must be a string or an iterable of strings.")
             
 ##-------------------start-of-gemini_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def gemini_translate(text:typing.Union[str, typing.Iterable[str]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
+                        logging_directory:str | None = None,
+                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
                         translation_instructions:str | None = None,
                         model:str="gemini-pro",
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
                         stop_sequences:typing.List[str] | None=None,
-                        max_output_tokens:int | None=None) -> str | typing.List[str]:
+                        max_output_tokens:int | None=None) -> typing.Union[typing.List[str], str, GenerateContentResponse, typing.List[GenerateContentResponse]]:
         
         """
 
         Translates the given text using Gemini.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
+        It is not known whether Gemini has backoff retrying implemented. (Their API is a mess.)
+        
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
-        translation_instructions (string or None) : The translation instructions to use.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a GenerateContentResponse object, 'json' returns a json-parseable string.
+        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
         model (string) : The model to use. 
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : The sequences to stop at.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
-        EasyTL.test_api_key_validity("gemini")
+        assert response_type in ["text", "raw", "json"], ValueError("Invalid response type specified. Must be 'text', 'raw' or 'json'.")
 
         _settings = {
         "gemini_model": "",
         "gemini_temperature": "",
         "gemini_top_p": "",
         "gemini_top_k": "",
         "gemini_stop_sequences": "",
         "gemini_max_output_tokens": ""
         }
 
-        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions"]
+        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type"]
         _custom_validation_params = ["gemini_stop_sequences"]
 
         assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), "text must be a string or an iterable of strings."
 
         for _key in _settings.keys():
             param_name = _key.replace("gemini_", "")
             if(param_name in locals() and _key not in _non_gemini_params and _key not in _custom_validation_params):
                 _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
-        if(decorator != None):
-            GeminiService._set_decorator(decorator)
+        EasyTL.test_api_key_validity("gemini")
+
+        GeminiService._set_decorator(decorator)
+
+        GeminiService._set_json_mode(True if response_type == "json" else False)
 
         translation_instructions = translation_instructions or GeminiService._system_message
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
                                           candidate_count=1,
                                           stream=False,
                                           stop_sequences=stop_sequences,
-                                          max_output_tokens=max_output_tokens)
+                                          max_output_tokens=max_output_tokens,
+                                          semaphore=None,
+                                          logging_directory=logging_directory)
 
         if(isinstance(text, str)):
             _result = GeminiService._translate_text(text)
-
-            if(hasattr(_result, "text")):
+            
+            if(response_type == "text" or response_type == "json"):
                 return _result.text
             
             else:
-                raise EasyTLException("Result does not have a 'text' attribute due to an unexpected error.")
-        
+                return _result
+
         elif(_is_iterable_of_strings(text)):
             
             _results = [GeminiService._translate_text(t) for t in text]
 
-            if(all(hasattr(_r, "text") for _r in _results)):
+            if(response_type == "text" or response_type == "json"):
                 return [_r.text for _r in _results]
             
-        else:
-            raise ValueError("text must be a string or an iterable of strings.")
+            else:
+                return _results
+            
+        raise ValueError("text must be a string or an iterable of strings.")
         
-        raise EasyTLException("Unexpected state reached in gemini_translate.")
-
 ##-------------------start-of-gemini_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def gemini_translate_async(text:typing.Union[str, typing.Iterable[str]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
+                                    logging_directory:str | None = None,
                                     semaphore:int | None = None,
+                                    response_type:typing.Literal["text", "raw", "json"] | None = "text",
                                     translation_instructions:str | None = None,
                                     model:str="gemini-pro",
                                     temperature:float=0.5,
                                     top_p:float=0.9,
                                     top_k:int=40,
                                     stop_sequences:typing.List[str] | None=None,
-                                    max_output_tokens:int | None=None) -> str | typing.List[str]:
+                                    max_output_tokens:int | None=None) -> typing.Union[typing.List[str], str, AsyncGenerateContentResponse, typing.List[AsyncGenerateContentResponse]]:
         
         """
 
         Asynchronous version of gemini_translate().
         Will generally be faster for iterables. Order is preserved.
 
         Translates the given text using Gemini.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
+        It is not known whether Gemini has backoff retrying implemented. (Their API is a mess.)
+        
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a Gemini translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         semaphore (int) : The number of concurrent requests to make. Default is 15 for 1.0 and 2 for 1.5 gemini models.
-        translation_instructions (string or None) : The translation instructions to use.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a AsyncGenerateContentResponse object, 'json' returns a json-parseable string.
+        translation_instructions (string or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         top_k (int) : The top k tokens to consider. Generally, alter this or temperature or top_p, not all three.
         stop_sequences (list or None) : The sequences to stop at.
         max_output_tokens (int or None) : The maximum number of tokens to output.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
-        EasyTL.test_api_key_validity("gemini")
-
         _settings = {
         "gemini_model": "",
         "gemini_temperature": "",
         "gemini_top_p": "",
         "gemini_top_k": "",
         "gemini_stop_sequences": "",
         "gemini_max_output_tokens": ""
         }
 
-        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions"]
+        _non_gemini_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "semaphore", "response_type"]
         _custom_validation_params = ["gemini_stop_sequences"]
 
         assert stop_sequences is None or isinstance(stop_sequences, str) or (hasattr(stop_sequences, '__iter__') and all(isinstance(i, str) for i in stop_sequences)), "stop_sequences must be a string or an iterable of strings."
 
         for _key in _settings.keys():
             param_name = _key.replace("gemini_", "")
             if(param_name in locals() and _key not in _non_gemini_params and _key not in _custom_validation_params):
                 _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
 
         _validate_easytl_translation_settings(_settings, "gemini")
 
-        if(decorator != None):
-            GeminiService._set_decorator(decorator)
+        EasyTL.test_api_key_validity("gemini")
+
+        GeminiService._set_decorator(decorator)
+
+        GeminiService._set_json_mode(True if response_type == "json" else False)
 
         translation_instructions = translation_instructions or GeminiService._system_message
 
         if(override_previous_settings == True):
             GeminiService._set_attributes(model=model,
                                           system_message=translation_instructions,
                                           temperature=temperature,
                                           top_p=top_p,
                                           top_k=top_k,
                                           candidate_count=1,
                                           stream=False,
                                           stop_sequences=stop_sequences,
                                           max_output_tokens=max_output_tokens,
-                                          semaphore=semaphore)
+                                          semaphore=semaphore,
+                                          logging_directory=logging_directory)
             
         if(isinstance(text, str)):
             _result = await GeminiService._translate_text_async(text)
 
-            if(hasattr(_result, "text")):
-                return _result.text 
+            if(response_type == "text" or response_type == "json"):
+                return _result.text
             
             else:
-                raise Exception("Unexpected error occurred. Please try again.")
+                return _result
             
         elif(_is_iterable_of_strings(text)):
             _tasks = [GeminiService._translate_text_async(_t) for _t in text]
 
             _results = await asyncio.gather(*_tasks)
 
-            if(all(hasattr(_r, "text") for _r in _results)):
-                return [_r.text for _r in _results]  
+            if(response_type == "text" or response_type == "json"):
+                return [_r.text for _r in _results]
             
-        else:
-            raise ValueError("text must be a string or an iterable of strings.")
+            else:
+                return _results 
+
+        raise ValueError("text must be a string or an iterable of strings.")
             
-        raise Exception("Unexpected state reached in gemini_translate_async.")
-    
 ##-------------------start-of-openai_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def openai_translate(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
+                        logging_directory:str | None = None,
+                        response_type:typing.Literal["text", "raw", "json"] | None = "text",
                         translation_instructions:str | SystemTranslationMessage | None = None,
                         model:str="gpt-4",
                         temperature:float=0.3,
                         top_p:float=1.0,
                         stop:typing.List[str] | None=None,
                         max_tokens:int | None=None,
                         presence_penalty:float=0.0,
                         frequency_penalty:float=0.0
-                        ) -> str | typing.List[str]:
+                        ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Translates the given text to the target language using OpenAI.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
+        OpenAI has it's backoff retrying disabled by EasyTL.
+
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
-        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         stop (list or None) : The sequences to stop at.
         max_tokens (int or None) : The maximum number of tokens to output.
         presence_penalty (float) : The presence penalty to use.
         frequency_penalty (float) : The frequency penalty to use.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
-        EasyTL.test_api_key_validity("openai")
-
         _settings = {
         "openai_model": "",
         "openai_temperature": "",
         "openai_top_p": "",
         "openai_stop": "",
         "openai_max_tokens": "",
         "openai_presence_penalty": "",
         "openai_frequency_penalty": ""
         }
 
-        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions"]
+        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "response_type"]
         _custom_validation_params = ["openai_stop"]
     
         assert stop is None or isinstance(stop, str) or (hasattr(stop, '__iter__') and all(isinstance(i, str) for i in stop)), "stop must be a string or an iterable of strings."
 
         for _key in _settings.keys():
             param_name = _key.replace("openai_", "")
             if(param_name in locals() and _key not in _non_openai_params and _key not in _custom_validation_params):
                 _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
 
+        EasyTL.test_api_key_validity("openai")
+
         _validate_easytl_translation_settings(_settings, "openai")
 
-        if(decorator != None):
-            OpenAIService._set_decorator(decorator)
+        OpenAIService._set_decorator(decorator)
+
+        OpenAIService._set_json_mode(True if response_type == "json" else False)
 
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
                                         top_p=top_p,
                                         n=1,
                                         stop=stop,
                                         max_tokens=max_tokens,
                                         presence_penalty=presence_penalty,
-                                        frequency_penalty=frequency_penalty)
+                                        frequency_penalty=frequency_penalty,
+                                        semaphore=None,
+                                        logging_directory=logging_directory)
             
         translation_batches = OpenAIService._build_translation_batches(text, translation_instructions)
         
         translations = []
 
         for _text, _translation_instructions in translation_batches:
 
             _result = OpenAIService._translate_text(_translation_instructions, _text)
 
-            translation = _result.choices[0].message.content
+            if(response_type == "text" or response_type == "json"):
+                translation = _result.choices[0].message.content
 
-            if(translation is None):
-                raise EasyTLException("Unexpected error occurred. Please try again.")
+            else:
+                translation = _result
             
             translations.append(translation)
         
         ## If originally a single text was provided, return a single translation instead of a list
         return translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else translations[0]
         
 ##-------------------start-of-openai_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def openai_translate_async(text:typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                     override_previous_settings:bool = True,
                                     decorator:typing.Callable | None = None,
                                     semaphore:int | None = None,
+                                    logging_directory:str | None = None,
+                                    response_type:typing.Literal["text", "raw", "json"] | None = "text",
                                     translation_instructions:str | SystemTranslationMessage | None = None,
                                     model:str="gpt-4",
                                     temperature:float=0.3,
                                     top_p:float=1.0,
                                     stop:typing.List[str] | None=None,
                                     max_tokens:int | None=None,
                                     presence_penalty:float=0.0,
                                     frequency_penalty:float=0.0
-                                    ) -> str | typing.List[str]:
+                                    ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Asynchronous version of openai_translate().
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
+        OpenAI has it's backoff retrying disabled by EasyTL.
+
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
         semaphore (int) : The number of concurrent requests to make. Default is 5.
-        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use.
+        logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
+        response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
+        translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output in the instructions. The default system message will ask for json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         stop (list or None) : The sequences to stop at.
         max_tokens (int or None) : The maximum number of tokens to output.
         presence_penalty (float) : The presence penalty to use.
         frequency_penalty (float) : The frequency penalty to use.
 
         Returns:
         translation (list - string or string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
-        EasyTL.test_api_key_validity("openai")
-
         _settings = {
         "openai_model": "",
         "openai_temperature": "",
         "openai_top_p": "",
         "openai_stop": "",
         "openai_max_tokens": "",
         "openai_presence_penalty": "",
         "openai_frequency_penalty": ""
         }
 
-        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions"]
+        _non_openai_params = ["text", "override_previous_settings", "decorator", "translation_instructions", "logging_directory", "semaphore", "response_type"]
         _custom_validation_params = ["openai_stop"]
 
         assert stop is None or isinstance(stop, str) or (hasattr(stop, '__iter__') and all(isinstance(i, str) for i in stop)), "stop must be a string or an iterable of strings."
 
         for _key in _settings.keys():
             param_name = _key.replace("openai_", "")
             if(param_name in locals() and _key not in _non_openai_params and _key not in _custom_validation_params):
                 _settings[_key] = _convert_to_correct_type(_key, locals()[param_name])
 
         _validate_easytl_translation_settings(_settings, "openai")
 
-        if(decorator != None):
-            OpenAIService._set_decorator(decorator)
+        EasyTL.test_api_key_validity("openai")
+
+        OpenAIService._set_decorator(decorator)
+
+        OpenAIService._set_json_mode(True if response_type == "json" else False)
 
         if(override_previous_settings == True):
             OpenAIService._set_attributes(model=model,
                                         temperature=temperature,
                                         logit_bias=None,
-                                        semaphore=semaphore,
                                         top_p=top_p,
                                         n=1,
                                         stop=stop,
                                         max_tokens=max_tokens,
                                         presence_penalty=presence_penalty,
-                                        frequency_penalty=frequency_penalty)
+                                        frequency_penalty=frequency_penalty,
+                                        semaphore=semaphore,
+                                        logging_directory=logging_directory)
 
         _translation_batches = OpenAIService._build_translation_batches(text, translation_instructions)
 
         _translation_tasks = []
 
         for _text, _translation_instructions in _translation_batches:
             _task = OpenAIService._translate_text_async(_translation_instructions, _text)
             _translation_tasks.append(_task)
 
         _results = await asyncio.gather(*_translation_tasks)
 
         _results:typing.List[ChatCompletion] = _results
+        
+        if(response_type == "text" or response_type == "json"):
+            _translations = [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
 
-        _translations = [result.choices[0].message.content for result in _results if result.choices[0].message.content is not None]
+        elif(response_type == "raw"):
+            _translations = _results
 
         # If the original input was a single text (not an iterable of texts), return a single translation instead of a list
         return _translations if isinstance(text, typing.Iterable) and not isinstance(text, str) else _translations[0]
-            
+    
 ##-------------------start-of-translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def translate(text:str | typing.Iterable[str],
                   service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl", 
-                  **kwargs) -> typing.Union[typing.List[str], str]:
+                  **kwargs) -> typing.Union[typing.List[str], str, 
+                                            typing.List[TextResult], TextResult, 
+                                            typing.List[GenerateContentResponse], GenerateContentResponse, 
+                                            typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Translates the given text to the target language using the specified service.
 
         Please see the documentation for the specific translation function for the service you want to use.
 
@@ -731,15 +818,19 @@
             raise ValueError("Invalid service specified.")
         
 ##-------------------start-of-translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     async def translate_async(text:str | typing.Iterable[str],
                               service:typing.Optional[typing.Literal["deepl", "openai", "gemini"]] = "deepl", 
-                              **kwargs) -> typing.Union[typing.List[str], str]:
+                              **kwargs) -> typing.Union[typing.List[str], str, 
+                                                        typing.List[TextResult], TextResult, 
+                                                        typing.List[GenerateContentResponse], GenerateContentResponse, 
+                                                        typing.List[ChatCompletion], ChatCompletion,
+                                                        AsyncGenerateContentResponse, typing.List[AsyncGenerateContentResponse]]:
         
         """
 
         Asynchronous version of translate().
         
         Translates the given text to the target language using the specified service.
         This function assumes that the API key has already been set.
```

### Comparing `easytl-0.1.2/src/easytl/exceptions.py` & `easytl-0.2.0b0/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.2/src/easytl/gemini_service.py` & `easytl-0.2.0b0/src/easytl/gemini_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 ## Use of this source code is governed by a GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
-## third party libraries
-from google.generativeai import GenerationConfig
-from google.generativeai.types import GenerateContentResponse, AsyncGenerateContentResponse
-
 import google.generativeai as genai
 
 ## custom modules
 from .util import _estimate_cost, _convert_iterable_to_str, _is_iterable_of_strings
+from .decorators import _async_logging_decorator, _sync_logging_decorator
+
+from .classes import GenerationConfig, GenerateContentResponse, AsyncGenerateContentResponse
 
 class GeminiService:
 
     _default_translation_instructions:str = "Please translate the following text into English."
     _default_model:str = "gemini-pro"
 
     _system_message = _default_translation_instructions
@@ -31,20 +30,21 @@
     _stop_sequences:typing.List[str] | None = None
     _max_output_tokens:int | None = None
 
     _client:genai.GenerativeModel
     _generation_config:GenerationConfig
 
     _semaphore_value:int = 15
-
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
-    ## I don't plan to allow users to change these settings, as I believe that translations should be as accurate as possible, avoiding any censorship or filtering of content.
+    _log_directory:str | None = None
+
+    ## I don't plan to easily allowing users to change these settings, as I believe that translations should be as accurate as possible, avoiding any censorship or filtering of content.
     _safety_settings = [
         {
             "category": "HARM_CATEGORY_DANGEROUS",
             "threshold": "BLOCK_NONE",
         },
         {
             "category": "HARM_CATEGORY_HARASSMENT",
@@ -60,14 +60,16 @@
         },
         {
             "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
             "threshold": "BLOCK_NONE",
         },
     ]
 
+    _json_mode:bool = False
+
 ##-------------------start-of-_set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
 
@@ -79,40 +81,57 @@
         """
 
         genai.configure(api_key=api_key)
 
 ##-------------------start-of-_set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def _set_decorator(decorator:typing.Callable) -> None:
+    def _set_decorator(decorator:typing.Callable | None) -> None:
 
         """
 
-        Sets the decorator to use for the Gemini service. Should be a callable that returns a decorator.
+        Sets the decorator to use for the Gemini service. Should be a callable that returns a decorator or None.
 
         Parameters:
-        decorator (callable) : The decorator to use.
+        decorator (callable | None) : The decorator to use.
 
         """
 
         GeminiService._decorator_to_use = decorator
 
+##-------------------start-of-_set_json_mode()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def _set_json_mode(json_mode:bool) -> None:
+
+        """
+
+        Sets the JSON mode for the Gemini service.
+
+        Parameters:
+        json_mode (bool) : True if the service should return JSON responses, False if it should return text responses.
+
+        """
+
+        GeminiService._json_mode = json_mode
+
 ##-------------------start-of-_set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str="gemini-pro",
                         system_message:str = _default_translation_instructions,
                         temperature:float=0.5,
                         top_p:float=0.9,
                         top_k:int=40,
                         candidate_count:int=1,
                         stream:bool=False,
                         stop_sequences:typing.List[str] | None=None,
                         max_output_tokens:int | None=None,
-                        semaphore:int | None=None
+                        semaphore:int | None=None,
+                        logging_directory:str | None=None
                         ) -> None:
         
         """
 
         Sets the attributes for the Gemini service.
 
         """
@@ -128,46 +147,63 @@
         GeminiService._max_output_tokens = max_output_tokens
 
         ## if a semaphore is not provided, set it to the default value based on the model
         if(semaphore is not None):
             GeminiService._semaphore_value = semaphore
 
         else:
-            GeminiService._semaphore_value = 15 if GeminiService._model != "gemini--1.5-pro-latest" else 2
+            GeminiService._semaphore_value = 15 if GeminiService._model != "gemini-1.5-pro-latest" else 2
+
+        GeminiService._log_directory = logging_directory
+
+        if(GeminiService._json_mode and GeminiService._model != "gemini-1.5-pro-latest"):
+            GeminiService._default_translation_instructions = "Please translate the following text into English. Make sure to return the translated text in JSON format."
+
+        else:
+            GeminiService._default_translation_instructions = "Please translate the following text into English."
         
 ##-------------------start-of-_redefine_client()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _redefine_client() -> None:
 
         """
 
         Redefines the Gemini client and generation config. This should be called before making any requests to the Gemini service, or after changing any of the service's settings.
 
         """
 
-        ## as of now, the only model that allows for system instructions is gemini--1.5-pro-latest
-        if(GeminiService._model == "gemini--1.5-pro-latest"):
+        response_mime_type = "text/plain"
+
+        if(GeminiService._json_mode):
+            response_mime_type = "application/json"
 
-            GeminiService._client = genai.GenerativeModel(model_name=GeminiService._model,
-                                                        safety_settings=GeminiService._safety_settings,
-                                                        system_instruction=GeminiService._system_message,
-                                                        )
+        gen_model_params = {
+            "model_name": GeminiService._model,
+            "safety_settings": GeminiService._safety_settings
+        }
+
+        ## gemini 1.5 is the only model that supports json responses and system instructions
+        if(GeminiService._model == "gemini-1.5-pro-latest"):
+            gen_model_params["system_instruction"] = GeminiService._system_message
         else:
-            GeminiService._client = genai.GenerativeModel(model_name=GeminiService._model,
-                                                        safety_settings=GeminiService._safety_settings)
+            response_mime_type = "text/plain"
 
+        GeminiService._client = genai.GenerativeModel(**gen_model_params)
+
+        GeminiService._generation_config = GenerationConfig(
+            candidate_count=GeminiService._candidate_count,
+            stop_sequences=GeminiService._stop_sequences,
+            max_output_tokens=GeminiService._max_output_tokens,
+            temperature=GeminiService._temperature,
+            top_p=GeminiService._top_p,
+            top_k=GeminiService._top_k,
+            response_mime_type=response_mime_type
+        )
 
-        GeminiService._generation_config = GenerationConfig(candidate_count=GeminiService._candidate_count,
-                                                           stop_sequences=GeminiService._stop_sequences,
-                                                           max_output_tokens=GeminiService._max_output_tokens,
-                                                            temperature=GeminiService._temperature,
-                                                            top_p=GeminiService._top_p,
-                                                            top_k=GeminiService._top_k)
-        
         GeminiService._semaphore = asyncio.Semaphore(GeminiService._semaphore_value)
 
 ##-------------------start-of-_redefine_client_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _redefine_client_decorator(func):
 
@@ -189,14 +225,15 @@
         
         return wrapper
             
 ##-------------------start-of-_translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     @_redefine_client_decorator
+    @_async_logging_decorator
     async def _translate_text_async(text_to_translate:str) -> AsyncGenerateContentResponse:
 
         """
 
         Asynchronously translates a text.
         Instructions default to translating whatever text is input into English.
 
@@ -214,14 +251,15 @@
         _decorated_function = GeminiService._decorator_to_use(GeminiService.__translate_text_async)
         return await _decorated_function(text_to_translate)
     
 ##-------------------start-of-_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     @_redefine_client_decorator
+    @_sync_logging_decorator
     def _translate_text(text_to_translate:str) -> GenerateContentResponse:
 
         """
 
         Synchronously translates a text.
         Instructions default to translating whatever text is input into English.
```

### Comparing `easytl-0.1.2/src/easytl/openai_service.py` & `easytl-0.2.0b0/src/easytl/openai_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 ## built-in libraries
 import typing
 import asyncio
 
 ## third-party libraries
 from openai import AsyncOpenAI, OpenAI
-from openai.types.chat.chat_completion import ChatCompletion
 
 ## custom modules
-from .classes import SystemTranslationMessage, ModelTranslationMessage
-from .util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings
+from .classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion
+from .util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings, VALID_JSON_OPENAI_MODELS
+from .decorators import _async_logging_decorator, _sync_logging_decorator
 
 class OpenAIService:
 
     _default_model:str = "gpt-4"
     _default_translation_instructions:SystemTranslationMessage = SystemTranslationMessage("Please translate the following text into English.")
 
     _system_message:typing.Optional[typing.Union[SystemTranslationMessage, str]] = _default_translation_instructions
@@ -29,22 +29,25 @@
     _stream:bool = False
     _stop:typing.List[str] | None = None
     _max_tokens:int | None = None
     _presence_penalty:float = 0.0
     _frequency_penalty:float = 0.0
 
     _semaphore_value:int = 5
-
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _sync_client = OpenAI(max_retries=0, api_key="DummyKey")
     _async_client = AsyncOpenAI(max_retries=0, api_key="DummyKey")
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
+    _json_mode:bool = False
+
+    _log_directory:str | None = None
+
 ##-------------------start-of-set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
 
         """
 
@@ -57,41 +60,59 @@
 
         OpenAIService._async_client.api_key = api_key
         OpenAIService._sync_client.api_key = api_key
 
 ##-------------------start-of-set_decorator()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def _set_decorator(decorator:typing.Callable) -> None:
+    def _set_decorator(decorator:typing.Callable | None) -> None:
 
         """
 
-        Sets the decorator to use for the OpenAI service. Should be a callable that returns a decorator.
+        Sets the decorator to use for the OpenAI service. Should be a callable that returns a decorator or None.
 
         Parameters:
-        decorator (callable) : The decorator to use.
+        decorator (callable | None) : The decorator to use.
 
         """
 
         OpenAIService._decorator_to_use = decorator
 
+##-------------------start-of-set_json_mode()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    @staticmethod
+    def _set_json_mode(json_mode:bool) -> None:
+            
+        """
+
+        Sets the JSON mode for the OpenAI service.
+
+        Parameters:
+        json_mode (bool) : True if the JSON mode is to be used, False otherwise.
+
+        """
+
+        OpenAIService._json_mode = json_mode
+
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str = _default_model,
                         temperature:float = 0.3,
                         logit_bias:typing.Dict[str, int] | None = None,
-                        semaphore:int | None = None,
                         top_p:float = 1.0,
                         n:int = 1,
                         stream:bool = False,
                         stop:typing.List[str] | None = None,
                         max_tokens:int | None = None,
                         presence_penalty:float = 0.0,
-                        frequency_penalty:float = 0.0) -> None:
+                        frequency_penalty:float = 0.0,
+                        semaphore:int | None = None,
+                        logging_directory:str | None = None
+                        ) -> None:
     
             """
     
             Sets the attributes for the OpenAI service.
     
             """
     
@@ -106,14 +127,22 @@
             OpenAIService._presence_penalty = presence_penalty
             OpenAIService._frequency_penalty = frequency_penalty
 
             if(semaphore is not None):
                 OpenAIService._semaphore_value = semaphore
                 OpenAIService._semaphore = asyncio.Semaphore(OpenAIService._semaphore_value)
 
+            OpenAIService._log_directory = logging_directory
+
+            if(OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS):
+                OpenAIService._default_translation_instructions = SystemTranslationMessage("Please translate the following text into English. Make sure to return the translated text in JSON format.")
+
+            else:
+                OpenAIService._default_translation_instructions = SystemTranslationMessage("Please translate the following text into English.")
+
 ##-------------------start-of-_build_translation_batches()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _build_translation_batches(text: typing.Union[str, typing.Iterable[str], ModelTranslationMessage, typing.Iterable[ModelTranslationMessage]],
                                 instructions: typing.Optional[typing.Union[str, SystemTranslationMessage]] = None) -> typing.List[typing.Tuple[ModelTranslationMessage, SystemTranslationMessage]]:
         
         """
@@ -151,14 +180,15 @@
             raise ValueError("Invalid type in iterable. Must be either strings or ModelTranslationMessage objects.")
         
         return [(item, instructions) for item in text]
 
 ##-------------------start-of-_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
+    @_sync_logging_decorator
     def _translate_text(translation_instructions: typing.Optional[SystemTranslationMessage],
                                 translation_prompt: ModelTranslationMessage
                                 ) -> ChatCompletion:
         
         """
         
         Synchronously translates the text using the OpenAI API.
@@ -180,14 +210,15 @@
 
         decorated_function = OpenAIService._decorator_to_use(OpenAIService.__translate_text)
         return decorated_function(translation_instructions, translation_prompt)
     
 ##-------------------start-of-_translate_text()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
+    @_async_logging_decorator
     async def _translate_text_async(translation_instructions: typing.Optional[SystemTranslationMessage],
                                 translation_prompt: ModelTranslationMessage
                                 ) -> ChatCompletion:
         
         """
 
         Asynchronously translates the text using the OpenAI API.
@@ -224,16 +255,19 @@
         prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
         response (ChatCompletion) : The response from the API.
 
         """
 
+        response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
+
         response = OpenAIService._sync_client.chat.completions.create(
-            messages=[
+            response_format={ "type": response_format },
+            messages=[ 
                 instructions.to_dict(),
                 prompt.to_dict()
             ], # type: ignore
 
             model=OpenAIService._model,
             temperature=OpenAIService._temperature,
             logit_bias=OpenAIService._logit_bias,
@@ -263,17 +297,20 @@
         prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
         response (ChatCompletion) : The response from the API.
 
         """
 
+        response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
+
         async with OpenAIService._semaphore:
 
             response = await OpenAIService._async_client.chat.completions.create(
+                response_format={ "type": response_format },
                 messages=[
                     instruction.to_dict(),
                     prompt.to_dict()
                 ],  # type: ignore
 
                 model=OpenAIService._model,
                 temperature=OpenAIService._temperature,
```

### Comparing `easytl-0.1.2/src/easytl/util.py` & `easytl-0.2.0b0/src/easytl/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ## Copyright Bikatr7 (https://github.com/Bikatr7)
 ## Use of this source code is governed by a GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
+
+## third-party libraries
 import tiktoken
 
 ## custom modules
 import google.generativeai as genai
-
-## custom modules
 from .exceptions import InvalidEasyTLSettings
 
 ##-------------------start-of-_string_to_bool()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _string_to_bool(string:str) -> bool:
 
     return string.lower() in ['true', '1', 'yes', 'y', 't']
@@ -394,15 +394,15 @@
 
         return _num_tokens, _min_cost, model
     
     ## _type checker doesn't like the chance of None being returned, so we raise an exception here if it gets to this point, which it shouldn't
     raise Exception("An unknown error occurred while calculating the minimum cost of translation.")
 
 ##-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
 ## https://platform.openai.com/docs/models/overview
 ALLOWED_OPENAI_MODELS  = [
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-0301",
     "gpt-3.5-turbo-0125",
     "gpt-3.5-turbo-0613",
     "gpt-3.5-turbo-1106",
@@ -419,15 +419,22 @@
     "gpt-4-turbo-2024-04-09",
     "gpt-4-0125-preview",
     "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4-1106-vision-preview",
 ]
 
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
+VALID_JSON_OPENAI_MODELS = [
+    "gpt-3.5-turbo-0125",
+    "gpt-4-turbo",
+    "gpt-4-turbo-preview",
+    "gpt-4-turbo-2024-04-09",
+]
+
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
 ## https://ai.google.dev/models/gemini
 ALLOWED_GEMINI_MODELS = [
     "gemini-1.0-pro-001",
     "gemini-1.0-pro",
     "gemini-1.0-pro-latest",
     "gemini-1.0-pro-vision-001",
     "gemini-1.0-pro-vision",
@@ -435,15 +442,15 @@
     "gemini-1.5-pro-latest",
   ##  "gemini-1.0-ultra-latest",
     "gemini-pro",
     "gemini-pro-vision",
   ##  "gemini-ultra"
 ]
 
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-09
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
 MODEL_COSTS = {
     # Grouping GPT-3.5 models together
     "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-0301": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-1106": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
     "gpt-3.5-turbo-16k-0613": {"price_case": 3, "_input_cost": 0.0030, "_output_cost": 0.0040},
```

### Comparing `easytl-0.1.2/src/easytl.egg-info/PKG-INFO` & `easytl-0.2.0b0/src/easytl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.1.2
+Version: 0.2.0b0
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.0
+Requires-Dist: google-generativeai==0.5.1
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
 Requires-Dist: tiktoken==0.6.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
@@ -33,14 +33,17 @@
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 ## EasyTL
 
 Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 
+EasyTL has a trello board:
+https://trello.com/b/Td555CoW/easytl
+
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
@@ -94,15 +97,15 @@
 
 wheel
 
 setuptools_scm>=6.0
 
 tomli
 
-google-generativeai==0.5.0
+google-generativeai==0.5.1
 
 deepl==1.16.1
 
 openai==1.13.3
 
 backoff==2.2.1
```

