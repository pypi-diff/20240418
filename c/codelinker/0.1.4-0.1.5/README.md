# Comparing `tmp/codelinker-0.1.4.tar.gz` & `tmp/codelinker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelinker-0.1.4.tar", max compression
+gzip compressed data, was "codelinker-0.1.5.tar", max compression
```

## Comparing `codelinker-0.1.4.tar` & `codelinker-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-18 08:28:07.884080 codelinker-0.1.4/LICENSE
--rw-r--r--   0        0        0     1968 2024-04-18 08:28:07.884080 codelinker-0.1.4/README.md
--rw-r--r--   0        0        0     1584 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/__init__.py
--rw-r--r--   0        0        0     3392 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/config.py
--rw-r--r--   0        0        0     8412 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/linker.py
--rw-r--r--   0        0        0       64 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/__init__.py
--rw-r--r--   0        0        0      273 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/labels.py
--rw-r--r--   0        0        0      308 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/models/structuredRet.py
--rw-r--r--   0        0        0       32 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/__init__.py
--rw-r--r--   0        0        0    12268 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/objGen.py
--rw-r--r--   0        0        0     5086 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/request/openai.py
--rw-r--r--   0        0        0     1510 2024-04-18 08:28:07.884080 codelinker-0.1.4/codelinker/utils.py
--rw-r--r--   0        0        0      359 2024-04-18 08:28:07.884080 codelinker-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 08:31:55.590747 codelinker-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-18 08:31:55.590747 codelinker-0.1.5/README.md
+-rw-r--r--   0        0        0     1584 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/__init__.py
+-rw-r--r--   0        0        0     3430 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/config.py
+-rw-r--r--   0        0        0     8412 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/linker.py
+-rw-r--r--   0        0        0       64 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/labels.py
+-rw-r--r--   0        0        0      308 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/models/structuredRet.py
+-rw-r--r--   0        0        0       32 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/__init__.py
+-rw-r--r--   0        0        0    12364 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/objGen.py
+-rw-r--r--   0        0        0     5086 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/request/openai.py
+-rw-r--r--   0        0        0     1510 2024-04-18 08:31:55.594747 codelinker-0.1.5/codelinker/utils.py
+-rw-r--r--   0        0        0      359 2024-04-18 08:31:55.594747 codelinker-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.5/PKG-INFO
```

### Comparing `codelinker-0.1.4/LICENSE` & `codelinker-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/README.md` & `codelinker-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/codelinker/__init__.py` & `codelinker-0.1.5/codelinker/__init__.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/codelinker/config.py` & `codelinker-0.1.5/codelinker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         req_name_mapping: dict[str, str] = {
             "gpt-4v": "gpt-4-vision",
             "gpt4": "gpt-4",
             "gpt4-32": "gpt-4-32k",
             "gpt-35-16k": "gpt-3.5-turbo-16k",
         }
 
-        save_completion: bool = False
+        save_completions: bool = False
         # default to save in current working directory 
-        save_completion_path: str = os.getcwd()
+        save_completions_path: str = os.path.join(os.getcwd(),"cache","completions")
 
     request: RequestConfig = RequestConfig()
     
     class ExectionConfig(BaseModel):
         max_ai_functions_tokens: int = 12800
         max_message_tokens: int = 15872
```

### Comparing `codelinker-0.1.4/codelinker/linker.py` & `codelinker-0.1.5/codelinker/linker.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/codelinker/request/objGen.py` & `codelinker-0.1.5/codelinker/request/objGen.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,16 +134,17 @@
 
         rets = []
 
         try:
             async for attempt in AsyncRetrying(stop=stop_after_attempt(max_retry_times), reraise=True):
                 with attempt:
                     response = await self._chatcompletion_request(**kwargs)
-                    if self.config.request.save_completion:
-                        with open(os.path.join(self.config.request.save_completion_path,
+                    if self.config.request.save_completions:
+                        os.makedirs(self.config.request.save_completions_path, exist_ok=True)
+                        with open(os.path.join(self.config.request.save_completions_path,
                                                datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S-%f")+f"{uuid.uuid4().hex}.json"
                                                ), 'w') as f:
                             f.write(json.dumps({
                                 "request": kwargs,
                                 "response": response
                                 }, indent=4))
```

### Comparing `codelinker-0.1.4/codelinker/request/openai.py` & `codelinker-0.1.5/codelinker/request/openai.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/codelinker/utils.py` & `codelinker-0.1.5/codelinker/utils.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.4/PKG-INFO` & `codelinker-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelinker
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: luyaxi
 Author-email: luyaxi@live.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

