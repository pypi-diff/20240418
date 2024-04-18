# Comparing `tmp/transformermath-0.1.2.tar.gz` & `tmp/transformermath-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformermath-0.1.2.tar", last modified: Thu Apr 18 12:05:44 2024, max compression
+gzip compressed data, was "transformermath-0.1.3.tar", last modified: Thu Apr 18 12:26:22 2024, max compression
```

## Comparing `transformermath-0.1.2.tar` & `transformermath-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.577506 transformermath-0.1.2/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:05:44.577275 transformermath-0.1.2/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.2/README.md
--rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:05:44.577607 transformermath-0.1.2/setup.cfg
--rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:05:18.000000 transformermath-0.1.2/setup.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.575345 transformermath-0.1.2/transformermath/
--rw-r--r--   0 aaronkher   (501) staff       (20)     1034 2024-04-18 11:33:41.000000 transformermath-0.1.2/transformermath/__init__.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.2/transformermath/attention_analyzer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)    11771 2024-04-18 05:00:26.000000 transformermath-0.1.2/transformermath/data_creator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.2/transformermath/encoded_representations.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.2/transformermath/evaluator.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.2/transformermath/general_helper.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     6874 2024-04-18 11:29:41.000000 transformermath-0.1.2/transformermath/main.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.2/transformermath/prober.py
--rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.2/transformermath/run_config.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.2/transformermath/run_device.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.2/transformermath/tokenizer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.2/transformermath/trainer.py
--rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.2/transformermath/visualiser.py
-drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:05:44.576891 transformermath-0.1.2/transformermath.egg-info/
--rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/PKG-INFO
--rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/SOURCES.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/dependency_links.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/requires.txt
--rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:05:44.000000 transformermath-0.1.2/transformermath.egg-info/top_level.txt
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.533014 transformermath-0.1.3/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:26:22.532724 transformermath-0.1.3/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)        0 2024-04-18 07:27:06.000000 transformermath-0.1.3/README.md
+-rw-r--r--   0 aaronkher   (501) staff       (20)       38 2024-04-18 12:26:22.533194 transformermath-0.1.3/setup.cfg
+-rw-r--r--   0 aaronkher   (501) staff       (20)      405 2024-04-18 12:26:17.000000 transformermath-0.1.3/setup.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.530440 transformermath-0.1.3/transformermath/
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1214 2024-04-18 12:22:33.000000 transformermath-0.1.3/transformermath/__init__.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3614 2024-04-18 04:30:10.000000 transformermath-0.1.3/transformermath/attention_analyzer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)    11771 2024-04-18 05:00:26.000000 transformermath-0.1.3/transformermath/data_creator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3028 2024-04-17 05:02:27.000000 transformermath-0.1.3/transformermath/encoded_representations.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     2641 2024-04-18 07:29:13.000000 transformermath-0.1.3/transformermath/evaluator.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1105 2024-04-18 07:35:28.000000 transformermath-0.1.3/transformermath/general_helper.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     7209 2024-04-18 12:26:07.000000 transformermath-0.1.3/transformermath/main.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1721 2024-04-18 11:40:36.000000 transformermath-0.1.3/transformermath/prober.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)      757 2024-03-06 06:47:30.000000 transformermath-0.1.3/transformermath/run_config.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1080 2024-04-18 10:52:53.000000 transformermath-0.1.3/transformermath/run_device.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     1305 2024-04-18 04:52:17.000000 transformermath-0.1.3/transformermath/tokenizer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     4360 2024-04-18 10:44:56.000000 transformermath-0.1.3/transformermath/trainer.py
+-rw-r--r--   0 aaronkher   (501) staff       (20)     3589 2024-04-17 05:09:03.000000 transformermath-0.1.3/transformermath/visualiser.py
+drwxr-xr-x   0 aaronkher   (501) staff       (20)        0 2024-04-18 12:26:22.532063 transformermath-0.1.3/transformermath.egg-info/
+-rw-r--r--   0 aaronkher   (501) staff       (20)       59 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/PKG-INFO
+-rw-r--r--   0 aaronkher   (501) staff       (20)      612 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/SOURCES.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)        1 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/dependency_links.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)      141 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/requires.txt
+-rw-r--r--   0 aaronkher   (501) staff       (20)       16 2024-04-18 12:26:22.000000 transformermath-0.1.3/transformermath.egg-info/top_level.txt
```

### Comparing `transformermath-0.1.2/transformermath/__init__.py` & `transformermath-0.1.3/transformermath/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     get_sequence_embedding_representations,
     visualise_sequence_embeddings,
     visualise_token_embeddings,
     plot_explained_variance,
     display_attention_map,
     display_average_attention_map,
     display_attention_distributional_histogram,
-    perform_distributional_significance_tests
+    perform_distributional_significance_tests,
+    get_addition_tokenizer,
+    get_sequence_tokenizer,
+    get_subtraction_tokenizer
 )
 
 __all__ = [
     'train',
     'generate_addition_data',
     'generate_subtraction_data',
     'generate_sequence_data',
@@ -27,9 +30,12 @@
     'get_sequence_embedding_representations',
     'visualise_sequence_embeddings',
     'visualise_token_embeddings',
     'plot_explained_variance',
     'display_attention_map',
     'display_average_attention_map',
     'display_attention_distributional_histogram',
-    'perform_distributional_significance_tests'
+    'perform_distributional_significance_tests',
+    'get_addition_tokenizer',
+    'get_sequence_tokenizer',
+    'get_subtraction_tokenizer'
 ]
```

### Comparing `transformermath-0.1.2/transformermath/attention_analyzer.py` & `transformermath-0.1.3/transformermath/attention_analyzer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/data_creator.py` & `transformermath-0.1.3/transformermath/data_creator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/encoded_representations.py` & `transformermath-0.1.3/transformermath/encoded_representations.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/evaluator.py` & `transformermath-0.1.3/transformermath/evaluator.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/general_helper.py` & `transformermath-0.1.3/transformermath/general_helper.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/main.py` & `transformermath-0.1.3/transformermath/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from transformermath.attention_analyzer import AttentionAnalyzer
 from transformermath.data_creator import DataCreator
 from transformermath.encoded_representations import EncodedRepresentations
 from transformermath.evaluator import Evaluator
 from transformermath.prober import Prober
+from transformermath.tokenizer import AdditionTokenizer, SequencesTokenizer, SubtractionTokenizer
 from transformermath.trainer import Trainer
 from transformermath.visualiser import Visualiser
 
 
 """
 Data creation methods
 """
@@ -116,17 +117,27 @@
 def display_attention_distributional_histogram(attention_weights_ID, attention_weights_OOD, layer, head, tokenizer):
     attention_analyzer = AttentionAnalyzer(tokenizer=tokenizer) 
     ID_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_ID, layer=layer,head=head)
     OOD_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_OOD,layer=layer,head=head)
     attention_analyzer.plot_attention_weight_histogram(ID_values=ID_weights,OOD_values=OOD_weights)
 
 
-def perform_distributional_significance_tests(attention_weights_ID, attention_weights_OOD, layer, head, tokenizer)
+def perform_distributional_significance_tests(attention_weights_ID, attention_weights_OOD, layer, head, tokenizer):
     attention_analyzer = AttentionAnalyzer(tokenizer=tokenizer) 
-    ID_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_ID,layer=0,head=0)
-    OOD_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_OOD,layer=0,head=0)
+    ID_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_ID,layer=layer,head=head)
+    OOD_weights = attention_analyzer.flatten_attention_weights(attention_maps=attention_weights_OOD,layer=layer,head=head)
 
     ks_statistic, ks_p_value = attention_analyzer.compare_attention_maps_ks(values_1=ID_weights,values_2=OOD_weights)
     cosine_sim = attention_analyzer.compare_attention_maps_cosine_similarity(values_1=ID_weights,values_2=OOD_weights)
     energy_distance = attention_analyzer.compare_attention_maps_energy_distance(values_1=ID_weights,values_2=OOD_weights)
 
-    return ks_statistic, ks_p_value, cosine_sim, energy_distance
+    return ks_statistic, ks_p_value, cosine_sim, energy_distance
+
+
+def get_addition_tokenizer():
+    return AdditionTokenizer().REPLACER
+
+def get_sequence_tokenizer():
+    return SequencesTokenizer().REPLACER
+
+def get_subtraction_tokenizer():
+    return SubtractionTokenizer().REPLACER
```

### Comparing `transformermath-0.1.2/transformermath/prober.py` & `transformermath-0.1.3/transformermath/prober.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/run_config.py` & `transformermath-0.1.3/transformermath/run_config.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/run_device.py` & `transformermath-0.1.3/transformermath/run_device.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/tokenizer.py` & `transformermath-0.1.3/transformermath/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/trainer.py` & `transformermath-0.1.3/transformermath/trainer.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath/visualiser.py` & `transformermath-0.1.3/transformermath/visualiser.py`

 * *Files identical despite different names*

### Comparing `transformermath-0.1.2/transformermath.egg-info/SOURCES.txt` & `transformermath-0.1.3/transformermath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

