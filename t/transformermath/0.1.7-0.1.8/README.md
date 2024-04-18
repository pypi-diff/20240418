# Comparing `tmp/transformermath-0.1.7.tar.gz` & `tmp/transformermath-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformermath-0.1.7.tar", last modified: Thu Apr 18 12:44:22 2024, max compression
+gzip compressed data, was "transformermath-0.1.8.tar", last modified: Thu Apr 18 12:46:34 2024, max compression
```

## Comparing `transformermath-0.1.7.tar` & `transformermath-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:44:22.969371 transformermath-0.1.7/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:44:22.969142 transformermath-0.1.7/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.7/README.md
--rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:44:22.969565 transformermath-0.1.7/setup.cfg
--rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:44:19.000000 transformermath-0.1.7/setup.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:44:22.966597 transformermath-0.1.7/transformermath/
--rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.7/transformermath/__init__.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.7/transformermath/attention_analyzer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)    11762 2024-04-18 12:44:13.000000 transformermath-0.1.7/transformermath/data_creator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3051 2024-04-18 12:38:26.000000 transformermath-0.1.7/transformermath/encoded_representations.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     2657 2024-04-18 12:44:07.000000 transformermath-0.1.7/transformermath/evaluator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1151 2024-04-18 12:43:54.000000 transformermath-0.1.7/transformermath/general_helper.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     7220 2024-04-18 12:31:59.000000 transformermath-0.1.7/transformermath/main.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1737 2024-04-18 12:43:47.000000 transformermath-0.1.7/transformermath/prober.py
--rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.7/transformermath/run_config.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.7/transformermath/run_device.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.7/transformermath/tokenizer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     4376 2024-04-18 12:34:47.000000 transformermath-0.1.7/transformermath/trainer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-18 12:34:51.000000 transformermath-0.1.7/transformermath/visualiser.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:44:22.968647 transformermath-0.1.7/transformermath.egg-info/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:44:22.000000 transformermath-0.1.7/transformermath.egg-info/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:44:22.000000 transformermath-0.1.7/transformermath.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:44:22.000000 transformermath-0.1.7/transformermath.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:44:22.000000 transformermath-0.1.7/transformermath.egg-info/requires.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:44:22.000000 transformermath-0.1.7/transformermath.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:46:34.975863 transformermath-0.1.8/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:46:34.975641 transformermath-0.1.8/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.8/README.md
+-rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:46:34.976033 transformermath-0.1.8/setup.cfg
+-rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:46:30.000000 transformermath-0.1.8/setup.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:46:34.973661 transformermath-0.1.8/transformermath/
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.8/transformermath/__init__.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.8/transformermath/attention_analyzer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)    11762 2024-04-18 12:44:13.000000 transformermath-0.1.8/transformermath/data_creator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3051 2024-04-18 12:38:26.000000 transformermath-0.1.8/transformermath/encoded_representations.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     2657 2024-04-18 12:44:07.000000 transformermath-0.1.8/transformermath/evaluator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1151 2024-04-18 12:43:54.000000 transformermath-0.1.8/transformermath/general_helper.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     7220 2024-04-18 12:31:59.000000 transformermath-0.1.8/transformermath/main.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1737 2024-04-18 12:43:47.000000 transformermath-0.1.8/transformermath/prober.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.8/transformermath/run_config.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 12:46:25.000000 transformermath-0.1.8/transformermath/run_device.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.8/transformermath/tokenizer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     4392 2024-04-18 12:46:19.000000 transformermath-0.1.8/transformermath/trainer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-18 12:34:51.000000 transformermath-0.1.8/transformermath/visualiser.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:46:34.975165 transformermath-0.1.8/transformermath.egg-info/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:46:34.000000 transformermath-0.1.8/transformermath.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:46:34.000000 transformermath-0.1.8/transformermath.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:46:34.000000 transformermath-0.1.8/transformermath.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:46:34.000000 transformermath-0.1.8/transformermath.egg-info/requires.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:46:34.000000 transformermath-0.1.8/transformermath.egg-info/top_level.txt
```

### Comparing `transformermath-0.1.7/transformermath/__init__.py` & `transformermath-0.1.8/transformermath/__init__.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/attention_analyzer.py` & `transformermath-0.1.8/transformermath/attention_analyzer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/data_creator.py` & `transformermath-0.1.8/transformermath/data_creator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/encoded_representations.py` & `transformermath-0.1.8/transformermath/encoded_representations.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/evaluator.py` & `transformermath-0.1.8/transformermath/evaluator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/general_helper.py` & `transformermath-0.1.8/transformermath/general_helper.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/main.py` & `transformermath-0.1.8/transformermath/main.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/prober.py` & `transformermath-0.1.8/transformermath/prober.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/run_config.py` & `transformermath-0.1.8/transformermath/run_config.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/run_device.py` & `transformermath-0.1.8/transformermath/run_device.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/tokenizer.py` & `transformermath-0.1.8/transformermath/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath/trainer.py` & `transformermath-0.1.8/transformermath/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
 import matplotlib.pyplot as plt
 from typing import List, Tuple, Any
-from model.minGPT    import *
+from transformermath.model.minGPT    import *
 from transformermath.run_device import RunDevice
 
 @dataclass
 class TrainModel:
     model: GPT
     epoch: int
```

### Comparing `transformermath-0.1.7/transformermath/visualiser.py` & `transformermath-0.1.8/transformermath/visualiser.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.7/transformermath.egg-info/SOURCES.txt` & `transformermath-0.1.8/transformermath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

