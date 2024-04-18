# Comparing `tmp/vlite-0.2.1.tar.gz` & `tmp/vlite-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.2.1.tar", last modified: Thu Apr 11 04:25:00 2024, max compression
+gzip compressed data, was "vlite-0.2.3.tar", last modified: Thu Apr 18 05:19:30 2024, max compression
```

## Comparing `vlite-0.2.1.tar` & `vlite-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.230357 vlite-0.2.1/
--rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.1/LICENSE
--rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-11 04:25:00.230217 vlite-0.2.1/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     2635 2024-04-05 11:47:06.000000 vlite-0.2.1/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-11 04:25:00.230404 vlite-0.2.1/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      558 2024-04-11 04:24:38.000000 vlite-0.2.1/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.229364 vlite-0.2.1/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       80 2024-04-11 04:24:48.000000 vlite-0.2.1/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     6915 2024-04-11 03:44:32.000000 vlite-0.2.1/vlite/ctx.py
--rw-r--r--   0 sdan       (501) staff       (20)    10160 2024-04-11 04:17:33.000000 vlite-0.2.1/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     3156 2024-04-11 02:57:53.000000 vlite-0.2.1/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     7747 2024-04-11 04:24:51.000000 vlite-0.2.1/vlite/server.py
--rw-r--r--   0 sdan       (501) staff       (20)     7733 2024-04-11 04:23:32.000000 vlite-0.2.1/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.230027 vlite-0.2.1/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      261 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)      118 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-18 05:19:30.787827 vlite-0.2.3/
+-rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.3/LICENSE
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-18 05:19:30.787672 vlite-0.2.3/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     3247 2024-04-18 04:36:43.000000 vlite-0.2.3/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-18 05:19:30.787881 vlite-0.2.3/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)     1043 2024-04-17 20:14:43.000000 vlite-0.2.3/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-18 05:19:30.783419 vlite-0.2.3/tests/
+-rw-r--r--   0 sdan       (501) staff       (20)     6320 2024-04-03 19:37:27.000000 vlite-0.2.3/tests/test_server.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-18 05:19:30.786296 vlite-0.2.3/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       57 2024-04-17 20:14:36.000000 vlite-0.2.3/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     6744 2024-04-17 09:21:55.000000 vlite-0.2.3/vlite/ctx.py
+-rw-r--r--   0 sdan       (501) staff       (20)     1313 2024-04-17 09:02:04.000000 vlite-0.2.3/vlite/index.py
+-rw-r--r--   0 sdan       (501) staff       (20)    13387 2024-04-18 04:37:17.000000 vlite-0.2.3/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     4484 2024-04-17 09:30:24.000000 vlite-0.2.3/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7781 2024-04-17 20:14:19.000000 vlite-0.2.3/vlite/server.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7980 2024-04-14 22:49:23.000000 vlite-0.2.3/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-18 05:19:30.787446 vlite-0.2.3/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-18 05:19:30.000000 vlite-0.2.3/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      297 2024-04-18 05:19:30.000000 vlite-0.2.3/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-18 05:19:30.000000 vlite-0.2.3/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)      154 2024-04-18 05:19:30.000000 vlite-0.2.3/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-18 05:19:30.000000 vlite-0.2.3/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.2.1/LICENSE` & `vlite-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vlite-0.2.1/vlite/ctx.py` & `vlite-0.2.3/vlite/ctx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import os
 import struct
 import json
 from enum import Enum
 from typing import List, Dict, Union
 import numpy as np
+import logging
+
+
+logging.basicConfig(level=logging.WARNING, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
 
 class CtxSectionType(Enum):
     HEADER = 0
     EMBEDDINGS = 1
     CONTEXTS = 2
     METADATA = 3
 
@@ -37,45 +42,42 @@
         self.embeddings.append(embedding)
 
     def add_context(self, context: str):
         self.contexts.append(context)
 
     def add_metadata(self, key: str, value: Union[int, float, str]):
         self.metadata[key] = value
-
+        
     def save(self):
-        print("Number of embeddings to save: ", len(self.embeddings))
-        print("Number of metadata keys to save: ", len(self.metadata))
         with open(self.file_path, "wb") as file:
             file.write(self.MAGIC_NUMBER)
             file.write(struct.pack("<I", self.VERSION))
 
             header_json = json.dumps(self.header).encode("utf-8")
             file.write(struct.pack("<II", CtxSectionType.HEADER.value, len(header_json)))
             file.write(header_json)
 
             if self.embeddings:
                 embeddings_data = b"".join(
-                    struct.pack(f"<{len(emb)}f", *[float(x) if not np.isnan(x) else 0.0 for x in emb])
+                    struct.pack(f"<{64}f", *emb[:64])  # Use a fixed size of 64
                     for emb in self.embeddings
                 )
                 file.write(struct.pack("<II", CtxSectionType.EMBEDDINGS.value, len(embeddings_data)))
                 file.write(embeddings_data)
 
             contexts_data = b"".join(struct.pack("<I", len(context.encode("utf-8"))) + context.encode("utf-8") for context in self.contexts)
             file.write(struct.pack("<II", CtxSectionType.CONTEXTS.value, len(contexts_data)))
             file.write(contexts_data)
 
             metadata_json = json.dumps(self.metadata).encode("utf-8")
             file.write(struct.pack("<II", CtxSectionType.METADATA.value, len(metadata_json)))
             file.write(metadata_json)
         
+
     def load(self):
-        print("Number of embeddings loaded: ", len(self.embeddings))
-        print("Number of metadata keys loaded: ", len(self.metadata))
         try:
             with open(self.file_path, "rb") as file:
                 # Read and verify header
                 magic_number = file.read(len(self.MAGIC_NUMBER))
                 if magic_number != self.MAGIC_NUMBER:
                     raise ValueError(f"Invalid magic number: {magic_number}")
 
@@ -92,41 +94,41 @@
 
                     if section_type == CtxSectionType.HEADER.value:
                         header_json = file.read(section_length).decode("utf-8")
                         self.header = json.loads(header_json)
                     elif section_type == CtxSectionType.EMBEDDINGS.value:
                         embeddings_data = file.read(section_length)
                         if embeddings_data:
-                            embedding_size = len(embeddings_data) // 4
+                            embedding_size = 64  # Use a fixed size of 64
+                            num_embeddings = len(embeddings_data) // (embedding_size * 4)
                             self.embeddings = [
-                                list(struct.unpack_from(f"<{embedding_size // len(self.embeddings)}f", embeddings_data, i * embedding_size))
-                                for i in range(len(self.embeddings))
-                            ] if self.embeddings else [list(struct.unpack_from(f"<{embedding_size}f", embeddings_data))]
+                                list(struct.unpack_from(f"<{embedding_size}f", embeddings_data, i * embedding_size * 4))
+                                for i in range(num_embeddings)
+                            ]
                     elif section_type == CtxSectionType.CONTEXTS.value:
                         contexts_data = file.read(section_length)
                         self.contexts = []
                         offset = 0
                         while offset < len(contexts_data):
                             context_length = struct.unpack_from("<I", contexts_data, offset)[0]
                             offset += 4
                             try:
                                 context = contexts_data[offset : offset + context_length].decode("utf-8")
                                 self.contexts.append(context)
                             except UnicodeDecodeError as e:
-                                print(f"Error decoding context: {e}")
+                                logger.error(f"Error decoding context: {e}")
                             offset += context_length
                     elif section_type == CtxSectionType.METADATA.value:
                         metadata_json = file.read(section_length).decode("utf-8")
                         self.metadata = json.loads(metadata_json)
                     else:
                         raise ValueError(f"Unknown section type: {section_type}")
-
         except FileNotFoundError:
             pass
-    
+
     def __repr__(self):
         output = "CtxFile:\n\n"
         output += "Header:\n"
         for key, value in self.header.items():
             output += f"  {key}: {value}\n"
         output += "\nEmbeddings:\n"
         for i, embedding in enumerate(self.embeddings):
@@ -141,15 +143,15 @@
 
     def __enter__(self):
         self.load()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.save()
-    
+
 class Ctx:
     def __init__(self, directory="contexts"):
         self.directory = directory
         if not os.path.exists(directory):
             os.makedirs(directory)
 
     def get(self, user):
```

### Comparing `vlite-0.2.1/vlite/main.py` & `vlite-0.2.3/vlite/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,298 @@
 import numpy as np
 from uuid import uuid4
+from .utils import check_cuda_available, check_mps_available
 from .model import EmbeddingModel
 from .utils import chop_and_chunk
 import datetime
 from .ctx import Ctx
+import time
+import logging
+
+# Configure logging
+logging.basicConfig(level=logging.WARNING, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
+
 
 class VLite:
-    def __init__(self, collection=None, device='cpu', model_name='mixedbread-ai/mxbai-embed-large-v1'):
+    def __init__(self, collection=None, device=None, model_name='mixedbread-ai/mxbai-embed-large-v1'):
+        start_time = time.time()
+        if device is None:
+            if check_cuda_available():
+                device = 'cuda'
+            elif check_mps_available():
+                device = 'mps'
+            else:
+                device = 'cpu'
+        logger.info(f"[VLite.__init__] Initializing VLite with device: {device}")
+        self.device = device
         if collection is None:
             current_datetime = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
             collection = f"vlite_{current_datetime}"
         self.collection = f"{collection}"
-        self.device = device
-        self.model = EmbeddingModel(model_name) if model_name else EmbeddingModel()
-        
+        self.model = EmbeddingModel(model_name, device=device) if model_name else EmbeddingModel()
         self.ctx = Ctx()
         self.index = {}
-
         try:
             ctx_file = self.ctx.read(collection)
             ctx_file.load()
-            # debug print
-            print("Number of embeddings: ", len(ctx_file.embeddings))
-            print("Number of metadata: ", len(ctx_file.metadata))
+
             self.index = {
                 chunk_id: {
                     'text': ctx_file.contexts[idx] if idx < len(ctx_file.contexts) else "",
                     'metadata': ctx_file.metadata.get(chunk_id, {}),
-                    'binary_vector': np.array(ctx_file.embeddings[idx]) if idx < len(ctx_file.embeddings) else np.zeros(self.model.embedding_size)
+                    'binary_vector': np.array(ctx_file.embeddings[idx]) if idx < len(ctx_file.embeddings) else np.zeros(self.model.dimension)
                 }
                 for idx, chunk_id in enumerate(ctx_file.metadata.keys())
             }
         except FileNotFoundError:
-            print(f"Collection file {self.collection} not found. Initializing empty attributes.")
+            logger.warning(f"[VLite.__init__] Collection file {self.collection} not found. Initializing empty attributes.")
+
+        end_time = time.time()
+        logger.debug(f"[VLite.__init__] Execution time: {end_time - start_time:.5f} seconds")
+        logger.info(f"[VLite.__init__] Using device: {self.device}")
 
-    def add(self, data, metadata=None, item_id=None, need_chunks=True, fast=True):
+    def add(self, data, metadata=None, item_id=None, need_chunks=False, fast=True):
+        start_time = time.time()
         data = [data] if not isinstance(data, list) else data
         results = []
         all_chunks = []
         all_metadata = []
         all_ids = []
-
         for item in data:
             if isinstance(item, dict):
                 text_content = item['text']
                 item_metadata = item.get('metadata', {})
             else:
                 text_content = item
                 item_metadata = {}
-
             if item_id is None:
                 item_id = str(uuid4())
-
             item_metadata.update(metadata or {})
-
             if need_chunks:
                 chunks = chop_and_chunk(text_content, fast=fast)
             else:
                 chunks = [text_content]
-                print("Encoding text... not chunking")
-
+            logger.debug("[VLite.add] Encoding text... not chunking")
             all_chunks.extend(chunks)
             all_metadata.extend([item_metadata] * len(chunks))
             all_ids.extend([item_id] * len(chunks))
+        binary_encoded_data = self.model.embed(all_chunks, precision="binary")
 
-        encoded_data = self.model.embed(all_chunks, device=self.device)
-        binary_encoded_data = self.model.quantize(encoded_data, precision="binary")
 
         for idx, (chunk, binary_vector, metadata) in enumerate(zip(all_chunks, binary_encoded_data, all_metadata)):
             chunk_id = f"{item_id}_{idx}"
             self.index[chunk_id] = {
                 'text': chunk,
                 'metadata': metadata,
                 'binary_vector': binary_vector.tolist()
             }
 
         if item_id not in [result[0] for result in results]:
             results.append((item_id, binary_encoded_data, metadata))
 
         self.save()
-        print("Text added successfully.")
+        logger.info("[VLite.add] Text added successfully.")
+        end_time = time.time()
+        logger.debug(f"[VLite.add] Execution time: {end_time - start_time:.5f} seconds")
         return results
 
+        
+
     def retrieve(self, text=None, top_k=5, metadata=None, return_scores=False):
-        print("Retrieving similar texts...")
+        start_time = time.time()
+        logger.info("[VLite.retrieve] Retrieving similar texts...")
         if text:
-            print(f"Retrieving top {top_k} similar texts for query: {text}")
-            query_chunks = chop_and_chunk(text, fast=True)
-            query_vectors = self.model.embed(query_chunks, device=self.device)
-            query_binary_vectors = self.model.quantize(query_vectors, precision="binary")
-            
+            logger.info(f"[VLite.retrieve] Retrieving top {top_k} similar texts for query: {text}")
+            query_binary_vectors = self.model.embed(text, precision="binary")
+            # Perform search on the query binary vectors
             results = []
             for query_binary_vector in query_binary_vectors:
-                chunk_results = self.search(query_binary_vector, top_k, metadata)
+                chunk_results = self.rank_and_filter(query_binary_vector, top_k, metadata)
                 results.extend(chunk_results)
-            
-            results.sort(key=lambda x: x[1], reverse=True)
+            # Sort the results by similarity score
+            results.sort(key=lambda x: x[1])
             results = results[:top_k]
-            
-            print("Retrieval completed.")
+            logger.info("[VLite.retrieve] Retrieval completed.")
+            end_time = time.time()
+            logger.debug(f"[VLite.retrieve] Execution time: {end_time - start_time:.5f} seconds")
             if return_scores:
-                return [(self.index[idx]['text'], score, self.index[idx]['metadata']) for idx, score in results]
+                return [(idx, self.index[idx]['text'], self.index[idx]['metadata'], score) for idx, score in results]
             else:
-                return [(self.index[idx]['text'], self.index[idx]['metadata']) for idx, _ in results]
-        
-    def search(self, query_binary_vector, top_k, metadata=None):
-        # Reshape query_binary_vector to 1D array
-        query_binary_vector = query_binary_vector.reshape(-1)
-
-        # Perform binary search
-        binary_vectors = np.array([item['binary_vector'] for item in self.index.values()])
-        binary_similarities = np.einsum('i,ji->j', query_binary_vector, binary_vectors)
-        top_k_indices = np.argpartition(binary_similarities, -top_k)[-top_k:]
-        top_k_ids = [list(self.index.keys())[idx] for idx in top_k_indices]
+                return [(idx, self.index[idx]['text'], self.index[idx]['metadata']) for idx, _ in results]
 
+    def rank_and_filter(self, query_binary_vector, top_k, metadata=None):
+        start_time = time.time()
+        logger.debug(f"[VLite.rank_and_filter] Shape of query vector: {query_binary_vector.shape}")
+        query_binary_vector = np.array(query_binary_vector).reshape(-1)
+        logger.debug(f"[VLite.rank_and_filter] Shape of query vector after reshaping: {query_binary_vector.shape}")
+        # Collect all binary vectors and ensure they all have the same shape as the query vector
+        binary_vectors = [item['binary_vector'] for item in self.index.values() if len(item['binary_vector']) == len(query_binary_vector)]        
+        binary_vector_indices = [idx for idx, item in enumerate(self.index.values()) if len(item['binary_vector']) == len(query_binary_vector)]
+        if binary_vectors:
+            corpus_binary_vectors = np.asarray(binary_vectors, dtype=np.float32)
+            logger.debug(f"[VLite.rank_and_filter] Shape of corpus binary vectors array: {corpus_binary_vectors.shape}")
+        else:
+            raise ValueError("No valid binary vectors found for comparison.")
+        top_k_indices, top_k_scores = self.model.search(query_binary_vector, corpus_binary_vectors, top_k)
+        logger.debug(f"[VLite.rank_and_filter] Top {top_k} indices: {top_k_indices}")
+        logger.debug(f"[VLite.rank_and_filter] Top {top_k} scores: {top_k_scores}")
+        logger.debug(f"[VLite.rank_and_filter] No. of items in the collection: {len(self.index)}")
+        logger.debug(f"[VLite.rank_and_filter] Vlite count: {self.count()}")
+
+        top_k_ids = [list(self.index.keys())[binary_vector_indices[idx]] for idx in top_k_indices]
         # Apply metadata filter on the retrieved top_k items
+        filtered_ids = []
         if metadata:
-            filtered_ids = []
             for chunk_id in top_k_ids:
                 item_metadata = self.index[chunk_id]['metadata']
                 if all(item_metadata.get(key) == value for key, value in metadata.items()):
                     filtered_ids.append(chunk_id)
             top_k_ids = filtered_ids[:top_k]
-
-        # Get the similarity scores for the top_k items
-        top_k_scores = binary_similarities[top_k_indices]
-
+            top_k_scores = top_k_scores[:len(top_k_ids)]
+        end_time = time.time()
+        logger.debug(f"[VLite.rank_and_filter] Execution time: {end_time - start_time:.5f} seconds")
         return list(zip(top_k_ids, top_k_scores))
 
-
     def update(self, id, text=None, metadata=None, vector=None):
+        start_time = time.time()
         chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
         if chunk_ids:
             for chunk_id in chunk_ids:
                 if text is not None:
                     self.index[chunk_id]['text'] = text
                 if metadata is not None:
                     self.index[chunk_id]['metadata'].update(metadata)
                 if vector is not None:
                     self.index[chunk_id]['vector'] = vector
             self.save()
-            print(f"Item with ID '{id}' updated successfully.")
+            logger.info(f"[VLite.update] Item with ID '{id}' updated successfully.")
+            end_time = time.time()
+            logger.debug(f"[VLite.update] Execution time: {end_time - start_time:.5f} seconds")
             return True
         else:
-            print(f"Item with ID '{id}' not found.")
+            logger.warning(f"[VLite.update] Item with ID '{id}' not found.")
             return False
 
-
     def delete(self, ids):
         if isinstance(ids, str):
             ids = [ids]
-
         deleted_count = 0
         for id in ids:
             chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
             for chunk_id in chunk_ids:
                 if chunk_id in self.index:
                     del self.index[chunk_id]
                     deleted_count += 1
-
         if deleted_count > 0:
             self.save()
-            print(f"Deleted {deleted_count} item(s) from the collection.")
+            logger.info(f"[VLite.delete] Deleted {deleted_count} item(s) from the collection.")
         else:
-            print("No items found with the specified IDs.")
-
+            logger.warning("[VLite.delete] No items found with the specified IDs.")
         return deleted_count
 
-    
-
     def get(self, ids=None, where=None):
         if ids is not None:
             if isinstance(ids, str):
                 ids = [ids]
             items = []
             for id in ids:
                 item_chunks = []
                 item_metadata = {}
                 for chunk_id, chunk_data in self.index.items():
                     if chunk_id.startswith(f"{id}_"):
                         item_chunks.append(chunk_data['text'])
                         item_metadata.update(chunk_data['metadata'])
                 if item_chunks:
                     item_text = ' '.join(item_chunks)
-                    items.append((item_text, item_metadata))
+                    items.append((id, item_text, item_metadata))
         else:
             items = []
-            item_dict = {}
             for chunk_id, chunk_data in self.index.items():
                 item_id = chunk_id.split('_')[0]
-                if item_id not in item_dict:
-                    item_dict[item_id] = {'chunks': [], 'metadata': {}}
-                item_dict[item_id]['chunks'].append(chunk_data['text'])
-                item_dict[item_id]['metadata'].update(chunk_data['metadata'])
-            for item_id, item_data in item_dict.items():
-                item_text = ' '.join(item_data['chunks'])
-                item_metadata = item_data['metadata']
-                items.append((item_text, item_metadata))
-
+                item_text = chunk_data['text']
+                item_metadata = chunk_data['metadata']
+                items.append((item_id, item_text, item_metadata))
         if where is not None:
-            items = [item for item in items if all(item[1].get(key) == value for key, value in where.items())]
-
+            items = [item for item in items if all(item[2].get(key) == value for key, value in where.items())]
         return items
 
     def set(self, id, text=None, metadata=None, vector=None):
-        print(f"Setting attributes for item with ID: {id}")
+        logger.info(f"[VLite.set] Setting attributes for item with ID: {id}")
         chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
         if chunk_ids:
             self.update(id, text, metadata, vector)
         else:
             self.add(text, metadata=metadata, item_id=id)
-            print(f"Item with ID '{id}' created successfully.")
-            
-                
+        logger.info(f"[VLite.set] Item with ID '{id}' created successfully.")
+    
+    
+    def set_batch(self, texts, embeddings, metadatas=None):
+        start_time = time.time()
+        if not isinstance(texts, list):
+            texts = [texts]
+
+        if metadatas is None:
+            metadatas = [{}] * len(texts)
+        elif not isinstance(metadatas, list):
+            metadatas = [metadatas]
+
+        if len(texts) != len(embeddings):
+            print("asdasd",len(texts), len(embeddings))
+            raise ValueError("The number of texts and embeddings must be the same.")
+
+        if len(texts) != len(metadatas):
+            raise ValueError("The number of texts and metadatas must be the same.")
+
+        for text, embedding, metadata in zip(texts, embeddings, metadatas):
+            item_id = str(uuid4())
+            chunk_id = f"{item_id}_0"
+
+            self.index[chunk_id] = {
+                'text': text,
+                'metadata': metadata,
+                'binary_vector': embedding.tolist()
+            }
+    
+
+        self.save()
+        logger.info("[VLite.set_batch] Texts added successfully.")
+        end_time = time.time()
+        logger.debug(f"[VLite.set_batch] Execution time: {end_time - start_time:.5f} seconds")
+        
 
     def count(self):
         return len(self.index)
-    
 
     def save(self):
-        print(f"Saving collection to {self.collection}")
+        logger.info(f"[VLite.save] Saving collection to {self.collection}")
         with self.ctx.create(self.collection) as ctx_file:
             ctx_file.set_header(
                 embedding_model="mixedbread-ai/mxbai-embed-large-v1",
-                embedding_size=self.model.model_metadata.get('bert.embedding_length', 1024),
+                embedding_size=64,  # Set the correct embedding size here
                 embedding_dtype=self.model.embedding_dtype,
-                context_length=self.model.model_metadata.get('bert.context_length', 512)
+                context_length=self.model.context_length
             )
             for chunk_id, chunk_data in self.index.items():
                 ctx_file.add_embedding(chunk_data['binary_vector'])
                 ctx_file.add_context(chunk_data['text'])
                 if 'metadata' in chunk_data:
                     ctx_file.add_metadata(chunk_id, chunk_data['metadata'])
-        print("Collection saved successfully.")
+        logger.info("[VLite.save] Collection saved successfully.")
 
     def clear(self):
-        print("Clearing the collection...")
+        logger.info("[VLite.clear] Clearing the collection...")
         self.index = {}
         self.ctx.delete(self.collection)
-        print("Collection cleared.")
-    
+        logger.info("[VLite.clear] Collection cleared.")
+
     def info(self):
-        print("Collection Information:")
-        print(f"  Items: {self.count()}")
-        print(f"  Collection file: {self.collection}")
-        print(f"  Embedding model: {self.model}")
+        print("[VLite.info] Collection Information:")
+        print(f"[VLite.info] Items: {self.count()}")
+        print(f"[VLite.info] Collection file: {self.collection}")
+        print(f"[VLite.info] Embedding model: {self.model}")
 
     def __repr__(self):
         return f"VLite(collection={self.collection}, device={self.device}, model={self.model})"
 
     def dump(self):
         return self.index
```

### Comparing `vlite-0.2.1/vlite/server.py` & `vlite-0.2.3/vlite/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from fastapi import FastAPI, HTTPException, File, UploadFile
 from pydantic import BaseModel
 from typing import List, Optional, Union
 from vlite.main import VLite
 from vlite.utils import process_file, process_pdf, process_webpage
+from setup import __version__
 
 app = FastAPI(
     title="VLite API",
     description="API for VLite, a simple vector database for text embedding and retrieval.",
-    version="0.2.1",
+    version=__version__,
 )
 
 vlite = VLite()
 
 class TextData(BaseModel):
     text: str
     metadata: Optional[dict] = None
```

### Comparing `vlite-0.2.1/vlite/utils.py` & `vlite-0.2.3/vlite/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from typing import List
 import tiktoken
 import numpy as np
 import itertools
+import platform
+import subprocess
 
 try:
     from surya.ocr import run_ocr
     from surya.model.detection import segformer
     from surya.model.recognition.model import load_model
     from surya.model.recognition.processor import load_processor
     from surya.input.load import load_from_file, load_pdf
@@ -24,16 +26,14 @@
     """
     Chop text into chunks of max_seq_length tokens or max_seq_length*4 characters (fast mode).
     """
     if isinstance(text, str):
         text = [text]
     enc = tiktoken.get_encoding("cl100k_base")
     chunks = []
-    print(f"Length of text: {len(text)}")
-    # print(f"Original text: {text}")
     for t in text:
         if fast:
             chunk_size = max_seq_length * 4
             chunks.extend([t[i:i + chunk_size] for i in range(0, len(t), chunk_size)])
         else:
             token_ids = enc.encode(t, disallowed_special=())
             num_tokens = len(token_ids)
@@ -221,8 +221,20 @@
         for page in iter(reader.pages):
             extracted_text.append(page.extract_text())  
     return extracted_text
 
 def count_tokens(text):
     enc = tiktoken.get_encoding("cl100k_base")
     token_ids = enc.encode(text, disallowed_special=())
-    return len(token_ids)
+    return len(token_ids)
+
+def check_cuda_available():
+    try:
+        subprocess.check_output(['nvidia-smi'])
+        return True
+    except Exception:
+        return False
+
+def check_mps_available():
+    if platform.system() == "Darwin" or platform.processor().upper() == "ARM":
+        return True
+    return False
```

