# Comparing `tmp/aioease-0.1.23-py3-none-any.whl.zip` & `tmp/aioease-0.1.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3909 bytes, number of entries: 7
+Zip file size: 4007 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 24-Apr-11 19:27 aioease/__init__.py
--rw-rw-rw-  2.0 fat     3169 b- defN 24-Apr-18 15:18 aioease/main.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1962 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      536 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/RECORD
-7 files, 6864 bytes uncompressed, 2959 bytes compressed:  56.9%
+-rw-rw-rw-  2.0 fat     3330 b- defN 24-Apr-18 20:34 aioease/main.py
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-18 20:35 aioease-0.1.24.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-18 20:35 aioease-0.1.24.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 20:35 aioease-0.1.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-18 20:35 aioease-0.1.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 24-Apr-18 20:35 aioease-0.1.24.dist-info/RECORD
+7 files, 7839 bytes uncompressed, 3057 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: aioease/__init__.py
 Comment: 
 
 Filename: aioease/main.py
 Comment: 
 
-Filename: aioease-0.1.23.dist-info/LICENSE
+Filename: aioease-0.1.24.dist-info/LICENSE
 Comment: 
 
-Filename: aioease-0.1.23.dist-info/METADATA
+Filename: aioease-0.1.24.dist-info/METADATA
 Comment: 
 
-Filename: aioease-0.1.23.dist-info/WHEEL
+Filename: aioease-0.1.24.dist-info/WHEEL
 Comment: 
 
-Filename: aioease-0.1.23.dist-info/top_level.txt
+Filename: aioease-0.1.24.dist-info/top_level.txt
 Comment: 
 
-Filename: aioease-0.1.23.dist-info/RECORD
+Filename: aioease-0.1.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioease/main.py

```diff
@@ -22,25 +22,29 @@
             "get": session.get,
             "post": session.post,
             "put": session.put,
             "delete": session.delete,
         }
         method = methods.get(request["method"].lower(), session.get)
         url = request["url"]
+        id = request.get("id", None)
         # Debug-level log of the request details
         logger.debug(f"Sending {request['method'].upper()} request to {url}")
         del request["method"]
 
         async with self.limiter:
             try:
                 async with method(**request) as resp:
                     response = await resp.text()
                     # Debug-level log of the response details
                     logger.debug(f"Received response {resp.status} from {url}")
-                    return {"status": resp.status, "response": response, "request": request}
+                    if id:
+                        return {"status": resp.status, "response": response, "id": id}
+                    else:
+                        return {"status": resp.status, "response": response}
             except Exception as e:
                 # Error-level log if an exception occurs
                 logger.error(f"Error making request to {url}: {e}")
                 return {"status": "error", "response": str(e)}
 
     async def _main(self, requests: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         """
```

## Comparing `aioease-0.1.23.dist-info/LICENSE` & `aioease-0.1.24.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aioease-0.1.23.dist-info/METADATA` & `aioease-0.1.24.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioease
-Version: 0.1.23
+Version: 0.1.24
 Summary: A simple and easy way to use asyncio & aiohttp libraries.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp >=3
 Requires-Dist: aiolimiter >=1
 
 # AIOEase
@@ -26,30 +26,57 @@
 from aioease import execute_async_requests
 
 requests = [
     {"url": "https://httpbin.org/ip", "method": "get", "data": {"key": "value"}, "headers": {"header": "value"}},
     {"url": "https://httpbin.org/ip", "method": "post", "data": {"key": "value"}, "headers": {"header": "value"}},
 ]
 
-responses = execute_async_requests(requests,requests_per_second_max=10)
+responses = execute_async_requests(requests, requests_per_second_max=10)
 ```
 
 Returns:
 
 ```python
 responses = [
   {
     "status": 200,
     "response": "{\n  \"origin\": \"00.000.00.000\"\n}\n",
-    "request": {"url": "https://httpbin.org/ip", "method": "get",}
   },
   {
     "status": 405,
     "response": "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 3.2 Final//EN\">\n<title>405 Method Not Allowed</title>\n<h1>Method Not Allowed</h1>\n<p>The method is not allowed for the requested URL.</p>\n",
-    "request": {"url": "https://httpbin.org/ip", "method": "post",}
+  }
+]
+```
+## Given a unique identifyer to match requests to the responses.
+
+```python
+from aioease import execute_async_requests
+
+requests = [
+    {"url": "https://httpbin.org/ip", "method": "get", "data": {"key": "value"}, "headers": {"header": "value"},"id": "unique-identifyer-1"},
+    {"url": "https://httpbin.org/ip", "method": "post", "data": {"key": "value"}, "headers": {"header": "value"},"id": "unique-identifyer-2"},
+]
+
+responses = execute_async_requests(requests, requests_per_second_max=10)
+```
+
+Returns:
+
+```python
+responses = [
+  {
+    "status": 200,
+    "response": "{\n  \"origin\": \"00.000.00.000\"\n}\n",
+    "id": "unique-identifyer-1"
+  },
+  {
+    "status": 405,
+    "response": "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 3.2 Final//EN\">\n<title>405 Method Not Allowed</title>\n<h1>Method Not Allowed</h1>\n<p>The method is not allowed for the requested URL.</p>\n",
+    "id": "unique-identifyer-2"
   }
 ]
 ```
 
 ## Configuring Logging
 
 Control the verbosity of logs for debugging:
```

