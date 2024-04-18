# Comparing `tmp/llm-mistral-0.3.tar.gz` & `tmp/llm_mistral-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-mistral-0.3.tar", last modified: Mon Feb 26 16:06:36 2024, max compression
+gzip compressed data, was "llm_mistral-0.3.1.tar", last modified: Thu Apr 18 03:07:26 2024, max compression
```

## Comparing `llm-mistral-0.3.tar` & `llm_mistral-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:06:36.838027 llm-mistral-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-26 16:06:23.000000 llm-mistral-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-26 16:06:36.838027 llm-mistral-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-02-26 16:06:23.000000 llm-mistral-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:06:36.838027 llm-mistral-0.3/llm_mistral.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 16:06:36.000000 llm-mistral-0.3/llm_mistral.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-02-26 16:06:23.000000 llm-mistral-0.3/llm_mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-26 16:06:23.000000 llm-mistral-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 16:06:36.838027 llm-mistral-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:06:36.838027 llm-mistral-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-02-26 16:06:23.000000 llm-mistral-0.3/tests/test_mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:07:26.328220 llm_mistral-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 03:07:15.000000 llm_mistral-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-18 03:07:26.328220 llm_mistral-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-18 03:07:15.000000 llm_mistral-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:07:26.324220 llm_mistral-0.3.1/llm_mistral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 03:07:26.000000 llm_mistral-0.3.1/llm_mistral.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-18 03:07:15.000000 llm_mistral-0.3.1/llm_mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-18 03:07:15.000000 llm_mistral-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:07:26.328220 llm_mistral-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:07:26.324220 llm_mistral-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-18 03:07:15.000000 llm_mistral-0.3.1/tests/test_mistral.py
```

### Comparing `llm-mistral-0.3/LICENSE` & `llm_mistral-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-mistral-0.3/PKG-INFO` & `llm_mistral-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-mistral
-Version: 0.3
+Version: 0.3.1
 Summary: LLM plugin providing access to Mistral models busing the Mistral API
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-mistral
 Project-URL: Changelog, https://github.com/simonw/llm-mistral/releases
 Project-URL: Issues, https://github.com/simonw/llm-mistral/issues
 Project-URL: CI, https://github.com/simonw/llm-mistral/actions
```

### Comparing `llm-mistral-0.3/README.md` & `llm_mistral-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `llm-mistral-0.3/llm_mistral.egg-info/PKG-INFO` & `llm_mistral-0.3.1/llm_mistral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-mistral
-Version: 0.3
+Version: 0.3.1
 Summary: LLM plugin providing access to Mistral models busing the Mistral API
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-mistral
 Project-URL: Changelog, https://github.com/simonw/llm-mistral/releases
 Project-URL: Issues, https://github.com/simonw/llm-mistral/issues
 Project-URL: CI, https://github.com/simonw/llm-mistral/actions
```

### Comparing `llm-mistral-0.3/llm_mistral.py` & `llm_mistral-0.3.1/llm_mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
 
 
 def get_model_ids():
     user_dir = llm.user_dir()
     mistral_models = user_dir / "mistral_models.json"
     if mistral_models.exists():
         models = json.loads(mistral_models.read_text())
-    else:
+    elif llm.get_key("", "mistral", "LLM_MISTRAL_KEY"):
         models = refresh_models()
+    else:
+        models = {"data": []}
     return [model["id"] for model in models["data"] if "embed" not in model["id"]]
 
 
 @llm.hookimpl
 def register_commands(cli):
     @cli.group()
     def mistral():
@@ -143,15 +145,17 @@
             messages.append({"role": "assistant", "content": prev_response.text()})
         if prompt.system and prompt.system != current_system:
             messages.append({"role": "system", "content": prompt.system})
         messages.append({"role": "user", "content": prompt.prompt})
         return messages
 
     def execute(self, prompt, stream, response, conversation):
-        key = llm.get_key("", "mistral", "LLM_MISTRAL_KEY") or getattr(self, "key", None)
+        key = llm.get_key("", "mistral", "LLM_MISTRAL_KEY") or getattr(
+            self, "key", None
+        )
         messages = self.build_messages(prompt, conversation)
         response._prompt_json = {"messages": messages}
         body = {
             "model": self.mistral_model_id,
             "messages": messages,
         }
         if prompt.options.temperature:
```

### Comparing `llm-mistral-0.3/pyproject.toml` & `llm_mistral-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-mistral"
-version = "0.3"
+version = "0.3.1"
 description = "LLM plugin providing access to Mistral models busing the Mistral API"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `llm-mistral-0.3/tests/test_mistral.py` & `llm_mistral-0.3.1/tests/test_mistral.py`

 * *Files identical despite different names*

