# Comparing `tmp/kdp-1.4.0.tar.gz` & `tmp/kdp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-1.4.0.tar", max compression
+gzip compressed data, was "kdp-1.5.0.tar", max compression
```

## Comparing `kdp-1.4.0.tar` & `kdp-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-04-15 11:27:26.891808 kdp-1.4.0/LICENSE
--rw-r--r--   0        0        0     3851 2024-04-15 11:27:26.891808 kdp-1.4.0/README.md
--rw-r--r--   0        0        0   102413 2024-04-15 11:27:26.899808 kdp-1.4.0/docs/kdp_logo.png
--rw-r--r--   0        0        0      668 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/__init__.py
--rw-r--r--   0        0        0     2632 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/custom_layers.py
--rw-r--r--   0        0        0     5046 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/features.py
--rw-r--r--   0        0        0     8096 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/layers_factory.py
--rw-r--r--   0        0        0     3322 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/pipeline.py
--rw-r--r--   0        0        0    26344 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/processor.py
--rw-r--r--   0        0        0    11967 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/stats.py
--rw-r--r--   0        0        0     4034 2024-04-15 11:28:49.564487 kdp-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 kdp-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-18 15:22:06.750477 kdp-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4114 2024-04-18 15:22:06.750477 kdp-1.5.0/README.md
+-rw-r--r--   0        0        0   102413 2024-04-18 15:22:06.758477 kdp-1.5.0/docs/kdp_logo.png
+-rw-r--r--   0        0        0      668 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/__init__.py
+-rw-r--r--   0        0        0     2632 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/custom_layers.py
+-rw-r--r--   0        0        0     5046 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/features.py
+-rw-r--r--   0        0        0     8180 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/layers_factory.py
+-rw-r--r--   0        0        0     3322 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/pipeline.py
+-rw-r--r--   0        0        0    26497 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/processor.py
+-rw-r--r--   0        0        0    11967 2024-04-18 15:22:06.758477 kdp-1.5.0/kdp/stats.py
+-rw-r--r--   0        0        0     4034 2024-04-18 15:23:39.342925 kdp-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 kdp-1.5.0/PKG-INFO
```

### Comparing `kdp-1.4.0/LICENSE` & `kdp-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/README.md` & `kdp-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # 🌟 Welcome to Keras Data Processor (KDP) - Preprocessing Power with TensorFlow Keras 🌟
 
 <p align="center">
   <img src="docs/kdp_logo.png" width="350"/>
 </p>
 
-** Welcome to the Future of Data Preprocessing!**
+**Welcome to the Future of Data Preprocessing!**
 
 Diving into the world of machine learning and data science, we often find ourselves tangled in the preprocessing jungle.
 Worry no more! Introducing a state-of-the-art data preprocessing model based on TensorFlow Keras and the innovative use of Keras preprocessing layers.
 
 Say goodbye to tedious data preparation tasks and hello to streamlined, efficient, and scalable data pipelines. Whether you're a seasoned data scientist or just starting out, this tool is designed to supercharge your ML workflows, making them more robust and faster than ever!
 
 ## 🔑 Key Features:
 
-- Automated Feature Engineering: Automatically detects and applies the optimal preprocessing steps for each feature type in your dataset.
+- Automatic and scalable features statistics extraction: Automatically infer the feature tatistics from your data, saving you time and efforts.
 
 - Customizable Preprocessing Pipelines: Tailor your preprocessing steps with ease, choosing from a wide range of options for numeric, categorical, and even complex feature crosses.
 
 - Scalability and Efficiency: Designed for performance, handling large datasets with ease thanks to TensorFlow's powerful backend.
 
 - Easy Integration: Seamlessly fits into your TensorFlow Keras models (as first layers of the mode), making it a breeze to go from raw data to trained model faster than ever.
 
@@ -92,10 +92,16 @@
 
 This will result in the following preprocessing steps:
 
 <p align="center">
   <img src="docs/imgs/Model_Architecture.png" width="800"/>
 </p>
 
+
+**This preprocessing model can be used independentyly or as the first layer of any Keras model.
+This means you can ship your model with the preprocessing pipeline (built-in) as a single entity and deploy it with ease using Tesnorflow Serving.**
+
+```python
+
 ## 🔍 Dive Deeper:
 
 Explore the detailed documentation to leverage the full potential of this preprocessing tool. Learn about customizing feature crosses, bucketization strategies, embedding sizes, and much more to truly tailor your preprocessing pipeline to your project's needs.
```

### Comparing `kdp-1.4.0/docs/kdp_logo.png` & `kdp-1.5.0/docs/kdp_logo.png`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/kdp/__init__.py` & `kdp-1.5.0/kdp/__init__.py`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/kdp/custom_layers.py` & `kdp-1.5.0/kdp/custom_layers.py`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/kdp/features.py` & `kdp-1.5.0/kdp/features.py`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/kdp/layers_factory.py` & `kdp-1.5.0/kdp/layers_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tensorflow as tf
 
 from kdp.custom_layers import CastToFloat32Layer, TextPreprocessingLayer
 
 
 class PreprocessorLayerFactory:
     @staticmethod
-    def create_layer(layer_class, name: str = None, **kwargs) -> tf.keras.layers.Layer:
+    def create_layer(layer_class, name: str = None, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a layer, automatically filtering kwargs based on the provided layer_class.
 
         Args:
             layer_class: The class of the layer to be created.
             name: The name of the layer. Optional.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
@@ -29,15 +29,15 @@
 
         # Create an instance of the layer class with the filtered kwargs
         layer_instance = layer_class(**filtered_kwargs)
         return layer_instance
 
     # Example usage for specific layer types
     @staticmethod
-    def normalization_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def normalization_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Normalization layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -46,15 +46,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Normalization,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def discretization_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def discretization_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Discretization layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -63,15 +63,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Discretization,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def rescaling_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def rescaling_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Rescaling layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -80,15 +80,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Rescaling,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def embedding_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def embedding_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Embedding layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -97,15 +97,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Embedding,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def category_encoding_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def category_encoding_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a CategoryEncoding layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -114,15 +114,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.CategoryEncoding,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def string_lookup_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def string_lookup_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a StringLookup layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -131,15 +131,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.StringLookup,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def integer_lookup_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def integer_lookup_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a IntegerLookup layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -148,15 +148,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.IntegerLookup,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def crossing_layer(name: str, **kwargs) -> tf.keras.layers.Layer:
+    def crossing_layer(name: str, **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a HashedCrossing layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -165,15 +165,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.HashedCrossing,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def flatten_layer(name: str = "flatten", **kwargs) -> tf.keras.layers.Layer:
+    def flatten_layer(name: str = "flatten", **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Flatten layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -182,15 +182,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Flatten,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def concat_layer(name: str = "concat", **kwargs) -> tf.keras.layers.Layer:
+    def concat_layer(name: str = "concat", **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a Concatenate layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -199,15 +199,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.Concatenate,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def text_preprocessing_layer(name: str = "text_preprocessing", **kwargs) -> tf.keras.layers.Layer:
+    def text_preprocessing_layer(name: str = "text_preprocessing", **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a TextPreprocessingLayer layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -216,15 +216,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=TextPreprocessingLayer,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def text_vectorization_layer(name: str = "text_vectorization", **kwargs) -> tf.keras.layers.Layer:
+    def text_vectorization_layer(name: str = "text_vectorization", **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a TextVectorization layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
@@ -233,15 +233,15 @@
         return PreprocessorLayerFactory.create_layer(
             layer_class=tf.keras.layers.TextVectorization,
             name=name,
             **kwargs,
         )
 
     @staticmethod
-    def cast_to_float32_layer(name: str = "cast_to_float32", **kwargs) -> tf.keras.layers.Layer:
+    def cast_to_float32_layer(name: str = "cast_to_float32", **kwargs: dict) -> tf.keras.layers.Layer:
         """Create a CastToFloat32Layer layer.
 
         Args:
             name: The name of the layer.
             **kwargs: Additional keyword arguments to pass to the layer constructor.
 
         Returns:
```

### Comparing `kdp-1.4.0/kdp/pipeline.py` & `kdp-1.5.0/kdp/pipeline.py`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/kdp/processor.py` & `kdp-1.5.0/kdp/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,15 +566,19 @@
         self.model = tf.keras.Model(
             inputs=self.inputs,
             outputs=self.outputs,
             name="preprocessor",
         )
 
         # displaying information.
-        _output_dims = self.model.output_shape[1]
+        logger.info("Building preprocessor Model")
+        _output_dims = (
+            self.model.output_shape[1] if self.output_mode == OutputModeOptions.CONCAT else self.model.output_shape
+        )
+
         logger.info(f"Preprocessor Model built successfully ✅, summary: {self.model.summary()}")
         logger.info(f"Imputs: {self.inputs.keys()}")
         logger.info(f"Output model mode: {self.output_mode} with size: {_output_dims}")
         return {
             "model": self.model,
             "inputs": self.inputs,
             "signature": self.signature,
```

### Comparing `kdp-1.4.0/kdp/stats.py` & `kdp-1.5.0/kdp/stats.py`

 * *Files identical despite different names*

### Comparing `kdp-1.4.0/pyproject.toml` & `kdp-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kdp"
-version = "1.4.0"
+version = "1.5.0"
 documentation = "http://piotrlaczkowski.github.io/keras-data-processor/"
 repository = "https://github.com/piotrlaczkowski/keras-data-processor"
 description = "Data Preprocessing model based on Keras preprocessing layers"
 authors = ["piotrlaczkowski <piotr.laczkowski@gmail.com>"]
 readme = "README.md"
 include = ["docs/kdp_logo.png"]
```

### Comparing `kdp-1.4.0/PKG-INFO` & `kdp-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Data Preprocessing model based on Keras preprocessing layers
 Home-page: https://github.com/piotrlaczkowski/keras-data-processor
 Author: piotrlaczkowski
 Author-email: piotr.laczkowski@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -17,24 +17,24 @@
 
 # 🌟 Welcome to Keras Data Processor (KDP) - Preprocessing Power with TensorFlow Keras 🌟
 
 <p align="center">
   <img src="docs/kdp_logo.png" width="350"/>
 </p>
 
-** Welcome to the Future of Data Preprocessing!**
+**Welcome to the Future of Data Preprocessing!**
 
 Diving into the world of machine learning and data science, we often find ourselves tangled in the preprocessing jungle.
 Worry no more! Introducing a state-of-the-art data preprocessing model based on TensorFlow Keras and the innovative use of Keras preprocessing layers.
 
 Say goodbye to tedious data preparation tasks and hello to streamlined, efficient, and scalable data pipelines. Whether you're a seasoned data scientist or just starting out, this tool is designed to supercharge your ML workflows, making them more robust and faster than ever!
 
 ## 🔑 Key Features:
 
-- Automated Feature Engineering: Automatically detects and applies the optimal preprocessing steps for each feature type in your dataset.
+- Automatic and scalable features statistics extraction: Automatically infer the feature tatistics from your data, saving you time and efforts.
 
 - Customizable Preprocessing Pipelines: Tailor your preprocessing steps with ease, choosing from a wide range of options for numeric, categorical, and even complex feature crosses.
 
 - Scalability and Efficiency: Designed for performance, handling large datasets with ease thanks to TensorFlow's powerful backend.
 
 - Easy Integration: Seamlessly fits into your TensorFlow Keras models (as first layers of the mode), making it a breeze to go from raw data to trained model faster than ever.
 
@@ -109,11 +109,17 @@
 
 This will result in the following preprocessing steps:
 
 <p align="center">
   <img src="docs/imgs/Model_Architecture.png" width="800"/>
 </p>
 
+
+**This preprocessing model can be used independentyly or as the first layer of any Keras model.
+This means you can ship your model with the preprocessing pipeline (built-in) as a single entity and deploy it with ease using Tesnorflow Serving.**
+
+```python
+
 ## 🔍 Dive Deeper:
 
 Explore the detailed documentation to leverage the full potential of this preprocessing tool. Learn about customizing feature crosses, bucketization strategies, embedding sizes, and much more to truly tailor your preprocessing pipeline to your project's needs.
```

