# Comparing `tmp/vjepa_encoder-0.0.3.tar.gz` & `tmp/vjepa_encoder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjepa_encoder-0.0.3.tar", last modified: Fri Apr 12 18:35:29 2024, max compression
+gzip compressed data, was "dist/vjepa_encoder-0.0.4.tar", last modified: Wed Apr 17 01:37:07 2024, max compression
```

## Comparing `vjepa_encoder-0.0.3.tar` & `vjepa_encoder-0.0.4.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    19337 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/LICENSE
--rw-r--r--   0 rpal      (1000) rpal      (1000)      449 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/PKG-INFO
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2816 2024-04-12 06:43:46.000000 vjepa_encoder-0.0.3/README.md
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.470041 vjepa_encoder-0.0.3/jepa_src/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:15.000000 vjepa_encoder-0.0.3/jepa_src/__init__.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.470041 vjepa_encoder-0.0.3/jepa_src/datasets/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:34.000000 vjepa_encoder-0.0.3/jepa_src/datasets/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2644 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/data_manager.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2079 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/image_dataset.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.470041 vjepa_encoder-0.0.3/jepa_src/datasets/utils/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:36.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/__init__.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:39.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     3116 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/functional.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    15452 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/randaugment.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     6809 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/randerase.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    40437 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/transforms.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     4729 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/volume_transforms.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2727 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/utils/weighted_sampler.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     9500 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/datasets/video_dataset.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/jepa_src/masks/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:28.000000 vjepa_encoder-0.0.3/jepa_src/masks/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)      456 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/masks/default.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     7259 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/masks/multiblock3d.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     3643 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/masks/random_tube.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)      681 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/masks/utils.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/jepa_src/models/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:24.000000 vjepa_encoder-0.0.3/jepa_src/models/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     4130 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/models/attentive_pooler.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     8582 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/models/predictor.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/jepa_src/models/utils/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:26.000000 vjepa_encoder-0.0.3/jepa_src/models/utils/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     5334 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/models/utils/modules.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     1322 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/models/utils/multimask.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     1372 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/models/utils/patch_embed.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     3579 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/models/utils/pos_embs.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    10154 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/jepa_src/models/vision_transformer.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/jepa_src/utils/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:19.000000 vjepa_encoder-0.0.3/jepa_src/utils/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     3037 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/utils/distributed.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     3519 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/utils/logging.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     5973 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/utils/monitoring.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2138 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/utils/schedulers.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     2220 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.3/jepa_src/utils/tensors.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)       38 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/setup.cfg
--rw-rw-r--   0 rpal      (1000) rpal      (1000)      735 2024-04-12 18:35:20.000000 vjepa_encoder-0.0.3/setup.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/vjepa_encoder/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 04:16:49.000000 vjepa_encoder-0.0.3/vjepa_encoder/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    12271 2024-04-12 07:03:38.000000 vjepa_encoder-0.0.3/vjepa_encoder/vision_encoder.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/vjepa_encoder/vjepa/
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 04:18:47.000000 vjepa_encoder-0.0.3/vjepa_encoder/vjepa/__init__.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)    22405 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/vjepa_encoder/vjepa/train.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     5061 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/vjepa_encoder/vjepa/transforms.py
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     6166 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.3/vjepa_encoder/vjepa/utils.py
-drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-12 18:35:29.474042 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/
--rw-r--r--   0 rpal      (1000) rpal      (1000)      449 2024-04-12 18:35:29.000000 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/PKG-INFO
--rw-rw-r--   0 rpal      (1000) rpal      (1000)     1505 2024-04-12 18:35:29.000000 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/SOURCES.txt
--rw-rw-r--   0 rpal      (1000) rpal      (1000)        1 2024-04-12 18:35:29.000000 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/dependency_links.txt
--rw-rw-r--   0 rpal      (1000) rpal      (1000)       94 2024-04-12 18:35:29.000000 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/requires.txt
--rw-rw-r--   0 rpal      (1000) rpal      (1000)       23 2024-04-12 18:35:29.000000 vjepa_encoder-0.0.3/vjepa_encoder.egg-info/top_level.txt
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    19337 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/LICENSE
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)      190 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/PKG-INFO
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3345 2024-04-17 01:33:59.000000 vjepa_encoder-0.0.4/README.md
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:15.000000 vjepa_encoder-0.0.4/jepa_src/__init__.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/datasets/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:34.000000 vjepa_encoder-0.0.4/jepa_src/datasets/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     2644 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/data_manager.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     2079 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/image_dataset.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:36.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/__init__.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:39.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3116 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/functional.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    15452 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/randaugment.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     6809 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/randerase.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    40437 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/transforms.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     4729 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/volume_transforms.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     2727 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/utils/weighted_sampler.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     9500 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/datasets/video_dataset.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/masks/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:28.000000 vjepa_encoder-0.0.4/jepa_src/masks/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)      456 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/masks/default.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     7259 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/masks/multiblock3d.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3643 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/masks/random_tube.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)      681 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/masks/utils.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/models/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:24.000000 vjepa_encoder-0.0.4/jepa_src/models/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     4130 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/models/attentive_pooler.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     8582 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/models/predictor.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:26.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     5375 2024-04-17 01:33:00.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/modules.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     1322 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/multimask.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     1372 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/patch_embed.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3579 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/models/utils/pos_embs.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    10154 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/jepa_src/models/vision_transformer.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/jepa_src/utils/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 06:54:19.000000 vjepa_encoder-0.0.4/jepa_src/utils/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3037 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/utils/distributed.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     1099 2024-04-17 00:37:23.000000 vjepa_encoder-0.0.4/jepa_src/utils/functional.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     3519 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/utils/logging.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     5973 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/utils/monitoring.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     2138 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/utils/schedulers.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     2220 2024-04-10 05:44:03.000000 vjepa_encoder-0.0.4/jepa_src/utils/tensors.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)       38 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/setup.cfg
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)      735 2024-04-17 01:32:24.000000 vjepa_encoder-0.0.4/setup.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 04:16:49.000000 vjepa_encoder-0.0.4/vjepa_encoder/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    12271 2024-04-12 07:03:38.000000 vjepa_encoder-0.0.4/vjepa_encoder/vision_encoder.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder/vjepa/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        0 2024-04-12 04:18:47.000000 vjepa_encoder-0.0.4/vjepa_encoder/vjepa/__init__.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)    22405 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/vjepa_encoder/vjepa/train.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     5061 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/vjepa_encoder/vjepa/transforms.py
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     6166 2024-04-12 03:38:03.000000 vjepa_encoder-0.0.4/vjepa_encoder/vjepa/utils.py
+drwxrwxr-x   0 rpal      (1000) rpal      (1000)        0 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)      190 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/PKG-INFO
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)     1534 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)        1 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)       94 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/requires.txt
+-rw-rw-r--   0 rpal      (1000) rpal      (1000)       23 2024-04-17 01:37:07.000000 vjepa_encoder-0.0.4/vjepa_encoder.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `vjepa_encoder-0.0.3/LICENSE` & `vjepa_encoder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/README.md` & `vjepa_encoder-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The VJEPA Encoder is a Python package that provides an implementation of the encoder component from the JEPA (Joint Encoding for Prediction and Alignment) architecture proposed by Facebook AI Research. The encoder is designed to extract meaningful representations from visual data. I do not own the rights or lay claim to the copyright of this software. This package is an adaptation to `facebookresearch/jepa` to enable ease of use of the Jepa Architecture built with Vision Transformers.
 
 ## Installation
 
 To install the VJEPA Encoder package, you can use pip:
 
 ```
-pip install vjepa_encoder
+pip install vjepa-encoder
 ```
 
 ## Usage
 
 To use the VJEPA Encoder in your Python code, you can import it as follows:
 
 ```python
@@ -27,14 +27,19 @@
 devices = ["cuda:0"]
 encoder = JepaEncoder.load_model(config_file_path, devices)
 ```
 
 - `config_file_path`: Path to the configuration file (YAML) containing the model settings.
 - `devices`: List of devices (e.g., `['cuda:0']`) to use for distributed training. If not provided, the model will be loaded on the CPU.
 
+
+#### Important Notes about the Config File:
+
+- the config file provided in this repo provides the basics for loading and using the encoder. The most important things to note in this file are the `r_checkpoint`: points at the `.tar` file for the JEPA checkpoint, and the `tabulet_size`: this is used in some temporal calculation and if you plan on embedding images you should set this to `1`; set this to `N` if you plan on using a temporal dimension for your data, where N corresponds to however many temporal inputs you have.
+
 ### Preprocessing Data
 
 The VJEPA Encoder provides a `preprocess_data` function to preprocess input data before feeding it to the encoder:
 
 ```python
 preprocessed_data = encoder.preprocess_data(input_data)
 ```
```

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/data_manager.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/data_manager.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/image_dataset.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/functional.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/functional.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/randaugment.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/randaugment.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/randerase.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/randerase.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/transforms.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/transforms.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/video/volume_transforms.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/video/volume_transforms.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/utils/weighted_sampler.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/utils/weighted_sampler.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/datasets/video_dataset.py` & `vjepa_encoder-0.0.4/jepa_src/datasets/video_dataset.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/masks/multiblock3d.py` & `vjepa_encoder-0.0.4/jepa_src/masks/multiblock3d.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/masks/random_tube.py` & `vjepa_encoder-0.0.4/jepa_src/masks/random_tube.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/masks/utils.py` & `vjepa_encoder-0.0.4/jepa_src/masks/utils.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/attentive_pooler.py` & `vjepa_encoder-0.0.4/jepa_src/models/attentive_pooler.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/predictor.py` & `vjepa_encoder-0.0.4/jepa_src/models/predictor.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/utils/modules.py` & `vjepa_encoder-0.0.4/jepa_src/models/utils/modules.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 #
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+import jepa_src.utils.functional as JF
 
 class MLP(nn.Module):
     def __init__(
         self,
         in_features,
         hidden_features=None,
         out_features=None,
@@ -61,15 +62,15 @@
     def forward(self, x, mask=None):
         B, N, C = x.shape
         qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 1, 4)
         q, k, v = qkv[0], qkv[1], qkv[2]  # [B, num_heads, N, D]
 
         if self.use_sdpa:
             with torch.backends.cuda.sdp_kernel():
-                x = F.scaled_dot_product_attention(q, k, v, dropout_p=self.proj_drop_prob)
+                x = JF.scaled_dot_product_attention(q, k, v, dropout_p=self.proj_drop_prob)
                 attn = None
         else:
             attn = (q @ k.transpose(-2, -1)) * self.scale  # [B, num_heads, D, D]
             attn = attn.softmax(dim=-1)
             attn = self.attn_drop(attn)
             x = (attn @ v)
         x = x.transpose(1, 2).reshape(B, N, C)
@@ -143,15 +144,15 @@
 
         B, N, C = x.shape
         kv = self.kv(x).reshape(B, N, 2, self.num_heads, C // self.num_heads).permute(2, 0, 3, 1, 4)
         k, v = kv[0], kv[1]  # (batch_size, num_heads, seq_len, feature_dim_per_head)
 
         if self.use_sdpa:
             with torch.backends.cuda.sdp_kernel():
-                q = F.scaled_dot_product_attention(q, k, v)
+                q = JF.scaled_dot_product_attention(q, k, v)
         else:
             xattn = (q @ k.transpose(-2, -1)) * self.scale
             xattn = xattn.softmax(dim=-1)  # (batch_size, num_heads, query_len, seq_len)
             q = (xattn @ v)
 
         q = q.transpose(1, 2).reshape(B, n, C)
         q = self.proj(q)
```

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/utils/multimask.py` & `vjepa_encoder-0.0.4/jepa_src/models/utils/multimask.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/utils/patch_embed.py` & `vjepa_encoder-0.0.4/jepa_src/models/utils/patch_embed.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/utils/pos_embs.py` & `vjepa_encoder-0.0.4/jepa_src/models/utils/pos_embs.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/models/vision_transformer.py` & `vjepa_encoder-0.0.4/jepa_src/models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/utils/distributed.py` & `vjepa_encoder-0.0.4/jepa_src/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/utils/logging.py` & `vjepa_encoder-0.0.4/jepa_src/utils/logging.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/utils/monitoring.py` & `vjepa_encoder-0.0.4/jepa_src/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/utils/schedulers.py` & `vjepa_encoder-0.0.4/jepa_src/utils/schedulers.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/jepa_src/utils/tensors.py` & `vjepa_encoder-0.0.4/jepa_src/utils/tensors.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/setup.py` & `vjepa_encoder-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 #
 
 import os
 from setuptools import setup
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 from setuptools import setup, find_packages
 
 def get_requirements():
     with open("./requirements.txt") as reqsf:
         reqs = reqsf.readlines()
     return reqs
@@ -20,11 +20,11 @@
 if __name__ == "__main__":
     setup(
         name="vjepa_encoder",
         version=VERSION,
         description="JEPA research code.",
         author="Jonathan Koch",
         author_email="johnnykoch02@gmail.com",
-        python_requires=">=3.9",
+        python_requires=">=3.7",
         packages=find_packages(),
         install_requires=get_requirements(),
     )
```

### Comparing `vjepa_encoder-0.0.3/vjepa_encoder/vision_encoder.py` & `vjepa_encoder-0.0.4/vjepa_encoder/vision_encoder.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/vjepa_encoder/vjepa/train.py` & `vjepa_encoder-0.0.4/vjepa_encoder/vjepa/train.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/vjepa_encoder/vjepa/transforms.py` & `vjepa_encoder-0.0.4/vjepa_encoder/vjepa/transforms.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/vjepa_encoder/vjepa/utils.py` & `vjepa_encoder-0.0.4/vjepa_encoder/vjepa/utils.py`

 * *Files identical despite different names*

### Comparing `vjepa_encoder-0.0.3/vjepa_encoder.egg-info/SOURCES.txt` & `vjepa_encoder-0.0.4/vjepa_encoder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 jepa_src/models/utils/__init__.py
 jepa_src/models/utils/modules.py
 jepa_src/models/utils/multimask.py
 jepa_src/models/utils/patch_embed.py
 jepa_src/models/utils/pos_embs.py
 jepa_src/utils/__init__.py
 jepa_src/utils/distributed.py
+jepa_src/utils/functional.py
 jepa_src/utils/logging.py
 jepa_src/utils/monitoring.py
 jepa_src/utils/schedulers.py
 jepa_src/utils/tensors.py
 vjepa_encoder/__init__.py
 vjepa_encoder/vision_encoder.py
 vjepa_encoder.egg-info/PKG-INFO
```

