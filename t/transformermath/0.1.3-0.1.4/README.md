# Comparing `tmp/transformermath-0.1.3.tar.gz` & `tmp/transformermath-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformermath-0.1.3.tar", last modified: Thu Apr 18 12:26:22 2024, max compression
+gzip compressed data, was "transformermath-0.1.4.tar", last modified: Thu Apr 18 12:32:15 2024, max compression
```

## Comparing `transformermath-0.1.3.tar` & `transformermath-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.533014 transformermath-0.1.3/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:26:22.532724 transformermath-0.1.3/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.3/README.md
--rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:26:22.533194 transformermath-0.1.3/setup.cfg
--rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:26:17.000000 transformermath-0.1.3/setup.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.530440 transformermath-0.1.3/transformermath/
--rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.3/transformermath/__init__.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.3/transformermath/attention_analyzer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)    11771 2024-04-18 05:00:26.000000 transformermath-0.1.3/transformermath/data_creator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.3/transformermath/encoded_representations.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.3/transformermath/evaluator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.3/transformermath/general_helper.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     7209 2024-04-18 12:26:07.000000 transformermath-0.1.3/transformermath/main.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.3/transformermath/prober.py
--rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.3/transformermath/run_config.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.3/transformermath/run_device.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.3/transformermath/tokenizer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.3/transformermath/trainer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.3/transformermath/visualiser.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.532063 transformermath-0.1.3/transformermath.egg-info/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/requires.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:32:15.719791 transformermath-0.1.4/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:32:15.719557 transformermath-0.1.4/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.4/README.md
+-rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:32:15.719964 transformermath-0.1.4/setup.cfg
+-rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:32:08.000000 transformermath-0.1.4/setup.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:32:15.717483 transformermath-0.1.4/transformermath/
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.4/transformermath/__init__.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.4/transformermath/attention_analyzer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)    11746 2024-04-18 12:29:06.000000 transformermath-0.1.4/transformermath/data_creator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.4/transformermath/encoded_representations.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.4/transformermath/evaluator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.4/transformermath/general_helper.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     7220 2024-04-18 12:31:59.000000 transformermath-0.1.4/transformermath/main.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.4/transformermath/prober.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.4/transformermath/run_config.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.4/transformermath/run_device.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.4/transformermath/tokenizer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.4/transformermath/trainer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.4/transformermath/visualiser.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:32:15.719080 transformermath-0.1.4/transformermath.egg-info/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:32:15.000000 transformermath-0.1.4/transformermath.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:32:15.000000 transformermath-0.1.4/transformermath.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:32:15.000000 transformermath-0.1.4/transformermath.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:32:15.000000 transformermath-0.1.4/transformermath.egg-info/requires.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:32:15.000000 transformermath-0.1.4/transformermath.egg-info/top_level.txt
```

### Comparing `transformermath-0.1.3/transformermath/__init__.py` & `transformermath-0.1.4/transformermath/__init__.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/attention_analyzer.py` & `transformermath-0.1.4/transformermath/attention_analyzer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/data_creator.py` & `transformermath-0.1.4/transformermath/data_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import random
 from typing import Any, List
 import numpy as np
 import pandas as pd
 from dataclasses import asdict, dataclass
-from tokenizer import AdditionTokenizer, MultiplicationTokenizer, SubtractionTokenizer, SequencesTokenizer
+from tokenizer import AdditionTokenizer, SubtractionTokenizer, SequencesTokenizer
 import copy
 
 
 # A + B = C
 @dataclass
 class ArithmeticItem:
     A: int
```

### Comparing `transformermath-0.1.3/transformermath/encoded_representations.py` & `transformermath-0.1.4/transformermath/encoded_representations.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/evaluator.py` & `transformermath-0.1.4/transformermath/evaluator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/general_helper.py` & `transformermath-0.1.4/transformermath/general_helper.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/main.py` & `transformermath-0.1.4/transformermath/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from transformermath.attention_analyzer import AttentionAnalyzer
 from transformermath.data_creator import DataCreator
 from transformermath.encoded_representations import EncodedRepresentations
 from transformermath.evaluator import Evaluator
 from transformermath.prober import Prober
-from transformermath.tokenizer import AdditionTokenizer, SequencesTokenizer, SubtractionTokenizer
+from transformermath.tokenizer import Tokenizer, AdditionTokenizer, SequencesTokenizer, SubtractionTokenizer
 from transformermath.trainer import Trainer
 from transformermath.visualiser import Visualiser
 
 
 """
 Data creation methods
 """
```

### Comparing `transformermath-0.1.3/transformermath/prober.py` & `transformermath-0.1.4/transformermath/prober.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/run_config.py` & `transformermath-0.1.4/transformermath/run_config.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/run_device.py` & `transformermath-0.1.4/transformermath/run_device.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/tokenizer.py` & `transformermath-0.1.4/transformermath/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/trainer.py` & `transformermath-0.1.4/transformermath/trainer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath/visualiser.py` & `transformermath-0.1.4/transformermath/visualiser.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.3/transformermath.egg-info/SOURCES.txt` & `transformermath-0.1.4/transformermath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

