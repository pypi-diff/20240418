# Comparing `tmp/instructor-1.2.0.tar.gz` & `tmp/instructor-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.0.tar", max compression
+gzip compressed data, was "instructor-1.2.1.tar", max compression
```

## Comparing `instructor-1.2.0.tar` & `instructor-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2024-04-14 14:59:27.585821 instructor-1.2.0/LICENSE
--rw-r--r--   0        0        0     9715 2024-04-14 14:59:27.585821 instructor-1.2.0/README.md
--rw-r--r--   0        0        0     1312 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/cli/usage.py
--rw-r--r--   0        0        0     9625 2024-04-14 14:59:27.649823 instructor-1.2.0/instructor/client.py
--rw-r--r--   0        0        0     2445 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2340 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/client_cohere.py
--rw-r--r--   0        0        0     1371 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/client_groq.py
--rw-r--r--   0        0        0     8968 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2580 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11052 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/exceptions.py
--rw-r--r--   0        0        0     7878 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/mode.py
--rw-r--r--   0        0        0     4845 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/patch.py
--rw-r--r--   0        0        0    13509 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/py.typed
--rw-r--r--   0        0        0     7595 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/retry.py
--rw-r--r--   0        0        0     4767 2024-04-14 14:59:27.653823 instructor-1.2.0/instructor/utils.py
--rw-r--r--   0        0        0     2252 2024-04-14 14:59:27.653823 instructor-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11542 1970-01-01 00:00:00.000000 instructor-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-18 00:19:56.934164 instructor-1.2.1/LICENSE
+-rw-r--r--   0        0        0     9715 2024-04-18 00:19:56.934164 instructor-1.2.1/README.md
+-rw-r--r--   0        0        0     1312 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6494 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9662 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client.py
+-rw-r--r--   0        0        0     2445 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2340 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1371 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/client_groq.py
+-rw-r--r--   0        0        0     8968 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2580 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11052 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/exceptions.py
+-rw-r--r--   0        0        0     7878 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/mode.py
+-rw-r--r--   0        0        0     4845 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/patch.py
+-rw-r--r--   0        0        0    13509 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/py.typed
+-rw-r--r--   0        0        0     7595 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/retry.py
+-rw-r--r--   0        0        0     4767 2024-04-18 00:19:56.998165 instructor-1.2.1/instructor/utils.py
+-rw-r--r--   0        0        0     2252 2024-04-18 00:19:57.002164 instructor-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11542 1970-01-01 00:00:00.000000 instructor-1.2.1/PKG-INFO
```

### Comparing `instructor-1.2.0/LICENSE` & `instructor-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/README.md` & `instructor-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/__init__.py` & `instructor-1.2.1/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/_types/_alias.py` & `instructor-1.2.1/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/cli/cli.py` & `instructor-1.2.1/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/cli/files.py` & `instructor-1.2.1/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/cli/hub.py` & `instructor-1.2.1/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/cli/jobs.py` & `instructor-1.2.1/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/cli/usage.py` & `instructor-1.2.1/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/client.py` & `instructor-1.2.1/instructor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,15 @@
     ), "Client must be an instance of openai.OpenAI or openai.AsyncOpenAI"
 
     if provider in {Provider.ANYSCALE, Provider.TOGETHER}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.JSON_SCHEMA,
+            instructor.Mode.MD_JSON,
         }
 
     if provider in {Provider.OPENAI}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.FUNCTIONS,
```

### Comparing `instructor-1.2.0/instructor/client_anthropic.py` & `instructor-1.2.1/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/client_cohere.py` & `instructor-1.2.1/instructor/client_cohere.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/client_groq.py` & `instructor-1.2.1/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/distil.py` & `instructor-1.2.1/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/citation.py` & `instructor-1.2.1/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/iterable.py` & `instructor-1.2.1/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/maybe.py` & `instructor-1.2.1/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/parallel.py` & `instructor-1.2.1/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/partial.py` & `instructor-1.2.1/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/simple_type.py` & `instructor-1.2.1/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/dsl/validators.py` & `instructor-1.2.1/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/function_calls.py` & `instructor-1.2.1/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/mode.py` & `instructor-1.2.1/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/patch.py` & `instructor-1.2.1/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/process_response.py` & `instructor-1.2.1/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/retry.py` & `instructor-1.2.1/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/instructor/utils.py` & `instructor-1.2.1/instructor/utils.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.0/pyproject.toml` & `instructor-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.0"
+version = "1.2.1"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.1.0"
 pydantic = "2.7.0"
-docstring-parser = "^0.15"
+docstring-parser = "^0.16"
 typer = ">=0.9.0,<1.0.0"
 rich = "^13.7.0"
 aiohttp = "^3.9.1"
 tenacity = "^8.2.3"
 pydantic-core = "^2.18.0"
 
 # dependency versions for extras
```

### Comparing `instructor-1.2.0/PKG-INFO` & `instructor-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.0
+Version: 1.2.1
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Provides-Extra: cohere
 Provides-Extra: groq
 Provides-Extra: test-docs
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "test-docs"
 Requires-Dist: cohere (>=5.1.8,<6.0.0) ; extra == "cohere" or extra == "test-docs"
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
-Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: docstring-parser (>=0.16,<0.17)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
 Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
```

