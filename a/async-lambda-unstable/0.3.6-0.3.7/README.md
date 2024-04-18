# Comparing `tmp/async-lambda-unstable-0.3.6.tar.gz` & `tmp/async-lambda-unstable-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lambda-unstable-0.3.6.tar", last modified: Wed Apr  3 15:46:53 2024, max compression
+gzip compressed data, was "async-lambda-unstable-0.3.7.tar", last modified: Thu Apr 18 15:37:21 2024, max compression
```

## Comparing `async-lambda-unstable-0.3.6.tar` & `async-lambda-unstable-0.3.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.174629 async-lambda-unstable-0.3.6/
--rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-04-03 15:46:53.174422 async-lambda-unstable-0.3.6/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)    14286 2024-03-25 20:21:32.000000 async-lambda-unstable-0.3.6/README.md
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.170789 async-lambda-unstable-0.3.6/async_lambda/
--rw-r--r--   0 henryjones   (501) staff       (20)      692 2024-04-03 15:45:53.000000 async-lambda-unstable-0.3.6/async_lambda/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-03-25 20:13:13.000000 async-lambda-unstable-0.3.6/async_lambda/build_config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-04-03 15:45:25.000000 async-lambda-unstable-0.3.6/async_lambda/cli.py
--rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/client.py
--rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    19117 2024-03-25 20:51:58.000000 async-lambda-unstable-0.3.6/async_lambda/controller.py
--rw-r--r--   0 henryjones   (501) staff       (20)      723 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/env.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.171303 async-lambda-unstable-0.3.6/async_lambda/models/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/__init__.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.172856 async-lambda-unstable-0.3.6/async_lambda/models/events/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/api_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/base_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/managed_sqs_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/scheduled_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/events/unmanaged_sqs_event.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.173267 async-lambda-unstable-0.3.6/async_lambda/models/mock/
--rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_context.py
--rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)    17705 2024-04-03 15:42:11.000000 async-lambda-unstable-0.3.6/async_lambda/models/task.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.6/async_lambda/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-03-27 19:59:17.000000 async-lambda-unstable-0.3.6/async_lambda/util.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-03 15:46:53.174259 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)    14546 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      910 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       48 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-04-03 15:46:53.000000 async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/top_level.txt
--rw-r--r--   0 henryjones   (501) staff       (20)      821 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.6/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-04-03 15:46:53.174682 async-lambda-unstable-0.3.6/setup.cfg
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.799222 async-lambda-unstable-0.3.7/
+-rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-18 15:37:21.798939 async-lambda-unstable-0.3.7/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)    15541 2024-04-18 15:16:55.000000 async-lambda-unstable-0.3.7/README.md
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.794582 async-lambda-unstable-0.3.7/async_lambda/
+-rw-r--r--   0 henryjones   (501) staff       (20)      726 2024-04-18 12:29:21.000000 async-lambda-unstable-0.3.7/async_lambda/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.7/async_lambda/build_config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.7/async_lambda/cli.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.7/async_lambda/client.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    19117 2024-04-18 15:06:27.000000 async-lambda-unstable-0.3.7/async_lambda/controller.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1176 2024-04-18 12:28:57.000000 async-lambda-unstable-0.3.7/async_lambda/defer.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      809 2024-04-18 10:34:41.000000 async-lambda-unstable-0.3.7/async_lambda/env.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.794953 async-lambda-unstable-0.3.7/async_lambda/models/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/__init__.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.796773 async-lambda-unstable-0.3.7/async_lambda/models/events/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/api_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/base_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/managed_sqs_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/scheduled_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/events/unmanaged_sqs_event.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.797316 async-lambda-unstable-0.3.7/async_lambda/models/mock/
+-rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/models/mock/mock_context.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.7/async_lambda/models/mock/mock_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    18748 2024-04-18 14:49:06.000000 async-lambda-unstable-0.3.7/async_lambda/models/task.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.7/async_lambda/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.7/async_lambda/util.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-18 15:37:21.798735 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      932 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       48 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-04-18 15:37:21.000000 async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/top_level.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)      821 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.7/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-04-18 15:37:21.799283 async-lambda-unstable-0.3.7/setup.cfg
```

### Comparing `async-lambda-unstable-0.3.6/PKG-INFO` & `async-lambda-unstable-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: async-lambda-unstable
-Version: 0.3.6
-Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
-Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
-Description-Content-Type: text/markdown
-Provides-Extra: local
-
 # async-lambda
 
 `async-lambda` is a framework for creating `AWS Lambda` applications with built
 in support for asynchronous invocation via a SQS Queue. This is useful if you
 have workloads you need to split up into separate execution contexts.
 
 `async-lambda` converts your application into a `Serverless Application Model (SAM)`
@@ -45,14 +37,47 @@
 All task decorators share common arguments for configuring the underlying lambda function:
 
 - `memory: int = 128` Sets the memory allocation for the function.
 - `timeout: int = 60` Sets the timeout for the function (max 900 seconds).
 - `ephemeral_storage: int = 512` Sets the ephemeral storage allocation for the function.
 - `maximum_concurrency: Optional[int | List[int]] = None` Sets the maximum concurrency value for the SQS trigger for the function. (only applies to `async_task` and `sqs_task` tasks.) When using the `lanes` feature, this can be a list of maximum concurrency for each lane. The length of the list must equal the # of lanes.
 
+It is often useful to run code during the `INIT_START` phase of the lambda lifecycle.
+This is achieved by placing that code outside of the lambda handler, this will
+result in this code being run for all tasks within the application as it is
+executed on import. `async-lambda` provides a utility `init_tasks` argument which
+will run given functions during the `INIT_START` phase only for that specific task.
+
+The functions should have either 0 or 1 arguments, if they have 1 argument then
+the `task_id` will be passed in.
+
+`async-lambda` also provides a helper class for when a value needs to be stored
+from this execution. The `Defer` class takes a function, and args/kwargs and
+will only execute the function when its value is requested. This can be used in
+combination with `init_tasks` to cache values during the `INIT_START` phase.
+
+EX:
+
+```python
+
+def get_a_value(a: int, b: int) -> int:
+    return random.randint(a, b)
+
+cache = Defer(get_a_value, 10, 100)
+
+@controller.async_task("Task", init_tasks=[cache.execute])
+def task(event: ManagedSQSEvent):
+    for i in range(cache.value):
+        # Do Something
+        ...
+```
+
+For all lambda executions which share a container `cache.value` will be the same
+and `get_a_value` will only be called once.
+
 ## Async Task
 
 All async tasks have a matching SQS queue which the lambda function consumes from (1 message per invocation).
 All async task queues share a DLQ. Async tasks can be invoked from anywhere within the app by using the
 `AsyncLambdaController.async_invoke` method. Calling this method sends a message into the queue for the given task.
 The task function should have a single parameter of the `ManagedSQSEvent` type.
```

### Comparing `async-lambda-unstable-0.3.6/README.md` & `async-lambda-unstable-0.3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: async-lambda-unstable
+Version: 0.3.7
+Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
+Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
+Description-Content-Type: text/markdown
+Provides-Extra: local
+
 # async-lambda
 
 `async-lambda` is a framework for creating `AWS Lambda` applications with built
 in support for asynchronous invocation via a SQS Queue. This is useful if you
 have workloads you need to split up into separate execution contexts.
 
 `async-lambda` converts your application into a `Serverless Application Model (SAM)`
@@ -37,14 +45,47 @@
 All task decorators share common arguments for configuring the underlying lambda function:
 
 - `memory: int = 128` Sets the memory allocation for the function.
 - `timeout: int = 60` Sets the timeout for the function (max 900 seconds).
 - `ephemeral_storage: int = 512` Sets the ephemeral storage allocation for the function.
 - `maximum_concurrency: Optional[int | List[int]] = None` Sets the maximum concurrency value for the SQS trigger for the function. (only applies to `async_task` and `sqs_task` tasks.) When using the `lanes` feature, this can be a list of maximum concurrency for each lane. The length of the list must equal the # of lanes.
 
+It is often useful to run code during the `INIT_START` phase of the lambda lifecycle.
+This is achieved by placing that code outside of the lambda handler, this will
+result in this code being run for all tasks within the application as it is
+executed on import. `async-lambda` provides a utility `init_tasks` argument which
+will run given functions during the `INIT_START` phase only for that specific task.
+
+The functions should have either 0 or 1 arguments, if they have 1 argument then
+the `task_id` will be passed in.
+
+`async-lambda` also provides a helper class for when a value needs to be stored
+from this execution. The `Defer` class takes a function, and args/kwargs and
+will only execute the function when its value is requested. This can be used in
+combination with `init_tasks` to cache values during the `INIT_START` phase.
+
+EX:
+
+```python
+
+def get_a_value(a: int, b: int) -> int:
+    return random.randint(a, b)
+
+cache = Defer(get_a_value, 10, 100)
+
+@controller.async_task("Task", init_tasks=[cache.execute])
+def task(event: ManagedSQSEvent):
+    for i in range(cache.value):
+        # Do Something
+        ...
+```
+
+For all lambda executions which share a container `cache.value` will be the same
+and `get_a_value` will only be called once.
+
 ## Async Task
 
 All async tasks have a matching SQS queue which the lambda function consumes from (1 message per invocation).
 All async task queues share a DLQ. Async tasks can be invoked from anywhere within the app by using the
 `AsyncLambdaController.async_invoke` method. Calling this method sends a message into the queue for the given task.
 The task function should have a single parameter of the `ManagedSQSEvent` type.
```

### Comparing `async-lambda-unstable-0.3.6/async_lambda/__init__.py` & `async-lambda-unstable-0.3.7/async_lambda/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .config import config_set_name as config_set_name
 from .config import config_set_runtime as config_set_runtime
 from .controller import AsyncLambdaController as AsyncLambdaController
+from .defer import Defer as Defer
 from .env import disable_force_sync_mode as disable_force_sync_mode
 from .env import enable_force_sync_mode as enable_force_sync_mode
 from .env import is_build_mode as is_build_mode
 from .models.events.api_event import APIEvent as APIEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent as ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent as ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent as UnmanagedSQSEvent
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

### Comparing `async-lambda-unstable-0.3.6/async_lambda/build_config.py` & `async-lambda-unstable-0.3.7/async_lambda/build_config.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/cli.py` & `async-lambda-unstable-0.3.7/async_lambda/cli.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/client.py` & `async-lambda-unstable-0.3.7/async_lambda/client.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/controller.py` & `async-lambda-unstable-0.3.7/async_lambda/controller.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/events/api_event.py` & `async-lambda-unstable-0.3.7/async_lambda/models/events/api_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/events/base_event.py` & `async-lambda-unstable-0.3.7/async_lambda/models/events/base_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/events/managed_sqs_event.py` & `async-lambda-unstable-0.3.7/async_lambda/models/events/managed_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/events/unmanaged_sqs_event.py` & `async-lambda-unstable-0.3.7/async_lambda/models/events/unmanaged_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/mock/mock_event.py` & `async-lambda-unstable-0.3.7/async_lambda/models/mock/mock_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda/models/task.py` & `async-lambda-unstable-0.3.7/async_lambda/models/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import json
 import re
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Generic, List, Optional, TypeVar, Union
 
 from async_lambda.util import make_cf_tags
 
@@ -35,39 +36,49 @@
     trigger_type: TaskTriggerType
     trigger_config: dict
 
     timeout: int
     memory: int
     ephemeral_storage: int
     maximum_concurrency: Optional[Union[int, List[int]]]
+    init_tasks: List[Union[Callable[[str], Any], Callable[[], Any]]]
+    _has_run_init_tasks: bool
 
     executable: Callable[[EventType], Any]
 
     def __init__(
         self,
         controller: "AsyncLambdaController",
         executable: Callable[[EventType], Any],
         task_id: str,
         trigger_type: TaskTriggerType,
         trigger_config: Optional[dict] = None,
         timeout: int = 60,
         memory: int = 128,
         ephemeral_storage: int = 512,
         maximum_concurrency: Optional[Union[int, List[int]]] = None,
+        init_tasks: Optional[
+            List[Union[Callable[[str], Any], Callable[[], Any]]]
+        ] = None,
     ):
         AsyncLambdaTask.validate_task_id(task_id)
         self.controller = controller
         self.executable = executable
         self.task_id = task_id
         self.trigger_type = trigger_type
         self.trigger_config = trigger_config if trigger_config is not None else dict()
         self.timeout = timeout
         self.memory = memory
         self.ephemeral_storage = ephemeral_storage
         self.maximum_concurrency = maximum_concurrency
+        if init_tasks is None:
+            self.init_tasks = []
+        else:
+            self.init_tasks = init_tasks
+        self._has_run_init_tasks = False
 
         if (
             self.trigger_type == TaskTriggerType.MANAGED_SQS
             and "dlq_task_id" in self.trigger_config
         ):
             dlq_task_id = self.trigger_config["dlq_task_id"]
             if dlq_task_id:
@@ -76,14 +87,29 @@
                     raise Exception(
                         f"Error setting DLQ Task ID: No task with the task_id {dlq_task_id} exists."
                     )
                 if dlq_task.trigger_type != TaskTriggerType.MANAGED_SQS:
                     raise Exception(
                         f"Error setting DLQ Task ID: Task {dlq_task_id} is not an async-task."
                     )
+        if env.is_cloud() and env.get_current_task_id() == self.task_id:
+            self._run_init_tasks()
+
+    def _run_init_tasks(self):
+        if self._has_run_init_tasks:
+            return
+        for _init_task in self.init_tasks:
+            if len(inspect.signature(_init_task).parameters) == 0:
+                _init_task()  # type: ignore
+            elif len(inspect.signature(_init_task).parameters) == 1:
+                _init_task(self.task_id)  # type: ignore
+            else:
+                raise Exception(f"The init task {_init_task} has an invalid signature.")
+
+        self._has_run_init_tasks = True
 
     @staticmethod
     def validate_task_id(task_id: str):
         if not task_id.isalnum():
             raise ValueError("Task ID must contain only A-Za-z0-9")
         if len(task_id) > 32:
             raise ValueError("Task ID must be less than 32 characters long.")
@@ -435,8 +461,9 @@
             return self.controller.get_task(self.trigger_config["dlq_task_id"])
         return self.controller.get_dlq_task()
 
     def execute(self, event: EventType) -> Any:
         """
         Executes the tasks function
         """
+        self._run_init_tasks()
         return self.executable(event)
```

### Comparing `async-lambda-unstable-0.3.6/async_lambda/util.py` & `async-lambda-unstable-0.3.7/async_lambda/util.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/PKG-INFO` & `async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.3.6
+Version: 0.3.7
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
 
@@ -45,14 +45,47 @@
 All task decorators share common arguments for configuring the underlying lambda function:
 
 - `memory: int = 128` Sets the memory allocation for the function.
 - `timeout: int = 60` Sets the timeout for the function (max 900 seconds).
 - `ephemeral_storage: int = 512` Sets the ephemeral storage allocation for the function.
 - `maximum_concurrency: Optional[int | List[int]] = None` Sets the maximum concurrency value for the SQS trigger for the function. (only applies to `async_task` and `sqs_task` tasks.) When using the `lanes` feature, this can be a list of maximum concurrency for each lane. The length of the list must equal the # of lanes.
 
+It is often useful to run code during the `INIT_START` phase of the lambda lifecycle.
+This is achieved by placing that code outside of the lambda handler, this will
+result in this code being run for all tasks within the application as it is
+executed on import. `async-lambda` provides a utility `init_tasks` argument which
+will run given functions during the `INIT_START` phase only for that specific task.
+
+The functions should have either 0 or 1 arguments, if they have 1 argument then
+the `task_id` will be passed in.
+
+`async-lambda` also provides a helper class for when a value needs to be stored
+from this execution. The `Defer` class takes a function, and args/kwargs and
+will only execute the function when its value is requested. This can be used in
+combination with `init_tasks` to cache values during the `INIT_START` phase.
+
+EX:
+
+```python
+
+def get_a_value(a: int, b: int) -> int:
+    return random.randint(a, b)
+
+cache = Defer(get_a_value, 10, 100)
+
+@controller.async_task("Task", init_tasks=[cache.execute])
+def task(event: ManagedSQSEvent):
+    for i in range(cache.value):
+        # Do Something
+        ...
+```
+
+For all lambda executions which share a container `cache.value` will be the same
+and `get_a_value` will only be called once.
+
 ## Async Task
 
 All async tasks have a matching SQS queue which the lambda function consumes from (1 message per invocation).
 All async task queues share a DLQ. Async tasks can be invoked from anywhere within the app by using the
 `AsyncLambdaController.async_invoke` method. Calling this method sends a message into the queue for the given task.
 The task function should have a single parameter of the `ManagedSQSEvent` type.
```

### Comparing `async-lambda-unstable-0.3.6/async_lambda_unstable.egg-info/SOURCES.txt` & `async-lambda-unstable-0.3.7/async_lambda_unstable.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 async_lambda/__init__.py
 async_lambda/build_config.py
 async_lambda/cli.py
 async_lambda/client.py
 async_lambda/config.py
 async_lambda/controller.py
+async_lambda/defer.py
 async_lambda/env.py
 async_lambda/py.typed
 async_lambda/util.py
 async_lambda/models/__init__.py
 async_lambda/models/task.py
 async_lambda/models/events/__init__.py
 async_lambda/models/events/api_event.py
```

### Comparing `async-lambda-unstable-0.3.6/pyproject.toml` & `async-lambda-unstable-0.3.7/pyproject.toml`

 * *Files identical despite different names*

