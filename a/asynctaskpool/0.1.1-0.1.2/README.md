# Comparing `tmp/asynctaskpool-0.1.1.tar.gz` & `tmp/asynctaskpool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctaskpool-0.1.1.tar", max compression
+gzip compressed data, was "asynctaskpool-0.1.2.tar", max compression
```

## Comparing `asynctaskpool-0.1.1.tar` & `asynctaskpool-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      269 2024-04-17 01:27:05.871060 asynctaskpool-0.1.1/README.md
--rw-r--r--   0        0        0       36 2024-04-17 01:22:02.972148 asynctaskpool-0.1.1/asynctaskpool/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-17 01:22:31.908809 asynctaskpool-0.1.1/asynctaskpool/in_progress_task.py
--rw-r--r--   0        0        0     3963 2024-04-17 01:21:53.207925 asynctaskpool-0.1.1/asynctaskpool/task_pool.py
--rw-r--r--   0        0        0      589 2024-04-17 02:40:47.100693 asynctaskpool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 asynctaskpool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      269 2024-04-17 01:27:05.871060 asynctaskpool-0.1.2/README.md
+-rw-r--r--   0        0        0       36 2024-04-17 01:22:02.972148 asynctaskpool-0.1.2/asynctaskpool/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-17 01:22:31.908809 asynctaskpool-0.1.2/asynctaskpool/in_progress_task.py
+-rw-r--r--   0        0        0     4434 2024-04-18 02:58:21.795855 asynctaskpool-0.1.2/asynctaskpool/task_pool.py
+-rw-r--r--   0        0        0      566 2024-04-18 02:58:42.340541 asynctaskpool-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 asynctaskpool-0.1.2/PKG-INFO
```

### Comparing `asynctaskpool-0.1.1/asynctaskpool/in_progress_task.py` & `asynctaskpool-0.1.2/asynctaskpool/in_progress_task.py`

 * *Files identical despite different names*

### Comparing `asynctaskpool-0.1.1/asynctaskpool/task_pool.py` & `asynctaskpool-0.1.2/asynctaskpool/task_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,25 @@
         self._task_tracker: dict[object, asyncio.Event | T | None] = {}
         self._semaphore = asyncio.Semaphore()
         self._restart_task_if_finished: bool = restart_if_finished
 
     def take_in_precomputed_result_map(self, results: dict[object, T]) -> None:
         self._task_tracker.update(**results)
 
+    async def wait_for_task_to_finish_if_running(self, task_id: str):
+        task_to_wait_for: None | TaskpoolTask = None
+
+        async with self._semaphore:
+            if self._has_task_been_submitted_yet(task_id) and self._is_task_in_progress(task_id):
+                task_to_wait_for = self._get_tracked_task(task_id)
+
+        if task_to_wait_for is not None:
+            # Ignore result, we don't need it
+            await task_to_wait_for.wait_and_get_result()
+
     async def submit_new_task(self, task_id: object, future: Coroutine) -> T | None:
         # Any async item that we need to await is put into this.
         # Then we await it at the end of the function, so we can use exception-safe 'with' block without holding the semaphore too long.
         async_operation_to_wait_for: Coroutine | None = None
 
         async with self._semaphore:
             if self._has_task_been_submitted_yet(task_id):
```

### Comparing `asynctaskpool-0.1.1/pyproject.toml` & `asynctaskpool-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "asynctaskpool"
-version = "0.1.1"
+version = "0.1.2"
 description = "Provides a task pool for asynchronous tasks to be executed only once."
 authors = ["QCanvas <qcanvas@noreply.codeberg.org>"]
 readme = "README.md"
 repository = "https://codeberg.org/QCanvas/AsyncTaskPool"
 keywords = ["async", "taskpool"]
 classifiers = [
     "Framework :: AsyncIO"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
-block-timer = "^0.2.0"
 pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asynctaskpool-0.1.1/PKG-INFO` & `asynctaskpool-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynctaskpool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides a task pool for asynchronous tasks to be executed only once.
 Home-page: https://codeberg.org/QCanvas/AsyncTaskPool
 Keywords: async,taskpool
 Author: QCanvas
 Author-email: qcanvas@noreply.codeberg.org
 Requires-Python: >=3.10
 Classifier: Framework :: AsyncIO
```

