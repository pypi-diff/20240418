# Comparing `tmp/paper_qa-4.5.1.tar.gz` & `tmp/paper_qa-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper_qa-4.5.1.tar", last modified: Sun Apr 14 16:44:54 2024, max compression
+gzip compressed data, was "paper_qa-4.5.2.tar", last modified: Thu Apr 18 05:44:19 2024, max compression
```

## Comparing `paper_qa-4.5.1.tar` & `paper_qa-4.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.149600 paper_qa-4.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 16:42:43.000000 paper_qa-4.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-14 16:44:54.149600 paper_qa-4.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-14 16:42:43.000000 paper_qa-4.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-14 16:42:43.000000 paper_qa-4.5.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31980 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/llms.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-14 16:42:43.000000 paper_qa-4.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:44:54.149600 paper_qa-4.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    62211 2024-04-14 16:42:43.000000 paper_qa-4.5.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:42:23.000000 paper_qa-4.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-18 05:44:19.291207 paper_qa-4.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-18 05:42:23.000000 paper_qa-4.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 05:42:23.000000 paper_qa-4.5.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 05:44:19.000000 paper_qa-4.5.2/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.287207 paper_qa-4.5.2/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.287207 paper_qa-4.5.2/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/llms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 05:42:23.000000 paper_qa-4.5.2/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-18 05:42:23.000000 paper_qa-4.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:44:19.291207 paper_qa-4.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:44:19.291207 paper_qa-4.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    63137 2024-04-18 05:42:23.000000 paper_qa-4.5.2/tests/test_paperqa.py
```

### Comparing `paper_qa-4.5.1/LICENSE` & `paper_qa-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/PKG-INFO` & `paper_qa-4.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.1
+Version: 4.5.2
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `paper_qa-4.5.1/README.md` & `paper_qa-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paper_qa.egg-info/PKG-INFO` & `paper_qa-4.5.2/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.1
+Version: 4.5.2
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `paper_qa-4.5.1/paperqa/__init__.py` & `paper_qa-4.5.2/paperqa/__init__.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paperqa/contrib/zotero.py` & `paper_qa-4.5.2/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paperqa/docs.py` & `paper_qa-4.5.2/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,15 +711,15 @@
             contexts + answer.contexts, key=lambda x: x.score, reverse=True
         )
         answer.contexts = answer.contexts[:max_sources]
         context_str = "\n\n".join(
             [
                 f"{c.text.name}: {c.context}"
                 + "".join([f"\n{k}: {v}" for k, v in c.model_extra.items()])
-                + (f". From {c.text.doc.citation}" if detailed_citations else "")
+                + (f"\nFrom {c.text.doc.citation}" if detailed_citations else "")
                 for c in answer.contexts
             ]
         )
 
         valid_names = [c.text.name for c in answer.contexts]
         context_str += "\n\nValid keys: " + ", ".join(valid_names)
         answer.context = context_str
```

### Comparing `paper_qa-4.5.1/paperqa/llms.py` & `paper_qa-4.5.2/paperqa/llms.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,15 +694,15 @@
     async def embed_documents(self, client: Any, texts: list[str]) -> list[list[float]]:
         return await client.aembed_documents(texts)
 
 
 class LangchainVectorStore(VectorStore):
     """A wrapper around the wrapper langchain.
 
-    Note that if you this is cleared (e.g., by `Docs` having `jit_texts_index` set to True),
+    Note that if this is cleared (e.g., by `Docs` having `jit_texts_index` set to True),
     this will calls the `from_texts` class method on the `store`. This means that any non-default
     constructor arguments will be lost. You can override the clear method on this class.
     """
 
     _store_builder: Any | None = None
     _store: Any | None = None
     # JIT Generics - store the class type (Doc or Text)
```

### Comparing `paper_qa-4.5.1/paperqa/prompts.py` & `paper_qa-4.5.2/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paperqa/readers.py` & `paper_qa-4.5.2/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paperqa/types.py` & `paper_qa-4.5.2/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/paperqa/utils.py` & `paper_qa-4.5.2/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper_qa-4.5.1/pyproject.toml` & `paper_qa-4.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     {email = "jamesbraza@gmail.com", name = "James Braza"},
     {email = "white.d.andrew@gmail.com", name = "Andrew White"},
 ]
 name = "paper-qa"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {repository = "https://github.com/whitead/paper-qa"}
-version = "4.5.1"
+version = "4.5.2"
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 # SEE: https://github.com/codespell-project/codespell/issues/1212#issuecomment-1744768533
 ignore-regex = ".{1024}|.*codespell-ignore.*"
 ignore-words-list = "aadd,ser"
```

### Comparing `paper_qa-4.5.1/tests/test_paperqa.py` & `paper_qa-4.5.2/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,15 +567,14 @@
     original_doc = next(iter(docs.docs.values()))
     assert (
         original_doc.embedding is not None
     ), "For downstream assertions of in-tact embedding, we need an embedding"
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
-    print(evidence.context)
     assert "Missouri" in evidence.context
     assert original_doc.embedding is not None, "Embedding should have remained in-tact"
     assert (
         evidence.contexts[0].text.doc.embedding is None
     ), "Embedding should have been removed"
 
     evidence = docs.get_evidence(
@@ -606,15 +605,14 @@
         summary_llm_model=summary_llm,
         llm_result_callback=print_callback,
     )
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")  # type: ignore[arg-type]
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
-    print(evidence.context)
     assert "Missouri" in evidence.context
 
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"),
         detailed_citations=True,
     )
     assert "From WikiMedia Foundation, 2023, Accessed now" in evidence.context
@@ -654,15 +652,14 @@
     )
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")  # type: ignore[arg-type]
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
     assert "person_name" in evidence.contexts[0].model_extra
     assert "person_name: " in evidence.context
-    print(evidence.context)
     answer = docs.query("What is Frederick Bates's greatest accomplishment?")
     assert "person_name" in answer.context
     os.remove(doc_path)
 
 
 def test_query():
     docs = Docs()
@@ -775,14 +772,20 @@
     assert docs.embedding.startswith("sparse")  # type: ignore[union-attr]
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     assert any(docs.docs["test"].embedding)  # type: ignore[arg-type]
+    assert all(
+        len(np.array(x.embedding).shape) == 1 for x in docs.docs.values()
+    ), "Embeddings should be 1D"
+    assert all(
+        len(np.array(x.embedding).shape) == 1 for x in docs.texts
+    ), "Embeddings should be 1D"
 
     # check the embeddings are the same size
     assert np.shape(docs.texts[0].embedding) == np.shape(docs.texts[1].embedding)
 
     # test alias
     docs = Docs(embedding="sparse")
     assert docs._embedding_client is None
@@ -1603,35 +1606,54 @@
         or "does not provide" in answer3.answer
         or "ambiguous" in answer3.answer
     )
 
 
 def test_add_texts():
     llm_config = {"temperature": 0.1, "model": "babbage-02"}
-    docs = Docs(llm_model=OpenAILLMModel(config=llm_config))
+    # want to use sparse embedding because
+    # we get some randomness in the OpenAI embeddings
+    docs = Docs(
+        llm_model=OpenAILLMModel(config=llm_config),
+        docs_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        texts_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        embedding_client=None,
+    )
+
     docs.add_url(
         "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
 
-    docs2 = Docs()
+    docs2 = Docs(
+        docs_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        texts_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        embedding_client=None,
+    )
     texts = [Text(**dict(t)) for t in docs.texts]
     for t in texts:
         t.embedding = None
     docs2.add_texts(texts, next(iter(docs.docs.values())))
 
     for t1, t2 in zip(docs2.texts, docs.texts):
         assert t1.text == t2.text
+        print(
+            "docs2", np.array(t1.embedding).shape, "docs", np.array(t2.embedding).shape
+        )
         assert np.allclose(t1.embedding, t2.embedding, atol=1e-3)
-
     docs2._build_texts_index()
     # now do it again to test after text index is already built
     llm_config = {"temperature": 0.1, "model": "babbage-02"}
-    docs = Docs(llm_model=OpenAILLMModel(config=llm_config))
+    docs = Docs(
+        llm_model=OpenAILLMModel(config=llm_config),
+        docs_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        texts_index=NumpyVectorStore(embedding_model=SparseEmbeddingModel()),
+        embedding_client=None,
+    )
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test3",
     )
 
     texts = [Text(**dict(t)) for t in docs.texts]
@@ -1682,15 +1704,14 @@
 def test_external_texts_index():
     docs = Docs(jit_texts_index=True)
     docs.add_url(
         "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
         citation="Flag Day of Canada, WikiMedia Foundation, 2023, Accessed now",
     )
     answer = docs.query(query="On which date is flag day annually observed?")
-    print(answer.model_dump())
     assert "February 15" in answer.answer
 
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
     )
```

