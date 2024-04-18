# Comparing `tmp/wkregister-0.0.1.tar.gz` & `tmp/wkregister-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkregister-0.0.1.tar", last modified: Tue Apr 16 17:25:36 2024, max compression
+gzip compressed data, was "wkregister-0.0.2.tar", last modified: Thu Apr 18 17:21:47 2024, max compression
```

## Comparing `wkregister-0.0.1.tar` & `wkregister-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-16 17:25:36.992875 wkregister-0.0.1/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.1/LICENSE
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-16 17:25:36.992656 wkregister-0.0.1/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-16 17:24:17.000000 wkregister-0.0.1/README.md
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-16 17:24:43.000000 wkregister-0.0.1/pyproject.toml
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-16 17:25:36.992920 wkregister-0.0.1/setup.cfg
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-16 17:25:36.990621 wkregister-0.0.1/src/
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-16 17:25:36.990861 wkregister-0.0.1/src/test/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.1/src/test/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      606 2024-04-16 16:55:14.000000 wkregister-0.0.1/src/test/test_logs.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      386 2024-04-16 17:18:54.000000 wkregister-0.0.1/src/test.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-16 17:25:36.991511 wkregister-0.0.1/src/wkregister/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.1/src/wkregister/__init__.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1395 2024-04-16 17:14:44.000000 wkregister-0.0.1/src/wkregister/decorator.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      420 2024-04-16 16:16:25.000000 wkregister-0.0.1/src/wkregister/models.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-16 17:09:58.000000 wkregister-0.0.1/src/wkregister/producer.py
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      686 2024-04-16 17:09:08.000000 wkregister-0.0.1/src/wkregister/util.py
-drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-16 17:25:36.992416 wkregister-0.0.1/src/wkregister.egg-info/
--rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-16 17:25:36.000000 wkregister-0.0.1/src/wkregister.egg-info/PKG-INFO
--rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-16 17:25:36.000000 wkregister-0.0.1/src/wkregister.egg-info/SOURCES.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-16 17:25:36.000000 wkregister-0.0.1/src/wkregister.egg-info/dependency_links.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-16 17:25:36.000000 wkregister-0.0.1/src/wkregister.egg-info/requires.txt
--rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-16 17:25:36.000000 wkregister-0.0.1/src/wkregister.egg-info/top_level.txt
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.603553 wkregister-0.0.2/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1073 2023-11-28 19:55:03.000000 wkregister-0.0.2/LICENSE
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:21:47.603308 wkregister-0.0.2/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3246 2024-04-17 16:54:30.000000 wkregister-0.0.2/README.md
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      539 2024-04-18 17:21:33.000000 wkregister-0.0.2/pyproject.toml
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       38 2024-04-18 17:21:47.603598 wkregister-0.0.2/setup.cfg
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.599502 wkregister-0.0.2/src/
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.599870 wkregister-0.0.2/src/test/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 18:05:55.000000 wkregister-0.0.2/src/test/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      633 2024-04-18 17:20:58.000000 wkregister-0.0.2/src/test/test_logs.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      386 2024-04-16 17:18:54.000000 wkregister-0.0.2/src/test.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.601693 wkregister-0.0.2/src/wkregister/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        0 2024-04-15 16:15:44.000000 wkregister-0.0.2/src/wkregister/__init__.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1849 2024-04-18 17:21:06.000000 wkregister-0.0.2/src/wkregister/decorator.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      420 2024-04-16 16:16:25.000000 wkregister-0.0.2/src/wkregister/models.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     1394 2024-04-16 17:09:58.000000 wkregister-0.0.2/src/wkregister/producer.py
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      690 2024-04-18 17:18:56.000000 wkregister-0.0.2/src/wkregister/util.py
+drwxr-xr-x   0 gustavogordillo   (501) staff       (20)        0 2024-04-18 17:21:47.602987 wkregister-0.0.2/src/wkregister.egg-info/
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)     3722 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/PKG-INFO
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)      406 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)        1 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/requires.txt
+-rw-r--r--   0 gustavogordillo   (501) staff       (20)       16 2024-04-18 17:21:47.000000 wkregister-0.0.2/src/wkregister.egg-info/top_level.txt
```

### Comparing `wkregister-0.0.1/LICENSE` & `wkregister-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.1/PKG-INFO` & `wkregister-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `wkregister-0.0.1/README.md` & `wkregister-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.1/pyproject.toml` & `wkregister-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wkregister"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gustavo", email="gustavo.gordillo.giron@gmail.com" },
 ]
 description = "A wk register library for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wkregister-0.0.1/src/test/test_logs.py` & `wkregister-0.0.2/src/test/test_logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import unittest
 from wkregister.decorator import record  # Import your decorator
 from wkregister.models import Records
+import asyncio
 
 
 @record()
 def add(a: float, b: float):
 
     record = Records(
-        org="commonsense",
-        key="logs",
+        org="nmi",
+        key="commonsense",
         userId="2",
         actionType="update",
         status="success",
         errorMessage=None,
         service="pay-service",
     )
     return {"result": a + b, "record": record}
 
 
 class TestLogs(unittest.TestCase):
 
     def test_log(self):
         # Await the asynchronous method
-        add(12, 12)
+        asyncio.run(add(12, 12))
 
         # Assert your test condition
         self.assertTrue(True)
```

### Comparing `wkregister-0.0.1/src/wkregister/decorator.py` & `wkregister-0.0.2/src/wkregister/decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from wkregister.producer import KafkaProducerWrapper, KafkaMessageSender
 from wkregister.models import Records
 from wkregister.util import kafkaParams
-from typing import Callable, Any
+from typing import Callable, Any, Dict
 from functools import wraps
-import json
+import inspect
 import asyncio
+import json
 import time
 
 
-async def record2Kafka(org: str, key: str, value: str):
+async def record2Kafka(org: str, key: str, value: Dict) -> None:
     producer_wrapper = KafkaProducerWrapper()
     # Crear el enviador de mensajes
     message_sender = KafkaMessageSender(producer_wrapper)
     # Enviar un mensaje
     topic = f"{org}_logs"
     key = f"{key}"
     value = json.dumps(value)
@@ -22,27 +23,41 @@
 
 
 # Decorator for logging
 def record():
     def decorator_log(func: Callable):
         @wraps(func)
         async def wrapper(*args, **kwargs):
-            result = func(*args, **kwargs)
+            input = func(*args, **kwargs)
+
+            if inspect.iscoroutine(input):
+                result = await input
+            else:
+                result = input
 
             org, key, log = kafkaParams(result)
             print(f"log={log.dict()}")
 
             start_time = time.time()  # Capture the start time
 
             # Log after function execution, you can adjust what you log as needed
             asyncio.create_task(record2Kafka(org, key, log.dict()))
 
             end_time = time.time()  # Capture the end time
 
             elapsed_time = end_time - start_time  # Calculate elapsed time
             # print(f"The function took {elapsed_time} seconds to complete.")
 
-            return result
+            output = {}
+            for key, value in result.items():
+                if not key == "record" or not key == "log":
+                    output[key] = value
+                if key == "record" or key == "log":
+                    output[key] = log.dict()
+
+            print(output)
+
+            return output
 
         return wrapper
 
     return decorator_log
```

### Comparing `wkregister-0.0.1/src/wkregister/producer.py` & `wkregister-0.0.2/src/wkregister/producer.py`

 * *Files identical despite different names*

### Comparing `wkregister-0.0.1/src/wkregister/util.py` & `wkregister-0.0.2/src/wkregister/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from wkregister.models import Records
 from typing import Callable, Any
 
 
 def kafkaParams(result: Any):
 
     # Retrieve 'record' or 'log', defaulting to None if neither is found
-    log: Records = result.get("record") or result.get("log")
+    log: Records = (result).get("record") or (result).get("log")
     # Check if 'log' was not retrieved and inform the user
     if not log:
         print("No record/log was set")
 
     # Extract 'org' and 'key' from the log, defaulting to None if not found
     org = log.org
     key = log.key
```

### Comparing `wkregister-0.0.1/src/wkregister.egg-info/PKG-INFO` & `wkregister-0.0.2/src/wkregister.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkregister
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wk register library for python
 Author-email: Gustavo <gustavo.gordillo.giron@gmail.com>
 Project-URL: Homepage, https://github.com/gtavo95/wknmi.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

