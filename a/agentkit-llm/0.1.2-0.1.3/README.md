# Comparing `tmp/agentkit-llm-0.1.2.tar.gz` & `tmp/agentkit-llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.2.tar", last modified: Mon Apr 15 17:41:55 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.3.tar", last modified: Thu Apr 18 03:00:39 2024, max compression
```

## Comparing `agentkit-llm-0.1.2.tar` & `agentkit-llm-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.2/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5522 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5058 2024-04-14 15:43:56.000000 agentkit-llm-0.1.2/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      929 2024-04-15 17:40:35.000000 agentkit-llm-0.1.2/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.2/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.2/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.2/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.2/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.2/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.2/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2661 2024-04-08 11:05:20.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4129 2024-04-08 11:05:36.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.2/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.2/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.2/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.2/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-15 17:41:55.670139 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     5522 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       26 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-15 17:41:55.000000 agentkit-llm-0.1.2/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:00:39.994719 agentkit-llm-0.1.3/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.3/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6370 2024-04-18 03:00:39.994719 agentkit-llm-0.1.3/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     5906 2024-04-18 03:00:10.000000 agentkit-llm-0.1.3/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-04-18 03:00:39.994719 agentkit-llm-0.1.3/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      929 2024-04-18 02:57:18.000000 agentkit-llm-0.1.3/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:00:39.990719 agentkit-llm-0.1.3/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:00:39.990719 agentkit-llm-0.1.3/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.3/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2799 2024-04-14 16:35:34.000000 agentkit-llm-0.1.3/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.3/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.3/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.3/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.3/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:00:39.990719 agentkit-llm-0.1.3/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2661 2024-04-08 11:05:20.000000 agentkit-llm-0.1.3/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.3/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3965 2024-04-08 11:05:44.000000 agentkit-llm-0.1.3/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4129 2024-04-08 11:05:36.000000 agentkit-llm-0.1.3/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1403 2024-04-08 11:05:05.000000 agentkit-llm-0.1.3/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.3/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.3/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.3/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-04-18 03:00:39.994719 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6370 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       26 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-04-18 03:00:39.000000 agentkit-llm-0.1.3/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.2/LICENSE` & `agentkit-llm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/PKG-INFO` & `agentkit-llm-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,16 +14,16 @@
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Structured LLM Reasoning with Dynamic Graphs**
 
 <!-- [[Website]](https://TODO.org) -->
-[[Arxiv Paper]](TODO)
-[[PDF]](TODO)
+[[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
+[[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
@@ -65,14 +65,15 @@
 # Getting Started
 
 The basic building block in AgentKit is a node, containing a natural language prompt for a specific subtask. The nodes are linked together by the dependency specifications, which specify the order of evaluation. Different arrangements of nodes can represent different different logic and throught processes.
 
 At inference time, AgentKit evaluates all nodes in specified order as a directed acyclic graph (DAG).
 
 ```python
+import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4")
 
 graph = Graph()
@@ -106,19 +107,35 @@
     'completion': $completion token counts,
 }
 ```
 
 # Using AgentKit without Programming Experience
 First, follow [the installation guide](#Installation) to install AgentKit.
 
+Then, run the following to evoke the command line interface (CLI):
+
+```bash
+git clone https://github.com/holmeswww/AgentKit && cd AgentKit
+cd examples/prompt_without_coding
+python generate_graph.py
+```
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
+
+You need to install openai and/or anthropic API in order to use their LLMs.
+See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
 
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
-TBD
+@article{wu2024agentkit,
+    title={AgentKit: Flow Engineering with Graphs, not Coding}, 
+    author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
+    year={2024},
+    journal={arXiv preprint arXiv:2404.11483}
+}
 ```
```

### Comparing `agentkit-llm-0.1.2/README.md` & `agentkit-llm-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Structured LLM Reasoning with Dynamic Graphs**
 
 <!-- [[Website]](https://TODO.org) -->
-[[Arxiv Paper]](TODO)
-[[PDF]](TODO)
+[[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
+[[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
@@ -51,14 +51,15 @@
 # Getting Started
 
 The basic building block in AgentKit is a node, containing a natural language prompt for a specific subtask. The nodes are linked together by the dependency specifications, which specify the order of evaluation. Different arrangements of nodes can represent different different logic and throught processes.
 
 At inference time, AgentKit evaluates all nodes in specified order as a directed acyclic graph (DAG).
 
 ```python
+import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4")
 
 graph = Graph()
@@ -92,19 +93,35 @@
     'completion': $completion token counts,
 }
 ```
 
 # Using AgentKit without Programming Experience
 First, follow [the installation guide](#Installation) to install AgentKit.
 
+Then, run the following to evoke the command line interface (CLI):
+
+```bash
+git clone https://github.com/holmeswww/AgentKit && cd AgentKit
+cd examples/prompt_without_coding
+python generate_graph.py
+```
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
+
+You need to install openai and/or anthropic API in order to use their LLMs.
+See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
 
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
-TBD
+@article{wu2024agentkit,
+    title={AgentKit: Flow Engineering with Graphs, not Coding}, 
+    author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
+    year={2024},
+    journal={arXiv preprint arXiv:2404.11483}
+}
 ```
```

### Comparing `agentkit-llm-0.1.2/setup.py` & `agentkit-llm-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 EXTRAS = {
     "logging": ["wandb"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
     version=VERSION,
```

### Comparing `agentkit-llm-0.1.2/src/agentkit/after_query.py` & `agentkit-llm-0.1.3/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/base_node.py` & `agentkit-llm-0.1.3/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.3/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/exceptions.py` & `agentkit-llm-0.1.3/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/graph.py` & `agentkit-llm-0.1.3/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.3/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/llm_api/__init__.py` & `agentkit-llm-0.1.3/src/agentkit/llm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.3/src/agentkit/llm_api/base.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.3/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.3/src/agentkit/llm_api/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/node.py` & `agentkit-llm-0.1.3/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit/utils.py` & `agentkit-llm-0.1.3/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.2/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.3/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A LLM prompting framework for LLM agents
 Home-page: https://github.com/Holmeswww/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -14,16 +14,16 @@
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Structured LLM Reasoning with Dynamic Graphs**
 
 <!-- [[Website]](https://TODO.org) -->
-[[Arxiv Paper]](TODO)
-[[PDF]](TODO)
+[[Arxiv Paper]](https://arxiv.org/abs/2404.11483)
+[[PDF]](https://arxiv.org/pdf/2404.11483.pdf)
 [[Docs]](https://agentkit.readthedocs.io/)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI](https://img.shields.io/pypi/v/agentkit-llm)](https://pypi.org/project/agentkit-llm/)
 [![PyPI Status](https://pepy.tech/badge/agentkit-llm)](https://pepy.tech/project/agentkit-llm)
 [![Docs](https://readthedocs.org/projects/agentkit/badge/?version=latest)](https://agentkit.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/holmeswww/agentkit)](https://github.com/holmeswww/AgentKit/blob/main/LICENSE)
@@ -65,14 +65,15 @@
 # Getting Started
 
 The basic building block in AgentKit is a node, containing a natural language prompt for a specific subtask. The nodes are linked together by the dependency specifications, which specify the order of evaluation. Different arrangements of nodes can represent different different logic and throught processes.
 
 At inference time, AgentKit evaluates all nodes in specified order as a directed acyclic graph (DAG).
 
 ```python
+import agentkit
 from agentkit import Graph, BaseNode
 
 import agentkit.llm_api
 
 LLM_API_FUNCTION = agentkit.llm_api.get_query("gpt-4")
 
 graph = Graph()
@@ -106,19 +107,35 @@
     'completion': $completion token counts,
 }
 ```
 
 # Using AgentKit without Programming Experience
 First, follow [the installation guide](#Installation) to install AgentKit.
 
+Then, run the following to evoke the command line interface (CLI):
+
+```bash
+git clone https://github.com/holmeswww/AgentKit && cd AgentKit
+cd examples/prompt_without_coding
+python generate_graph.py
+```
+![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/screenshot.png)
+
+You need to install openai and/or anthropic API in order to use their LLMs.
+See https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for installation guides.
 
 # Node Components
 
 ![](https://github.com/Holmeswww/AgentKit/raw/main/imgs/node_archi.png)
 Inside each node (as shown to the left of the figure), AgentKit runs a built-in flow that **preprocesses** the input (Compose), queryies the LLM with a preprocessed input and prompt $q_v$, and optionally **postprocesses** the output of the LLM (After-query).
 
 To support advanced capabilities such as branching, AgentKit offers API to dynamically modify the DAG at inference time (as shown to the right of the figure). Nodes/edges could be dynamically added or removed based on the LLM response at some ancestor nodes.
 
 # Citing AgentKit
 ```bibtex
-TBD
+@article{wu2024agentkit,
+    title={AgentKit: Flow Engineering with Graphs, not Coding}, 
+    author={Yue Wu and Yewen Fan and So Yeon Min and Shrimai Prabhumoye and Stephen McAleer and Yonatan Bisk and Ruslan Salakhutdinov and Yuanzhi Li and Tom Mitchell},
+    year={2024},
+    journal={arXiv preprint arXiv:2404.11483}
+}
 ```
```

### Comparing `agentkit-llm-0.1.2/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.3/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

