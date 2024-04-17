# Comparing `tmp/llm-anyscale-endpoints-0.4.tar.gz` & `tmp/llm_anyscale_endpoints-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-anyscale-endpoints-0.4.tar", last modified: Thu Dec 14 04:56:20 2023, max compression
+gzip compressed data, was "llm_anyscale_endpoints-0.5.tar", last modified: Wed Apr 17 22:58:01 2024, max compression
```

## Comparing `llm-anyscale-endpoints-0.4.tar` & `llm_anyscale_endpoints-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 04:56:20.874432 llm-anyscale-endpoints-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-14 04:56:07.000000 llm-anyscale-endpoints-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-14 04:56:20.874432 llm-anyscale-endpoints-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-12-14 04:56:07.000000 llm-anyscale-endpoints-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 04:56:20.874432 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-14 04:56:20.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-14 04:56:07.000000 llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-14 04:56:07.000000 llm-anyscale-endpoints-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 04:56:20.874432 llm-anyscale-endpoints-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 04:56:20.874432 llm-anyscale-endpoints-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-12-14 04:56:07.000000 llm-anyscale-endpoints-0.4/tests/test_llm_anyscale_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/tests/test_llm_anyscale_endpoints.py
```

### Comparing `llm-anyscale-endpoints-0.4/LICENSE` & `llm_anyscale_endpoints-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-anyscale-endpoints-0.4/PKG-INFO` & `llm_anyscale_endpoints-0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-anyscale-endpoints
-Version: 0.4
+Version: 0.5
 Summary:  LLM plugin for models hosted by Anyscale Endpoints
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-anyscale-endpoints
 Project-URL: Changelog, https://github.com/simonw/llm-anyscale-endpoints/releases
 Project-URL: Issues, https://github.com/simonw/llm-anyscale-endpoints/issues
 Project-URL: CI, https://github.com/simonw/llm-anyscale-endpoints/actions
@@ -52,33 +52,44 @@
 ```bash
 llm models list
 ```
 You should see a list that looks something like this:
 ```
 AnyscaleEndpoints: meta-llama/Llama-2-7b-chat-hf
 AnyscaleEndpoints: meta-llama/Llama-2-13b-chat-hf
-AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
-AnyscaleEndpoints: codellama/CodeLlama-34b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x7B-Instruct-v0.1
 AnyscaleEndpoints: mistralai/Mistral-7B-Instruct-v0.1
+AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
+AnyscaleEndpoints: codellama/CodeLlama-70b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x22B-Instruct-v0.1
+AnyscaleEndpoints: mlabonne/NeuralHermes-2.5-Mistral-7B
+AnyscaleEndpoints: google/gemma-7b-it
 ```
 To run a prompt against a model, pass its full model ID to the `-m` option, like this:
 ```bash
-llm -m meta-llama/Llama-2-70b-chat-hf \
+llm -m mistralai/Mixtral-8x22B-Instruct-v0.1 \
   'Five strident names for a pet walrus' \
   --system 'You love coming up with creative names for pets'
 ```
 You can set a shorter alias for a model using the `llm aliases` command like so:
 ```bash
-llm aliases set llama70b meta-llama/Llama-2-70b-chat-hf
+llm aliases set mix22b mistralai/Mixtral-8x22B-Instruct-v0.1
 ```
-Now you can prompt Llama 2 70B using:
+Now you can prompt Mixtral-8x22B-Instruct-v0.1 using the alias `mix22b`:
 ```bash
 cat llm_anyscale_endpoints.py | \
-  llm -m llama70b -s 'explain this code'
+  llm -m mix22b -s 'explain this code'
+```
+
+You can refresh the list of models by running:
+```bash
+llm anyscale-endpoints refresh
 ```
+This will fetch the latest list of models from Anyscale Endpoints and story it in a local cache file.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd llm-anyscale-endpoints
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `llm-anyscale-endpoints-0.4/README.md` & `llm_anyscale_endpoints-0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -34,33 +34,44 @@
 ```bash
 llm models list
 ```
 You should see a list that looks something like this:
 ```
 AnyscaleEndpoints: meta-llama/Llama-2-7b-chat-hf
 AnyscaleEndpoints: meta-llama/Llama-2-13b-chat-hf
-AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
-AnyscaleEndpoints: codellama/CodeLlama-34b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x7B-Instruct-v0.1
 AnyscaleEndpoints: mistralai/Mistral-7B-Instruct-v0.1
+AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
+AnyscaleEndpoints: codellama/CodeLlama-70b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x22B-Instruct-v0.1
+AnyscaleEndpoints: mlabonne/NeuralHermes-2.5-Mistral-7B
+AnyscaleEndpoints: google/gemma-7b-it
 ```
 To run a prompt against a model, pass its full model ID to the `-m` option, like this:
 ```bash
-llm -m meta-llama/Llama-2-70b-chat-hf \
+llm -m mistralai/Mixtral-8x22B-Instruct-v0.1 \
   'Five strident names for a pet walrus' \
   --system 'You love coming up with creative names for pets'
 ```
 You can set a shorter alias for a model using the `llm aliases` command like so:
 ```bash
-llm aliases set llama70b meta-llama/Llama-2-70b-chat-hf
+llm aliases set mix22b mistralai/Mixtral-8x22B-Instruct-v0.1
 ```
-Now you can prompt Llama 2 70B using:
+Now you can prompt Mixtral-8x22B-Instruct-v0.1 using the alias `mix22b`:
 ```bash
 cat llm_anyscale_endpoints.py | \
-  llm -m llama70b -s 'explain this code'
+  llm -m mix22b -s 'explain this code'
+```
+
+You can refresh the list of models by running:
+```bash
+llm anyscale-endpoints refresh
 ```
+This will fetch the latest list of models from Anyscale Endpoints and story it in a local cache file.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd llm-anyscale-endpoints
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `llm-anyscale-endpoints-0.4/llm_anyscale_endpoints.egg-info/PKG-INFO` & `llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-anyscale-endpoints
-Version: 0.4
+Version: 0.5
 Summary:  LLM plugin for models hosted by Anyscale Endpoints
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-anyscale-endpoints
 Project-URL: Changelog, https://github.com/simonw/llm-anyscale-endpoints/releases
 Project-URL: Issues, https://github.com/simonw/llm-anyscale-endpoints/issues
 Project-URL: CI, https://github.com/simonw/llm-anyscale-endpoints/actions
@@ -52,33 +52,44 @@
 ```bash
 llm models list
 ```
 You should see a list that looks something like this:
 ```
 AnyscaleEndpoints: meta-llama/Llama-2-7b-chat-hf
 AnyscaleEndpoints: meta-llama/Llama-2-13b-chat-hf
-AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
-AnyscaleEndpoints: codellama/CodeLlama-34b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x7B-Instruct-v0.1
 AnyscaleEndpoints: mistralai/Mistral-7B-Instruct-v0.1
+AnyscaleEndpoints: meta-llama/Llama-2-70b-chat-hf
+AnyscaleEndpoints: codellama/CodeLlama-70b-Instruct-hf
+AnyscaleEndpoints: mistralai/Mixtral-8x22B-Instruct-v0.1
+AnyscaleEndpoints: mlabonne/NeuralHermes-2.5-Mistral-7B
+AnyscaleEndpoints: google/gemma-7b-it
 ```
 To run a prompt against a model, pass its full model ID to the `-m` option, like this:
 ```bash
-llm -m meta-llama/Llama-2-70b-chat-hf \
+llm -m mistralai/Mixtral-8x22B-Instruct-v0.1 \
   'Five strident names for a pet walrus' \
   --system 'You love coming up with creative names for pets'
 ```
 You can set a shorter alias for a model using the `llm aliases` command like so:
 ```bash
-llm aliases set llama70b meta-llama/Llama-2-70b-chat-hf
+llm aliases set mix22b mistralai/Mixtral-8x22B-Instruct-v0.1
 ```
-Now you can prompt Llama 2 70B using:
+Now you can prompt Mixtral-8x22B-Instruct-v0.1 using the alias `mix22b`:
 ```bash
 cat llm_anyscale_endpoints.py | \
-  llm -m llama70b -s 'explain this code'
+  llm -m mix22b -s 'explain this code'
+```
+
+You can refresh the list of models by running:
+```bash
+llm anyscale-endpoints refresh
 ```
+This will fetch the latest list of models from Anyscale Endpoints and story it in a local cache file.
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd llm-anyscale-endpoints
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `llm-anyscale-endpoints-0.4/pyproject.toml` & `llm_anyscale_endpoints-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-anyscale-endpoints"
-version = "0.4"
+version = "0.5"
 description = " LLM plugin for models hosted by Anyscale Endpoints"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `llm-anyscale-endpoints-0.4/tests/test_llm_anyscale_endpoints.py` & `llm_anyscale_endpoints-0.5/tests/test_llm_anyscale_endpoints.py`

 * *Files identical despite different names*

