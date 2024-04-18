# Comparing `tmp/thinkcol_llm_client-0.1.1.tar.gz` & `tmp/thinkcol_llm_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkcol_llm_client-0.1.1.tar", max compression
+gzip compressed data, was "thinkcol_llm_client-0.1.2.tar", max compression
```

## Comparing `thinkcol_llm_client-0.1.1.tar` & `thinkcol_llm_client-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      588 2024-03-27 03:21:52.969866 thinkcol_llm_client-0.1.1/README.md
--rw-r--r--   0        0        0      586 2024-03-27 04:50:06.800791 thinkcol_llm_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      134 2024-03-27 04:30:13.486172 thinkcol_llm_client-0.1.1/thinkcol_llm_client/__init__.py
--rw-r--r--   0        0        0      891 2024-03-27 04:09:01.301069 thinkcol_llm_client-0.1.1/thinkcol_llm_client/chat_client.py
--rw-r--r--   0        0        0     4348 2024-03-27 04:14:54.241051 thinkcol_llm_client-0.1.1/thinkcol_llm_client/clients/bedrock_client.py
--rw-r--r--   0        0        0     2991 2024-03-27 04:01:03.369578 thinkcol_llm_client-0.1.1/thinkcol_llm_client/clients/openai_client.py
--rw-r--r--   0        0        0      420 2024-03-25 03:20:48.259124 thinkcol_llm_client-0.1.1/thinkcol_llm_client/constants.py
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 thinkcol_llm_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      590 2024-04-18 06:47:47.305968 thinkcol_llm_client-0.1.2/README.md
+-rw-r--r--   0        0        0      586 2024-04-18 08:24:17.501008 thinkcol_llm_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-04-18 04:33:44.460350 thinkcol_llm_client-0.1.2/thinkcol_llm_client/__init__.py
+-rw-r--r--   0        0        0     2397 2024-04-18 05:29:06.750834 thinkcol_llm_client-0.1.2/thinkcol_llm_client/bedrock/bedrock_models.py
+-rw-r--r--   0        0        0     5521 2024-04-18 06:35:35.760369 thinkcol_llm_client-0.1.2/thinkcol_llm_client/bedrock/clients.py
+-rw-r--r--   0        0        0      666 2024-04-18 05:16:21.950699 thinkcol_llm_client-0.1.2/thinkcol_llm_client/bedrock/payloads.py
+-rw-r--r--   0        0        0     1154 2024-04-18 06:39:20.342081 thinkcol_llm_client-0.1.2/thinkcol_llm_client/chat_client.py
+-rw-r--r--   0        0        0      420 2024-04-15 06:41:39.867967 thinkcol_llm_client-0.1.2/thinkcol_llm_client/constants.py
+-rw-r--r--   0        0        0     3024 2024-04-18 06:39:28.119900 thinkcol_llm_client-0.1.2/thinkcol_llm_client/openai_client.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 thinkcol_llm_client-0.1.2/PKG-INFO
```

### Comparing `thinkcol_llm_client-0.1.1/README.md` & `thinkcol_llm_client-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # LLM Client 
-Internal package for making calls to LLMs.
+Internal package for making multi-threaded calls to LLMs.
+
+# Supported Models
+Cohere Command, Cohere Embed, OpenAI Models, Titan Embed, Mixtral
 
 ## Install
 ```
 pip install thinkcol_llm_client
 ```
 
 ## Usage: 
 ### Normal Usage
 ```
-import asyncio
-from clients.openai_client import OpenAIClient
+from thinkcol_llm_client import OpenAIClient, AnthropicClient
 
 texts = ["Hello", "Text 1", "ThinkCol"]
 
 client = OpenAIClient()
-asyncio.run(client.embed(texts))
+client.embed(texts)
 
 questions = ["How do I implement best practices in data science projects" for _ in range(500)]
-asyncio.run(client.invoke(questions))
-```
+client.invoke(questions)
 
-### Jupyter Notebook
-
-An event loop is created and run automatically by Jupyter. Replace asyncio.run with await.
+anthropic_client = AnthropicClient()
+anthropic_client.invoke(questions)
 ```
-await client.embed(texts)
-```
+
```

### Comparing `thinkcol_llm_client-0.1.1/pyproject.toml` & `thinkcol_llm_client-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkcol_llm_client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Package for calling llm clients asynchronously"
 authors = ["jedric01 <jedric@connect.ust.hk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 openai = "^1.14.2"
```

### Comparing `thinkcol_llm_client-0.1.1/thinkcol_llm_client/chat_client.py` & `thinkcol_llm_client-0.1.2/thinkcol_llm_client/chat_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from abc import ABC, abstractmethod
 from typing import Iterable
+import asyncio
 
 
 class ChatClient(ABC):
 
+    def __init__(self) -> None:
+        super().__init__()
+        # set event loop
+        try:
+            self.loop = asyncio.get_running_loop()
+        except Exception:
+            self.loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(self.loop)
+
     @abstractmethod
     def invoke(self, msgs: list, model_name: str, batch_size: int):
         pass
 
     @abstractmethod
-    def embed(
-        self, texts: list, model_name: str, batch_size: int, texts_per_request: int
-    ):
+    def embed(self, texts: list, model_name: str, batch_size: int):
         pass
 
     # helper generator for chunking iterables into {chunk_size}-sized chunks
     def _chunk(
         self, iter: Iterable, chunk_size: int = 50, transform_fn=lambda x: x, **args
     ):
         chunk: list = []
         while True:
-            el = next(iter, None)
+            el = next(iter, None)  # type: ignore
             # check if iterator is empty
             if el is None:
                 if chunk:
                     yield chunk
                 break
             chunk.append(transform_fn(el, **args))
             if len(chunk) == chunk_size:
```

### Comparing `thinkcol_llm_client-0.1.1/thinkcol_llm_client/clients/openai_client.py` & `thinkcol_llm_client-0.1.2/thinkcol_llm_client/openai_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 from openai import AsyncAzureOpenAI
 import asyncio
-from tqdm.asyncio import tqdm
-from ..chat_client import ChatClient
-from typing import Iterable, AsyncGenerator
+from tqdm import tqdm
+from .chat_client import ChatClient
+from typing import Iterable, Generator
 from dotenv import load_dotenv
 from math import ceil
-from ..constants import OPENAI_SYSTEM_PROMPT
+from .constants import OPENAI_SYSTEM_PROMPT
 
 
 class OpenAIClient(ChatClient):
 
     def __init__(self):
+        super().__init__()
         load_dotenv()
         self.client = AsyncAzureOpenAI(api_version="2023-09-01-preview")
 
-    async def batch_invoke(
-        self, msgs: Iterable, model_name: str, batch_size: int = 50
-    ) -> AsyncGenerator:
+    def batch_invoke(
+        self, msgs: Iterable, model_name: str = "gpt-4", batch_size: int = 50
+    ) -> Generator:
         for chunk in self._chunk(msgs, batch_size):
             coros = [
                 self.client.chat.completions.create(
                     model=model_name,
                     messages=[
                         {"role": "system", "content": OPENAI_SYSTEM_PROMPT},
                         {"role": "user", "content": msg},
                     ],
                     temperature=0,
                 )
                 for msg in chunk
             ]
+
             yield [
                 completion.choices[0].message.content
-                for completion in await asyncio.gather(*coros)
+                for completion in self.loop.run_until_complete(asyncio.gather(*coros))
             ]
 
-    async def batch_embed(
+    def batch_embed(
         self,
         texts: Iterable,
         model_name: str = "text-embedding-ada-002",
         batch_size: int = 50,
         texts_per_request: int = 50,
-    ):
+    ) -> Generator:
         # split text into {batch_size}-size batches, i.e. {batch_size} number of texts per request
         splits = self._chunk(texts, texts_per_request)
         # further split batches into {batch_size}-size superbatches, i.e. {batch_size} number of requests fired
         for chunk in self._chunk(splits, batch_size):
             coros = [
                 self.client.embeddings.create(input=texts, model=model_name)
                 for texts in chunk
             ]
             yield [
                 d.embedding
-                for response in await asyncio.gather(*coros)
+                for response in self.loop.run_until_complete(asyncio.gather(*coros))
                 for d in response.data
             ]
 
     # wrapper for acummulating results from batch_invoke
-    async def invoke(
+    def invoke(
         self, msgs: list[str], model_name: str = "gpt-4", batch_size: int = 50
-    ):
+    ) -> list:
         return [
-            completion
-            async for completion_batch in tqdm(
+            res
+            for batch_res in tqdm(
                 self.batch_invoke(iter(msgs), model_name, batch_size),
                 total=ceil(len(msgs) / batch_size),
             )
-            for completion in completion_batch
+            for res in batch_res
         ]
 
     # wrapper for acummulating results from batch_embed
-    async def embed(
+    def embed(
         self,
         texts: list,
         model_name: str = "text-embedding-ada-002",
         batch_size: int = 50,
         texts_per_request: int = 50,
-    ):
+    ) -> list:
         return [
             embed
-            async for embed_batch in tqdm(
+            for embed_batch in tqdm(
                 self.batch_embed(
                     iter(texts), model_name, batch_size, texts_per_request
                 ),
-                total=ceil(len(texts) / batch_size * texts_per_request),
+                total=ceil(len(texts) / (batch_size * texts_per_request)),
             )
             for embed in embed_batch
         ]
```

### Comparing `thinkcol_llm_client-0.1.1/PKG-INFO` & `thinkcol_llm_client-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: thinkcol_llm_client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package for calling llm clients asynchronously
 Author: jedric01
 Author-email: jedric@connect.ust.hk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.68,<2.0.0)
 Requires-Dist: openai (>=1.14.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # LLM Client 
-Internal package for making calls to LLMs.
+Internal package for making multi-threaded calls to LLMs.
+
+# Supported Models
+Cohere Command, Cohere Embed, OpenAI Models, Titan Embed, Mixtral
 
 ## Install
 ```
 pip install thinkcol_llm_client
 ```
 
 ## Usage: 
 ### Normal Usage
 ```
-import asyncio
-from clients.openai_client import OpenAIClient
+from thinkcol_llm_client import OpenAIClient, AnthropicClient
 
 texts = ["Hello", "Text 1", "ThinkCol"]
 
 client = OpenAIClient()
-asyncio.run(client.embed(texts))
+client.embed(texts)
 
 questions = ["How do I implement best practices in data science projects" for _ in range(500)]
-asyncio.run(client.invoke(questions))
+client.invoke(questions)
+
+anthropic_client = AnthropicClient()
+anthropic_client.invoke(questions)
 ```
 
-### Jupyter Notebook
 
-An event loop is created and run automatically by Jupyter. Replace asyncio.run with await.
-```
-await client.embed(texts)
-```
```

