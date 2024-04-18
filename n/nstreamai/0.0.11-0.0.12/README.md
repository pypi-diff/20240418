# Comparing `tmp/nstreamai-0.0.11.tar.gz` & `tmp/nstreamai-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstreamai-0.0.11.tar", last modified: Wed Apr 17 08:26:39 2024, max compression
+gzip compressed data, was "nstreamai-0.0.12.tar", last modified: Wed Apr 17 16:38:52 2024, max compression
```

## Comparing `nstreamai-0.0.11.tar` & `nstreamai-0.0.12.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.396360 nstreamai-0.0.11/
--rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.11/LICENSE
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 08:26:39.396274 nstreamai-0.0.11/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.11/README.md
--rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-17 08:26:03.000000 nstreamai-0.0.11/pyproject.toml
--rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-17 08:26:39.396605 nstreamai-0.0.11/setup.cfg
--rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-17 08:26:10.000000 nstreamai-0.0.11/setup.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.389042 nstreamai-0.0.11/src/
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.395967 nstreamai-0.0.11/src/nstreamai.egg-info/
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)      774 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/SOURCES.txt
--rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/dependency_links.txt
--rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/requires.txt
--rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-17 08:26:39.000000 nstreamai-0.0.11/src/nstreamai.egg-info/top_level.txt
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.391237 nstreamai-0.0.11/src/nstreamai_nstream_ai/
--rw-r--r--   0 shiv       (501) staff       (20)       58 2024-04-17 08:25:05.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/__init__.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.392952 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/
--rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 08:25:23.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     4490 2024-04-17 07:56:39.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsgraph.py
--rw-r--r--   0 shiv       (501) staff       (20)     3924 2024-04-16 16:23:31.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsinit.py
--rw-r--r--   0 shiv       (501) staff       (20)      682 2024-04-16 16:23:44.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsneuron.py
--rw-r--r--   0 shiv       (501) staff       (20)     6971 2024-04-16 16:23:55.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsnode.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 08:26:39.395738 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/
--rw-r--r--   0 shiv       (501) staff       (20)     1244 2024-04-17 08:25:18.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/logger.py
--rw-r--r--   0 shiv       (501) staff       (20)      531 2024-04-17 08:17:40.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/output_data.py
--rw-r--r--   0 shiv       (501) staff       (20)     5542 2024-04-17 08:17:24.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/run.py
--rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-17 08:16:45.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/template.py
--rw-r--r--   0 shiv       (501) staff       (20)     1182 2024-04-17 08:18:32.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/variables.py
--rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-17 08:20:20.000000 nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/welcome.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.438497 nstreamai-0.0.12/
+-rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.12/LICENSE
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 16:38:52.438223 nstreamai-0.0.12/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.12/README.md
+-rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-17 08:26:03.000000 nstreamai-0.0.12/pyproject.toml
+-rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-17 16:38:52.438944 nstreamai-0.0.12/setup.cfg
+-rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-17 16:38:49.000000 nstreamai-0.0.12/setup.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.431759 nstreamai-0.0.12/src/
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.437933 nstreamai-0.0.12/src/nstreamai.egg-info/
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)      774 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/SOURCES.txt
+-rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/dependency_links.txt
+-rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/requires.txt
+-rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/top_level.txt
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.434023 nstreamai-0.0.12/src/nstreamai_nstream_ai/
+-rw-r--r--   0 shiv       (501) staff       (20)       58 2024-04-17 10:42:16.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/__init__.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.435826 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/
+-rw-r--r--   0 shiv       (501) staff       (20)      344 2024-04-17 16:23:21.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     4562 2024-04-17 16:29:17.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsgraph.py
+-rw-r--r--   0 shiv       (501) staff       (20)     4234 2024-04-17 16:23:11.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsinit.py
+-rw-r--r--   0 shiv       (501) staff       (20)      682 2024-04-16 16:23:44.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsneuron.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6971 2024-04-17 16:23:36.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsnode.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.437742 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/
+-rw-r--r--   0 shiv       (501) staff       (20)     1260 2024-04-17 16:24:48.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/logger.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1193 2024-04-17 16:25:03.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/output_data.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1600 2024-04-17 16:25:26.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/run.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-17 16:25:37.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/template.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1182 2024-04-17 08:18:32.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/variables.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-17 08:20:20.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/welcome.py
```

### Comparing `nstreamai-0.0.11/LICENSE` & `nstreamai-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/PKG-INFO` & `nstreamai-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.11
+Version: 0.0.12
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nstreamai-0.0.11/README.md` & `nstreamai-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/setup.py` & `nstreamai-0.0.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 else:
     platform_specific_requires = []
 # if sys.platform == 'darwin':  # macOS
 #     extension_mod.extra_compile_args = ['-stdlib=libc++']
 
 setup(
     name='nstreamai',
-    version='0.0.11',
+    version='0.0.12',
     description='Official SDK for nstream ai stream processing powered by Gen AI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords="nstreamai, streaming, rag, analytics, realtime",
     package_dir={"": "src"},
     python_requires=">=3.8, <4",
     packages=find_packages(where="src"),
```

### Comparing `nstreamai-0.0.11/src/nstreamai.egg-info/PKG-INFO` & `nstreamai-0.0.12/src/nstreamai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.11
+Version: 0.0.12
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nstreamai-0.0.11/src/nstreamai.egg-info/SOURCES.txt` & `nstreamai-0.0.12/src/nstreamai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsgraph.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     create_token_detail_mutation, 
     create_io_throughput_mutation, 
     create_inference_latency_mutation,
     create_node_message_mutation
     )
 from ..utils.logger import logger
 import json
-from ..utils.output_data import chat_completion
+from ..utils.output_data import generate_openai_data
 
 
 class NsGraph(object):
 
     def __init__(self, socket: NsSocket) -> None:
         self.graph = list(dict())
         self.socket = socket
@@ -59,15 +59,15 @@
         return self
 
     def terminate(self, run_time):
         logger.info("Processing graph")
         if run_time:
             self.run_data_out(run_time=run_time)
             payload = json.dumps([int(i) for i in self.list_node_id])
-            # _ = self.socket.call_rest_endpoint(method="DELETE", route="nodes", payload=payload)
+            _ = self.socket.call_rest_endpoint(method="DELETE", route="nodes", payload=payload)
         self.socket.call_grpc_endpoint(method=(lambda x: x))
         return self
 
     @staticmethod
     def node_to_dict(node: NsNode) -> Dict:
         node_dict = dict()
         return node_dict
@@ -94,15 +94,15 @@
                 data["node_id"], data["llm_inference_speed"],
                 data["context_retrieval_speed"],
                 data["total_node_inference_speed"])
             _ = send_graphql_request(self.socket.dashboard_server,
                                      self.socket.headers, mutation)
             
             # Example usage
-            message = chat_completion.choices[0].message.content
+            message = generate_openai_data(oauth_token=self.socket.oauth, endpoint=self.socket.api_server).choices[0].message.content
             key = random.randint(1, 10)
             message = json.loads(message)
             mutation = create_node_message_mutation(message=message, node_id=int(data["node_id"]), key=key)
             result = send_graphql_request(
                 self.socket.dashboard_server,
                 self.socket.headers,
                 mutation
```

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsinit.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsinit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import json
 import httpx
 import requests
 from types import FunctionType
 from ..utils.logger import logger
 from ..utils.welcome import welcome
 from typing import Dict, Optional
-
+import os
 
 class NsSocket(object):
     def __init__(
             self,
             grpc_endpoint: str = "api.nstream.ai:50031",
             api_server_url: str = "https://api.nstream.ai",
             headers: dict = {},
-            dashboard_server: str = "https://api.nstream.ai/graphql") -> None:
+            dashboard_server: str = "https://api.nstream.ai/graphql", 
+            oauth_token: str = None) -> None:
         self.grpc_endpoint = grpc_endpoint
         self.http_client = httpx.Client()
         self.api_server = api_server_url
         self.dashboard_server = dashboard_server
         self.status = False
         self.headers = headers
+        self.oauth = oauth_token
         logger.info("NsSocket initialized with API server: {0}".format(api_server_url))
 
     def call_grpc_endpoint(self, method: FunctionType):
         self.status = True
         logger.info("gRPC endpoint called")
         return self.status
 
@@ -55,30 +57,38 @@
 class NsInit(object):
     def __init__(self, api_key="", username="", password="") -> None:
         welcome()
         self.api_key = api_key
         self.username = username
         self.password = password
         self.socket = NsSocket()
+        self.oauth_token = ""
         self.headers = {}
         self.params = {}
         logger.info("NsInit initialized with API key: {0}".format(api_key))
 
-    def connect(self) -> NsSocket:
+    def generate_oauth(self)->str:
         try:
             result = self.socket.call_rest_endpoint(method="POST", route="sign-in", payload={"email": self.username, "password": self.password})
-            print(result)
-            oauth_token = result.json().get("access_token")
-            if oauth_token:
-                self.headers = {"Authorization": "Bearer {0}".format(oauth_token), 'Content-Type': 'application/json'}
-                self.socket = NsSocket(headers=self.headers)
+            self.oauth_token = result.json().get("access_token")
+            print(self.oauth_token)
+        except Exception as e: 
+            print(e)
+
+    def connect(self) -> NsSocket:
+        try:
+            self.generate_oauth()
+            if self.oauth_token:
+                self.headers = {"Authorization": "Bearer {0}".format(self.oauth_token), 'Content-Type': 'application/json'}
                 logger.info("Authorization Token Received")
             else:
                 logger.error("Failed to retrieve authorization token")
                 raise Exception("Failed to authenticate")
+            
+            self.socket = NsSocket(headers=self.headers, oauth_token=self.oauth_token)
 
             result = self.socket.call_rest_endpoint(route="validate-api-key/{}".format(self.api_key))
             result = result.json()
             api_secret = result.get("api_secret")
             if api_secret:
                 logger.info("API Key approved")
                 return self.socket
```

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsneuron.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsneuron.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/core/nsnode.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsnode.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/logger.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/template.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/template.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/variables.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/variables.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.11/src/nstreamai_nstream_ai/utils/welcome.py` & `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/welcome.py`

 * *Files identical despite different names*

