# Comparing `tmp/bpm_ai-1.6.0.tar.gz` & `tmp/bpm_ai-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.6.0.tar", max compression
+gzip compressed data, was "bpm_ai-1.6.1.tar", max compression
```

## Comparing `bpm_ai-1.6.0.tar` & `bpm_ai-1.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      932 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1645 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3577 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      950 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     8786 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     8181 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4862 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     3044 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7530 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1631 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     3138 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/bpm_ai/translate/util.py
--rw-r--r--   0        0        0     1391 2024-04-16 22:19:46.385786 bpm_ai-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 bpm_ai-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1645 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3577 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4862 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7530 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1631 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     3138 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0      900 2024-04-18 11:51:28.716531 bpm_ai-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.6.1/PKG-INFO
```

### Comparing `bpm_ai-1.6.0/README.md` & `bpm_ai-1.6.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 # bpm-ai
 _AI task automation for BPM engines._
 
-See [camunda-8-connector-gpt](https://github.com/holunda-io/camunda-8-connector-gpt) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
+See [bpm-ai-connectors-camunda-8](https://github.com/holunda-io/bpm-ai-connectors-camunda-8) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
 
 ## Installation
 Requires Python 3.11.
-### Default
-```bash
-$ pip install bpm-ai
-```
 
-### For Local Inference
-Install PyTorch (remove index url for CUDA GPU support) and spaCy:
 ```bash
-$ pip install torch --index-url https://download.pytorch.org/whl/cpu
-$ pip install spacy
-```
-
-For Apple Silicon:
-```bash
-$ pip install torch spacy[apple]
+$ pip install bpm-ai
 ```
 
-Install bpm-ai with inference extra:
+## Development (install test dependencies)
+### Linux
+Install PyTorch (CPU) and spaCy:
 ```bash
-$ pip install bpm-ai[inference]
+$ pip install -r requirements.dev.txt
 ```
 
 ---
 
 ## License
 
 This project is developed under
```

### Comparing `bpm_ai-1.6.0/bpm_ai/common/multimodal.py` & `bpm_ai-1.6.1/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.6.1/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.6.1/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/compose/compose.py` & `bpm_ai-1.6.1/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/compose/util.py` & `bpm_ai-1.6.1/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.6.1/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.6.1/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/decide/decide.py` & `bpm_ai-1.6.1/bpm_ai/decide/decide.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/decide/schema.py` & `bpm_ai-1.6.1/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.6.1/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.6.1/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/extract/extract.py` & `bpm_ai-1.6.1/bpm_ai/extract/extract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/extract/util.py` & `bpm_ai-1.6.1/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.6.1/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.6.1/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/generic/generic.py` & `bpm_ai-1.6.1/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.6.1/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.6.1/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/translate/translate.py` & `bpm_ai-1.6.1/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/bpm_ai/translate/util.py` & `bpm_ai-1.6.1/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.6.0/PKG-INFO` & `bpm_ai-1.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.6.0
+Version: 1.6.1
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,47 +13,37 @@
 Requires-Dist: aiobotocore (>=2.12.3,<3.0.0)
 Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
 Requires-Dist: anthropic (>=0.25.2,<0.26.0)
 Requires-Dist: av (>=11.0.0,<12.0.0)
 Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
-Requires-Dist: bpm-ai-core (==2.4.1)
+Requires-Dist: bpm-ai-core (==2.4.2)
 Requires-Dist: langfuse (>=2.25.0,<3.0.0)
 Requires-Dist: openai (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
 
-See [camunda-8-connector-gpt](https://github.com/holunda-io/camunda-8-connector-gpt) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
+See [bpm-ai-connectors-camunda-8](https://github.com/holunda-io/bpm-ai-connectors-camunda-8) for actual integration with the Camunda Platform 8 BPM engine using custom BPMN elements (Connectors).
 
 ## Installation
 Requires Python 3.11.
-### Default
-```bash
-$ pip install bpm-ai
-```
 
-### For Local Inference
-Install PyTorch (remove index url for CUDA GPU support) and spaCy:
 ```bash
-$ pip install torch --index-url https://download.pytorch.org/whl/cpu
-$ pip install spacy
-```
-
-For Apple Silicon:
-```bash
-$ pip install torch spacy[apple]
+$ pip install bpm-ai
 ```
 
-Install bpm-ai with inference extra:
+## Development (install test dependencies)
+### Linux
+Install PyTorch (CPU) and spaCy:
 ```bash
-$ pip install bpm-ai[inference]
+$ pip install -r requirements.dev.txt
 ```
 
 ---
 
 ## License
 
 This project is developed under
```

