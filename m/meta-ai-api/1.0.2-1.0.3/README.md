# Comparing `tmp/meta_ai_api-1.0.2.tar.gz` & `tmp/meta_ai_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.2.tar", last modified: Thu Apr 18 21:28:25 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.3.tar", last modified: Thu Apr 18 21:36:36 2024, max compression
```

## Comparing `meta_ai_api-1.0.2.tar` & `meta_ai_api-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.888744 meta_ai_api-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:36:36.502407 meta_ai_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-18 21:36:36.502407 meta_ai_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-18 21:36:31.000000 meta_ai_api-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:36:31.000000 meta_ai_api-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:36:36.502407 meta_ai_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:36:31.000000 meta_ai_api-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:36:36.498407 meta_ai_api-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:36:36.498407 meta_ai_api-1.0.3/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:36:31.000000 meta_ai_api-1.0.3/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-18 21:36:31.000000 meta_ai_api-1.0.3/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:36:36.502407 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-18 21:36:36.000000 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:36:36.000000 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:36:36.000000 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:36:36.000000 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:36:36.000000 meta_ai_api-1.0.3/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.2/PKG-INFO` & `meta_ai_api-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -23,22 +23,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
-# MetaAI
+# MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
+Meta AI is running Llama 3 LLM.
+
 ## Usage
 1. **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```

### Comparing `meta_ai_api-1.0.2/README.md` & `meta_ai_api-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# MetaAI
+# MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
+Meta AI is running Llama 3 LLM.
+
 ## Usage
 1. **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```

### Comparing `meta_ai_api-1.0.2/setup.py` & `meta_ai_api-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.2/src/meta_ai_api/main.py` & `meta_ai_api-1.0.3/src/meta_ai_api/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import requests
 from requests_html import HTMLSession
 
 
 class MetaAI:
     def __init__(self):
         self.session = requests.Session()
-        self.access_token = self.get_access_token()
 
     def get_access_token(self):
         cookies = self.get_cookies()
         url = "https://www.meta.ai/api/graphql/"
 
         payload = "av=0&__user=0&__a=1&__req=4&__ccg=UNKNOWN&lsd=AVrWIDJrQQI&__jssesw=1&fb_api_caller_class=RelayModern&fb_api_req_friendly_name=useAbraAcceptTOSForTempUserMutation&variables=%7B%22dob%22%3A%221999-01-01%22%2C%22icebreaker_type%22%3A%22TEXT%22%2C%22__relay_internal__pv__WebPixelRatiorelayprovider%22%3A1%7D&server_timestamps=true&doc_id=7604648749596940"
         headers = {
@@ -45,32 +44,39 @@
         abra_csrf_start = raw_text.find('abra_csrf":{"value":"')
         abra_csrf_end = raw_text.find('",', abra_csrf_start)
         abra_csrf = raw_text[abra_csrf_start:abra_csrf_end].replace(
             'abra_csrf":{"value":"', ""
         )
         return {"_js_datr": _js_datr, "abra_csrf": abra_csrf}
 
-    def prompt(self, message: str):
+    def prompt(self, message: str, attempts: int = 0):
         url = "https://graph.meta.ai/graphql?locale=user"
 
-        payload = f"av=0&access_token={self.access_token}&__user=0&__a=1&__req=p&__hs=19831.HYP%3Aabra_pkg.2.1..0.0&dpr=1&__ccg=UNKNOWN&__s=%3A0ryskm%3Aewvpqb&__comet_req=46&lsd=AVrLt4uZ-4k&__spin_b=trunk&__jssesw=1&fb_api_caller_class=RelayModern&fb_api_req_friendly_name=useAbraSendMessageMutation&variables=%7B%22message%22%3A%7B%22sensitive_string_value%22%3A%22{message}%22%7D%2C%22externalConversationId%22%3A%22dae20bda-6450-4ce7-880c-1db1b3ae7da3%22%2C%22offlineThreadingId%22%3A%227186784311738402039%22%2C%22suggestedPromptIndex%22%3Anull%2C%22flashVideoRecapInput%22%3A%7B%22images%22%3A%5B%5D%7D%2C%22flashPreviewInput%22%3Anull%2C%22promptPrefix%22%3Anull%2C%22entrypoint%22%3A%22ABRA__CHAT__TEXT%22%2C%22icebreaker_type%22%3A%22TEXT%22%2C%22__relay_internal__pv__AbraDebugDevOnlyrelayprovider%22%3Afalse%2C%22__relay_internal__pv__WebPixelRatiorelayprovider%22%3A1%7D&server_timestamps=true&doc_id=7783822248314888"
+        payload = f"av=0&access_token={self.get_access_token()}&__user=0&__a=1&__req=p&__hs=19831.HYP%3Aabra_pkg.2.1..0.0&dpr=1&__ccg=UNKNOWN&__s=%3A0ryskm%3Aewvpqb&__comet_req=46&lsd=AVrLt4uZ-4k&__spin_b=trunk&__jssesw=1&fb_api_caller_class=RelayModern&fb_api_req_friendly_name=useAbraSendMessageMutation&variables=%7B%22message%22%3A%7B%22sensitive_string_value%22%3A%22{message}%22%7D%2C%22externalConversationId%22%3A%22dae20bda-6450-4ce7-880c-1db1b3ae7da3%22%2C%22offlineThreadingId%22%3A%227186784311738402039%22%2C%22suggestedPromptIndex%22%3Anull%2C%22flashVideoRecapInput%22%3A%7B%22images%22%3A%5B%5D%7D%2C%22flashPreviewInput%22%3Anull%2C%22promptPrefix%22%3Anull%2C%22entrypoint%22%3A%22ABRA__CHAT__TEXT%22%2C%22icebreaker_type%22%3A%22TEXT%22%2C%22__relay_internal__pv__AbraDebugDevOnlyrelayprovider%22%3Afalse%2C%22__relay_internal__pv__WebPixelRatiorelayprovider%22%3A1%7D&server_timestamps=true&doc_id=7783822248314888"
         headers = {
             "content-type": "application/x-www-form-urlencoded",
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             "x-fb-friendly-name": "useAbraSendMessageMutation",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         raw_response = response.text
         last_streamed_response = None
         text = ""
         for line in raw_response.split("\n"):
             json_line = json.loads(line)
             if "errors" not in json_line.keys():
                 last_streamed_response = json_line
+
+        if last_streamed_response is None:
+            if attempts > 3:
+                raise Exception(
+                    "Was not able to query Meta AI. Either patched or MetaAI is having issues."
+                )
+            return self.prompt(message=message, attempts=attempts + 1)
         for content in last_streamed_response["data"]["node"]["bot_response_message"][
             "composed_text"
         ]["content"]:
             text += content["text"] + "\n"
         return text
```

### Comparing `meta_ai_api-1.0.2/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.3/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
@@ -23,22 +23,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: requests-html
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 
-# MetaAI
+# MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
+Meta AI is running Llama 3 LLM.
+
 ## Usage
 1. **Download**:
 
    ```bash
    pip install meta-ai-api
    ```
```

