# Comparing `tmp/optscale_arcee-0.1.38.tar.gz` & `tmp/optscale_arcee-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.38.tar", last modified: Tue Apr  2 10:01:11 2024, max compression
+gzip compressed data, was "optscale_arcee-0.1.39.tar", last modified: Thu Apr 18 12:55:11 2024, max compression
```

## Comparing `optscale_arcee-0.1.38.tar` & `optscale_arcee-0.1.39.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/arcee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/sender/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/sender/sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/tests/test_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.827022 optscale_arcee-0.1.39/optscale_arcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/arcee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/collectors/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/platforms_meta/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/sender/sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/optscale_arcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/optscale_arcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:55:11.000000 optscale_arcee-0.1.39/optscale_arcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:55:11.831022 optscale_arcee-0.1.39/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-18 12:55:08.000000 optscale_arcee-0.1.39/tests/test_platform.py
```

### Comparing `optscale_arcee-0.1.38/LICENSE` & `optscale_arcee-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/PKG-INFO` & `optscale_arcee-0.1.39/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.38
+Version: 0.1.39
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/hystax/optscale_arcee
 Keywords: arcee,ml,optscale,finops,mlops
 Requires-Python: <4,>=3.7
@@ -96,12 +96,23 @@
 To create a model, use the model method with the following parameters:
 - key (str): the unique key of the model
 - path (str): the path of the run artifacts
 ```
 arcee.model("my_model", "/home/user/my_model")
 ```
 
-To set custom model version, use the set_model_version method with the following parameter:
+To set a custom model version, use the model_version method with the following parameter:
 - version (str): version name
 ```
-arcee.set_model_version("1.2.3-release")
+arcee.model_version("1.2.3-release")
+```
+
+To set a model version alias, use the model_version_alias method with the following parameter:
+- alias (str): alias name
+```
+arcee.model_version_alias("winner")
+```
+
+To add tags to model version (key, value):
+```
+arcee.model_version_tag("env", "staging demo")
 ```
```

### Comparing `optscale_arcee-0.1.38/README.md` & `optscale_arcee-0.1.39/optscale_arcee.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: optscale_arcee
+Version: 0.1.39
+Summary: ML profiling tool for OptScale
+Home-page: https://my.optscale.com/
+Author: Hystax
+License: "Apache License 2.0"
+Project-URL: Source, https://github.com/hystax/optscale_arcee
+Keywords: arcee,ml,optscale,finops,mlops
+Requires-Python: <4,>=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.8.4
+Requires-Dist: aiofiles==22.1.0
+Requires-Dist: GPUtil==1.4.0
+Requires-Dist: psutil==5.9.2
+
 # Arcee
 ## *The OptScale ML profiling tool by Hystax*
 
 Arcee is a tool that hepls you to integrate ML tasks with [OptScale](https://my.optscale.com/).
 This tool can automatically collect executor metadata from cloud and process stats.
 
 ## Installation
@@ -79,12 +96,23 @@
 To create a model, use the model method with the following parameters:
 - key (str): the unique key of the model
 - path (str): the path of the run artifacts
 ```
 arcee.model("my_model", "/home/user/my_model")
 ```
 
-To set custom model version, use the set_model_version method with the following parameter:
+To set a custom model version, use the model_version method with the following parameter:
 - version (str): version name
 ```
-arcee.set_model_version("1.2.3-release")
-```
+arcee.model_version("1.2.3-release")
+```
+
+To set a model version alias, use the model_version_alias method with the following parameter:
+- alias (str): alias name
+```
+arcee.model_version_alias("winner")
+```
+
+To add tags to model version (key, value):
+```
+arcee.model_version_tag("env", "staging demo")
+```
```

### Comparing `optscale_arcee-0.1.38/optscale_arcee/arcee.py` & `optscale_arcee-0.1.39/optscale_arcee/arcee.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         self.hb = None
         self._run = None
         self._tags = dict()
         self._name = None
         self._hyperparams = dict()
         self._dataset = None
         self._model = None
+        self._model_version = None
+        self._model_version_tags = dict()
+        self._model_version_aliases = list()
 
     @property
     def run(self):
         return self._run
 
     @run.setter
     def run(self, value):
@@ -107,14 +110,41 @@
     def model(self):
         return self._model
 
     @model.setter
     def model(self, value):
         self._model = value
 
+    @property
+    def model_version(self):
+        return self._model_version
+
+    @model_version.setter
+    def model_version(self, value):
+        self._model_version = value
+
+    @property
+    def model_version_tags(self):
+        return self._model_version_tags
+
+    @model_version_tags.setter
+    def model_version_tags(self, value):
+        k, v = value
+        self._model_version_tags.update({k: v})
+
+    @property
+    def model_version_aliases(self):
+        return self._model_version_aliases
+
+    @model_version_aliases.setter
+    def model_version_aliases(self, value):
+        aliases = set(self._model_version_aliases)
+        aliases.add(value)
+        self._model_version_aliases = list(aliases)
+
 
 def init(
     token, task_key=None, run_name=None, endpoint_url=None, ssl=True, period=1,
         model_key=None
 ):
     if model_key:
         warnings.warn(
@@ -257,14 +287,34 @@
     asyncio.run(
         arcee.sender.assign_model_run(
             arcee.model, arcee.run, arcee.token, path=path
         )
     )
 
 
-def set_model_version(version):
+def model_version(version):
     arcee = Arcee()
     asyncio.run(
         arcee.sender.add_version(
             arcee.model, arcee.run, arcee.token, version
         )
     )
+
+
+def model_version_alias(alias):
+    arcee = Arcee()
+    arcee.model_version_aliases = alias
+    asyncio.run(
+        arcee.sender.add_version_aliases(
+            arcee.model, arcee.run, arcee.token, arcee.model_version_aliases
+        )
+    )
+
+
+def model_version_tag(key, value):
+    arcee = Arcee()
+    arcee.model_version_tags = (key, value)
+    asyncio.run(
+        arcee.sender.add_version_tags(
+            arcee.model, arcee.run, arcee.token, arcee.model_version_tags
+        )
+    )
```

### Comparing `optscale_arcee-0.1.38/optscale_arcee/collectors/console.py` & `optscale_arcee-0.1.39/optscale_arcee/collectors/console.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/collectors/git.py` & `optscale_arcee-0.1.39/optscale_arcee/collectors/git.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/collectors/hardware.py` & `optscale_arcee-0.1.39/optscale_arcee/collectors/hardware.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/collectors/module.py` & `optscale_arcee-0.1.39/optscale_arcee/collectors/module.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.39/optscale_arcee/name_generator.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/platform.py` & `optscale_arcee-0.1.39/optscale_arcee/platform.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.39/optscale_arcee/platforms_meta/azure.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.39/optscale_arcee/sender/sender.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,12 +175,23 @@
     async def assign_model_run(self, model_id, run_id, token, path=None):
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
         body = {'path': path} if path else {}
         await self.send_post_request(uri, headers, body)
 
     @check_shutdown_flag_set
-    async def add_version(self, model_id, run_id, token, version):
+    async def patch_model_version(self, model_id, run_id, token, params):
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
+        await self.send_patch_request(uri, headers, params)
+
+    async def add_version(self, model_id, run_id, token, version):
         body = {'version': str(version)}
-        await self.send_patch_request(uri, headers, body)
+        await self.patch_model_version(model_id, run_id, token, body)
+
+    async def add_version_aliases(self, model_id, run_id, token, aliases):
+        body = {'aliases': aliases}
+        await self.patch_model_version(model_id, run_id, token, body)
+
+    async def add_version_tags(self, model_id, run_id, token, tags):
+        body = {'tags': tags}
+        await self.patch_model_version(model_id, run_id, token, body)
```

### Comparing `optscale_arcee-0.1.38/optscale_arcee/utils.py` & `optscale_arcee-0.1.39/optscale_arcee/utils.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/optscale_arcee.egg-info/SOURCES.txt` & `optscale_arcee-0.1.39/optscale_arcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/setup.cfg` & `optscale_arcee-0.1.39/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.38
+version = 0.1.39
 author = Hystax
 description = ML profiling tool for OptScale
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "Apache License 2.0"
 url = https://my.optscale.com/
 project_urls =
```

### Comparing `optscale_arcee-0.1.38/tests/test_data.py` & `optscale_arcee-0.1.39/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.38/tests/test_platform.py` & `optscale_arcee-0.1.39/tests/test_platform.py`

 * *Files identical despite different names*

