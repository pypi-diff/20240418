# Comparing `tmp/irtorch-0.0.3.tar.gz` & `tmp/irtorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irtorch-0.0.3.tar", last modified: Thu Apr  4 11:56:24 2024, max compression
+gzip compressed data, was "irtorch-0.0.4.tar", last modified: Thu Apr 18 13:28:33 2024, max compression
```

## Comparing `irtorch-0.0.3.tar` & `irtorch-0.0.4.tar`

### file list

```diff
@@ -1,98 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.319711 irtorch-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2227 2024-04-04 11:56:24.319711 irtorch-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-03-08 15:11:37.000000 irtorch-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.257140 irtorch-0.0.3/irtorch/
--rw-rw-rw-   0        0        0      255 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/__init__.py
--rw-rw-rw-   0        0        0    14040 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/_internal_utils.py
--rw-rw-rw-   0        0        0     3279 2024-02-25 18:33:40.000000 irtorch-0.0.3/irtorch/activation_functions.py
--rw-rw-rw-   0        0        0     1000 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/config.py
--rw-rw-rw-   0        0        0     5326 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/cross_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.246655 irtorch-0.0.3/irtorch/datasets/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.277765 irtorch-0.0.3/irtorch/datasets/big_five/
--rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.0.3/irtorch/datasets/big_five/big_five.pt
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.281717 irtorch-0.0.3/irtorch/datasets/national_mathematics/
--rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_1.pt
--rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_2.pt
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.300421 irtorch-0.0.3/irtorch/datasets/swedish_sat/
--rw-rw-rw-   0        0        0 12183084 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
--rw-rw-rw-   0        0        0 12183079 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
--rw-rw-rw-   0        0        0       80 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
--rw-rw-rw-   0        0        0       82 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.302421 irtorch-0.0.3/irtorch/estimation_algorithms/
--rw-rw-rw-   0        0        0      104 2024-02-08 14:34:51.000000 irtorch-0.0.3/irtorch/estimation_algorithms/__init__.py
--rw-rw-rw-   0        0        0    14839 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/estimation_algorithms/aeirt.py
--rw-rw-rw-   0        0        0     2893 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/estimation_algorithms/base_irt_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.305967 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/
--rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/__init__.py
--rw-rw-rw-   0        0        0      751 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/base_encoder.py
--rw-rw-rw-   0        0        0     1427 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/bounded_encoder.py
--rw-rw-rw-   0        0        0     1361 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/standard_encoder.py
--rw-rw-rw-   0        0        0     1478 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/estimation_algorithms/encoders/variational_encoder.py
--rw-rw-rw-   0        0        0    14716 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/estimation_algorithms/vaeirt.py
--rw-rw-rw-   0        0        0     4002 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/gaussian_mixture_model.py
--rw-rw-rw-   0        0        0    67068 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt.py
--rw-rw-rw-   0        0        0    34307 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt_evaluator.py
--rw-rw-rw-   0        0        0    55406 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/irt_plotter.py
--rw-rw-rw-   0        0        0    62880 2024-04-04 11:55:33.000000 irtorch-0.0.3/irtorch/irt_scorer.py
--rw-rw-rw-   0        0        0     2644 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/latent_variable_functions.py
--rw-rw-rw-   0        0        0     8310 2024-02-20 20:30:27.000000 irtorch-0.0.3/irtorch/layers.py
--rw-rw-rw-   0        0        0     5099 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/load_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.307967 irtorch-0.0.3/irtorch/models/
--rw-rw-rw-   0        0        0      115 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/models/__init__.py
--rw-rw-rw-   0        0        0     8057 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/base_irt_model.py
--rw-rw-rw-   0        0        0    13816 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/monotone_nn.py
--rw-rw-rw-   0        0        0    13397 2024-04-03 14:22:41.000000 irtorch-0.0.3/irtorch/models/parametric.py
--rw-rw-rw-   0        0        0     6868 2024-02-25 18:33:40.000000 irtorch-0.0.3/irtorch/outlier_detector.py
--rw-rw-rw-   0        0        0     3163 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/quantile_mv_normal.py
--rw-rw-rw-   0        0        0      767 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/timer.py
--rw-rw-rw-   0        0        0     6670 2024-03-08 13:28:02.000000 irtorch-0.0.3/irtorch/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:24.276945 irtorch-0.0.3/irtorch.egg-info/
--rw-rw-rw-   0        0        0     2227 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2098 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.0.3/irtorch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 11:56:24.000000 irtorch-0.0.3/irtorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 11:56:24.319711 irtorch-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1099 2024-04-04 11:55:33.000000 irtorch-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:28.045904 irtorch-0.0.3/tests/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:28.499829 irtorch-0.0.3/tests/__pycache__/
--rw-rw-rw-   0        0        0     5098 2024-04-04 11:56:28.047904 irtorch-0.0.3/tests/__pycache__/test_activation_functions.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    13774 2024-04-04 11:56:28.059825 irtorch-0.0.3/tests/__pycache__/test_aeirt.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    30081 2024-04-04 11:56:28.070861 irtorch-0.0.3/tests/__pycache__/test_base_irt_model.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     9527 2024-04-04 11:56:28.074860 irtorch-0.0.3/tests/__pycache__/test_config.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    15714 2024-04-04 11:56:28.080860 irtorch-0.0.3/tests/__pycache__/test_gaussian_mixture_torch.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0      175 2024-04-04 11:56:28.081861 irtorch-0.0.3/tests/__pycache__/test_integration.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    33306 2024-04-04 11:56:28.092861 irtorch-0.0.3/tests/__pycache__/test_internal_utils.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    86867 2024-04-04 11:56:28.117860 irtorch-0.0.3/tests/__pycache__/test_irt_evaluator.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     3508 2024-04-04 11:56:28.121860 irtorch-0.0.3/tests/__pycache__/test_irt_plotter.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    50778 2024-04-04 11:56:28.170475 irtorch-0.0.3/tests/__pycache__/test_irt_scorer.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    21348 2024-04-04 11:56:28.178475 irtorch-0.0.3/tests/__pycache__/test_latent_variable_functions.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    32202 2024-04-04 11:56:28.440395 irtorch-0.0.3/tests/__pycache__/test_layers.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    21163 2024-04-04 11:56:28.444405 irtorch-0.0.3/tests/__pycache__/test_load_dataset.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    44373 2024-04-04 11:56:28.452909 irtorch-0.0.3/tests/__pycache__/test_monotone_nn.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    12294 2024-04-04 11:56:28.452909 irtorch-0.0.3/tests/__pycache__/test_outlier_detector.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    48430 2024-04-04 11:56:28.468585 irtorch-0.0.3/tests/__pycache__/test_parametric.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    17322 2024-04-04 11:56:28.484207 irtorch-0.0.3/tests/__pycache__/test_quantile_mv_normal.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    19709 2024-04-04 11:56:28.484207 irtorch-0.0.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    20215 2024-04-04 11:56:28.499829 irtorch-0.0.3/tests/__pycache__/test_vaeirt.cpython-311-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.0.3/tests/test_activation_functions.py
--rw-rw-rw-   0        0        0     4099 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_aeirt.py
--rw-rw-rw-   0        0        0     5085 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_base_irt_model.py
--rw-rw-rw-   0        0        0      984 2024-02-21 12:30:49.000000 irtorch-0.0.3/tests/test_config.py
--rw-rw-rw-   0        0        0     2196 2024-04-04 11:55:33.000000 irtorch-0.0.3/tests/test_gaussian_mixture_torch.py
--rw-rw-rw-   0        0        0     9673 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_integration.py
--rw-rw-rw-   0        0        0     7678 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_internal_utils.py
--rw-rw-rw-   0        0        0    17038 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_irt_evaluator.py
--rw-rw-rw-   0        0        0     3632 2024-02-25 18:33:40.000000 irtorch-0.0.3/tests/test_irt_plotter.py
--rw-rw-rw-   0        0        0    14999 2024-04-04 11:55:33.000000 irtorch-0.0.3/tests/test_irt_scorer.py
--rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_latent_variable_functions.py
--rw-rw-rw-   0        0        0     5111 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_layers.py
--rw-rw-rw-   0        0        0     1803 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_load_dataset.py
--rw-rw-rw-   0        0        0     9007 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_monotone_nn.py
--rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_outlier_detector.py
--rw-rw-rw-   0        0        0    10121 2024-04-03 14:22:41.000000 irtorch-0.0.3/tests/test_parametric.py
--rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.0.3/tests/test_quantile_mv_normal.py
--rw-rw-rw-   0        0        0     4670 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_utils.py
--rw-rw-rw-   0        0        0     6369 2024-03-08 13:28:02.000000 irtorch-0.0.3/tests/test_vaeirt.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.010614 irtorch-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2158 2024-04-18 13:28:33.009615 irtorch-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-18 13:25:52.000000 irtorch-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.970152 irtorch-0.0.4/irtorch/
+-rw-rw-rw-   0        0        0      255 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/__init__.py
+-rw-rw-rw-   0        0        0    14040 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/_internal_utils.py
+-rw-rw-rw-   0        0        0     3279 2024-02-25 18:33:40.000000 irtorch-0.0.4/irtorch/activation_functions.py
+-rw-rw-rw-   0        0        0     1000 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/config.py
+-rw-rw-rw-   0        0        0     5326 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/cross_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.958153 irtorch-0.0.4/irtorch/datasets/
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.983152 irtorch-0.0.4/irtorch/datasets/big_five/
+-rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.0.4/irtorch/datasets/big_five/big_five.pt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.987156 irtorch-0.0.4/irtorch/datasets/national_mathematics/
+-rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_1.pt
+-rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_2.pt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.991155 irtorch-0.0.4/irtorch/datasets/swedish_sat/
+-rw-rw-rw-   0        0        0  1601324 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
+-rw-rw-rw-   0        0        0  1601319 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
+-rw-rw-rw-   0        0        0       80 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
+-rw-rw-rw-   0        0        0       82 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.993156 irtorch-0.0.4/irtorch/estimation_algorithms/
+-rw-rw-rw-   0        0        0      104 2024-02-08 14:34:51.000000 irtorch-0.0.4/irtorch/estimation_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    14839 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/estimation_algorithms/aeirt.py
+-rw-rw-rw-   0        0        0     2893 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/estimation_algorithms/base_irt_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.996157 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/
+-rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/base_encoder.py
+-rw-rw-rw-   0        0        0     1427 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/bounded_encoder.py
+-rw-rw-rw-   0        0        0     1361 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/standard_encoder.py
+-rw-rw-rw-   0        0        0     1478 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/variational_encoder.py
+-rw-rw-rw-   0        0        0    14716 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/estimation_algorithms/vaeirt.py
+-rw-rw-rw-   0        0        0     4002 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/gaussian_mixture_model.py
+-rw-rw-rw-   0        0        0    67843 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/irt.py
+-rw-rw-rw-   0        0        0    34296 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/irt_evaluator.py
+-rw-rw-rw-   0        0        0    55406 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/irt_plotter.py
+-rw-rw-rw-   0        0        0    62880 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/irt_scorer.py
+-rw-rw-rw-   0        0        0     2644 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/latent_variable_functions.py
+-rw-rw-rw-   0        0        0     8310 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/layers.py
+-rw-rw-rw-   0        0        0     5137 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/load_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.000615 irtorch-0.0.4/irtorch/models/
+-rw-rw-rw-   0        0        0      308 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/__init__.py
+-rw-rw-rw-   0        0        0     8219 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/base_irt_model.py
+-rw-rw-rw-   0        0        0     6441 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/generalized_partial_credit.py
+-rw-rw-rw-   0        0        0    13816 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/models/monotone_nn.py
+-rw-rw-rw-   0        0        0     7627 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/nominal_response.py
+-rw-rw-rw-   0        0        0     4895 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/one_parameter_logistic.py
+-rw-rw-rw-   0        0        0     5240 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/two_parameter_logistic.py
+-rw-rw-rw-   0        0        0     6868 2024-02-25 18:33:40.000000 irtorch-0.0.4/irtorch/outlier_detector.py
+-rw-rw-rw-   0        0        0     3163 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/quantile_mv_normal.py
+-rw-rw-rw-   0        0        0      767 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/timer.py
+-rw-rw-rw-   0        0        0     6670 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.982153 irtorch-0.0.4/irtorch.egg-info/
+-rw-rw-rw-   0        0        0     2158 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2151 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.0.4/irtorch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:28:33.010614 irtorch-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-04-18 13:25:53.000000 irtorch-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.009615 irtorch-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.0.4/tests/test_activation_functions.py
+-rw-rw-rw-   0        0        0     4099 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_aeirt.py
+-rw-rw-rw-   0        0        0      984 2024-02-21 12:30:49.000000 irtorch-0.0.4/tests/test_config.py
+-rw-rw-rw-   0        0        0     2196 2024-04-04 11:55:33.000000 irtorch-0.0.4/tests/test_gaussian_mixture_torch.py
+-rw-rw-rw-   0        0        0     9680 2024-04-18 13:25:53.000000 irtorch-0.0.4/tests/test_integration.py
+-rw-rw-rw-   0        0        0     7678 2024-04-03 14:22:41.000000 irtorch-0.0.4/tests/test_internal_utils.py
+-rw-rw-rw-   0        0        0    17038 2024-04-03 14:22:41.000000 irtorch-0.0.4/tests/test_irt_evaluator.py
+-rw-rw-rw-   0        0        0     3632 2024-02-25 18:33:40.000000 irtorch-0.0.4/tests/test_irt_plotter.py
+-rw-rw-rw-   0        0        0    14999 2024-04-04 11:55:33.000000 irtorch-0.0.4/tests/test_irt_scorer.py
+-rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_latent_variable_functions.py
+-rw-rw-rw-   0        0        0     5111 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_layers.py
+-rw-rw-rw-   0        0        0     1799 2024-04-18 13:25:53.000000 irtorch-0.0.4/tests/test_load_dataset.py
+-rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_outlier_detector.py
+-rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_quantile_mv_normal.py
+-rw-rw-rw-   0        0        0     4670 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_utils.py
+-rw-rw-rw-   0        0        0     6369 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_vaeirt.py
```

### Comparing `irtorch-0.0.3/LICENSE.txt` & `irtorch-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/PKG-INFO` & `irtorch-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -36,17 +36,15 @@
 To cite IRTorch in publications use:
 
 Wallmark, J. (2024). IRTorch: Item response theory with Python (Version X.X) [Software]. GitHub. https://github.com/joakimwallmark/irtorch
 
 Or use the following BibTeX entry:
 
 ```bibtex
-@misc{irtorch2024,
+@manual{irtorch,
+  title = {{IRTorch}: Item response theory with Python},
   author = {Wallmark, Joakim},
-  title = {IRTorch: Item response theory with Python},
   year = {2024},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/joakimwallmark/irtorch}},
-  version = {X.X}
+  note = {Version X.X},
+  url = {https://github.com/joakimwallmark/irtorch}
 }
 ```
```

### Comparing `irtorch-0.0.3/README.md` & `irtorch-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 To cite IRTorch in publications use:
 
 Wallmark, J. (2024). IRTorch: Item response theory with Python (Version X.X) [Software]. GitHub. https://github.com/joakimwallmark/irtorch
 
 Or use the following BibTeX entry:
 
 ```bibtex
-@misc{irtorch2024,
+@manual{irtorch,
+  title = {{IRTorch}: Item response theory with Python},
   author = {Wallmark, Joakim},
-  title = {IRTorch: Item response theory with Python},
   year = {2024},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/joakimwallmark/irtorch}},
-  version = {X.X}
+  note = {Version X.X},
+  url = {https://github.com/joakimwallmark/irtorch}
 }
 ```
```

### Comparing `irtorch-0.0.3/irtorch/_internal_utils.py` & `irtorch-0.0.4/irtorch/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/activation_functions.py` & `irtorch-0.0.4/irtorch/activation_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/config.py` & `irtorch-0.0.4/irtorch/config.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/cross_validation.py` & `irtorch-0.0.4/irtorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/datasets/big_five/big_five.pt` & `irtorch-0.0.4/irtorch/datasets/big_five/big_five.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_1.pt` & `irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_1.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/datasets/national_mathematics/mathematics_2.pt` & `irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_2.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/aeirt.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/aeirt.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/base_irt_algorithm.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/base_irt_algorithm.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/base_encoder.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/bounded_encoder.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/bounded_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/standard_encoder.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/standard_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/encoders/variational_encoder.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/variational_encoder.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/estimation_algorithms/vaeirt.py` & `irtorch-0.0.4/irtorch/estimation_algorithms/vaeirt.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/gaussian_mixture_model.py` & `irtorch-0.0.4/irtorch/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/irt.py` & `irtorch-0.0.4/irtorch/irt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 import torch
 import pandas as pd
 from plotly import graph_objects as go
-from irtorch.models import BaseIRTModel
-from irtorch.models import Parametric
-from irtorch.models import MonotoneNN
+from irtorch.models import BaseIRTModel, MonotoneNN, OneParameterLogistic, TwoParameterLogistic, GeneralizedPartialCredit, NominalResponse
 from irtorch.estimation_algorithms import AEIRT, VAEIRT
 from irtorch.irt_scorer import IRTScorer
 from irtorch.irt_plotter import IRTPlotter
 from irtorch.irt_evaluator import IRTEvaluator
 from irtorch.estimation_algorithms.encoders import BaseEncoder
 
 logger = logging.getLogger('irtorch')
@@ -27,15 +25,15 @@
         - "2PL": Two-parameter logistic model.
         - "GPC": Generalized partial credit model.
         - "NR": Nominal response model.
         - "MNN": Monotone neural network model.
         - "MMCNN": Monotone multiple choice neural network model.
         
         Default is None and uses either MNN or MMCNN depending on whether mc_correct is provided or not. 
-        An instantiated model can also be provided, see :class:`irtorch.models.parametric.Parametric` and :class:`irtorch.models.monotone_nn.MonotoneNN` for model specific details.
+        An instantiated model inheriting :class:`irtorch.models.BaseIRTModel` can also be provided, see :doc:`irt_models` for model specific details.
     estimation_algorithm : str, optional
         The estimation algorithm to use. Available options are
 
         - "AE" for autoencoder. This is the default. 
         - "VAE" for variational autoencoder.
 
     latent_variables : int, optional
@@ -90,23 +88,40 @@
             if item_categories is None:
                 if data is None:
                     raise ValueError("Either an instantiated model, item_categories or data must be provided to initialize the model.")
                 else:
                     # replace nan with -inf to get max
                     item_categories = (torch.where(~data.isnan(), data, torch.tensor(float('-inf'))).max(dim=0).values + 1).int().tolist()
 
-            if model in ["1PL", "2PL", "3PL", "GPC", "NR"]:
-                self.model = Parametric(
+            if model == "1PL":
+                self.model = OneParameterLogistic(
+                    latent_variables=latent_variables,
+                    items=len(item_categories),
+                    item_z_relationships=item_z_relationships
+                )
+            elif model == "2PL":
+                self.model = TwoParameterLogistic(
+                    latent_variables=latent_variables,
+                    items=len(item_categories),
+                    item_z_relationships=item_z_relationships
+                )
+            elif model == "GPC":
+                self.model = GeneralizedPartialCredit(
                     latent_variables=latent_variables,
                     item_categories=item_categories,
-                    model=model,
+                    item_z_relationships=item_z_relationships
+                )
+            elif model == "NR":
+                self.model = NominalResponse(
+                    latent_variables=latent_variables,
+                    item_categories=item_categories,
+                    item_z_relationships=item_z_relationships,
                     model_missing=model_missing,
                     mc_correct=mc_correct,
-                    item_z_relationships=item_z_relationships,
-                    reference_category=nominal_reference_category,
+                    reference_category=nominal_reference_category
                 )
             elif model in ["MMCNN", "MNN"] or model is None:
                 if hidden_layers_decoder is None:  # 1 layer with 2x number of categories as neurons is default
                     hidden_layers_decoder = [3]
 
                 self.model = MonotoneNN(
                     latent_variables=latent_variables,
@@ -521,32 +536,32 @@
             groups = groups,
             latent_variable = latent_variable,
             scale = scale,
             population_z = population_z,
             **kwargs
         )
 
-    def item_parameters(self, IRT_format = False) -> pd.DataFrame:
+    def item_parameters(self, irt_format = False) -> pd.DataFrame:
         """
         For parametric models, get the item parameters for a fitted model.
 
         Parameters
         ----------
-        IRT_format : bool, optional
-            Only for unidimensional models. Whether to return the item parameters in traditional IRT format. Otherwise returns weights and biases. (default is False)
+        irt_format : bool, optional
+            Only for unidimensional parametric models. Whether to return the item parameters in traditional IRT format. Otherwise returns weights and biases. (default is False)
 
         Returns
         -------
         pd.DataFrame
             A dataframe with the item parameters.
         """
-        if isinstance(self.model, Parametric):
-            return self.model.item_parameters(IRT_format)
+        if hasattr(self.model, 'item_parameters'):
+            return self.model.item_parameters(irt_format)
         else:
-            raise ValueError("Item parameters are only available for parametric models.")
+            raise AttributeError("item_parameters method is not available for the chosen IRT model.")
 
     def infit_outfit(
         self,
         data: torch.Tensor = None,
         z: torch.Tensor = None,
         z_estimation_method: str = "ML",
         level: str = "item",
@@ -760,15 +775,15 @@
         self,
         data: torch.Tensor = None,
         z: torch.Tensor = None,
         z_estimation_method: str = "ML",
         average_over: str = "none",
     ) -> torch.Tensor:
         """
-        Calculate the residuals of the model for the supplied data. 
+        Compute model residuals using the supplied data.  
         
         For multiple choice models, the residuals are computed as 1 - the probability of the selected response option.
         For other models, the residuals are computed as the difference between the observed and model expected item scores.
 
         Parameters
         ----------
         data : torch.Tensor
```

### Comparing `irtorch-0.0.3/irtorch/irt_evaluator.py` & `irtorch-0.0.4/irtorch/irt_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self,
         data: torch.Tensor = None,
         z: torch.Tensor = None,
         z_estimation_method: str = "ML",
         average_over: str = "none",
     ) -> torch.Tensor:
         """
-        Calculate the residuals of the model for the supplied data. 
+        Compute model residuals using the supplied data. 
         
         For multiple choice models, the residuals are computed as 1 - the probability of the selected response option.
         For other models, the residuals are computed as the difference between the observed and model expected item scores.
 
         Parameters
         ----------
         data : torch.Tensor
```

### Comparing `irtorch-0.0.3/irtorch/irt_plotter.py` & `irtorch-0.0.4/irtorch/irt_plotter.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/irt_scorer.py` & `irtorch-0.0.4/irtorch/irt_scorer.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/latent_variable_functions.py` & `irtorch-0.0.4/irtorch/latent_variable_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/layers.py` & `irtorch-0.0.4/irtorch/layers.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/load_dataset.py` & `irtorch-0.0.4/irtorch/load_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
     return data
 
 def swedish_sat_verbal() -> tuple[torch.Tensor, list[int]]:
     """
-    Load the verbal part of the Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data.
+    Load a sample from the verbal part of the Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data.
 
     Returns
     -------
     tuple (torch.Tensor, list[int])
         A tuple containing the loaded dataset and the correct item responses.
     """
     try:
@@ -58,15 +58,15 @@
     except Exception as e:
         raise RuntimeError("Failed to load correct item responses") from e
 
     return data - 1, correct_category
 
 def swedish_sat_quantitative() -> tuple[torch.Tensor, list[int]]:
     """
-    Load the quantitative part Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data.
+    Load a sample from the quantitative part Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data.
 
     Returns
     -------
     tuple (torch.Tensor, list[int])
         A tuple containing the loaded dataset and the correct item responses.
     """
     try:
@@ -82,15 +82,15 @@
     except Exception as e:
         raise RuntimeError("Failed to load correct item responses") from e
 
     return data - 1, correct_category
 
 def swedish_sat() -> tuple[torch.Tensor, list[int]]:
     """
-    Load the full Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data. The first 80 items are from the quantitative test, and the last 80 items are from the verbal test. 
+    Load a sample from Swedish SAT dataset and the correct item responses. The correct item responses start from one, and thus a 1 corresponds to a response of 0 in the data. The first 80 items are from the quantitative test, and the last 80 items are from the verbal test. 
 
     Returns
     -------
     tuple (torch.Tensor, list[int])
         A tuple containing the loaded dataset and the correct item responses.
     """
     data_quant, correct_quant = swedish_sat_quantitative()
@@ -99,15 +99,15 @@
     # concatenate the correct item responses
     correct_category = correct_quant + correct_verb
 
     return data, correct_category
 
 def swedish_sat_binary() -> torch.Tensor:
     """
-    Load the full Swedish SAT dataset coded as incorrect/correct. 
+    Load a sample from Swedish SAT dataset coded as incorrect/correct. 
 
     Returns
     -------
     torch.Tensor
         A tuple containing the loaded dataset.
     """
     data_quant, correct_quant = swedish_sat_quantitative()
```

### Comparing `irtorch-0.0.3/irtorch/models/base_irt_model.py` & `irtorch-0.0.4/irtorch/models/base_irt_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,30 @@
 
         Returns
         -------
         output : torch.Tensor
             Output tensor.
         """
 
-    @abstractmethod
     def probabilities_from_output(self, output: torch.Tensor) -> torch.Tensor:
         """
         Compute probabilities from the output tensor from the forward method.
 
         Parameters
         ----------
         output : torch.Tensor
             Output tensor from the forward pass.
 
         Returns
         -------
         torch.Tensor
             3D tensor with dimensions (respondents, items, item categories)
         """
+        reshaped_output = output.reshape(-1, self.max_item_responses)
+        return F.softmax(reshaped_output, dim=1).reshape(output.shape[0], self.items, self.max_item_responses)
 
     def item_probabilities(self, z: torch.Tensor) -> torch.Tensor:
         """
         Returns the probabilities for each possible response for all items.
 
         Parameters
         ----------
```

### Comparing `irtorch-0.0.3/irtorch/models/monotone_nn.py` & `irtorch-0.0.4/irtorch/models/monotone_nn.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/models/parametric.py` & `irtorch-0.0.4/irtorch/models/nominal_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,66 @@
-import logging
 import pandas as pd
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 from irtorch.models.base_irt_model import BaseIRTModel
 
-logger = logging.getLogger('irtorch')
-
-class Parametric(BaseIRTModel):
+class NominalResponse(BaseIRTModel):
     """
-    Parametric IRT model. Currently supports 1PL, 2PL, 3PL, Generalized partial credit and nominal models.
+    Nominal response IRT model.
 
     Parameters
     ----------
     latent_variables : int
         Number of latent variables.
     item_categories : list[int]
         Number of categories for each item. One integer for each item. Missing responses exluded.
-    model : str
-        Type of parametric model. Can be "1PL", "2PL", "3PL", "GPC" or "NR".
+    item_z_relationships : torch.Tensor, optional
+        A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
     model_missing : bool, optional
         Whether to model missing item responses as separate item response categories. (Default: False)
     mc_correct : list[int], optional
         The correct response category for each item. If specified, the logits for the correct responses are cumulative logits. (Default: None)
-    item_z_relationships : torch.Tensor, optional
-        A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
     reference_category : bool, optional
-        Only for the nomimal model. Whether to use the first category as an unparameterized reference category. (Default: False and uses the original parameterization given by Bock(1972))
+        Whether to use the first category as an unparameterized reference category. (Default: False and uses the original parameterization given by Bock(1972))
     """
     def __init__(
         self,
         latent_variables: int,
         item_categories: list[int],
-        model: str,
+        item_z_relationships: torch.Tensor = None,
         model_missing: bool = False,
         mc_correct: list[int] = None,
-        item_z_relationships: torch.Tensor = None,
         reference_category: bool = False
     ):
         super().__init__(latent_variables=latent_variables, item_categories=item_categories, model_missing=model_missing, mc_correct=mc_correct)
         if item_z_relationships is not None:
             if item_z_relationships.shape != (len(item_categories), latent_variables):
                 raise ValueError(
                     f"latent_item_connections must have shape ({len(item_categories)}, {latent_variables})."
                 )
             assert(item_z_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
             assert(torch.all(item_z_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
-        if model not in ["1PL", "2PL", "3PL", "GPC", "NR"]:
-            raise ValueError("model_type must be one of '1PL', '2PL', '3PL', 'GPC', 'NR'.")
-        if model in ["1PL", "2PL", "3PL"]:
-            item_categories = [2] * len(item_categories)
 
-        self.model = model
         self.output_size = self.items * self.max_item_responses
 
-        if model == "1PL":
-            free_weights = torch.ones(latent_variables)
-        elif model in ["2PL", "3PL"]:
-            free_weights = torch.zeros(self.items, self.max_item_responses - 1, latent_variables)
-            for item, item_cat in enumerate(self.modeled_item_responses):
-                if item_z_relationships is not None:
-                    free_weights[item, 0:item_cat, :] = item_z_relationships[item, :]
-                else:
-                    free_weights[item, 0:item_cat, :] = 1.0
-            free_weights = free_weights.reshape(-1, latent_variables)
-        elif model == "NR":
-            free_weights = torch.zeros(self.items, self.max_item_responses, latent_variables)
-            for item, item_cat in enumerate(self.modeled_item_responses):
-                start_1 = 1 if reference_category else 0
-                if item_z_relationships is not None:
-                    free_weights[item, start_1:item_cat, :] = item_z_relationships[item, :]
-                else:
-                    free_weights[item, start_1:item_cat, :] = 1.0
-            free_weights = free_weights.reshape(-1, latent_variables)
-        elif model == "GPC":
-            free_weights = torch.ones(self.items, latent_variables)
-            self.register_buffer("gpc_weight_multiplier", torch.arange(0, self.max_item_responses).repeat(self.items))
+        free_weights = torch.zeros(self.items, self.max_item_responses, latent_variables)
+        for item, item_cat in enumerate(self.modeled_item_responses):
+            start_1 = 1 if reference_category else 0
             if item_z_relationships is not None:
-                for item, item_cat in enumerate(self.modeled_item_responses):
-                    free_weights[item, :] = item_z_relationships[item, :]
+                free_weights[item, start_1:item_cat, :] = item_z_relationships[item, :]
+            else:
+                free_weights[item, start_1:item_cat, :] = 1.0
 
-        if model == "1PL":
-            self.weight_param = nn.Parameter(torch.zeros(latent_variables))
-        elif model in ["2PL", "3PL", "NR", "GPC"]:
-            self.weight_param = nn.Parameter(torch.zeros(free_weights.sum().int()))
-            if model == "3PL":
-                self.guessing_param = nn.Parameter(torch.zeros(self.items))
+        free_weights = free_weights.reshape(-1, latent_variables)
+        self.weight_param = nn.Parameter(torch.zeros(free_weights.sum().int()))
 
-        number_of_bias_parameters = sum(self.modeled_item_responses) if model == "NR" and not reference_category else sum(self.modeled_item_responses) - self.items
+        number_of_bias_parameters = sum(self.modeled_item_responses) if not reference_category else sum(self.modeled_item_responses) - self.items
         self.bias_param = nn.Parameter(torch.zeros(number_of_bias_parameters))
         first_category = torch.zeros(self.items, self.max_item_responses)
-        if model != "NR" or reference_category:
+        if reference_category:
             first_category[:, 0] = 1.0
         first_category = first_category.reshape(-1)
         missing_category = torch.zeros(self.items, self.max_item_responses)
         for item, item_cat in enumerate(self.modeled_item_responses):
             missing_category[item, item_cat:self.max_item_responses] = 1.0
         missing_category = missing_category.reshape(-1)
         free_bias = (1 - first_category) * (1 - missing_category)
@@ -103,16 +69,14 @@
         self.register_buffer("missing_category", missing_category.bool())
         self.register_buffer("first_category", first_category.bool())
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         nn.init.normal_(self.weight_param, mean=1., std=0.01)
         nn.init.zeros_(self.bias_param)
-        if self.model == "3PL":
-            self.guessing_param.data.fill_(0.25)
     
     def forward(self, z: torch.Tensor) -> torch.Tensor:
         """
         Forward pass of the model.
 
         Parameters
         ----------
@@ -123,130 +87,55 @@
         -------
         output : torch.Tensor
             2D tensor. Rows are respondents and columns are item category logits.
         """
         bias = torch.zeros(self.output_size, device=z.device)
         bias[self.free_bias] = self.bias_param
         
-        if self.model == "1PL":
-            weighted_z = (self.weight_param * z).sum(dim=1, keepdim=True)
-        elif self.model in ["2PL", "3PL", "GPC"]:
-            weights = torch.zeros(self.items, self.latent_variables, device=z.device)
-            weights[self.free_weights] = self.weight_param
-            weighted_z = torch.matmul(z, weights.T).repeat_interleave(self.max_item_responses, dim=1)
-            if self.model == "GPC":
-                weighted_z *= self.gpc_weight_multiplier
-        elif self.model == "NR":
-            weights = torch.zeros(self.output_size, self.latent_variables, device=z.device)
-            weights[self.free_weights] = self.weight_param
-            weighted_z = torch.matmul(z, weights.T)
+        weights = torch.zeros(self.output_size, self.latent_variables, device=z.device)
+        weights[self.free_weights] = self.weight_param
+        weighted_z = torch.matmul(z, weights.T)
 
         output = weighted_z + bias
-        if self.model in ["GPC", "NR"]:
-            # stop gradients from flowing through the missing categories
-            output[:, self.missing_category] = -torch.inf
+        # stop gradients from flowing through the missing categories
+        output[:, self.missing_category] = -torch.inf
 
         output[:, self.first_category] = 0
 
         return output
 
-    def log_likelihood(
-        self,
-        data: torch.Tensor,
-        output: torch.Tensor,
-        loss_reduction: str = "sum",
-    ) -> torch.Tensor:
-        """
-        Compute the log likelihood of the data given the model. This is equivalent to the negative cross entropy loss.
-
-        Parameters
-        ----------
-        data: torch.Tensor
-            A 2D tensor with test data. Columns are items and rows are respondents
-        output: torch.Tensor
-            A 2D tensor with output. Columns are item response categories and rows are respondents
-        loss_reduction: str, optional 
-            The reduction argument for torch.nn.CrossEntropyLoss. (default is 'sum')
-        
-        Returns
-        -------
-        torch.Tensor
-            The log likelihood.
-        """
-        data = data.long()
-        data = data.view(-1)
-        reshaped_output = output.reshape(-1, self.max_item_responses)
-        if self.model == "3PL":
-            raise NotImplementedError("3PL not implemented yet")
-            # probabilities = torch.softmax(reshaped_output, dim=1)
-            # guessing = self.guessing_param.unsqueeze(1).repeat(int(data.shape[0]/self.items), reshaped_output.shape[1])
-            # guessing[:, 0] *= -1
-            # probabilities += guessing
-            # return -F.nll_loss(torch.log(probabilities), data, reduction=loss_reduction)
-        else:
-            return -F.cross_entropy(reshaped_output, data, reduction=loss_reduction)
-
-    def probabilities_from_output(self, output: torch.Tensor) -> list:
-        """
-        Compute item probabilities from the output tensor.
-
-        Parameters
-        ----------
-        output : torch.Tensor
-            Output tensor from the forward pass.
-
-        Returns
-        -------
-        probabilities : torch.Tensor
-            3D torch tensor with dimensions (respondents, items, item categories).
-        """
-        reshaped_output = output.reshape(-1, self.max_item_responses)
-        return F.softmax(reshaped_output, dim=1).reshape(output.shape[0], self.items, self.max_item_responses)
-
-    def item_parameters(self, IRT_format = False) -> pd.DataFrame:
+    def item_parameters(self, irt_format = False) -> pd.DataFrame:
         """
         Get the item parameters for a fitted model.
 
         Parameters
         ----------
-        IRT_format : bool, optional
+        irt_format : bool, optional
             Only for unidimensional models. Whether to return the item parameters in traditional IRT format. Otherwise returns weights and biases. (default is False)
 
         Returns
         -------
         pd.DataFrame
             A dataframe with the item parameters.
         """
         biases = torch.zeros(self.output_size)
         biases[self.free_bias] = self.bias_param
         biases = biases.reshape(-1, self.max_item_responses)
-        if self.model == "1PL":
-            weights = self.weight_param.repeat(self.items, 1)
-        elif self.model == "NR":
-            weights = torch.zeros(self.output_size, self.latent_variables)
-            weights[self.free_weights] = self.weight_param
-            weights = weights.reshape(-1, self.max_item_responses * self.latent_variables)
-        else:
-            weights = torch.zeros(self.items, self.latent_variables)
-            weights[self.free_weights] = self.weight_param
+
+        weights = torch.zeros(self.output_size, self.latent_variables)
+        weights[self.free_weights] = self.weight_param
+        weights = weights.reshape(-1, self.max_item_responses * self.latent_variables)
 
         weights_df = pd.DataFrame(weights.detach().numpy())
-        if IRT_format and self.latent_variables == 1:
-            if self.model == "NR":
-                weights_df.columns = [f"a{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
-                biases_df = pd.DataFrame(-(weights*biases).detach().numpy())
-            else:
-                weights_df.columns = [f"a{i+1}" for i in range(weights.shape[1])]
-                biases_df = pd.DataFrame(-(weights*biases).detach()[:, 1:].numpy())
+        if irt_format and self.latent_variables == 1:
+            biases_df = pd.DataFrame(-(weights*biases).detach().numpy())
+            weights_df.columns = [f"a{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
         else:
-            if self.model == "NR":
-                weights_df.columns = [f"w{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
-            else:
-                weights_df.columns = [f"w{i+1}" for i in range(weights.shape[1])]
             biases_df = pd.DataFrame(biases.detach().numpy())
+            weights_df.columns = [f"w{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
             
         biases_df.columns = [f"b{i+1}" for i in range(biases_df.shape[1])]
         parameters = pd.concat([weights_df, biases_df], axis=1)
 
         return parameters
 
     @torch.inference_mode()
@@ -260,18 +149,10 @@
             Only needed for NR models. A 2D tensor with latent z scores from the population of interest. Each row represents one respondent, and each column represents a latent variable.
 
         Returns
         -------
         torch.Tensor
             A 2D tensor with the relationships between the items and latent variables. Items are rows and latent variables are columns.
         """
-        if self.model == "1PL":
-            weights = self.weight_param.repeat(self.items, 1)
-        if self.model == "NR":
-            if z is None:
-                raise ValueError("z must be provided to get item to z relationships for NR models.")
-            return super().item_z_relationship_directions(z)
-        else:
-            weights = torch.zeros(self.items, self.latent_variables)
-            weights[self.free_weights] = self.weight_param
-        return weights.sign().int()
-    
+        if z is None:
+            raise ValueError("z must be provided to get item to z relationships for NR models.")
+        return super().item_z_relationship_directions(z)
```

### Comparing `irtorch-0.0.3/irtorch/outlier_detector.py` & `irtorch-0.0.4/irtorch/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/quantile_mv_normal.py` & `irtorch-0.0.4/irtorch/quantile_mv_normal.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/timer.py` & `irtorch-0.0.4/irtorch/timer.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch/utils.py` & `irtorch-0.0.4/irtorch/utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/irtorch.egg-info/PKG-INFO` & `irtorch-0.0.4/irtorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -36,17 +36,15 @@
 To cite IRTorch in publications use:
 
 Wallmark, J. (2024). IRTorch: Item response theory with Python (Version X.X) [Software]. GitHub. https://github.com/joakimwallmark/irtorch
 
 Or use the following BibTeX entry:
 
 ```bibtex
-@misc{irtorch2024,
+@manual{irtorch,
+  title = {{IRTorch}: Item response theory with Python},
   author = {Wallmark, Joakim},
-  title = {IRTorch: Item response theory with Python},
   year = {2024},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/joakimwallmark/irtorch}},
-  version = {X.X}
+  note = {Version X.X},
+  url = {https://github.com/joakimwallmark/irtorch}
 }
 ```
```

### Comparing `irtorch-0.0.3/irtorch.egg-info/SOURCES.txt` & `irtorch-0.0.4/irtorch.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 irtorch/estimation_algorithms/encoders/__init__.py
 irtorch/estimation_algorithms/encoders/base_encoder.py
 irtorch/estimation_algorithms/encoders/bounded_encoder.py
 irtorch/estimation_algorithms/encoders/standard_encoder.py
 irtorch/estimation_algorithms/encoders/variational_encoder.py
 irtorch/models/__init__.py
 irtorch/models/base_irt_model.py
+irtorch/models/generalized_partial_credit.py
 irtorch/models/monotone_nn.py
-irtorch/models/parametric.py
+irtorch/models/nominal_response.py
+irtorch/models/one_parameter_logistic.py
+irtorch/models/two_parameter_logistic.py
 tests/test_activation_functions.py
 tests/test_aeirt.py
-tests/test_base_irt_model.py
 tests/test_config.py
 tests/test_gaussian_mixture_torch.py
 tests/test_integration.py
 tests/test_internal_utils.py
 tests/test_irt_evaluator.py
 tests/test_irt_plotter.py
 tests/test_irt_scorer.py
 tests/test_latent_variable_functions.py
 tests/test_layers.py
 tests/test_load_dataset.py
-tests/test_monotone_nn.py
 tests/test_outlier_detector.py
-tests/test_parametric.py
 tests/test_quantile_mv_normal.py
 tests/test_utils.py
 tests/test_vaeirt.py
```

### Comparing `irtorch-0.0.3/setup.py` & `irtorch-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="irtorch",
-    version="0.0.3",
+    version="0.0.4",
     description="IRTorch: An item response theory package for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     url="https://github.com/joakimwallmark/irtorch",
     author="Joakim Wallmark",
     author_email="wallmark.joakim@gmail.com",
```

### Comparing `irtorch-0.0.3/tests/test_activation_functions.py` & `irtorch-0.0.4/tests/test_activation_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_aeirt.py` & `irtorch-0.0.4/tests/test_aeirt.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_config.py` & `irtorch-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_gaussian_mixture_torch.py` & `irtorch-0.0.4/tests/test_gaussian_mixture_torch.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_integration.py` & `irtorch-0.0.4/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #     initial_parameter_dict = {k: v.clone() for k, v in model.model.state_dict().items()}
 #     model.fit(
 #         train_data=data,
 #         device=device
 #     )
     
 #     # Save models for other tests
-#     # model.save_model(f"tests/models/{model_type}_latent_variables{latent_variables}_{data_type}_{device}.pt")
+#     # model.save_model(f"tests/fitted_models/{model_type}_latent_variables{latent_variables}_{data_type}_{device}.pt")
 
 #     for name, param in model.model.state_dict().items():
 #         if 'free' not in name and 'missing_categories' not in name and not re.match(r'negation_dim\d+\.weight', name):
 #             assert not torch.equal(initial_parameter_dict[name], param), f"Parameter {name} was not updated."
 
 # @pytest.mark.integration
 # def test_latent_scores(model: IRT, data, latent_variables):
```

### Comparing `irtorch-0.0.3/tests/test_internal_utils.py` & `irtorch-0.0.4/tests/test_internal_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_irt_evaluator.py` & `irtorch-0.0.4/tests/test_irt_evaluator.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_irt_plotter.py` & `irtorch-0.0.4/tests/test_irt_plotter.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_irt_scorer.py` & `irtorch-0.0.4/tests/test_irt_scorer.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_latent_variable_functions.py` & `irtorch-0.0.4/tests/test_latent_variable_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_layers.py` & `irtorch-0.0.4/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_load_dataset.py` & `irtorch-0.0.4/tests/test_load_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,36 @@
     data = swedish_national_mathematics_1()
     assert data.dtype == torch.float32
     assert data.shape == (1008, 28)
 
 def test_swedish_sat_verbal():
     data, correct_category = swedish_sat_verbal()
     assert data.dtype == torch.float32
-    assert data.shape == (38068, 80)
+    assert data.shape == (5000, 80)
     assert len(correct_category) == 80
     assert all([isinstance(x, int) for x in correct_category])
 
 def test_swedish_sat_quantitative():
     data, correct_category = swedish_sat_quantitative()
     assert data.dtype == torch.float32
-    assert data.shape == (38068, 80)
+    assert data.shape == (5000, 80)
     assert len(correct_category) == 80
     assert all([isinstance(x, int) for x in correct_category])
 
 def test_swedish_sat():
     data, correct_category = swedish_sat()
     assert data.dtype == torch.float32
-    assert data.shape == (38068, 160)
+    assert data.shape == (5000, 160)
     assert len(correct_category) == 160
     assert all([isinstance(x, int) for x in correct_category])
 
 def test_swedish_sat_binary():
     data = swedish_sat_binary()
     assert data.dtype == torch.float32
-    assert data.shape == (38068, 160)
+    assert data.shape == (5000, 160)
     assert data[~data.isnan()].max() == 1.0
     assert data[~data.isnan()].min() == 0.0
 
 def test_big_five():
     data = big_five()
     assert data.dtype == torch.float32
     assert data.shape == (19719, 50)
```

### Comparing `irtorch-0.0.3/tests/test_outlier_detector.py` & `irtorch-0.0.4/tests/test_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_quantile_mv_normal.py` & `irtorch-0.0.4/tests/test_quantile_mv_normal.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_utils.py` & `irtorch-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.3/tests/test_vaeirt.py` & `irtorch-0.0.4/tests/test_vaeirt.py`

 * *Files identical despite different names*

