# Comparing `tmp/langchain_cohere-0.1.3rc1.tar.gz` & `tmp/langchain_cohere-0.1.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.3rc1.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.4rc0.tar", max compression
```

## Comparing `langchain_cohere-0.1.3rc1.tar` & `langchain_cohere-0.1.4rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/LICENSE
--rw-r--r--   0        0        0     5585 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/README.md
--rw-r--r--   0        0        0      608 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    17262 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8173 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1215 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/common.py
--rw-r--r--   0        0        0     5813 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8058 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3349 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4899 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4060 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    10981 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9694 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     4134 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2682 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/LICENSE
+-rw-r--r--   0        0        0     5585 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/README.md
+-rw-r--r--   0        0        0      608 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    17262 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8173 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1585 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5813 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8058 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3349 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4913 2024-04-18 18:09:53.761207 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4060 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    11351 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9728 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     4134 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2682 2024-04-18 18:09:53.765208 langchain_cohere-0.1.4rc0/pyproject.toml
+-rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.4rc0/PKG-INFO
```

### Comparing `langchain_cohere-0.1.3rc1/LICENSE` & `langchain_cohere-0.1.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/README.md` & `langchain_cohere-0.1.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/__init__.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/cohere_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/llms.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/rag_retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Cohere multi-hop agent enables multiple tools to be used in sequence to complete a
     task.
 
     This agent uses a multi hop prompt by Cohere, which is experimental and subject
     to change. The latest prompt can be used by upgrading the langchain-cohere package.
 """
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
+from typing import Any, Dict, List, MutableMapping, Optional, Sequence, Union
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import (
     Runnable,
     RunnableConfig,
@@ -118,15 +118,15 @@
         if not isinstance(agent_steps, AgentFinish):
             # We're not on the AgentFinish step.
             return agent_steps
         agent_finish = agent_steps
 
         # Build a list of documents from the intermediate_steps used in this chain.
         intermediate_steps = input.get("chain_input", {}).get("intermediate_steps", [])
-        documents: List[Mapping] = []
+        documents: List[MutableMapping] = []
         for _, observation in intermediate_steps:
             documents.extend(convert_to_documents(observation))
 
         # Build a list of citations, if any, from the documents + grounded answer.
         grounded_answer = agent_finish.return_values.pop(GROUNDED_ANSWER_KEY, "")
         output, citations = parse_citations(
             grounded_answer=grounded_answer, documents=documents
```

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 import re
-from typing import Any, Dict, List, Mapping, Tuple, Union
+from typing import Any, Dict, List, Mapping, MutableMapping, Tuple, Union
 
 from langchain_core.agents import AgentAction, AgentActionMessageLog, AgentFinish
 from langchain_core.messages import AIMessage
 from langchain_core.output_parsers import BaseOutputParser
 
 from langchain_cohere import CohereCitation
 
@@ -159,48 +159,55 @@
         logging.error(f"Error: {e}")
 
     parsed_actions = parse_jsonified_tool_use_generation(actions, "Action:")
     return generation, plan, parsed_actions
 
 
 def parse_citations(
-    grounded_answer: str, documents: List[Mapping]
+    grounded_answer: str, documents: List[MutableMapping]
 ) -> Tuple[str, List[CohereCitation]]:
     """
     Parses a grounded_generation (from parse_actions) and documents (from
     convert_to_documents) into a (generation, CohereCitation list) tuple.
     """
 
     no_markup_answer, parsed_answer = _parse_answer_spans(grounded_answer)
     citations: List[CohereCitation] = []
     start = 0
 
+    # Add an id field to each document. This may be useful for future deduplication.
+    for i in range(len(documents)):
+        documents[i]["id"] = documents[i].get("id") or f"doc_{i}"
+
     for answer in parsed_answer:
         text = answer.get("text", "")
         document_indexes = answer.get("cited_docs")
         if not document_indexes:
             # There were no citations for this piece of text.
             start += len(text)
             continue
         end = start + len(text)
 
         # Look up the cited document by index
         cited_documents: List[Mapping] = []
+        cited_document_ids: List[str] = []
         for index in set(document_indexes):
             if index >= len(documents):
                 # The document index doesn't exist
                 continue
             cited_documents.append(documents[index])
+            cited_document_ids.append(documents[index]["id"])
 
         citations.append(
             CohereCitation(
                 start=start,
                 end=end,
                 text=text,
                 documents=cited_documents,
+                document_ids=set(cited_document_ids),
             )
         )
         start = end
 
     return no_markup_answer, citations
```

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/react_multi_hop/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Mapping,
+    MutableMapping,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
 from langchain_core.agents import AgentAction, AgentActionMessageLog
@@ -135,17 +136,17 @@
 
     prompt_content = "<results>\n" + "\n\n".join(rendered_documents) + "\n</results>"
     return SystemMessage(content=prompt_content), index
 
 
 def convert_to_documents(
     observations: Any,
-) -> List[Mapping]:
+) -> List[MutableMapping]:
     """Converts observations into a 'document' dict"""
-    documents: List[Mapping] = []
+    documents: List[MutableMapping] = []
     if isinstance(observations, str):
         # strings are turned into a key/value pair and a key of 'output' is added.
         observations = [{"output": observations}]
     elif isinstance(observations, Mapping):
         # single mappings are transformed into a list to simplify the rest of the code.
         observations = [observations]
     elif not isinstance(observations, Sequence):
```

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/rerank.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/langchain_cohere/utils.py` & `langchain_cohere-0.1.4rc0/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc1/pyproject.toml` & `langchain_cohere-0.1.4rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.3rc1"
+version = "0.1.4rc0"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_cohere-0.1.3rc1/PKG-INFO` & `langchain_cohere-0.1.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-cohere
-Version: 0.1.3rc1
+Version: 0.1.4rc0
 Summary: An integration package connecting Cohere and LangChain
 Home-page: https://github.com/langchain-ai/langchain-cohere
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

