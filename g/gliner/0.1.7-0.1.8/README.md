# Comparing `tmp/gliner-0.1.7.tar.gz` & `tmp/gliner-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-0.1.7.tar", last modified: Tue Apr  9 17:35:12 2024, max compression
+gzip compressed data, was "gliner-0.1.8.tar", last modified: Thu Apr 18 19:50:27 2024, max compression
```

## Comparing `gliner-0.1.7.tar` & `gliner-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.239247 gliner-0.1.7/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.7/LICENSE
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9343 2024-04-09 17:35:12.238990 gliner-0.1.7/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8645 2024-04-09 17:32:05.000000 gliner-0.1.7/README.md
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.235698 gliner-0.1.7/gliner/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-03 11:51:52.000000 gliner-0.1.7/gliner/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.7/gliner/model.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.238479 gliner-0.1.7/gliner/modules/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.7/gliner/modules/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5991 2024-04-01 10:36:39.000000 gliner-0.1.7/gliner/modules/base.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/data_proc.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.7/gliner/modules/evaluator.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/layers.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.7/gliner/modules/run_evaluation.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.7/gliner/modules/span_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.7/gliner/modules/token_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.7/gliner/modules/token_splitter.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-09 17:35:12.238767 gliner-0.1.7/gliner.egg-info/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9343 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/SOURCES.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/dependency_links.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       85 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/requires.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-09 17:35:12.000000 gliner-0.1.7/gliner.egg-info/top_level.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1026 2024-03-28 17:31:49.000000 gliner-0.1.7/pyproject.toml
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-09 17:35:12.239301 gliner-0.1.7/setup.cfg
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.779560 gliner-0.1.8/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.8/LICENSE
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9531 2024-04-18 19:50:27.779284 gliner-0.1.8/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8806 2024-04-11 21:21:31.000000 gliner-0.1.8/README.md
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.775515 gliner-0.1.8/gliner/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-18 19:44:11.000000 gliner-0.1.8/gliner/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.8/gliner/model.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.778697 gliner-0.1.8/gliner/modules/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.8/gliner/modules/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5991 2024-04-01 10:36:39.000000 gliner-0.1.8/gliner/modules/base.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/data_proc.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.8/gliner/modules/evaluator.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/layers.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.8/gliner/modules/run_evaluation.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.8/gliner/modules/span_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.8/gliner/modules/token_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.8/gliner/modules/token_splitter.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-18 19:50:27.779013 gliner-0.1.8/gliner.egg-info/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9531 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/SOURCES.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/dependency_links.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/requires.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-18 19:50:27.000000 gliner-0.1.8/gliner.egg-info/top_level.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-18 19:46:25.000000 gliner-0.1.8/pyproject.toml
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-18 19:50:27.779614 gliner-0.1.8/setup.cfg
```

### Comparing `gliner-0.1.7/LICENSE` & `gliner-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/PKG-INFO` & `gliner-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: huggingface_hub>=0.21.4
 Requires-Dist: flair==0.13.1
+Requires-Dist: scipy<=1.12
 Requires-Dist: seqeval
 Requires-Dist: tqdm
 
 # 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- **[08/04]** - Some pretrained weights contained a **bug** which caused performance degradation. For now use base or multi versions.
+- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 🚀 `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
-- **GLiNER Small v2**: `urchade/gliner_smallv2` *(Apache 2.0)*
+- **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
+- **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
-- **GLiNER Medium v2**: `urchade/gliner_mediumv2` *(Apache 2.0)*
-- **GLiNER Medium v2.1**: `urchade/gliner_mediumv2.1` *(Apache 2.0)*
+- **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
+- **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
-- **GLiNER Large v2**: `urchade/gliner_largev2` *(Apache 2.0)*
+- **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
-- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)*
+- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
@@ -66,23 +68,23 @@
 
 After the installation of the GLiNER library, import the `GLiNER` class. Following this, you can load your chosen model with `GLiNER.from_pretrained` and utilize `predict_entities` to discern entities within your text.
 
 ```python
 from gliner import GLiNER
 
 # Initialize GLiNER with the base model
-model = GLiNER.from_pretrained("urchade/gliner_base")
+model = GLiNER.from_pretrained("urchade/gliner_medium-v2.1")
 
 # Sample text for entity prediction
 text = """
 Cristiano Ronaldo dos Santos Aveiro (Portuguese pronunciation: [kɾiʃˈtjɐnu ʁɔˈnaldu]; born 5 February 1985) is a Portuguese professional footballer who plays as a forward for and captains both Saudi Pro League club Al Nassr and the Portugal national team. Widely regarded as one of the greatest players of all time, Ronaldo has won five Ballon d'Or awards,[note 3] a record three UEFA Men's Player of the Year Awards, and four European Golden Shoes, the most by a European player. He has won 33 trophies in his career, including seven league titles, five UEFA Champions Leagues, the UEFA European Championship and the UEFA Nations League. Ronaldo holds the records for most appearances (183), goals (140) and assists (42) in the Champions League, goals in the European Championship (14), international goals (128) and international appearances (205). He is one of the few players to have made over 1,200 professional career appearances, the most by an outfield player, and has scored over 850 official senior career goals for club and country, making him the top goalscorer of all time.
 """
 
 # Labels for entity prediction
-labels = ["person", "award", "date", "competitions", "teams"]
+labels = ["Person", "Award", "Date", "Competitions", "Teams"] # for v2.1 use capital case for better performance
 
 # Perform entity prediction
 entities = model.predict_entities(text, labels, threshold=0.5)
 
 # Display predicted entities and their labels
 for entity in entities:
     print(entity["text"], "=>", entity["label"])
@@ -97,15 +99,14 @@
 Portugal national team => teams
 Ballon d'Or => award
 UEFA Men's Player of the Year Awards => award
 European Golden Shoes => award
 UEFA Champions Leagues => competitions
 UEFA European Championship => competitions
 UEFA Nations League => competitions
-Champions League => competitions
 European Championship => competitions
 ```
 
 ### 🔌 Usage with spaCy
 
 GLiNER can be seamlessly integrated with spaCy. To begin, install the `gliner-spacy` library via pip:
 
@@ -117,15 +118,15 @@
 
 ```python
 import spacy
 from gliner_spacy.pipeline import GlinerSpacy
 
 # Configuration for GLiNER integration
 custom_spacy_config = {
-    "gliner_model": "urchade/gliner_multi",
+    "gliner_model": "urchade/gliner_multi-v2.1",
     "chunk_size": 250,
     "labels": ["person", "organization", "email"],
     "style": "ent",
     "threshold": 0.3
 }
 
 # Initialize a blank English spaCy pipeline and add GLiNER
```

### Comparing `gliner-0.1.7/README.md` & `gliner-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- **[08/04]** - Some pretrained weights contained a **bug** which caused performance degradation. For now use base or multi versions.
+- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 🚀 `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
-- **GLiNER Small v2**: `urchade/gliner_smallv2` *(Apache 2.0)*
+- **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
+- **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
-- **GLiNER Medium v2**: `urchade/gliner_mediumv2` *(Apache 2.0)*
-- **GLiNER Medium v2.1**: `urchade/gliner_mediumv2.1` *(Apache 2.0)*
+- **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
+- **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
-- **GLiNER Large v2**: `urchade/gliner_largev2` *(Apache 2.0)*
+- **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
-- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)*
+- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
@@ -47,23 +48,23 @@
 
 After the installation of the GLiNER library, import the `GLiNER` class. Following this, you can load your chosen model with `GLiNER.from_pretrained` and utilize `predict_entities` to discern entities within your text.
 
 ```python
 from gliner import GLiNER
 
 # Initialize GLiNER with the base model
-model = GLiNER.from_pretrained("urchade/gliner_base")
+model = GLiNER.from_pretrained("urchade/gliner_medium-v2.1")
 
 # Sample text for entity prediction
 text = """
 Cristiano Ronaldo dos Santos Aveiro (Portuguese pronunciation: [kɾiʃˈtjɐnu ʁɔˈnaldu]; born 5 February 1985) is a Portuguese professional footballer who plays as a forward for and captains both Saudi Pro League club Al Nassr and the Portugal national team. Widely regarded as one of the greatest players of all time, Ronaldo has won five Ballon d'Or awards,[note 3] a record three UEFA Men's Player of the Year Awards, and four European Golden Shoes, the most by a European player. He has won 33 trophies in his career, including seven league titles, five UEFA Champions Leagues, the UEFA European Championship and the UEFA Nations League. Ronaldo holds the records for most appearances (183), goals (140) and assists (42) in the Champions League, goals in the European Championship (14), international goals (128) and international appearances (205). He is one of the few players to have made over 1,200 professional career appearances, the most by an outfield player, and has scored over 850 official senior career goals for club and country, making him the top goalscorer of all time.
 """
 
 # Labels for entity prediction
-labels = ["person", "award", "date", "competitions", "teams"]
+labels = ["Person", "Award", "Date", "Competitions", "Teams"] # for v2.1 use capital case for better performance
 
 # Perform entity prediction
 entities = model.predict_entities(text, labels, threshold=0.5)
 
 # Display predicted entities and their labels
 for entity in entities:
     print(entity["text"], "=>", entity["label"])
@@ -78,15 +79,14 @@
 Portugal national team => teams
 Ballon d'Or => award
 UEFA Men's Player of the Year Awards => award
 European Golden Shoes => award
 UEFA Champions Leagues => competitions
 UEFA European Championship => competitions
 UEFA Nations League => competitions
-Champions League => competitions
 European Championship => competitions
 ```
 
 ### 🔌 Usage with spaCy
 
 GLiNER can be seamlessly integrated with spaCy. To begin, install the `gliner-spacy` library via pip:
 
@@ -98,15 +98,15 @@
 
 ```python
 import spacy
 from gliner_spacy.pipeline import GlinerSpacy
 
 # Configuration for GLiNER integration
 custom_spacy_config = {
-    "gliner_model": "urchade/gliner_multi",
+    "gliner_model": "urchade/gliner_multi-v2.1",
     "chunk_size": 250,
     "labels": ["person", "organization", "email"],
     "style": "ent",
     "threshold": 0.3
 }
 
 # Initialize a blank English spaCy pipeline and add GLiNER
```

### Comparing `gliner-0.1.7/gliner/model.py` & `gliner-0.1.8/gliner/model.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/base.py` & `gliner-0.1.8/gliner/modules/base.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/data_proc.py` & `gliner-0.1.8/gliner/modules/data_proc.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/evaluator.py` & `gliner-0.1.8/gliner/modules/evaluator.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/layers.py` & `gliner-0.1.8/gliner/modules/layers.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/run_evaluation.py` & `gliner-0.1.8/gliner/modules/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/span_rep.py` & `gliner-0.1.8/gliner/modules/span_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/token_rep.py` & `gliner-0.1.8/gliner/modules/token_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner/modules/token_splitter.py` & `gliner-0.1.8/gliner/modules/token_splitter.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.7/gliner.egg-info/PKG-INFO` & `gliner-0.1.8/gliner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.0.0
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: huggingface_hub>=0.21.4
 Requires-Dist: flair==0.13.1
+Requires-Dist: scipy<=1.12
 Requires-Dist: seqeval
 Requires-Dist: tqdm
 
 # 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
-- **[08/04]** - Some pretrained weights contained a **bug** which caused performance degradation. For now use base or multi versions.
+- ⚙️ `pip install gliner==0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 🚀 `gliner_mediumv2.1` is available under the Apache 2.0 license. It should have similar performance as `gliner_base` and `gliner_medium`.
 - 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
-- **GLiNER Small v2**: `urchade/gliner_smallv2` *(Apache 2.0)*
+- **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
+- **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
-- **GLiNER Medium v2**: `urchade/gliner_mediumv2` *(Apache 2.0)*
-- **GLiNER Medium v2.1**: `urchade/gliner_mediumv2.1` *(Apache 2.0)*
+- **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
+- **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
-- **GLiNER Large v2**: `urchade/gliner_largev2` *(Apache 2.0)*
+- **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
-- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)*
+- **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
 - **Biomedical**: 🧬 `urchade/gliner_large_bio-v0.1` *(Apache 2.0)*
 
 ## 🛠 Installation & Usage
 
 To begin using the GLiNER model, first install the GLiNER Python library through pip:
@@ -66,23 +68,23 @@
 
 After the installation of the GLiNER library, import the `GLiNER` class. Following this, you can load your chosen model with `GLiNER.from_pretrained` and utilize `predict_entities` to discern entities within your text.
 
 ```python
 from gliner import GLiNER
 
 # Initialize GLiNER with the base model
-model = GLiNER.from_pretrained("urchade/gliner_base")
+model = GLiNER.from_pretrained("urchade/gliner_medium-v2.1")
 
 # Sample text for entity prediction
 text = """
 Cristiano Ronaldo dos Santos Aveiro (Portuguese pronunciation: [kɾiʃˈtjɐnu ʁɔˈnaldu]; born 5 February 1985) is a Portuguese professional footballer who plays as a forward for and captains both Saudi Pro League club Al Nassr and the Portugal national team. Widely regarded as one of the greatest players of all time, Ronaldo has won five Ballon d'Or awards,[note 3] a record three UEFA Men's Player of the Year Awards, and four European Golden Shoes, the most by a European player. He has won 33 trophies in his career, including seven league titles, five UEFA Champions Leagues, the UEFA European Championship and the UEFA Nations League. Ronaldo holds the records for most appearances (183), goals (140) and assists (42) in the Champions League, goals in the European Championship (14), international goals (128) and international appearances (205). He is one of the few players to have made over 1,200 professional career appearances, the most by an outfield player, and has scored over 850 official senior career goals for club and country, making him the top goalscorer of all time.
 """
 
 # Labels for entity prediction
-labels = ["person", "award", "date", "competitions", "teams"]
+labels = ["Person", "Award", "Date", "Competitions", "Teams"] # for v2.1 use capital case for better performance
 
 # Perform entity prediction
 entities = model.predict_entities(text, labels, threshold=0.5)
 
 # Display predicted entities and their labels
 for entity in entities:
     print(entity["text"], "=>", entity["label"])
@@ -97,15 +99,14 @@
 Portugal national team => teams
 Ballon d'Or => award
 UEFA Men's Player of the Year Awards => award
 European Golden Shoes => award
 UEFA Champions Leagues => competitions
 UEFA European Championship => competitions
 UEFA Nations League => competitions
-Champions League => competitions
 European Championship => competitions
 ```
 
 ### 🔌 Usage with spaCy
 
 GLiNER can be seamlessly integrated with spaCy. To begin, install the `gliner-spacy` library via pip:
 
@@ -117,15 +118,15 @@
 
 ```python
 import spacy
 from gliner_spacy.pipeline import GlinerSpacy
 
 # Configuration for GLiNER integration
 custom_spacy_config = {
-    "gliner_model": "urchade/gliner_multi",
+    "gliner_model": "urchade/gliner_multi-v2.1",
     "chunk_size": 250,
     "labels": ["person", "organization", "email"],
     "style": "ent",
     "threshold": 0.3
 }
 
 # Initialize a blank English spaCy pipeline and add GLiNER
```

### Comparing `gliner-0.1.7/pyproject.toml` & `gliner-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 ]
 
 dependencies = [
     "torch>=2.0.0",
     "transformers>=4.38.2",
     "huggingface_hub>=0.21.4",
     "flair==0.13.1",
+    "scipy<=1.12",
     "seqeval",
     "tqdm",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/urchade/GLiNER"
+Homepage = "https://github.com/urchade/GLiNER"
```

