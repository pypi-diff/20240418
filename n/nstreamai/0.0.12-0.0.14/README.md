# Comparing `tmp/nstreamai-0.0.12.tar.gz` & `tmp/nstreamai-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstreamai-0.0.12.tar", last modified: Wed Apr 17 16:38:52 2024, max compression
+gzip compressed data, was "nstreamai-0.0.14.tar", last modified: Thu Apr 18 06:12:22 2024, max compression
```

## Comparing `nstreamai-0.0.12.tar` & `nstreamai-0.0.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.438497 nstreamai-0.0.12/
--rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.12/LICENSE
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 16:38:52.438223 nstreamai-0.0.12/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.12/README.md
--rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-17 08:26:03.000000 nstreamai-0.0.12/pyproject.toml
--rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-17 16:38:52.438944 nstreamai-0.0.12/setup.cfg
--rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-17 16:38:49.000000 nstreamai-0.0.12/setup.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.431759 nstreamai-0.0.12/src/
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.437933 nstreamai-0.0.12/src/nstreamai.egg-info/
--rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)      774 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/SOURCES.txt
--rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/dependency_links.txt
--rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/requires.txt
--rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-17 16:38:52.000000 nstreamai-0.0.12/src/nstreamai.egg-info/top_level.txt
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.434023 nstreamai-0.0.12/src/nstreamai_nstream_ai/
--rw-r--r--   0 shiv       (501) staff       (20)       58 2024-04-17 10:42:16.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/__init__.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.435826 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/
--rw-r--r--   0 shiv       (501) staff       (20)      344 2024-04-17 16:23:21.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     4562 2024-04-17 16:29:17.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsgraph.py
--rw-r--r--   0 shiv       (501) staff       (20)     4234 2024-04-17 16:23:11.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsinit.py
--rw-r--r--   0 shiv       (501) staff       (20)      682 2024-04-16 16:23:44.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsneuron.py
--rw-r--r--   0 shiv       (501) staff       (20)     6971 2024-04-17 16:23:36.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsnode.py
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-17 16:38:52.437742 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/
--rw-r--r--   0 shiv       (501) staff       (20)     1260 2024-04-17 16:24:48.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/logger.py
--rw-r--r--   0 shiv       (501) staff       (20)     1193 2024-04-17 16:25:03.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/output_data.py
--rw-r--r--   0 shiv       (501) staff       (20)     1600 2024-04-17 16:25:26.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/run.py
--rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-17 16:25:37.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/template.py
--rw-r--r--   0 shiv       (501) staff       (20)     1182 2024-04-17 08:18:32.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/variables.py
--rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-17 08:20:20.000000 nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/welcome.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.925499 nstreamai-0.0.14/
+-rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.14/LICENSE
+-rw-r--r--   0 shiv       (501) staff       (20)    16474 2024-04-18 06:12:22.925398 nstreamai-0.0.14/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)    15297 2024-04-18 06:10:11.000000 nstreamai-0.0.14/README.md
+-rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-17 08:26:03.000000 nstreamai-0.0.14/pyproject.toml
+-rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-18 06:12:22.925771 nstreamai-0.0.14/setup.cfg
+-rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-18 06:12:18.000000 nstreamai-0.0.14/setup.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.918908 nstreamai-0.0.14/src/
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.925066 nstreamai-0.0.14/src/nstreamai.egg-info/
+-rw-r--r--   0 shiv       (501) staff       (20)    16474 2024-04-18 06:12:22.000000 nstreamai-0.0.14/src/nstreamai.egg-info/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)      774 2024-04-18 06:12:22.000000 nstreamai-0.0.14/src/nstreamai.egg-info/SOURCES.txt
+-rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-18 06:12:22.000000 nstreamai-0.0.14/src/nstreamai.egg-info/dependency_links.txt
+-rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-18 06:12:22.000000 nstreamai-0.0.14/src/nstreamai.egg-info/requires.txt
+-rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-18 06:12:22.000000 nstreamai-0.0.14/src/nstreamai.egg-info/top_level.txt
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.921083 nstreamai-0.0.14/src/nstreamai_nstream_ai/
+-rw-r--r--   0 shiv       (501) staff       (20)       58 2024-04-17 10:42:16.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/__init__.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.922687 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/
+-rw-r--r--   0 shiv       (501) staff       (20)      344 2024-04-17 16:23:21.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     4575 2024-04-18 05:58:19.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsgraph.py
+-rw-r--r--   0 shiv       (501) staff       (20)     4198 2024-04-18 06:02:15.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsinit.py
+-rw-r--r--   0 shiv       (501) staff       (20)      682 2024-04-16 16:23:44.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsneuron.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6971 2024-04-17 16:23:36.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsnode.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-18 06:12:22.924767 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/
+-rw-r--r--   0 shiv       (501) staff       (20)     1260 2024-04-17 16:24:48.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/__init__.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1890 2024-04-16 12:19:23.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/logger.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1193 2024-04-17 16:25:03.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/output_data.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1600 2024-04-17 16:25:26.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/run.py
+-rw-r--r--   0 shiv       (501) staff       (20)     6263 2024-04-17 16:25:37.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/template.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1178 2024-04-18 05:46:06.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/variables.py
+-rw-r--r--   0 shiv       (501) staff       (20)     1191 2024-04-17 08:20:20.000000 nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/welcome.py
```

### Comparing `nstreamai-0.0.12/LICENSE` & `nstreamai-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/PKG-INFO` & `nstreamai-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.12
+Version: 0.0.14
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
@@ -255,15 +255,14 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).end(ns_node_2).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ##
 ### Using the Nstream SDK for Genaration Usage Example
 
 #### Building the Pipeline
@@ -301,15 +300,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 Final Code:
 ```python
 
 # Import necessary modules from the Nstream SDK and utility libraries
@@ -364,15 +362,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ### Using the Nstream SDK for Context transformation Usage Example
 In this section, we demonstrate a use case of the Nstream SDK for transforming user data 
 into a structured format for analysis and insights.
 
@@ -419,10 +416,9 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
```

### Comparing `nstreamai-0.0.12/README.md` & `nstreamai-0.0.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -219,15 +219,14 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).end(ns_node_2).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ##
 ### Using the Nstream SDK for Genaration Usage Example
 
 #### Building the Pipeline
@@ -265,15 +264,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 Final Code:
 ```python
 
 # Import necessary modules from the Nstream SDK and utility libraries
@@ -328,15 +326,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ### Using the Nstream SDK for Context transformation Usage Example
 In this section, we demonstrate a use case of the Nstream SDK for transforming user data 
 into a structured format for analysis and insights.
 
@@ -383,10 +380,9 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
```

### Comparing `nstreamai-0.0.12/setup.py` & `nstreamai-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 else:
     platform_specific_requires = []
 # if sys.platform == 'darwin':  # macOS
 #     extension_mod.extra_compile_args = ['-stdlib=libc++']
 
 setup(
     name='nstreamai',
-    version='0.0.12',
+    version='0.0.14',
     description='Official SDK for nstream ai stream processing powered by Gen AI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords="nstreamai, streaming, rag, analytics, realtime",
     package_dir={"": "src"},
     python_requires=">=3.8, <4",
     packages=find_packages(where="src"),
```

### Comparing `nstreamai-0.0.12/src/nstreamai.egg-info/PKG-INFO` & `nstreamai-0.0.14/src/nstreamai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nstreamai
-Version: 0.0.12
+Version: 0.0.14
 Summary: Official SDK for nstream ai stream processing powered by Gen AI
 Home-page: https://github.com/nstream-ai/ms-public-sdk
 Author: Nstream AI
 Author-email: hello@nstream.ai
 License: MIT
 Keywords: nstreamai,streaming,rag,analytics,realtime
 Classifier: License :: OSI Approved :: MIT License
@@ -255,15 +255,14 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).end(ns_node_2).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ##
 ### Using the Nstream SDK for Genaration Usage Example
 
 #### Building the Pipeline
@@ -301,15 +300,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 Final Code:
 ```python
 
 # Import necessary modules from the Nstream SDK and utility libraries
@@ -364,15 +362,14 @@
     logger.info("Graph execution started")
 
     # Terminate the graph execution after a predefined runtime
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
     # Signal completion of the main execution
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
 
 ### Using the Nstream SDK for Context transformation Usage Example
 In this section, we demonstrate a use case of the Nstream SDK for transforming user data 
 into a structured format for analysis and insights.
 
@@ -419,10 +416,9 @@
 
     ns_graph = NsGraph(conn).start(ns_node_1).submit(ns_graph_sink)
     logger.info("Graph execution started")
 
     ns_graph.terminate(run_time=6)
     logger.info("Graph execution terminated")
 
-    print("Execution Completed")
     logger.info("Main execution completed")
 ```
```

### Comparing `nstreamai-0.0.12/src/nstreamai.egg-info/SOURCES.txt` & `nstreamai-0.0.14/src/nstreamai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsgraph.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,40 +72,39 @@
         node_dict = dict()
         return node_dict
 
     def run_data_out(self, run_time) -> None:
         st = time.time()
         while run_time > 0:
             # Generate synthetic data
-            data = generate_synthetic_data()
-            data["node_id"] = random.choice(self.list_node_id)
+            for node_id in self.list_node_id:
+                data = generate_synthetic_data()
+                mutation = create_token_detail_mutation(data["tokens"],
+                                                        node_id)
+                _ = send_graphql_request(self.socket.dashboard_server,
+                                        self.socket.headers, mutation)
 
-            mutation = create_token_detail_mutation(data["tokens"],
-                                                    data["node_id"])
-            _ = send_graphql_request(self.socket.dashboard_server,
-                                     self.socket.headers, mutation)
+                mutation = create_io_throughput_mutation(node_id,
+                                                        data["input_throughput"],
+                                                        data["output_throughput"])
+                _ = send_graphql_request(self.socket.dashboard_server,
+                                        self.socket.headers, mutation)
 
-            mutation = create_io_throughput_mutation(data["node_id"],
-                                                     data["input_throughput"],
-                                                     data["output_throughput"])
-            _ = send_graphql_request(self.socket.dashboard_server,
-                                     self.socket.headers, mutation)
-
-            mutation = create_inference_latency_mutation(
-                data["node_id"], data["llm_inference_speed"],
-                data["context_retrieval_speed"],
-                data["total_node_inference_speed"])
-            _ = send_graphql_request(self.socket.dashboard_server,
-                                     self.socket.headers, mutation)
-            
+                mutation = create_inference_latency_mutation(
+                    node_id, data["llm_inference_speed"],
+                    data["context_retrieval_speed"],
+                    data["total_node_inference_speed"])
+                _ = send_graphql_request(self.socket.dashboard_server,
+                                        self.socket.headers, mutation)
+                
             # Example usage
             message = generate_openai_data(oauth_token=self.socket.oauth, endpoint=self.socket.api_server).choices[0].message.content
             key = random.randint(1, 10)
             message = json.loads(message)
-            mutation = create_node_message_mutation(message=message, node_id=int(data["node_id"]), key=key)
+            mutation = create_node_message_mutation(message=message, node_id=int(node_id), key=key)
             result = send_graphql_request(
                 self.socket.dashboard_server,
                 self.socket.headers,
                 mutation
                 )
             logger.info(result.json())
             logger.info(f"Pushed Output")
```

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsinit.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsinit.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         self.params = {}
         logger.info("NsInit initialized with API key: {0}".format(api_key))
 
     def generate_oauth(self)->str:
         try:
             result = self.socket.call_rest_endpoint(method="POST", route="sign-in", payload={"email": self.username, "password": self.password})
             self.oauth_token = result.json().get("access_token")
-            print(self.oauth_token)
         except Exception as e: 
             print(e)
 
     def connect(self) -> NsSocket:
         try:
             self.generate_oauth()
             if self.oauth_token:
```

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsneuron.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsneuron.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/core/nsnode.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/core/nsnode.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/__init__.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/logger.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/output_data.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/output_data.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/run.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/run.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/template.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/template.py`

 * *Files identical despite different names*

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/variables.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     return json.dumps({
         random_string(5): random_string(5)
         for _ in range(random.randint(1, 1))
     })
 
 
 def generate_synthetic_data():
-    tokens = random.randint(50, 500)
-    input_throughput = random.randint(50, 1000)
-    output_throughput = random.randint(50, 1000)
-    llm_inference_speed = random.randint(10, 5000)
-    context_retrieval_speed = random.randint(10, 5000)
+    tokens = random.randint(10, 300)
+    input_throughput = random.randint(50, 500)
+    output_throughput = random.randint(50, 500)
+    llm_inference_speed = random.randint(10, 800)
+    context_retrieval_speed = random.randint(10, 300)
     total_node_inference_speed = llm_inference_speed + context_retrieval_speed + random.randint(
         10, 100)
 
     return {
         "tokens": tokens,
         "input_throughput": input_throughput,
         "output_throughput": output_throughput,
```

### Comparing `nstreamai-0.0.12/src/nstreamai_nstream_ai/utils/welcome.py` & `nstreamai-0.0.14/src/nstreamai_nstream_ai/utils/welcome.py`

 * *Files identical despite different names*

