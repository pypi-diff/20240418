# Comparing `tmp/ollama_haystack-0.0.5.tar.gz` & `tmp/ollama_haystack-0.0.6.tar.gz`

## Comparing `ollama_haystack-0.0.5.tar` & `ollama_haystack-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/example/chat_generator_example.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/example/generator_example.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/pydoc/config.yml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/embedders/ollama/__init__.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/embedders/ollama/document_embedder.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/embedders/ollama/text_embedder.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/__init__.py
--rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/chat/__init__.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/tests/test_chat_generator.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/tests/test_document_embedder.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/tests/test_generator.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/README.md
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ollama_haystack-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/chat_generator_example.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/embedders_example.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/examples/generator_example.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/pydoc/config.yml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/__init__.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/document_embedder.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/text_embedder.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/__init__.py
+-rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/chat/__init__.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_chat_generator.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_generator.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/README.md
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ollama_haystack-0.0.6/PKG-INFO
```

### Comparing `ollama_haystack-0.0.5/example/chat_generator_example.py` & `ollama_haystack-0.0.6/examples/chat_generator_example.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/example/generator_example.py` & `ollama_haystack-0.0.6/examples/generator_example.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/pydoc/config.yml` & `ollama_haystack-0.0.6/pydoc/config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 loaders:
   - type: haystack_pydoc_tools.loaders.CustomPythonLoader
     search_path: [../src]
     modules: [
       "haystack_integrations.components.generators.ollama.generator",
-      "haystack_integrations.components.generators.ollama.chat.chat_generator"
+      "haystack_integrations.components.generators.ollama.chat.chat_generator",
+      "haystack_integrations.components.embedders.ollama.document_embedder",
+      "haystack_integrations.components.embedders.ollama.text_embedder",
     ]
     ignore_when_discovered: ["__init__"]
 processors:
   - type: filter
     expression:
     documented_only: true
     do_not_filter_modules: false
@@ -19,11 +21,12 @@
   excerpt: Ollama integration for Haystack
   category_slug: integrations-api
   title: Ollama
   slug: integrations-ollama
   order: 170
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
-    filename: _readme_ollama.md
+    filename: _readme_ollama.md
```

### Comparing `ollama_haystack-0.0.5/src/haystack_integrations/components/embedders/ollama/document_embedder.py` & `ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/document_embedder.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,54 @@
 import requests
 from haystack import Document, component
 from tqdm import tqdm
 
 
 @component
 class OllamaDocumentEmbedder:
+    """
+    Computes the embeddings of a list of Documents and stores the obtained vectors in the embedding field of each
+    Document. It uses embedding models compatible with the Ollama Library.
+
+    Usage example:
+    ```python
+    from haystack import Document
+    from haystack_integrations.components.embedders.ollama import OllamaDocumentEmbedder
+
+    doc = Document(content="What do llamas say once you have thanked them? No probllama!")
+    document_embedder = OllamaDocumentEmbedder()
+
+    result = document_embedder.run([doc])
+    print(result['documents'][0].embedding)
+    ```
+    """
+
     def __init__(
         self,
         model: str = "nomic-embed-text",
         url: str = "http://localhost:11434/api/embeddings",
         generation_kwargs: Optional[Dict[str, Any]] = None,
         timeout: int = 120,
         prefix: str = "",
         suffix: str = "",
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
-        :param model: The name of the model to use. The model should be available in the running Ollama instance.
-            Default is "nomic-embed-text". "https://ollama.com/library/nomic-embed-text"
-        :param url: The URL of the chat endpoint of a running Ollama instance.
-            Default is "http://localhost:11434/api/embeddings".
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
-            top_p, and others. See the available arguments in
+        :param model:
+            The name of the model to use. The model should be available in the running Ollama instance.
+        :param url:
+            The URL of the chat endpoint of a running Ollama instance.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature, top_p, and others.
+            See the available arguments in
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :param timeout: The number of seconds before throwing a timeout error from the Ollama API.
-            Default is 120 seconds.
+        :param timeout:
+            The number of seconds before throwing a timeout error from the Ollama API.
         """
         self.timeout = timeout
         self.generation_kwargs = generation_kwargs or {}
         self.url = url
         self.model = model
         self.batch_size = 1  # API only supports a single call at the moment
         self.progress_bar = progress_bar
@@ -40,23 +58,20 @@
         self.embedding_separator = embedding_separator
         self.suffix = suffix
         self.prefix = prefix
 
     def _create_json_payload(self, text: str, generation_kwargs: Optional[Dict[str, Any]]) -> Dict[str, Any]:
         """
         Returns A dictionary of JSON arguments for a POST request to an Ollama service
-          :param text: Text that is to be converted to an embedding
-          :param generation_kwargs:
-          :return: A dictionary of arguments for a POST request to an Ollama service
         """
         return {"model": self.model, "prompt": text, "options": {**self.generation_kwargs, **(generation_kwargs or {})}}
 
     def _prepare_texts_to_embed(self, documents: List[Document]) -> List[str]:
         """
-        Prepare the texts to embed by concatenating the Document text with the metadata fields to embed.
+        Prepares the texts to embed by concatenating the Document text with the metadata fields to embed.
         """
         texts_to_embed = []
         for doc in documents:
             if self.meta_fields_to_embed is not None:
                 meta_values_to_embed = [
                     str(doc.meta[key])
                     for key in self.meta_fields_to_embed
@@ -97,20 +112,25 @@
         meta["model"] = self.model
 
         return all_embeddings, meta
 
     @component.output_types(documents=List[Document], meta=Dict[str, Any])
     def run(self, documents: List[Document], generation_kwargs: Optional[Dict[str, Any]] = None):
         """
-        Run an Ollama Model on a provided documents.
-        :param documents: Documents to be converted to an embedding.
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        Runs an Ollama Model to compute embeddings of the provided documents.
+
+        :param documents:
+            Documents to be converted to an embedding.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, etc. See the
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :return: Documents with embedding information attached and metadata in a dictionary
+        :returns: A dictionary with the following keys:
+            - `documents`: Documents with embedding information attached
+            - `meta`: The metadata collected during the embedding process
         """
         if not isinstance(documents, list) or documents and not isinstance(documents[0], Document):
             msg = (
                 "OllamaDocumentEmbedder expects a list of Documents as input."
                 "In case you want to embed a list of strings, please use the OllamaTextEmbedder."
             )
             raise TypeError(msg)
```

### Comparing `ollama_haystack-0.0.5/src/haystack_integrations/components/embedders/ollama/text_embedder.py` & `ollama_haystack-0.0.6/src/haystack_integrations/components/embedders/ollama/text_embedder.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,55 +2,72 @@
 
 import requests
 from haystack import component
 
 
 @component
 class OllamaTextEmbedder:
+    """
+    Computes the embeddings of a list of Documents and stores the obtained vectors in the embedding field of
+    each Document. It uses embedding models compatible with the Ollama Library.
+
+    Usage example:
+    ```python
+    from haystack_integrations.components.embedders.ollama import OllamaTextEmbedder
+
+    embedder = OllamaTextEmbedder()
+    result = embedder.run(text="What do llamas say once you have thanked them? No probllama!")
+    print(result['embedding'])
+    ```
+    """
+
     def __init__(
         self,
         model: str = "nomic-embed-text",
         url: str = "http://localhost:11434/api/embeddings",
         generation_kwargs: Optional[Dict[str, Any]] = None,
         timeout: int = 120,
     ):
         """
-        :param model: The name of the model to use. The model should be available in the running Ollama instance.
-            Default is "nomic-embed-text". "https://ollama.com/library/nomic-embed-text"
-        :param url: The URL of the chat endpoint of a running Ollama instance.
-            Default is "http://localhost:11434/api/embeddings".
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        :param model:
+            The name of the model to use. The model should be available in the running Ollama instance.
+        :param url:
+            The URL of the chat endpoint of a running Ollama instance.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, and others. See the available arguments in
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :param timeout: The number of seconds before throwing a timeout error from the Ollama API.
-            Default is 120 seconds.
+        :param timeout:
+            The number of seconds before throwing a timeout error from the Ollama API.
         """
         self.timeout = timeout
         self.generation_kwargs = generation_kwargs or {}
         self.url = url
         self.model = model
 
     def _create_json_payload(self, text: str, generation_kwargs: Optional[Dict[str, Any]]) -> Dict[str, Any]:
         """
         Returns A dictionary of JSON arguments for a POST request to an Ollama service
-          :param text: Text that is to be converted to an embedding
-          :param generation_kwargs:
-          :return: A dictionary of arguments for a POST request to an Ollama service
         """
         return {"model": self.model, "prompt": text, "options": {**self.generation_kwargs, **(generation_kwargs or {})}}
 
     @component.output_types(embedding=List[float], meta=Dict[str, Any])
     def run(self, text: str, generation_kwargs: Optional[Dict[str, Any]] = None):
         """
-        Run an Ollama Model on a given chat history.
-        :param text: Text to be converted to an embedding.
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        Runs an Ollama Model to compute embeddings of the provided text.
+
+        :param text:
+            Text to be converted to an embedding.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, etc. See the
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :return: A dictionary with the key "embedding" and a list of floats as the value
+        :returns: A dictionary with the following keys:
+            - `embedding`: The computed embeddings
+            - `meta`: The metadata collected during the embedding process
         """
 
         payload = self._create_json_payload(text, generation_kwargs)
 
         response = requests.post(url=self.url, json=payload, timeout=self.timeout)
 
         response.raise_for_status()
```

### Comparing `ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/generator.py` & `ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,59 +7,79 @@
 from haystack.utils.callable_serialization import deserialize_callable, serialize_callable
 from requests import Response
 
 
 @component
 class OllamaGenerator:
     """
-    Generator based on Ollama. Ollama is a library for easily running LLMs locally.
-    This component provides an interface to generate text using a LLM running in Ollama.
+    Provides an interface to generate text using an LLM running on Ollama.
+
+    Usage example:
+    ```python
+    from haystack_integrations.components.generators.ollama import OllamaGenerator
+
+    generator = OllamaGenerator(model="zephyr",
+                                url = "http://localhost:11434/api/generate",
+                                generation_kwargs={
+                                "num_predict": 100,
+                                "temperature": 0.9,
+                                })
+
+    print(generator.run("Who is the best American actor?"))
+    ```
     """
 
     def __init__(
         self,
         model: str = "orca-mini",
         url: str = "http://localhost:11434/api/generate",
         generation_kwargs: Optional[Dict[str, Any]] = None,
         system_prompt: Optional[str] = None,
         template: Optional[str] = None,
         raw: bool = False,
         timeout: int = 120,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
     ):
         """
-        :param model: The name of the model to use. The model should be available in the running Ollama instance.
-            Default is "orca-mini".
-        :param url: The URL of the generation endpoint of a running Ollama instance.
-            Default is "http://localhost:11434/api/generate".
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        :param model:
+            The name of the model to use. The model should be available in the running Ollama instance.
+        :param url:
+            The URL of the generation endpoint of a running Ollama instance.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, and others. See the available arguments in
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :param system_prompt: Optional system message (overrides what is defined in the Ollama Modelfile).
-        :param template: The full prompt template (overrides what is defined in the Ollama Modelfile).
-        :param raw: If True, no formatting will be applied to the prompt. You may choose to use the raw parameter
+        :param system_prompt:
+            Optional system message (overrides what is defined in the Ollama Modelfile).
+        :param template:
+            The full prompt template (overrides what is defined in the Ollama Modelfile).
+        :param raw:
+            If True, no formatting will be applied to the prompt. You may choose to use the raw parameter
             if you are specifying a full templated prompt in your API request.
-        :param timeout: The number of seconds before throwing a timeout error from the Ollama API.
-            Default is 120 seconds.
-        :param streaming_callback: A callback function that is called when a new token is received from the stream.
+        :param timeout:
+            The number of seconds before throwing a timeout error from the Ollama API.
+        :param streaming_callback:
+            A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
         """
         self.timeout = timeout
         self.raw = raw
         self.template = template
         self.system_prompt = system_prompt
         self.model = model
         self.url = url
         self.generation_kwargs = generation_kwargs or {}
         self.streaming_callback = streaming_callback
 
     def to_dict(self) -> Dict[str, Any]:
         """
-        Serialize this component to a dictionary.
-        :return: The serialized component as a dictionary.
+        Serializes the component to a dictionary.
+
+        :returns:
+              Dictionary with serialized data.
         """
         callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
         return default_to_dict(
             self,
             timeout=self.timeout,
             raw=self.raw,
             template=self.template,
@@ -69,111 +89,106 @@
             generation_kwargs=self.generation_kwargs,
             streaming_callback=callback_name,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "OllamaGenerator":
         """
-        Deserialize this component from a dictionary.
-        :param data: The dictionary representation of this component.
-        :return: The deserialized component instance.
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized component.
         """
         init_params = data.get("init_parameters", {})
         serialized_callback_handler = init_params.get("streaming_callback")
         if serialized_callback_handler:
             data["init_parameters"]["streaming_callback"] = deserialize_callable(serialized_callback_handler)
         return default_from_dict(cls, data)
 
     def _create_json_payload(self, prompt: str, stream: bool, generation_kwargs=None) -> Dict[str, Any]:
         """
         Returns a dictionary of JSON arguments for a POST request to an Ollama service.
-        :param prompt: The prompt to generate a response for.
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
-            top_p, and others. See the available arguments in
-            [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :return: A dictionary of arguments for a POST request to an Ollama service.
         """
         generation_kwargs = generation_kwargs or {}
         return {
             "prompt": prompt,
             "model": self.model,
             "stream": stream,
             "raw": self.raw,
             "template": self.template,
             "system": self.system_prompt,
             "options": generation_kwargs,
         }
 
     def _convert_to_response(self, ollama_response: Response) -> Dict[str, List[Any]]:
         """
-        Convert a response from the Ollama API to the required Haystack format.
-        :param ollama_response: A response (requests library) from the Ollama API.
-        :return: A dictionary of the returned responses and metadata.
+        Converts a response from the Ollama API to the required Haystack format.
         """
 
         resp_dict = ollama_response.json()
 
         replies = [resp_dict["response"]]
         meta = {key: value for key, value in resp_dict.items() if key != "response"}
 
         return {"replies": replies, "meta": [meta]}
 
     def _convert_to_streaming_response(self, chunks: List[StreamingChunk]) -> Dict[str, List[Any]]:
         """
-        Convert a list of chunks response required Haystack format.
-        :param chunks: List of StreamingChunks
-        :return: A dictionary of the returned responses and metadata.
+        Converts a list of chunks response required Haystack format.
         """
 
         replies = ["".join([c.content for c in chunks])]
         meta = {key: value for key, value in chunks[0].meta.items() if key != "response"}
 
         return {"replies": replies, "meta": [meta]}
 
     def _handle_streaming_response(self, response) -> List[StreamingChunk]:
-        """Handles Streaming response case
-
-        :param response: streaming response from ollama api.
-        :return: The List[StreamingChunk].
+        """
+        Handles Streaming response cases
         """
         chunks: List[StreamingChunk] = []
         for chunk in response.iter_lines():
             chunk_delta: StreamingChunk = self._build_chunk(chunk)
             chunks.append(chunk_delta)
             if self.streaming_callback is not None:
                 self.streaming_callback(chunk_delta)
         return chunks
 
     def _build_chunk(self, chunk_response: Any) -> StreamingChunk:
         """
         Converts the response from the Ollama API to a StreamingChunk.
-        :param chunk: The chunk returned by the Ollama API.
-        :return: The StreamingChunk.
         """
         decoded_chunk = json.loads(chunk_response.decode("utf-8"))
 
         content = decoded_chunk["response"]
         meta = {key: value for key, value in decoded_chunk.items() if key != "response"}
 
         chunk_message = StreamingChunk(content, meta)
         return chunk_message
 
-    @component.output_types(replies=List[str], metadata=List[Dict[str, Any]])
+    @component.output_types(replies=List[str], meta=List[Dict[str, Any]])
     def run(
         self,
         prompt: str,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
-        Run an Ollama Model on the given prompt.
-        :param prompt: The prompt to generate a response for.
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        Runs an Ollama Model on the given prompt.
+
+        :param prompt:
+            The prompt to generate a response for.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, and others. See the available arguments in
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :return: A dictionary of the response and returned metadata
+        :returns: A dictionary with the following keys:
+            - `replies`: The responses from the model
+            - `meta`: The metadata collected during the run
         """
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
         stream = self.streaming_callback is not None
 
         json_payload = self._create_json_payload(prompt, stream, generation_kwargs)
```

### Comparing `ollama_haystack-0.0.5/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py` & `ollama_haystack-0.0.6/src/haystack_integrations/components/generators/ollama/chat/chat_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,88 +5,107 @@
 from haystack.dataclasses import ChatMessage
 from requests import Response
 
 
 @component
 class OllamaChatGenerator:
     """
-    Chat Generator based on Ollama. Ollama is a library for easily running LLMs locally.
-    This component provides an interface to generate text using a LLM running in Ollama.
+    Supports models running on Ollama, such as llama2 and mixtral.  Find the full list of supported models
+    [here](https://ollama.ai/library).
+
+    Usage example:
+    ```python
+    from haystack_integrations.components.generators.ollama import OllamaChatGenerator
+    from haystack.dataclasses import ChatMessage
+
+    generator = OllamaChatGenerator(model="zephyr",
+                                url = "http://localhost:11434/api/chat",
+                                generation_kwargs={
+                                "num_predict": 100,
+                                "temperature": 0.9,
+                                })
+
+    messages = [ChatMessage.from_system("\nYou are a helpful, respectful and honest assistant"),
+    ChatMessage.from_user("What's Natural Language Processing?")]
+
+    print(generator.run(messages=messages))
+    ```
     """
 
     def __init__(
         self,
         model: str = "orca-mini",
         url: str = "http://localhost:11434/api/chat",
         generation_kwargs: Optional[Dict[str, Any]] = None,
         template: Optional[str] = None,
         timeout: int = 120,
     ):
         """
-        :param model: The name of the model to use. The model should be available in the running Ollama instance.
-            Default is "orca-mini".
-        :param url: The URL of the chat endpoint of a running Ollama instance.
-            Default is "http://localhost:11434/api/chat".
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        :param model:
+            The name of the model to use. The model should be available in the running Ollama instance.
+        :param url:
+            The URL of the chat endpoint of a running Ollama instance.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, and others. See the available arguments in
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :param template: The full prompt template (overrides what is defined in the Ollama Modelfile).
-        :param timeout: The number of seconds before throwing a timeout error from the Ollama API.
-            Default is 120 seconds.
+        :param template:
+            The full prompt template (overrides what is defined in the Ollama Modelfile).
+        :param timeout:
+            The number of seconds before throwing a timeout error from the Ollama API.
         """
 
         self.timeout = timeout
         self.template = template
         self.generation_kwargs = generation_kwargs or {}
         self.url = url
         self.model = model
 
     def _message_to_dict(self, message: ChatMessage) -> Dict[str, str]:
         return {"role": message.role.value, "content": message.content}
 
     def _create_json_payload(self, messages: List[ChatMessage], generation_kwargs=None) -> Dict[str, Any]:
         """
         Returns A dictionary of JSON arguments for a POST request to an Ollama service
-        :param messages: A history/list of chat messages
-        :param generation_kwargs:
-        :return: A dictionary of arguments for a POST request to an Ollama service
         """
         generation_kwargs = generation_kwargs or {}
         return {
             "messages": [self._message_to_dict(message) for message in messages],
             "model": self.model,
             "stream": False,
             "template": self.template,
             "options": generation_kwargs,
         }
 
     def _build_message_from_ollama_response(self, ollama_response: Response) -> ChatMessage:
         """
         Converts the non-streaming response from the Ollama API to a ChatMessage.
-        :param ollama_response: The completion returned by the Ollama API.
-        :return: The ChatMessage.
         """
         json_content = ollama_response.json()
         message = ChatMessage.from_assistant(content=json_content["message"]["content"])
         message.meta.update({key: value for key, value in json_content.items() if key != "message"})
         return message
 
     @component.output_types(replies=List[ChatMessage])
     def run(
         self,
         messages: List[ChatMessage],
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
-        Run an Ollama Model on a given chat history.
-        :param messages: A list of ChatMessage instances representing the input messages.
-        :param generation_kwargs: Optional arguments to pass to the Ollama generation endpoint, such as temperature,
+        Runs an Ollama Model on a given chat history.
+
+        :param messages:
+            A list of ChatMessage instances representing the input messages.
+        :param generation_kwargs:
+            Optional arguments to pass to the Ollama generation endpoint, such as temperature,
             top_p, etc. See the
             [Ollama docs](https://github.com/jmorganca/ollama/blob/main/docs/modelfile.md#valid-parameters-and-values).
-        :return: A dictionary of the replies containing their metadata
+        :returns: A dictionary with the following keys:
+            - `replies`: The responses from the model
         """
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
         json_payload = self._create_json_payload(messages, generation_kwargs)
 
         response = requests.post(url=self.url, json=json_payload, timeout=self.timeout)
```

### Comparing `ollama_haystack-0.0.5/tests/test_chat_generator.py` & `ollama_haystack-0.0.6/tests/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/tests/test_document_embedder.py` & `ollama_haystack-0.0.6/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/tests/test_generator.py` & `ollama_haystack-0.0.6/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/tests/test_text_embedder.py` & `ollama_haystack-0.0.6/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/.gitignore` & `ollama_haystack-0.0.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 .pyre/
 
 # IDEs
 .vscode
 
 # Docs generation artifacts
 _readme_*.md
+.idea
```

### Comparing `ollama_haystack-0.0.5/LICENSE.txt` & `ollama_haystack-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/README.md` & `ollama_haystack-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ollama_haystack-0.0.5/pyproject.toml` & `ollama_haystack-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -96,20 +96,20 @@
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.ruff.isort]
 known-first-party = ["src"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
@@ -149,32 +149,29 @@
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 # Examples can print their output
-"example/**" = ["T201"]
+"examples/**" = ["T201"]
 
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
-
-
-[tool.coverage.paths]
-ollama_haystack = ["src/haystack_integrations", "*/ollama-haystack/src"]
-tests = ["tests", "*/ollama-haystack/tests"]
+parallel = false
 
 [tool.coverage.report]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
 exclude_lines = [
-    "no cov",
-    "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:",
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
 ]
 
 [tool.pytest.ini_options]
 markers = [
     "integration: marks tests as slow (deselect with '-m \"not integration\"')",
 ]
 addopts = [
```

### Comparing `ollama_haystack-0.0.5/PKG-INFO` & `ollama_haystack-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ollama-haystack
-Version: 0.0.5
+Version: 0.0.6
 Summary: An integration between the Ollama LLM framework and Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ollama#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ollama
 Author-email: Alistair Rogers <alistairlr112@gmail.com>, Sachin Sachdeva <emailforsachinsachdeva@gmail.com>, deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

