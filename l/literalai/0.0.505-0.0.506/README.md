# Comparing `tmp/literalai-0.0.505.tar.gz` & `tmp/literalai-0.0.506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.505.tar", last modified: Wed Apr 17 09:38:23 2024, max compression
+gzip compressed data, was "literalai-0.0.506.tar", last modified: Thu Apr 18 13:49:20 2024, max compression
```

## Comparing `literalai-0.0.505.tar` & `literalai-0.0.506.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.391110 literalai-0.0.505/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 09:38:13.000000 literalai-0.0.505/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 09:38:23.387110 literalai-0.0.505/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 09:38:13.000000 literalai-0.0.505/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    40395 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-17 09:38:13.000000 literalai-0.0.505/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 09:38:23.000000 literalai-0.0.505/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:38:23.391110 literalai-0.0.505/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 09:38:13.000000 literalai-0.0.505/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:23.387110 literalai-0.0.505/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:38:13.000000 literalai-0.0.505/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 13:49:11.000000 literalai-0.0.506/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 13:49:20.447400 literalai-0.0.506/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 13:49:11.000000 literalai-0.0.506/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.435400 literalai-0.0.506/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.443400 literalai-0.0.506/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    40395 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.443400 literalai-0.0.506/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-18 13:49:11.000000 literalai-0.0.506/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.439400 literalai-0.0.506/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 13:49:20.000000 literalai-0.0.506/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:49:20.447400 literalai-0.0.506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 13:49:11.000000 literalai-0.0.506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:20.447400 literalai-0.0.506/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:49:11.000000 literalai-0.0.506/tests/__init__.py
```

### Comparing `literalai-0.0.505/LICENSE` & `literalai-0.0.506/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/README.md` & `literalai-0.0.506/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/__init__.py` & `literalai-0.0.506/literalai/api/__init__.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/attachment_helpers.py` & `literalai-0.0.506/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/dataset_helpers.py` & `literalai-0.0.506/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/generation_helpers.py` & `literalai-0.0.506/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/gql.py` & `literalai-0.0.506/literalai/api/gql.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/prompt_helpers.py` & `literalai-0.0.506/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/score_helpers.py` & `literalai-0.0.506/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/step_helpers.py` & `literalai-0.0.506/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/thread_helpers.py` & `literalai-0.0.506/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/api/user_helpers.py` & `literalai-0.0.506/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/callback/langchain_callback.py` & `literalai-0.0.506/literalai/callback/langchain_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 from importlib.metadata import version
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, TypedDict, Union
 
-from literalai.context import active_steps_var, active_thread_var
 from literalai.helper import ensure_values_serializable
 from literalai.my_types import ChatGeneration, CompletionGeneration, GenerationMessage
 from literalai.step import Step
 
 if TYPE_CHECKING:
     from uuid import UUID
 
@@ -177,17 +176,14 @@
             GenerationHelper.__init__(self)
 
             self.client = client
             self.steps = {}
             self.parent_id_map = {}
             self.ignored_runs = set()
 
-            self.step_context = active_steps_var.get()
-            self.thread_context = active_thread_var.get()
-
             if to_ignore is None:
                 self.to_ignore = DEFAULT_TO_IGNORE
             else:
                 self.to_ignore = to_ignore
 
             if to_keep is None:
                 self.to_keep = DEFAULT_TO_KEEP
@@ -323,17 +319,14 @@
                     # Tag the run as ignored
                     self.ignored_runs.add(str(run.id))
                 return ignore, parent_id
 
         def _start_trace(self, run: Run) -> None:
             super()._start_trace(run)
 
-            active_thread_var.set(self.thread_context)
-            active_steps_var.set(self.step_context)
-
             ignore, parent_id = self._should_ignore_run(run)
 
             if run.run_type in ["chain", "prompt"]:
                 self.generation_inputs[str(run.id)] = ensure_values_serializable(
                     run.inputs
                 )
```

### Comparing `literalai-0.0.505/literalai/callback/llama_index_callback.py` & `literalai-0.0.506/literalai/callback/llama_index_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,52 +51,37 @@
         ) -> None:
             """Initialize the base callback handler."""
             super().__init__(
                 event_starts_to_ignore=event_starts_to_ignore,
                 event_ends_to_ignore=event_ends_to_ignore,
             )
             self.client = client
-            self.active_steps = active_steps_var.get()
 
             self.steps = {}
 
         def _get_parent_id(
             self, event_parent_id: Optional[str] = None
         ) -> Optional[str]:
+            active_steps = active_steps_var.get()
             if event_parent_id and event_parent_id in self.steps:
                 return event_parent_id
-            elif self.active_steps:
-                return self.active_steps[-1].id
+            elif active_steps:
+                return active_steps[-1].id
             else:
                 return None
 
-        def _restore_context(self) -> None:
-            """Restore Chainlit context in the current thread
-
-            Chainlit context is local to the main thread, and LlamaIndex
-            runs the callbacks in its own threads, so they don't have a
-            Chainlit context by default.
-
-            This method restores the context in which the callback handler
-            has been created (it's always created in the main thread), so
-            that we can actually send messages.
-            """
-            active_steps_var.set(self.active_steps)
-
         def on_event_start(
             self,
             event_type: CBEventType,
             payload: Optional[Dict[str, Any]] = None,
             event_id: str = "",
             parent_id: str = "",
             **kwargs: Any,
         ) -> str:
             """Run when an event starts and return id of event."""
-            self._restore_context()
-
             step_type: TrueStepType = "undefined"
             if event_type == CBEventType.RETRIEVE:
                 step_type = "retrieval"
             elif event_type == CBEventType.QUERY:
                 step_type = "retrieval"
             elif event_type == CBEventType.LLM:
                 step_type = "llm"
@@ -124,16 +109,14 @@
         ) -> None:
             """Run when an event ends."""
             step = self.steps.get(event_id, None)
 
             if payload is None or step is None:
                 return
 
-            self._restore_context()
-
             step.end_time = utc_now()
 
             if event_type == CBEventType.QUERY:
                 response = payload.get(EventPayload.RESPONSE)
                 source_nodes = getattr(response, "source_nodes", None)
                 if source_nodes:
                     step.attachments = []
```

### Comparing `literalai-0.0.505/literalai/client.py` & `literalai-0.0.506/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/dataset.py` & `literalai-0.0.506/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/dataset_experiment.py` & `literalai-0.0.506/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/dataset_item.py` & `literalai-0.0.506/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/event_processor.py` & `literalai-0.0.506/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/filter.py` & `literalai-0.0.506/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/helper.py` & `literalai-0.0.506/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/instrumentation/openai.py` & `literalai-0.0.506/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/message.py` & `literalai-0.0.506/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/my_types.py` & `literalai-0.0.506/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/prompt.py` & `literalai-0.0.506/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/requirements.py` & `literalai-0.0.506/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/step.py` & `literalai-0.0.506/literalai/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             thread_id=self.thread_id,
         )
         return self.step
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             self.step.error = str(exc_val)
-            await self.client.event_processor.flush()
+            await self.client.event_processor.aflush()
         self.step.end()
 
     def __enter__(self) -> Step:
         self.step = self.client.start_step(
             name=self.step_name,
             type=self.step_type,
             id=self.id,
```

### Comparing `literalai-0.0.505/literalai/thread.py` & `literalai-0.0.506/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai/wrappers.py` & `literalai-0.0.506/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.505/literalai.egg-info/SOURCES.txt` & `literalai-0.0.506/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

