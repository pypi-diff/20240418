# Comparing `tmp/bbm25_haystack-0.1.3.tar.gz` & `tmp/bbm25_haystack-0.2.0.tar.gz`

## Comparing `bbm25_haystack-0.1.3.tar` & `bbm25_haystack-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/benchmarks/.gitkeep
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/scripts/benchmark_beir.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/__init__.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_retriever.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_store.py
--rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/default.model
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/filters.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/test_document_store.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/test_retriever.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/LICENSE
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/README.md
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/benchmarks/.gitkeep
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/scripts/benchmark_beir.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/__init__.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_retriever.py
+-rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_store.py
+-rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/default.model
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/filters.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/README.md
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/PKG-INFO
```

### Comparing `bbm25_haystack-0.1.3/.github/workflows/test.yml` & `bbm25_haystack-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/scripts/benchmark_beir.py` & `bbm25_haystack-0.2.0/scripts/benchmark_beir.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_retriever.py` & `bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_retriever.py`

 * *Files 7% similar despite different names*

```diff
@@ -111,18 +111,18 @@
         top_k = top_k or self.top_k
 
         _validate_search_params(filters, top_k)
 
         sim = self.document_store._retrieval(query, filters=filters, top_k=top_k)
 
         ret = []
-        for doc, score in sim:
+        for doc, scr in sim:
             data = doc.to_dict()
             if self.set_score:
-                data["score"] = score
+                data["score"] = scr
             ret.append(Document.from_dict(data))
 
         return {"documents": ret}
 
     def to_dict(self) -> dict[str, Any]:
         """
         Serializes the component to a dictionary.
```

### Comparing `bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_store.py` & `bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 # SPDX-FileCopyrightText: 2024-present Yuxuan Wang <wangy49@seas.upenn.edu>
 #
 # SPDX-License-Identifier: Apache-2.0
 import heapq
 import math
 import os
-from collections import Counter
+from collections import Counter, deque
+from collections.abc import Iterable
+from itertools import chain
 from typing import Any, Final, Optional, Union
 
+import pandas as pd
 from haystack import Document, default_from_dict, default_to_dict, logging
 from haystack.document_stores.errors import (
     DuplicateDocumentError,
     MissingDocumentError,
 )
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.utils.filters import document_matches_filter
 from sentencepiece import SentencePieceProcessor  # type: ignore
 
 from bbm25_haystack.filters import apply_filters_to_document
 
 logger = logging.getLogger(__name__)
 
 
+def _n_grams(seq: Iterable[str], n: int):
+    """
+    Returns a sliding window (of width n) over data from the iterable.
+
+    :param seq: the input token sequence.
+    :type seq: Iterable[str]
+    :param n: the window size.
+    :type n: int
+
+    :return: the n-gram window generator.
+    :rtype: Generator[tuple[str], None, None]
+    """
+    it = iter(seq)
+    wd = deque((next(it, None) for _ in range(n)), maxlen=n)
+
+    yield tuple(wd)
+    for el in it:
+        wd.append(el)
+        yield tuple(wd)
+
+
 class BetterBM25DocumentStore:
     """
     An in-memory document store intended to improve the default BM25 document
     store shipped with Haystack.
     """
 
     default_sp_file: Final = os.path.join(
@@ -34,14 +58,15 @@
     def __init__(
         self,
         *,
         k: float = 1.5,
         b: float = 0.75,
         delta: float = 1.0,
         sp_file: Optional[str] = None,
+        n_grams: Union[int, tuple[int, int]] = 1,
         haystack_filter_logic: bool = True,
     ) -> None:
         """
         Creates a new BetterBM25DocumentStore instance.
 
         An in-memory document store intended to improve the default
         BM25 document store shipped with Haystack. The default store
@@ -59,93 +84,138 @@
         :param b: the b parameter in BM25+ formula.
         :type b: float, optional
         :param delta: the delta parameter in BM25+ formula.
         :type delta: float, optional
         :param sp_file: the SentencePiece model file to use for
             tokenization.
         :type sp_file: Optional[str], optional
+        :param n_grams: the n-gram window size.
+        :type n_grams: Optional[Union[int, tuple[int, int]]], optional
         :param haystack_filter_logic: Whether to use the Haystack
             filter logic or the one implemented in this store,
             which is more conservative.
         :type haystack_filter_logic: bool, optional
         """
         self.k = k
         self.b = b
 
         # Adjust the delta value so that we can bring the `(k1 + 1)`
         # term out of the 'term frequency' term in BM25+ formula and
         # delete it; this will not affect the ranking
         self.delta = delta / (self.k + 1.0)
 
-        self._sp_file = sp_file
-        self._sp_inst = SentencePieceProcessor(
-            model_file=(self._sp_file or self.default_sp_file)
-        )
+        self._parse_sp_file(sp_file=sp_file)
+        self._parse_n_grams(n_grams=n_grams)
 
         self._haystack_filter_logic = haystack_filter_logic
         self._filter_func = (
             document_matches_filter
             if self._haystack_filter_logic
             else apply_filters_to_document
         )
 
         self._avg_doc_len: float = 0.0
         self._freq_doc: Counter = Counter()
-        self._index: dict[str, tuple[Document, dict[str, int], int]] = {}
+        self._index: dict[str, tuple[Document, dict[tuple[str], int], int]] = {}
+
+    def _parse_sp_file(self, sp_file: Optional[str]) -> None:
+        self._sp_file = sp_file
+
+        if sp_file is None:
+            self._sp_inst = SentencePieceProcessor(model_file=self.default_sp_file)
+            return
+
+        if not os.path.exists(sp_file) or not os.path.isfile(sp_file):
+            msg = (
+                f"Tokenizer model file '{sp_file}' not accessible; "
+                f"fallback to default {self.default_sp_file}."
+            )
+            logger.warn(msg)
+            self._sp_inst = SentencePieceProcessor(model_file=self.default_sp_file)
+            return
+
+        try:
+            self._sp_inst = SentencePieceProcessor(model_file=sp_file)
+        except Exception as exc:
+            msg = (
+                f"Failed to load tokenizer model file '{sp_file}': {exc}; "
+                f"fallback to default {self.default_sp_file}."
+            )
+            logger.error(msg)
+            self._sp_inst = SentencePieceProcessor(model_file=self.default_sp_file)
+
+    def _parse_n_grams(self, n_grams: Optional[Union[int, tuple[int, int]]]) -> None:
+        self._n_grams = n_grams
+
+        if isinstance(n_grams, int):
+            self._n_grams_min = 1
+            self._n_grams_max = n_grams
+            return
+
+        if isinstance(n_grams, tuple):
+            self._n_grams_min, self._n_grams_max = n_grams
+            if not all(isinstance(n, int) for n in n_grams):
+                msg = f"Invalid n-gram window size: {n_grams}."
+                raise ValueError(msg)
+            return
+
+        msg = f"Invalid n-gram window size: {n_grams}; expected int or tuple."
+        raise ValueError(msg)
 
-    def _tokenize(self, texts: Union[str, list[str]]) -> list[list[str]]:
+    def _tokenize(self, texts: Union[str, list[str]]) -> list[list[tuple[str]]]:
         """
         Tokenize input text using SentencePiece model.
 
         The input text can either be a single string or a list of strings,
-        such as a single user query or a group of raw document.
+        such as a single user query or a group of raw document. The tokenized
+        text will be augmented into set of n-grams based.
 
         :param texts: the input text to tokenize.
         :type texts: Union[str, list[str]]
 
-        :return: the tokenized text.
-        :rtype: list[list[str]]
-        """
-        if isinstance(texts, str):
-            texts = [texts]
-        return self._sp_inst.encode(texts, out_type=str)
-
-    def _compute_idf(self, tokens: list[str]) -> dict[str, float]:
+        :return: the tokenized text, with n-grams augmented.
+        :rtype: list[list[tuple[str]]]
         """
-        Calculate the inverse document frequency for each token.
 
-        :param tokens: the tokens to calculate the IDF for.
-        :type tokens: list[str]
+        def _augment_to_n_grams(tokens: list[str]) -> list[tuple[str]]:
+            it = (
+                _n_grams(tokens, n)
+                for n in range(self._n_grams_min, self._n_grams_max + 1)
+            )
+            return list(chain(*it))
 
-        :return: the IDF for each token.
-        :rtype: dict[str, float]
-        """
-        cnt = lambda token: self._freq_doc.get(token, 0)
-        idf = {
-            t: math.log(1 + (len(self._index) - cnt(t) + 0.5) / (cnt(t) + 0.5))
-            for t in tokens
-        }
-        return idf
+        if isinstance(texts, str):
+            texts = [texts]
+        return [
+            _augment_to_n_grams(tokens)
+            for tokens in self._sp_inst.encode(texts, out_type=str)
+        ]
 
     def _compute_bm25plus(
         self,
-        idf: dict[str, float],
+        query: str,
         documents: list[Document],
     ) -> list[tuple[Document, float]]:
         """
         Calculate the BM25+ score for all documents in this index.
 
-        :param idf: the IDF for each token.
-        :type idf: dict[str, float]
+        :param query: the query to calculate the BM25+ score for.
+        :type query: str
         :param documents: the pool of documents to calculate the BM25+ score for.
         :type documents: list[Document]
 
         :return: the BM25+ scores for all documents.
         :rtype: list[tuple[Document, float]]
         """
+        cnt = lambda ng: self._freq_doc.get(ng, 0)
+        idf = {
+            ng: math.log(1 + (len(self._index) - cnt(ng) + 0.5) / (cnt(ng) + 0.5))
+            for ng in self._tokenize(query)[0]
+        }
+
         sim = []
         for doc in documents:
             _, freq, doc_len = self._index[doc.id]
             doc_len_scaled = doc_len / self._avg_doc_len
 
             scr = 0.0
             for token, idf_val in idf.items():
@@ -179,17 +249,15 @@
         :return: the top-k documents and corresponding sim score.
         :rtype: list[tuple[Document, float]]
         """
         documents = self.filter_documents(filters)
         if not documents:
             return []
 
-        idf = self._compute_idf(self._tokenize(query)[0])
-        sim = self._compute_bm25plus(idf, documents)
-
+        sim = self._compute_bm25plus(query, documents)
         if top_k is None:
             return sorted(sim, key=lambda x: x[1], reverse=True)
         return heapq.nlargest(top_k, sim, key=lambda x: x[1])
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
@@ -257,15 +325,19 @@
 
                 # Overwrite if exists; delete first to keep the statistics consistent
                 logger.debug(
                     f"Document '{doc.id}' already exists in the store, overwriting."
                 )
                 self.delete_documents([doc.id])
 
-            tokens = self._tokenize(doc.content or "")[0]
+            content = doc.content or ""
+            if content == "" and isinstance(doc.dataframe, pd.DataFrame):
+                content = doc.dataframe.astype(str).to_csv(index=False)
+
+            tokens = self._tokenize(content)[0]
 
             self._index[doc.id] = (doc, Counter(tokens), len(tokens))
             self._freq_doc.update(set(tokens))
             self._avg_doc_len = (
                 len(tokens) + self._avg_doc_len * len(self._index)
             ) / (len(self._index) + 1)
 
@@ -313,14 +385,15 @@
         """Serializes this store to a dictionary."""
         return default_to_dict(
             self,
             k=self.k,
             b=self.b,
             delta=self.delta * (self.k + 1.0),  # Because we scaled it on init
             sp_file=self._sp_file,
+            n_grams=self._n_grams,
             haystack_filter_logic=self._haystack_filter_logic,
         )
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> "BetterBM25DocumentStore":
         """Deserializes the store from a dictionary."""
         return default_from_dict(cls, data)
```

### Comparing `bbm25_haystack-0.1.3/src/bbm25_haystack/default.model` & `bbm25_haystack-0.2.0/src/bbm25_haystack/default.model`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/src/bbm25_haystack/filters.py` & `bbm25_haystack-0.2.0/src/bbm25_haystack/filters.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/tests/test_document_store.py` & `bbm25_haystack-0.2.0/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/tests/test_retriever.py` & `bbm25_haystack-0.2.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/.gitignore` & `bbm25_haystack-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/LICENSE` & `bbm25_haystack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/README.md` & `bbm25_haystack-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/pyproject.toml` & `bbm25_haystack-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.3/PKG-INFO` & `bbm25_haystack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bbm25-haystack
-Version: 0.1.3
+Version: 0.2.0
 Summary: Haystack 2.x In-memory Document Store with Enhanced Efficiency
 Project-URL: Documentation, https://github.com/Guest400123064/bbm25-haystack#readme
 Project-URL: Issues, https://github.com/Guest400123064/bbm25-haystack/issues
 Project-URL: Source, https://github.com/Guest400123064/bbm25-haystack
 Author-email: Yuxuan Wang <wangy49@seas.upenn.edu>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

