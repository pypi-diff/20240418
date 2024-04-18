# Comparing `tmp/alibi-0.9.6.tar.gz` & `tmp/alibi-0.9.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alibi-0.9.6.tar", last modified: Thu Apr 18 15:28:46 2024, max compression
+gzip compressed data, was "alibi-0.9.7.dev0.tar", last modified: Thu Apr 18 15:28:31 2024, max compression
```

## Comparing `alibi-0.9.6.tar` & `alibi-0.9.7.dev0.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.739416 alibi-0.9.6/
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4435 2024-03-08 11:18:09.000000 alibi-0.9.6/LICENSE
--rw-r--r--   0 jesse     (1000) jesse     (1000)       58 2024-03-08 11:18:09.000000 alibi-0.9.6/MANIFEST.in
--rw-r--r--   0 jesse     (1000) jesse     (1000)    22016 2024-04-18 15:28:46.739416 alibi-0.9.6/PKG-INFO
--rw-r--r--   0 jesse     (1000) jesse     (1000)    19962 2024-03-08 11:18:09.000000 alibi-0.9.6/README.md
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.728416 alibi-0.9.6/alibi/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      187 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/__init__.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.729416 alibi-0.9.6/alibi/api/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/api/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     7096 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/api/defaults.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     6960 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/api/interfaces.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.729416 alibi-0.9.6/alibi/api/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/api/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2793 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/api/tests/test_interfaces.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.729416 alibi-0.9.6/alibi/confidence/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      251 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    18571 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/model_linearity.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.729416 alibi-0.9.6/alibi/confidence/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     8326 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/tests/test_model_linearity.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2174 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/tests/test_trustscore.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     8182 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/confidence/trustscore.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.729416 alibi-0.9.6/alibi/data/
--rw-r--r--   0 jesse     (1000) jesse     (1000)   116015 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/data/cats.tar.gz
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.730416 alibi-0.9.6/alibi/datasets/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      451 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/datasets/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    12940 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/datasets/default.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1037 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/datasets/tensorflow.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.730416 alibi-0.9.6/alibi/datasets/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/datasets/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4559 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/datasets/tests/test_datasets.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1813 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/exceptions.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.731416 alibi-0.9.6/alibi/explainers/
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2230 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    29966 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/ale.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.731416 alibi-0.9.6/alibi/explainers/anchors/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    35805 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4371 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_explanation.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    28076 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_image.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    49238 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_tabular.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    12848 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_tabular_distributed.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    24277 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/anchor_text.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    27204 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/language_model_text_sampler.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    16942 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/anchors/text_samplers.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.731416 alibi-0.9.6/alibi/explainers/backends/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4211 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/cfrl_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    39331 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/cfrl_tabular.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/backends/pytorch/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/pytorch/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    17733 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/pytorch/cfrl_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     6141 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/pytorch/cfrl_tabular.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/backends/tensorflow/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/tensorflow/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    19783 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/tensorflow/cfrl_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     6379 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/backends/tensorflow/cfrl_tabular.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    35184 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/cem.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    66395 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/cfproto.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    44884 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/cfrl_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    23850 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/cfrl_tabular.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    27167 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/counterfactual.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    56311 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/integrated_gradients.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    73449 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/partial_dependence.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    39615 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/pd_variance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    45107 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/permutation_importance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    80158 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/shap_wrappers.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/similarity/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/__init__.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/similarity/backends/
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1321 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/backends/__init__.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/similarity/backends/pytorch/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/backends/pytorch/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4753 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/backends/pytorch/base.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.732416 alibi-0.9.6/alibi/explainers/similarity/backends/tensorflow/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/backends/tensorflow/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4341 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/backends/tensorflow/base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     8837 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    13302 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/grad.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2654 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/similarity/metrics.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.734416 alibi-0.9.6/alibi/explainers/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    11006 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/conftest.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    17481 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_ale.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2582 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_anchor_base.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     7874 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_anchor_image.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    16247 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_anchor_tabular.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    18774 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_anchor_text.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1572 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_cem.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     6681 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_cfproto.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    20718 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_cfrl.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4900 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_counterfactual.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    37074 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_integrated_gradients.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    43230 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_partial_dependence.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    28620 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_pd_variance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    23539 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_permutation_importance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    65489 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_shap_wrappers.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.734416 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     5831 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/conftest.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     5864 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_backends.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    17977 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     9302 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3086 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/explainers/tests/utils.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.734416 alibi-0.9.6/alibi/models/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/__init__.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.735416 alibi-0.9.6/alibi/models/pytorch/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      477 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2748 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/actor_critic.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3094 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/autoencoder.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     8134 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/cfrl_models.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4952 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/metrics.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    12988 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/model.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.735416 alibi-0.9.6/alibi/models/pytorch/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1767 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/test_actor_critic.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      647 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/test_autoencoder.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3778 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/test_cfrl_models.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1847 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/test_metrics.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    21220 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/pytorch/tests/test_model.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.735416 alibi-0.9.6/alibi/models/tensorflow/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      486 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2913 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/actor_critic.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3378 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/autoencoder.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     8692 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/cfrl_models.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.735416 alibi-0.9.6/alibi/models/tensorflow/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1655 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/tests/test_actor_critic.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      643 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/tests/test_autoencoder.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3708 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/models/tensorflow/tests/test_cfrl_models.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.736416 alibi-0.9.6/alibi/prototypes/
--rw-r--r--   0 jesse     (1000) jesse     (1000)      250 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/prototypes/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    32737 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/prototypes/protoselect.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.736416 alibi-0.9.6/alibi/prototypes/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/prototypes/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    11674 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/prototypes/tests/test_protoselect.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3195 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/prototypes/tests/test_utils.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    16214 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/saving.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.736416 alibi-0.9.6/alibi/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      622 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/conftest.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     7230 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/test_dep_management.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    18797 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/test_saving.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1033 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/test_utils.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4809 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/tests/utils.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.737416 alibi-0.9.6/alibi/utils/
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1276 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4968 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/approximation_methods.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2652 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/data.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3592 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/discretizer.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    12090 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/distance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    31311 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/distributed.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      582 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/distributions.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      513 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/download.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      320 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/frameworks.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2915 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/gradients.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4666 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/kernel.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    15019 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/lang_model.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     4722 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/mapping.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     5365 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/missing_optional_dependency.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.738416 alibi-0.9.6/alibi/utils/tests/
--rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/__init__.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      194 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/mocked_opt_dep.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1014 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_data.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     3193 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_distance.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    15565 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_distributed.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1631 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_gradients.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2855 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_import_optional.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1103 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_mapping.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      398 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tests/test_misc.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      919 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/tf.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)    23141 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/visualization.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)     1707 2024-03-08 11:18:09.000000 alibi-0.9.6/alibi/utils/wrappers.py
--rw-r--r--   0 jesse     (1000) jesse     (1000)      213 2024-04-18 15:28:43.000000 alibi-0.9.6/alibi/version.py
-drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:46.738416 alibi-0.9.6/alibi.egg-info/
--rw-r--r--   0 jesse     (1000) jesse     (1000)    22016 2024-04-18 15:28:46.000000 alibi-0.9.6/alibi.egg-info/PKG-INFO
--rw-r--r--   0 jesse     (1000) jesse     (1000)     5394 2024-04-18 15:28:46.000000 alibi-0.9.6/alibi.egg-info/SOURCES.txt
--rw-r--r--   0 jesse     (1000) jesse     (1000)        1 2024-04-18 15:28:46.000000 alibi-0.9.6/alibi.egg-info/dependency_links.txt
--rw-r--r--   0 jesse     (1000) jesse     (1000)        1 2024-03-08 11:22:34.000000 alibi-0.9.6/alibi.egg-info/not-zip-safe
--rw-r--r--   0 jesse     (1000) jesse     (1000)      649 2024-04-18 15:28:46.000000 alibi-0.9.6/alibi.egg-info/requires.txt
--rw-r--r--   0 jesse     (1000) jesse     (1000)        6 2024-04-18 15:28:46.000000 alibi-0.9.6/alibi.egg-info/top_level.txt
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2121 2024-04-18 15:28:46.740416 alibi-0.9.6/setup.cfg
--rw-r--r--   0 jesse     (1000) jesse     (1000)     2942 2024-04-18 14:02:57.000000 alibi-0.9.6/setup.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.774660 alibi-0.9.7.dev0/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4435 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/LICENSE
+-rw-r--r--   0 jesse     (1000) jesse     (1000)       58 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/MANIFEST.in
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    22021 2024-04-18 15:28:31.774660 alibi-0.9.7.dev0/PKG-INFO
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    19962 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/README.md
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.764659 alibi-0.9.7.dev0/alibi/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      187 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/__init__.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/api/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/api/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     7096 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/api/defaults.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     6960 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/api/interfaces.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/api/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/api/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2793 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/api/tests/test_interfaces.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/confidence/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      251 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    18571 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/model_linearity.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/confidence/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     8326 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/tests/test_model_linearity.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2174 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/tests/test_trustscore.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     8182 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/confidence/trustscore.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/data/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)   116015 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/data/cats.tar.gz
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.765659 alibi-0.9.7.dev0/alibi/datasets/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      451 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/datasets/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    12940 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/datasets/default.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1037 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/datasets/tensorflow.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.766659 alibi-0.9.7.dev0/alibi/datasets/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/datasets/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4559 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/datasets/tests/test_datasets.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1813 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/exceptions.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.766659 alibi-0.9.7.dev0/alibi/explainers/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2230 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    29966 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/ale.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.767659 alibi-0.9.7.dev0/alibi/explainers/anchors/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    35805 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4371 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_explanation.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    28076 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_image.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    49238 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_tabular.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    12848 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_tabular_distributed.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    24277 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_text.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    27204 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/language_model_text_sampler.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    16942 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/anchors/text_samplers.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.767659 alibi-0.9.7.dev0/alibi/explainers/backends/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4211 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/cfrl_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    39331 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/cfrl_tabular.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.767659 alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    17733 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/cfrl_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     6141 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/cfrl_tabular.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.768659 alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    19783 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/cfrl_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     6379 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/cfrl_tabular.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    35184 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/cem.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    66395 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/cfproto.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    44884 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/cfrl_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    23850 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/cfrl_tabular.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    27167 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/counterfactual.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    56311 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/integrated_gradients.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    73449 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/partial_dependence.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    39615 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/pd_variance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    45107 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/permutation_importance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    80158 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/shap_wrappers.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.768659 alibi-0.9.7.dev0/alibi/explainers/similarity/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/__init__.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.768659 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1321 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/__init__.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.768659 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/pytorch/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/pytorch/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4753 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/pytorch/base.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.768659 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/tensorflow/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/tensorflow/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4341 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/backends/tensorflow/base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     8837 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    13302 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/grad.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2654 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/similarity/metrics.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.769659 alibi-0.9.7.dev0/alibi/explainers/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    11006 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/conftest.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    17481 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_ale.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2582 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_base.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     7874 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_image.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    16247 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_tabular.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    18774 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_text.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1572 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_cem.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     6681 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_cfproto.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    20718 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_cfrl.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4900 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_counterfactual.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    37074 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_integrated_gradients.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    43230 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_partial_dependence.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    28620 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_pd_variance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    23539 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_permutation_importance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    65489 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_shap_wrappers.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.769659 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     5831 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/conftest.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     5864 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_backends.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    17977 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     9302 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3086 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/explainers/tests/utils.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.770660 alibi-0.9.7.dev0/alibi/models/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/__init__.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.770660 alibi-0.9.7.dev0/alibi/models/pytorch/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      477 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2748 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/actor_critic.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3094 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/autoencoder.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     8134 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/cfrl_models.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4952 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/metrics.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    12988 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/model.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.770660 alibi-0.9.7.dev0/alibi/models/pytorch/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1767 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_actor_critic.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      647 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_autoencoder.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3778 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_cfrl_models.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1847 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_metrics.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    21220 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_model.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.770660 alibi-0.9.7.dev0/alibi/models/tensorflow/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      486 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2913 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/actor_critic.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3378 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/autoencoder.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     8692 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/cfrl_models.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.771659 alibi-0.9.7.dev0/alibi/models/tensorflow/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1655 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_actor_critic.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      643 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_autoencoder.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3708 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_cfrl_models.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.771659 alibi-0.9.7.dev0/alibi/prototypes/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      250 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/prototypes/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    32737 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/prototypes/protoselect.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.771659 alibi-0.9.7.dev0/alibi/prototypes/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/prototypes/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    11674 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/prototypes/tests/test_protoselect.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3195 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/prototypes/tests/test_utils.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    16214 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/saving.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.771659 alibi-0.9.7.dev0/alibi/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      622 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/conftest.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     7230 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/test_dep_management.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    18797 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/test_saving.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1033 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/test_utils.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4809 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/tests/utils.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.772660 alibi-0.9.7.dev0/alibi/utils/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1276 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4968 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/approximation_methods.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2652 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/data.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3592 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/discretizer.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    12090 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/distance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    31311 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/distributed.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      582 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/distributions.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      513 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/download.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      320 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/frameworks.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2915 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/gradients.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4666 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/kernel.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    15019 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/lang_model.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     4722 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/mapping.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     5365 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/missing_optional_dependency.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.773660 alibi-0.9.7.dev0/alibi/utils/tests/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        0 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/__init__.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      194 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/mocked_opt_dep.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1014 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_data.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     3193 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_distance.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    15565 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_distributed.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1631 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_gradients.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2855 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_import_optional.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1103 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_mapping.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      398 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tests/test_misc.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      919 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/tf.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    23141 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/visualization.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     1707 2024-03-08 11:18:09.000000 alibi-0.9.7.dev0/alibi/utils/wrappers.py
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      218 2024-04-18 15:24:07.000000 alibi-0.9.7.dev0/alibi/version.py
+drwxr-xr-x   0 jesse     (1000) jesse     (1000)        0 2024-04-18 15:28:31.773660 alibi-0.9.7.dev0/alibi.egg-info/
+-rw-r--r--   0 jesse     (1000) jesse     (1000)    22021 2024-04-18 15:28:31.000000 alibi-0.9.7.dev0/alibi.egg-info/PKG-INFO
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     5394 2024-04-18 15:28:31.000000 alibi-0.9.7.dev0/alibi.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        1 2024-04-18 15:28:31.000000 alibi-0.9.7.dev0/alibi.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        1 2024-03-08 11:22:34.000000 alibi-0.9.7.dev0/alibi.egg-info/not-zip-safe
+-rw-r--r--   0 jesse     (1000) jesse     (1000)      649 2024-04-18 15:28:31.000000 alibi-0.9.7.dev0/alibi.egg-info/requires.txt
+-rw-r--r--   0 jesse     (1000) jesse     (1000)        6 2024-04-18 15:28:31.000000 alibi-0.9.7.dev0/alibi.egg-info/top_level.txt
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2121 2024-04-18 15:28:31.775660 alibi-0.9.7.dev0/setup.cfg
+-rw-r--r--   0 jesse     (1000) jesse     (1000)     2942 2024-04-18 14:02:57.000000 alibi-0.9.7.dev0/setup.py
```

### Comparing `alibi-0.9.6/LICENSE` & `alibi-0.9.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/PKG-INFO` & `alibi-0.9.7.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.6
+Version: 0.9.7.dev0
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Business Source License 1.1
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `alibi-0.9.6/README.md` & `alibi-0.9.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/api/defaults.py` & `alibi-0.9.7.dev0/alibi/api/defaults.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/api/interfaces.py` & `alibi-0.9.7.dev0/alibi/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/api/tests/test_interfaces.py` & `alibi-0.9.7.dev0/alibi/api/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/confidence/model_linearity.py` & `alibi-0.9.7.dev0/alibi/confidence/model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/confidence/tests/test_model_linearity.py` & `alibi-0.9.7.dev0/alibi/confidence/tests/test_model_linearity.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/confidence/tests/test_trustscore.py` & `alibi-0.9.7.dev0/alibi/confidence/tests/test_trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/confidence/trustscore.py` & `alibi-0.9.7.dev0/alibi/confidence/trustscore.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/data/cats.tar.gz` & `alibi-0.9.7.dev0/alibi/data/cats.tar.gz`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/datasets/default.py` & `alibi-0.9.7.dev0/alibi/datasets/default.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/datasets/tensorflow.py` & `alibi-0.9.7.dev0/alibi/datasets/tensorflow.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/datasets/tests/test_datasets.py` & `alibi-0.9.7.dev0/alibi/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/exceptions.py` & `alibi-0.9.7.dev0/alibi/exceptions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/__init__.py` & `alibi-0.9.7.dev0/alibi/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/ale.py` & `alibi-0.9.7.dev0/alibi/explainers/ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_base.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_explanation.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_explanation.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_image.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_tabular_distributed.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_tabular_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/anchor_text.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/language_model_text_sampler.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/language_model_text_sampler.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/anchors/text_samplers.py` & `alibi-0.9.7.dev0/alibi/explainers/anchors/text_samplers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/cfrl_base.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/cfrl_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/pytorch/cfrl_base.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/pytorch/cfrl_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/pytorch/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/tensorflow/cfrl_base.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/backends/tensorflow/cfrl_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/backends/tensorflow/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/cem.py` & `alibi-0.9.7.dev0/alibi/explainers/cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/cfproto.py` & `alibi-0.9.7.dev0/alibi/explainers/cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/cfrl_base.py` & `alibi-0.9.7.dev0/alibi/explainers/cfrl_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/cfrl_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/cfrl_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/counterfactual.py` & `alibi-0.9.7.dev0/alibi/explainers/counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/integrated_gradients.py` & `alibi-0.9.7.dev0/alibi/explainers/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/partial_dependence.py` & `alibi-0.9.7.dev0/alibi/explainers/partial_dependence.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/pd_variance.py` & `alibi-0.9.7.dev0/alibi/explainers/pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/permutation_importance.py` & `alibi-0.9.7.dev0/alibi/explainers/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/shap_wrappers.py` & `alibi-0.9.7.dev0/alibi/explainers/shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/backends/__init__.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/backends/pytorch/base.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/backends/pytorch/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/backends/tensorflow/base.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/backends/tensorflow/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/base.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/grad.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/grad.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/similarity/metrics.py` & `alibi-0.9.7.dev0/alibi/explainers/similarity/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/conftest.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_ale.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_ale.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_anchor_base.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_base.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_anchor_image.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_image.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_anchor_tabular.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_tabular.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_anchor_text.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_anchor_text.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_cem.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_cfproto.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_cfproto.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_cfrl.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_cfrl.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_counterfactual.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_counterfactual.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_integrated_gradients.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_partial_dependence.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_pd_variance.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_pd_variance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_permutation_importance.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_shap_wrappers.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_shap_wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_simiarlity/conftest.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_backends.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_backends.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_grad_methods_integration.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/test_simiarlity/test_grad_methods_unit.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/explainers/tests/utils.py` & `alibi-0.9.7.dev0/alibi/explainers/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/actor_critic.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/autoencoder.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/cfrl_models.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/metrics.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/model.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/tests/test_actor_critic.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/tests/test_autoencoder.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/tests/test_cfrl_models.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/tests/test_metrics.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/pytorch/tests/test_model.py` & `alibi-0.9.7.dev0/alibi/models/pytorch/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/actor_critic.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/autoencoder.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/cfrl_models.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/tests/test_actor_critic.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_actor_critic.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/tests/test_autoencoder.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/models/tensorflow/tests/test_cfrl_models.py` & `alibi-0.9.7.dev0/alibi/models/tensorflow/tests/test_cfrl_models.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/prototypes/protoselect.py` & `alibi-0.9.7.dev0/alibi/prototypes/protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/prototypes/tests/test_protoselect.py` & `alibi-0.9.7.dev0/alibi/prototypes/tests/test_protoselect.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/prototypes/tests/test_utils.py` & `alibi-0.9.7.dev0/alibi/prototypes/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/saving.py` & `alibi-0.9.7.dev0/alibi/saving.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/tests/conftest.py` & `alibi-0.9.7.dev0/alibi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/tests/test_dep_management.py` & `alibi-0.9.7.dev0/alibi/tests/test_dep_management.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/tests/test_saving.py` & `alibi-0.9.7.dev0/alibi/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/tests/test_utils.py` & `alibi-0.9.7.dev0/alibi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/tests/utils.py` & `alibi-0.9.7.dev0/alibi/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/__init__.py` & `alibi-0.9.7.dev0/alibi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/approximation_methods.py` & `alibi-0.9.7.dev0/alibi/utils/approximation_methods.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/data.py` & `alibi-0.9.7.dev0/alibi/utils/data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/discretizer.py` & `alibi-0.9.7.dev0/alibi/utils/discretizer.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/distance.py` & `alibi-0.9.7.dev0/alibi/utils/distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/distributed.py` & `alibi-0.9.7.dev0/alibi/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/distributions.py` & `alibi-0.9.7.dev0/alibi/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/download.py` & `alibi-0.9.7.dev0/alibi/utils/download.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/gradients.py` & `alibi-0.9.7.dev0/alibi/utils/gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/kernel.py` & `alibi-0.9.7.dev0/alibi/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/lang_model.py` & `alibi-0.9.7.dev0/alibi/utils/lang_model.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/mapping.py` & `alibi-0.9.7.dev0/alibi/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/missing_optional_dependency.py` & `alibi-0.9.7.dev0/alibi/utils/missing_optional_dependency.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_data.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_distance.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_distributed.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_gradients.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_import_optional.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_import_optional.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tests/test_mapping.py` & `alibi-0.9.7.dev0/alibi/utils/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/tf.py` & `alibi-0.9.7.dev0/alibi/utils/tf.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/visualization.py` & `alibi-0.9.7.dev0/alibi/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi/utils/wrappers.py` & `alibi-0.9.7.dev0/alibi/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi.egg-info/PKG-INFO` & `alibi-0.9.7.dev0/alibi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibi
-Version: 0.9.6
+Version: 0.9.7.dev0
 Summary: Algorithms for monitoring and explaining machine learning models
 Home-page: https://github.com/SeldonIO/alibi
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Business Source License 1.1
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `alibi-0.9.6/alibi.egg-info/SOURCES.txt` & `alibi-0.9.7.dev0/alibi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/alibi.egg-info/requires.txt` & `alibi-0.9.7.dev0/alibi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/setup.cfg` & `alibi-0.9.7.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `alibi-0.9.6/setup.py` & `alibi-0.9.7.dev0/setup.py`

 * *Files identical despite different names*

