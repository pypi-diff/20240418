# Comparing `tmp/degann-0.3.tar.gz` & `tmp/degann-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degann-0.3.tar", last modified: Wed Sep 27 10:42:23 2023, max compression
+gzip compressed data, was "degann-1.0.tar", last modified: Thu Apr 18 15:16:11 2024, max compression
```

## Comparing `degann-0.3.tar` & `degann-1.0.tar`

### file list

```diff
@@ -1,49 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.670467 degann-0.3/
--rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-0.3/LICENSE
--rw-rw-rw-   0        0        0     2668 2023-09-27 10:42:23.669471 degann-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1820 2023-09-27 10:41:38.000000 degann-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.627612 degann-0.3/degann/
--rw-rw-rw-   0        0        0       80 2023-09-27 09:30:32.000000 degann-0.3/degann/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.638575 degann-0.3/degann/equations/
--rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-0.3/degann/equations/__init__.py
--rw-rw-rw-   0        0        0     2932 2023-09-27 09:30:32.000000 degann-0.3/degann/equations/equation_utils.py
--rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-0.3/degann/equations/simple_equation.py
--rw-rw-rw-   0        0        0     4158 2023-06-22 20:01:24.000000 degann-0.3/degann/equations/system_ode.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.657511 degann-0.3/degann/networks/
--rw-rw-rw-   0        0        0      299 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/__init__.py
--rw-rw-rw-   0        0        0     2076 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/__main__.py
--rw-rw-rw-   0        0        0     1953 2023-09-27 09:56:41.000000 degann-0.3/degann/networks/activations.py
--rw-rw-rw-   0        0        0     2707 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/callbacks.py
--rw-rw-rw-   0        0        0      461 2023-09-27 10:41:13.000000 degann-0.3/degann/networks/config_format.py
--rw-rw-rw-   0        0        0     8280 2023-06-22 20:01:24.000000 degann-0.3/degann/networks/cpp_utils.py
--rw-rw-rw-   0        0        0    14159 2023-09-27 09:30:34.000000 degann-0.3/degann/networks/expert.py
--rw-rw-rw-   0        0        0     7488 2023-09-27 08:57:59.000000 degann-0.3/degann/networks/generate.py
--rw-rw-rw-   0        0        0    13624 2023-09-27 09:20:29.000000 degann-0.3/degann/networks/imodel.py
--rw-rw-rw-   0        0        0     2715 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/layer_creator.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.659505 degann-0.3/degann/networks/layers/
--rw-rw-rw-   0        0        0       22 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/layers/__init__.py
--rw-rw-rw-   0        0        0     5202 2023-08-26 16:23:33.000000 degann-0.3/degann/networks/layers/dense.py
--rw-rw-rw-   0        0        0     3671 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/losses.py
--rw-rw-rw-   0        0        0     5381 2023-06-22 20:01:24.000000 degann-0.3/degann/networks/metrics.py
--rw-rw-rw-   0        0        0     1198 2023-09-27 09:36:30.000000 degann-0.3/degann/networks/nn_code.py
--rw-rw-rw-   0        0        0      690 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/optimizers.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.661498 degann-0.3/degann/networks/topology/
--rw-rw-rw-   0        0        0       25 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/topology/__init__.py
--rw-rw-rw-   0        0        0    13897 2023-09-27 09:34:51.000000 degann-0.3/degann/networks/topology/densenet.py
--rw-rw-rw-   0        0        0    19170 2023-06-22 20:01:24.000000 degann-0.3/degann/networks/trainer.py
--rw-rw-rw-   0        0        0     3663 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/unrefactored.py
--rw-rw-rw-   0        0        0     3064 2023-09-27 09:30:32.000000 degann-0.3/degann/networks/utils.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.668475 degann-0.3/degann/testlaunches/
--rw-rw-rw-   0        0        0       83 2023-09-27 09:30:32.000000 degann-0.3/degann/testlaunches/__init__.py
--rw-rw-rw-   0        0        0     1054 2023-09-27 09:30:32.000000 degann-0.3/degann/testlaunches/__main__.py
--rw-rw-rw-   0        0        0     4119 2023-08-06 08:10:19.000000 degann-0.3/degann/testlaunches/build_tables.py
--rw-rw-rw-   0        0        0     2957 2023-09-27 09:30:32.000000 degann-0.3/degann/testlaunches/experiments.py
--rw-rw-rw-   0        0        0     4004 2023-09-27 09:30:32.000000 degann-0.3/degann/testlaunches/functions.py
-drwxrwxrwx   0        0        0        0 2023-09-27 10:42:23.634590 degann-0.3/degann.egg-info/
--rw-rw-rw-   0        0        0     2668 2023-09-27 10:42:23.000000 degann-0.3/degann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-09-27 10:42:23.000000 degann-0.3/degann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-27 10:42:23.000000 degann-0.3/degann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-09-27 10:42:23.000000 degann-0.3/degann.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-09-27 10:42:23.000000 degann-0.3/degann.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-27 10:42:23.670467 degann-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1505 2023-09-27 09:30:32.000000 degann-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.839355 degann-1.0/
+-rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.0/LICENSE
+-rw-rw-rw-   0        0        0     3026 2024-04-18 15:16:11.839355 degann-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2024-04-18 14:22:40.000000 degann-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.814356 degann-1.0/degann/
+-rw-rw-rw-   0        0        0       74 2024-03-19 14:02:34.000000 degann-1.0/degann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.825355 degann-1.0/degann/equations/
+-rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.0/degann/equations/__init__.py
+-rw-rw-rw-   0        0        0     2934 2023-12-26 18:47:41.000000 degann-1.0/degann/equations/equation_utils.py
+-rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.0/degann/equations/simple_equation.py
+-rw-rw-rw-   0        0        0     4158 2023-06-22 20:01:24.000000 degann-1.0/degann/equations/system_ode.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.829357 degann-1.0/degann/expert/
+-rw-rw-rw-   0        0        0      108 2024-03-19 14:02:34.000000 degann-1.0/degann/expert/__init__.py
+-rw-rw-rw-   0        0        0     7725 2024-04-13 13:40:21.000000 degann-1.0/degann/expert/generate.py
+-rw-rw-rw-   0        0        0     1265 2024-02-26 17:01:06.000000 degann-1.0/degann/expert/nn_code.py
+-rw-rw-rw-   0        0        0    19246 2024-04-18 15:08:00.000000 degann-1.0/degann/expert/search_algorithms.py
+-rw-rw-rw-   0        0        0     6514 2024-04-18 15:08:00.000000 degann-1.0/degann/expert/selector.py
+-rw-rw-rw-   0        0        0    11634 2024-04-17 17:20:26.000000 degann-1.0/degann/expert/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.836356 degann-1.0/degann/networks/
+-rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.0/degann/networks/__init__.py
+-rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/activations.py
+-rw-rw-rw-   0        0        0     2707 2023-09-27 09:30:32.000000 degann-1.0/degann/networks/callbacks.py
+-rw-rw-rw-   0        0        0      465 2024-04-18 14:22:40.000000 degann-1.0/degann/networks/config_format.py
+-rw-rw-rw-   0        0        0     8267 2024-03-17 08:10:56.000000 degann-1.0/degann/networks/cpp_utils.py
+-rw-rw-rw-   0        0        0    13744 2024-04-17 17:09:28.000000 degann-1.0/degann/networks/imodel.py
+-rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/layer_creator.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.837355 degann-1.0/degann/networks/layers/
+-rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     5220 2024-03-26 15:50:19.000000 degann-1.0/degann/networks/layers/tf_dense.py
+-rw-rw-rw-   0        0        0     3631 2024-04-17 13:40:01.000000 degann-1.0/degann/networks/losses.py
+-rw-rw-rw-   0        0        0     2421 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/metrics.py
+-rw-rw-rw-   0        0        0      690 2023-09-27 16:24:36.000000 degann-1.0/degann/networks/optimizers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.838355 degann-1.0/degann/networks/topology/
+-rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/topology/__init__.py
+-rw-rw-rw-   0        0        0    14102 2024-04-17 17:10:30.000000 degann-1.0/degann/networks/topology/tf_densenet.py
+-rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.822362 degann-1.0/degann.egg-info/
+-rw-rw-rw-   0        0        0     3026 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:16:11.839355 degann-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1517 2024-04-18 14:43:31.000000 degann-1.0/setup.py
```

### Comparing `degann-0.3/LICENSE` & `degann-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degann-0.3/PKG-INFO` & `degann-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 0.3
+Version: 1.0
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -20,28 +20,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-0.3-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
 - Choosing the Best Neural Network from Several for Fixed Training Parameters
 - Iterating over training parameters with choosing the best neural network for each set
-- Export neural networks as a function in C++
+- Export Neural Networks as a function in C++
 - Export Neural Networks as a Parameter Set
 - Import Neural Networks from a Parameter Set
 - Building a dataset with complete training results for approximating the solution of a differential equation for each neural network that participated in training
+- Advanced search for optimal topology using a language that describes the topology of a neural network
+- Random search for optimal neural network topology
+- Method for simulating annealing of optimal neural network topology
+- Expert system for automatic selection of optimal parameters for algorithms for searching neural network topologies
 
 ## Install
 
 ### Manual
 Download the repository as a zip archive, unpack and run the command from the root of the repository
 ```bash
 pip install -r requirements.txt
```

### Comparing `degann-0.3/README.md` & `degann-1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-0.3-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
 - Choosing the Best Neural Network from Several for Fixed Training Parameters
 - Iterating over training parameters with choosing the best neural network for each set
-- Export neural networks as a function in C++
+- Export Neural Networks as a function in C++
 - Export Neural Networks as a Parameter Set
 - Import Neural Networks from a Parameter Set
 - Building a dataset with complete training results for approximating the solution of a differential equation for each neural network that participated in training
+- Advanced search for optimal topology using a language that describes the topology of a neural network
+- Random search for optimal neural network topology
+- Method for simulating annealing of optimal neural network topology
+- Expert system for automatic selection of optimal parameters for algorithms for searching neural network topologies
 
 ## Install
 
 ### Manual
 Download the repository as a zip archive, unpack and run the command from the root of the repository
 ```bash
 pip install -r requirements.txt
```

### Comparing `degann-0.3/degann/equations/equation_utils.py` & `degann-1.0/degann/equations/equation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     interval: Tuple[float, float]
         The interval for which the plot will be built
     step: float
         Interval coverage step (number of points per interval)
     title: str
         Title for plot
     labels: list[str]
-        Labels for each network and true data
+        Labels for each network and `true` data
     true_data: tuple[list, list]
         x and f(x)
     is_debug: bool
         Console debug output marker
     Returns
     -------
     None
```

### Comparing `degann-0.3/degann/equations/simple_equation.py` & `degann-1.0/degann/equations/simple_equation.py`

 * *Files identical despite different names*

### Comparing `degann-0.3/degann/equations/system_ode.py` & `degann-1.0/degann/equations/system_ode.py`

 * *Files identical despite different names*

### Comparing `degann-0.3/degann/networks/activations.py` & `degann-1.0/degann/networks/activations.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,25 @@
     new_x: tf.Tensor
         Data vector after applying activation function
     """
     return tf.where(x >= 0, beta + tf.sqrt(2 * p * x), beta - tf.sqrt(-2 * p * x))
 
 
 _activation_name = {
-    # "perceptron_threshold": perceptron_threshold,
     "elu": tf.keras.activations.elu,
     "relu": tf.keras.activations.relu,
     "gelu": tf.keras.activations.gelu,
     "selu": tf.keras.activations.selu,
     "exponential": tf.keras.activations.exponential,
     "linear": tf.keras.activations.linear,
     "sigmoid": tf.keras.activations.sigmoid,
     "hard_sigmoid": tf.keras.activations.hard_sigmoid,
     "swish": tf.keras.activations.swish,
     "tanh": tf.keras.activations.tanh,
     "softplus": tf.keras.activations.softplus,
-    # "softmax": tf.keras.activations.softmax,
     "softsign": tf.keras.activations.softsign,
     "parabolic": parabolic,
 }
 
 
 def get(name: str) -> Callable:
     """
```

### Comparing `degann-0.3/degann/networks/callbacks.py` & `degann-1.0/degann/networks/callbacks.py`

 * *Files identical despite different names*

### Comparing `degann-0.3/degann/networks/cpp_utils.py` & `degann-1.0/degann/networks/cpp_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -214,59 +214,61 @@
     left_name: str,
     left_size: int,
     right_name: str,
     right_size: int,
     weight_name: str,
     bias_name: str,
     activation_func: str,
-    decorator_params: list = None,
 ) -> str:
     res = f"""
     for (int i = 0; i < {right_size}; i++)
     {{
         for (int j = 0; j < {left_size}; j++)
         {{
             {right_name}[i] += {weight_name}[j][i] * {left_name}[j];
         }}
         {right_name}[i] += {bias_name}[i];
-        {activation_to_cpp_template(right_name + "[i]", activation_func, decorator_params)}
+        {activation_to_cpp_template(right_name + "[i]", activation_func)}
     }}
     """
 
     return res
 
 
-def activation_to_cpp_template(
-    name: str, activation_name: str, decorator_params: list = None
-) -> str:
+def activation_to_cpp_template(name: str, activation_name: str) -> str:
+    """
+    Build code for activation function by function name and variable name
+
+    Parameters
+    ----------
+    name: str
+        Name of variable
+    activation_name: str
+        Name of activation func
+
+    Returns
+    -------
+    c_activation: str
+        Translated activation
+    """
     d = {
         "linear": lambda x: f"{x} = {x};\n",
         "elu": lambda x: f"if ({x} >= 0) {x} = {x}; else {x} = 1.0 * (exp({x}) - 1);\n",
-        # "gelu": lambda x: ,
-        "relu": lambda x: f"{x} = max({x}, 0);\n",
+        "gelu": lambda x: f"{x} = 0.5 * {x} * (1 + tanh(sqrt(2 / 3.14159265) * ({x} + 0.044715 * {x} * {x} * {x})))",
+        "relu": lambda x: f"{x} = max({x}, 0.0f);\n",
         "selu": lambda x: f"if ({x} >= 0) {x} = 1.05070098 * {x}; else {x} = 1.05070098 * 1.67326324 * (exp({x}) - 1);\n",
         "exponential": lambda x: f"{x} = exp({x});\n",
         "hard_sigmoid": lambda x: f"if ({x} < -2.5) {x} = 0; else if ({x} > 2.5) {x} = 1; else {x} = 0.2 * {x} + 0.5;\n",
         "sigmoid": lambda x: f"{x} = 1 / (1 + exp(-{x}));\n",
         "softplus": lambda x: f"{x} = log(exp({x}) + 1);\n",
         "softsign": lambda x: f"{x} = {x} / (abs({x}) + 1.0);\n",
-        # "softmax": lambda x: ,
         "swish": lambda x: f"{x} = {x} / (1 + exp(-{x}));\n",
         "tanh": lambda x: f"{x} = ((exp({x}) - exp(-{x}))/(exp({x}) + exp(-{x})));\n",
     }
 
-    if activation_name == "perceptron_threshold":
-        d.update(
-            {
-                "perceptron_threshold": lambda x: _fill_values(
-                    f"if ({x} >= threshold) {x} = 1; else {x} = 0;\n", decorator_params
-                )
-            }
-        )
-
     return d[activation_name](name)
 
 
 def _fill_values(act_func: str, values: List[Tuple[str, float]]):
     for key, value in values:
         act_func = act_func.replace(key, str(value))
     return act_func
```

### Comparing `degann-0.3/degann/networks/expert.py` & `degann-1.0/degann/networks/topology/tf_densenet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,470 +1,455 @@
-import csv
-import math
-import random
-from datetime import datetime
-from itertools import product
-from typing import Callable, List, Tuple
+import os
+from typing import List, Optional, Dict, Callable
+
 import tensorflow as tf
+from tensorflow import keras
 
-from degann.networks.callbacks import MeasureTrainTime
-from degann.networks import imodel
-from degann.networks.nn_code import decode
-from degann.networks.generate import (
-    choose_neighbor,
-    EpochParameter,
-    CodeParameter,
-    random_generate,
-    generate_neighbor,
-)
-
-_algorithms_for_random_generator = {0: "auto_select", 1: "philox", 2: "threefry"}
-
-
-def update_random_generator(curr_iter: int, cycle_size: int = 0) -> None:
-    """
-    Set global tensorflow random generator to random state every *cycle_size* times
-
-    Parameters
-    ----------
-    curr_iter: int
-        Counter showing whether it's time to update the random number generator
-    cycle_size: int
-        How often should we update random number generator (if not positive, then the generator does not change)
-
-    Returns
-    -------
-    """
-    if cycle_size > 0 and curr_iter % cycle_size == 0:
-        new_g = tf.random.Generator.from_non_deterministic_state(
-            alg=_algorithms_for_random_generator[
-                random.randint(0, len(_algorithms_for_random_generator) - 1)
-            ]
-        )
-        tf.random.set_global_generator(new_g)
-    else:
-        pass
-
-
-def temperature_exp(t: float, alpha: float, **kwargs) -> float:
-    """
-    Calculate new temperature for simulated annealing as *t * alpha*
-
-    Parameters
-    ----------
-    t: float
-        Current temperature
-    alpha: float
-        Exponential exponent
-
-    Returns
-    -------
-    new_t: float
-        New temperature
-    """
-    return t * alpha
-
-
-def temperature_lin(k: int, k_max: int, **kwargs) -> float:
-    """
-    Calculate new temperature for simulated annealing as *1 - (k + 1) / k_max*
-
-    Parameters
-    ----------
-    k: float
-        Current iteration
-    k_max: float
-        Amount of all iterations
-
-    Returns
-    -------
-    new_t: float
-        New temperature
-    """
-    return 1 - (k + 1) / k_max
-
-
-def distance_const(d: float) -> Callable:
-    """
-    Calculate distance to neighbour for simulated annealing as constant
-
-    Parameters
-    ----------
-    d: float
-        Constant distance
-
-    Returns
-    -------
-    d_c: Callable
-        Function returning a constant distance
-    """
-
-    def d_c(**kwargs) -> float:
-        return d
-
-    return d_c
-
-
-def distance_lin(offset, multiplier):
-    """
-    Calculate distance to neighbour for simulated annealing as *offset + temperature * multiplier*
-
-    Parameters
-    ----------
-    offset: float
-    multiplier: float
-
-    Returns
-    -------
-    d_l: Callable
-        Function returning a new distance depending on current temperature
-    """
-
-    def d_l(temperature, **kwargs):
-        return offset + temperature * multiplier
-
-    return d_l
-
-
-def simulated_annealing(
-    in_size,
-    out_size,
-    data,
-    val_data=None,
-    k_max: int = 100,
-    start_net: dict = None,
-    method: Callable = generate_neighbor,
-    temperature_method: Callable = temperature_lin,
-    distance_method: Callable = distance_const(150),
-    opt: str = "Adam",
-    loss: str = "Huber",
-    update_gen_cycle: int = 0,
-    file_name: str = "",
-    logging: bool = False,
-):
-    gen = random_generate()
-    if start_net is None:
-        b, a = decode(gen[0].value(), offset=8)
-        curr_best = imodel.IModel(in_size, b, out_size, a + ["linear"])
-        curr_best.compile(optimizer=opt, loss_func=loss)
-    else:
-        curr_best = imodel.IModel(in_size, [], out_size, ["linear"])
-        curr_best = curr_best.from_dict(start_net)
-    curr_epoch = gen[1].value()
-    hist = curr_best.train(data[0], data[1], epochs=curr_epoch, verbose=0)
-    curr_loss = hist.history["loss"][-1]
-    best_val_loss = (
-        curr_best.evaluate(val_data[0], val_data[1], verbose=0, return_dict=True)[
-            "loss"
-        ]
-        if val_data is not None
-        else None
-    )
-    best_epoch = curr_epoch
-    best_nn = curr_best.to_dict()
-    best_gen = gen
-    best_a = curr_best.get_activations
-    best_loss = curr_loss
-
-    gen = (CodeParameter(gen[0].value()), EpochParameter(gen[1].value()))
-    k = 0
-    t = 1
-    while k < k_max - 1 and curr_loss > 1e-20:
-        update_random_generator(k, cycle_size=update_gen_cycle)
-        t = temperature_method(k=k, k_max=k_max, t=1, alpha=0.97)
-        distance = distance_method(temperature=t)
+from degann.networks.config_format import LAYER_DICT_NAMES
+from degann.networks import layer_creator, losses, metrics, cpp_utils
+from degann.networks import optimizers
+from degann.networks.layers.tf_dense import TensorflowDense
+
+
+class TensorflowDenseNet(tf.keras.Model):
+    def __init__(
+        self,
+        input_size: int = 2,
+        block_size: list = None,
+        output_size: int = 10,
+        activation_func: str = "linear",
+        weight=keras.initializers.RandomUniform(minval=-1, maxval=1),
+        biases=keras.initializers.RandomUniform(minval=-1, maxval=1),
+        is_debug: bool = False,
+        **kwargs,
+    ):
+        decorator_params: List[Optional[Dict]] = [None]
+        if "decorator_params" in kwargs.keys():
+            decorator_params = kwargs.get("decorator_params")
+            kwargs.pop("decorator_params")
+        else:
+            decorator_params = [None]
 
-        gen_neighbor = choose_neighbor(
-            method, parameters=(gen[0].value(), gen[1].value()), distance=distance
-        )
-        b, a = decode(gen_neighbor[0].value(), offset=8)
-        neighbor = imodel.IModel(in_size, b, out_size, a + ["linear"])
-        neighbor.compile(optimizer=opt, loss_func=loss)
-        neighbor_hist = neighbor.train(
-            data[0], data[1], epochs=gen_neighbor[1].value(), verbose=0
-        )
-        neighbor_loss = neighbor_hist.history["loss"][-1]
+        if (
+            isinstance(decorator_params, list)
+            and len(decorator_params) == 1
+            and decorator_params[0] is None
+            or decorator_params is None
+        ):
+            decorator_params = [None] * (len(block_size) + 1)
 
         if (
-            neighbor_loss < curr_loss
-            or math.e ** ((curr_loss - neighbor_loss) / t) > random.random()
+            isinstance(decorator_params, list)
+            and len(decorator_params) == 1
+            and decorator_params[0] is not None
         ):
-            curr_best = neighbor
-            gen = gen_neighbor
-            curr_epoch = gen_neighbor[1].value()
-            curr_loss = neighbor_loss
-
-            history = {
-                "code": [gen[0].value()],
-                "epoch": [gen[1].value()],
-                "shapes": [curr_best.get_shape],
-                "activations": [a],
-                "loss function": [loss],
-                "optimizer": [opt],
-                "loss": [curr_loss],
-            }
-            curr_val_loss = (
-                curr_best.evaluate(
-                    val_data[0], val_data[1], verbose=0, return_dict=True
-                )["loss"]
-                if val_data is not None
-                else None
+            decorator_params = decorator_params * (len(block_size) + 1)
+
+        super(TensorflowDenseNet, self).__init__(**kwargs)
+        self.blocks: List[TensorflowDense] = []
+
+        if not isinstance(activation_func, list):
+            activation_func = [activation_func] * (len(block_size) + 1)
+        if len(block_size) != 0:
+            self.blocks.append(
+                layer_creator.create_dense(
+                    input_size,
+                    block_size[0],
+                    activation=activation_func[0],
+                    weight=weight,
+                    bias=biases,
+                    is_debug=is_debug,
+                    name=f"MyDense0",
+                    decorator_params=decorator_params[0],
+                )
             )
-            history["validation loss"] = [curr_val_loss]
+            for i in range(1, len(block_size)):
+                self.blocks.append(
+                    layer_creator.create_dense(
+                        block_size[i - 1],
+                        block_size[i],
+                        activation=activation_func[i],
+                        weight=weight,
+                        bias=biases,
+                        is_debug=is_debug,
+                        name=f"MyDense{i}",
+                        decorator_params=decorator_params[i],
+                    )
+                )
+            last_block_size = block_size[-1]
+        else:
+            last_block_size = input_size
+
+        self.out_layer = layer_creator.create_dense(
+            last_block_size,
+            output_size,
+            activation=activation_func[-1],
+            weight=weight,
+            bias=biases,
+            is_debug=is_debug,
+            name=f"OutLayerMyDense",
+            decorator_params=decorator_params[-1],
+        )
 
-            if logging:
-                fn = f"{file_name}_{len(data[0])}_ann_{loss}_{opt}"
-                with open(
-                    f"./{fn}.csv",
-                    "a",
-                    newline="",
-                ) as outfile:
-                    writer = csv.writer(outfile)
-                    writer.writerows(zip(*history.values()))
-
-            if curr_loss < best_loss:
-                best_loss = curr_loss
-                best_epoch = curr_epoch
-                best_nn = curr_best.to_dict()
-                best_gen = gen
-                best_a = a.copy()
-                best_val_loss = curr_val_loss
-        k += 1
-
-    history = {
-        "code": [best_gen[0].value()],
-        "epoch": [best_gen[1].value()],
-        "shapes": [curr_best.get_shape],
-        "activations": [best_a],
-        "loss function": [loss],
-        "optimizer": [opt],
-        "loss": [best_loss],
-        "validation loss": [best_val_loss],
-    }
-
-    if logging:
-        fn = f"{file_name}_{len(data[0])}_annealing_{loss}_{opt}"
-        with open(
-            f"./{fn}.csv",
-            "a",
-            newline="",
-        ) as outfile:
-            writer = csv.writer(outfile)
-            writer.writerows(zip(*history.values()))
-    return best_loss, best_epoch, loss, opt, best_nn
-
-
-def random_search(
-    in_size,
-    out_size,
-    data,
-    opt,
-    loss,
-    iterations,
-    val_data=None,
-    callbacks=None,
-    logging=False,
-    update_gen_cycle: int = 0,
-    file_name: str = "",
-):
-    best_net = None
-    best_loss = 1e6
-    best_epoch = None
-    for i in range(iterations):
-        update_random_generator(i, cycle_size=update_gen_cycle)
-        gen = random_generate()
-        b, a = decode(gen[0].value(), offset=8)
-        curr_best = imodel.IModel(in_size, b, out_size, a + ["linear"])
-        curr_best.compile(optimizer=opt, loss_func=loss)
-        curr_epoch = gen[1].value()
-        hist = curr_best.train(
-            data[0], data[1], epochs=curr_epoch, verbose=0, callbacks=callbacks
+        self.activation_funcs = activation_func
+        self.weight_initializer = weight
+        self.bias_initializer = biases
+        self.input_size = input_size
+        self.block_size = block_size
+        self.output_size = output_size
+        self.trained_time = {"train_time": 0.0, "epoch_time": [], "predict_time": 0}
+
+    def custom_compile(
+        self,
+        rate=1e-2,
+        optimizer="SGD",
+        loss_func="MeanSquaredError",
+        metric_funcs=None,
+        run_eagerly=False,
+    ):
+        """
+        Configures the model for training
+
+        Parameters
+        ----------
+        rate: float
+            learning rate for optimizer
+        optimizer: str
+            name of optimizer
+        loss_func: str
+            name of loss function
+        metric_funcs: list[str]
+            list with metric function names
+        run_eagerly: bool
+
+        Returns
+        -------
+
+        """
+        opt = optimizers.get_optimizer(optimizer)(learning_rate=rate)
+        loss = losses.get_loss(loss_func)
+        m = [metrics.get_metric(metric) for metric in metric_funcs]
+        self.compile(
+            optimizer=opt,
+            loss=loss,
+            metrics=m,
+            run_eagerly=run_eagerly,
         )
-        curr_loss = hist.history["loss"][-1]
-        history = {
-            "code": [gen[0].value()],
-            "epoch": [gen[1].value()],
-            "shapes": [curr_best.get_shape],
-            "activations": [a],
-            "loss": [curr_loss],
-            "loss function": [loss],
-            "optimizer": [opt],
+
+    def call(self, inputs, **kwargs):
+        """
+        Obtaining a neural network response on the input data vector
+        Parameters
+        ----------
+        inputs
+        kwargs
+
+        Returns
+        -------
+
+        """
+        x = inputs
+        for layer in self.blocks:
+            x = layer(x, **kwargs)
+        return self.out_layer(x, **kwargs)
+
+    def train_step(self, data):
+        """
+        Custom train step from tensorflow tutorial
+
+        Parameters
+        ----------
+        data: tuple
+            Pair of x and y (or dataset)
+        Returns
+        -------
+
+        """
+        # Unpack the data. Its structure depends on your model and
+        # on what you pass to `fit()`.
+        x, y = data
+        with tf.GradientTape() as tape:
+            y_pred = self(x, training=True)  # Forward pass
+            # Compute the loss value
+            # (the loss function is configured in `compile()`)
+            loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
+
+        # Compute gradients
+        trainable_vars = self.trainable_variables
+        gradients = tape.gradient(loss, trainable_vars)
+        # Update weights
+        self.optimizer.apply_gradients(zip(gradients, trainable_vars))
+        # Update metrics (includes the metric that tracks the loss)
+        self.compiled_metrics.update_state(y, y_pred)
+        # Return a dict mapping metric names to current value
+        return {m.name: m.result() for m in self.metrics}
+
+    def set_name(self, new_name):
+        self._name = new_name
+
+    def __str__(self):
+        res = f"IModel {self.name}\n"
+        for layer in self.blocks:
+            res += str(layer)
+        res += str(self.out_layer)
+        return res
+
+    def to_dict(self, **kwargs):
+        """
+        Export neural network to dictionary
+
+        Parameters
+        ----------
+        kwargs
+
+        Returns
+        -------
+
+        """
+        res = {
+            "net_type": "MyDense",
+            "name": self._name,
+            "input_size": self.input_size,
+            "block_size": self.block_size,
+            "output_size": self.output_size,
+            "layer": [],
+            "out_layer": self.out_layer.to_dict(),
         }
 
-        if val_data is not None:
-            curr_val_loss = curr_best.evaluate(
-                val_data[0], val_data[1], verbose=0, return_dict=True
-            )["loss"]
-            history["validation loss"] = [curr_val_loss]
-
-        if curr_loss < best_loss:
-            best_epoch = curr_epoch
-            best_net = curr_best.to_dict()
-            best_loss = curr_loss
-        if logging:
-            fn = f"{file_name}_{len(data[0])}_random_{loss}_{opt}"
-            with open(
-                f"./{fn}.csv",
-                "a",
-                newline="",
-            ) as outfile:
-                writer = csv.writer(outfile)
-                writer.writerows(zip(*history.values()))
-    return best_loss, best_epoch, loss, opt, best_net
-
-
-def random_search_endless(
-    in_size,
-    out_size,
-    data,
-    opt,
-    loss,
-    threshold,
-    val_data=None,
-    callbacks=None,
-    logging=False,
-    file_name: str = "",
-    verbose=False,
-):
-    nn_loss, nn_epoch, loss_f, opt_n, net = random_search(
-        in_size,
-        out_size,
-        data,
-        opt,
-        loss,
-        1,
-        val_data=val_data,
-        callbacks=callbacks,
-        logging=logging,
-        file_name=file_name,
-    )
-    i = 1
-    best_net = net
-    best_loss = nn_loss
-    best_epoch = nn_epoch
-    while nn_loss > threshold or i >= 1e6:
-        if verbose:
-            print(
-                f"Random search until less than threshold. Last loss = {nn_loss}. Iterations = {i}"
+        for i, layer in enumerate(self.blocks):
+            res["layer"].append(layer.to_dict())
+
+        return res
+
+    @classmethod
+    def from_layers(
+        cls,
+        input_size: int,
+        block_size: List[int],
+        output_size: int,
+        layers: List[TensorflowDense],
+        **kwargs,
+    ):
+        """
+        Restore neural network from list of layers
+        Parameters
+        ----------
+        input_size
+        block_size
+        output_size
+        layers
+        kwargs
+
+        Returns
+        -------
+
+        """
+        res = cls(
+            input_size=input_size,
+            block_size=block_size,
+            output_size=output_size,
+            **kwargs,
+        )
+
+        for layer_num in range(len(res.blocks)):
+            res.blocks[layer_num] = layers[layer_num]
+
+        return res
+
+    def from_dict(self, config, **kwargs):
+        """
+        Restore neural network from dictionary of params
+        Parameters
+        ----------
+        config
+        kwargs
+
+        Returns
+        -------
+
+        """
+        input_size = config["input_size"]
+        block_size = config["block_size"]
+        output_size = config["output_size"]
+
+        self.block_size = list(block_size)
+        self.input_size = input_size
+        self.output_size = output_size
+
+        layers: List[TensorflowDense] = []
+        for layer_config in config["layer"]:
+            layers.append(layer_creator.from_dict(layer_config))
+
+        self.blocks: List[TensorflowDense] = []
+        for layer_num in range(len(layers)):
+            self.blocks.append(layers[layer_num])
+
+        self.out_layer = layer_creator.from_dict(config["out_layer"])
+
+    def export_to_cpp(
+        self, path: str, array_type: str = "[]", path_to_compiler: str = None, **kwargs
+    ) -> None:
+        """
+        Export neural network as feedforward function on c++
+
+        Parameters
+        ----------
+        path: str
+            path to file with name, without extension
+        array_type: str
+            c-style or cpp-style ("[]" or "vector")
+        path_to_compiler: str
+            path to c/c++ compiler
+        kwargs
+
+        Returns
+        -------
+
+        """
+        res = """
+#include <cmath>
+#include <vector>
+
+#define max(x, y) ((x < y) ? y : x)
+
+        \n"""
+
+        config = self.to_dict(**kwargs)
+
+        input_size = self.input_size
+        output_size = self.output_size
+        blocks = self.block_size
+        reverse = False
+        layers = config["layer"] + [config["out_layer"]]
+
+        comment = f"// This function takes {input_size} elements array and returns {output_size} elements array\n"
+        signature = f""
+        start_func = "{\n"
+        end_func = "}\n"
+        transform_input_vector = ""
+        transform_output_array = ""
+        return_stat = "return answer;\n"
+
+        creator_1d: Callable[
+            [str, int, Optional[list]], str
+        ] = cpp_utils.array1d_creator("float")
+        creator_heap_1d: Callable[[str, int], str] = cpp_utils.array1d_heap_creator(
+            "float"
+        )
+        creator_2d: Callable[
+            [str, int, int, Optional[list]], str
+        ] = cpp_utils.array2d_creator("float")
+        if array_type == "[]":
+            signature = f"float* feedforward(float x_array[])\n"
+
+        if array_type == "vector":
+            signature = f"std::vector<float> feedforward(std::vector<float> x)\n"
+
+            transform_input_vector = cpp_utils.transform_1dvector_to_array(
+                "float", input_size, "x", "x_array"
+            )
+            transform_output_array = cpp_utils.transform_1darray_to_vector(
+                "float", output_size, "answer_vector", "answer"
             )
-        nn_loss, nn_epoch, loss_f, opt_n, net = random_search(
-            in_size,
-            out_size,
-            data,
-            opt,
-            loss,
-            1,
-            val_data=val_data,
-            callbacks=callbacks,
-            logging=logging,
-            file_name=file_name,
+            return_stat = "return answer_vector;\n"
+
+        create_layers = ""
+        create_layers += creator_1d(f"layer_0", input_size, initial_value=0)
+        for i, size in enumerate(blocks):
+            create_layers += creator_1d(f"layer_{i + 1}", size, initial_value=0)
+        create_layers += creator_1d(
+            f"layer_{len(blocks) + 1}", output_size, initial_value=0
         )
-        i += 1
-        if nn_loss < best_loss:
-            best_net = net
-            best_loss = nn_loss
-            best_epoch = nn_epoch
-    return best_loss, best_epoch, loss, opt, best_net, i
-
-
-def full_search_step(
-    code,
-    num_epoch,
-    opt,
-    loss,
-    data,
-    repeat: int = 1,
-    offset: int = 8,
-    val_data=None,
-    update_gen_cycle: int = 0,
-    logging=False,
-    file_name: str = "",
-    callbacks=None,
-):
-    best_net = None
-    best_loss = 1e6
-    best_val_loss = 1e6
-    for i in range(repeat):
-        update_random_generator(i, cycle_size=update_gen_cycle)
-        history = dict()
-        b, a = decode(code, block_size=1, offset=offset)
-        nn = imodel.IModel(1, b, 1, a + ["linear"])
-        nn.compile(optimizer=opt, loss_func=loss)
-        temp_his = nn.train(
-            data[0], data[1], epochs=num_epoch, verbose=0, callbacks=callbacks
+        create_layers += cpp_utils.copy_1darray_to_array(
+            input_size, "x_array", "layer_0"
         )
 
-        history["shapes"] = [nn.get_shape]
-        history["activations"] = [a]
-        history["code"] = [code]
-        history["epoch"] = [num_epoch]
-        history["optimizer"] = [opt]
-        history["loss function"] = [loss]
-        history["loss"] = [temp_his.history["loss"][-1]]
-        history["validation loss"] = (
-            [nn.evaluate(val_data[0], val_data[1], verbose=0, return_dict=True)["loss"]]
-            if val_data is not None
-            else [None]
+        create_weights = ""
+        for i, layer_dict in enumerate(layers):
+            create_weights += creator_2d(
+                f"weight_{i}_{i + 1}",
+                layer_dict[LAYER_DICT_NAMES["inp_size"]],
+                layer_dict[LAYER_DICT_NAMES["shape"]],
+                layer_dict[LAYER_DICT_NAMES["weights"]],
+                reverse=reverse,
+            )
+
+        fill_weights = ""
+
+        create_biases = ""
+        for i, layer_dict in enumerate(layers):
+            create_biases += creator_1d(
+                f"bias_{i + 1}",
+                layer_dict[LAYER_DICT_NAMES["shape"]],
+                layer_dict[LAYER_DICT_NAMES["bias"]],
+            )
+
+        fill_biases = ""
+        feed_forward_cycles = ""
+        for i, layer_dict in enumerate(layers):
+            left_size = layer_dict[
+                LAYER_DICT_NAMES["inp_size"]
+            ]  # if i != 0 else input_size
+            right_size = layer_dict[LAYER_DICT_NAMES["shape"]]
+            act_func = layer_dict[LAYER_DICT_NAMES["activation"]]
+            decorator_params = layer_dict.get(LAYER_DICT_NAMES["decorator_params"])
+            feed_forward_cycles += cpp_utils.feed_forward_step(
+                f"layer_{i}",
+                left_size,
+                f"layer_{i + 1}",
+                right_size,
+                f"weight_{i}_{i + 1}",
+                f"bias_{i + 1}",
+                act_func,
+            )
+
+        move_result = creator_heap_1d("answer", output_size)
+        move_result += cpp_utils.copy_1darray_to_array(
+            output_size, f"layer_{len(blocks) + 1}", "answer"
         )
-        history["train_time"] = [nn.network.trained_time["train_time"]]
 
-        if logging:
-            file_name = f"{file_name}_{len(data[0])}_{num_epoch}_{loss}_{opt}"
-            with open(
-                f"./{file_name}.csv",
-                "a",
-                newline="",
-            ) as outfile:
-                writer = csv.writer(outfile)
-                writer.writerows(zip(*history.values()))
-        if history["loss"][0] < best_loss:
-            best_loss = history["loss"][0]
-            best_val_loss = history["validation loss"][0]
-            best_net = nn.to_dict()
-    return (best_loss, best_val_loss, best_net)
-
-
-def full_search(
-    data: tuple,
-    net_size: Tuple[int, int],
-    alph,
-    epoch_bound: Tuple[int, int, int],
-    optimizers: List[str],
-    losses: List[str],
-    val_data=None,
-    logging=False,
-    file_name: str = "",
-    verbose=False,
-):
-    best_net = None
-    best_loss = 1e6
-    best_epoch = None
-    best_loss_func = None
-    best_opt = None
-    time_viewer = MeasureTrainTime()
-    for i in range(net_size[0], net_size[1] + 1):
-        if verbose:
-            print(i, datetime.today().strftime("%Y-%m-%d %H:%M:%S"))
-        codes = product(alph, repeat=i)
-        for elem in codes:
-            code = "".join(elem)
-            for epoch in range(epoch_bound[0], epoch_bound[1] + 1, epoch_bound[2]):
-                for opt in optimizers:
-                    for loss in losses:
-                        curr_loss, curr_val_loss, curr_nn = full_search_step(
-                            code=code,
-                            num_epoch=epoch,
-                            opt=opt,
-                            loss=loss,
-                            data=data,
-                            val_data=val_data,
-                            callbacks=[time_viewer],
-                            logging=logging,
-                            file_name=file_name,
-                        )
-                        if best_loss > curr_loss:
-                            best_net = curr_nn
-                            best_loss = curr_loss
-                            best_epoch = epoch
-                            best_loss_func = (loss,)
-                            best_opt = opt
-    return best_loss, best_epoch, best_loss_func, best_opt, best_net
+        res += comment
+        res += signature
+        res += start_func
+        res += transform_input_vector
+        res += create_layers
+        res += create_weights
+        res += fill_weights
+        res += create_biases
+        res += fill_biases
+        res += feed_forward_cycles
+        res += move_result
+        res += transform_output_array
+        res += return_stat
+        res += end_func
+
+        header_res = f"""
+        #ifndef {path[0].upper() + path[1:]}_hpp
+        #define {path[0].upper() + path[1:]}_hpp
+        #include "{path}.cpp"
+
+        {comment}
+        {signature};
+
+        #endif /* {path[0].upper() + path[1:]}_hpp */
+
+                """
+
+        with open(path + ".cpp", "w") as f:
+            f.write(res)
+
+        with open(path + ".hpp", "w") as f:
+            f.write(header_res)
+
+        if path_to_compiler is not None:
+            os.system(path_to_compiler + " -c -Ofast " + path + ".cpp")
+
+    @property
+    def get_activations(self) -> List:
+        """
+        Get list of activations functions for each layer
+
+        Returns
+        -------
+        activation: list
+        """
+        return [layer.get_activation for layer in self.blocks]
```

### Comparing `degann-0.3/degann/networks/imodel.py` & `degann-1.0/degann/networks/imodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import json
-import os
 from collections import defaultdict
-from typing import List, Callable, Optional, Dict
+from typing import List, Optional, Dict, Union
 
-import keras.initializers
 import numpy as np
 import tensorflow as tf
+from tensorflow import keras
 
-from degann.networks import cpp_utils
-from degann.networks.config_format import LAYER_DICT_NAMES, HEADER_OF_FILE
-from degann.networks.topology.densenet import DenseNet
+from degann.networks.config_format import HEADER_OF_APG_FILE
+from degann.networks.topology.tf_densenet import TensorflowDenseNet
 
 
 def _get_act_and_init(
     kwargs: dict,
     default_act,
     default_dec: Optional[List[Optional[Dict[str, float]]]],
     default_init,
@@ -52,16 +50,16 @@
 
     def __init__(
         self,
         input_size: int,
         block_size: List[int],
         output_size: int,
         activation_func="sigmoid",
-        weight_init=tf.random_normal_initializer(),
-        bias_init=tf.random_normal_initializer(),
+        weight_init=tf.random_uniform_initializer(minval=-1, maxval=1),
+        bias_init=tf.random_uniform_initializer(minval=-1, maxval=1),
         name="net",
         net_type="DenseNet",
         is_debug=False,
         **kwargs,
     ):
         self.network = _create_functions[net_type](
             input_size,
@@ -223,15 +221,15 @@
         self,
         x_data: np.ndarray,
         y_data: np.ndarray,
         batch_size=None,
         callbacks: List = None,
         verbose="auto",
         **kwargs,
-    ) -> keras.callbacks.History:
+    ) -> Union[float, List[float]]:
         """
         Evaluate network on passed dataset and return evaluate history
 
         Parameters
         ----------
         x_data: np.ndarray
             Array of input vectors
@@ -242,16 +240,18 @@
         callbacks: list
             List of tensorflow callbacks for evaluate function
         verbose: int
             Output accompanying evaualing
 
         Returns
         -------
-        history: tf.keras.callbacks.History
-            History of evaluating
+        history: Union[float, List[float]]
+            Scalar test loss (if the model has a single output and no metrics)
+            or list of scalars (if the model has multiple outputs
+            and/or metrics).
         """
         if self._is_debug:
             if callbacks is not None:
                 callbacks.append(
                     tf.keras.callbacks.CSVLogger(
                         f"log_{self.get_name}.csv", separator=",", append=False
                     )
@@ -324,17 +324,17 @@
 
         Returns
         -------
 
         """
         config = self.to_dict(**kwargs)
         with open(path + ".apg", "w") as f:
-            f.write(HEADER_OF_FILE + json.dumps(config, indent=2))
+            f.write(HEADER_OF_APG_FILE + json.dumps(config, indent=2))
 
-    def from_dict(self, config, **kwargs):
+    def from_dict(self, config: dict, **kwargs):
         """
         Import neural network from dictionary
 
         Parameters
         ----------
         config: dict
             Network configuration
@@ -342,31 +342,30 @@
         Returns
         -------
 
         """
         self._shape = config["block_size"]
         self.network.from_dict(config, **kwargs)
 
-    def from_file(self, path, **kwargs):
+    def from_file(self, path: str, **kwargs):
         """
         Import neural network as parameters from file
 
         Parameters
         ----------
         path:
             path to file with name, without extension
         kwargs
 
         Returns
         -------
 
         """
         with open(path + ".apg", "r") as f:
-            for header in range(HEADER_OF_FILE.count("\n")):
-                # TODO: check version compability
+            for header in range(HEADER_OF_APG_FILE.count("\n")):
                 _ = f.readline()
             config_str = ""
             for line in f:
                 config_str += line
             config = json.loads(config_str)
             self.network.from_dict(config)
             self.set_name(config["name"])
@@ -512,9 +511,9 @@
     #         decorator_params=decorator_params,
     #         **kwargs,
     #     )
     #
     #     return res
 
 
-_create_functions = defaultdict(lambda: DenseNet)
-_create_functions["DenseNet"] = DenseNet
+_create_functions = defaultdict(lambda: TensorflowDenseNet)
+_create_functions["DenseNet"] = TensorflowDenseNet
```

### Comparing `degann-0.3/degann/networks/layers/dense.py` & `degann-1.0/degann/networks/layers/tf_dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return None
     res = {}
     for pair in params:
         res[pair[0]] = pair[1]
     return res
 
 
-class MyDense(keras.layers.Layer):
+class TensorflowDense(keras.layers.Layer):
     def __init__(
         self,
         input_dim=32,
         units=32,
         activation_func: str = "linear",
         weight_initializer=tf.random_normal_initializer(),
         bias_initializer=tf.random_normal_initializer(),
@@ -48,15 +48,15 @@
 
         if not isinstance(decorator_params, dict) and decorator_params is not None:
             raise "Additional parameters for activation function must be dictionary"
 
         if input_dim == 0 or units == 0:
             raise "Layer cannot have zero inputs or zero size"
 
-        super(MyDense, self).__init__(**kwargs)
+        super(TensorflowDense, self).__init__(**kwargs)
         w_init = weight_initializer
         self.w = tf.Variable(
             initial_value=w_init(shape=(input_dim, units), dtype="float32"),
             name=f"Var_w_{self.name}",
             trainable=True,
         )
         b_init = bias_initializer
@@ -129,14 +129,15 @@
         }
 
         return res
 
     def from_dict(self, config):
         """
         Restore layer from dictionary of parameters
+
         Parameters
         ----------
         config
 
         Returns
         -------
```

### Comparing `degann-0.3/degann/networks/nn_code.py` & `degann-1.0/degann/expert/nn_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 }
 reverse_act_to_hex = {v: k for k, v in act_to_hex.items()}
 
 alph_n_full = "0123456789abcdef"
 alph_n_div3 = "0369cf"
 alph_n_div2 = "02468ace"
 alph_n_div4 = "048c"
-alph_a = "0689"
 
+alphabet_activations_cut = "0689"
+alphabet_activations = "0123456789abc"
 
-def encode(nn: imodel.IModel, offset: int = None):
+
+def encode(nn: imodel.IModel, offset: int = None) -> str:
     blocks = nn.get_shape
     activations = nn.get_activations
     res = ""
 
     offset = min(blocks) if offset is None else offset
     for layer, act in zip(blocks, activations):
         curr = hex(layer - offset)[2:] + act_to_hex[act]
```

### Comparing `degann-0.3/degann/networks/optimizers.py` & `degann-1.0/degann/networks/optimizers.py`

 * *Files identical despite different names*

### Comparing `degann-0.3/degann/networks/utils.py` & `degann-1.0/degann/networks/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,55 +6,14 @@
 from typing import Tuple
 
 import numpy as np
 
 from degann.networks import imodel
 
 
-def export_network(path: str, net: imodel.IModel) -> None:
-    """
-    !DEPRECATED!
-    This method saves the neural network to a file
-    using the pickle library functions.
-
-    Parameters
-    ----------
-    path: str
-        Path to file
-    net: network.INetwork
-        Neural network to be saved
-    Returns
-    -------
-    None
-    """
-    with open(path, "wb") as file:
-        pickle.dump(net, file)
-
-
-def import_network(path: str) -> imodel.IModel:
-    """
-    !DEPRECATED!
-    This method loads the neural network from a file
-    using the pickle library functions.
-
-    Parameters
-    ----------
-    path: str
-        Path to file
-
-    Returns
-    -------
-    net: network.INetwork
-        Neural network to be loaded
-    """
-    with open(path, "rb") as file:
-        net = pickle.load(file)
-    return net
-
-
 def import_csv_table(path: str) -> np.ndarray:
     """
     Import csv table as numpy array.
 
     Parameters
     ----------
     path: str
```

### Comparing `degann-0.3/degann.egg-info/PKG-INFO` & `degann-1.0/degann.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 0.3
+Version: 1.0
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -20,28 +20,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-0.3-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
 - Choosing the Best Neural Network from Several for Fixed Training Parameters
 - Iterating over training parameters with choosing the best neural network for each set
-- Export neural networks as a function in C++
+- Export Neural Networks as a function in C++
 - Export Neural Networks as a Parameter Set
 - Import Neural Networks from a Parameter Set
 - Building a dataset with complete training results for approximating the solution of a differential equation for each neural network that participated in training
+- Advanced search for optimal topology using a language that describes the topology of a neural network
+- Random search for optimal neural network topology
+- Method for simulating annealing of optimal neural network topology
+- Expert system for automatic selection of optimal parameters for algorithms for searching neural network topologies
 
 ## Install
 
 ### Manual
 Download the repository as a zip archive, unpack and run the command from the root of the repository
 ```bash
 pip install -r requirements.txt
```

### Comparing `degann-0.3/degann.egg-info/SOURCES.txt` & `degann-1.0/degann.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,28 @@
 degann.egg-info/dependency_links.txt
 degann.egg-info/requires.txt
 degann.egg-info/top_level.txt
 degann/equations/__init__.py
 degann/equations/equation_utils.py
 degann/equations/simple_equation.py
 degann/equations/system_ode.py
+degann/expert/__init__.py
+degann/expert/generate.py
+degann/expert/nn_code.py
+degann/expert/search_algorithms.py
+degann/expert/selector.py
+degann/expert/trainer.py
 degann/networks/__init__.py
-degann/networks/__main__.py
 degann/networks/activations.py
 degann/networks/callbacks.py
 degann/networks/config_format.py
 degann/networks/cpp_utils.py
-degann/networks/expert.py
-degann/networks/generate.py
 degann/networks/imodel.py
 degann/networks/layer_creator.py
 degann/networks/losses.py
 degann/networks/metrics.py
-degann/networks/nn_code.py
 degann/networks/optimizers.py
-degann/networks/trainer.py
-degann/networks/unrefactored.py
 degann/networks/utils.py
 degann/networks/layers/__init__.py
-degann/networks/layers/dense.py
+degann/networks/layers/tf_dense.py
 degann/networks/topology/__init__.py
-degann/networks/topology/densenet.py
-degann/testlaunches/__init__.py
-degann/testlaunches/__main__.py
-degann/testlaunches/build_tables.py
-degann/testlaunches/experiments.py
-degann/testlaunches/functions.py
+degann/networks/topology/tf_densenet.py
```

### Comparing `degann-0.3/setup.py` & `degann-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "numpy~=1.23.5",
         "scipy~=1.10.1",
         "tensorflow~=2.12.0",
     ],
     python_requires=">=3.10",
     keywords=["python", "ode", "differential equation", "neural network"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Physics",
```

