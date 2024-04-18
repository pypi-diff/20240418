# Comparing `tmp/orq_ai_sdk-2.3.3.tar.gz` & `tmp/orq_ai_sdk-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orq_ai_sdk-2.3.3.tar", max compression
+gzip compressed data, was "orq_ai_sdk-2.3.4.tar", max compression
```

## Comparing `orq_ai_sdk-2.3.3.tar` & `orq_ai_sdk-2.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2024-03-15 09:27:20.060670 orq_ai_sdk-2.3.3/LICENSE
--rw-r--r--   0        0        0     7382 2024-03-21 12:42:41.520384 orq_ai_sdk-2.3.3/README.md
--rw-r--r--   0        0        0       38 2024-03-15 09:27:20.061191 orq_ai_sdk-2.3.3/orq_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 09:27:20.061230 orq_ai_sdk-2.3.3/orq_ai_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0    14123 2024-03-26 00:32:08.214534 orq_ai_sdk-2.3.3/orq_ai_sdk/api_resources/async_deployments.py
--rw-r--r--   0        0        0    14144 2024-03-26 00:32:08.257393 orq_ai_sdk-2.3.3/orq_ai_sdk/api_resources/deployments.py
--rw-r--r--   0        0        0     2739 2024-03-15 09:27:20.061820 orq_ai_sdk-2.3.3/orq_ai_sdk/client.py
--rw-r--r--   0        0        0     1653 2024-03-15 09:27:20.061947 orq_ai_sdk-2.3.3/orq_ai_sdk/exceptions.py
--rw-r--r--   0        0        0     2075 2024-03-21 12:25:53.696282 orq_ai_sdk-2.3.3/orq_ai_sdk/http_client.py
--rw-r--r--   0        0        0      136 2024-03-15 09:27:20.062170 orq_ai_sdk-2.3.3/orq_ai_sdk/models.py
--rw-r--r--   0        0        0     1399 2024-03-21 12:24:03.900585 orq_ai_sdk-2.3.3/orq_ai_sdk/util.py
--rw-r--r--   0        0        0       18 2024-03-21 12:42:58.529168 orq_ai_sdk-2.3.3/orq_ai_sdk/version.py
--rw-r--r--   0        0        0     1306 2024-03-26 00:37:53.067695 orq_ai_sdk-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     8474 1970-01-01 00:00:00.000000 orq_ai_sdk-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-15 09:27:20.060670 orq_ai_sdk-2.3.4/LICENSE
+-rw-r--r--   0        0        0     7382 2024-03-21 12:42:41.520384 orq_ai_sdk-2.3.4/README.md
+-rw-r--r--   0        0        0       38 2024-03-15 09:27:20.061191 orq_ai_sdk-2.3.4/orq_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:27:20.061230 orq_ai_sdk-2.3.4/orq_ai_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0    14123 2024-03-26 00:32:08.214534 orq_ai_sdk-2.3.4/orq_ai_sdk/api_resources/async_deployments.py
+-rw-r--r--   0        0        0    14144 2024-03-26 00:32:08.257393 orq_ai_sdk-2.3.4/orq_ai_sdk/api_resources/deployments.py
+-rw-r--r--   0        0        0     2739 2024-03-15 09:27:20.061820 orq_ai_sdk-2.3.4/orq_ai_sdk/client.py
+-rw-r--r--   0        0        0     1653 2024-03-15 09:27:20.061947 orq_ai_sdk-2.3.4/orq_ai_sdk/exceptions.py
+-rw-r--r--   0        0        0     2201 2024-04-18 08:51:26.170624 orq_ai_sdk-2.3.4/orq_ai_sdk/http_client.py
+-rw-r--r--   0        0        0      136 2024-03-15 09:27:20.062170 orq_ai_sdk-2.3.4/orq_ai_sdk/models.py
+-rw-r--r--   0        0        0     1399 2024-03-21 12:24:03.900585 orq_ai_sdk-2.3.4/orq_ai_sdk/util.py
+-rw-r--r--   0        0        0       18 2024-04-18 08:55:45.591026 orq_ai_sdk-2.3.4/orq_ai_sdk/version.py
+-rw-r--r--   0        0        0     1306 2024-04-18 08:55:45.584267 orq_ai_sdk-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8474 1970-01-01 00:00:00.000000 orq_ai_sdk-2.3.4/PKG-INFO
```

### Comparing `orq_ai_sdk-2.3.3/LICENSE` & `orq_ai_sdk-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/README.md` & `orq_ai_sdk-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/api_resources/async_deployments.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/api_resources/async_deployments.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/api_resources/deployments.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/api_resources/deployments.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/client.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/exceptions.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/http_client.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 def stream(url: str, api_key: str, body: dict, environment=None):
     headers = build_headers(api_key)
     body = build_body(environment, body)
     headers["Accept"] = "text/event-stream"
     body["stream"] = True
     with httpx.stream("POST", url, json=body, headers=headers, timeout=300) as response:
         for chunk in response.iter_bytes():
-            yield chunk
+            buffer += chunk
+            while b"\n\n" in buffer:
+                event, buffer = buffer.split(b"\n\n", 1)
+                yield event
 
 
 async def post_async(url: str, api_key: str, body: dict, environment=None):
     headers = build_headers(api_key)
     body = build_body(environment, body)
 
     async with httpx.AsyncClient(timeout=300) as client:
```

### Comparing `orq_ai_sdk-2.3.3/orq_ai_sdk/util.py` & `orq_ai_sdk-2.3.4/orq_ai_sdk/util.py`

 * *Files identical despite different names*

### Comparing `orq_ai_sdk-2.3.3/pyproject.toml` & `orq_ai_sdk-2.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orq_ai_sdk"
-version = '2.3.3'
+version = '2.3.4'
 description = "Integrate and operate your products with the power of Large Language Models from a single collaboration platform. Conduct prompt engineering, experimentation, operations and monitoring across models, with full transparency on quality and costs."
 authors = ["orq.ai <support@orq.ai>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `orq_ai_sdk-2.3.3/PKG-INFO` & `orq_ai_sdk-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orq_ai_sdk
-Version: 2.3.3
+Version: 2.3.4
 Summary: Integrate and operate your products with the power of Large Language Models from a single collaboration platform. Conduct prompt engineering, experimentation, operations and monitoring across models, with full transparency on quality and costs.
 Author: orq.ai
 Author-email: support@orq.ai
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: orq_ai_sdk Version: 2.3.3 Summary: Integrate and
+Metadata-Version: 2.1 Name: orq_ai_sdk Version: 2.3.4 Summary: Integrate and
 operate your products with the power of Large Language Models from a single
 collaboration platform. Conduct prompt engineering, experimentation, operations
 and monitoring across models, with full transparency on quality and costs.
 Author: orq.ai Author-email: support@orq.ai Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
```

