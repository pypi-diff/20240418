# Comparing `tmp/minimax_client-0.5.3.tar.gz` & `tmp/minimax_client-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimax_client-0.5.3.tar", last modified: Tue Apr 16 09:13:21 2024, max compression
+gzip compressed data, was "minimax_client-0.5.4.tar", last modified: Thu Apr 18 06:18:53 2024, max compression
```

## Comparing `minimax_client-0.5.3.tar` & `minimax_client-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.3/LICENSE.md
--rw-r--r--   0        0        0    11623 2024-04-16 08:49:13.990564 minimax_client-0.5.3/README.md
--rw-r--r--   0        0        0     2337 2024-04-16 09:13:21.759502 minimax_client-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.3/src/minimax_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-16 09:12:49.636287 minimax_client-0.5.3/src/minimax_client/__version__.py
--rw-r--r--   0        0        0     5995 2024-04-12 06:44:51.187297 minimax_client-0.5.3/src/minimax_client/client.py
--rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.3/src/minimax_client/entities/__init__.py
--rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.3/src/minimax_client/entities/assistant.py
--rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.3/src/minimax_client/entities/chat_completion.py
--rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.3/src/minimax_client/entities/common.py
--rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.3/src/minimax_client/entities/embedding.py
--rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.3/src/minimax_client/entities/file.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.3/src/minimax_client/entities/fine_tuning.py
--rw-r--r--   0        0        0     7233 2024-04-16 09:11:38.581853 minimax_client-0.5.3/src/minimax_client/entities/thread.py
--rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.3/src/minimax_client/interfaces/__init__.py
--rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.3/src/minimax_client/interfaces/assistant.py
--rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.3/src/minimax_client/interfaces/base.py
--rw-r--r--   0        0        0     8832 2024-03-21 09:50:23.229159 minimax_client-0.5.3/src/minimax_client/interfaces/chat_completion.py
--rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.3/src/minimax_client/interfaces/embedding.py
--rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.3/src/minimax_client/interfaces/file.py
--rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.3/src/minimax_client/interfaces/fine_tuning.py
--rw-r--r--   0        0        0    27437 2024-04-16 09:10:10.160861 minimax_client-0.5.3/src/minimax_client/interfaces/thread.py
--rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.3/tests/test_client.py
--rw-r--r--   0        0        0    12592 1970-01-01 00:00:00.000000 minimax_client-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-03-06 04:02:14.299362 minimax_client-0.5.4/LICENSE.md
+-rw-r--r--   0        0        0    12307 2024-04-18 06:12:14.577504 minimax_client-0.5.4/README.md
+-rw-r--r--   0        0        0     2337 2024-04-18 06:18:53.053586 minimax_client-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-13 04:59:39.590202 minimax_client-0.5.4/src/minimax_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-18 06:17:40.850643 minimax_client-0.5.4/src/minimax_client/__version__.py
+-rw-r--r--   0        0        0     5995 2024-04-12 06:44:51.187297 minimax_client-0.5.4/src/minimax_client/client.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:42:19.334547 minimax_client-0.5.4/src/minimax_client/entities/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-12 09:41:25.234703 minimax_client-0.5.4/src/minimax_client/entities/assistant.py
+-rw-r--r--   0        0        0     1431 2024-03-27 06:52:42.426086 minimax_client-0.5.4/src/minimax_client/entities/chat_completion.py
+-rw-r--r--   0        0        0      651 2024-03-26 08:25:32.233150 minimax_client-0.5.4/src/minimax_client/entities/common.py
+-rw-r--r--   0        0        0      288 2024-03-27 06:51:31.873794 minimax_client-0.5.4/src/minimax_client/entities/embedding.py
+-rw-r--r--   0        0        0     1144 2024-03-27 06:50:23.603022 minimax_client-0.5.4/src/minimax_client/entities/file.py
+-rw-r--r--   0        0        0     1956 2024-03-27 09:21:05.226495 minimax_client-0.5.4/src/minimax_client/entities/fine_tuning.py
+-rw-r--r--   0        0        0     8261 2024-04-18 06:04:51.025280 minimax_client-0.5.4/src/minimax_client/entities/thread.py
+-rw-r--r--   0        0        0        0 2024-03-12 08:49:51.948241 minimax_client-0.5.4/src/minimax_client/interfaces/__init__.py
+-rw-r--r--   0        0        0    23479 2024-04-12 05:59:39.461781 minimax_client-0.5.4/src/minimax_client/interfaces/assistant.py
+-rw-r--r--   0        0        0      532 2024-03-15 09:50:38.059327 minimax_client-0.5.4/src/minimax_client/interfaces/base.py
+-rw-r--r--   0        0        0     8842 2024-04-18 06:15:41.712616 minimax_client-0.5.4/src/minimax_client/interfaces/chat_completion.py
+-rw-r--r--   0        0        0     3168 2024-03-21 09:42:08.928420 minimax_client-0.5.4/src/minimax_client/interfaces/embedding.py
+-rw-r--r--   0        0        0     8150 2024-03-27 06:44:53.186708 minimax_client-0.5.4/src/minimax_client/interfaces/file.py
+-rw-r--r--   0        0        0    12362 2024-03-27 07:04:43.648435 minimax_client-0.5.4/src/minimax_client/interfaces/fine_tuning.py
+-rw-r--r--   0        0        0    35334 2024-04-18 06:14:48.411198 minimax_client-0.5.4/src/minimax_client/interfaces/thread.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:45:59.529113 minimax_client-0.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     2412 2024-03-25 11:51:29.057995 minimax_client-0.5.4/tests/test_client.py
+-rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 minimax_client-0.5.4/PKG-INFO
```

### Comparing `minimax_client-0.5.3/LICENSE.md` & `minimax_client-0.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/README.md` & `minimax_client-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 [![License](https://img.shields.io/pypi/l/minimax-client.svg)](https://pypi.org/project/minimax-client)
 [![python-versions](https://img.shields.io/pypi/pyversions/minimax-client.svg)](https://pypi.org/project/minimax-client)
 [![Main Workflow](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml)
 
 An (unofficial) python native client for easy interaction with [MiniMax Open Platform](https://www.minimaxi.com/platform)
 
 The current implementation includes the following official APIs offered by MiniMax:
+
 - ChatCompletion v2
 - Embeddings
 - File
 - Finetune
 - Assistants
-    - Assistant
-    - Assistant File
-    - Thread
-    - Message
-    - Run
+  - Assistant
+  - Assistant File
+  - Thread
+  - Message
+  - Run
+  - Run Step
 
 ## Prerequisites
+
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
 
 ## Quick Start
 
@@ -139,15 +142,14 @@
 
 for chunk in stream:
     print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
 
 # It's currently sunny in Log Angeles, with a temperature of 51°F and wind from the east at 5 mph.
 ```
 
-
 #### 2.4 Async call
 
 ```python
 import asyncio
 
 from minimax_client import AsyncMiniMax
 
@@ -465,7 +467,37 @@
 for step in resp.data:
     resp = client.threads.runs.steps.retrieve(
         step_id=step.id, thread_id=thread_id, run_id=run_id
     )
 
     print(resp.model_dump())
 ```
+
+#### 2.16 Sync call for assistant STREAMED runs and run steps
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.assistants.create(
+    model="abab5.5-chat",
+    name="test-assistant",
+    instructions="You are a helpful assistant.",
+)
+
+assistant_id = resp.id
+
+resp = client.threads.create(metadata={"key1": "value1"})
+
+thread_id = resp.id
+
+for part in client.threads.runs.stream(
+    stream_mode=1,
+    thread_id=thread_id,
+    assistant_id=assistant_id,
+    messages=[{"type": 1, "role": "user", "content": "1 + 1 equals:"}],
+):
+    print(part.data.model_dump())
+    print("\n-----\n")
+```
```

### Comparing `minimax_client-0.5.3/pyproject.toml` & `minimax_client-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.3"
+version = "0.5.4"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=8.1.1,<9",
```

### Comparing `minimax_client-0.5.3/src/minimax_client/client.py` & `minimax_client-0.5.4/src/minimax_client/client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/assistant.py` & `minimax_client-0.5.4/src/minimax_client/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/chat_completion.py` & `minimax_client-0.5.4/src/minimax_client/entities/chat_completion.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/common.py` & `minimax_client-0.5.4/src/minimax_client/entities/common.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/file.py` & `minimax_client-0.5.4/src/minimax_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/fine_tuning.py` & `minimax_client-0.5.4/src/minimax_client/entities/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/entities/thread.py` & `minimax_client-0.5.4/src/minimax_client/entities/thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 from pydantic import BaseModel, HttpUrl, NonNegativeInt
 
 from minimax_client.entities.assistant import AssistantTool
 from minimax_client.entities.chat_completion import ChoiceMessageToolCall
 from minimax_client.entities.common import BareResponse
 
 
+class StreamedRunBaseResp(BaseModel):
+    """Streamed Run Base Resp"""
+
+    code: Optional[NonNegativeInt] = None
+    message: Optional[str] = None
+
+
 class Thread(BaseModel):
     """Thread"""
 
     id: str
     object: Literal["thread"]
     created_at: NonNegativeInt
     metadata: Dict[str, str] = {}
@@ -58,15 +65,15 @@
     web_citation: Optional[MessageTextContentAnnotationWebCitation] = None
 
 
 class MessageTextContent(BaseModel):
     """Message Text Content"""
 
     value: str
-    annotations: List[MessageTextContentAnnotation] = []
+    annotations: Optional[List[MessageTextContentAnnotation]] = None
 
 
 class MessageImageFile(BaseModel):
     """Message Image File"""
 
     file_id: str
 
@@ -108,14 +115,21 @@
 
     object: Literal["list"]
     data: List[Message]
     first_id: str
     last_id: str
 
 
+class StreamedRunMessageResponse(BaseModel):
+    """Streamed Run Message Response"""
+
+    data: Message
+    base_resp: StreamedRunBaseResp
+
+
 class RunError(BaseModel):
     """Run Error"""
 
     code: str
     message: str
 
 
@@ -128,54 +142,80 @@
 class RunRequiredAction(BaseModel):
     """Run Required Action"""
 
     type: Literal["submit_tool_outputs", ""]
     submit_tool_outputs: Optional[RunRequiredActionSubmitToolOutputs] = None
 
 
+class T2AOption(BaseModel):
+    """T2A Option"""
+
+    model: Literal["speech-01"]
+    voice_id: str
+
+
+class StreamedRunT2AControl(BaseModel):
+    """Streamed Run T2A Control"""
+
+    combine: bool
+    model: Literal["speech-01"]
+    oss: str
+    return_bytes: bool
+    text: str
+    timbre_weights: Dict[str, float]
+
+
 class Run(BaseModel):
     """Run"""
 
     id: str
-    object: Literal["thread.run"]
-    created_at: NonNegativeInt
+    object: Literal["thread.run", "run"]
     assistant_id: str
     thread_id: str
     status: Literal[
         "queued",
         "started",
         "in_progress",
         "requires_action",
         "completed",
         "expired",
         "cancelled",
         "failed",
     ]
-    started_at: NonNegativeInt
+    created_at: NonNegativeInt
+    started_at: Optional[NonNegativeInt] = None
     expires_at: Optional[NonNegativeInt] = None
     cancelled_at: Optional[NonNegativeInt] = None
     failed_at: Optional[NonNegativeInt] = None
     completed_at: Optional[NonNegativeInt] = None
     updated_at: Optional[NonNegativeInt] = None
     last_error: Optional[RunError] = None
     model: Literal[
         "abab6-chat",
         "abab5.5-chat",
         "abab5.5-chat-240131",
         "abab5.5s-chat",
         "abab5.5s-chat-240123",
     ]
-    t2a_option: Optional[Dict[str, str]] = None
+    t2a_option: Optional[T2AOption] = None
+    t2a_control: Optional[StreamedRunT2AControl] = None
     instructions: str
     tools: List[AssistantTool] = []
     file_ids: List[str] = []
     metadata: Optional[Dict[str, str]] = None
     required_action: Optional[RunRequiredAction] = None
 
 
+class StreamedRunResponse(BaseModel):
+    """Streamed Run Response"""
+
+    data: Run
+    base_resp: StreamedRunBaseResp
+
+
 class RunCreateResponse(BareResponse, Run):
     """Run Create Response"""
 
 
 class RunRetrieveResponse(BareResponse, Run):
     """Run Retrieve Response"""
 
@@ -266,32 +306,39 @@
     tool_calls: Optional[List[RunStepDetailToolCall]] = None
 
 
 class RunStep(BaseModel):
     """Run Step"""
 
     id: str
-    object: Literal["thread.run.step"]
+    object: Literal["thread.run.step", "run step"]
     run_id: str
     assistant_id: str
     thread_id: str
     type: Literal["message_creation", "tool_calls"]
     status: str
     created_at: NonNegativeInt
     expired_at: Optional[NonNegativeInt] = None
     cancelled_at: Optional[NonNegativeInt] = None
     failed_at: Optional[NonNegativeInt] = None
     completed_at: Optional[NonNegativeInt] = None
     last_error: Optional[RunError] = None
     step_details: RunStepDetail
-    base_resp: Dict
+    base_resp: Optional[Dict] = None
 
 
 class RunStepRetrieveResponse(BareResponse, RunStep):
     """Run Step Retrieve response"""
 
 
 class RunStepListResponse(BareResponse):
     """Run Step List response"""
 
     object: Literal["list"]
     data: List[RunStep]
+
+
+class StreamedRunStepResponse(BaseModel):
+    """Streamed Run Step Response"""
+
+    data: RunStep
+    base_resp: StreamedRunBaseResp
```

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/assistant.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/assistant.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/base.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/chat_completion.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,21 +110,21 @@
         """
         with self.client.stream(
             method="post", url=self.url_path, json=json_body
         ) as resp:
             if resp.status_code != HTTPStatus.OK:
                 raise Exception(f"status: {resp.status_code}; {resp.text}")
 
-            for data in resp.iter_text():
-                json_body = json.loads(data.split("data: ", 2)[1])
+            for data_text in resp.iter_text():
+                data_json = json.loads(data_text.split("data: ", 2)[1])
 
-                yield ChatCompletionResponse(**json_body)
+                yield ChatCompletionResponse(**data_json)
 
                 # If the stream is finished, break out of the loop
-                if "finish_reason" in json_body["choices"][0]:
+                if "finish_reason" in data_json["choices"][0]:
                     break
 
 
 class AsyncChatCompletions(BaseAsyncInterface, ChatCompletions):
     """Asynchronous Chat Completions interface"""
 
     async def create(
```

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/embedding.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/embedding.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/file.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/file.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/fine_tuning.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/src/minimax_client/interfaces/thread.py` & `minimax_client-0.5.4/src/minimax_client/interfaces/thread.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """thread.py"""
 
-from typing import Any, Dict, List, Literal, Optional
+import json
+from typing import Any, AsyncGenerator, Dict, Generator, List, Literal, Optional, Union
 
 import httpx
 
 from minimax_client.entities.thread import (
     MessageCreateResponse,
     MessageListResponse,
     MessageRetrieveResponse,
@@ -12,14 +13,17 @@
     RunCreateResponse,
     RunListResponse,
     RunRetrieveResponse,
     RunStepListResponse,
     RunStepRetrieveResponse,
     RunSubmitToolOutputsResponse,
     RunUpdateResponse,
+    StreamedRunMessageResponse,
+    StreamedRunResponse,
+    StreamedRunStepResponse,
     ThreadCreateResponse,
     ThreadRetrieveResponse,
     ThreadUpdateResponse,
 )
 from minimax_client.interfaces.base import BaseAsyncInterface, BaseSyncInterface
 
 
@@ -357,15 +361,15 @@
                 "abab6-chat",
                 "abab5.5-chat",
                 "abab5.5-chat-240131",
                 "abab5.5s-chat",
                 "abab5.5s-chat-240123",
             ]
         ] = None,
-        tools: Optional[List] = None,
+        tools: Optional[List[Dict[str, Union[str, Dict]]]] = None,
         metadata: Optional[Dict[str, str]] = None,
     ) -> RunCreateResponse:
         """
         Create a non-stream run
 
         Args:
             thread_id (str): The ID of the thread to create the run for
@@ -378,15 +382,15 @@
                         "abab6-chat", "abab5.5-chat", "abab5.5-chat-240131",
                         "abab5.5s-chat", "abab5.5s-chat-240123"
                     ]
                 ],
                 optional
             ):
                 The model to use for the run. Defaults to None.
-            tools (Optional[List], optional):
+            tools (Optional[List[Dict[str, Union[str, Dict]]]], optional):
                 The tools to use for the run. Defaults to None.
             metadata (Optional[Dict[str, str]], optional):
                 The metadata of the run. Defaults to None.
 
         Returns:
             RunCreateResponse: The response from the API
         """
@@ -407,14 +411,116 @@
         if metadata:
             json_body["metadata"] = metadata
 
         resp = self.client.post(url=f"{self.url_path}/create", json=json_body)
 
         return RunCreateResponse(**resp.json())
 
+    def stream(  # noqa: C901
+        self,
+        *,
+        stream_mode: Literal[1, 2],
+        thread_id: str,
+        assistant_id: str,
+        messages: List[Dict[str, Union[int, str, List[str], Dict]]],
+        model: Optional[
+            Literal[
+                "abab6-chat",
+                "abab5.5-chat",
+                "abab5.5-chat-240131",
+                "abab5.5s-chat",
+                "abab5.5s-chat-240123",
+            ]
+        ] = None,
+        t2a_option: Optional[Dict[str, str]] = None,
+        instructions: Optional[str] = None,
+        tools: Optional[List[Dict[str, Union[str, Dict]]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+    ) -> Generator[
+        Union[StreamedRunMessageResponse, StreamedRunStepResponse, StreamedRunResponse],
+        None,
+        None,
+    ]:
+        """
+        Create a stream run
+
+        Args:
+            stream_mode (Literal[1, 2]):
+                The stream mode to use.
+                1 for TEXT_STREAM,
+                2 for TEXT_AND_AUDIO_STREAM (In this mode, the input could be audio)
+            thread_id (str): The ID of the thread to create the run for
+            assistant_id (str): The ID of the assistant to run
+            messages (List[Dict[str, Union[int, str, List[str], Dict]]]):
+                The messages to use for the run
+            model (
+                Optional[
+                    Literal[
+                        "abab6-chat", "abab5.5-chat", "abab5.5-chat-240131",
+                        "abab5.5s-chat", "abab5.5s-chat-240123"
+                    ]
+                ]
+            ):
+                The model to use for the run.
+                If not specified (ie. None), the model of the assistant will be used.
+            t2a_option (Optional[Dict[str, str]], optional):
+                T2A option to use for the run. Defaults to None.
+            instructions (Optional[str], optional):
+                The instructions of the run. Defaults to None.
+            tools (Optional[List[Dict[str, Union[str, Dict]]]], optional):
+                The tools to use for the run. Defaults to None.
+            metadata (Optional[Dict[str, str]], optional):
+                The metadata of the run. Defaults to None.
+
+        Returns:
+            Generator[Union[
+                StreamedRunMessageResponse, StreamedRunStepResponse, StreamedRunResponse
+            ], None, None]: The response from the API
+        """
+        json_body = {
+            "stream": stream_mode,
+            "thread_id": thread_id,
+            "assistant_id": assistant_id,
+            "messages": messages,
+        }
+
+        if model:
+            json_body["model"] = model
+
+        if t2a_option:
+            json_body["t2a_option"] = t2a_option
+
+        if instructions:
+            json_body["instructions"] = instructions
+
+        if tools:
+            json_body["tools"] = tools
+
+        if metadata:
+            json_body["metadata"] = metadata
+
+        with self.client.stream(
+            method="post", url=f"{self.url_path}/create_stream", json=json_body
+        ) as resp:
+            for data_text in resp.iter_text():
+                if not data_text.startswith("data:"):
+                    continue
+
+                data_json = json.loads(data_text.split("data: ", 2)[1])
+
+                if not data_json.get("data"):
+                    continue
+
+                if (object_tag := data_json["data"]["object"]) == "run":
+                    yield StreamedRunResponse(**data_json)
+                elif object_tag == "message":
+                    yield StreamedRunMessageResponse(**data_json)
+                elif object_tag == "run step":
+                    yield StreamedRunStepResponse(**data_json)
+
     def retrieve(self, run_id: str, thread_id: str) -> RunRetrieveResponse:
         """
         Retrieve general info of the given run
 
         Args:
             run_id (str): The ID of the run to retrieve
             thread_id (str): The ID of the thread the run belongs to
@@ -555,15 +661,15 @@
                 "abab6-chat",
                 "abab5.5-chat",
                 "abab5.5-chat-240131",
                 "abab5.5s-chat",
                 "abab5.5s-chat-240123",
             ]
         ] = None,
-        tools: Optional[List] = None,
+        tools: Optional[List[Dict[str, Union[str, Dict]]]] = None,
         metadata: Optional[Dict[str, str]] = None,
     ) -> RunCreateResponse:
         """
         Create a non-stream run
 
         Args:
             thread_id (str): The ID of the thread to create the run for
@@ -576,15 +682,15 @@
                         "abab6-chat", "abab5.5-chat", "abab5.5-chat-240131",
                         "abab5.5s-chat", "abab5.5s-chat-240123"
                     ]
                 ],
                 optional
             ):
                 The model to use for the run. Defaults to None.
-            tools (Optional[List], optional):
+            tools (Optional[List[Dict[str, Union[str, Dict]]]], optional):
                 The tools to use for the run. Defaults to None.
             metadata (Optional[Dict[str, str]], optional):
                 The metadata of the run. Defaults to None.
 
         Returns:
             RunCreateResponse: The response from the API
         """
@@ -605,14 +711,115 @@
         if metadata:
             json_body["metadata"] = metadata
 
         resp = await self.client.post(url=f"{self.url_path}/create", json=json_body)
 
         return RunCreateResponse(**resp.json())
 
+    async def stream(  # noqa: C901
+        self,
+        *,
+        stream_mode: Literal[1, 2],
+        thread_id: str,
+        assistant_id: str,
+        messages: List[Dict[str, Union[int, str, List[str], Dict]]],
+        model: Optional[
+            Literal[
+                "abab6-chat",
+                "abab5.5-chat",
+                "abab5.5-chat-240131",
+                "abab5.5s-chat",
+                "abab5.5s-chat-240123",
+            ]
+        ] = None,
+        t2a_option: Optional[Dict[str, str]] = None,
+        instructions: Optional[str] = None,
+        tools: Optional[List[Dict[str, Union[str, Dict]]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+    ) -> AsyncGenerator[
+        Union[StreamedRunMessageResponse, StreamedRunStepResponse, StreamedRunResponse],
+        None,
+    ]:
+        """
+        Create a stream run
+
+        Args:
+            stream_mode (Literal[1, 2]):
+                The stream mode to use.
+                1 for TEXT_STREAM,
+                2 for TEXT_AND_AUDIO_STREAM (In this mode, the input could be audio)
+            thread_id (str): The ID of the thread to create the run for
+            assistant_id (str): The ID of the assistant to run
+            messages (List[Dict[str, Union[int, str, List[str], Dict]]]):
+                The messages to use for the run
+            model (
+                Optional[
+                    Literal[
+                        "abab6-chat", "abab5.5-chat", "abab5.5-chat-240131",
+                        "abab5.5s-chat", "abab5.5s-chat-240123"
+                    ]
+                ]
+            ):
+                The model to use for the run.
+                If not specified (ie. None), the model of the assistant will be used.
+            t2a_option (Optional[Dict[str, str]], optional):
+                T2A option to use for the run. Defaults to None.
+            instructions (Optional[str], optional):
+                The instructions of the run. Defaults to None.
+            tools (Optional[List[Dict[str, Union[str, Dict]]]], optional):
+                The tools to use for the run. Defaults to None.
+            metadata (Optional[Dict[str, str]], optional):
+                The metadata of the run. Defaults to None.
+
+        Returns:
+            AsyncGenerator[Union[
+                StreamedRunMessageResponse, StreamedRunStepResponse, StreamedRunResponse
+            ], None]: The response from the API
+        """
+        json_body = {
+            "stream": stream_mode,
+            "thread_id": thread_id,
+            "assistant_id": assistant_id,
+            "messages": messages,
+        }
+
+        if model:
+            json_body["model"] = model
+
+        if t2a_option:
+            json_body["t2a_option"] = t2a_option
+
+        if instructions:
+            json_body["instructions"] = instructions
+
+        if tools:
+            json_body["tools"] = tools
+
+        if metadata:
+            json_body["metadata"] = metadata
+
+        async with self.client.stream(
+            method="post", url=f"{self.url_path}/create_stream", json=json_body
+        ) as resp:
+            for data_text in resp.iter_text():
+                if not data_text.startswith("data:"):
+                    continue
+
+                data_json = json.loads(data_text.split("data: ", 2)[1])
+
+                if not data_json.get("data"):
+                    continue
+
+                if (object_tag := data_json["data"]["object"]) == "run":
+                    yield StreamedRunResponse(**data_json)
+                elif object_tag == "message":
+                    yield StreamedRunMessageResponse(**data_json)
+                elif object_tag == "run step":
+                    yield StreamedRunStepResponse(**data_json)
+
     async def retrieve(self, run_id: str, thread_id: str) -> RunRetrieveResponse:
         """
         Retrieve general info of the given run
 
         Args:
             run_id (str): The ID of the run to retrieve
             thread_id (str): The ID of the thread the run belongs to
```

### Comparing `minimax_client-0.5.3/tests/test_client.py` & `minimax_client-0.5.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `minimax_client-0.5.3/PKG-INFO` & `minimax_client-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimax-client
-Version: 0.5.3
+Version: 0.5.4
 Summary: An (unofficial) python native client for easy interaction with MiniMax Open Platform
 Keywords: web,api,llm
 Author-Email: Zeyang Lin <4020306+linzeyang@users.noreply.github.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -41,26 +41,29 @@
 [![License](https://img.shields.io/pypi/l/minimax-client.svg)](https://pypi.org/project/minimax-client)
 [![python-versions](https://img.shields.io/pypi/pyversions/minimax-client.svg)](https://pypi.org/project/minimax-client)
 [![Main Workflow](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/linzeyang/minimax-python-client/actions/workflows/main.yml)
 
 An (unofficial) python native client for easy interaction with [MiniMax Open Platform](https://www.minimaxi.com/platform)
 
 The current implementation includes the following official APIs offered by MiniMax:
+
 - ChatCompletion v2
 - Embeddings
 - File
 - Finetune
 - Assistants
-    - Assistant
-    - Assistant File
-    - Thread
-    - Message
-    - Run
+  - Assistant
+  - Assistant File
+  - Thread
+  - Message
+  - Run
+  - Run Step
 
 ## Prerequisites
+
 - Python >= 3.8
 - pip (or any other tool that does the same job)
 - Internet connection
 - An API KEY acquired from [MiniMax Open Platform](https://www.minimaxi.com/user-center/basic-information/interface-key)
 
 ## Quick Start
 
@@ -173,15 +176,14 @@
 
 for chunk in stream:
     print(chunk.choices[0].delta.content if chunk.choices[0].delta else "", end="")
 
 # It's currently sunny in Log Angeles, with a temperature of 51°F and wind from the east at 5 mph.
 ```
 
-
 #### 2.4 Async call
 
 ```python
 import asyncio
 
 from minimax_client import AsyncMiniMax
 
@@ -499,7 +501,37 @@
 for step in resp.data:
     resp = client.threads.runs.steps.retrieve(
         step_id=step.id, thread_id=thread_id, run_id=run_id
     )
 
     print(resp.model_dump())
 ```
+
+#### 2.16 Sync call for assistant STREAMED runs and run steps
+
+```python
+from minimax_client import MiniMax
+
+
+client = MiniMax(api_key="<YOUR_API_KEY>")
+
+resp = client.assistants.create(
+    model="abab5.5-chat",
+    name="test-assistant",
+    instructions="You are a helpful assistant.",
+)
+
+assistant_id = resp.id
+
+resp = client.threads.create(metadata={"key1": "value1"})
+
+thread_id = resp.id
+
+for part in client.threads.runs.stream(
+    stream_mode=1,
+    thread_id=thread_id,
+    assistant_id=assistant_id,
+    messages=[{"type": 1, "role": "user", "content": "1 + 1 equals:"}],
+):
+    print(part.data.model_dump())
+    print("\n-----\n")
+```
```

