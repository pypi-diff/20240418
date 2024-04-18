# Comparing `tmp/fuxictr-2.2.1.tar.gz` & `tmp/fuxictr-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.2.1.tar", last modified: Tue Apr 16 03:53:28 2024, max compression
+gzip compressed data, was "dist/fuxictr-2.2.2.tar", last modified: Thu Apr 18 06:22:02 2024, max compression
```

## Comparing `fuxictr-2.2.1.tar` & `fuxictr-2.2.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-16 03:53:28.000000 fuxictr-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-16 03:53:25.000000 fuxictr-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/autotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/avazu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/kkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/feature_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/rank_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/multitask_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/model_zoo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/model_zoo/multitask/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 03:53:25.000000 fuxictr-2.2.1/model_zoo/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:53:28.000000 fuxictr-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 03:53:25.000000 fuxictr-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-18 06:22:02.000000 fuxictr-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-18 06:21:58.000000 fuxictr-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/autotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/avazu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/kkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18058 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/feature_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/rank_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/multitask_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/model_zoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/model_zoo/multitask/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 06:21:58.000000 fuxictr-2.2.2/model_zoo/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:22:02.000000 fuxictr-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 06:21:58.000000 fuxictr-2.2.2/setup.py
```

### Comparing `fuxictr-2.2.1/PKG-INFO` & `fuxictr-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.1
+Version: 2.2.2
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.1 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.2 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.1/README.md` & `fuxictr-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/autotuner.py` & `fuxictr-2.2.2/fuxictr/autotuner.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/datasets/avazu.py` & `fuxictr-2.2.2/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/datasets/criteo.py` & `fuxictr-2.2.2/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/datasets/kkbox.py` & `fuxictr-2.2.2/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/features.py` & `fuxictr-2.2.2/fuxictr/features.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/metrics.py` & `fuxictr-2.2.2/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.2.2/fuxictr/preprocess/build_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 import os
 import logging
 import numpy as np
 import gc
 import multiprocessing as mp
+import polars as pl
 
 
 def split_train_test(train_ddf=None, valid_ddf=None, test_ddf=None, valid_size=0, 
                      test_size=0, split_type="sequential"):
     num_samples = len(train_ddf)
     train_size = num_samples
     instance_IDs = np.arange(num_samples)
@@ -49,36 +50,36 @@
 
 def save_npz(darray_dict, data_path):
     logging.info("Saving data to npz: " + data_path)
     os.makedirs(os.path.dirname(data_path), exist_ok=True)
     np.savez(data_path, **darray_dict)
 
 
-def transform_block(feature_encoder, df_block, filename, preprocess=False):
-    if preprocess:
-        df_block = feature_encoder.preprocess(df_block)
+def transform_block(feature_encoder, df_block, filename):
     darray_dict = feature_encoder.transform(df_block)
     save_npz(darray_dict, os.path.join(feature_encoder.data_dir, filename))
 
 
-def transform(feature_encoder, ddf, filename, preprocess=False, block_size=0):
+def transform(feature_encoder, ddf, filename, block_size=0):
     if block_size > 0:
         pool = mp.Pool(mp.cpu_count() // 2)
         block_id = 0
         for idx in range(0, len(ddf), block_size):
-            df_block = ddf[idx: (idx + block_size)]
-            pool.apply_async(transform_block, args=(feature_encoder,
-                                                    df_block,
-                                                    '{}/part_{:05d}.npz'.format(filename, block_id),
-                                                    preprocess))
+            df_block = ddf.iloc[idx:(idx + block_size)]
+            pool.apply_async(
+                transform_block, 
+                args=(feature_encoder,
+                      df_block,
+                      '{}/part_{:05d}.npz'.format(filename, block_id))
+            )
             block_id += 1
         pool.close()
         pool.join()
     else:
-        transform_block(feature_encoder, ddf, filename, preprocess)
+        transform_block(feature_encoder, ddf, filename)
 
 
 def build_dataset(feature_encoder, train_data=None, valid_data=None, test_data=None, valid_size=0, 
                   test_size=0, split_type="sequential", data_block_size=0, **kwargs):
     """ Build feature_map and transform data """
 
     feature_map_json = os.path.join(feature_encoder.data_dir, "feature_map.json")
@@ -92,36 +93,38 @@
         test_ddf = None
 
         # Split data for train/validation/test
         if valid_size > 0 or test_size > 0:
             valid_ddf = feature_encoder.read_csv(valid_data, **kwargs)
             test_ddf = feature_encoder.read_csv(test_data, **kwargs)
             train_ddf, valid_ddf, test_ddf = split_train_test(train_ddf, valid_ddf, test_ddf, 
-                                                            valid_size, test_size, split_type)
+                                                              valid_size, test_size, split_type)
         
         # fit and transform train_ddf
         train_ddf = feature_encoder.preprocess(train_ddf)
         feature_encoder.fit(train_ddf, **kwargs)
-        transform(feature_encoder, train_ddf, 'train', preprocess=False, block_size=data_block_size)
+        transform(feature_encoder, train_ddf, 'train', block_size=data_block_size)
         del train_ddf
         gc.collect()
 
         # Transfrom valid_ddf
         if valid_ddf is None and (valid_data is not None):
             valid_ddf = feature_encoder.read_csv(valid_data, **kwargs)
         if valid_ddf is not None:
-            transform(feature_encoder, valid_ddf, 'valid', preprocess=True, block_size=data_block_size)
+            valid_ddf = feature_encoder.preprocess(valid_ddf)
+            transform(feature_encoder, valid_ddf, 'valid', block_size=data_block_size)
             del valid_ddf
             gc.collect()
 
         # Transfrom test_ddf
         if test_ddf is None and (test_data is not None):
             test_ddf = feature_encoder.read_csv(test_data, **kwargs)
         if test_ddf is not None:
-            transform(feature_encoder, test_ddf, 'test', preprocess=True, block_size=data_block_size)
+            test_ddf = feature_encoder.preprocess(test_ddf)
+            transform(feature_encoder, test_ddf, 'test', block_size=data_block_size)
             del test_ddf
             gc.collect()
         logging.info("Transform csv data to npz done.")
     
     # Return processed data splits
     return os.path.join(feature_encoder.data_dir, "train"), \
            os.path.join(feature_encoder.data_dir, "valid"), \
```

### Comparing `fuxictr-2.2.1/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.2.2/fuxictr/preprocess/feature_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 # limitations under the License.
 # =========================================================================
 
 
 import numpy as np
 from collections import Counter, OrderedDict
 import pandas as pd
+import polars as pl
 import pickle
 import os
 import logging
 import json
 import re
 import shutil
+import glob
 from pathlib import Path
 import sklearn.preprocessing as sklearn_preprocess
 from fuxictr.features import FeatureMap
 from .tokenizer import Tokenizer
 from .normalizer import Normalizer
 
 
@@ -61,71 +63,62 @@
                     _col = col.copy()
                     _col["name"] = _name
                     full_feature_cols.append(_col)
             else:
                 full_feature_cols.append(col)
         return full_feature_cols
 
-    def read_csv(self, data_path, sep=",", nrows=None, **kwargs):
+    def read_csv(self, data_path, sep=",", n_rows=None, **kwargs):
         logging.info("Reading file: " + data_path)
-        usecols_fn = lambda x: x in self.dtype_dict
-        ddf = pd.read_csv(data_path, sep=sep, usecols=usecols_fn, 
-                          dtype=object, memory_map=True, nrows=nrows)
+        file_names = sorted(glob.glob(data_path))
+        assert len(file_names) > 0, f"Invalid data path: {data_path}"
+        # Require python >= 3.8 for use polars to scan multiple csv files
+        file_names = file_names[0]
+        ddf = pl.scan_csv(source=file_names, separator=sep, dtypes=self.dtype_dict,
+                          low_memory=False, n_rows=n_rows)
         return ddf
 
     def preprocess(self, ddf):
         logging.info("Preprocess feature columns...")
         all_cols = self.label_cols + self.feature_cols[::-1]
         for col in all_cols:
             name = col["name"]
             if name in ddf.columns:
-                if ddf[name].isnull().values.any():
-                    ddf[name] = self._fill_na_(col, ddf[name])
-                ddf[name] = ddf[name].astype(self.dtype_dict[name])
+                fill_na = "" if col["dtype"] in ["str", str] else 0
+                fill_na = col.get("fill_na", fill_na)
+                ddf = ddf.with_columns(pl.col(name).fill_null(fill_na))
             if col.get("preprocess"):
-                preprocess_splits = re.split(r"\(|\)", col["preprocess"])
-                preprocess_fn = getattr(self, preprocess_splits[0])
-                if len(preprocess_splits) > 1:
-                    ddf[name] = preprocess_fn(ddf, preprocess_splits[1])
-                else:
-                    ddf[name] = preprocess_fn(ddf, name)
-                ddf[name] = ddf[name].astype(self.dtype_dict[name])
+                preprocess_args = re.split(r"\(|\)", col["preprocess"])
+                preprocess_fn = getattr(self, preprocess_args[0])
+                ddf = preprocess_fn(ddf, name, *preprocess_args[1:-1])
+                ddf = ddf.with_columns(pl.col(name).cast(self.dtype_dict[name]))
         active_cols = [col["name"] for col in all_cols if col.get("active") != False]
-        ddf = ddf.loc[:, active_cols]
+        ddf = ddf.select(active_cols)
         return ddf
 
-    def _fill_na_(self, col, series):
-        na_value = col.get("fill_na")
-        if na_value is not None:
-            return series.fillna(na_value)
-        elif col["dtype"] in ["str", str]:
-            return series.fillna("")
-        else:
-            raise RuntimeError("Feature column={} requires to assign fill_na value!".format(col["name"]))
-
     def fit(self, train_ddf, min_categr_count=1, num_buckets=10, **kwargs):    
         logging.info("Fit feature processor...")
         for col in self.feature_cols:
             name = col["name"]
             if col["active"]:
                 logging.info("Processing column: {}".format(col))
+                col_series = train_ddf.select(name).collect().to_series().to_pandas()
                 if col["type"] == "meta": # e.g. group_id
-                    self.fit_meta_col(col, train_ddf[name].values)
+                    self.fit_meta_col(col)
                 elif col["type"] == "numeric":
-                    self.fit_numeric_col(col, train_ddf[name].values)
+                    self.fit_numeric_col(col, col_series)
                 elif col["type"] == "categorical":
-
-                    self.fit_categorical_col(col, train_ddf[name].values, 
+                    self.fit_categorical_col(col, col_series,
                                              min_categr_count=min_categr_count,
                                              num_buckets=num_buckets)
                 elif col["type"] == "sequence":
-                    self.fit_sequence_col(col, train_ddf[name].values, 
+                    self.fit_sequence_col(col, col_series, 
                                           min_categr_count=min_categr_count)
                 else:
-                    raise NotImplementedError("feature_col={}".format(feature_col))
+                    raise NotImplementedError("feature type={}".format(col["type"]))
         
         # Expand vocab from pretrained_emb
         os.makedirs(self.data_dir, exist_ok=True)
         for col in self.feature_cols:
             name = col["name"]
             if "pretrained_emb" in col:
                 logging.info("Loading pretrained embedding: " + name)
@@ -162,38 +155,37 @@
         self.feature_map.num_fields = self.feature_map.get_num_fields()
         self.feature_map.set_column_index()
         self.save_pickle(self.pickle_file)
         self.save_vocab(self.vocab_file)
         self.feature_map.save(self.json_file)
         logging.info("Set feature processor done.")
 
-    def fit_meta_col(self, col, col_values):
+    def fit_meta_col(self, col):
         name = col["name"]
         feature_type = col["type"]
         self.feature_map.features[name] = {"type": feature_type}
-        # assert col.get("remap") == False, "Meta feature currently only supports `remap=False`, \
-            # since it needs to map train and validation sets together."
         if col.get("remap", True):
+            # No need to fit, update vocab in encode_meta()
             tokenizer = Tokenizer(min_freq=1, remap=True)
             self.processor_dict[name + "::tokenizer"] = tokenizer
 
-    def fit_numeric_col(self, col, col_values):
+    def fit_numeric_col(self, col, col_series):
         name = col["name"]
         feature_type = col["type"]
         feature_source = col.get("source", "")
         self.feature_map.features[name] = {"source": feature_source,
                                                 "type": feature_type}
         if "feature_encoder" in col:
             self.feature_map.features[name]["feature_encoder"] = col["feature_encoder"]
         if "normalizer" in col:
             normalizer = Normalizer(col["normalizer"])
-            normalizer.fit(col_values)
+            normalizer.fit(col_series.dropna().values)
             self.processor_dict[name + "::normalizer"] = normalizer
 
-    def fit_categorical_col(self, col, col_values, min_categr_count=1, num_buckets=10):
+    def fit_categorical_col(self, col, col_series, min_categr_count=1, num_buckets=10):
         name = col["name"]
         feature_type = col["type"]
         feature_source = col.get("source", "")
         min_categr_count = col.get("min_categr_count", min_categr_count)
         self.feature_map.features[name] = {"source": feature_source,
                                                 "type": feature_type}
         if "feature_encoder" in col:
@@ -202,15 +194,15 @@
             self.feature_map.features[name]["embedding_dim"] = col["embedding_dim"]
         if "emb_output_dim" in col:
             self.feature_map.features[name]["emb_output_dim"] = col["emb_output_dim"]
         if "category_processor" not in col:
             tokenizer = Tokenizer(min_freq=min_categr_count, 
                                   na_value=col.get("fill_na", ""), 
                                   remap=col.get("remap", True))
-            tokenizer.fit_on_texts(col_values)
+            tokenizer.fit_on_texts(col_series)
             if "share_embedding" in col:
                 self.feature_map.features[name]["share_embedding"] = col["share_embedding"]
                 tknzr_name = col["share_embedding"] + "::tokenizer"
                 # update vocab of both tokenizers
                 self.processor_dict[tknzr_name] = tokenizer.merge_vocab(self.processor_dict[tknzr_name])
                 self.feature_map.features[col["share_embedding"]] \
                                 .update({"oov_idx": self.processor_dict[tknzr_name].vocab["__OOV__"],
@@ -221,28 +213,26 @@
                                                     "vocab_size": tokenizer.vocab_size()})
         else:
             category_processor = col["category_processor"]
             self.feature_map.features[name]["category_processor"] = category_processor
             if category_processor == "quantile_bucket": # transform numeric value to bucket
                 num_buckets = col.get("num_buckets", num_buckets)
                 qtf = sklearn_preprocess.QuantileTransformer(n_quantiles=num_buckets + 1)
-                qtf.fit(col_values)
+                qtf.fit(col_series.values)
                 boundaries = qtf.quantiles_[1:-1]
                 self.feature_map.features[name]["vocab_size"] = num_buckets
                 self.processor_dict[name + "::boundaries"] = boundaries
             elif category_processor == "hash_bucket":
                 num_buckets = col.get("num_buckets", num_buckets)
-                uniques = Counter(col_values)
-                num_buckets = min(num_buckets, len(uniques))
                 self.feature_map.features[name]["vocab_size"] = num_buckets
                 self.processor_dict[name + "::num_buckets"] = num_buckets
             else:
                 raise NotImplementedError("category_processor={} not supported.".format(category_processor))
 
-    def fit_sequence_col(self, col, col_values, min_categr_count=1):
+    def fit_sequence_col(self, col, col_series, min_categr_count=1):
         name = col["name"]
         feature_type = col["type"]
         feature_source = col.get("source", "")
         min_categr_count = col.get("min_categr_count", min_categr_count)
         self.feature_map.features[name] = {"source": feature_source,
                                            "type": feature_type}
         feature_encoder = col.get("feature_encoder", "layers.MaskedAveragePooling()")
@@ -255,15 +245,15 @@
         splitter = col.get("splitter")
         na_value = col.get("fill_na", "")
         max_len = col.get("max_len", 0)
         padding = col.get("padding", "post") # "post" or "pre"
         tokenizer = Tokenizer(min_freq=min_categr_count, splitter=splitter, 
                               na_value=na_value, max_len=max_len, padding=padding,
                               remap=col.get("remap", True))
-        tokenizer.fit_on_texts(col_values)
+        tokenizer.fit_on_texts(col_series)
         if "share_embedding" in col:
             self.feature_map.features[name]["share_embedding"] = col["share_embedding"]
             tknzr_name = col["share_embedding"] + "::tokenizer"
             # update vocab of both tokenizers
             self.processor_dict[tknzr_name] = tokenizer.merge_vocab(self.processor_dict[tknzr_name])
             self.feature_map.features[col["share_embedding"]] \
                             .update({"oov_idx": self.processor_dict[tknzr_name].vocab["__OOV__"],
@@ -271,47 +261,47 @@
         self.processor_dict[name + "::tokenizer"] = tokenizer
         self.feature_map.features[name].update({"padding_idx": 0,
                                                 "oov_idx": tokenizer.vocab["__OOV__"],
                                                 "max_len": tokenizer.max_len,
                                                 "vocab_size": tokenizer.vocab_size()})
 
     def transform(self, ddf):
-        logging.info("Transform feature columns...")
+        logging.info("Transform feature columns with ID mapping...")
         data_dict = dict()
         for feature, feature_spec in self.feature_map.features.items():
             if feature in ddf.columns:
                 feature_type = feature_spec["type"]
-                col_values = ddf.loc[:, feature].values
+                col_series = ddf[feature]
                 if feature_type == "meta":
                     if feature + "::tokenizer" in self.processor_dict:
                         tokenizer = self.processor_dict[feature + "::tokenizer"]
-                        data_dict[feature] = tokenizer.encode_meta(col_values)
+                        data_dict[feature] = tokenizer.encode_meta(col_series)
                         # Update vocab in tokenizer
                         self.processor_dict[feature + "::tokenizer"] = tokenizer
                     else:
-                        data_dict[feature] = col_values.astype(self.dtype_dict[feature])
+                        data_dict[feature] = col_series.values
                 elif feature_type == "numeric":
-                    col_values = col_values.astype(float)
+                    col_values = col_series.values
                     normalizer = self.processor_dict.get(feature + "::normalizer")
                     if normalizer:
                          col_values = normalizer.transform(col_values)
                     data_dict[feature] = col_values
                 elif feature_type == "categorical":
                     category_processor = feature_spec.get("category_processor")
                     if category_processor is None:
-                        data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_category(col_values)
+                        data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_category(col_series)
                     elif category_processor == "numeric_bucket":
                         raise NotImplementedError
                     elif category_processor == "hash_bucket":
                         raise NotImplementedError
                 elif feature_type == "sequence":
-                    data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_sequence(col_values)
+                    data_dict[feature] = self.processor_dict.get(feature + "::tokenizer").encode_sequence(col_series)
         for label in self.feature_map.labels:
             if label in ddf.columns:
-                data_dict[label] = ddf.loc[:, label].values
+                data_dict[label] = ddf[label].values
         return data_dict
 
     def load_pickle(self, pickle_file=None):
         """ Load feature processor from cache """
         if pickle_file is None:
             pickle_file = self.pickle_file
         logging.info("Load feature_processor from pickle: " + pickle_file)
@@ -331,10 +321,10 @@
         for feature, spec in self.feature_map.features.items():
             if spec["type"] in ["categorical", "sequence"]:
                 vocab[feature] = OrderedDict(
                     sorted(self.processor_dict[feature + "::tokenizer"].vocab.items(), key=lambda x:x[1]))
         with open(vocab_file, "w") as fd:
             fd.write(json.dumps(vocab, indent=4))
 
-    def copy_from(self, ddf, src_name):
-        return ddf[src_name]
-
+    def copy_from(self, ddf, name, src_name):
+        ddf = ddf.with_columns(pl.col(src_name).alias(name))
+        return ddf
```

### Comparing `fuxictr-2.2.1/fuxictr/preprocess/normalizer.py` & `fuxictr-2.2.2/fuxictr/preprocess/normalizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         else:
             # normalizer is a method
             self.normalizer = normalizer
             self.callable = True
 
     def fit(self, X):
         if not self.callable:
-            null_index = np.isnan(X)
-            self.normalizer.fit(X[~null_index].reshape(-1, 1))
+            self.normalizer.fit(X.reshape(-1, 1))
 
     def transform(self, X):
         if self.callable:
             return self.normalizer(X)
         else:
             return self.normalizer.transform(X.reshape(-1, 1)).flatten()
```

### Comparing `fuxictr-2.2.1/fuxictr/preprocess/tokenizer.py` & `fuxictr-2.2.2/fuxictr/preprocess/tokenizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,50 +12,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========================================================================
 
 from collections import Counter
 import numpy as np
-import pandas as pd
 import h5py
 from tqdm import tqdm
+import polars as pl
 from keras_preprocessing.sequence import pad_sequences
 from concurrent.futures import ProcessPoolExecutor, as_completed
+import multiprocessing as mp
 
 
 class Tokenizer(object):
     def __init__(self, max_features=None, na_value="", min_freq=1, splitter=None, remap=True,
-                 lower=False, max_len=0, padding="pre", num_workers=8):
+                 lower=False, max_len=0, padding="pre"):
         self._max_features = max_features
         self._na_value = na_value
         self._min_freq = min_freq
         self._lower = lower
         self._splitter = splitter
         self.vocab = dict()
         self.max_len = max_len
         self.padding = padding
-        self.num_workers = num_workers
         self.remap = remap
 
-    def fit_on_texts(self, texts):
+    def fit_on_texts(self, series):
+        max_len = 0
         word_counts = Counter()
-        if self._splitter is not None: # for sequence
-            max_len = 0
-            with ProcessPoolExecutor(max_workers=self.num_workers) as executor:
-                chunks = np.array_split(texts, self.num_workers)
-                tasks = [executor.submit(count_tokens, chunk, self._splitter) for chunk in chunks]
-                for future in tqdm(as_completed(tasks), total=len(tasks)):
-                    block_word_counts, block_max_len = future.result()
-                    word_counts.update(block_word_counts)
-                    max_len = max(max_len, block_max_len)
-            if self.max_len == 0:  # if argument max_len not given
-                self.max_len = max_len
-        else:
-            word_counts = Counter(list(texts))
+        with ProcessPoolExecutor(max_workers=(mp.cpu_count() // 2)) as executor:
+            chunk_size = 1000000
+            tasks = []
+            for idx in range(0, len(series), chunk_size):
+                data_chunk = series.iloc[idx: (idx + chunk_size)]
+                tasks.append(executor.submit(count_tokens, data_chunk, self._splitter))
+            for future in tqdm(as_completed(tasks), total=len(tasks)):
+                chunk_word_counts, chunk_max_len = future.result()
+                word_counts.update(chunk_word_counts)
+                max_len = max(max_len, chunk_max_len)
+        if self.max_len == 0:  # if argument max_len not given
+            self.max_len = max_len
         self.build_vocab(word_counts)
 
     def build_vocab(self, word_counts):
         word_counts = word_counts.items()
         # sort to guarantee the determinism of index order
         word_counts = sorted(word_counts, key=lambda x: (-x[1], x[0]))
         if self._max_features: # keep the most frequent features
@@ -97,38 +97,36 @@
         for word in word_list:
             if word not in self.vocab:
                 self.vocab[word] = self.vocab["__OOV__"] + new_words
                 new_words += 1
         if new_words > 0:
             self.vocab["__OOV__"] = self.vocab_size()
 
-    def encode_meta(self, values):
-        word_counts = Counter(list(values))
+    def encode_meta(self, series):
+        word_counts = dict(series.value_counts())
         if len(self.vocab) == 0:
             self.build_vocab(word_counts)
         else: # for considering meta data in test data
             self.update_vocab(word_counts.keys())
-        meta_values = [self.vocab.get(x, self.vocab["__OOV__"]) for x in values]
-        return np.array(meta_values)
+        series = series.map(lambda x: self.vocab.get(x, self.vocab["__OOV__"]))
+        return series.values
 
-    def encode_category(self, categories):
-        category_indices = [self.vocab.get(x, self.vocab["__OOV__"]) for x in categories]
-        return np.array(category_indices)
-
-    def encode_sequence(self, texts):
-        sequence_list = []
-        for text in texts:
-            if pd.isnull(text) or text == '':
-                sequence_list.append([])
-            else:
-                sequence_list.append([self.vocab.get(x, self.vocab["__OOV__"]) if x != self._na_value \
-                                      else self.vocab["__PAD__"] for x in text.split(self._splitter)])
-        sequence_list = pad_sequences(sequence_list, maxlen=self.max_len, value=self.vocab["__PAD__"],
-                                      padding=self.padding, truncating=self.padding)
-        return np.array(sequence_list)
+    def encode_category(self, series):
+        series = series.map(lambda x: self.vocab.get(x, self.vocab["__OOV__"]))
+        return series.values
+
+    def encode_sequence(self, series):
+        series = series.map(
+            lambda text: [self.vocab.get(x, self.vocab["__OOV__"]) if x != self._na_value \
+            else self.vocab["__PAD__"] for x in text.split(self._splitter)]
+        )
+        seqs = pad_sequences(series.to_list(), maxlen=self.max_len,
+                             value=self.vocab["__PAD__"],
+                             padding=self.padding, truncating=self.padding)
+        return np.array(seqs)
     
     def load_pretrained_vocab(self, feature_dtype, pretrain_path, expand_vocab=True):
         if pretrain_path.endswith(".h5"):
             with h5py.File(pretrain_path, 'r') as hf:
                 keys = hf["key"][:]
                 # in case mismatch of dtype between int and str
                 keys = keys.astype(feature_dtype)
@@ -140,16 +138,16 @@
             vocab_size = self.vocab_size()
             for word in keys:
                 if word not in self.vocab:
                     self.vocab[word] = vocab_size
                     vocab_size += 1
 
 
-def count_tokens(texts, splitter):
-    word_counts = Counter()
+def count_tokens(series, splitter=None):
     max_len = 0
-    for text in texts:
-        text_split = text.split(splitter)
-        max_len = max(max_len, len(text_split))
-        for token in text_split:
-            word_counts[token] += 1
-    return word_counts, max_len
+    if splitter is not None: # for sequence
+        series = series.map(lambda text: text.split(splitter))
+        max_len = series.str.len().max()
+        word_counts = series.explode().value_counts()
+    else:
+        word_counts = series.value_counts()
+    return dict(word_counts), max_len
```

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_block_dataloader.py` & `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_block_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         self.num_blocks = len(self.data_blocks)
         self.feature_map = feature_map
         self.batch_size = batch_size
         self.num_batches, self.num_samples = self.count_batches_and_samples()
         datapipe = BlockDataPipe(data_blocks, feature_map)
         if shuffle:
             datapipe = datapipe.shuffle(buffer_size=buffer_size)
+        else:
+            num_workers = 1 # multiple workers cannot keep the order of data reading 
         super(NpzBlockDataLoader, self).__init__(dataset=datapipe, batch_size=batch_size,
                                                  num_workers=num_workers)
 
     def __len__(self):
         return self.num_batches
 
     def count_batches_and_samples(self):
```

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_dataloader.py` & `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/rank_dataloader.py` & `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/rank_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.2.2/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.2.2/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/models/rank_model.py` & `fuxictr-2.2.2/fuxictr/pytorch/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.2.2/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.2.2/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/models/rank_model.py` & `fuxictr-2.2.2/fuxictr/tensorflow/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.2.2/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr/utils.py` & `fuxictr-2.2.2/fuxictr/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.2.2/fuxictr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.1
+Version: 2.2.2
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.1 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.2 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.1/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.2.2/fuxictr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.1/setup.py` & `fuxictr-2.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.2.1",
+    version="2.2.2",
     author="RECZOO",
     author_email="reczoo@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/reczoo/FuxiCTR",
     download_url='https://github.com/reczoo/FuxiCTR/tags',
```

