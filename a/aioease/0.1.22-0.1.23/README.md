# Comparing `tmp/aioease-0.1.22-py3-none-any.whl.zip` & `tmp/aioease-0.1.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3674 bytes, number of entries: 7
+Zip file size: 3909 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       25 b- defN 24-Apr-11 19:27 aioease/__init__.py
--rw-rw-rw-  2.0 fat     3119 b- defN 24-Apr-11 20:29 aioease/main.py
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-11 20:48 aioease-0.1.22.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1399 b- defN 24-Apr-11 20:48 aioease-0.1.22.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 20:48 aioease-0.1.22.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-11 20:48 aioease-0.1.22.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      536 b- defN 24-Apr-11 20:48 aioease-0.1.22.dist-info/RECORD
-7 files, 6251 bytes uncompressed, 2724 bytes compressed:  56.4%
+-rw-rw-rw-  2.0 fat     3169 b- defN 24-Apr-18 15:18 aioease/main.py
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1962 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      536 b- defN 24-Apr-18 17:01 aioease-0.1.23.dist-info/RECORD
+7 files, 6864 bytes uncompressed, 2959 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: aioease/__init__.py
 Comment: 
 
 Filename: aioease/main.py
 Comment: 
 
-Filename: aioease-0.1.22.dist-info/LICENSE
+Filename: aioease-0.1.23.dist-info/LICENSE
 Comment: 
 
-Filename: aioease-0.1.22.dist-info/METADATA
+Filename: aioease-0.1.23.dist-info/METADATA
 Comment: 
 
-Filename: aioease-0.1.22.dist-info/WHEEL
+Filename: aioease-0.1.23.dist-info/WHEEL
 Comment: 
 
-Filename: aioease-0.1.22.dist-info/top_level.txt
+Filename: aioease-0.1.23.dist-info/top_level.txt
 Comment: 
 
-Filename: aioease-0.1.22.dist-info/RECORD
+Filename: aioease-0.1.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioease/main.py

```diff
@@ -32,15 +32,15 @@
 
         async with self.limiter:
             try:
                 async with method(**request) as resp:
                     response = await resp.text()
                     # Debug-level log of the response details
                     logger.debug(f"Received response {resp.status} from {url}")
-                    return {"status": resp.status, "response": response}
+                    return {"status": resp.status, "response": response, "request": request}
             except Exception as e:
                 # Error-level log if an exception occurs
                 logger.error(f"Error making request to {url}: {e}")
                 return {"status": "error", "response": str(e)}
 
     async def _main(self, requests: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         """
@@ -63,16 +63,16 @@
         """
         logger.info(
             f"AsyncRequest instance created with a rate limit of {requests_per_second_max} requests per second.")
         self.limiter = AsyncLimiter(requests_per_second_max, 1)
         logger.info(f"Executing {len(requests)} request(s) asynchronously.")
         return asyncio.run(self._main(requests))
 
-def execute(requests: List[Dict[str, Any]], requests_per_second_max: int = 1) -> List[Dict[str, Any]]:
+def execute_async_requests(requests: List[Dict[str, Any]], requests_per_second_max: int = 1) -> List[Dict[str, Any]]:
     """
-    Execute multiple HTTP requests asynchronously.
+    Execute_async_requests multiple HTTP requests asynchronously.
 
     :param requests: A list of request details.
     :param requests_per_second_max: Maximum number of requests per second.
     :return: A list of responses.
     """
     return AIOEase().execute(requests, requests_per_second_max)
```

## Comparing `aioease-0.1.22.dist-info/LICENSE` & `aioease-0.1.23.dist-info/LICENSE`

 * *Files identical despite different names*

