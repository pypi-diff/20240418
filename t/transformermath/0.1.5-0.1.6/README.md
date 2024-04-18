# Comparing `tmp/transformermath-0.1.5.tar.gz` & `tmp/transformermath-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformermath-0.1.5.tar", last modified: Thu Apr 18 12:35:02 2024, max compression
+gzip compressed data, was "transformermath-0.1.6.tar", last modified: Thu Apr 18 12:41:55 2024, max compression
```

## Comparing `transformermath-0.1.5.tar` & `transformermath-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:35:02.617163 transformermath-0.1.5/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:35:02.616951 transformermath-0.1.5/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.5/README.md
--rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:35:02.617365 transformermath-0.1.5/setup.cfg
--rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:34:58.000000 transformermath-0.1.5/setup.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:35:02.614989 transformermath-0.1.5/transformermath/
--rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.5/transformermath/__init__.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.5/transformermath/attention_analyzer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)    11762 2024-04-18 12:34:23.000000 transformermath-0.1.5/transformermath/data_creator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.5/transformermath/encoded_representations.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.5/transformermath/evaluator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.5/transformermath/general_helper.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     7220 2024-04-18 12:31:59.000000 transformermath-0.1.5/transformermath/main.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.5/transformermath/prober.py
--rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.5/transformermath/run_config.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.5/transformermath/run_device.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.5/transformermath/tokenizer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     4376 2024-04-18 12:34:47.000000 transformermath-0.1.5/transformermath/trainer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-18 12:34:51.000000 transformermath-0.1.5/transformermath/visualiser.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:35:02.616485 transformermath-0.1.5/transformermath.egg-info/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:35:02.000000 transformermath-0.1.5/transformermath.egg-info/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:35:02.000000 transformermath-0.1.5/transformermath.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:35:02.000000 transformermath-0.1.5/transformermath.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:35:02.000000 transformermath-0.1.5/transformermath.egg-info/requires.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:35:02.000000 transformermath-0.1.5/transformermath.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:41:55.050162 transformermath-0.1.6/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:41:55.049947 transformermath-0.1.6/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.6/README.md
+-rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:41:55.050328 transformermath-0.1.6/setup.cfg
+-rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:40:18.000000 transformermath-0.1.6/setup.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:41:55.047659 transformermath-0.1.6/transformermath/
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.6/transformermath/__init__.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.6/transformermath/attention_analyzer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)    11762 2024-04-18 12:34:23.000000 transformermath-0.1.6/transformermath/data_creator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3051 2024-04-18 12:38:26.000000 transformermath-0.1.6/transformermath/encoded_representations.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.6/transformermath/evaluator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1135 2024-04-18 12:37:26.000000 transformermath-0.1.6/transformermath/general_helper.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     7220 2024-04-18 12:31:59.000000 transformermath-0.1.6/transformermath/main.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.6/transformermath/prober.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.6/transformermath/run_config.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.6/transformermath/run_device.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.6/transformermath/tokenizer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     4376 2024-04-18 12:34:47.000000 transformermath-0.1.6/transformermath/trainer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-18 12:34:51.000000 transformermath-0.1.6/transformermath/visualiser.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:41:55.049433 transformermath-0.1.6/transformermath.egg-info/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:41:55.000000 transformermath-0.1.6/transformermath.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:41:55.000000 transformermath-0.1.6/transformermath.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:41:55.000000 transformermath-0.1.6/transformermath.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:41:55.000000 transformermath-0.1.6/transformermath.egg-info/requires.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:41:55.000000 transformermath-0.1.6/transformermath.egg-info/top_level.txt
```

### Comparing `transformermath-0.1.5/transformermath/__init__.py` & `transformermath-0.1.6/transformermath/__init__.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/attention_analyzer.py` & `transformermath-0.1.6/transformermath/attention_analyzer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/data_creator.py` & `transformermath-0.1.6/transformermath/data_creator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/encoded_representations.py` & `transformermath-0.1.6/transformermath/encoded_representations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from dataclasses import dataclass
-
+from typing import List
 
 @dataclass
 class TokenRepresentation:
     encoded_token: int
-    token_embedding_representation: list[int]
-    encoded_sequence: list[int]
+    token_embedding_representation: List[int]
+    encoded_sequence: List[int]
     token_position_in_sequence: int
 
 @dataclass
 class SequenceRepresentation:
-    pooled_representation: list[float]
-    encoded_sequence: list[int]
+    pooled_representation: List[float]
+    encoded_sequence: List[int]
 
 class EncodedRepresentations:
     def __init__(self) -> None:
         pass
 
     """
     Gets the transformed output pooled-sequence
```

### Comparing `transformermath-0.1.5/transformermath/evaluator.py` & `transformermath-0.1.6/transformermath/evaluator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/general_helper.py` & `transformermath-0.1.6/transformermath/general_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
 import torch
 from run_device import RunDevice
-
+from typing import List, Tuple
 
 class GeneralHelper:
     def __init__(self) -> None:
         self.device = RunDevice().get_device()
 
     def load_model(self, model_path:str):
         model = torch.load(model_path)
         model.eval()
         return model
     
-    def tensor_data(self, input_data: list, labels: list) -> tuple:
+    def tensor_data(self, input_data: List, labels: List) -> Tuple:
         TX = torch.tensor(input_data, dtype=torch.long).to(self.device)
         TY = torch.tensor(labels, dtype=torch.long).to(self.device)
         return TX, TY
     
     def decode_examples(self, examples, replacer):
         decoded_examples = []
         inv_token_encodings = {v: k for k, v in replacer.items()}
```

### Comparing `transformermath-0.1.5/transformermath/main.py` & `transformermath-0.1.6/transformermath/main.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/prober.py` & `transformermath-0.1.6/transformermath/prober.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/run_config.py` & `transformermath-0.1.6/transformermath/run_config.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/run_device.py` & `transformermath-0.1.6/transformermath/run_device.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/tokenizer.py` & `transformermath-0.1.6/transformermath/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/trainer.py` & `transformermath-0.1.6/transformermath/trainer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath/visualiser.py` & `transformermath-0.1.6/transformermath/visualiser.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.5/transformermath.egg-info/SOURCES.txt` & `transformermath-0.1.6/transformermath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

