# Comparing `tmp/llm-replicate-0.2.tar.gz` & `tmp/llm_replicate-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-replicate-0.2.tar", last modified: Tue Jul 18 19:00:45 2023, max compression
+gzip compressed data, was "llm_replicate-0.3.1.tar", last modified: Thu Apr 18 17:14:11 2024, max compression
```

## Comparing `llm-replicate-0.2.tar` & `llm_replicate-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.523337 llm-replicate-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-18 19:00:45.523337 llm-replicate-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-18 19:00:24.000000 llm-replicate-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate/
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate/vendored_replicate/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-18 19:00:24.000000 llm-replicate-0.2/llm_replicate/vendored_replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.519337 llm-replicate-0.2/llm_replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 19:00:45.000000 llm-replicate-0.2/llm_replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-18 19:00:24.000000 llm-replicate-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:00:45.523337 llm-replicate-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:45.523337 llm-replicate-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-18 19:00:24.000000 llm-replicate-0.2/tests/test_replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:14:11.447767 llm_replicate-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 17:14:02.000000 llm_replicate-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-18 17:14:11.447767 llm_replicate-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-18 17:14:02.000000 llm_replicate-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:14:11.443767 llm_replicate-0.3.1/llm_replicate/
+-rw-r--r--   0 runner    (1001) docker     (127)    10219 2024-04-18 17:14:02.000000 llm_replicate-0.3.1/llm_replicate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:14:11.447767 llm_replicate-0.3.1/llm_replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 17:14:11.000000 llm_replicate-0.3.1/llm_replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 17:14:02.000000 llm_replicate-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:14:11.447767 llm_replicate-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:14:11.447767 llm_replicate-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-18 17:14:02.000000 llm_replicate-0.3.1/tests/test_replicate.py
```

### Comparing `llm-replicate-0.2/PKG-INFO` & `llm_replicate-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: llm-replicate
-Version: 0.2
-Summary: LLM plugin for models hosted on Replicate
-Author: Simon Willison
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/simonw/llm-replicate
-Project-URL: Changelog, https://github.com/simonw/llm-replicate/releases
-Project-URL: Issues, https://github.com/simonw/llm-replicate/issues
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # llm-replicate
 
 [![PyPI](https://img.shields.io/pypi/v/llm-replicate.svg)](https://pypi.org/project/llm-replicate/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm-replicate?include_prereleases&label=changelog)](https://github.com/simonw/llm-replicate/releases)
 [![Tests](https://github.com/simonw/llm-replicate/workflows/Test/badge.svg)](https://github.com/simonw/llm-replicate/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm-replicate/blob/main/LICENSE)
 
@@ -51,14 +37,20 @@
 
 ```bash
 llm replicate add a16z-infra/llama13b-v2-chat \
   --chat --alias llama2
 ```
 The `--chat` flag indicates that this is a chat model, which means it will be able to work with `-c` continue mode.
 
+Here's the [70b version](https://replicate.com/replicate/llama70b-v2-chat) of that model:
+```bash
+llm replicate add \
+  replicate/llama70b-v2-chat \
+  --chat --alias llama70b
+```
 ## Usage
 
 To run a prompt against a model, pass its name or an alias to `llm -m`:
 ```bash
 llm -m llama2 "Ten great names for a pet pelican"
 ```
 
@@ -163,22 +155,61 @@
 10. Splishy
 
 I hope these suggestions help you find the perfect name for your pet pelican! Do you have any other questions?
 User: Five more and make them more nautical
 Assistant:
 ```
 
-## Development
+## Fetching all Replicate predictions
 
-To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+Replicate logs all predictions made against models. You can fetch all of these predictions using the `llm replicate fetch-predictions` command:
 
-    cd llm-palm
-    python3 -m venv venv
-    source venv/bin/activate
+```bash
+llm replicate fetch-predictions
+```
+This will create or populate a table in your LLM `logs.db` database called `replicate_predictions`.
 
-Now install the dependencies and test dependencies:
+The data in this table will cover ALL Replicate models, not just language models that have been queried using this tool.
 
-    pip install -e '.[test]'
+Running `llm replicate fetch-predictions` multiple times will only fetch predictions that have been created since the last time the command was run.
 
-To run the tests:
+To browse the resulting data in [Datasette](https://datasette.io/), run this:
+```bash
+datasette "$(llm logs path)"
+```
+The schema for that table will look like this:
+```sql
+CREATE TABLE [replicate_predictions] (
+   [id] TEXT PRIMARY KEY,
+   [_model_guess] TEXT,
+   [completed_at] TEXT,
+   [created_at] TEXT,
+   [error] TEXT,
+   [input] TEXT,
+   [logs] TEXT,
+   [metrics] TEXT,
+   [output] TEXT,
+   [started_at] TEXT,
+   [status] TEXT,
+   [urls] TEXT,
+   [version] TEXT,
+   [webhook_completed] TEXT
+)
+```
+This schema may change if the Replicate API adds new fields in the future.
 
-    pytest
+## Development
+
+To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+```bash
+cd llm-replicate
+python3 -m venv venv
+source venv/bin/activate
+```
+Now install the dependencies and test dependencies:
+```bash
+pip install -e '.[test]'
+```
+To run the tests:
+```bash
+pytest
+```
```

### Comparing `llm-replicate-0.2/README.md` & `llm_replicate-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: llm-replicate
+Version: 0.3.1
+Summary: LLM plugin for models hosted on Replicate
+Author: Simon Willison
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/simonw/llm-replicate
+Project-URL: Changelog, https://github.com/simonw/llm-replicate/releases
+Project-URL: Issues, https://github.com/simonw/llm-replicate/issues
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llm
+Requires-Dist: requests-mock
+Requires-Dist: replicate>=0.9.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+
 # llm-replicate
 
 [![PyPI](https://img.shields.io/pypi/v/llm-replicate.svg)](https://pypi.org/project/llm-replicate/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm-replicate?include_prereleases&label=changelog)](https://github.com/simonw/llm-replicate/releases)
 [![Tests](https://github.com/simonw/llm-replicate/workflows/Test/badge.svg)](https://github.com/simonw/llm-replicate/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm-replicate/blob/main/LICENSE)
 
@@ -37,14 +56,20 @@
 
 ```bash
 llm replicate add a16z-infra/llama13b-v2-chat \
   --chat --alias llama2
 ```
 The `--chat` flag indicates that this is a chat model, which means it will be able to work with `-c` continue mode.
 
+Here's the [70b version](https://replicate.com/replicate/llama70b-v2-chat) of that model:
+```bash
+llm replicate add \
+  replicate/llama70b-v2-chat \
+  --chat --alias llama70b
+```
 ## Usage
 
 To run a prompt against a model, pass its name or an alias to `llm -m`:
 ```bash
 llm -m llama2 "Ten great names for a pet pelican"
 ```
 
@@ -149,22 +174,61 @@
 10. Splishy
 
 I hope these suggestions help you find the perfect name for your pet pelican! Do you have any other questions?
 User: Five more and make them more nautical
 Assistant:
 ```
 
-## Development
+## Fetching all Replicate predictions
 
-To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+Replicate logs all predictions made against models. You can fetch all of these predictions using the `llm replicate fetch-predictions` command:
 
-    cd llm-palm
-    python3 -m venv venv
-    source venv/bin/activate
+```bash
+llm replicate fetch-predictions
+```
+This will create or populate a table in your LLM `logs.db` database called `replicate_predictions`.
 
-Now install the dependencies and test dependencies:
+The data in this table will cover ALL Replicate models, not just language models that have been queried using this tool.
 
-    pip install -e '.[test]'
+Running `llm replicate fetch-predictions` multiple times will only fetch predictions that have been created since the last time the command was run.
 
-To run the tests:
+To browse the resulting data in [Datasette](https://datasette.io/), run this:
+```bash
+datasette "$(llm logs path)"
+```
+The schema for that table will look like this:
+```sql
+CREATE TABLE [replicate_predictions] (
+   [id] TEXT PRIMARY KEY,
+   [_model_guess] TEXT,
+   [completed_at] TEXT,
+   [created_at] TEXT,
+   [error] TEXT,
+   [input] TEXT,
+   [logs] TEXT,
+   [metrics] TEXT,
+   [output] TEXT,
+   [started_at] TEXT,
+   [status] TEXT,
+   [urls] TEXT,
+   [version] TEXT,
+   [webhook_completed] TEXT
+)
+```
+This schema may change if the Replicate API adds new fields in the future.
 
-    pytest
+## Development
+
+To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+```bash
+cd llm-replicate
+python3 -m venv venv
+source venv/bin/activate
+```
+Now install the dependencies and test dependencies:
+```bash
+pip install -e '.[test]'
+```
+To run the tests:
+```bash
+pytest
+```
```

### Comparing `llm-replicate-0.2/llm_replicate/__init__.py` & `llm_replicate-0.3.1/llm_replicate/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 import json
 import llm
+import replicate
 import requests
+import sqlite_utils
 
 
 @llm.hookimpl
 def register_commands(cli):
     @cli.group(name="replicate")
     def replicate():
         "Commands for working with models hosted on Replicate"
@@ -95,22 +97,109 @@
         Edit registered models using the default $EDITOR
         """
         models_path = config_dir() / "models.json"
         if not models_path.exists():
             models_path.write_text("[]")
         click.edit(filename=str(models_path))
 
+    @replicate.command(name="fetch-predictions")
+    @click.option("--key", "-k", help="Replicate API key")
+    def fetch_predictions(key):
+        """
+        Fetch data on all Replicate predictions, save to SQLite replicate_predictions
+
+        Example usage:
+
+            llm replicate fetch-predictions
+        """
+        token = llm.get_key(key, "replicate", env_var="REPLICATE_API_TOKEN")
+        db = sqlite_utils.Database(llm.user_dir() / "logs.db")
+        table = db["replicate_predictions"]
+
+        if not table.exists():
+
+            def id_exists(id):
+                return False
+
+        else:
+
+            def id_exists(id):
+                try:
+                    row = table.get(id)
+                    if row["completed_at"]:
+                        return True
+                    # No completed_at, check if it's still running
+                    if row["status"] in ("starting", "processing"):
+                        return False
+                    return True
+                except sqlite_utils.db.NotFoundError:
+                    return False
+
+        # Need all Replicate models to guess model name
+        version_to_model = {
+            ma.model.version_id: "{}/{}".format(ma.model.owner, ma.model.name)
+            for ma in llm.get_models_with_aliases()
+            if isinstance(ma.model, ReplicateModel)
+        }
+
+        # First we fetch a list of all predictions to fetch - to get the total count
+        # so we can show a progress bar
+        next_url = "https://api.replicate.com/v1/predictions"
+        to_fetch = []
+        while next_url:
+            response = requests.get(
+                next_url, headers={"Authorization": "Token {}".format(token)}
+            )
+            if response.status_code != 200:
+                raise click.ClickException(
+                    "Error fetching model details: {}".format(response.text)
+                )
+            data = response.json()
+            next_url = data.get("next")
+            # For each one check if we already have it
+            for result in data["results"]:
+                id = result["id"]
+                if not id_exists(id):
+                    to_fetch.append(result["urls"]["get"])
+
+        def get_prediction(url):
+            r = requests.get(url, headers={"Authorization": "Token {}".format(token)})
+            if r.status_code != 200:
+                raise click.ClickException(
+                    "Error fetching prediction details: {}".format(url)
+                )
+            data = r.json()
+            # Guess the model name, rewrite JSON with _model_guess after id
+            info = {}
+            info["id"] = data.pop("id")
+            info["_model_guess"] = version_to_model.get(data["version"])
+            # Copy remaining keys
+            for key, value in data.items():
+                info[key] = value
+            return info
+
+        # Fetch URLs, with a progress bar
+        with click.progressbar(
+            to_fetch, label="Fetching predictions", show_eta=True, show_pos=True
+        ) as bar:
+            for url in bar:
+                info = get_prediction(url)
+                table.insert(info, pk="id", replace=True, alter=True)
+
 
 @llm.hookimpl
 def register_models(register):
     # First do cached JSON collection
     fetch_models_path = config_dir() / "fetch-models.json"
     if fetch_models_path.exists():
         models = json.loads(fetch_models_path.read_text())
         for details in models:
+            if not details["latest_version"]:
+                # Skipping some broken models
+                continue
             register(
                 ReplicateModel(
                     owner=details["owner"],
                     name=details["name"],
                     version_id=details["latest_version"]["id"],
                     chat=False,
                 ),
@@ -163,24 +252,22 @@
                 f"User: {prompt.prompt}\n",
                 f"Assistant:",
             ]
         )
         return prompt_lines
 
     def execute(self, prompt, stream, response, conversation):
-        from . import vendored_replicate
-
         if conversation and not self.chat:
             raise llm.ModelError("Conversation mode is not supported")
 
         lines = [prompt.prompt]
         if self.chat:
             lines = self.build_chat_prompt(prompt, conversation)
 
-        client = vendored_replicate.Client(api_token=self.get_key())
+        client = replicate.Client(api_token=self.get_key())
         output = client.run(
             "{owner}/{name}:{version_id}".format(
                 owner=self.owner,
                 name=self.name,
                 version_id=self.version_id,
             ),
             input={"prompt": "".join(lines)},
```

### Comparing `llm-replicate-0.2/llm_replicate.egg-info/PKG-INFO` & `llm_replicate-0.3.1/llm_replicate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: llm-replicate
-Version: 0.2
+Version: 0.3.1
 Summary: LLM plugin for models hosted on Replicate
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-replicate
 Project-URL: Changelog, https://github.com/simonw/llm-replicate/releases
 Project-URL: Issues, https://github.com/simonw/llm-replicate/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: llm
+Requires-Dist: requests-mock
+Requires-Dist: replicate>=0.9.0
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # llm-replicate
 
 [![PyPI](https://img.shields.io/pypi/v/llm-replicate.svg)](https://pypi.org/project/llm-replicate/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm-replicate?include_prereleases&label=changelog)](https://github.com/simonw/llm-replicate/releases)
 [![Tests](https://github.com/simonw/llm-replicate/workflows/Test/badge.svg)](https://github.com/simonw/llm-replicate/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm-replicate/blob/main/LICENSE)
@@ -51,14 +56,20 @@
 
 ```bash
 llm replicate add a16z-infra/llama13b-v2-chat \
   --chat --alias llama2
 ```
 The `--chat` flag indicates that this is a chat model, which means it will be able to work with `-c` continue mode.
 
+Here's the [70b version](https://replicate.com/replicate/llama70b-v2-chat) of that model:
+```bash
+llm replicate add \
+  replicate/llama70b-v2-chat \
+  --chat --alias llama70b
+```
 ## Usage
 
 To run a prompt against a model, pass its name or an alias to `llm -m`:
 ```bash
 llm -m llama2 "Ten great names for a pet pelican"
 ```
 
@@ -163,22 +174,61 @@
 10. Splishy
 
 I hope these suggestions help you find the perfect name for your pet pelican! Do you have any other questions?
 User: Five more and make them more nautical
 Assistant:
 ```
 
-## Development
+## Fetching all Replicate predictions
 
-To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+Replicate logs all predictions made against models. You can fetch all of these predictions using the `llm replicate fetch-predictions` command:
 
-    cd llm-palm
-    python3 -m venv venv
-    source venv/bin/activate
+```bash
+llm replicate fetch-predictions
+```
+This will create or populate a table in your LLM `logs.db` database called `replicate_predictions`.
 
-Now install the dependencies and test dependencies:
+The data in this table will cover ALL Replicate models, not just language models that have been queried using this tool.
 
-    pip install -e '.[test]'
+Running `llm replicate fetch-predictions` multiple times will only fetch predictions that have been created since the last time the command was run.
 
-To run the tests:
+To browse the resulting data in [Datasette](https://datasette.io/), run this:
+```bash
+datasette "$(llm logs path)"
+```
+The schema for that table will look like this:
+```sql
+CREATE TABLE [replicate_predictions] (
+   [id] TEXT PRIMARY KEY,
+   [_model_guess] TEXT,
+   [completed_at] TEXT,
+   [created_at] TEXT,
+   [error] TEXT,
+   [input] TEXT,
+   [logs] TEXT,
+   [metrics] TEXT,
+   [output] TEXT,
+   [started_at] TEXT,
+   [status] TEXT,
+   [urls] TEXT,
+   [version] TEXT,
+   [webhook_completed] TEXT
+)
+```
+This schema may change if the Replicate API adds new fields in the future.
 
-    pytest
+## Development
+
+To set up this plugin locally, first checkout the code. Then create a new virtual environment:
+```bash
+cd llm-replicate
+python3 -m venv venv
+source venv/bin/activate
+```
+Now install the dependencies and test dependencies:
+```bash
+pip install -e '.[test]'
+```
+To run the tests:
+```bash
+pytest
+```
```

