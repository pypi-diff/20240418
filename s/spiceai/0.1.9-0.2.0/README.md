# Comparing `tmp/spiceai-0.1.9.tar.gz` & `tmp/spiceai-0.2.0.tar.gz`

## Comparing `spiceai-0.1.9.tar` & `spiceai-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 spiceai-0.1.9/tags
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.1.9/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.1.9/.ropeproject/globalnames
--rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.1.9/.ropeproject/history
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 spiceai-0.1.9/scripts/run.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/errors.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/models.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/providers.py
--rw-r--r--   0        0        0    18856 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/spice.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/spice_message.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/utils.py
--rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 spiceai-0.1.9/spice/wrapped_clients.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.1.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.1.9/LICENSE
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 spiceai-0.1.9/README.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 spiceai-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 spiceai-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.2.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.2.0/scripts/prompt.txt
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.2.0/scripts/run.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/errors.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/models.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/providers.py
+-rw-r--r--   0        0        0    28247 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/spice_message.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/utils.py
+-rw-r--r--   0        0        0    18407 2020-02-02 00:00:00.000000 spiceai-0.2.0/spice/wrapped_clients.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.2.0/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 spiceai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 spiceai-0.2.0/PKG-INFO
```

### Comparing `spiceai-0.1.9/.github/workflows/ruff.yml` & `spiceai-0.2.0/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.9/scripts/run.py` & `spiceai-0.2.0/scripts/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import os
 import sys
-from typing import Dict, List
+from typing import List
 
 # Modify sys.path to ensure the script can run even when it's not part of the installed library.
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 from spice import Spice
 from spice.spice_message import SpiceMessage
 
@@ -22,16 +22,20 @@
     print(response.text)
 
 
 async def streaming_example():
     # You can set a default model for the client instead of passing it with each call
     client = Spice(default_text_model="claude-3-opus-20240229")
 
+    # You can easily load prompts from files, directories, or even urls.
+    client.load_prompt("scripts/prompt.txt", name="my prompt")
+
+    # Spice can also automatically render Jinja templates.
     messages: List[SpiceMessage] = [
-        {"role": "system", "content": "You are a helpful assistant."},
+        {"role": "system", "content": client.get_rendered_prompt("my prompt", assistant_name="Ryan Reynolds")},
         {"role": "user", "content": "list 5 random words"},
     ]
     stream = await client.stream_response(messages=messages)
 
     async for text in stream:
         print(text, end="", flush=True)
     # Retrieve the complete response from the stream
@@ -100,34 +104,56 @@
     print(response.text)
 
     # Creating the model automatically registers it in Spice's model list, so listing the provider is no longer needed
     response = await client.get_response(messages=messages, model="first-gpt35")
     print(response.text)
 
 
+async def vision_example():
+    client = Spice()
+
+    # Spice makes it easy to add images from files or the internet
+    from spice import SpiceMessage, SpiceMessages
+    from spice.models import CLAUDE_3_OPUS_20240229, GPT_4_1106_VISION_PREVIEW
+    from spice.spice_message import file_image_message, user_message
+
+    messages: List[SpiceMessage] = [user_message("What do you see?"), file_image_message("~/.mentat/picture.png")]
+    response = await client.get_response(messages, GPT_4_1106_VISION_PREVIEW)
+    print(response.text)
+
+    # Alternatively, you can use the SpiceMessages wrapper to easily create your prompts
+    spice_messages: SpiceMessages = SpiceMessages(client)
+    spice_messages.add_user_message("What do you see?")
+    spice_messages.add_file_image_message("~/.mentat/picture.png")
+    response = await client.get_response(spice_messages, CLAUDE_3_OPUS_20240229)
+    print(response.text)
+
+
 async def embeddings_and_transcription_example():
     client = Spice()
     input_texts = ["Once upon a time...", "Cinderella"]
 
     # Spice can easily fetch embeddings and audio transcriptions
     from spice.models import TEXT_EMBEDDING_ADA_002, WHISPER_1
 
     embeddings = await client.get_embeddings(input_texts, TEXT_EMBEDDING_ADA_002)
     transcription = await client.get_transcription("~/.mentat/logs/audio/talk_transcription.wav", WHISPER_1)
-    print(transcription)
+    print(transcription.text)
 
 
 async def run_all_examples():
-    print("Running Azure example:")
-    await azure_example()
     print("Running basic example:")
     await basic_example()
     print("\n\nRunning streaming example:")
     await streaming_example()
     print("\n\nRunning multiple providers example:")
     await multiple_providers_example()
+    print("Running Azure example:")
+    await azure_example()
+    print("\n\nRunning vision example:")
+    await vision_example()
     print("\n\nRunning embeddings and transcription example:")
     await embeddings_and_transcription_example()
 
 
 if __name__ == "__main__":
     asyncio.run(run_all_examples())
```

### Comparing `spiceai-0.1.9/spice/providers.py` & `spiceai-0.2.0/spice/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return cache[0]
 
     key = os.getenv("AZURE_OPENAI_KEY")
     endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
     if key is None:
         raise NoAPIKeyError("AZURE_OPENAI_KEY not set")
     if endpoint is None:
-        raise SpiceError("AZURE_OPENAI_ENDPOINT not set")
+        raise NoAPIKeyError("AZURE_OPENAI_ENDPOINT not set")
 
     client = WrappedAzureClient(key, endpoint)
     cache.append(client)
     return client
 
 
 def get_anthropic_client(cache=[]):
```

### Comparing `spiceai-0.1.9/spice/spice.py` & `spiceai-0.2.0/spice/spice.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from __future__ import annotations
 
+import dataclasses
+import glob
+import json
 from dataclasses import dataclass
+from datetime import datetime
+from json import JSONDecodeError
 from pathlib import Path
 from timeit import default_timer as timer
-from typing import AsyncIterator, Callable, Dict, List, Literal, Optional, Sequence, cast
+from typing import Any, AsyncIterator, Callable, Collection, Dict, List, Optional, cast
 
-from spice.errors import InvalidModelError
+import httpx
+from jinja2 import Environment
+from openai.types.chat.completion_create_params import ResponseFormat
+
+from spice.errors import InvalidModelError, UnknownModelError
 from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
-from spice.spice_message import SpiceMessage
+from spice.spice_message import MessagesEncoder, SpiceMessage, SpiceMessages
 from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
-ResponseFormat = Dict[str, Literal["text", "json_object"]]
-
 
 @dataclass
 class SpiceCallArgs:
     model: str
-    messages: List[SpiceMessage]
+    messages: Collection[SpiceMessage]
     stream: bool = False
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
     response_format: Optional[ResponseFormat] = None
 
 
 @dataclass
@@ -70,28 +77,27 @@
 
     def __init__(
         self,
         model: TextModel,
         call_args: SpiceCallArgs,
         client: WrappedClient,
         stream: AsyncIterator,
-        cost_callback: Callable[[float], None],
+        callback: Callable[[SpiceResponse], None],
     ):
         self._model = model
         self._call_args = call_args
         self._text = []
         self._start_time = timer()
         self._end_time = None
         self._input_tokens = None
         self._output_tokens = None
         self._finished = False
         self._client = client
         self._stream = stream
-        self._cost_added = 0
-        self._cost_callback = cost_callback
+        self._callback = callback
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         with self._client.catch_and_convert_errors():
             try:
@@ -124,61 +130,92 @@
         if input_tokens is None:
             input_tokens = self._client.count_messages_tokens(self._call_args.messages, self._model)
         output_tokens = self._output_tokens
         if output_tokens is None:
             output_tokens = self._client.count_string_tokens(full_output, self._model, full_message=False)
 
         cost = text_request_cost(self._model, input_tokens, output_tokens)
-        if cost is not None:
-            new_cost = cost - self._cost_added
-            self._cost_added = cost
-            self._cost_callback(new_cost)
-
-        return SpiceResponse(
+        response = SpiceResponse(
             self._call_args,
             full_output,
             self._end_time - self._start_time,
             input_tokens,
             output_tokens,
             self._finished,
             cost,
         )
+        self._callback(response)
+
+        return response
 
     async def complete_response(self) -> SpiceResponse:
         """
         Waits until the entire LLM call finishes, collects it, and returns its SpiceResponse.
         """
         async for _ in self:
             pass
         return self.current_response()
 
 
+@dataclass
+class EmbeddingResponse:
+    embeddings: List[List[float]]
+    """The list of embeddings of the list of input texts."""
+
+    total_time: float
+    """How long it took for the response to be completed."""
+
+    input_tokens: int
+    """The number of input tokens given in this response."""
+
+    cost: Optional[float]
+    """The cost of this request in cents. Will be None if the cost of the model used is not known."""
+
+
+@dataclass
+class TranscriptionResponse:
+    text: str
+    """The transcription of the input audio."""
+
+    total_time: float
+    """How long it took for the response to be completed."""
+
+    input_length: float
+    """The length of the input audio in seconds."""
+
+    cost: Optional[float]
+    """The cost of this request in cents. Will be None if the cost of the model used is not known."""
+
+
 class Spice:
     """
     The Spice client. The majority of the time, only one Spice client should be initialized and used.
     Automatically handles multiple providers and their respective errors.
     """
 
     def __init__(
         self,
         default_text_model: Optional[TextModel | str] = None,
         default_embeddings_model: Optional[EmbeddingModel | str] = None,
         model_aliases: Optional[Dict[str, Model | str]] = None,
+        logging_dir: Optional[Path | str] = None,
     ):
         """
         Creates a new Spice client.
 
         Args:
             default_text_model: The default model that will be used for chat completions if no other model is given.
             Will raise an InvalidModelError if the model is not a text model.
 
             default_embeddings_model: The default model that will be used for embeddings if no other model is given.
             Will raise an InvalidModelError if the model is not an embeddings model.
 
             model_aliases: A custom model name map.
+
+            logging_dir: If not None, will log all api calls to the given directory.
         """
 
         if isinstance(default_text_model, str):
             text_model = get_model_from_name(default_text_model)
         else:
             text_model = default_text_model
         if text_model and not isinstance(text_model, TextModel):
@@ -193,14 +230,22 @@
             raise InvalidModelError("Default embeddings model must be an embeddings model")
         self._default_embeddings_model = embeddings_model
 
         # TODO: Should we validate model aliases?
         self._model_aliases = model_aliases
 
         self._total_cost: float = 0
+        self._prompts: Dict[str, str] = {}
+
+        if logging_dir is not None:
+            logging_dir = Path(logging_dir).expanduser().resolve()
+            timestamp = datetime.now().strftime("%m%d%y_%H%M%S")
+            self._log_file = logging_dir / f"spice_{timestamp}.json"
+        else:
+            self._log_file = None
 
     @property
     def total_cost(self) -> float:
         """The total cost in cents of all api calls made through this Spice client."""
         return self._total_cost
 
     def load_provider(self, provider: Provider | str):
@@ -216,17 +261,26 @@
     def _get_client(self, model: Model, provider: Optional[Provider | str]) -> WrappedClient:
         if provider is not None:
             if isinstance(provider, str):
                 provider = get_provider_from_name(provider)
             return provider.get_client()
         else:
             if model.provider is None:
-                raise InvalidModelError("Provider is required when unknown models are used")
+                raise UnknownModelError("Provider is required when unknown models are used")
             return model.provider.get_client()
 
+    def _get_model(self, model: Model | str) -> Model:
+        if self._model_aliases is not None and model in self._model_aliases:
+            model = self._model_aliases[model]
+
+        if isinstance(model, str):
+            model = get_model_from_name(model)
+
+        return model
+
     def _get_text_model(self, model: Optional[Model | str]) -> TextModel:
         if model is None:
             if self._default_text_model is None:
                 raise InvalidModelError("Model is required when default text model is not set at initialization")
             model = self._default_text_model
 
         if self._model_aliases is not None and model in self._model_aliases:
@@ -238,15 +292,15 @@
         if not isinstance(model, TextModel):
             raise InvalidModelError(f"Model {model} is not a text model")
 
         return model
 
     def _fix_call_args(
         self,
-        messages: List[SpiceMessage],
+        messages: Collection[SpiceMessage],
         model: Model,
         stream: bool,
         temperature: Optional[float],
         max_tokens: Optional[int],
         response_format: Optional[ResponseFormat],
     ):
         # Not all providers support response format
@@ -259,32 +313,43 @@
             messages=messages,
             stream=stream,
             temperature=temperature,
             max_tokens=max_tokens,
             response_format=response_format,
         )
 
+    def _log_response(self, response: SpiceResponse):
+        if self._log_file is not None:
+            response_json = json.dumps(dataclasses.asdict(response), cls=MessagesEncoder)
+
+            # TODO: This unfortunately isn't a valid json file (since it has multiple objects) but it's the easiest way to keep all requests from one client together
+            with self._log_file.open("a") as file:
+                file.write(response_json)
+                file.write("\n")
+
     async def get_response(
         self,
-        messages: List[SpiceMessage],
+        messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
     ) -> SpiceResponse:
         """
         Asynchronously retrieves a chat completion response.
 
         Args:
             messages: The list of messages given as context for the completion.
+            Will raise an ImageError if any invalid images are given.
 
             model: The model to use. Must be a text based model. If no model is given, will use the default text model
             the client was initialized with. If the model is unknown to Spice, a provider must be given.
-            Will raise an InvalidModelError if the model is not a text model, or if the model is unknown and no provider was given.
+            Will raise an InvalidModelError if the model is not a text model.
+            Will raise an UnknownModelError if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
 
             temperature: The temperature to give the model.
 
             max_tokens: The maximum tokens the model can output.
 
@@ -303,34 +368,37 @@
         text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
 
         cost = text_request_cost(text_model, input_tokens, output_tokens)
         if cost is not None:
             self._total_cost += cost
 
         response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
+        self._log_response(response)
         return response
 
     async def stream_response(
         self,
-        messages: List[SpiceMessage],
+        messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
     ) -> StreamingSpiceResponse:
         """
         Asynchronously retrieves a chat completion stream that can be iterated over asynchronously.
 
         Args:
             messages: The list of messages given as context for the completion.
+            Will raise an ImageError if any invalid images are given.
 
             model: The model to use. Must be a text based model. If no model is given, will use the default text model
             the client was initialized with. If the model is unknown to Spice, a provider must be given.
-            Will raise an InvalidModelError if the model is not a text model, or if the model is unknown and no provider was given.
+            Will raise an InvalidModelError if the model is not a text model.
+            Will raise an UnknownModelError if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
 
             temperature: The temperature to give the model.
 
             max_tokens: The maximum tokens the model can output.
 
@@ -342,18 +410,21 @@
         client = self._get_client(text_model, provider)
         call_args = self._fix_call_args(messages, text_model, True, temperature, max_tokens, response_format)
 
         with client.catch_and_convert_errors():
             stream = await client.get_chat_completion_or_stream(call_args)
         stream = cast(AsyncIterator, stream)
 
-        def cost_callback(cost):
-            self._total_cost += cost
+        def callback(response: SpiceResponse, cache: List[float] = [0]):
+            if response.cost is not None:
+                self._total_cost += response.cost - cache[0]
+                cache[0] = response.cost
+            self._log_response(response)
 
-        return StreamingSpiceResponse(text_model, call_args, client, stream, cost_callback)
+        return StreamingSpiceResponse(text_model, call_args, client, stream, callback)
 
     def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel:
         if model is None:
             if self._default_embeddings_model is None:
                 raise InvalidModelError("Model is required when default embeddings model is not set at initialization")
             model = self._default_embeddings_model
 
@@ -369,66 +440,76 @@
         return model
 
     async def get_embeddings(
         self,
         input_texts: List[str],
         model: Optional[EmbeddingModel | str] = None,
         provider: Optional[Provider | str] = None,
-    ) -> Sequence[Sequence[float]]:
+    ) -> EmbeddingResponse:
         """
         Asynchronously retrieves embeddings for a list of text.
 
         Args:
             input_texts: The texts to generate embeddings for.
 
             model: The embedding model to use. If no model is given, will use the default embedding model
             the client was initialized with. If the model is unknown to Spice, a provider must be given.
-            Will raise an InvalidModelError if the model is not a embedding model, or if the model is unknown and no provider was given.
+            Will raise an InvalidModelError if the model is not a embedding model.
+            Will raise an UnknownModelError if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
         embedding_model = self._get_embedding_model(model)
         client = self._get_client(embedding_model, provider)
 
         input_tokens = sum(client.count_string_tokens(text, embedding_model, False) for text in input_texts)
         cost = embeddings_request_cost(embedding_model, input_tokens)
         if cost is not None:
             self._total_cost += cost
 
-        return await client.get_embeddings(input_texts, embedding_model.name)
+        start_time = timer()
+        embeddings = await client.get_embeddings(input_texts, embedding_model.name)
+        end_time = timer()
+
+        return EmbeddingResponse(embeddings, end_time - start_time, input_tokens, cost)
 
     def get_embeddings_sync(
         self,
         input_texts: List[str],
         model: Optional[EmbeddingModel | str] = None,
         provider: Optional[Provider | str] = None,
-    ) -> Sequence[Sequence[float]]:
+    ) -> EmbeddingResponse:
         """
         Synchronously retrieves embeddings for a list of text.
 
         Args:
             input_texts: The texts to generate embeddings for.
 
             model: The embedding model to use. If no model is given, will use the default embedding model
             the client was initialized with. If the model is unknown to Spice, a provider must be given.
-            Will raise an InvalidModelError if the model is not a embedding model, or if the model is unknown and no provider was given.
+            Will raise an InvalidModelError if the model is not a embedding model.
+            Will raise an UnknownModelError if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
         embedding_model = self._get_embedding_model(model)
         client = self._get_client(embedding_model, provider)
 
         input_tokens = sum(client.count_string_tokens(text, embedding_model, False) for text in input_texts)
         cost = embeddings_request_cost(embedding_model, input_tokens)
         if cost is not None:
             self._total_cost += cost
 
-        return client.get_embeddings_sync(input_texts, embedding_model.name)
+        start_time = timer()
+        embeddings = client.get_embeddings_sync(input_texts, embedding_model.name)
+        end_time = timer()
+
+        return EmbeddingResponse(embeddings, end_time - start_time, input_tokens, cost)
 
     def _get_transcription_model(self, model: Model | str) -> TranscriptionModel:
         if self._model_aliases is not None and model in self._model_aliases:
             model = self._model_aliases[model]
 
         if isinstance(model, str):
             model = get_model_from_name(model)
@@ -439,31 +520,208 @@
         return model
 
     async def get_transcription(
         self,
         audio_path: Path | str,
         model: TranscriptionModel | str,
         provider: Optional[Provider | str] = None,
-    ) -> str:
+    ) -> TranscriptionResponse:
         """
         Asynchronously retrieves embeddings for a list of text.
 
         Args:
             audio_path: The path to the audio file to transcribe.
 
             model: The model to use. Must be a transciption model. If the model is unknown to Spice, a provider must be given.
-            Will raise an InvalidModelError if the model is not a transciption model, or if the model is unknown and no provider was given.
+            Will raise an InvalidModelError if the model is not a transciption model.
+            Will raise an UnknownModelError if the model is unknown and no provider was given.
 
             provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
         """
 
         transcription_model = self._get_transcription_model(model)
         client = self._get_client(transcription_model, provider)
 
+        start_time = timer()
         transcription, input_length = await client.get_transcription(
             Path(audio_path).expanduser().resolve(), transcription_model.name
         )
+        end_time = timer()
+
         cost = transcription_request_cost(transcription_model, input_length)
         if cost is not None:
             self._total_cost += cost
 
-        return transcription
+        return TranscriptionResponse(transcription, end_time - start_time, input_length, cost)
+
+    def count_tokens(
+        self, text: str, model: Model | str, provider: Optional[Provider | str] = None, is_message: bool = False
+    ) -> int:
+        """
+        Calculates the tokens in the given text. Will not be accurate for a chat completion prompt.
+        Use count_prompt_tokens to get the exact amount of tokens for a prompt.
+
+        Args:
+            text: The text to count the tokens of.
+
+            model: The model whose tokenizer will be used. Will raise UnknownModelError if the model is unknown and no provider is given.
+
+            provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
+
+            is_message: If true, will include the extra tokens that messages in chat completions add on. Most of the time, you'll want to keep this false.
+        """
+
+        model = self._get_model(model)
+        client = self._get_client(model, provider)
+
+        return client.count_string_tokens(text, model, is_message)
+
+    def count_prompt_tokens(
+        self, messages: Collection[SpiceMessage], model: Model | str, provider: Optional[Provider | str] = None
+    ) -> int:
+        """
+        Calculates the tokens that the messages would have if used in a chat completion.
+
+        Args:
+            messages: The messages to count the tokens of.
+
+            model: The model whose tokenizer will be used. Will raise UnknownModelError if the model is unknown and no provider is given.
+
+            provider: The provider to use. If specified, will override the model's default provider if known. Must be specified if an unknown model is used.
+        """
+
+        model = self._get_model(model)
+        client = self._get_client(model, provider)
+
+        return client.count_messages_tokens(messages, model)
+
+    ### Prompts ###
+
+    def store_prompt(self, prompt: str, name: str):
+        """
+        Stores a prompt under the given name
+
+        Args:
+            prompt: The prompt to store.
+
+            name: The name of the prompt. If the name collides with the name of a previously loaded prompt, the previous prompt will be overwritten.
+        """
+
+        if name in self._prompts:
+            # Overwriting prompt; should we do anything?
+            pass
+        self._prompts[name] = prompt
+
+    def get_prompt(self, name: str) -> str:
+        """
+        Gets the prompt currently mapped to the given name.
+
+        Args:
+            name: The name of the prompt.
+        """
+
+        return self._prompts[name]
+
+    def get_rendered_prompt(self, name: str, **context: Any) -> str:
+        """
+        Gets the prompt currently mapped to the given name and renders it using jinja.
+
+        Args:
+            name: The name of the prompt.
+
+            context: The jinja kwargs to render the prompt with.
+        """
+        return Environment().from_string(self._prompts[name]).render(context)
+
+    def load_prompt(self, file_path: Path | str, name: Optional[str] = None):
+        """
+        Loads a prompt from the given file.
+
+        Args:
+            file_path: The path to the file. Must be a text encoded file.
+
+            name: The name of the prompt. If no name is given, the name will be the file name without the extension; i.e., the name of /path/to/prompt.txt will be `prompt`.
+            If the name collides with the name of a previously loaded prompt, the previous prompt will be overwritten.
+        """
+
+        file_path = Path(file_path).expanduser().resolve()
+
+        try:
+            prompt = file_path.read_text()
+        except (UnicodeDecodeError, FileNotFoundError):
+            raise
+
+        if name is None:
+            name = file_path.name.rsplit(".", 1)[0]
+
+        self.store_prompt(prompt, name)
+
+    def load_dir(self, dir_path: Path | str):
+        """
+        Loads a prompts from a given directory. Will recursively load all text encoded .txt files in the directory and its subdirectories.
+        Prompt names will be the filenames with their .txt extension stripped with a `.` separating each subdirectory. For example, this directory would have these prompt names:
+        If any name collides with the name of a previously loaded prompt, the previous prompt will be overwritten.
+
+        ```
+        dir_path/
+            sub_dir/
+                prompt_1.txt        - sub_dir.prompt_1
+                not_a_prompt.jpg
+            prompt_2.txt            - prompt_2
+            another_prompt.txt      - another_prompt.txt
+        ```
+
+        Args:
+            dir_path: The path to the directory.
+        """
+
+        dir_path = Path(dir_path).expanduser().resolve()
+        if not dir_path.exists():
+            raise FileNotFoundError()
+
+        file_paths = glob.glob(f"{dir_path}/**/*.txt", recursive=True)
+        for file_path in file_paths:
+            file_path = Path(file_path)
+
+            try:
+                prompt = file_path.read_text()
+            except (UnicodeDecodeError, FileNotFoundError):
+                continue
+
+            rel_path = file_path.relative_to(dir_path)
+            name = ".".join(
+                (part if i != len(rel_path.parts) - 1 else part.rsplit(".", 1)[0])
+                for i, part in enumerate(rel_path.parts)
+            )
+            self.store_prompt(prompt, name)
+
+    def load_url(self, url: str):
+        """
+        Loads a prompt from the given url. Will send a GET request to the url and expects a response with the following schema:
+        ```
+        {
+            "prompts": [
+                {
+                    "name": "<prompt_name>",
+                    "prompt": "<prompt>"
+                }, ...
+            ]
+        }
+        ```
+        If any name collides with the name of a previously loaded prompt, the previous prompt will be overwritten.
+
+        Args:
+            url: The url.
+        """
+
+        raw_json = httpx.get(url).content.decode("utf-8")
+        try:
+            prompts = json.loads(raw_json)
+        except JSONDecodeError:
+            raise
+
+        try:
+            for prompt_object in prompts["prompts"]:
+                name, prompt = prompt_object["name"], prompt_object["prompt"]
+                self.store_prompt(prompt, name)
+        except:
+            raise
```

### Comparing `spiceai-0.1.9/spice/utils.py` & `spiceai-0.2.0/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.9/LICENSE` & `spiceai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.1.9/README.md` & `spiceai-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Spice
 
-Spice is an open source library for working with AI projects in Python. Spice simplifies LLM creations, embeddings, and transcriptions while using a single API for multiple providers, making switching between providers such as OpenAI and Anthropic incredibly simple.
+Spice is a light wrapper for AI SDKs like OpenAI's and Anthropic's. Spice simplifies LLM creations, embeddings, and transcriptions without obscuring any underlying parameters or processes. Spice also makes it ridiculously easy to switch between different providers, such as OpenAI and Anthropic, without having to modify your code.
 
-Spice also gathers useful information such as tokens used, time spent, and cost for each call, making it easily available no matter which LLM provider is being used.
+Spice also collects useful information such as tokens used, time spent, and cost for each call, making it easily available no matter which LLM provider is being used.
 
 ## Install
 
 Spice is listed under `spiceai` on PyPi. To install, simply `pip install spiceai`.
 
 ### API Keys
 
@@ -42,16 +42,20 @@
 
 ### Streaming
 
 ```python
 # You can set a default model for the client instead of passing it with each call
 client = Spice(default_text_model="claude-3-opus-20240229")
 
+# You can easily load prompts from files, directories, or even urls.
+client.load_prompt("prompt.txt", name="my prompt")
+
+# Spice can also automatically render Jinja templates.
 messages: List[SpiceMessage] = [
-    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "system", "content": client.get_rendered_prompt("my prompt", assistant_name="Ryan Reynolds")},
     {"role": "user", "content": "list 5 random words"},
 ]
 stream = await client.stream_response(messages=messages)
 
 async for text in stream:
     print(text, end="", flush=True)
 # Retrieve the complete response from the stream
@@ -124,20 +128,40 @@
 print(response.text)
 
 # Creating the model automatically registers it in Spice's model list, so listing the provider is no longer needed
 response = await client.get_response(messages=messages, model="first-gpt35")
 print(response.text)
 ```
 
+### Vision models
+
+```python
+client = Spice()
+
+# Spice makes it easy to add images from files or the internet
+from spice.spice_message import file_image_message, user_message
+
+messages: List[SpiceMessage] = [user_message("What do you see?"), file_image_message("/path/to/image.png")]
+response = await client.get_response(messages, GPT_4_1106_VISION_PREVIEW)
+print(response.text)
+
+# Alternatively, you can use the SpiceMessages wrapper to easily create your prompts
+spice_messages: SpiceMessages = SpiceMessages(client)
+spice_messages.add_user_message("What do you see?")
+spice_messages.add_file_image_message("https://example.com/image.png")
+response = await client.get_response(spice_messages, CLAUDE_3_OPUS_20240229)
+print(response.text)
+```
+
 ### Embeddings and Transcriptions
 
 ```python
 client = Spice()
 input_texts = ["Once upon a time...", "Cinderella"]
 
 # Spice can easily fetch embeddings and audio transcriptions
 from spice.models import TEXT_EMBEDDING_ADA_002, WHISPER_1
 
 embeddings = await client.get_embeddings(input_texts, TEXT_EMBEDDING_ADA_002)
 transcription = await client.get_transcription("/path/to/audio/file", WHISPER_1)
-print(transcription)
+print(transcription.text)
 ```
```

### Comparing `spiceai-0.1.9/PKG-INFO` & `spiceai-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
+Requires-Dist: httpx
+Requires-Dist: jinja2
 Requires-Dist: openai
 Requires-Dist: pillow
 Requires-Dist: python-dotenv
 Requires-Dist: tiktoken
 Provides-Extra: dev
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Spice
 
-Spice is an open source library for working with AI projects in Python. Spice simplifies LLM creations, embeddings, and transcriptions while using a single API for multiple providers, making switching between providers such as OpenAI and Anthropic incredibly simple.
+Spice is a light wrapper for AI SDKs like OpenAI's and Anthropic's. Spice simplifies LLM creations, embeddings, and transcriptions without obscuring any underlying parameters or processes. Spice also makes it ridiculously easy to switch between different providers, such as OpenAI and Anthropic, without having to modify your code.
 
-Spice also gathers useful information such as tokens used, time spent, and cost for each call, making it easily available no matter which LLM provider is being used.
+Spice also collects useful information such as tokens used, time spent, and cost for each call, making it easily available no matter which LLM provider is being used.
 
 ## Install
 
 Spice is listed under `spiceai` on PyPi. To install, simply `pip install spiceai`.
 
 ### API Keys
 
@@ -58,16 +60,20 @@
 
 ### Streaming
 
 ```python
 # You can set a default model for the client instead of passing it with each call
 client = Spice(default_text_model="claude-3-opus-20240229")
 
+# You can easily load prompts from files, directories, or even urls.
+client.load_prompt("prompt.txt", name="my prompt")
+
+# Spice can also automatically render Jinja templates.
 messages: List[SpiceMessage] = [
-    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "system", "content": client.get_rendered_prompt("my prompt", assistant_name="Ryan Reynolds")},
     {"role": "user", "content": "list 5 random words"},
 ]
 stream = await client.stream_response(messages=messages)
 
 async for text in stream:
     print(text, end="", flush=True)
 # Retrieve the complete response from the stream
@@ -140,20 +146,40 @@
 print(response.text)
 
 # Creating the model automatically registers it in Spice's model list, so listing the provider is no longer needed
 response = await client.get_response(messages=messages, model="first-gpt35")
 print(response.text)
 ```
 
+### Vision models
+
+```python
+client = Spice()
+
+# Spice makes it easy to add images from files or the internet
+from spice.spice_message import file_image_message, user_message
+
+messages: List[SpiceMessage] = [user_message("What do you see?"), file_image_message("/path/to/image.png")]
+response = await client.get_response(messages, GPT_4_1106_VISION_PREVIEW)
+print(response.text)
+
+# Alternatively, you can use the SpiceMessages wrapper to easily create your prompts
+spice_messages: SpiceMessages = SpiceMessages(client)
+spice_messages.add_user_message("What do you see?")
+spice_messages.add_file_image_message("https://example.com/image.png")
+response = await client.get_response(spice_messages, CLAUDE_3_OPUS_20240229)
+print(response.text)
+```
+
 ### Embeddings and Transcriptions
 
 ```python
 client = Spice()
 input_texts = ["Once upon a time...", "Cinderella"]
 
 # Spice can easily fetch embeddings and audio transcriptions
 from spice.models import TEXT_EMBEDDING_ADA_002, WHISPER_1
 
 embeddings = await client.get_embeddings(input_texts, TEXT_EMBEDDING_ADA_002)
 transcription = await client.get_transcription("/path/to/audio/file", WHISPER_1)
-print(transcription)
+print(transcription.text)
 ```
```

