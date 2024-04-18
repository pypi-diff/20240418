# Comparing `tmp/bert4torch-0.4.9.post2.tar.gz` & `tmp/bert4torch-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.4.9.post2.tar", last modified: Sun Mar 17 15:36:58 2024, max compression
+gzip compressed data, was "bert4torch-0.5.0.tar", last modified: Thu Apr 18 15:51:53 2024, max compression
```

## Comparing `bert4torch-0.4.9.post2.tar` & `bert4torch-0.5.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.296209 bert4torch-0.4.9.post2/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.4.9.post2/LICENSE
--rw-rw-rw-   0        0        0    35497 2024-03-17 15:36:58.294215 bert4torch-0.4.9.post2/PKG-INFO
--rw-rw-rw-   0        0        0    35241 2024-03-17 15:34:52.000000 bert4torch-0.4.9.post2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.182206 bert4torch-0.4.9.post2/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.4.9.post2/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/activations.py
--rw-rw-rw-   0        0        0    11035 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    51934 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/generation.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.206234 bert4torch-0.4.9.post2/bert4torch/layers/
--rw-rw-rw-   0        0        0      332 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/__init__.py
--rw-rw-rw-   0        0        0    35115 2024-03-17 15:14:57.000000 bert4torch-0.4.9.post2/bert4torch/layers/attention.py
--rw-rw-rw-   0        0        0    12069 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/core.py
--rw-rw-rw-   0        0        0    12699 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/layers/crf.py
--rw-rw-rw-   0        0        0     4688 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/global_point.py
--rw-rw-rw-   0        0        0    18574 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/misc.py
--rw-rw-rw-   0        0        0     6294 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/moe.py
--rw-rw-rw-   0        0        0    14954 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/position_encoding.py
--rw-rw-rw-   0        0        0    16762 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/layers/transformer_block.py
--rw-rw-rw-   0        0        0    19802 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/losses.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.246195 bert4torch-0.4.9.post2/bert4torch/models/
--rw-rw-rw-   0        0        0    11469 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/models/__init__.py
--rw-rw-rw-   0        0        0     7709 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/albert.py
--rw-rw-rw-   0        0        0     8073 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/bart.py
--rw-rw-rw-   0        0        0    26026 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/models/base.py
--rw-rw-rw-   0        0        0    21558 2024-02-21 15:55:42.000000 bert4torch-0.4.9.post2/bert4torch/models/bert.py
--rw-rw-rw-   0        0        0     4116 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/bloom.py
--rw-rw-rw-   0        0        0     5135 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/deberta.py
--rw-rw-rw-   0        0        0     4345 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/deepseek.py
--rw-rw-rw-   0        0        0     2311 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/electra.py
--rw-rw-rw-   0        0        0     2408 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/ernie.py
--rw-rw-rw-   0        0        0     7964 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/falcon.py
--rw-rw-rw-   0        0        0     1829 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/gau_alpha.py
--rw-rw-rw-   0        0        0    15938 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/glm.py
--rw-rw-rw-   0        0        0    16830 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/gpt.py
--rw-rw-rw-   0        0        0     2900 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/internlm.py
--rw-rw-rw-   0        0        0     4380 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/models/llama.py
--rw-rw-rw-   0        0        0      954 2024-02-21 15:55:42.000000 bert4torch-0.4.9.post2/bert4torch/models/nezha.py
--rw-rw-rw-   0        0        0     3326 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/qwen.py
--rw-rw-rw-   0        0        0     2537 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/roformer.py
--rw-rw-rw-   0        0        0    10675 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/t5.py
--rw-rw-rw-   0        0        0     9089 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/transformer.py
--rw-rw-rw-   0        0        0    13015 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/transformer_xl.py
--rw-rw-rw-   0        0        0     2742 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/uie.py
--rw-rw-rw-   0        0        0     6710 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/bert4torch/models/xlnet.py
--rw-rw-rw-   0        0        0     7640 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/optimizers.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.253193 bert4torch-0.4.9.post2/bert4torch/pipelines/
--rw-rw-rw-   0        0        0      171 2024-02-21 15:55:42.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/__init__.py
--rw-rw-rw-   0        0        0     1412 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/base.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.259229 bert4torch-0.4.9.post2/bert4torch/pipelines/chat/
--rw-rw-rw-   0        0        0      191 2024-01-10 16:17:12.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/chat/__init__.py
--rw-rw-rw-   0        0        0    15028 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/chat/base.py
--rw-rw-rw-   0        0        0    13543 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/chat/llm.py
--rw-rw-rw-   0        0        0    17120 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/chat/openai_api.py
--rw-rw-rw-   0        0        0     3394 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/fill_mask.py
--rw-rw-rw-   0        0        0     3472 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/text2vec.py
--rw-rw-rw-   0        0        0    19246 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/pipelines/uie_predictor.py
--rw-rw-rw-   0        0        0    20925 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/quantization.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.271193 bert4torch-0.4.9.post2/bert4torch/snippets/
--rw-rw-rw-   0        0        0      209 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/snippets/__init__.py
--rw-rw-rw-   0        0        0    24362 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/snippets/data_process.py
--rw-rw-rw-   0        0        0    12605 2024-03-17 15:16:36.000000 bert4torch-0.4.9.post2/bert4torch/snippets/hub.py
--rw-rw-rw-   0        0        0     1492 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/snippets/import_utils.py
--rw-rw-rw-   0        0        0    11499 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/snippets/misc.py
--rw-rw-rw-   0        0        0    37004 2024-02-21 15:55:42.000000 bert4torch-0.4.9.post2/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.281211 bert4torch-0.4.9.post2/bert4torch/trainer/
--rw-rw-rw-   0        0        0      349 2024-02-21 15:55:42.000000 bert4torch-0.4.9.post2/bert4torch/trainer/__init__.py
--rw-rw-rw-   0        0        0     1159 2023-12-26 07:11:58.000000 bert4torch-0.4.9.post2/bert4torch/trainer/dpo_trainer.py
--rw-rw-rw-   0        0        0     6898 2024-01-10 16:17:12.000000 bert4torch-0.4.9.post2/bert4torch/trainer/ppo_trainer.py
--rw-rw-rw-   0        0        0     4090 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/trainer/ptuningv2_trainer.py
--rw-rw-rw-   0        0        0     1416 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/bert4torch/trainer/sequence_classification_trainer.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.189233 bert4torch-0.4.9.post2/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    35497 2024-03-17 15:36:57.000000 bert4torch-0.4.9.post2/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2163 2024-03-17 15:36:58.000000 bert4torch-0.4.9.post2/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 15:36:57.000000 bert4torch-0.4.9.post2/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-17 15:36:57.000000 bert4torch-0.4.9.post2/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-17 15:36:57.000000 bert4torch-0.4.9.post2/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 15:36:58.297214 bert4torch-0.4.9.post2/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-03-17 15:26:51.000000 bert4torch-0.4.9.post2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 15:36:58.292195 bert4torch-0.4.9.post2/test/
--rw-rw-rw-   0        0        0      638 2024-02-21 15:55:43.000000 bert4torch-0.4.9.post2/test/test_entity_extract_rule.py
--rw-rw-rw-   0        0        0      593 2024-02-21 15:55:43.000000 bert4torch-0.4.9.post2/test/test_fill_mask.py
--rw-rw-rw-   0        0        0      731 2024-02-21 15:55:43.000000 bert4torch-0.4.9.post2/test/test_generate_speed.py
--rw-rw-rw-   0        0        0     9120 2024-02-21 15:55:43.000000 bert4torch-0.4.9.post2/test/test_hf_download.py
--rw-rw-rw-   0        0        0     5939 2024-02-04 09:55:51.000000 bert4torch-0.4.9.post2/test/test_save_pretrained.py
--rw-rw-rw-   0        0        0     2216 2024-03-16 07:47:39.000000 bert4torch-0.4.9.post2/test/test_tokenizer.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.599403 bert4torch-0.5.0/
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1068 2024-03-07 08:23:49.000000 bert4torch-0.5.0/LICENSE
+-rw-r--r--   0 lb        (1000) lb        (1000)    35172 2024-04-18 15:51:53.599403 bert4torch-0.5.0/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)    35050 2024-04-18 15:44:23.000000 bert4torch-0.5.0/README.md
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.595403 bert4torch-0.5.0/bert4torch/
+-rw-rw-r--   0 lb        (1000) lb        (1000)        0 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3257 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/activations.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    11035 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/callbacks.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    52034 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/generation.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.595403 bert4torch-0.5.0/bert4torch/layers/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      332 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/layers/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    35905 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/layers/attention.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12516 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/layers/core.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12699 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/layers/crf.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     4788 2024-03-31 15:30:03.000000 bert4torch-0.5.0/bert4torch/layers/global_point.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    18574 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/layers/misc.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     6294 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/layers/moe.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    14954 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/layers/position_encoding.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    17065 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/layers/transformer_block.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    20697 2024-03-28 15:23:07.000000 bert4torch-0.5.0/bert4torch/losses.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.595403 bert4torch-0.5.0/bert4torch/models/
+-rw-rw-r--   0 lb        (1000) lb        (1000)    11467 2024-04-08 10:45:09.000000 bert4torch-0.5.0/bert4torch/models/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     7709 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/albert.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     8073 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/bart.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    26592 2024-04-18 01:14:44.000000 bert4torch-0.5.0/bert4torch/models/base.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    21719 2024-04-03 14:00:16.000000 bert4torch-0.5.0/bert4torch/models/bert.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     4116 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/bloom.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     5135 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/deberta.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     4345 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/deepseek.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2311 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/electra.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2408 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/ernie.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     7964 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/falcon.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1829 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/gau_alpha.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    15938 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/glm.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    16830 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/gpt.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2900 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/internlm.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     4380 2024-03-18 01:00:54.000000 bert4torch-0.5.0/bert4torch/models/llama.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      954 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/nezha.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3326 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/qwen.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2537 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/roformer.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    10675 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/t5.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     9089 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/transformer.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    13015 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/transformer_xl.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2742 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/uie.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     6710 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/models/xlnet.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     7640 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/optimizers.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.595403 bert4torch-0.5.0/bert4torch/pipelines/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      171 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/pipelines/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1767 2024-04-03 06:04:32.000000 bert4torch-0.5.0/bert4torch/pipelines/base.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.599403 bert4torch-0.5.0/bert4torch/pipelines/chat/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      191 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/pipelines/chat/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    15652 2024-03-21 02:40:10.000000 bert4torch-0.5.0/bert4torch/pipelines/chat/base.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    13917 2024-03-20 10:23:45.000000 bert4torch-0.5.0/bert4torch/pipelines/chat/llm.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    18195 2024-04-10 06:55:49.000000 bert4torch-0.5.0/bert4torch/pipelines/chat/openai_api.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3394 2024-03-15 07:28:55.000000 bert4torch-0.5.0/bert4torch/pipelines/fill_mask.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     3713 2024-04-03 06:23:39.000000 bert4torch-0.5.0/bert4torch/pipelines/text2vec.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    19246 2024-03-15 07:28:55.000000 bert4torch-0.5.0/bert4torch/pipelines/uie_predictor.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    21344 2024-04-18 06:11:49.000000 bert4torch-0.5.0/bert4torch/quantization.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.599403 bert4torch-0.5.0/bert4torch/snippets/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      209 2024-03-07 09:48:25.000000 bert4torch-0.5.0/bert4torch/snippets/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    24899 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/snippets/data_process.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    12914 2024-04-03 07:50:06.000000 bert4torch-0.5.0/bert4torch/snippets/hub.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1492 2024-03-07 09:48:25.000000 bert4torch-0.5.0/bert4torch/snippets/import_utils.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    11535 2024-04-05 04:43:37.000000 bert4torch-0.5.0/bert4torch/snippets/misc.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)    37075 2024-04-03 15:07:27.000000 bert4torch-0.5.0/bert4torch/tokenizers.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.599403 bert4torch-0.5.0/bert4torch/trainer/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      349 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/trainer/__init__.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1159 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/trainer/dpo_trainer.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     6898 2024-03-07 08:23:49.000000 bert4torch-0.5.0/bert4torch/trainer/ppo_trainer.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     4090 2024-03-07 09:48:25.000000 bert4torch-0.5.0/bert4torch/trainer/ptuningv2_trainer.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     1416 2024-03-07 09:48:25.000000 bert4torch-0.5.0/bert4torch/trainer/sequence_classification_trainer.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.595403 bert4torch-0.5.0/bert4torch.egg-info/
+-rw-r--r--   0 lb        (1000) lb        (1000)    35172 2024-04-18 15:51:53.000000 bert4torch-0.5.0/bert4torch.egg-info/PKG-INFO
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2163 2024-04-18 15:51:53.000000 bert4torch-0.5.0/bert4torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)        1 2024-04-18 15:51:53.000000 bert4torch-0.5.0/bert4torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       44 2024-04-18 15:51:53.000000 bert4torch-0.5.0/bert4torch.egg-info/requires.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       11 2024-04-18 15:51:53.000000 bert4torch-0.5.0/bert4torch.egg-info/top_level.txt
+-rw-rw-r--   0 lb        (1000) lb        (1000)       38 2024-04-18 15:51:53.599403 bert4torch-0.5.0/setup.cfg
+-rw-rw-r--   0 lb        (1000) lb        (1000)      575 2024-04-18 15:40:53.000000 bert4torch-0.5.0/setup.py
+drwxrwxr-x   0 lb        (1000) lb        (1000)        0 2024-04-18 15:51:53.599403 bert4torch-0.5.0/test/
+-rw-rw-r--   0 lb        (1000) lb        (1000)      638 2024-03-07 08:23:49.000000 bert4torch-0.5.0/test/test_entity_extract_rule.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      593 2024-03-07 08:23:49.000000 bert4torch-0.5.0/test/test_fill_mask.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)      731 2024-03-07 08:23:49.000000 bert4torch-0.5.0/test/test_generate_speed.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     9120 2024-03-07 08:23:49.000000 bert4torch-0.5.0/test/test_hf_download.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     5939 2024-03-21 02:55:17.000000 bert4torch-0.5.0/test/test_save_pretrained.py
+-rw-rw-r--   0 lb        (1000) lb        (1000)     2216 2024-03-07 09:48:25.000000 bert4torch-0.5.0/test/test_tokenizer.py
```

### Comparing `bert4torch-0.4.9.post2/PKG-INFO` & `bert4torch-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.4.9.post2
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![bert4torch](./docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -99,18 +89,17 @@
 - [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本和更新历史
 ### 4.1 版本历史
 |更新日期| bert4torch | torch4keras | 版本说明 |
 |------| ---------------- | ----------------- |----------- |
+|20240418| 0.5.0          | 0.2.2 | 修复chatglm3的bug, 修复save_pretrained时多文件的bug，增加CausalLMLoss, 修改deepspeed的传参逻辑，修改Text2Vec的bug, 完善openai client, 增加get_weight_decay_optim_groups|
 |20240317| 0.4.9.post2    | 0.2.1.post2 |增加get_weight_decay_optim_groups函数, attention中允许is_causal，修改repetition_penalty的bug，把baichuan从llama中剥离，修复config_path的bug，允许num_key_value_heads参数，[torch4keras-v0.2.1.post2](https://github.com/Tongjilibo/torch4keras/releases/tag/v0.2.1.post2)更新特性|
 |20240221| 0.4.8          | 0.2.0|fastapi发布服务允许闲时offload到cpu, `build_transformer_model`允许从hf下载, 添加`FillMask`的pipeline, 添加`SequenceClassificationTrainer`|
-|20240204| 0.4.7          | 0.1.9|修改`save_pretrained`用于保存文件夹, 增加GenerateSpeed用于统计token生成速度，修复t5在use_states=True时候的错误, 修改层次编码的bug, 增加deepseek_moe模型，修复generation并发错误，优化大模型耗时|
-|20240116| 0.4.6          | 0.1.8|bug修复，增加`save_pretrained`用于保存`transformer`格式的权重, 增加部分`embedding`模型|
 
 [更多版本](https://github.com/Tongjilibo/bert4torch/blob/master/docs/Update.md)
 
 ### 4.2 更新历史
 
 [更多历史](https://github.com/Tongjilibo/bert4torch/blob/master/docs/History.md)
```

### Comparing `bert4torch-0.4.9.post2/README.md` & `bert4torch-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,238 +1,252 @@
-![bert4torch](./docs/pics/bert4torch.png)
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
-[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
-[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
-
-[Documentation](https://bert4torch.readthedocs.io) |
-[Torch4keras](https://github.com/Tongjilibo/torch4keras) |
-[Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples) |
-[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
-
-## 目录
-- [目录](#目录)
-- [1. 下载安装](#1-下载安装)
-- [2. 功能](#2-功能)
-- [3. 快速上手](#3-快速上手)
-- [4. 版本和更新历史](#4-版本和更新历史)
-  - [4.1 版本历史](#41-版本历史)
-  - [4.2 更新历史](#42-更新历史)
-- [5. 预训练权重](#5-预训练权重)
-- [6. 鸣谢](#6-鸣谢)
-- [7. 引用](#7-引用)
-- [8. 其他](#8-其他)
-  
-
-## 1. 下载安装
-
-安装稳定版
-
-```shell
-pip install bert4torch
-```
-
-安装最新版
-
-```shell
-pip install git+https://github.com/Tongjilibo/bert4torch
-```
-
-- **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
-- **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
-- **自行训练**：针对自己的数据，修改相应的数据处理代码块
-- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
-
-## 2. 功能
-- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
-- **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
-- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
-- **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/DATA.md)
-- **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
-- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
-- **训练过程**：
-
-  ```text
-  2022-10-28 23:16:10 - Start Training
-  2022-10-28 23:16:10 - Epoch: 1/2
-  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-  test_acc: 0.98045. best_test_acc: 0.98045
-
-  2022-10-28 23:16:27 - Epoch: 2/2
-  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-  test_acc: 0.98280. best_test_acc: 0.98280
-
-  2022-10-28 23:16:44 - Finish Training
-  ```
-
-|          功能                | bert4torch |  transformers | 备注 |
-|-----------------------------|------------|----------------|--------|
-|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
-|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
-|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
-|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
-|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
-|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
-|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
-|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
-
-
-## 3. 快速上手
-
-- [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
-- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
-- [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
-
-## 4. 版本和更新历史
-### 4.1 版本历史
-|更新日期| bert4torch | torch4keras | 版本说明 |
-|------| ---------------- | ----------------- |----------- |
-|20240317| 0.4.9.post2    | 0.2.1.post2 |增加get_weight_decay_optim_groups函数, attention中允许is_causal，修改repetition_penalty的bug，把baichuan从llama中剥离，修复config_path的bug，允许num_key_value_heads参数，[torch4keras-v0.2.1.post2](https://github.com/Tongjilibo/torch4keras/releases/tag/v0.2.1.post2)更新特性|
-|20240221| 0.4.8          | 0.2.0|fastapi发布服务允许闲时offload到cpu, `build_transformer_model`允许从hf下载, 添加`FillMask`的pipeline, 添加`SequenceClassificationTrainer`|
-|20240204| 0.4.7          | 0.1.9|修改`save_pretrained`用于保存文件夹, 增加GenerateSpeed用于统计token生成速度，修复t5在use_states=True时候的错误, 修改层次编码的bug, 增加deepseek_moe模型，修复generation并发错误，优化大模型耗时|
-|20240116| 0.4.6          | 0.1.8|bug修复，增加`save_pretrained`用于保存`transformer`格式的权重, 增加部分`embedding`模型|
-
-[更多版本](https://github.com/Tongjilibo/bert4torch/blob/master/docs/Update.md)
-
-### 4.2 更新历史
-
-[更多历史](https://github.com/Tongjilibo/bert4torch/blob/master/docs/History.md)
-
-## 5. 预训练权重
-- 预训练模型支持多种代码加载方式
-```python
-from bert4torch.models import build_transformer_model
-
-# 1. 仅指定config_path: 从头初始化模型结构, 不加载预训练模型
-model = build_transformer_model('./model/bert4torch_config.json')
-
-# 2. 仅指定checkpoint_path: 
-## 2.1 文件夹路径: 自动寻找路径下的*.bin/*.safetensors权重文件 + bert4torch_config.json/config.json文件
-model = build_transformer_model(checkpoint_path='./model')
-
-## 2.2 文件路径/列表: 文件路径即权重路径/列表, config会从同级目录下寻找
-model = build_transformer_model(checkpoint_path='./pytorch_model.bin')
-
-## 2.3 model_name: hf上预训练权重名称, 会自动下载hf权重以及bert4torch_config.json文件
-model = build_transformer_model(checkpoint_path='bert-base-chinese')
-
-# 3. 同时指定config_path和checkpoint_path(本地路径名或model_name排列组合): 
-config_path = './model/bert4torch_config.json'  # 或'bert-base-chinese'
-checkpoint_path = './model/pytorch_model.bin'  # 或'bert-base-chinese'
-model = build_transformer_model(config_path, checkpoint_path)
-```
-
-| 模型分类| 模型名称 | 权重来源| 权重链接/checkpoint_path | config_path|
-| ----- | ----- | ----- | ----- | ----- |
-| bert| bert-base-chinese| google-bert | [`bert-base-chinese`](https://huggingface.co/bert-base-chinese) | [`bert-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-chinese)|
-|     | chinese_L-12_H-768_A-12| 谷歌 | [github](https://github.com/google-research/bert), [tf](https://storage.googleapis.com/bert_models/2018_11_03/chinese_L-12_H-768_A-12.zip), [`Tongjilibo/bert-chinese_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/bert-chinese_L-12_H-768_A-12) | |
-|     | chinese-bert-wwm-ext| HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-bert-wwm-ext`](https://huggingface.co/hfl/chinese-bert-wwm-ext)| [`chinese-bert-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-bert-wwm-ext) |
-|     | bert-base-multilingual-cased| google-bert | [`bert-base-multilingual-cased`](https://huggingface.co/bert-base-multilingual-cased) | [`bert-base-multilingual-cased`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-multilingual-cased) |
-|     | macbert | HFL| [github](https://github.com/ymcui/MacBERT)，[`hfl/chinese-macbert-base`](https://huggingface.co/hfl/chinese-macbert-base), [`hfl/chinese-macbert-large`](https://huggingface.co/hfl/chinese-macbert-large) |[`chinese-macbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-base), [`chinese-macbert-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-large)|
-|     | wobert| 追一科技| [github](https://github.com/ZhuiyiTechnology/WoBERT)，[`junnyu/wobert_chinese_base`](https://huggingface.co/junnyu/wobert_chinese_base)，[`junnyu/wobert_chinese_plus_base`](https://huggingface.co/junnyu/wobert_chinese_plus_base) |[`wobert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_base), [`wobert_chinese_plus_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_plus_base)|
-|roberta|chinese-roberta-wwm-ext | HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-roberta-wwm-ext`](https://huggingface.co/hfl/chinese-roberta-wwm-ext), [`hfl/chinese-roberta-wwm-ext-large`](https://huggingface.co/hfl/chinese-roberta-wwm-ext-large) |[`chinese-roberta-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext), [`chinese-roberta-wwm-ext-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext-large) |
-|     |roberta-small/tiny| 追一科技| [github](https://github.com/ZhuiyiTechnology/pretrained-models)，[`Tongjilibo/chinese_roberta_L-4_H-312_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-4_H-312_A-12), [`Tongjilibo/chinese_roberta_L-6_H-384_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-6_H-384_A-12) | |
-|     |roberta-base| FacebookAI | [`roberta-base`](https://huggingface.co/roberta-base) | [`roberta-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roberta-base) |
-|     | guwenbert| ethanyt |[`ethanyt/guwenbert-base`](https://huggingface.co/ethanyt/guwenbert-base) | [`guwenbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/guwenbert-base)|
-| albert|albert| brightmart| [github](https://github.com/brightmart/albert_zh)，[torch](https://github.com/lonePatient/albert_pytorch), [`voidful/albert_chinese_tiny`](https://huggingface.co/voidful/albert_chinese_tiny)，[`voidful/albert_chinese_small`](https://huggingface.co/voidful/albert_chinese_small), [`voidful/albert_chinese_base`](https://huggingface.co/voidful/albert_chinese_base), [`voidful/albert_chinese_large`](https://huggingface.co/voidful/albert_chinese_large), [`voidful/albert_chinese_xlarge`](https://huggingface.co/voidful/albert_chinese_xlarge), [`voidful/albert_chinese_xxlarge`](https://huggingface.co/voidful/albert_chinese_xxlarge) | [`albert_chinese_tiny`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_tiny)，[`albert_chinese_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_small), [`albert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_base), [`albert_chinese_large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_large), [`albert_chinese_xlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xlarge), [`albert_chinese_xxlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xxlarge)|
-| nezha|NEZHA | 华为| [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-PyTorch)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch), [`sijunhe/nezha-cn-base`](https://huggingface.co/sijunhe/nezha-cn-base), [`sijunhe/nezha-cn-large`](https://huggingface.co/sijunhe/nezha-cn-large), [`sijunhe/nezha-base-wwm`](https://huggingface.co/sijunhe/nezha-base-wwm), [`sijunhe/nezha-large-wwm`](https://huggingface.co/sijunhe/nezha-large-wwm)|[`nezha-cn-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-base), [`nezha-cn-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-large), [`nezha-base-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-base-wwm), [`nezha-large-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-large-wwm)|
-|      |nezha_gpt_dialog| bojone| [github](https://github.com/bojone/nezha_gpt_dialog), [`Tongjilibo/nezha_gpt_dialog`](https://huggingface.co/Tongjilibo/nezha_gpt_dialog) | |
-| xlnet|chinese-xlnet | HFL | [github](https://github.com/ymcui/Chinese-XLNet), [`hfl/chinese-xlnet-base`](https://huggingface.co/hfl/chinese-xlnet-base) | [`chinese-xlnet-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-xlnet-base)|
-||tranformer_xl|huggingface|[`transfo-xl/transfo-xl-wt103`](https://huggingface.co/transfo-xl/transfo-xl-wt103)|[`transfo-xl-wt103`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/transfo-xl-wt103)|
-|deberta| Erlangshen-DeBERTa-v2| IDEA | [`IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese) |[`Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-97M-Chinese), [`Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-320M-Chinese), [`Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-710M-Chinese) |
-| electra|Chinese-ELECTRA | HFL | [github](https://github.com/ymcui/Chinese-ELECTRA)，[`hfl/chinese-electra-base-discriminator`](https://huggingface.co/hfl/chinese-electra-base-discriminator) |[`chinese-electra-base-discriminator`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-electra-base-discriminator)|
-| ernie|ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[`nghuyong/ernie-1.0-base-zh`](https://huggingface.co/nghuyong/ernie-1.0-base-zh), [`nghuyong/ernie-3.0-base-zh`](https://huggingface.co/nghuyong/ernie-3.0-base-zh)| [`ernie-1.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-1.0-base-zh), [`ernie-3.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-3.0-base-zh)|
-| roformer|roformer| 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer)，[`junnyu/roformer_chinese_base`](https://huggingface.co/junnyu/roformer_chinese_base) |[`roformer_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_base) |
-|         |roformer_v2 | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-v2)，[`junnyu/roformer_v2_chinese_char_base`](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)|[`roformer_v2_chinese_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_v2_chinese_char_base) |
-| simbert|simbert | 追一科技| [github](https://github.com/ZhuiyiTechnology/simbert)，[`Tongjilibo/simbert-chinese-base`](https://huggingface.co/Tongjilibo/simbert-chinese-base), [`Tongjilibo/simbert-chinese-small`](https://huggingface.co/Tongjilibo/simbert-chinese-small), [`Tongjilibo/simbert-chinese-tiny`](https://huggingface.co/Tongjilibo/simbert-chinese-tiny) | |
-|        |simbert_v2/roformer-sim | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-sim)，[`junnyu/roformer_chinese_sim_char_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)，[`junnyu/roformer_chinese_sim_char_ft_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_base)，[`junnyu/roformer_chinese_sim_char_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_small)，[`junnyu/roformer_chinese_sim_char_ft_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_small)|[`roformer_chinese_sim_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_base), [`roformer_chinese_sim_char_ft_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_base), [`roformer_chinese_sim_char_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_small), [`roformer_chinese_sim_char_ft_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_small) |
-| gau|GAU-alpha | 追一科技| [github](https://github.com/ZhuiyiTechnology/GAU-alpha), [`Tongjilibo/chinese_GAU-alpha-char_L-24_H-768`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12) | |
-| uie| uie | 百度| [github](https://github.com/universal-ie/UIE), [torch](https://github.com/HUSTAI/uie_pytorch), [`Tongjilibo/uie-base`](https://huggingface.co/Tongjilibo/uie-base) | |
-| gpt |CDial-GPT| thu-coai| [github](https://github.com/thu-coai/CDial-GPT), [`thu-coai/CDial-GPT_LCCC-base`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base), [`thu-coai/CDial-GPT_LCCC-large`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [`CDial-GPT_LCCC-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-base), [`CDial-GPT_LCCC-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-large) |
-|     | cmp_lm(26亿)|清华 | [github](https://github.com/TsinghuaAI/CPM-1-Generate), [`TsinghuaAI/CPM-Generate`](https://huggingface.co/TsinghuaAI/CPM-Generate) | [`CPM-Generate`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CPM-Generate) |
-|     |nezha_gen|huawei_noah|[github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow), [`Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12)|
-|     | gpt2-chinese-cluecorpussmall|UER | [`uer/gpt2-chinese-cluecorpussmall`](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [`gpt2-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-chinese-cluecorpussmall)|
-|     | gpt2-ml|imcaspar | [tf](https://github.com/imcaspar/gpt2-ml), [torch](https://github.com/ghosthamlet/gpt2-ml-torch), [BaiduYun(84dh)](https://pan.baidu.com/s/16tL4Bmoh6jPy0cOND0YyeA) | [`gpt2-ml_15g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_15g_corpus), [`gpt2-ml_30g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_30g_corpus) |
-| bart| bart_base_chinese|复旦fnlp| [github](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [`fnlp/bart-base-chinese`](https://huggingface.co/fnlp/bart-base-chinese/tree/main)| [`bart-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese), [`bart-base-chinese-v1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese-v1.0) |
-| t5  | t5| UER | [`uer/t5-small-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall), [`uer/t5-base-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [`t5-base-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-base-chinese-cluecorpussmall), [`t5-small-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-small-chinese-cluecorpussmall)|
-|     | mt5 | 谷歌| [`google/mt5-base`](https://huggingface.co/google/mt5-base)| [`mt5-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/mt5-base)|
-|     | t5_pegasus| 追一科技| [github](https://github.com/ZhuiyiTechnology/t5-pegasus), [`Tongjilibo/chinese_t5_pegasus_small`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_small), [`Tongjilibo/chinese_t5_pegasus_base`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_base)| |
-|     | chatyuan v1&v2| clue-ai | [github](https://github.com/clue-ai/ChatYuan), [`ClueAI/ChatYuan-large-v1`](https://huggingface.co/ClueAI/ChatYuan-large-v1), [`ClueAI/ChatYuan-large-v2`](https://huggingface.co/ClueAI/ChatYuan-large-v2)| [`ChatYuan-large-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v1), [`ChatYuan-large-v2`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v2)|
-|     | PromptCLUE| clue-ai | [github](https://github.com/clue-ai/PromptCLUE), [`ClueAI/PromptCLUE-base`](https://huggingface.co/ClueAI/PromptCLUE-base) | [`PromptCLUE-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/PromptCLUE-base)|
-| chatglm   |chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [`THUDM/chatglm-6b`](https://huggingface.co/THUDM/chatglm-6b), [`THUDM/chatglm-6b-int8`](https://huggingface.co/THUDM/chatglm-6b-int8), [`THUDM/chatglm-6b-int4`](https://huggingface.co/THUDM/chatglm-6b-int4), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0) | [`chatglm-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b), [`chatglm-6b-int8`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int8), [`chatglm-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int4), [`chatglm-6b-v0.1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-v0.1.0) |
-|       |chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [`THUDM/chatglm2-6b`](https://huggingface.co/THUDM/chatglm2-6b), [`THUDM/chatglm2-6b-int4`](https://huggingface.co/THUDM/chatglm2-6b-int4), [`THUDM/chatglm2-6b-32k`](https://huggingface.co/THUDM/chatglm2-6b-32k) | [`chatglm2-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b), [`chatglm2-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-int4), [`chatglm2-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-32k) |
-|       |chatglm3-6b | THUDM | [github](https://github.com/THUDM/ChatGLM3), [`THUDM/chatglm3-6b`](https://huggingface.co/THUDM/chatglm3-6b), [`THUDM/chatglm3-6b-32k`](https://huggingface.co/THUDM/chatglm3-6b-32k) | [`chatglm3-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b), [`chatglm3-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b-32k) |
-| llama | llama | meta| [github](https://github.com/facebookresearch/llama) | [`llama-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-7b), [`llama-13b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-13b)|
-|       | llama-2 | meta| [github](https://github.com/facebookresearch/llama), [meta-llama/Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf), [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [meta-llama/Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf), [meta-llama/Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [`Llama-2-7b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-hf), [`Llama-2-7b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-chat-hf), [`Llama-2-13b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-hf), [`Llama-2-13b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-chat-hf)|
-|       | chinese_llama_alpaca|HFL|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[`chinese_alpaca_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_alpaca_plus_7b), [`chinese_llama_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_llama_plus_7b)|
-|       | Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [BelleGroup/BELLE-LLaMA-7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[`BELLE-LLaMA-7B-2M-enc`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/BELLE-LLaMA-7B-2M-enc)|
-|       | Ziya | IDEA-CCNL | [IDEA-CCNL/Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [IDEA-CCNL/Ziya-LLaMA-13B-v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [`Ziya-LLaMA-13B-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1), [`Ziya-LLaMA-13B-v1.1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1.1) |
-|       | Baichuan | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan), [`baichuan-inc/Baichuan-7B`](https://huggingface.co/baichuan-inc/Baichuan-7B), [`baichuan-inc/Baichuan-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [`baichuan-inc/Baichuan-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [`Baichuan-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-7B), [`Baichuan-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Base), [`Baichuan-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Chat) |
-|       | Baichuan2 | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan2), [`baichuan-inc/Baichuan2-7B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base), [`baichuan-inc/Baichuan2-7B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Chat), [`baichuan-inc/Baichuan2-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Base), [`baichuan-inc/Baichuan2-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Chat) | [`Baichuan2-7B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Base), [`Baichuan2-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Chat), [`Baichuan2-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Base), [`Baichuan2-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Chat) |
-|       | vicuna | lmsys| [`lmsys/vicuna-7b-v1.5`](https://huggingface.co/lmsys/vicuna-7b-v1.5) | [`vicuna-7b-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/vicuna-7b-v1.5)|
-|       | Yi | 01-ai| [github](https://github.com/01-ai/Yi), [`01-ai/Yi-6B`](https://huggingface.co/01-ai/Yi-6B), [`01-ai/Yi-6B-200K`](https://huggingface.co/01-ai/Yi-6B-200K) | [`Yi-6B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B), [`Yi-6B-200K`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B-200K)|
-| bloom |bloom | bigscience | [`bigscience/bloom-560m`](https://huggingface.co/bigscience/bloom-560m), [`bigscience/bloomz-560m`](https://huggingface.co/bigscience/bloomz-560m) | [`bloom-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloom-560m), [`bloomz-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloomz-560m) |
-| Qwen  |Qwen | 阿里云 | [github](https://github.com/QwenLM/Qwen-7B), [`Qwen/Qwen-1_8B`](https://huggingface.co/Qwen/Qwen-1_8B), [`Qwen/Qwen-1_8B-Chat`](https://huggingface.co/Qwen/Qwen-1_8B-Chat), [`Qwen/Qwen-7B`](https://huggingface.co/Qwen/Qwen-7B), [`Qwen/Qwen-7B-Chat`](https://huggingface.co/Qwen/Qwen-7B-Chat) | [`Qwen-1_8B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B), [`Qwen-1_8B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B-Chat), [`Qwen-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B), [`Qwen-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B-Chat) |
-| InternLM|InternLM | 上海人工智能实验室 | [github](https://github.com/InternLM/InternLM), [`internlm/internlm-chat-7b`](https://huggingface.co/internlm/internlm-chat-7b), [`internlm/internlm-7b`](https://huggingface.co/internlm/internlm-7b) | [`internlm-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-7b), [`internlm-chat-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-chat-7b)|
-| Falcon|Falcon | tiiuae | [hf](https://huggingface.co/tiiuae), [`tiiuae/falcon-rw-1b`](https://huggingface.co/tiiuae/falcon-rw-1b), [`tiiuae/falcon-7b`](https://huggingface.co/tiiuae/falcon-7b), [`tiiuae/falcon-7b-instruct`](https://huggingface.co/tiiuae/falcon-7b-instruct) | [`falcon-rw-1b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-rw-1b), [`falcon-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b), [`falcon-7b-instruct`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b-instruct) |
-|  moe  |deeoseek-moe|deepseek| [github](https://github.com/deepseek-ai/DeepSeek-MoE), [`deepseek-ai/deepseek-moe-16b-base`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-base), [`deepseek-ai/deepseek-moe-16b-chat`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-chat) | [`deepseek-moe-16b-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-base), [`deepseek-moe-16b-chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-chat) |
-| embedding| text2vec-base-chinese |shibing624| [`shibing624/text2vec-base-chinese`](https://huggingface.co/shibing624/text2vec-base-chinese) |[`text2vec-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/text2vec-base-chinese) |
-|          | m3e |moka-ai| [`moka-ai/m3e-base`](https://huggingface.co/moka-ai/m3e-base) |[`m3e-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/m3e-base)|
-|          | bge |BAAI| [`BAAI/bge-large-en-v1.5`](https://huggingface.co/BAAI/bge-large-en-v1.5), [`BAAI/bge-large-zh-v1.5`](https://huggingface.co/BAAI/bge-large-zh-v1.5) | [`bge-large-en-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-en-v1.5), [`bge-large-zh-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-zh-v1.5)|
-|          | gte |thenlper| [`thenlper/gte-large-zh`](https://huggingface.co/thenlper/gte-large-zh), [`thenlper/gte-base-zh`](https://huggingface.co/thenlper/gte-base-zh) |[`gte-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-base-zh), [`gte-large-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-large-zh)|
-
-*注：
-1. `高亮格式`(如`bert-base-chinese`)的表示可直接`build_transformer_model()`联网下载
-2. 国内镜像网站加速下载
-   - `HF_ENDPOINT=https://hf-mirror.com python your_script.py`
-   - `export HF_ENDPOINT=https://hf-mirror.com`后再执行python代码
-   - 在python代码开头如下设置
-    ```python
-    import os
-    os.environ['HF_ENDPOINT'] = "https://hf-mirror.com"
-    ```
-
-## 6. 鸣谢
-
-- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
-- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
-
-## 7. 引用
-
-```
-@misc{bert4torch,
-  title={bert4torch},
-  author={Bo Li},
-  year={2022},
-  howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
-}
-```
-
-## 8. 其他
-
-- Wechat & Star History Chart
-
-<table border="0">
-  <tbody>
-    <tr align="center" >
-      <td>
-         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信号</a> 
-      </td>
-      <td>
-         <a href="https://github.com/Tongjilibo"><img width="190" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信群</a> 
-      </td>
-      <td>
-         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
-         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
-      </td>    
-      </tr>
-  </tbody>
-</table>
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.5.0
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: torch>1.6
+Requires-Dist: torch4keras==0.2.2
+Requires-Dist: six
+
+![bert4torch](./docs/pics/bert4torch.png)
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
+[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
+[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
+
+[Documentation](https://bert4torch.readthedocs.io) |
+[Torch4keras](https://github.com/Tongjilibo/torch4keras) |
+[Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples) |
+[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
+
+## 目录
+- [目录](#目录)
+- [1. 下载安装](#1-下载安装)
+- [2. 功能](#2-功能)
+- [3. 快速上手](#3-快速上手)
+- [4. 版本和更新历史](#4-版本和更新历史)
+  - [4.1 版本历史](#41-版本历史)
+  - [4.2 更新历史](#42-更新历史)
+- [5. 预训练权重](#5-预训练权重)
+- [6. 鸣谢](#6-鸣谢)
+- [7. 引用](#7-引用)
+- [8. 其他](#8-其他)
+  
+
+## 1. 下载安装
+
+安装稳定版
+
+```shell
+pip install bert4torch
+```
+
+安装最新版
+
+```shell
+pip install git+https://github.com/Tongjilibo/bert4torch
+```
+
+- **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
+- **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
+- **自行训练**：针对自己的数据，修改相应的数据处理代码块
+- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
+
+## 2. 功能
+- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
+- **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
+- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
+- **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/DATA.md)
+- **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
+- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
+- **训练过程**：
+
+  ```text
+  2022-10-28 23:16:10 - Start Training
+  2022-10-28 23:16:10 - Epoch: 1/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+  test_acc: 0.98045. best_test_acc: 0.98045
+
+  2022-10-28 23:16:27 - Epoch: 2/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+  test_acc: 0.98280. best_test_acc: 0.98280
+
+  2022-10-28 23:16:44 - Finish Training
+  ```
+
+|          功能                | bert4torch |  transformers | 备注 |
+|-----------------------------|------------|----------------|--------|
+|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
+|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
+|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
+|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
+|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
+|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
+|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
+|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
+
+
+## 3. 快速上手
+
+- [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
+- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
+- [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
+
+## 4. 版本和更新历史
+### 4.1 版本历史
+|更新日期| bert4torch | torch4keras | 版本说明 |
+|------| ---------------- | ----------------- |----------- |
+|20240418| 0.5.0          | 0.2.2 | 修复chatglm3的bug, 修复save_pretrained时多文件的bug，增加CausalLMLoss, 修改deepspeed的传参逻辑，修改Text2Vec的bug, 完善openai client, 增加get_weight_decay_optim_groups|
+|20240317| 0.4.9.post2    | 0.2.1.post2 |增加get_weight_decay_optim_groups函数, attention中允许is_causal，修改repetition_penalty的bug，把baichuan从llama中剥离，修复config_path的bug，允许num_key_value_heads参数，[torch4keras-v0.2.1.post2](https://github.com/Tongjilibo/torch4keras/releases/tag/v0.2.1.post2)更新特性|
+|20240221| 0.4.8          | 0.2.0|fastapi发布服务允许闲时offload到cpu, `build_transformer_model`允许从hf下载, 添加`FillMask`的pipeline, 添加`SequenceClassificationTrainer`|
+
+[更多版本](https://github.com/Tongjilibo/bert4torch/blob/master/docs/Update.md)
+
+### 4.2 更新历史
+
+[更多历史](https://github.com/Tongjilibo/bert4torch/blob/master/docs/History.md)
+
+## 5. 预训练权重
+- 预训练模型支持多种代码加载方式
+```python
+from bert4torch.models import build_transformer_model
+
+# 1. 仅指定config_path: 从头初始化模型结构, 不加载预训练模型
+model = build_transformer_model('./model/bert4torch_config.json')
+
+# 2. 仅指定checkpoint_path: 
+## 2.1 文件夹路径: 自动寻找路径下的*.bin/*.safetensors权重文件 + bert4torch_config.json/config.json文件
+model = build_transformer_model(checkpoint_path='./model')
+
+## 2.2 文件路径/列表: 文件路径即权重路径/列表, config会从同级目录下寻找
+model = build_transformer_model(checkpoint_path='./pytorch_model.bin')
+
+## 2.3 model_name: hf上预训练权重名称, 会自动下载hf权重以及bert4torch_config.json文件
+model = build_transformer_model(checkpoint_path='bert-base-chinese')
+
+# 3. 同时指定config_path和checkpoint_path(本地路径名或model_name排列组合): 
+config_path = './model/bert4torch_config.json'  # 或'bert-base-chinese'
+checkpoint_path = './model/pytorch_model.bin'  # 或'bert-base-chinese'
+model = build_transformer_model(config_path, checkpoint_path)
+```
+
+| 模型分类| 模型名称 | 权重来源| 权重链接/checkpoint_path | config_path|
+| ----- | ----- | ----- | ----- | ----- |
+| bert| bert-base-chinese| google-bert | [`bert-base-chinese`](https://huggingface.co/bert-base-chinese) | [`bert-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-chinese)|
+|     | chinese_L-12_H-768_A-12| 谷歌 | [github](https://github.com/google-research/bert), [tf](https://storage.googleapis.com/bert_models/2018_11_03/chinese_L-12_H-768_A-12.zip), [`Tongjilibo/bert-chinese_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/bert-chinese_L-12_H-768_A-12) | |
+|     | chinese-bert-wwm-ext| HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-bert-wwm-ext`](https://huggingface.co/hfl/chinese-bert-wwm-ext)| [`chinese-bert-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-bert-wwm-ext) |
+|     | bert-base-multilingual-cased| google-bert | [`bert-base-multilingual-cased`](https://huggingface.co/bert-base-multilingual-cased) | [`bert-base-multilingual-cased`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-multilingual-cased) |
+|     | macbert | HFL| [github](https://github.com/ymcui/MacBERT)，[`hfl/chinese-macbert-base`](https://huggingface.co/hfl/chinese-macbert-base), [`hfl/chinese-macbert-large`](https://huggingface.co/hfl/chinese-macbert-large) |[`chinese-macbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-base), [`chinese-macbert-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-large)|
+|     | wobert| 追一科技| [github](https://github.com/ZhuiyiTechnology/WoBERT)，[`junnyu/wobert_chinese_base`](https://huggingface.co/junnyu/wobert_chinese_base)，[`junnyu/wobert_chinese_plus_base`](https://huggingface.co/junnyu/wobert_chinese_plus_base) |[`wobert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_base), [`wobert_chinese_plus_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_plus_base)|
+|roberta|chinese-roberta-wwm-ext | HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-roberta-wwm-ext`](https://huggingface.co/hfl/chinese-roberta-wwm-ext), [`hfl/chinese-roberta-wwm-ext-large`](https://huggingface.co/hfl/chinese-roberta-wwm-ext-large) |[`chinese-roberta-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext), [`chinese-roberta-wwm-ext-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext-large) |
+|     |roberta-small/tiny| 追一科技| [github](https://github.com/ZhuiyiTechnology/pretrained-models)，[`Tongjilibo/chinese_roberta_L-4_H-312_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-4_H-312_A-12), [`Tongjilibo/chinese_roberta_L-6_H-384_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-6_H-384_A-12) | |
+|     |roberta-base| FacebookAI | [`roberta-base`](https://huggingface.co/roberta-base) | [`roberta-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roberta-base) |
+|     | guwenbert| ethanyt |[`ethanyt/guwenbert-base`](https://huggingface.co/ethanyt/guwenbert-base) | [`guwenbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/guwenbert-base)|
+| albert|albert| brightmart| [github](https://github.com/brightmart/albert_zh)，[torch](https://github.com/lonePatient/albert_pytorch), [`voidful/albert_chinese_tiny`](https://huggingface.co/voidful/albert_chinese_tiny)，[`voidful/albert_chinese_small`](https://huggingface.co/voidful/albert_chinese_small), [`voidful/albert_chinese_base`](https://huggingface.co/voidful/albert_chinese_base), [`voidful/albert_chinese_large`](https://huggingface.co/voidful/albert_chinese_large), [`voidful/albert_chinese_xlarge`](https://huggingface.co/voidful/albert_chinese_xlarge), [`voidful/albert_chinese_xxlarge`](https://huggingface.co/voidful/albert_chinese_xxlarge) | [`albert_chinese_tiny`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_tiny)，[`albert_chinese_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_small), [`albert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_base), [`albert_chinese_large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_large), [`albert_chinese_xlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xlarge), [`albert_chinese_xxlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xxlarge)|
+| nezha|NEZHA | 华为| [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-PyTorch)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch), [`sijunhe/nezha-cn-base`](https://huggingface.co/sijunhe/nezha-cn-base), [`sijunhe/nezha-cn-large`](https://huggingface.co/sijunhe/nezha-cn-large), [`sijunhe/nezha-base-wwm`](https://huggingface.co/sijunhe/nezha-base-wwm), [`sijunhe/nezha-large-wwm`](https://huggingface.co/sijunhe/nezha-large-wwm)|[`nezha-cn-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-base), [`nezha-cn-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-large), [`nezha-base-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-base-wwm), [`nezha-large-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-large-wwm)|
+|      |nezha_gpt_dialog| bojone| [github](https://github.com/bojone/nezha_gpt_dialog), [`Tongjilibo/nezha_gpt_dialog`](https://huggingface.co/Tongjilibo/nezha_gpt_dialog) | |
+| xlnet|chinese-xlnet | HFL | [github](https://github.com/ymcui/Chinese-XLNet), [`hfl/chinese-xlnet-base`](https://huggingface.co/hfl/chinese-xlnet-base) | [`chinese-xlnet-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-xlnet-base)|
+||tranformer_xl|huggingface|[`transfo-xl/transfo-xl-wt103`](https://huggingface.co/transfo-xl/transfo-xl-wt103)|[`transfo-xl-wt103`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/transfo-xl-wt103)|
+|deberta| Erlangshen-DeBERTa-v2| IDEA | [`IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese) |[`Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-97M-Chinese), [`Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-320M-Chinese), [`Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-710M-Chinese) |
+| electra|Chinese-ELECTRA | HFL | [github](https://github.com/ymcui/Chinese-ELECTRA)，[`hfl/chinese-electra-base-discriminator`](https://huggingface.co/hfl/chinese-electra-base-discriminator) |[`chinese-electra-base-discriminator`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-electra-base-discriminator)|
+| ernie|ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[`nghuyong/ernie-1.0-base-zh`](https://huggingface.co/nghuyong/ernie-1.0-base-zh), [`nghuyong/ernie-3.0-base-zh`](https://huggingface.co/nghuyong/ernie-3.0-base-zh)| [`ernie-1.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-1.0-base-zh), [`ernie-3.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-3.0-base-zh)|
+| roformer|roformer| 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer)，[`junnyu/roformer_chinese_base`](https://huggingface.co/junnyu/roformer_chinese_base) |[`roformer_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_base) |
+|         |roformer_v2 | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-v2)，[`junnyu/roformer_v2_chinese_char_base`](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)|[`roformer_v2_chinese_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_v2_chinese_char_base) |
+| simbert|simbert | 追一科技| [github](https://github.com/ZhuiyiTechnology/simbert)，[`Tongjilibo/simbert-chinese-base`](https://huggingface.co/Tongjilibo/simbert-chinese-base), [`Tongjilibo/simbert-chinese-small`](https://huggingface.co/Tongjilibo/simbert-chinese-small), [`Tongjilibo/simbert-chinese-tiny`](https://huggingface.co/Tongjilibo/simbert-chinese-tiny) | |
+|        |simbert_v2/roformer-sim | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-sim)，[`junnyu/roformer_chinese_sim_char_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)，[`junnyu/roformer_chinese_sim_char_ft_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_base)，[`junnyu/roformer_chinese_sim_char_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_small)，[`junnyu/roformer_chinese_sim_char_ft_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_small)|[`roformer_chinese_sim_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_base), [`roformer_chinese_sim_char_ft_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_base), [`roformer_chinese_sim_char_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_small), [`roformer_chinese_sim_char_ft_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_small) |
+| gau|GAU-alpha | 追一科技| [github](https://github.com/ZhuiyiTechnology/GAU-alpha), [`Tongjilibo/chinese_GAU-alpha-char_L-24_H-768`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12) | |
+| uie| uie | 百度| [github](https://github.com/universal-ie/UIE), [torch](https://github.com/HUSTAI/uie_pytorch), [`Tongjilibo/uie-base`](https://huggingface.co/Tongjilibo/uie-base) | |
+| gpt |CDial-GPT| thu-coai| [github](https://github.com/thu-coai/CDial-GPT), [`thu-coai/CDial-GPT_LCCC-base`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base), [`thu-coai/CDial-GPT_LCCC-large`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [`CDial-GPT_LCCC-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-base), [`CDial-GPT_LCCC-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-large) |
+|     | cmp_lm(26亿)|清华 | [github](https://github.com/TsinghuaAI/CPM-1-Generate), [`TsinghuaAI/CPM-Generate`](https://huggingface.co/TsinghuaAI/CPM-Generate) | [`CPM-Generate`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CPM-Generate) |
+|     |nezha_gen|huawei_noah|[github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow), [`Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12)|
+|     | gpt2-chinese-cluecorpussmall|UER | [`uer/gpt2-chinese-cluecorpussmall`](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [`gpt2-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-chinese-cluecorpussmall)|
+|     | gpt2-ml|imcaspar | [tf](https://github.com/imcaspar/gpt2-ml), [torch](https://github.com/ghosthamlet/gpt2-ml-torch), [BaiduYun(84dh)](https://pan.baidu.com/s/16tL4Bmoh6jPy0cOND0YyeA) | [`gpt2-ml_15g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_15g_corpus), [`gpt2-ml_30g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_30g_corpus) |
+| bart| bart_base_chinese|复旦fnlp| [github](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [`fnlp/bart-base-chinese`](https://huggingface.co/fnlp/bart-base-chinese/tree/main)| [`bart-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese), [`bart-base-chinese-v1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese-v1.0) |
+| t5  | t5| UER | [`uer/t5-small-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall), [`uer/t5-base-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [`t5-base-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-base-chinese-cluecorpussmall), [`t5-small-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-small-chinese-cluecorpussmall)|
+|     | mt5 | 谷歌| [`google/mt5-base`](https://huggingface.co/google/mt5-base)| [`mt5-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/mt5-base)|
+|     | t5_pegasus| 追一科技| [github](https://github.com/ZhuiyiTechnology/t5-pegasus), [`Tongjilibo/chinese_t5_pegasus_small`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_small), [`Tongjilibo/chinese_t5_pegasus_base`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_base)| |
+|     | chatyuan v1&v2| clue-ai | [github](https://github.com/clue-ai/ChatYuan), [`ClueAI/ChatYuan-large-v1`](https://huggingface.co/ClueAI/ChatYuan-large-v1), [`ClueAI/ChatYuan-large-v2`](https://huggingface.co/ClueAI/ChatYuan-large-v2)| [`ChatYuan-large-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v1), [`ChatYuan-large-v2`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v2)|
+|     | PromptCLUE| clue-ai | [github](https://github.com/clue-ai/PromptCLUE), [`ClueAI/PromptCLUE-base`](https://huggingface.co/ClueAI/PromptCLUE-base) | [`PromptCLUE-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/PromptCLUE-base)|
+| chatglm   |chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [`THUDM/chatglm-6b`](https://huggingface.co/THUDM/chatglm-6b), [`THUDM/chatglm-6b-int8`](https://huggingface.co/THUDM/chatglm-6b-int8), [`THUDM/chatglm-6b-int4`](https://huggingface.co/THUDM/chatglm-6b-int4), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0) | [`chatglm-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b), [`chatglm-6b-int8`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int8), [`chatglm-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int4), [`chatglm-6b-v0.1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-v0.1.0) |
+|       |chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [`THUDM/chatglm2-6b`](https://huggingface.co/THUDM/chatglm2-6b), [`THUDM/chatglm2-6b-int4`](https://huggingface.co/THUDM/chatglm2-6b-int4), [`THUDM/chatglm2-6b-32k`](https://huggingface.co/THUDM/chatglm2-6b-32k) | [`chatglm2-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b), [`chatglm2-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-int4), [`chatglm2-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-32k) |
+|       |chatglm3-6b | THUDM | [github](https://github.com/THUDM/ChatGLM3), [`THUDM/chatglm3-6b`](https://huggingface.co/THUDM/chatglm3-6b), [`THUDM/chatglm3-6b-32k`](https://huggingface.co/THUDM/chatglm3-6b-32k) | [`chatglm3-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b), [`chatglm3-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b-32k) |
+| llama | llama | meta| [github](https://github.com/facebookresearch/llama) | [`llama-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-7b), [`llama-13b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-13b)|
+|       | llama-2 | meta| [github](https://github.com/facebookresearch/llama), [meta-llama/Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf), [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [meta-llama/Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf), [meta-llama/Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [`Llama-2-7b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-hf), [`Llama-2-7b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-chat-hf), [`Llama-2-13b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-hf), [`Llama-2-13b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-chat-hf)|
+|       | chinese_llama_alpaca|HFL|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[`chinese_alpaca_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_alpaca_plus_7b), [`chinese_llama_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_llama_plus_7b)|
+|       | Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [BelleGroup/BELLE-LLaMA-7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[`BELLE-LLaMA-7B-2M-enc`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/BELLE-LLaMA-7B-2M-enc)|
+|       | Ziya | IDEA-CCNL | [IDEA-CCNL/Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [IDEA-CCNL/Ziya-LLaMA-13B-v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [`Ziya-LLaMA-13B-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1), [`Ziya-LLaMA-13B-v1.1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1.1) |
+|       | Baichuan | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan), [`baichuan-inc/Baichuan-7B`](https://huggingface.co/baichuan-inc/Baichuan-7B), [`baichuan-inc/Baichuan-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [`baichuan-inc/Baichuan-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [`Baichuan-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-7B), [`Baichuan-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Base), [`Baichuan-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Chat) |
+|       | Baichuan2 | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan2), [`baichuan-inc/Baichuan2-7B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base), [`baichuan-inc/Baichuan2-7B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Chat), [`baichuan-inc/Baichuan2-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Base), [`baichuan-inc/Baichuan2-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Chat) | [`Baichuan2-7B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Base), [`Baichuan2-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Chat), [`Baichuan2-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Base), [`Baichuan2-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Chat) |
+|       | vicuna | lmsys| [`lmsys/vicuna-7b-v1.5`](https://huggingface.co/lmsys/vicuna-7b-v1.5) | [`vicuna-7b-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/vicuna-7b-v1.5)|
+|       | Yi | 01-ai| [github](https://github.com/01-ai/Yi), [`01-ai/Yi-6B`](https://huggingface.co/01-ai/Yi-6B), [`01-ai/Yi-6B-200K`](https://huggingface.co/01-ai/Yi-6B-200K) | [`Yi-6B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B), [`Yi-6B-200K`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B-200K)|
+| bloom |bloom | bigscience | [`bigscience/bloom-560m`](https://huggingface.co/bigscience/bloom-560m), [`bigscience/bloomz-560m`](https://huggingface.co/bigscience/bloomz-560m) | [`bloom-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloom-560m), [`bloomz-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloomz-560m) |
+| Qwen  |Qwen | 阿里云 | [github](https://github.com/QwenLM/Qwen-7B), [`Qwen/Qwen-1_8B`](https://huggingface.co/Qwen/Qwen-1_8B), [`Qwen/Qwen-1_8B-Chat`](https://huggingface.co/Qwen/Qwen-1_8B-Chat), [`Qwen/Qwen-7B`](https://huggingface.co/Qwen/Qwen-7B), [`Qwen/Qwen-7B-Chat`](https://huggingface.co/Qwen/Qwen-7B-Chat) | [`Qwen-1_8B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B), [`Qwen-1_8B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B-Chat), [`Qwen-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B), [`Qwen-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B-Chat) |
+| InternLM|InternLM | 上海人工智能实验室 | [github](https://github.com/InternLM/InternLM), [`internlm/internlm-chat-7b`](https://huggingface.co/internlm/internlm-chat-7b), [`internlm/internlm-7b`](https://huggingface.co/internlm/internlm-7b) | [`internlm-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-7b), [`internlm-chat-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-chat-7b)|
+| Falcon|Falcon | tiiuae | [hf](https://huggingface.co/tiiuae), [`tiiuae/falcon-rw-1b`](https://huggingface.co/tiiuae/falcon-rw-1b), [`tiiuae/falcon-7b`](https://huggingface.co/tiiuae/falcon-7b), [`tiiuae/falcon-7b-instruct`](https://huggingface.co/tiiuae/falcon-7b-instruct) | [`falcon-rw-1b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-rw-1b), [`falcon-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b), [`falcon-7b-instruct`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b-instruct) |
+|  moe  |deeoseek-moe|deepseek| [github](https://github.com/deepseek-ai/DeepSeek-MoE), [`deepseek-ai/deepseek-moe-16b-base`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-base), [`deepseek-ai/deepseek-moe-16b-chat`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-chat) | [`deepseek-moe-16b-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-base), [`deepseek-moe-16b-chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-chat) |
+| embedding| text2vec-base-chinese |shibing624| [`shibing624/text2vec-base-chinese`](https://huggingface.co/shibing624/text2vec-base-chinese) |[`text2vec-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/text2vec-base-chinese) |
+|          | m3e |moka-ai| [`moka-ai/m3e-base`](https://huggingface.co/moka-ai/m3e-base) |[`m3e-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/m3e-base)|
+|          | bge |BAAI| [`BAAI/bge-large-en-v1.5`](https://huggingface.co/BAAI/bge-large-en-v1.5), [`BAAI/bge-large-zh-v1.5`](https://huggingface.co/BAAI/bge-large-zh-v1.5) | [`bge-large-en-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-en-v1.5), [`bge-large-zh-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-zh-v1.5)|
+|          | gte |thenlper| [`thenlper/gte-large-zh`](https://huggingface.co/thenlper/gte-large-zh), [`thenlper/gte-base-zh`](https://huggingface.co/thenlper/gte-base-zh) |[`gte-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-base-zh), [`gte-large-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-large-zh)|
+
+*注：
+1. `高亮格式`(如`bert-base-chinese`)的表示可直接`build_transformer_model()`联网下载
+2. 国内镜像网站加速下载
+   - `HF_ENDPOINT=https://hf-mirror.com python your_script.py`
+   - `export HF_ENDPOINT=https://hf-mirror.com`后再执行python代码
+   - 在python代码开头如下设置
+    ```python
+    import os
+    os.environ['HF_ENDPOINT'] = "https://hf-mirror.com"
+    ```
+
+## 6. 鸣谢
+
+- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
+- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
+
+## 7. 引用
+
+```
+@misc{bert4torch,
+  title={bert4torch},
+  author={Bo Li},
+  year={2022},
+  howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
+}
+```
+
+## 8. 其他
+
+- Wechat & Star History Chart
+
+<table border="0">
+  <tbody>
+    <tr align="center" >
+      <td>
+         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信号</a> 
+      </td>
+      <td>
+         <a href="https://github.com/Tongjilibo"><img width="190" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信群</a> 
+      </td>
+      <td>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
+      </td>    
+      </tr>
+  </tbody>
+</table>
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/activations.py` & `bert4torch-0.5.0/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/callbacks.py` & `bert4torch-0.5.0/bert4torch/callbacks.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/generation.py` & `bert4torch-0.5.0/bert4torch/generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,16 +716,16 @@
             # 由于batch是padding过的，因此要找到padding前的位置
             last_token_index = self.input_seqlen + output_ids.shape[1] - 1
             return torch.stack([logit[index_, :] for index_, logit in zip(last_token_index, logits)])
 
     @AutoRegressiveDecoder.wraps()
     def predict(self, inputs:Union[tuple,list], output_ids:torch.Tensor, states:Optional[dict]):
         '''
-        :params inputs: 原始输入，在整个预测过程中均不改变
-        :params outputs_ids: 输出的ids，随着预测进行，逐步增长
+        :param inputs: 原始输入，在整个预测过程中均不改变
+        :param outputs_ids: 输出的ids，随着预测进行，逐步增长
         '''
         if states is not None:
             assert self.use_states is True, 'Args `use_states` must be True when return states is not None'
         
         # 使用cache, 输入只能padding在左侧
         if self.use_states:
             if states is None:
@@ -875,17 +875,17 @@
             output_ids = self.random_sample(inputs, states=states)  # 基于随机采样
         elif self.mode == 'beam_search':
             output_ids = self.beam_search(inputs, states=states)  # 基于beam search
         return output_ids
 
     @model_inference_mode()
     @EmptyCacheDecorators.empty_cuda_cache()
-    def generate(self, text:Union[str, list], **kwargs):
+    def generate(self, text:Union[str, list, torch.Tensor], **kwargs):
         '''单条样本生成 / batch生成'''
-        if isinstance(text, str):
+        if isinstance(text, (str, torch.Tensor)):
             # 单条样本
             self.use_batch = False
         elif isinstance(text, list):
             # batch生成
             self.use_batch = True
             if 'generation_config' in kwargs:
                 kwargs['generation_config']['n'] = 1
@@ -899,15 +899,15 @@
         self.set_generation_config(kwargs)
         inputs = self.pre_process(text)
         output_ids = self._generate(inputs, states=kwargs.get('states'))
         return self.post_process(output_ids)
 
     @model_inference_mode()
     @EmptyCacheDecorators.empty_cuda_cache()
-    def stream_generate(self, text:str, **kwargs):
+    def stream_generate(self, text:Union[str, torch.Tensor], **kwargs):
         '''单条样本stream输出预测的结果'''
         self.set_generation_config(kwargs)
         self.use_batch = False
         inputs = self.pre_process(text)
         if self.mode == 'random_sample':
             for outputs in self.stream_random_sample(inputs, states=kwargs.get('states')):  # stream随机采样
                 yield self.post_process(outputs)
@@ -932,17 +932,17 @@
             inputs = [decoder_inputs] + encoder_outputs
         # inputs中包含了[decoder_ids, encoder_hidden_state, encoder_attention_mask]
         self.input_seqlen = torch.zeros(decoder_inputs.shape[0], dtype=torch.long).to(self.device)
         return inputs
 
     @model_inference_mode()
     @EmptyCacheDecorators.empty_cuda_cache()
-    def generate(self, text:Union[str, list], **kwargs):
+    def generate(self, text:Union[str, list, torch.Tensor], **kwargs):
         '''单条样本生成 / batch生成'''
-        if isinstance(text, str):
+        if isinstance(text, (str, torch.Tensor)):
             # 单条样本
             self.use_batch = False
         elif isinstance(text, list):
             # batch生成
             self.use_batch = True
             if 'generation_config' in kwargs:
                 kwargs['generation_config']['n'] = 1
@@ -954,15 +954,15 @@
         inputs = self._trans2tensors(inputs)
         encoder_output = self.encoder.predict(inputs)
         output = super()._generate(encoder_output, states=kwargs.get('states'))
         return self.post_process(output)
 
     @model_inference_mode()
     @EmptyCacheDecorators.empty_cuda_cache()
-    def stream_generate(self, text:str, **kwargs):
+    def stream_generate(self, text:Union[str, torch.Tensor], **kwargs):
         '''stream输出t时刻预测的结果'''
         self.set_generation_config(kwargs)
 
         self.use_batch = False
         inputs = self.pre_process(text)
         inputs = self._trans2tensors(inputs)
         encoder_output = self.encoder.predict(inputs)
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/attention.py` & `bert4torch-0.5.0/bert4torch/layers/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import torch
 import math
 import numpy as np
 import torch.nn.functional as F
 from bert4torch.layers.position_encoding import *
 from bert4torch.activations import get_activation
 from bert4torch.snippets import log_warn_once, is_flash_attn_available, is_xformers_available
+from typing import Literal, Optional, Tuple
 
 
 if is_xformers_available():
     from xformers import ops as xops
 
 
 if is_flash_attn_available():
     from flash_attn import flash_attn_func, flash_attn_varlen_func
     from flash_attn.bert_padding import index_first_axis, pad_input, unpad_input  # noqa
 
 
 class MultiHeadAttentionLayer(nn.Module):
     '''多头注意力
     '''
-    def __init__(self, hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate=0.1, attention_scale=True,
-                 output_attentions=False, bias=True, p_bias=None, use_dynamic_ntk=False, flash_attention=None, use_logn_attn=None, **kwargs):
+    def __init__(self, hidden_size:int, num_attention_heads:int, attention_probs_dropout_prob:float, dropout_rate:float=0.1, attention_scale:bool=True,
+                 output_attentions:bool=False, bias:bool=True, p_bias:Literal[None, 'typical_relative', 'rotary', 't5_relative', 'deberta_v2', 'alibi']=None, 
+                 use_dynamic_ntk:bool=False, flash_attention:Literal[None, True, 'sdpa', 'xformers', 'flash_attn_2']=None, use_logn_attn:bool=None, **kwargs):
         super(MultiHeadAttentionLayer, self).__init__()
         self.hidden_size = hidden_size
         self.num_attention_heads = num_attention_heads
         self.attention_probs_dropout_prob = attention_probs_dropout_prob
         self.is_decoder = kwargs.get('is_decoder', False)
         self.attention_scale = attention_scale
         self.output_attentions = output_attentions
@@ -112,21 +114,23 @@
             self.norm_rel_ebd = [x.strip() for x in kwargs.get("norm_rel_ebd", "none").lower().split("|")]
             if "layer_norm" in self.norm_rel_ebd:
                 self.layernorm = nn.LayerNorm(self.hidden_size, kwargs.get('layer_norm_eps', 1e-12), elementwise_affine=True)
             self.pos_dropout = nn.Dropout(dropout_rate)
         elif self.p_bias == 'alibi':
             self.relative_positions_encoding = ALiBiPositionsEncoding(num_attention_heads)
 
-    def forward(self, hidden_states=None, attention_mask=None, encoder_hidden_states=None, encoder_attention_mask=None, past_key_value=None, position_ids=None, **model_kwargs):
+    def forward(self, hidden_states:Optional[torch.Tensor]=None, attention_mask:Optional[torch.FloatTensor]=None, 
+                encoder_hidden_states:Optional[torch.FloatTensor]=None, encoder_attention_mask:Optional[torch.FloatTensor]=None, 
+                past_key_value:Optional[Tuple[Tuple[torch.FloatTensor]]]=None, position_ids=None, **model_kwargs):
         '''
-        hidden_states shape: [batch_size, seq_q, hidden_size]
-        attention_mask shape: [batch_size, 1, 1, seq_q] 或者 [batch_size, 1, seq_q, seq_q]
-        encoder_hidden_states shape: [batch_size, seq_k, hidden_size]
-        encoder_attention_mask shape: [batch_size, 1, 1, seq_k]
-        past_key_value shape: ([batch_size, num_attention_heads, key_len_cache, attention_head_size], ...)
+        :param hidden_states: [batch_size, seq_q, hidden_size]
+        :param attention_mask: [batch_size, 1, 1, seq_q] 或者 [batch_size, 1, seq_q, seq_q]
+        :param encoder_hidden_states: [batch_size, seq_k, hidden_size]
+        :param encoder_attention_mask: [batch_size, 1, 1, seq_k]
+        :param past_key_value: ([batch_size, num_attention_heads, key_len_cache, attention_head_size], ...)
         '''
 
         # query_layer shape: [batch_size, num_attention_heads, query_len, attention_head_size]
         # key_layer shape: [batch_size, num_attention_heads, key_len, attention_head_size]
         # value_layer shape: [batch_size, num_attention_heads, value_len, attention_head_size]
         query_layer = self.transpose_for_q_scores(self.q(hidden_states))
         if self.p_bias == 'rotary':
@@ -258,15 +262,16 @@
     def apply_alibi_pos_emb(self, attention_scores, key_layer):
         ''' 执行alibi相对位置编码，单独拎出来主要是falcon是在+之后再执行attention_scale的 '''
         key_position_scores_r_t = self.relative_positions_encoding(key_layer)
         attention_scores = attention_scores + key_position_scores_r_t
         attention_scores = torch.max(attention_scores, torch.tensor(torch.finfo(attention_scores.dtype).min))  # baichuan-13b逻辑
         return attention_scores
 
-    def apply_rotary_pos_emb(self, query_layer, key_layer, value_layer, position_ids, past_key_value):
+    def apply_rotary_pos_emb(self, query_layer:torch.FloatTensor, key_layer:torch.FloatTensor, value_layer:torch.FloatTensor, 
+                             position_ids:torch.Tensor, past_key_value:Optional[Tuple[Tuple[torch.FloatTensor]]]=None):
         ''' 执行rotary相对位置编码 '''
         kv_seq_len = key_layer.shape[-2]
         if past_key_value is not None:
             kv_seq_len += past_key_value[0].shape[-2]
         
         if self.use_dynamic_ntk:
             # rotary的ntk，其实仅仅在step=1时候会触发
@@ -289,15 +294,15 @@
             query_layer, key_layer = self.relative_positions_encoding([query_layer, key_layer], position_ids, kv_seq_len)
         
         if past_key_value is not None:  # 过了rope再concat
             key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
             value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
         return query_layer, key_layer, value_layer
 
-    def apply_deberta_pos_emb(self, query_layer, key_layer, relative_pos, rel_embeddings, scale_factor):
+    def apply_deberta_pos_emb(self, query_layer:torch.FloatTensor, key_layer:torch.FloatTensor, relative_pos, rel_embeddings, scale_factor):
         '''deberta_v2使用，和原版区别是query_layer是4维, 原disentangled_attention_bias'''
         btz, n_head, q_len, d_head = query_layer.size()
         k_len = key_layer.size(-2)
         if relative_pos is None:
             relative_pos = self.relative_positions(q_len, k_len)
         if relative_pos.dim() == 2:
             relative_pos = relative_pos.unsqueeze(0).unsqueeze(0)
@@ -338,15 +343,15 @@
 
             p2c_pos = torch.clamp(-r_pos + att_span, 0, att_span * 2 - 1)
             p2c_att = torch.matmul(key_layer, pos_query_layer.transpose(-1, -2))
             p2c_att = torch.gather(p2c_att, dim=-1, index=p2c_pos.squeeze(0).expand([btz, n_head, k_len, k_len])).transpose(-1, -2)
             score += p2c_att / scale.to(dtype=p2c_att.dtype)
         return score
     
-    def torch_attention_forward(self, query_layer, key_layer, value_layer, attention_mask):
+    def torch_attention_forward(self, query_layer:torch.FloatTensor, key_layer:torch.FloatTensor, value_layer:torch.FloatTensor, attention_mask:torch.Tensor):
         '''qkv attention: torch原生实现'''
         # 交换k的最后两个维度，然后q和k执行点积, 获得attention score
         attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
 
         # attention_scores shape: [batch_size, num_attention_heads, query_len, key_len]
         if (self.p_bias == 'typical_relative') and hasattr(self, 'relative_positions_encoding'):
             # ==================== nezha相对位置编码 ====================
@@ -414,15 +419,16 @@
             # value_position_scores_r_t = value_position_scores_r.permute(1, 2, 0, 3)
             # 新实现
             value_position_scores_r_t = torch.einsum('bnij,ijh->bnih', attention_probs, relations_values)
             context_layer = context_layer + value_position_scores_r_t
 
         return context_layer, attention_scores
     
-    def flash_attention_forward(self, query_layer, key_layer, value_layer, attention_mask, query_length, softmax_scale=None):
+    def flash_attention_forward(self, query_layer:torch.FloatTensor, key_layer:torch.FloatTensor, value_layer:torch.FloatTensor, 
+                                attention_mask:torch.Tensor, query_length:int, softmax_scale:float=None):
         """ flash_attn，参考transformers中的调用
         """
         def _get_unpad_data(attention_mask):
             seqlens_in_batch = attention_mask.sum(dim=-1, dtype=torch.int32)
             indices = torch.nonzero(attention_mask.flatten(), as_tuple=False).flatten()
             max_seqlen_in_batch = seqlens_in_batch.max().item()
             cu_seqlens = F.pad(torch.cumsum(seqlens_in_batch, dim=0, dtype=torch.torch.int32), (1, 0))
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/core.py` & `bert4torch-0.5.0/bert4torch/layers/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from torch import nn
 import torch
 import torch.nn.functional as F
 from bert4torch.activations import get_activation
 from bert4torch.layers import SinusoidalPositionEncoding
 from bert4torch.snippets import torch_div, take_along_dim
-from typing import Union
+from typing import Union, Literal, Optional, List, Tuple
 
 
 class LayerNorm(nn.Module):
-    def __init__(self, hidden_size, eps=1e-12, conditional_size=False, weight=True, bias=True, norm_mode='normal', **kwargs):
+    def __init__(self, hidden_size:int, eps:float=1e-12, conditional_size:Union[bool, int]=False, weight:bool=True, bias:bool=True, 
+                 norm_mode:Literal['normal', 'torch_buildin', 'rmsnorm']='normal', **kwargs):
         """ layernorm层，自行实现是为了兼容conditianal layernorm，使得可以做条件文本生成、条件分类等任务
 
             :param hidden_size: int, layernorm的神经元个数
             :param eps: float
             :param conditional_size: int, condition layernorm的神经元个数; 详情：https://spaces.ac.cn/archives/7124
             :param weight: bool, 是否包含权重
             :param bias: bool, 是否包含偏置
@@ -35,15 +36,15 @@
         if conditional_size:
             # 这里采用全零初始化, 目的是在初始状态不干扰原来的预训练权重
             self.dense1 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense1.weight.data.uniform_(0, 0)
             self.dense2 = nn.Linear(conditional_size, hidden_size, bias=False)
             self.dense2.weight.data.uniform_(0, 0)
 
-    def forward(self, hidden_states, cond=None):
+    def forward(self, hidden_states:torch.FloatTensor, cond:Optional[torch.Tensor]=None):
         if isinstance(hidden_states, (list, tuple)):  # 兼容以前的久逻辑，后期测试后可删除
             cond = hidden_states[1] if self.conditional_size else None
             hidden_states = hidden_states[0]
 
         # torch自带LayerNorm
         if self.norm_mode == 'torch_buildin':
             return F.layer_norm(hidden_states, self.normalized_shape, self.weight, self.bias, self.eps)
@@ -72,16 +73,16 @@
         return output.type_as(hidden_states)
 
 
 class BertEmbeddings(nn.Module):
     """embeddings层
        构造word, position and token_type embeddings, 一般是token、position、segment三者embedding之和
     """
-    def __init__(self, vocab_size, embedding_size, hidden_size, max_position, segment_vocab_size, shared_segment_embeddings, dropout_rate, conditional_size=False, 
-                 pad_token_id=0, **kwargs):
+    def __init__(self, vocab_size:int, embedding_size:int, hidden_size:int, max_position:int, segment_vocab_size:int, shared_segment_embeddings:bool, 
+                 dropout_rate:float, conditional_size:Union[bool, int]=False, pad_token_id:int=0, **kwargs):
         super(BertEmbeddings, self).__init__()
         self.shared_segment_embeddings = shared_segment_embeddings
         self.word_embeddings = nn.Embedding(vocab_size, embedding_size, padding_idx=pad_token_id)
 
         # 位置编码
         if kwargs.get('p_bias') == 'sinusoid':
             self.position_embeddings = SinusoidalPositionEncoding(max_position, embedding_size)
@@ -121,15 +122,16 @@
         position_index_reshape = position_index.flatten()[:, None]
         # 为兼容低版本pytorch没有take_along_dim
         embeddings_x = take_along_dim(embeddings,  torch_div(position_index_reshape, embeddings.size(0), rounding_mode='trunc'), dim=0)  # 兼容老版本
         embeddings_y = take_along_dim(embeddings, position_index_reshape % embeddings.size(0), dim=0)
         position_embeddings = alpha * embeddings_x + (1 - alpha) * embeddings_y
         return position_embeddings.reshape(btz, seqlen, -1)  # [btz, seq_len, embed_size]
 
-    def apply_embeddings(self, token_ids:torch.Tensor, segment_ids:torch.Tensor, position_ids:torch.Tensor, additional_embs:Union[tuple, list]=None, **kwargs):
+    def apply_embeddings(self, token_ids:torch.Tensor, segment_ids:torch.Tensor, position_ids:torch.Tensor, 
+                         additional_embs:Union[Tuple[torch.Tensor], List[torch.Tensor]]=None, **kwargs):
         '''单独拆分出来，方便下游继承和修改'''
         # word embedding
         if (not token_ids.requires_grad) and (token_ids.dtype in {torch.long, torch.int}):
             words_embeddings = self.word_embeddings(token_ids)
         else:
             words_embeddings = token_ids  # 自定义word_embedding，目前仅有VAT中使用
 
@@ -159,15 +161,16 @@
         
         # 额外的embedding，如词性等
         if additional_embs is not None:
             for emb in additional_embs:
                 embeddings += emb
         return embeddings
 
-    def forward(self, token_ids=None, segment_ids=None, position_ids=None, conditional_emb=None, additional_embs=None, attention_mask=None, **kwargs):
+    def forward(self, token_ids:torch.Tensor=None, segment_ids:torch.Tensor=None, position_ids:torch.Tensor=None, conditional_emb:Optional[torch.Tensor]=None, 
+                additional_embs:Union[Tuple[torch.Tensor], List[torch.Tensor]]=None, attention_mask:torch.Tensor=None, **kwargs):
         embeddings = self.apply_embeddings(token_ids, segment_ids, position_ids, additional_embs, **kwargs)
 
         if self.emb_scale != 1:
             embeddings = embeddings * self.emb_scale  # transform_xl, xlnet特有
 
         if hasattr(self, 'layerNorm'):
             embeddings = self.layerNorm(embeddings, conditional_emb)
@@ -180,15 +183,15 @@
 
         if hasattr(self, 'embedding_hidden_mapping_in'):
             embeddings = self.embedding_hidden_mapping_in(embeddings)
         return embeddings
 
 
 class PositionWiseFeedForward(nn.Module):
-    def __init__(self, hidden_size, intermediate_size, dropout_rate=0.5, hidden_act='gelu', is_dropout=False, bias=True, **kwargs):
+    def __init__(self, hidden_size:int, intermediate_size:int, dropout_rate:float=0.5, hidden_act:str='gelu', is_dropout:bool=False, bias:bool=True, **kwargs):
         # 原生的tf版本的bert在激活函数后，没有添加dropout层，但是在google AI的bert-pytorch开源项目中，多了一层dropout；
         # 并且在pytorch官方的TransformerEncoderLayer的实现中，也有一层dropout层，就像这样：self.linear2(self.dropout(self.activation(self.linear1(src))))；
         # 这样不统一做法的原因不得而知，不过有没有这一层，差别可能不会很大；
 
         # 为了适配是否dropout，用is_dropout，dropout_rate两个参数控制；如果是实现原始的transformer，直接使用默认参数即可；如果是实现bert，则is_dropout为False，此时的dropout_rate参数并不会使用.
         super(PositionWiseFeedForward, self).__init__()
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/crf.py` & `bert4torch-0.5.0/bert4torch/layers/crf.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/global_point.py` & `bert4torch-0.5.0/bert4torch/layers/global_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 class GlobalPointer(nn.Module):
     """全局指针模块
     将序列的每个(start, end)作为整体来进行判断
     参考：https://kexue.fm/archives/8373
 
     :param hidden_size: 即模型最顶层输出的hidden_size
-    :param heads heads: 在实体识别和关系提取中，分别代表着实体个数和关系个数
+    :param heads: 在实体识别和关系提取中，分别代表着实体个数和关系个数
     :param head_size: 即每个heads的神经元个数，点积时候使用，相当于attention
     """
-    def __init__(self, hidden_size, heads, head_size, RoPE=True, use_bias=True, tril_mask=True):
+    def __init__(self, hidden_size:int, heads:int, head_size:int, RoPE:bool=True, use_bias:bool=True, tril_mask:bool=True):
         super().__init__()
         self.heads = heads
         self.head_size = head_size
         self.RoPE = RoPE
         self.tril_mask = tril_mask
 
         self.dense = nn.Linear(hidden_size, heads * head_size * 2, bias=use_bias)
         if self.RoPE:
             self.position_embedding = RoPEPositionEncoding(head_size)
 
-    def forward(self, inputs, mask=None):
+    def forward(self, inputs:torch.Tensor, mask:torch.Tensor=None):
         ''' 
         :param inputs: shape=[..., hdsz]
         :param mask: shape=[btz, seq_len], padding部分为0
         '''
         sequence_output = self.dense(inputs)  # [..., heads*head_size*2]
         sequence_output = torch.stack(torch.chunk(sequence_output, self.heads, dim=-1), dim=-2)  # [..., heads, head_size*2]
         qw, kw = sequence_output[..., :self.head_size], sequence_output[..., self.head_size:]  # [..., heads, head_size]
@@ -57,27 +57,27 @@
 
 
 class EfficientGlobalPointer(nn.Module):
     """更加参数高效的GlobalPointer
     参考：https://kexue.fm/archives/8877
     这里实现和GlobalPointer相似，而未采用原版的奇偶位来取qw和kw，个人理解两种方式是无区别的
     """
-    def __init__(self, hidden_size, heads, head_size, RoPE=True, use_bias=True, tril_mask=True):
+    def __init__(self, hidden_size:int, heads:int, head_size:int, RoPE:bool=True, use_bias:bool=True, tril_mask:bool=True):
         super().__init__()
         self.heads = heads
         self.head_size = head_size
         self.RoPE = RoPE
         self.tril_mask = tril_mask
 
         self.p_dense = nn.Linear(hidden_size, head_size * 2, bias=use_bias)
         self.q_dense = nn.Linear(head_size * 2, heads * 2, bias=use_bias)
         if self.RoPE:
             self.position_embedding = RoPEPositionEncoding(head_size)
 
-    def forward(self, inputs, mask=None):
+    def forward(self, inputs:torch.Tensor, mask:torch.Tensor=None):
         ''' 
         :param inputs: shape=[..., hdsz]
         :param mask: shape=[btz, seq_len], padding部分为0
         '''
         sequence_output = self.p_dense(inputs)  # [..., head_size*2]
         qw, kw = sequence_output[..., :self.head_size], sequence_output[..., self.head_size:]  # [..., head_size]
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/misc.py` & `bert4torch-0.5.0/bert4torch/layers/misc.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/moe.py` & `bert4torch-0.5.0/bert4torch/layers/moe.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/position_encoding.py` & `bert4torch-0.5.0/bert4torch/layers/position_encoding.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/layers/transformer_block.py` & `bert4torch-0.5.0/bert4torch/layers/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from torch import nn
 import torch
 import math
 import torch.nn.functional as F
 from bert4torch.layers.core import LayerNorm, PositionWiseFeedForward
 from bert4torch.layers.attention import MultiHeadAttentionLayer, GatedAttentionUnit
+from typing import Union, Optional, Tuple
 
 
 class BertLayer(nn.Module):
     """Transformer层:
        顺序为: Attention --> Add --> LayerNorm --> Feed Forward --> Add --> LayerNorm
 
        注意:
         1. 以上都不计dropout层，并不代表没有dropout，每一层的dropout使用略有不同，注意区分
         2. 原始的Transformer的encoder中的Feed Forward层一共有两层linear，
         3. config.intermediate_size的大小不仅是第一层linear的输出尺寸，也是第二层linear的输入尺寸
     """
-    def __init__(self, hidden_size, num_attention_heads, dropout_rate, attention_probs_dropout_prob, intermediate_size, hidden_act, 
-                 is_dropout=False, conditional_size=False, pre_layernorm=False, apply_residual_post_layernorm=False, **kwargs):
+    def __init__(self, hidden_size:int, num_attention_heads:int, dropout_rate:float, attention_probs_dropout_prob:float, intermediate_size:int, hidden_act:str, 
+                 is_dropout:bool=False, conditional_size:Union[bool, int]=False, pre_layernorm:bool=False, apply_residual_post_layernorm:bool=False, **kwargs):
         super(BertLayer, self).__init__()
         self.dropout_rate = dropout_rate
         layer_norm_eps = kwargs.get('layer_norm_eps', 1e-12)
         self.pre_layernorm = pre_layernorm  # True表示pre, False表示post
         self.apply_residual_post_layernorm = apply_residual_post_layernorm
         self.is_decoder = kwargs.get('is_decoder', False)
         self.add_cross_attention = kwargs.get('add_cross_attention', False)
@@ -34,16 +35,17 @@
         self.ffnLayerNorm = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
 
         # cross attention
         if self.add_cross_attention and self.is_decoder:
             self.crossAttention = MultiHeadAttentionLayer(hidden_size, num_attention_heads, attention_probs_dropout_prob, dropout_rate, **kwargs)
             self.crossLayerNorm = LayerNorm(hidden_size, eps=layer_norm_eps, conditional_size=conditional_size, **kwargs)
 
-    def forward(self, hidden_states=None, attention_mask=None, position_ids=None, conditional_emb=None, encoder_hidden_states=None, 
-                encoder_attention_mask=None, past_key_value=None, cross_past_key_value=None, **model_kwargs):
+    def forward(self, hidden_states:torch.FloatTensor=None, attention_mask:torch.Tensor=None, position_ids:torch.FloatTensor=None, 
+                conditional_emb:Optional[torch.Tensor]=None, encoder_hidden_states=None, encoder_attention_mask:Optional[torch.FloatTensor]=None, 
+                past_key_value:Optional[Tuple[Tuple[torch.FloatTensor]]]=None, cross_past_key_value:Optional[Tuple[Tuple[torch.FloatTensor]]]=None, **model_kwargs):
         return_tensors = dict()
         # ============== self attention ==============
         x = self.attnLayerNorm(hidden_states, conditional_emb) if self.pre_layernorm else hidden_states  # pre/post layernorm
         self_attn_output = self.multiHeadAttention(x, attention_mask, past_key_value=past_key_value, position_ids=position_ids)  # self.decoder为true时候，这里的attention_mask是三角的
         residual = x if self.apply_residual_post_layernorm else hidden_states
         hidden_states = self.dropout_add(self_attn_output[0], residual)
         hidden_states = self.attnLayerNorm(hidden_states, conditional_emb) if not self.pre_layernorm else hidden_states
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/losses.py` & `bert4torch-0.5.0/bert4torch/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,8 +412,36 @@
             all_logps = (per_token_logps * loss_mask).sum(-1) / loss_mask.sum(-1)
         else:
             all_logps =  (per_token_logps * loss_mask).sum(-1)
 
         split = labels.shape[0] // 2
         chosen_logps = all_logps[:split]
         rejected_logps = all_logps[split:]
-        return chosen_logps, rejected_logps
+        return chosen_logps, rejected_logps
+    
+
+class CausalLMLoss(nn.CrossEntropyLoss):
+    '''Causal语言模型的Loss
+
+    :param offset: 是否对logit和labels做错位处理, 取决于在做数据时候是否已经offset过
+    '''
+    def __init__(self, *args, offset=False, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.offset = offset
+
+    def forward(self, logits, labels):
+        """
+        logits: [btz, seq_len, vocab_size]
+        labels: 即token_ids, [btz, seq_len]
+        """
+        raw_dtyps = logits.dtype
+        logits = logits.to(torch.float32)
+
+        if self.offset:
+            logits = logits[:, :-1, :].contiguous()  # 预测序列，错开一位
+            labels = labels[:, 1:].contiguous() # 目标token_ids
+
+        logits = logits.reshape(-1, logits.shape[-1])
+        labels = labels.flatten()
+        loss = super().forward(logits, labels)
+
+        return loss.to(raw_dtyps)
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/__init__.py` & `bert4torch-0.5.0/bert4torch/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Union
 from torch4keras.model import *
-from bert4torch.snippets import set_default_torch_dtype, get_checkpoint_path, get_config_path, is_accelerate_available
+from bert4torch.snippets import set_default_torch_dtype, get_checkpoint_path, get_config_path, is_accelerate_available, log_error
 from bert4torch.models.albert import *
 from bert4torch.models.bart import *
 from bert4torch.models.base import *
 from bert4torch.models.bert import *
 from bert4torch.models.deberta import *
 from bert4torch.models.electra import *
 from bert4torch.models.ernie import *
@@ -21,18 +20,19 @@
 from bert4torch.models.xlnet import *
 from bert4torch.models.bloom import *
 from bert4torch.models.qwen import *
 from bert4torch.models.internlm import *
 from bert4torch.models.falcon import *
 from bert4torch.models.deepseek import *
 from typing import Union, Literal
+import json
 
 
-def build_transformer_model(config_path:Union[str, os.PathLike]=None, checkpoint_path:Union[str, os.PathLike, list]=None, model:Union[str, BERT_BASE]=None, 
-                            application:Literal['encoder', 'lm', 'unilm']=None, 
+def build_transformer_model(config_path:Union[str, os.PathLike]=None, checkpoint_path:Union[str, os.PathLike, list]=None, 
+                            model:Union[str, BERT_BASE]=None, application:Literal['encoder', 'lm', 'unilm']=None, 
                             add_trainer:bool=False, verbose:int=1, **kwargs) -> Union[BERT_BASE, BERT, Transformer, Trainer]:
     """根据配置文件构建模型, 可选加载checkpoint权重
 
     :param config_path: str, 模型的config文件地址, 大部分模型都提供了bert4torch_config.json
     :param checkpoint_path: str/list[str], 模型文件/文件夹地址, 默认值None表示不加载预训练模型
     :param model: str, 加载的模型结构, 这里Model也可以基于nn.Module自定义后传入, 默认为'bert'
     :param application: str, 模型应用, 支持encoder, lm和unilm格式, 默认为'encoder'
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/albert.py` & `bert4torch-0.5.0/bert4torch/models/albert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/bart.py` & `bert4torch-0.5.0/bert4torch/models/bart.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/base.py` & `bert4torch-0.5.0/bert4torch/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 
 
 class BERT_BASE(nn.Module):
     """模型基类
     """
     def __init__(
             self,
-            vocab_size,  # 词表大小
-            hidden_size,  # 编码维度
-            num_hidden_layers,  # Transformer总层数
-            num_attention_heads,  # Attention的头数
-            intermediate_size,  # FeedForward的隐层维度
-            hidden_act,  # FeedForward隐层的激活函数
-            dropout_rate=None,  # Dropout比例
-            attention_probs_dropout_prob=None,  # Attention矩阵的Dropout比例
-            embedding_size=None,  # 指定embedding_size, 不指定则使用config文件的参数
-            attention_head_size=None,  # Attention中V的head_size
-            attention_key_size=None,  # Attention中Q,K的head_size
-            initializer_range=0.02,  # 权重初始化方差
-            sequence_length=None,  # 是否固定序列长度
-            keep_tokens=None,  # 要保留的词ID列表
-            compound_tokens=None,  # 扩展Embedding
-            residual_attention_scores=False,  # Attention矩阵加残差
-            keep_hidden_layers=None, # 保留的hidden_layer层的id
-            hierarchical_position=None,  # 是否层次分解位置编码
-            gradient_checkpoint=False, # 是否使用gradient_checkpoint
-            output_all_encoded_layers=False, # 是否返回所有layer的hidden_states
-            tie_emb_prj_weight=False,  # 是否绑定embedding和lm_head的权重
-            return_dict=False,  # 是否返回的格式是dict
+            vocab_size:int,  # 词表大小
+            hidden_size:int,  # 编码维度
+            num_hidden_layers:int,  # Transformer总层数
+            num_attention_heads:int,  # Attention的头数
+            intermediate_size:int,  # FeedForward的隐层维度
+            hidden_act:str,  # FeedForward隐层的激活函数
+            dropout_rate:float=None,  # Dropout比例
+            attention_probs_dropout_prob:float=None,  # Attention矩阵的Dropout比例
+            embedding_size:int=None,  # 指定embedding_size, 不指定则使用config文件的参数
+            attention_head_size:int=None,  # Attention中V的head_size
+            attention_key_size:int=None,  # Attention中Q,K的head_size
+            initializer_range:float=0.02,  # 权重初始化方差
+            sequence_length:int=None,  # 是否固定序列长度
+            keep_tokens:List[int]=None,  # 要保留的词ID列表
+            compound_tokens:List[int]=None,  # 扩展Embedding
+            residual_attention_scores:bool=False,  # Attention矩阵加残差
+            keep_hidden_layers:List[int]=None, # 保留的hidden_layer层的id
+            hierarchical_position:Union[bool, float]=None,  # 是否层次分解位置编码
+            gradient_checkpoint:bool=False, # 是否使用gradient_checkpoint
+            output_all_encoded_layers:bool=False, # 是否返回所有layer的hidden_states
+            tie_emb_prj_weight:bool=False,  # 是否绑定embedding和lm_head的权重
+            return_dict:bool=False,  # 是否返回的格式是dict
             **kwargs
     ):
         super(BERT_BASE, self).__init__()
         if keep_tokens is not None:
             vocab_size = len(keep_tokens)
         if compound_tokens is not None:
             vocab_size += len(compound_tokens)
@@ -328,20 +328,26 @@
         for k in list(state_dict.keys()):
             if isinstance(mapping, dict):
                 state_dict[mapping.get(k, k)] = state_dict.pop(k)
             elif isinstance(mapping, Callable):
                 state_dict[mapping(k)] = state_dict.pop(k)
         
         # 如果save_path是文件夹，则把对应的其他文件copy过去
-        save_dir = None if re.search('\.[a-zA-z0-9]+$', save_path) else save_path
+        save_dir = None if re.search(r'\.[a-zA-z0-9]+$', save_path) else save_path
 
         # 把checkpoint_path所在目录下，除了权重文件的其他文件copy过去
         if write_to_disk and hasattr(self, 'checkpoint_path') and (self.checkpoint_path is not None) and save_dir:
-            checkpoint_dir = os.path.dirname(self.checkpoint_path) if os.path.isfile(self.checkpoint_path) else self.checkpoint_path
-            copytree(checkpoint_dir, save_dir, ignore_copy_files=['\.bin$', '\.safetensors$'], dirs_exist_ok=True)  # 如果目录下文件存在也会强制覆盖
+            if isinstance(self.checkpoint_path, str):
+                checkpoint_dir = os.path.dirname(self.checkpoint_path) if os.path.isfile(self.checkpoint_path) else self.checkpoint_path
+            elif isinstance(self.checkpoint_path, (tuple, list)):
+                checkpoint_dir = os.path.dirname(self.checkpoint_path[0]) if os.path.isfile(self.checkpoint_path[0]) else self.checkpoint_path[0]
+            else:
+                raise TypeError(f'`self.checkpoint_path` only support str,tuple,list')
+
+            copytree(checkpoint_dir, save_dir, ignore_copy_files=[r'\.bin$', r'\.safetensors$'], dirs_exist_ok=True)  # 如果目录下文件存在也会强制覆盖
 
             # checkpoint shards对应的.index.json
             bin_index_json = [os.path.join(checkpoint_dir, i) for i in os.listdir(checkpoint_dir) if i.endswith('.index.json')]
             bin_index_json = bin_index_json[0] if bin_index_json else ''
             if (save_dir is not None) and os.path.exists(bin_index_json):
                 weight_map = weight_map or JsonConfig(bin_index_json).get('weight_map')
 
@@ -420,15 +426,15 @@
         outputs = outputs[:]
         self.outputs = outputs
         if len(outputs) > 1:
             self.output = outputs
         else:
             self.output = outputs[0]
 
-    def quantize(self, quantization_method, **kwargs):
+    def quantize(self, quantization_method:Literal['cpm_kernels', 'load_in_8bit', 'load_in_4bit'], **kwargs):
         '''量化'''
         if self.quantized:
             print("Already quantized.")
             return self
         
         new_kwargs = copy.deepcopy(kwargs)
         if 'model' in new_kwargs:
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/bert.py` & `bert4torch-0.5.0/bert4torch/models/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 from bert4torch.models.base import BERT_BASE
 from bert4torch.layers import LayerNorm, BertEmbeddings
 from bert4torch.layers import LayerNorm, BertEmbeddings, BertLayer, BlockIdentity
 from bert4torch.snippets import old_checkpoint, create_position_ids_start_at_padding, DottableDict, modify_variable_mapping
 from bert4torch.activations import get_activation
 import copy
 from packaging import version
-from typing import Union
+from typing import Union, Literal, List
 
 
 class BERT(BERT_BASE):
     """构建BERT模型
     """
     def __init__(
             self,
-            max_position,  # 序列最大长度
-            segment_vocab_size=2,  # segment总数目
-            with_pool=False,  # 是否包含Pool部分
-            with_nsp=False,  # 是否包含NSP部分
-            with_mlm=False,  # 是否包含MLM部分
-            custom_position_ids=False,  # 是否自行传入位置id, True表示传入，False表示不传入，'start_at_padding'表示从padding_idx+1开始
-            custom_attention_mask=False, # 是否自行传入attention_mask
-            shared_segment_embeddings=False,  # 若True，则segment跟token共用embedding
-            conditional_size=None,  # conditional layer_norm
-            additional_embs=False, # addtional_embeddng, 是否有额外的embedding, 比如加入词性，音调，word粒度的自定义embedding
-            is_dropout=False,
-            pad_token_id=0,  # 默认0是padding ids, 但是注意google的mt5padding不是0
+            max_position:int,  # 序列最大长度
+            segment_vocab_size:int=2,  # segment总数目
+            with_pool:bool=False,  # 是否包含Pool部分
+            with_nsp:bool=False,  # 是否包含NSP部分
+            with_mlm:bool=False,  # 是否包含MLM部分
+            custom_position_ids:Literal[True, False, 'start_at_padding']=False,  # 是否自行传入位置id, True表示传入，False表示不传入，'start_at_padding'表示从padding_idx+1开始
+            custom_attention_mask:bool=False, # 是否自行传入attention_mask
+            shared_segment_embeddings:bool=False,  # 若True，则segment跟token共用embedding
+            conditional_size:Union[bool, int]=None,  # conditional layer_norm
+            additional_embs:Union[bool, torch.Tensor, List[torch.Tensor]]=False, # addtional_embeddng, 是否有额外的embedding, 比如加入词性，音调，word粒度的自定义embedding
+            is_dropout:bool=False,
+            pad_token_id:int=0,  # 默认0是padding ids, 但是注意google的mt5padding不是0
             **kwargs  # 其余参数
     ):
         super(BERT, self).__init__(**kwargs)
         self.max_position = max_position
         self.segment_vocab_size = segment_vocab_size
         self.with_pool = with_pool
         self.with_nsp = with_nsp
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/bloom.py` & `bert4torch-0.5.0/bert4torch/models/bloom.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/deberta.py` & `bert4torch-0.5.0/bert4torch/models/deberta.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/deepseek.py` & `bert4torch-0.5.0/bert4torch/models/deepseek.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/electra.py` & `bert4torch-0.5.0/bert4torch/models/electra.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/ernie.py` & `bert4torch-0.5.0/bert4torch/models/ernie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/falcon.py` & `bert4torch-0.5.0/bert4torch/models/falcon.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/gau_alpha.py` & `bert4torch-0.5.0/bert4torch/models/gau_alpha.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/glm.py` & `bert4torch-0.5.0/bert4torch/models/glm.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/gpt.py` & `bert4torch-0.5.0/bert4torch/models/gpt.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/internlm.py` & `bert4torch-0.5.0/bert4torch/models/internlm.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/llama.py` & `bert4torch-0.5.0/bert4torch/models/llama.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/nezha.py` & `bert4torch-0.5.0/bert4torch/models/nezha.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/qwen.py` & `bert4torch-0.5.0/bert4torch/models/qwen.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/roformer.py` & `bert4torch-0.5.0/bert4torch/models/roformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/t5.py` & `bert4torch-0.5.0/bert4torch/models/t5.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/transformer.py` & `bert4torch-0.5.0/bert4torch/models/transformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/transformer_xl.py` & `bert4torch-0.5.0/bert4torch/models/transformer_xl.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/uie.py` & `bert4torch-0.5.0/bert4torch/models/uie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/models/xlnet.py` & `bert4torch-0.5.0/bert4torch/models/xlnet.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/optimizers.py` & `bert4torch-0.5.0/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/base.py` & `bert4torch-0.5.0/bert4torch/pipelines/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-from typing import List, Union, Dict
+from typing import List, Union, Dict, Literal
 import numpy as np
 import os
 import torch
 from bert4torch.models import build_transformer_model
 from bert4torch.snippets import sequence_padding
 from bert4torch.tokenizers import Tokenizer
 from tqdm.autonotebook import trange
 
 
 class PipeLineBase:
     '''基类
     '''
-    def __init__(self, checkpoint_path:str, device:str=None, **kwargs) -> None:        
+    def __init__(self, checkpoint_path:str, device:str=None, tokenizer_type:Literal['b4t', 'hf']='b4t', **kwargs) -> None:        
         self.checkpoint_path = checkpoint_path
         self.config_path = kwargs.get('config_path') or checkpoint_path
         if device is None:
             self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
         else:
             self.device = device
+        
+        if (tokenizer_type == 'b4t') and os.path.exists(os.path.join(self.checkpoint_path, 'vocab.txt')):
+            self.tokenizer_type = 'b4t'
+        else:
+            self.tokenizer_type = 'hf'
         self.tokenizer = self.build_tokenizer()
         self.model = self.build_model(kwargs)
         self.config = self.model.config
     
     def build_tokenizer(self):
-        vocab_path = os.path.join(self.checkpoint_path, 'vocab.txt')
-        if os.path.exists(vocab_path):
-            tokenizer = Tokenizer(vocab_path, do_lower_case=True)
+        # TODO: 默认优先使用默认的Tokenizer，如果没有vocab文件，则使用AutoTokenizer，后续可能修改
+        if self.tokenizer_type == 'b4t':
+            tokenizer = Tokenizer(os.path.join(self.checkpoint_path, 'vocab.txt'), do_lower_case=True)
         else:
             from transformers import AutoTokenizer
             tokenizer = AutoTokenizer.from_pretrained(self.checkpoint_path)
         return tokenizer
 
     def build_model(self, model_config):
         model = build_transformer_model(config_path=self.config_path, checkpoint_path=self.checkpoint_path, return_dict=True, **model_config).to(self.device)
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/chat/base.py` & `bert4torch-0.5.0/bert4torch/pipelines/chat/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,25 +74,25 @@
             log_info(f'{cur} - Moving model from cpu to {self.device}')
             self.model.to(self.device)
             gc.collect()
             cuda_empty_cache()
             
         return self.model
     
-    def process_response(self, response:Union[str,tuple,list], history:List[Tuple]=None):
+    def process_response(self, response:Union[str,tuple,list], history:List[Tuple]=None) -> str:
         '''对response进行后处理，可自行继承后来自定义'''
         if isinstance(response, str):
             return response
         elif isinstance(response, (tuple, list)):  # response, states
             assert len(response) == 2
             self.generation_config['states'] = response[1]
             return response[0]
         return response
 
-    def chat(self, query:Union[str,list], history:List[Tuple]=[]):
+    def chat(self, query:Union[str,list], history:List[Tuple]=[]) -> str:
         if isinstance(query, str):
             prompt = self.build_prompt(query, history)
         elif isinstance(query, list):
             prompt = [self.build_prompt(q, history) for q in query]
         self.model = self._build_model()
         response = self.model.generate(prompt, **self.generation_config)
         return self.process_response(response, history=history)
@@ -110,23 +110,37 @@
     :param init_str: str, 对话问候句
     :param history_maxlen: int, 保留的历史对话轮次
     '''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.init_str = kwargs.get('init_str', "输入内容进行对话，clear清空对话历史，stop终止程序")
         self.history_maxlen = kwargs.get('history_maxlen', 0)
+        log_info(f'History chat length = {self.history_maxlen}')
 
-    def build_cli_text(self, history):
+    def build_cli_text(self, history) -> str:
         '''构建命令行终端显示的text'''
         prompt = self.init_str
         for query, response in history:
             prompt += f"\n\nUser：{query}"
             prompt += f"\n\nAssistant：{response}"
         return prompt
 
+    def build_cli_history(self, cli_pre_history, cli_new_history):
+        # 带最近的几条历史
+        if self.history_maxlen > 0:
+            history = cli_new_history[-self.history_maxlen:]
+            if len(cli_new_history) >= self.history_maxlen:
+                cli_pre_history += cli_new_history[:-self.history_maxlen]
+        else:
+            # 默认不带历史聊天
+            history = []
+            cli_pre_history += cli_new_history
+        assert len(history) <= self.history_maxlen
+        return history, cli_pre_history
+
     def run(self, stream:bool=True):
         import platform
         os_name = platform.system()
         cli_pre_history, history = [], []
         clear_command = 'cls' if os_name == 'Windows' else 'clear'
         print(self.init_str)
         while True:
@@ -140,33 +154,32 @@
                 cuda_empty_cache()
                 os.system(clear_command)
                 print(self.init_str)
                 continue
             
             prompt = self.build_prompt(query, history)
             self.model = self._build_model()
+            # history是human和assistant的聊天历史
+            # 格式如[('你好', '有什么可以帮您的？'), ('你是谁？', '我是一款人工智能助手。')]
             if stream:
                 for response in self.model.stream_generate(prompt, **self.generation_config):
                     response = self.process_response(response, history)
                     cli_new_history = history + [(query, response)]
                     os.system(clear_command)
                     print(self.build_cli_text(cli_pre_history + cli_new_history), flush=True)
             else:
                 response = self.model.generate(prompt, **self.generation_config)
                 response = self.process_response(response, history)
                 cli_new_history = history + [(query, response)]
             
             os.system(clear_command)
             print(self.build_cli_text(cli_pre_history + cli_new_history), flush=True)
-            if self.history_maxlen > 0:
-                history = cli_new_history[-self.history_maxlen:]
-                if len(cli_new_history) > self.history_maxlen:
-                    cli_pre_history += cli_new_history[:-self.history_maxlen]
-            else:
-                cli_pre_history += cli_new_history
+
+            # 更新历史
+            history, cli_pre_history = self.build_cli_history(cli_pre_history, cli_new_history)
             cuda_empty_cache()
 
 
 def extend_with_cli(InputModel) -> ChatCli:
     """添加ChatCliDemo"""
     class ChatDemo(InputModel, ChatCli):
         pass
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/chat/llm.py` & `bert4torch-0.5.0/bert4torch/pipelines/chat/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         response = response.strip()
         response = response.replace("[[训练时间]]", "2023年")
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
             [";", "；"],
-            ["\?", "？"],
+            [r"\?", "？"],
         ]
         for item in punkts:
             response = re.sub(r"([\u4e00-\u9fff])%s" % item[0], r"\1%s" % item[1], response)
             response = re.sub(r"%s([\u4e00-\u9fff])" % item[0], r"%s\1" % item[1], response)
         return response
 ChatGlmCli = extend_with_cli(ChatGlm)
 ChatGlmWebGradio = extend_with_web_gradio(ChatGlm)
@@ -66,51 +66,62 @@
         response = response.strip()
         response = response.replace("[[训练时间]]", "2023年")
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
             [";", "；"],
-            ["\?", "？"],
+            [r"\?", "？"],
         ]
         for item in punkts:
             response = re.sub(r"([\u4e00-\u9fff])%s" % item[0], r"\1%s" % item[1], response)
             response = re.sub(r"%s([\u4e00-\u9fff])" % item[0], r"%s\1" % item[1], response)
         return response
 ChatGlm2Cli = extend_with_cli(ChatGlm2)
 ChatGlm2WebGradio = extend_with_web_gradio(ChatGlm2)
 ChatGlm2WebStreamlit = extend_with_web_streamlit(ChatGlm2)
 ChatGlm2OpenaiApi = extend_with_chat_openai_api(ChatGlm2)
 
 
 class ChatGlm3(Chat):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.history_maxlen *= 2
+
     def build_prompt(self, query, history=[]):
         # 由于tokenizer封装了部分逻辑，这里直接转成input_ids
         if (len(history) > 0) and isinstance(history[-1], tuple):
             history.pop()
         history.append({"role": "user", "content": query})
         history.append({"role": "assistant", "content": ""})
         if self.no_history_states():
             input_ids = self.tokenizer.build_chat_input(query, history=history, role="user")['input_ids']
         else:
-            input_ids = self.tokenizer.build_chat_input(query, role="user")['input_ids']  # TODO: 这里是否在开头需要增加last_token_id
+            input_ids += self.generation_config['states']['last_token']
         return input_ids
 
     def build_cli_text(self, history):
         '''构建命令行终端显示的text'''
         prompt = self.init_str
-        for hist in history[:-1]:  # 去除ChatCliDemo添加的当前回复的记录
-            if hist['role'] == 'user':
+        for hist in history:  # 去除ChatCliDemo添加的当前回复的记录
+            if not isinstance(hist, dict):
+                continue
+            elif hist['role'] == 'user':
                 query = hist['content']
                 prompt += f"\n\nUser：{query}"
             elif hist['role'] == 'assistant':
                 response = hist['content']
                 prompt += f"\n\nAssistant：{response}"
         return prompt
     
+    def build_cli_history(self, cli_pre_history, cli_new_history):
+        if (len(cli_new_history) > 0) and isinstance(cli_new_history[-1], tuple):
+            cli_new_history.pop()
+        return super().build_cli_history(cli_pre_history, cli_new_history)
+    
     def process_response(self, response, history):
         response = super().process_response(response)
         if (not response) or (response[-1] == "�"):
             return response, history
 
         content = ""
         for response in response.split("<|assistant|>"):
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/chat/openai_api.py` & `bert4torch-0.5.0/bert4torch/pipelines/chat/openai_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,15 +126,16 @@
     def __init__(self, checkpoint_path:str, name:str='default', route_api:str='/chat/completions', route_models:str='/models', 
                  max_callapi_interval:int=24*3600, scheduler_interval:int=10*60, offload_when_nocall:Literal['cpu', 'disk']=None, 
                  api_keys:List[str]=None, **kwargs):
         self.offload_when_nocall = offload_when_nocall
         if offload_when_nocall is not None:
             kwargs['create_model_at_startup'] = False
         super().__init__(checkpoint_path, **kwargs)
-        assert is_fastapi_available(), "No module found, use `pip install fastapi`"
+        if not is_fastapi_available():
+            raise ModuleNotFoundError("No module found, use `pip install fastapi`")
         from sse_starlette.sse import ServerSentEvent, EventSourceResponse
         import sse_starlette
         if version.parse(sse_starlette.__version__) > version.parse('1.8'):
             log_warn('Module `sse_starlette` above 1.8 not support stream output')
         self.max_callapi_interval = max_callapi_interval  # 最长调用间隔
         self.scheduler_interval = scheduler_interval
         self.api_keys = api_keys
@@ -217,14 +218,15 @@
         if request.repetition_penalty:
             self.generation_config['repetition_penalty'] = request.repetition_penalty
 
         if request.messages[-1].role != self.role_user:
             raise HTTPException(status_code=400, detail="Invalid request")
         query = request.messages[-1].content
 
+        # 首条可以是role_system
         prev_messages = request.messages[:-1]
         if len(prev_messages) > 0 and prev_messages[0].role == self.role_system:
             query = prev_messages.pop(0).content + query
 
         history = []
         if len(prev_messages) % 2 == 0:
             for i in range(0, len(prev_messages), 2):
@@ -342,92 +344,113 @@
     >>> 
     >>> # 流式
     >>> for token in client.stream_chat(messages):
     >>>     print(token, end='', flush=True)
     >>> # 非流式
     >>> print(client.chat(messages))
     '''
-    def __init__(self, base_url) -> None:
+    def __init__(self, base_url:str, api_key:str=None, **kwargs) -> None:
         from openai import OpenAI
-        self.client = OpenAI(base_url=base_url, api_key="EMPTY")
+        self.client = OpenAI(base_url=base_url, api_key=api_key, **kwargs)
     
-    def stream_chat(self, messages:List[Dict], model:str='default', max_length:int=None, temperature:float=None, top_p:float=None):
+    def stream_chat(self, messages:List[Dict], model:str='default', max_length:int=None, temperature:float=None, top_p:float=None, **kwargs):
         '''流式返回'''
         response = self.client.chat.completions.create(
             model=model,
             messages=messages,
             stream=True,
             max_tokens=max_length,
             temperature=temperature,
-            top_p=top_p
+            top_p=top_p,
+            **kwargs
             )
 
         for chunk in response:
             content = chunk.choices[0].delta.content
             if content is not None:
                 yield content
 
-    def chat(self, messages:List[Dict], model:str='default', max_length:int=None, temperature:float=None, top_p:float=None):
+    def chat(self, messages:List[Dict], model:str='default', max_length:int=None, temperature:float=None, top_p:float=None, **kwargs):
         '''一次性返回'''
         response = self.client.chat.completions.create(
             model=model,
             messages=messages,
             stream=False,
             max_tokens=max_length,
             temperature=temperature,
-            top_p=top_p
+            top_p=top_p,
+            **kwargs
             )
         content = response.choices[0].message.content
         return content
     
     def stream_chat_cli(self, *args, **kwargs):
         for token in self.stream_chat(*args, **kwargs):
             print(token, end='', flush=True)
 
 
 class ChatOpenaiClientSseclient:
     '''调用openai接口的client, 流式请求
+    
+    注意事项：部分调用时候有额外参数传入，如下：
+    >>> client = ChatOpenaiClientSseclient(url='https://chatpet.openai.azure.com/openai/deployments/chatGPT-turbo16K/chat/completions', 
+    >>>                                 header={'api-key': "填写对应的api-key"},
+    >>>                                 params={'api-version': '2023-03-15-preview'})
 
     Example
     --------------------------------------------
-    >>> messages = [
-    >>>         {"content": "你好", "role": "user"},
-    >>>         {"content": "你好，我是AI大模型，有什么可以帮助您的？", "role": "assistant"},
-    >>>         {"content": "你可以做什么？", "role": "user"}
-    >>>         ]
+    >>> body = {
+    >>>         "messages": [
+    >>>             {"content": "你好", "role": "user"},
+    >>>             {"content": "你好，我是法律大模型", "role": "assistant"},
+    >>>             {"content": "基金从业可以购买股票吗", "role": "user"}],
+    >>>         "model": "default",
+    >>>         "stream": True
+    >>>     }
+    >>>     
     >>> client = ChatOpenaiClientSseclient('http://127.0.0.1:8000')
     >>> # 测试打印
     >>> client.stream_chat_cli(body)
     >>> # 流式
     >>> for token in client.stream_chat(body):
     >>>     print(token, end='', flush=True)
     '''
-    def __init__(self, url) -> None:
+    def __init__(self, url:str, api_key:str=None, header:dict=None, params:dict=None) -> None:
         self.url = url
+        self.api_key = api_key
+        self.header = header
+        self.params = params
+
         if is_sseclient_available():
             import sseclient
         else:
-            raise ImportError('No module found, you may `pip install sseclient-py`')
+            raise ModuleNotFoundError('No module found, you may `pip install sseclient-py`')
         
         self.sseclient = sseclient
    
-    def stream_chat(self, body):
+    def stream_chat(self, body, **kwargs):
         '''接口调用'''
         reqHeaders = {'Accept': 'text/event-stream'}
-        request = requests.post(self.url, stream=True, headers=reqHeaders, json=body)
+        if self.api_key is not None:
+            reqHeaders["Authorization"] = f"Bearer {self.api_key}"
+
+        if self.header is not None:
+            reqHeaders.update(self.header)
+        
+        request = requests.post(self.url, stream=True, headers=reqHeaders, json=body, params=self.params, **kwargs)
         client = self.sseclient.SSEClient(request)
         for event in client.events():
             if event.data != '[DONE]':
                 data = json.loads(event.data)['choices'][0]['delta']
                 if 'content' in data:
                     yield data['content']
 
-    def stream_chat_cli(self, body):
+    def stream_chat_cli(self, body, **kwargs):
         '''简单测试在命令行打印'''
-        for token in self.stream_chat(body):
+        for token in self.stream_chat(body, **kwargs):
             print(token, end='', flush=True)
 
 
 def extend_with_chat_openai_api(InputModel) -> ChatOpenaiApi:
     """添加ChatWebDemo"""
     class ChatDemo(InputModel, ChatOpenaiApi):
         pass
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/fill_mask.py` & `bert4torch-0.5.0/bert4torch/pipelines/fill_mask.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/text2vec.py` & `bert4torch-0.5.0/bert4torch/pipelines/text2vec.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,26 +42,30 @@
             input_is_string = True
         
         length_sorted_idx = np.argsort([-len(s) for s in sentences])
         sentences_sorted = [sentences[idx] for idx in length_sorted_idx]
         all_embeddings = []
         for start_index in trange(0, len(sentences), batch_size, desc="Batches", disable=not show_progress_bar):
             sentences_batch = sentences_sorted[start_index: start_index + batch_size]
-            batch = self.tokenizer(sentences_batch, maxlen=max_seq_length)
-            batch_input = [torch.tensor(sequence_padding(item), dtype=torch.long, device=self.device) for item in batch]
-            output = self.model(batch_input)
+            if self.tokenizer_type == 'b4t':
+                batch_input = self.tokenizer(sentences_batch, max_length=max_seq_length, return_tensors='pt').to(self.device)
+                output = self.model(batch_input)
+            else:
+                batch_input = self.tokenizer(sentences_batch, max_length=max_seq_length, return_tensors='pt').to(self.device)
+                output = self.model(**batch_input)
 
             last_hidden_state = output.get('last_hidden_state')
             pooler = output.get('pooled_output')
             if isinstance(batch_input, list):
-                attention_mask = (batch_input[0] != self.tokenizer._token_pad_id).long()
+                attention_mask = (batch_input[0] != self.tokenizer.pad_token_id).long()
             elif isinstance(batch_input, torch.Tensor):
-                attention_mask = (batch_input != self.tokenizer._token_pad_id).long()
-            else:
-                raise TypeError('Args `batch_input` only support list(tensor)/tensor format')
+                attention_mask = (batch_input != self.tokenizer.pad_token_id).long()
+            else:  # 类似字典格式的
+                attention_mask = batch_input.get('attention_mask', (batch_input['input_ids'] != self.tokenizer.pad_token_id).long())
+
             pool_strategy = pool_strategy or self.pool_strategy
             embs = get_pool_emb(last_hidden_state, pooler, attention_mask, pool_strategy, custom_layer)
             if normalize_embeddings:
                 embs = torch.nn.functional.normalize(embs, p=2, dim=1)
             if convert_to_numpy:
                 embs = embs.cpu()
             all_embeddings.extend(embs)
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/pipelines/uie_predictor.py` & `bert4torch-0.5.0/bert4torch/pipelines/uie_predictor.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/quantization.py` & `bert4torch-0.5.0/bert4torch/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ''' 量化模块
 '''
 
 from torch.nn import Linear, Embedding
 from torch.nn.parameter import Parameter
+from torch import nn
 import torch.nn.functional as F
 import bz2
 import torch
 import base64
 import ctypes
-from typing import List
+from typing import List, Union, Dict
 import re
 from tqdm import tqdm
 from functools import partial
 import inspect
-from bert4torch.snippets import log_error
+from bert4torch.snippets import is_package_available
 
 try:
     from cpm_kernels.kernels.base import LazyKernelCModule, KernelFunction, round_up
 
     class Kernel:
         def __init__(self, code: bytes, function_names: List[str]):
             self.code = code
@@ -37,15 +38,14 @@
             "int4WeightExtractionHalf",
             "int8WeightExtractionFloat",
             "int8WeightExtractionHalf",
         ],
     )
 except Exception as exception:
     kernels = None
-    log_error("Failed to load cpm_kernels:" + str(exception))
 
 
 class W8A16Linear(torch.autograd.Function):
     @staticmethod
     def forward(ctx, inp: torch.Tensor, quant_w: torch.Tensor, scale_w: torch.Tensor, weight_bit_width):
         ctx.inp_shape = inp.size()
         ctx.weight_bit_width = weight_bit_width
@@ -218,22 +218,26 @@
         output = F.embedding(
             input, original_weight, self.padding_idx, self.max_norm,
             self.norm_type, self.scale_grad_by_freq, self.sparse
         )
         return output
 
 
-def quantize_cpm_kernels(model, quantization_bit, use_quantization_cache=False, empty_init=False, target_modules=None, **kwargs):
+def quantize_cpm_kernels(model:nn.Module, quantization_bit:int, use_quantization_cache:bool=False, 
+                         empty_init:bool=False, target_modules:Union[str, List]=None, **kwargs):
     """从chagglm-6b移植过来的的量化，方便以int8和int4进行推理
     源链接：https://huggingface.co/THUDM/chatglm-6b/blob/main/quantization.py
     
     Replace fp16 linear with quantized linear
     这里修改了hard code, 可以适配其他模型
     target_modules: str/list, 指定对某些层做量化
     """
+    if not is_package_available('cpm_kernels'):
+        raise ModuleNotFoundError('Module `cpm_kernels` not found, you may use `pip install cpm_kernels`')
+
     modules_trans = {}
     for name, module in model.named_modules():
         # target_modules=None, 表示对所有Linear层替换
         if (target_modules is None) and isinstance(module, Linear):
             modules_trans[name] = module
         elif (target_modules is not None) and isinstance(module, Linear):
             if isinstance(target_modules, str):
@@ -253,15 +257,15 @@
         bias=True,
         dtype=dtype,
         empty_init=empty_init
     )
         
     cache = dict()
     for name, module in tqdm(modules_trans.items(), desc='Quantize linear layers'):
-        cache_name = re.sub('\.[0-9]+\.', '.', name)
+        cache_name = re.sub(r'\.[0-9]+\.', '.', name)
         if use_quantization_cache and (cache_name not in cache):
             n, m = module.weight.size(0), module.weight.size(1)
             cache[cache_name] = CacheTensor(n, m, dtype=dtype, device=current_device, requires_grad=False)
 
         module_quant = QuantizedLinearWithPara(
                 weight_tensor=module.weight.to(current_device),
                 bias_tensor=module.bias,
@@ -269,25 +273,30 @@
                 out_features=module.out_features,
                 device=module.weight.device,
                 quantization_cache=cache.get(cache_name)
             )
         del module
         # 赋值
         name_new = list(name)
-        for iter_ in re.finditer('\.[0-9]+\.', name):
+        for iter_ in re.finditer(r'\.[0-9]+\.', name):
             iter_str = name[iter_.start():iter_.end()]
             name_new[iter_.start():iter_.end()] = [''] * (iter_.end()-iter_.start())
             name_new[iter_.start()] = '[' + iter_str[1:-1] + '].'
         exec('model.' + ''.join(name_new) + ' = module_quant')
     return model
 
 
-def quantize_load_in_kbit(model, load_in_8bit=False, load_in_4bit=False, keep_in_fp32_modules=None, llm_int8_skip_modules=None, quantization_config=None, **kwargs):
+def quantize_load_in_kbit(model:nn.Module, load_in_8bit:bool=False, load_in_4bit:bool=False, keep_in_fp32_modules:List=None, 
+                          llm_int8_skip_modules:List=None, quantization_config:Dict=None, **kwargs):
     '''transformer的load_in_8bit, 源自transformer源代码'''
-    from transformers.utils.bitsandbytes import replace_with_bnb_linear, set_module_quantized_tensor_to_device
+    # 兼容transformers新旧版本
+    try:
+        from transformers.integrations import replace_with_bnb_linear, set_module_quantized_tensor_to_device
+    except:
+        from transformers.utils.bitsandbytes import replace_with_bnb_linear, set_module_quantized_tensor_to_device
     from transformers.utils.quantization_config import BitsAndBytesConfig
     if quantization_config is None:
         quantization_config, kwargs = BitsAndBytesConfig.from_dict(
             config_dict={"load_in_8bit": load_in_8bit, "load_in_4bit": load_in_4bit}, return_unused_kwargs=True, **kwargs
         )
     elif quantization_config is not None:
         load_in_8bit = quantization_config.load_in_8bit
@@ -313,12 +322,12 @@
     modules_to_not_convert.extend([] if llm_int8_skip_modules is None else llm_int8_skip_modules)
 
     state_dict = model.state_dict()
     model = replace_with_bnb_linear(model, modules_to_not_convert=modules_to_not_convert, quantization_config=quantization_config)
 
     for key, param in model.named_parameters():
         if param.device == torch.device("meta"):
-            set_module_quantized_tensor_to_device(model, key, 'cpu', value=state_dict[key], fp16_statistics=None)
+            set_module_quantized_tensor_to_device(model, key, 'cpu', value=state_dict[key])
 
     model.is_loaded_in_8bit = load_in_8bit
     model.is_loaded_in_4bit = load_in_4bit
     return model
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/snippets/data_process.py` & `bert4torch-0.5.0/bert4torch/snippets/data_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import unicodedata
 import six
 import numpy as np
 import re
 import torch
 from torch.nn.utils.rnn import pad_sequence
-from typing import Optional, Union, List, Tuple
+from typing import Optional, Union, List, Tuple, Callable, Iterable, Set, Literal
 from torch4keras.snippets import log_warn
 import random
 
+
 is_py2 = six.PY2
 
 if not is_py2:
     basestring = str
 
 
 def is_string(s):
     """判断是否是字符串"""
     return isinstance(s, basestring)
     
 
-def truncate_sequences(maxlen, indices, *sequences):
+def truncate_sequences(maxlen:int, indices:Union[List[int], Tuple[int]], *sequences):
     """截断总长度至不超过maxlen"""
     sequences = [s for s in sequences if s]
     if not isinstance(indices, (list, tuple)):
         indices = [indices] * len(sequences)
 
     while True:
         lengths = [len(s) for s in sequences]
         if sum(lengths) > maxlen:
             i = np.argmax(lengths)
             sequences[i].pop(indices[i])
         else:
             return sequences
 
 
-def text_segmentate(text, maxlen, seps='\n', strips=None, truncate=True):
+def text_segmentate(text:str, maxlen:int, seps:str='\n', strips:str=None, truncate:bool=True):
     """将文本按照标点符号划分为若干个短句
        
        :param text: 待划分的句子
        :param maxlen: int, 截断长度
        :param seps: 分隔符
        :param strips: ''.strip()
        :param truncate: True表示标点符号切分后仍然超长时, 按照maxlen硬截断分成若干个短句
@@ -62,15 +63,15 @@
     elif truncate and (not seps) and (len(text) > maxlen):
         # 标点符号用完，仍然超长，且设置了truncate=True
         return [text[i*maxlen:(i+1)*maxlen] for i in range(0, int(np.ceil(len(text)/maxlen)))]
     else:
         return [text]
 
 
-def merge_segmentate(sequences, maxlen, sep=''):
+def merge_segmentate(sequences:List[str], maxlen:int, sep:str=''):
     '''把m个句子合并成不超过maxlen的n个句子, 主要用途是合并碎句子
 
     :param sequences: List(str), 短句子列表
     :param maxlen: int, 最大长度
     :param sep: str, 合并使用的分隔符, 可以是，。等标点符号
     '''
     sequences_new = []
@@ -87,15 +88,16 @@
             sequences_new.append(t)
             text = ''
     if text:
         sequences_new.append(text)
     return sequences_new
 
 
-def text_augmentation(texts, noise_dict=None, noise_len=0, noise_p=0.0, skip_words=None, strategy='random', allow_dup=True):
+def text_augmentation(texts:Union[str, List[str]], noise_dict:Union[List[str], Tuple[str], Set[str]]=None, noise_len:int=0, noise_p:float=0.0, 
+                      skip_words:Union[str, List[str]]=None, strategy:Literal['random', 'insert', 'delete', 'replace']='random', allow_dup:bool=True):
     '''简单的EDA策略, 增删改
     
     :param texts: 需要增强的文本/文本list
     :param noise_dict: 噪音数据, 元素为str的list, tuple, set
     :param noise_len: 噪音长度, 优先试用
     :param noise_p: 噪音比例
     :param skip_words: 跳过的短语, string/list
@@ -170,15 +172,15 @@
             elif random.random() < 0.667:
                 texts[id] = delete(text, sel_idx)
             else:
                 texts[id] = replace(text, sel_idx, noise_dict)
     return texts if len(texts) > 1 else texts[0]
 
 
-def lowercase_and_normalize(text, never_split=()):
+def lowercase_and_normalize(text:str, never_split:Union[Set, Tuple, List]=()):
     """转小写，并进行简单的标准化"""
     if is_py2:
         text = unicode(text)
     
     # convert non-special tokens to lowercase
     escaped_special_toks = [re.escape(s_tok) for s_tok in never_split]
     pattern = r"(" + r"|".join(escaped_special_toks) + r")|" + r"(.+?)"
@@ -186,15 +188,16 @@
 
     # text = text.lower()
     text = unicodedata.normalize('NFD', text)
     text = ''.join([ch for ch in text if unicodedata.category(ch) != 'Mn'])
     return text
 
 
-def sequence_padding(inputs, length=None, value=0, seq_dims=1, mode='post'):
+def sequence_padding(inputs:Union[List[np.ndarray], List[List], List[torch.Tensor]], length:Union[List, int]=None, 
+                     value:int=0, seq_dims:int=1, mode:Literal['pre', 'left', 'post', 'right']='post'):
     """将序列padding到同一长度"""
     if isinstance(inputs[0], (np.ndarray, list)):
         if length is None:
             length = np.max([np.shape(x)[:seq_dims] for x in inputs], axis=0)
         elif not hasattr(length, '__getitem__'):
             length = [length]
 
@@ -222,15 +225,15 @@
         if length is not None:
             inputs = [i[:length] for i in inputs]
         return pad_sequence(inputs, padding_value=value, batch_first=True)
     else:
         raise ValueError('"input" argument must be tensor/list/ndarray.')
 
 
-def parallel_apply_generator(func, iterable, workers, max_queue_size, dummy=False, random_seeds=True):
+def parallel_apply_generator(func:Callable, iterable:Iterable, workers:int, max_queue_size:int, dummy:bool=False, random_seeds:bool=True):
     """多进程或多线程地将func应用到iterable的每个元素中（直接从bert4keras中移植过来）。
     注意这个apply是异步且无序的，也就是说依次输入a,b,c，但是输出可能是func(c), func(a), func(b)。结果将作为一个
     generator返回，其中每个item是输入的序号以及该输入对应的处理结果。
     
     :param dummy: False是多进程/线性，True则是多线程/线性；
     :param random_seeds: 每个进程的随机种子。
     """
@@ -278,15 +281,15 @@
     while out_count != in_count:
         yield out_queue.get()
         out_count += 1
 
     pool.terminate()
 
 
-def parallel_apply(func, iterable, workers, max_queue_size, callback=None, dummy=False, random_seeds=True, unordered=True):
+def parallel_apply(func:Callable, iterable:Iterable, workers:int, max_queue_size:int, callback:Callable=None, dummy:bool=False, random_seeds:bool=True, unordered:bool=True):
     """多进程或多线程地将func应用到iterable的每个元素中（直接从bert4keras中移植过来）。
     注意这个apply是异步且无序的，也就是说依次输入a,b,c，但是输出可能是func(c), func(a), func(b)。
 
     :param callback: 处理单个输出的回调函数；
     :param dummy: False是多进程/线性，True则是多线程/线性；windows需设置dummy=True
     :param random_seeds: 每个进程的随机种子；
     :param unordered: 若为False，则按照输入顺序返回，仅当callback为None时生效。
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/snippets/hub.py` & `bert4torch-0.5.0/bert4torch/snippets/hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 '''下载权重和bert4torch_config.json
 '''
 
 import os
 import json
 from pathlib import Path
 from typing import Union, Optional, Dict
-from torch4keras.snippets import log_error_once, log_info_once, log_error, is_safetensors_available
+from torch4keras.snippets import log_error_once, log_info_once, log_error, is_safetensors_available, check_file_modified
 
 
 if os.environ.get('SAFETENSORS_FIRST', False):
     SAFETENSORS_BINS = ['.safetensors', '.bin']  # 优先查找safetensors格式权重
 else:
     SAFETENSORS_BINS = ['.bin', '.safetensors']  # 优先查找bin格式权重
 _CACHED_NO_EXIST = object()
@@ -159,15 +159,17 @@
                     # force_filename = filename,
                     library_name = library_name,
                     library_version = library_version,
                     user_agent = user_agent,
                 )
                 if resolved_file.endswith('config.json'):
                     storage_folder = os.path.dirname(resolved_file)
-                    log_info_once(f'Download {repo_id} to {storage_folder}')
+                    if check_file_modified(resolved_file, duration=2):
+                        # 如果文件在2s内下载的，则不打印
+                        log_info_once(f'Download {repo_id} to {storage_folder}')
             if os.path.exists(resolved_file + ".lock"):
                 os.remove(resolved_file + ".lock")
         return storage_folder
 
     # 下载指定文件
     else:
         # 从cache中恢复
@@ -190,15 +192,17 @@
                     force_download = force_download,
                     # force_filename = filename,
                     library_name = library_name,
                     library_version = library_version,
                     user_agent = user_agent,
                     endpoint = HF_ENDPOINT
                 )
-                log_info_once(f'Download {repo_id} to {resolved_file}')
+                if check_file_modified(resolved_file, duration=2):
+                    # 如果文件在2s内下载的，则不打印
+                    log_info_once(f'Download {repo_id} to {resolved_file}')
             except EntryNotFoundError:
                 log_error(
                     f"{repo_id} does not appear to have a file named {filename}. Checkout "
                     f"'https://huggingface.co/{repo_id}/tree/main' for available files."
                 )
                 resolved_file = None
         return resolved_file
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/snippets/import_utils.py` & `bert4torch-0.5.0/bert4torch/snippets/import_utils.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/snippets/misc.py` & `bert4torch-0.5.0/bert4torch/snippets/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #! -*- coding: utf-8 -*-
 '''工具函数
 '''
 
 import json
 import torch
+from torch import nn
 import gc
 import inspect
 import os
 from torch.utils.checkpoint import CheckpointFunction
 import shutil
 import re
 from torch4keras.snippets import log_info, log_warn, Timeit
@@ -286,18 +287,18 @@
         return to_ignore
 
     if src:
         os.makedirs(src, exist_ok=True)
     shutil.copytree(src, dst, ignore=_ignore_copy_files, dirs_exist_ok=dirs_exist_ok)
 
 
-def get_weight_decay_optim_groups(self, weight_decay:float) -> dict:
+def get_weight_decay_optim_groups(module:nn.Module, weight_decay:float) -> dict:
     '''获取weight_decay的参数列表'''
     # start with all of the candidate parameters
-    param_dict = {pn: p for pn, p in self.named_parameters()}
+    param_dict = {pn: p for pn, p in module.named_parameters()}
     # filter out those that do not require grad
     param_dict = {pn: p for pn, p in param_dict.items() if p.requires_grad}
     # create optim groups. Any parameters that is 2D will be weight decayed, otherwise no.
     # i.e. all weight tensors in matmuls + embeddings decay, all biases and layernorms don't.
     decay_params = [p for n, p in param_dict.items() if p.dim() >= 2]
     nodecay_params = [p for n, p in param_dict.items() if p.dim() < 2]
     optim_groups = [
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/tokenizers.py` & `bert4torch-0.5.0/bert4torch/tokenizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 '''Tokenization classes
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import collections
 import logging
-from typing import Any, Literal
+from typing import Any, Literal, List, Union
 import unicodedata
 from io import open
 from bert4torch.snippets import truncate_sequences, is_string, lowercase_and_normalize, sequence_padding
 import re
 import six
 from collections import OrderedDict
 import torch
 
 
 logger = logging.getLogger(__name__)
 is_py2 = six.PY2
 
-def load_vocab(dict_path, encoding="utf-8", simplified=False, startswith=None):
+def load_vocab(dict_path:str, encoding:str="utf-8", simplified:bool=False, startswith:List=None):
     """加载词典文件到dict"""
     token_dict = collections.OrderedDict()
     index = 0
     with open(dict_path, "r", encoding=encoding) as reader:
         while True:
             token = reader.readline()
             if not token:
@@ -108,15 +108,15 @@
 
     def _create_trie(self, unique_no_split_tokens):
         trie = Trie()
         for token in unique_no_split_tokens:
             trie.add(token)
         return trie
 
-    def tokenize(self, text, maxlen=None):
+    def tokenize(self, text:str, maxlen:int=None) -> List[str]:
         """分词函数
         """
         tokens = [self._token_translate.get(token) or token for token in self._tokenize(text)]
         if self._token_start is not None:
             tokens.insert(0, self._token_start)
         if self._token_end is not None:
             tokens.append(self._token_end)
@@ -128,15 +128,15 @@
         return tokens
 
     def token_to_id(self, token):
         """token转换为对应的id
         """
         raise NotImplementedError
 
-    def tokens_to_ids(self, tokens):
+    def tokens_to_ids(self, tokens:List[str]) -> List[int]:
         """token序列转换为对应的id序列
         """
         return [self.token_to_id(token) for token in tokens]
 
     def _encode(self, first_text, second_text=None, maxlen=None, pattern='S*E*E', truncate_from='right', return_offsets=False):
         """输出文本对应token id和segment id
         """
@@ -249,25 +249,20 @@
         """
         raise NotImplementedError
     
 
 class Tokenizer(TokenizerBase):
     """Bert原生分词器
     """
-    def __init__(self, token_dict, do_lower_case=True, do_basic_tokenize=True, do_tokenize_unk=False, **kwargs):
+    def __init__(self, token_dict:Union[str, dict], do_lower_case:bool=True, do_basic_tokenize:bool=True, do_tokenize_unk:bool=False, **kwargs):
         """
-        参数:
-            token_dict:
-                词典文件
-            do_lower_case:
-                是否转换成小写
-            do_basic_tokenize:
-                分词前，是否进行基础的分词
-            do_tokenize_unk:
-                分词后，是否生成[UNK]标记，还是在encode阶段生成
+        :param token_dict: 词典文件
+        :param do_lower_case: 是否转换成小写
+        :param do_basic_tokenize: 分词前，是否进行基础的分词
+        :param do_tokenize_unk: 分词后，是否生成[UNK]标记，还是在encode阶段生成
         """
         super(Tokenizer, self).__init__(**kwargs)
         if is_string(token_dict):
             token_dict = load_vocab(token_dict)
 
         self._do_lower_case = do_lower_case
         self._vocab_size = len(token_dict)
@@ -433,15 +428,15 @@
             for ch in Tokenizer.stem(token):
                 if (
                     Tokenizer._is_cjk_character(ch) or
                     Tokenizer._is_punctuation(ch)
                 ):
                     return True
 
-    def rematch(self, text, tokens):
+    def rematch(self, text:str, tokens:List[str]) -> List[List]:
         """给出原始的text和tokenize后的tokens的映射关系
         """
         if is_py2:
             text = unicode(text)
 
         if self._do_lower_case:
             text = text.lower()
@@ -477,15 +472,15 @@
         """Constructs a BasicTokenizer.
         Args:
           do_lower_case: Whether to lower case the input.
         """
         self.do_lower_case = do_lower_case
         self.never_split = never_split
 
-    def tokenize(self, text):
+    def tokenize(self, text:str):
         """文本切分成token"""
         text = self._clean_text(text)
         text = self._tokenize_chinese_chars(text)
         orig_tokens = whitespace_tokenize(text)
         split_tokens = []
         for token in orig_tokens:
             if self.do_lower_case and token not in self.never_split:
```

### Comparing `bert4torch-0.4.9.post2/bert4torch/trainer/dpo_trainer.py` & `bert4torch-0.5.0/bert4torch/trainer/dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/trainer/ppo_trainer.py` & `bert4torch-0.5.0/bert4torch/trainer/ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/trainer/ptuningv2_trainer.py` & `bert4torch-0.5.0/bert4torch/trainer/ptuningv2_trainer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch/trainer/sequence_classification_trainer.py` & `bert4torch-0.5.0/bert4torch/trainer/sequence_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.5.0/bert4torch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,248 +1,252 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.4.9.post2
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![bert4torch](./docs/pics/bert4torch.png)
-
-[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
-[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
-[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
-[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
-[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
-[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
-[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
-
-[Documentation](https://bert4torch.readthedocs.io) |
-[Torch4keras](https://github.com/Tongjilibo/torch4keras) |
-[Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples) |
-[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
-
-## 目录
-- [目录](#目录)
-- [1. 下载安装](#1-下载安装)
-- [2. 功能](#2-功能)
-- [3. 快速上手](#3-快速上手)
-- [4. 版本和更新历史](#4-版本和更新历史)
-  - [4.1 版本历史](#41-版本历史)
-  - [4.2 更新历史](#42-更新历史)
-- [5. 预训练权重](#5-预训练权重)
-- [6. 鸣谢](#6-鸣谢)
-- [7. 引用](#7-引用)
-- [8. 其他](#8-其他)
-  
-
-## 1. 下载安装
-
-安装稳定版
-
-```shell
-pip install bert4torch
-```
-
-安装最新版
-
-```shell
-pip install git+https://github.com/Tongjilibo/bert4torch
-```
-
-- **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
-- **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
-- **自行训练**：针对自己的数据，修改相应的数据处理代码块
-- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
-
-## 2. 功能
-- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
-- **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
-- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
-- **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/DATA.md)
-- **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
-- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
-- **训练过程**：
-
-  ```text
-  2022-10-28 23:16:10 - Start Training
-  2022-10-28 23:16:10 - Epoch: 1/2
-  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
-  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
-  test_acc: 0.98045. best_test_acc: 0.98045
-
-  2022-10-28 23:16:27 - Epoch: 2/2
-  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
-  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
-  test_acc: 0.98280. best_test_acc: 0.98280
-
-  2022-10-28 23:16:44 - Finish Training
-  ```
-
-|          功能                | bert4torch |  transformers | 备注 |
-|-----------------------------|------------|----------------|--------|
-|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
-|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
-|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
-|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
-|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
-|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
-|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
-|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
-
-
-## 3. 快速上手
-
-- [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
-- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
-- [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
-
-## 4. 版本和更新历史
-### 4.1 版本历史
-|更新日期| bert4torch | torch4keras | 版本说明 |
-|------| ---------------- | ----------------- |----------- |
-|20240317| 0.4.9.post2    | 0.2.1.post2 |增加get_weight_decay_optim_groups函数, attention中允许is_causal，修改repetition_penalty的bug，把baichuan从llama中剥离，修复config_path的bug，允许num_key_value_heads参数，[torch4keras-v0.2.1.post2](https://github.com/Tongjilibo/torch4keras/releases/tag/v0.2.1.post2)更新特性|
-|20240221| 0.4.8          | 0.2.0|fastapi发布服务允许闲时offload到cpu, `build_transformer_model`允许从hf下载, 添加`FillMask`的pipeline, 添加`SequenceClassificationTrainer`|
-|20240204| 0.4.7          | 0.1.9|修改`save_pretrained`用于保存文件夹, 增加GenerateSpeed用于统计token生成速度，修复t5在use_states=True时候的错误, 修改层次编码的bug, 增加deepseek_moe模型，修复generation并发错误，优化大模型耗时|
-|20240116| 0.4.6          | 0.1.8|bug修复，增加`save_pretrained`用于保存`transformer`格式的权重, 增加部分`embedding`模型|
-
-[更多版本](https://github.com/Tongjilibo/bert4torch/blob/master/docs/Update.md)
-
-### 4.2 更新历史
-
-[更多历史](https://github.com/Tongjilibo/bert4torch/blob/master/docs/History.md)
-
-## 5. 预训练权重
-- 预训练模型支持多种代码加载方式
-```python
-from bert4torch.models import build_transformer_model
-
-# 1. 仅指定config_path: 从头初始化模型结构, 不加载预训练模型
-model = build_transformer_model('./model/bert4torch_config.json')
-
-# 2. 仅指定checkpoint_path: 
-## 2.1 文件夹路径: 自动寻找路径下的*.bin/*.safetensors权重文件 + bert4torch_config.json/config.json文件
-model = build_transformer_model(checkpoint_path='./model')
-
-## 2.2 文件路径/列表: 文件路径即权重路径/列表, config会从同级目录下寻找
-model = build_transformer_model(checkpoint_path='./pytorch_model.bin')
-
-## 2.3 model_name: hf上预训练权重名称, 会自动下载hf权重以及bert4torch_config.json文件
-model = build_transformer_model(checkpoint_path='bert-base-chinese')
-
-# 3. 同时指定config_path和checkpoint_path(本地路径名或model_name排列组合): 
-config_path = './model/bert4torch_config.json'  # 或'bert-base-chinese'
-checkpoint_path = './model/pytorch_model.bin'  # 或'bert-base-chinese'
-model = build_transformer_model(config_path, checkpoint_path)
-```
-
-| 模型分类| 模型名称 | 权重来源| 权重链接/checkpoint_path | config_path|
-| ----- | ----- | ----- | ----- | ----- |
-| bert| bert-base-chinese| google-bert | [`bert-base-chinese`](https://huggingface.co/bert-base-chinese) | [`bert-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-chinese)|
-|     | chinese_L-12_H-768_A-12| 谷歌 | [github](https://github.com/google-research/bert), [tf](https://storage.googleapis.com/bert_models/2018_11_03/chinese_L-12_H-768_A-12.zip), [`Tongjilibo/bert-chinese_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/bert-chinese_L-12_H-768_A-12) | |
-|     | chinese-bert-wwm-ext| HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-bert-wwm-ext`](https://huggingface.co/hfl/chinese-bert-wwm-ext)| [`chinese-bert-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-bert-wwm-ext) |
-|     | bert-base-multilingual-cased| google-bert | [`bert-base-multilingual-cased`](https://huggingface.co/bert-base-multilingual-cased) | [`bert-base-multilingual-cased`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-multilingual-cased) |
-|     | macbert | HFL| [github](https://github.com/ymcui/MacBERT)，[`hfl/chinese-macbert-base`](https://huggingface.co/hfl/chinese-macbert-base), [`hfl/chinese-macbert-large`](https://huggingface.co/hfl/chinese-macbert-large) |[`chinese-macbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-base), [`chinese-macbert-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-large)|
-|     | wobert| 追一科技| [github](https://github.com/ZhuiyiTechnology/WoBERT)，[`junnyu/wobert_chinese_base`](https://huggingface.co/junnyu/wobert_chinese_base)，[`junnyu/wobert_chinese_plus_base`](https://huggingface.co/junnyu/wobert_chinese_plus_base) |[`wobert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_base), [`wobert_chinese_plus_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_plus_base)|
-|roberta|chinese-roberta-wwm-ext | HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-roberta-wwm-ext`](https://huggingface.co/hfl/chinese-roberta-wwm-ext), [`hfl/chinese-roberta-wwm-ext-large`](https://huggingface.co/hfl/chinese-roberta-wwm-ext-large) |[`chinese-roberta-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext), [`chinese-roberta-wwm-ext-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext-large) |
-|     |roberta-small/tiny| 追一科技| [github](https://github.com/ZhuiyiTechnology/pretrained-models)，[`Tongjilibo/chinese_roberta_L-4_H-312_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-4_H-312_A-12), [`Tongjilibo/chinese_roberta_L-6_H-384_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-6_H-384_A-12) | |
-|     |roberta-base| FacebookAI | [`roberta-base`](https://huggingface.co/roberta-base) | [`roberta-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roberta-base) |
-|     | guwenbert| ethanyt |[`ethanyt/guwenbert-base`](https://huggingface.co/ethanyt/guwenbert-base) | [`guwenbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/guwenbert-base)|
-| albert|albert| brightmart| [github](https://github.com/brightmart/albert_zh)，[torch](https://github.com/lonePatient/albert_pytorch), [`voidful/albert_chinese_tiny`](https://huggingface.co/voidful/albert_chinese_tiny)，[`voidful/albert_chinese_small`](https://huggingface.co/voidful/albert_chinese_small), [`voidful/albert_chinese_base`](https://huggingface.co/voidful/albert_chinese_base), [`voidful/albert_chinese_large`](https://huggingface.co/voidful/albert_chinese_large), [`voidful/albert_chinese_xlarge`](https://huggingface.co/voidful/albert_chinese_xlarge), [`voidful/albert_chinese_xxlarge`](https://huggingface.co/voidful/albert_chinese_xxlarge) | [`albert_chinese_tiny`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_tiny)，[`albert_chinese_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_small), [`albert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_base), [`albert_chinese_large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_large), [`albert_chinese_xlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xlarge), [`albert_chinese_xxlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xxlarge)|
-| nezha|NEZHA | 华为| [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-PyTorch)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch), [`sijunhe/nezha-cn-base`](https://huggingface.co/sijunhe/nezha-cn-base), [`sijunhe/nezha-cn-large`](https://huggingface.co/sijunhe/nezha-cn-large), [`sijunhe/nezha-base-wwm`](https://huggingface.co/sijunhe/nezha-base-wwm), [`sijunhe/nezha-large-wwm`](https://huggingface.co/sijunhe/nezha-large-wwm)|[`nezha-cn-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-base), [`nezha-cn-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-large), [`nezha-base-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-base-wwm), [`nezha-large-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-large-wwm)|
-|      |nezha_gpt_dialog| bojone| [github](https://github.com/bojone/nezha_gpt_dialog), [`Tongjilibo/nezha_gpt_dialog`](https://huggingface.co/Tongjilibo/nezha_gpt_dialog) | |
-| xlnet|chinese-xlnet | HFL | [github](https://github.com/ymcui/Chinese-XLNet), [`hfl/chinese-xlnet-base`](https://huggingface.co/hfl/chinese-xlnet-base) | [`chinese-xlnet-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-xlnet-base)|
-||tranformer_xl|huggingface|[`transfo-xl/transfo-xl-wt103`](https://huggingface.co/transfo-xl/transfo-xl-wt103)|[`transfo-xl-wt103`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/transfo-xl-wt103)|
-|deberta| Erlangshen-DeBERTa-v2| IDEA | [`IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese) |[`Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-97M-Chinese), [`Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-320M-Chinese), [`Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-710M-Chinese) |
-| electra|Chinese-ELECTRA | HFL | [github](https://github.com/ymcui/Chinese-ELECTRA)，[`hfl/chinese-electra-base-discriminator`](https://huggingface.co/hfl/chinese-electra-base-discriminator) |[`chinese-electra-base-discriminator`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-electra-base-discriminator)|
-| ernie|ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[`nghuyong/ernie-1.0-base-zh`](https://huggingface.co/nghuyong/ernie-1.0-base-zh), [`nghuyong/ernie-3.0-base-zh`](https://huggingface.co/nghuyong/ernie-3.0-base-zh)| [`ernie-1.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-1.0-base-zh), [`ernie-3.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-3.0-base-zh)|
-| roformer|roformer| 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer)，[`junnyu/roformer_chinese_base`](https://huggingface.co/junnyu/roformer_chinese_base) |[`roformer_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_base) |
-|         |roformer_v2 | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-v2)，[`junnyu/roformer_v2_chinese_char_base`](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)|[`roformer_v2_chinese_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_v2_chinese_char_base) |
-| simbert|simbert | 追一科技| [github](https://github.com/ZhuiyiTechnology/simbert)，[`Tongjilibo/simbert-chinese-base`](https://huggingface.co/Tongjilibo/simbert-chinese-base), [`Tongjilibo/simbert-chinese-small`](https://huggingface.co/Tongjilibo/simbert-chinese-small), [`Tongjilibo/simbert-chinese-tiny`](https://huggingface.co/Tongjilibo/simbert-chinese-tiny) | |
-|        |simbert_v2/roformer-sim | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-sim)，[`junnyu/roformer_chinese_sim_char_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)，[`junnyu/roformer_chinese_sim_char_ft_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_base)，[`junnyu/roformer_chinese_sim_char_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_small)，[`junnyu/roformer_chinese_sim_char_ft_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_small)|[`roformer_chinese_sim_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_base), [`roformer_chinese_sim_char_ft_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_base), [`roformer_chinese_sim_char_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_small), [`roformer_chinese_sim_char_ft_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_small) |
-| gau|GAU-alpha | 追一科技| [github](https://github.com/ZhuiyiTechnology/GAU-alpha), [`Tongjilibo/chinese_GAU-alpha-char_L-24_H-768`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12) | |
-| uie| uie | 百度| [github](https://github.com/universal-ie/UIE), [torch](https://github.com/HUSTAI/uie_pytorch), [`Tongjilibo/uie-base`](https://huggingface.co/Tongjilibo/uie-base) | |
-| gpt |CDial-GPT| thu-coai| [github](https://github.com/thu-coai/CDial-GPT), [`thu-coai/CDial-GPT_LCCC-base`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base), [`thu-coai/CDial-GPT_LCCC-large`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [`CDial-GPT_LCCC-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-base), [`CDial-GPT_LCCC-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-large) |
-|     | cmp_lm(26亿)|清华 | [github](https://github.com/TsinghuaAI/CPM-1-Generate), [`TsinghuaAI/CPM-Generate`](https://huggingface.co/TsinghuaAI/CPM-Generate) | [`CPM-Generate`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CPM-Generate) |
-|     |nezha_gen|huawei_noah|[github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow), [`Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12)|
-|     | gpt2-chinese-cluecorpussmall|UER | [`uer/gpt2-chinese-cluecorpussmall`](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [`gpt2-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-chinese-cluecorpussmall)|
-|     | gpt2-ml|imcaspar | [tf](https://github.com/imcaspar/gpt2-ml), [torch](https://github.com/ghosthamlet/gpt2-ml-torch), [BaiduYun(84dh)](https://pan.baidu.com/s/16tL4Bmoh6jPy0cOND0YyeA) | [`gpt2-ml_15g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_15g_corpus), [`gpt2-ml_30g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_30g_corpus) |
-| bart| bart_base_chinese|复旦fnlp| [github](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [`fnlp/bart-base-chinese`](https://huggingface.co/fnlp/bart-base-chinese/tree/main)| [`bart-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese), [`bart-base-chinese-v1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese-v1.0) |
-| t5  | t5| UER | [`uer/t5-small-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall), [`uer/t5-base-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [`t5-base-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-base-chinese-cluecorpussmall), [`t5-small-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-small-chinese-cluecorpussmall)|
-|     | mt5 | 谷歌| [`google/mt5-base`](https://huggingface.co/google/mt5-base)| [`mt5-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/mt5-base)|
-|     | t5_pegasus| 追一科技| [github](https://github.com/ZhuiyiTechnology/t5-pegasus), [`Tongjilibo/chinese_t5_pegasus_small`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_small), [`Tongjilibo/chinese_t5_pegasus_base`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_base)| |
-|     | chatyuan v1&v2| clue-ai | [github](https://github.com/clue-ai/ChatYuan), [`ClueAI/ChatYuan-large-v1`](https://huggingface.co/ClueAI/ChatYuan-large-v1), [`ClueAI/ChatYuan-large-v2`](https://huggingface.co/ClueAI/ChatYuan-large-v2)| [`ChatYuan-large-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v1), [`ChatYuan-large-v2`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v2)|
-|     | PromptCLUE| clue-ai | [github](https://github.com/clue-ai/PromptCLUE), [`ClueAI/PromptCLUE-base`](https://huggingface.co/ClueAI/PromptCLUE-base) | [`PromptCLUE-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/PromptCLUE-base)|
-| chatglm   |chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [`THUDM/chatglm-6b`](https://huggingface.co/THUDM/chatglm-6b), [`THUDM/chatglm-6b-int8`](https://huggingface.co/THUDM/chatglm-6b-int8), [`THUDM/chatglm-6b-int4`](https://huggingface.co/THUDM/chatglm-6b-int4), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0) | [`chatglm-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b), [`chatglm-6b-int8`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int8), [`chatglm-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int4), [`chatglm-6b-v0.1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-v0.1.0) |
-|       |chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [`THUDM/chatglm2-6b`](https://huggingface.co/THUDM/chatglm2-6b), [`THUDM/chatglm2-6b-int4`](https://huggingface.co/THUDM/chatglm2-6b-int4), [`THUDM/chatglm2-6b-32k`](https://huggingface.co/THUDM/chatglm2-6b-32k) | [`chatglm2-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b), [`chatglm2-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-int4), [`chatglm2-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-32k) |
-|       |chatglm3-6b | THUDM | [github](https://github.com/THUDM/ChatGLM3), [`THUDM/chatglm3-6b`](https://huggingface.co/THUDM/chatglm3-6b), [`THUDM/chatglm3-6b-32k`](https://huggingface.co/THUDM/chatglm3-6b-32k) | [`chatglm3-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b), [`chatglm3-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b-32k) |
-| llama | llama | meta| [github](https://github.com/facebookresearch/llama) | [`llama-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-7b), [`llama-13b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-13b)|
-|       | llama-2 | meta| [github](https://github.com/facebookresearch/llama), [meta-llama/Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf), [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [meta-llama/Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf), [meta-llama/Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [`Llama-2-7b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-hf), [`Llama-2-7b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-chat-hf), [`Llama-2-13b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-hf), [`Llama-2-13b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-chat-hf)|
-|       | chinese_llama_alpaca|HFL|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[`chinese_alpaca_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_alpaca_plus_7b), [`chinese_llama_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_llama_plus_7b)|
-|       | Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [BelleGroup/BELLE-LLaMA-7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[`BELLE-LLaMA-7B-2M-enc`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/BELLE-LLaMA-7B-2M-enc)|
-|       | Ziya | IDEA-CCNL | [IDEA-CCNL/Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [IDEA-CCNL/Ziya-LLaMA-13B-v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [`Ziya-LLaMA-13B-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1), [`Ziya-LLaMA-13B-v1.1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1.1) |
-|       | Baichuan | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan), [`baichuan-inc/Baichuan-7B`](https://huggingface.co/baichuan-inc/Baichuan-7B), [`baichuan-inc/Baichuan-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [`baichuan-inc/Baichuan-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [`Baichuan-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-7B), [`Baichuan-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Base), [`Baichuan-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Chat) |
-|       | Baichuan2 | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan2), [`baichuan-inc/Baichuan2-7B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base), [`baichuan-inc/Baichuan2-7B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Chat), [`baichuan-inc/Baichuan2-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Base), [`baichuan-inc/Baichuan2-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Chat) | [`Baichuan2-7B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Base), [`Baichuan2-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Chat), [`Baichuan2-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Base), [`Baichuan2-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Chat) |
-|       | vicuna | lmsys| [`lmsys/vicuna-7b-v1.5`](https://huggingface.co/lmsys/vicuna-7b-v1.5) | [`vicuna-7b-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/vicuna-7b-v1.5)|
-|       | Yi | 01-ai| [github](https://github.com/01-ai/Yi), [`01-ai/Yi-6B`](https://huggingface.co/01-ai/Yi-6B), [`01-ai/Yi-6B-200K`](https://huggingface.co/01-ai/Yi-6B-200K) | [`Yi-6B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B), [`Yi-6B-200K`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B-200K)|
-| bloom |bloom | bigscience | [`bigscience/bloom-560m`](https://huggingface.co/bigscience/bloom-560m), [`bigscience/bloomz-560m`](https://huggingface.co/bigscience/bloomz-560m) | [`bloom-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloom-560m), [`bloomz-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloomz-560m) |
-| Qwen  |Qwen | 阿里云 | [github](https://github.com/QwenLM/Qwen-7B), [`Qwen/Qwen-1_8B`](https://huggingface.co/Qwen/Qwen-1_8B), [`Qwen/Qwen-1_8B-Chat`](https://huggingface.co/Qwen/Qwen-1_8B-Chat), [`Qwen/Qwen-7B`](https://huggingface.co/Qwen/Qwen-7B), [`Qwen/Qwen-7B-Chat`](https://huggingface.co/Qwen/Qwen-7B-Chat) | [`Qwen-1_8B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B), [`Qwen-1_8B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B-Chat), [`Qwen-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B), [`Qwen-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B-Chat) |
-| InternLM|InternLM | 上海人工智能实验室 | [github](https://github.com/InternLM/InternLM), [`internlm/internlm-chat-7b`](https://huggingface.co/internlm/internlm-chat-7b), [`internlm/internlm-7b`](https://huggingface.co/internlm/internlm-7b) | [`internlm-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-7b), [`internlm-chat-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-chat-7b)|
-| Falcon|Falcon | tiiuae | [hf](https://huggingface.co/tiiuae), [`tiiuae/falcon-rw-1b`](https://huggingface.co/tiiuae/falcon-rw-1b), [`tiiuae/falcon-7b`](https://huggingface.co/tiiuae/falcon-7b), [`tiiuae/falcon-7b-instruct`](https://huggingface.co/tiiuae/falcon-7b-instruct) | [`falcon-rw-1b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-rw-1b), [`falcon-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b), [`falcon-7b-instruct`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b-instruct) |
-|  moe  |deeoseek-moe|deepseek| [github](https://github.com/deepseek-ai/DeepSeek-MoE), [`deepseek-ai/deepseek-moe-16b-base`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-base), [`deepseek-ai/deepseek-moe-16b-chat`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-chat) | [`deepseek-moe-16b-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-base), [`deepseek-moe-16b-chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-chat) |
-| embedding| text2vec-base-chinese |shibing624| [`shibing624/text2vec-base-chinese`](https://huggingface.co/shibing624/text2vec-base-chinese) |[`text2vec-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/text2vec-base-chinese) |
-|          | m3e |moka-ai| [`moka-ai/m3e-base`](https://huggingface.co/moka-ai/m3e-base) |[`m3e-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/m3e-base)|
-|          | bge |BAAI| [`BAAI/bge-large-en-v1.5`](https://huggingface.co/BAAI/bge-large-en-v1.5), [`BAAI/bge-large-zh-v1.5`](https://huggingface.co/BAAI/bge-large-zh-v1.5) | [`bge-large-en-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-en-v1.5), [`bge-large-zh-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-zh-v1.5)|
-|          | gte |thenlper| [`thenlper/gte-large-zh`](https://huggingface.co/thenlper/gte-large-zh), [`thenlper/gte-base-zh`](https://huggingface.co/thenlper/gte-base-zh) |[`gte-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-base-zh), [`gte-large-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-large-zh)|
-
-*注：
-1. `高亮格式`(如`bert-base-chinese`)的表示可直接`build_transformer_model()`联网下载
-2. 国内镜像网站加速下载
-   - `HF_ENDPOINT=https://hf-mirror.com python your_script.py`
-   - `export HF_ENDPOINT=https://hf-mirror.com`后再执行python代码
-   - 在python代码开头如下设置
-    ```python
-    import os
-    os.environ['HF_ENDPOINT'] = "https://hf-mirror.com"
-    ```
-
-## 6. 鸣谢
-
-- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
-- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
-
-## 7. 引用
-
-```
-@misc{bert4torch,
-  title={bert4torch},
-  author={Bo Li},
-  year={2022},
-  howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
-}
-```
-
-## 8. 其他
-
-- Wechat & Star History Chart
-
-<table border="0">
-  <tbody>
-    <tr align="center" >
-      <td>
-         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信号</a> 
-      </td>
-      <td>
-         <a href="https://github.com/Tongjilibo"><img width="190" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
-         <a href="https://github.com/Tongjilibo">微信群</a> 
-      </td>
-      <td>
-         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
-         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
-      </td>    
-      </tr>
-  </tbody>
-</table>
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.5.0
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: torch>1.6
+Requires-Dist: torch4keras==0.2.2
+Requires-Dist: six
+
+![bert4torch](./docs/pics/bert4torch.png)
+
+[![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
+[![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
+[![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
+[![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
+[![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/bert4torch.svg)](https://github.com/Tongjilibo/bert4torch/issues)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/bert4torch/issues)
+[![Generic badge](https://img.shields.io/badge/wechat-join-green.svg?logo=wechat)](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/wechat_group.jpg)
+
+[Documentation](https://bert4torch.readthedocs.io) |
+[Torch4keras](https://github.com/Tongjilibo/torch4keras) |
+[Examples](https://github.com/Tongjilibo/bert4torch/blob/master/examples) |
+[build_MiniLLM_from_scratch](https://github.com/Tongjilibo/build_MiniLLM_from_scratch)
+
+## 目录
+- [目录](#目录)
+- [1. 下载安装](#1-下载安装)
+- [2. 功能](#2-功能)
+- [3. 快速上手](#3-快速上手)
+- [4. 版本和更新历史](#4-版本和更新历史)
+  - [4.1 版本历史](#41-版本历史)
+  - [4.2 更新历史](#42-更新历史)
+- [5. 预训练权重](#5-预训练权重)
+- [6. 鸣谢](#6-鸣谢)
+- [7. 引用](#7-引用)
+- [8. 其他](#8-其他)
+  
+
+## 1. 下载安装
+
+安装稳定版
+
+```shell
+pip install bert4torch
+```
+
+安装最新版
+
+```shell
+pip install git+https://github.com/Tongjilibo/bert4torch
+```
+
+- **注意事项**：pip包的发布慢于git上的开发版本，git clone**注意引用路径**，注意权重是否需要转换
+- **测试用例**：`git clone https://github.com/Tongjilibo/bert4torch`，修改example中的预训练模型文件路径和数据路径即可启动脚本
+- **自行训练**：针对自己的数据，修改相应的数据处理代码块
+- **开发环境**：原使用`torch==1.10`版本进行开发，现已切换到`torch2.0`开发，如其他版本遇到不适配，欢迎反馈
+
+## 2. 功能
+- **LLM模型**: 加载chatglm、llama、 baichuan、ziya、bloom等开源大模型权重进行推理和微调
+- **核心功能**：加载bert、roberta、albert、xlnet、nezha、bart、RoFormer、RoFormer_V2、ELECTRA、GPT、GPT2、T5、GAU-alpha、ERNIE等预训练权重继续进行finetune、并支持在bert基础上灵活定义自己模型
+- [**丰富示例**](https://github.com/Tongjilibo/bert4torch/blob/master/examples/)：包含[llm](https://github.com/Tongjilibo/bert4torch/blob/master/examples/llm)、[pretrain](https://github.com/Tongjilibo/bert4torch/blob/master/examples/pretrain)、[sentence_classfication](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sentence_classfication)、[sentence_embedding](https://github.com/Tongjilibo/bert4torch/tree/master/examples/sentence_embedding)、[sequence_labeling](https://github.com/Tongjilibo/bert4torch/blob/master/examples/sequence_labeling)、[relation_extraction](https://github.com/Tongjilibo/bert4torch/blob/master/examples/relation_extraction)、[seq2seq](https://github.com/Tongjilibo/bert4torch/blob/master/examples/seq2seq)、[serving](https://github.com/Tongjilibo/bert4torch/blob/master/examples/serving/)等多种解决方案
+- **实验验证**：已在公开数据集实验验证，使用如下[examples数据集](https://github.com/Tongjilibo/bert4torch/blob/master/examples/DATA.md)
+- **易用trick**：集成了常见的[trick](https://github.com/Tongjilibo/bert4torch/blob/master/examples/training_trick)，即插即用
+- **其他特性**：[加载transformers库模型](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/tutorials_load_transformers_model.py)一起使用；调用方式简洁高效；有训练进度条动态展示；配合torchinfo打印参数量；默认Logger和Tensorboard简便记录训练过程；自定义fit过程，满足高阶需求
+- **训练过程**：
+
+  ```text
+  2022-10-28 23:16:10 - Start Training
+  2022-10-28 23:16:10 - Epoch: 1/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.1351 - acc: 0.9601
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 798.09it/s] 
+  test_acc: 0.98045. best_test_acc: 0.98045
+
+  2022-10-28 23:16:27 - Epoch: 2/2
+  5000/5000 [==============================] - 13s 3ms/step - loss: 0.0465 - acc: 0.9862
+  Evaluate: 100%|██████████████████████████████████████████████████| 2500/2500 [00:03<00:00, 635.78it/s] 
+  test_acc: 0.98280. best_test_acc: 0.98280
+
+  2022-10-28 23:16:44 - Finish Training
+  ```
+
+|          功能                | bert4torch |  transformers | 备注 |
+|-----------------------------|------------|----------------|--------|
+|训练进度条                     | ✅         |      ✅        |进度条打印loss和定义的metrics|
+|分布式训练dp/ddp               | ✅         |      ✅        |torch自带dp/ddp|
+|各类callbacks                 | ✅         |      ✅        |日志/tensorboard/earlystop/wandb等|
+|大模型推理，stream/batch输出    | ✅         |      ✅        |各个模型是通用的，无需单独维护脚本|
+|大模型微调                     | ✅         |      ✅        |lora依赖peft库，pv2自带|
+|丰富tricks                    | ✅         |      ❌        |对抗训练等tricks即插即用|
+|代码简洁易懂，自定义空间大        | ✅         |      ❌        |代码复用度高, keras代码训练风格|
+|仓库的维护能力/影响力/使用量/兼容性| ❌         |      ✅        |目前仓库个人维护|
+
+
+## 3. 快速上手
+
+- [Quick-Start](https://bert4torch.readthedocs.io/en/latest//Quick-Start.html)
+- [快速上手教程](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials/README.md)，[教程示例](https://github.com/Tongjilibo/bert4torch/blob/master//tutorials)，[实战示例](https://github.com/Tongjilibo/bert4torch/blob/master/examples)
+- [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
+
+## 4. 版本和更新历史
+### 4.1 版本历史
+|更新日期| bert4torch | torch4keras | 版本说明 |
+|------| ---------------- | ----------------- |----------- |
+|20240418| 0.5.0          | 0.2.2 | 修复chatglm3的bug, 修复save_pretrained时多文件的bug，增加CausalLMLoss, 修改deepspeed的传参逻辑，修改Text2Vec的bug, 完善openai client, 增加get_weight_decay_optim_groups|
+|20240317| 0.4.9.post2    | 0.2.1.post2 |增加get_weight_decay_optim_groups函数, attention中允许is_causal，修改repetition_penalty的bug，把baichuan从llama中剥离，修复config_path的bug，允许num_key_value_heads参数，[torch4keras-v0.2.1.post2](https://github.com/Tongjilibo/torch4keras/releases/tag/v0.2.1.post2)更新特性|
+|20240221| 0.4.8          | 0.2.0|fastapi发布服务允许闲时offload到cpu, `build_transformer_model`允许从hf下载, 添加`FillMask`的pipeline, 添加`SequenceClassificationTrainer`|
+
+[更多版本](https://github.com/Tongjilibo/bert4torch/blob/master/docs/Update.md)
+
+### 4.2 更新历史
+
+[更多历史](https://github.com/Tongjilibo/bert4torch/blob/master/docs/History.md)
+
+## 5. 预训练权重
+- 预训练模型支持多种代码加载方式
+```python
+from bert4torch.models import build_transformer_model
+
+# 1. 仅指定config_path: 从头初始化模型结构, 不加载预训练模型
+model = build_transformer_model('./model/bert4torch_config.json')
+
+# 2. 仅指定checkpoint_path: 
+## 2.1 文件夹路径: 自动寻找路径下的*.bin/*.safetensors权重文件 + bert4torch_config.json/config.json文件
+model = build_transformer_model(checkpoint_path='./model')
+
+## 2.2 文件路径/列表: 文件路径即权重路径/列表, config会从同级目录下寻找
+model = build_transformer_model(checkpoint_path='./pytorch_model.bin')
+
+## 2.3 model_name: hf上预训练权重名称, 会自动下载hf权重以及bert4torch_config.json文件
+model = build_transformer_model(checkpoint_path='bert-base-chinese')
+
+# 3. 同时指定config_path和checkpoint_path(本地路径名或model_name排列组合): 
+config_path = './model/bert4torch_config.json'  # 或'bert-base-chinese'
+checkpoint_path = './model/pytorch_model.bin'  # 或'bert-base-chinese'
+model = build_transformer_model(config_path, checkpoint_path)
+```
+
+| 模型分类| 模型名称 | 权重来源| 权重链接/checkpoint_path | config_path|
+| ----- | ----- | ----- | ----- | ----- |
+| bert| bert-base-chinese| google-bert | [`bert-base-chinese`](https://huggingface.co/bert-base-chinese) | [`bert-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-chinese)|
+|     | chinese_L-12_H-768_A-12| 谷歌 | [github](https://github.com/google-research/bert), [tf](https://storage.googleapis.com/bert_models/2018_11_03/chinese_L-12_H-768_A-12.zip), [`Tongjilibo/bert-chinese_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/bert-chinese_L-12_H-768_A-12) | |
+|     | chinese-bert-wwm-ext| HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-bert-wwm-ext`](https://huggingface.co/hfl/chinese-bert-wwm-ext)| [`chinese-bert-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-bert-wwm-ext) |
+|     | bert-base-multilingual-cased| google-bert | [`bert-base-multilingual-cased`](https://huggingface.co/bert-base-multilingual-cased) | [`bert-base-multilingual-cased`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bert-base-multilingual-cased) |
+|     | macbert | HFL| [github](https://github.com/ymcui/MacBERT)，[`hfl/chinese-macbert-base`](https://huggingface.co/hfl/chinese-macbert-base), [`hfl/chinese-macbert-large`](https://huggingface.co/hfl/chinese-macbert-large) |[`chinese-macbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-base), [`chinese-macbert-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-macbert-large)|
+|     | wobert| 追一科技| [github](https://github.com/ZhuiyiTechnology/WoBERT)，[`junnyu/wobert_chinese_base`](https://huggingface.co/junnyu/wobert_chinese_base)，[`junnyu/wobert_chinese_plus_base`](https://huggingface.co/junnyu/wobert_chinese_plus_base) |[`wobert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_base), [`wobert_chinese_plus_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/wobert_chinese_plus_base)|
+|roberta|chinese-roberta-wwm-ext | HFL | [github](https://github.com/ymcui/Chinese-BERT-wwm)，[`hfl/chinese-roberta-wwm-ext`](https://huggingface.co/hfl/chinese-roberta-wwm-ext), [`hfl/chinese-roberta-wwm-ext-large`](https://huggingface.co/hfl/chinese-roberta-wwm-ext-large) |[`chinese-roberta-wwm-ext`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext), [`chinese-roberta-wwm-ext-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-roberta-wwm-ext-large) |
+|     |roberta-small/tiny| 追一科技| [github](https://github.com/ZhuiyiTechnology/pretrained-models)，[`Tongjilibo/chinese_roberta_L-4_H-312_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-4_H-312_A-12), [`Tongjilibo/chinese_roberta_L-6_H-384_A-12`](https://huggingface.co/Tongjilibo/chinese_roberta_L-6_H-384_A-12) | |
+|     |roberta-base| FacebookAI | [`roberta-base`](https://huggingface.co/roberta-base) | [`roberta-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roberta-base) |
+|     | guwenbert| ethanyt |[`ethanyt/guwenbert-base`](https://huggingface.co/ethanyt/guwenbert-base) | [`guwenbert-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/guwenbert-base)|
+| albert|albert| brightmart| [github](https://github.com/brightmart/albert_zh)，[torch](https://github.com/lonePatient/albert_pytorch), [`voidful/albert_chinese_tiny`](https://huggingface.co/voidful/albert_chinese_tiny)，[`voidful/albert_chinese_small`](https://huggingface.co/voidful/albert_chinese_small), [`voidful/albert_chinese_base`](https://huggingface.co/voidful/albert_chinese_base), [`voidful/albert_chinese_large`](https://huggingface.co/voidful/albert_chinese_large), [`voidful/albert_chinese_xlarge`](https://huggingface.co/voidful/albert_chinese_xlarge), [`voidful/albert_chinese_xxlarge`](https://huggingface.co/voidful/albert_chinese_xxlarge) | [`albert_chinese_tiny`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_tiny)，[`albert_chinese_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_small), [`albert_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_base), [`albert_chinese_large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_large), [`albert_chinese_xlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xlarge), [`albert_chinese_xxlarge`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/albert_chinese_xxlarge)|
+| nezha|NEZHA | 华为| [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-PyTorch)，[torch](https://github.com/lonePatient/NeZha_Chinese_PyTorch), [`sijunhe/nezha-cn-base`](https://huggingface.co/sijunhe/nezha-cn-base), [`sijunhe/nezha-cn-large`](https://huggingface.co/sijunhe/nezha-cn-large), [`sijunhe/nezha-base-wwm`](https://huggingface.co/sijunhe/nezha-base-wwm), [`sijunhe/nezha-large-wwm`](https://huggingface.co/sijunhe/nezha-large-wwm)|[`nezha-cn-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-base), [`nezha-cn-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-cn-large), [`nezha-base-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-base-wwm), [`nezha-large-wwm`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/nezha-large-wwm)|
+|      |nezha_gpt_dialog| bojone| [github](https://github.com/bojone/nezha_gpt_dialog), [`Tongjilibo/nezha_gpt_dialog`](https://huggingface.co/Tongjilibo/nezha_gpt_dialog) | |
+| xlnet|chinese-xlnet | HFL | [github](https://github.com/ymcui/Chinese-XLNet), [`hfl/chinese-xlnet-base`](https://huggingface.co/hfl/chinese-xlnet-base) | [`chinese-xlnet-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-xlnet-base)|
+||tranformer_xl|huggingface|[`transfo-xl/transfo-xl-wt103`](https://huggingface.co/transfo-xl/transfo-xl-wt103)|[`transfo-xl-wt103`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/transfo-xl-wt103)|
+|deberta| Erlangshen-DeBERTa-v2| IDEA | [`IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-97M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-320M-Chinese), [`IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/IDEA-CCNL/Erlangshen-DeBERTa-v2-710M-Chinese) |[`Erlangshen-DeBERTa-v2-97M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-97M-Chinese), [`Erlangshen-DeBERTa-v2-320M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-320M-Chinese), [`Erlangshen-DeBERTa-v2-710M-Chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Erlangshen-DeBERTa-v2-710M-Chinese) |
+| electra|Chinese-ELECTRA | HFL | [github](https://github.com/ymcui/Chinese-ELECTRA)，[`hfl/chinese-electra-base-discriminator`](https://huggingface.co/hfl/chinese-electra-base-discriminator) |[`chinese-electra-base-discriminator`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese-electra-base-discriminator)|
+| ernie|ernie | 百度文心| [paddle](https://github.com/PaddlePaddle/ERNIE)，[`nghuyong/ernie-1.0-base-zh`](https://huggingface.co/nghuyong/ernie-1.0-base-zh), [`nghuyong/ernie-3.0-base-zh`](https://huggingface.co/nghuyong/ernie-3.0-base-zh)| [`ernie-1.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-1.0-base-zh), [`ernie-3.0-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ernie-3.0-base-zh)|
+| roformer|roformer| 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer)，[`junnyu/roformer_chinese_base`](https://huggingface.co/junnyu/roformer_chinese_base) |[`roformer_chinese_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_base) |
+|         |roformer_v2 | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-v2)，[`junnyu/roformer_v2_chinese_char_base`](https://huggingface.co/junnyu/roformer_v2_chinese_char_base)|[`roformer_v2_chinese_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_v2_chinese_char_base) |
+| simbert|simbert | 追一科技| [github](https://github.com/ZhuiyiTechnology/simbert)，[`Tongjilibo/simbert-chinese-base`](https://huggingface.co/Tongjilibo/simbert-chinese-base), [`Tongjilibo/simbert-chinese-small`](https://huggingface.co/Tongjilibo/simbert-chinese-small), [`Tongjilibo/simbert-chinese-tiny`](https://huggingface.co/Tongjilibo/simbert-chinese-tiny) | |
+|        |simbert_v2/roformer-sim | 追一科技| [github](https://github.com/ZhuiyiTechnology/roformer-sim)，[`junnyu/roformer_chinese_sim_char_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_base)，[`junnyu/roformer_chinese_sim_char_ft_base`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_base)，[`junnyu/roformer_chinese_sim_char_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_small)，[`junnyu/roformer_chinese_sim_char_ft_small`](https://huggingface.co/junnyu/roformer_chinese_sim_char_ft_small)|[`roformer_chinese_sim_char_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_base), [`roformer_chinese_sim_char_ft_base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_base), [`roformer_chinese_sim_char_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_small), [`roformer_chinese_sim_char_ft_small`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/roformer_chinese_sim_char_ft_small) |
+| gau|GAU-alpha | 追一科技| [github](https://github.com/ZhuiyiTechnology/GAU-alpha), [`Tongjilibo/chinese_GAU-alpha-char_L-24_H-768`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12) | |
+| uie| uie | 百度| [github](https://github.com/universal-ie/UIE), [torch](https://github.com/HUSTAI/uie_pytorch), [`Tongjilibo/uie-base`](https://huggingface.co/Tongjilibo/uie-base) | |
+| gpt |CDial-GPT| thu-coai| [github](https://github.com/thu-coai/CDial-GPT), [`thu-coai/CDial-GPT_LCCC-base`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base), [`thu-coai/CDial-GPT_LCCC-large`](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [`CDial-GPT_LCCC-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-base), [`CDial-GPT_LCCC-large`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CDial-GPT_LCCC-large) |
+|     | cmp_lm(26亿)|清华 | [github](https://github.com/TsinghuaAI/CPM-1-Generate), [`TsinghuaAI/CPM-Generate`](https://huggingface.co/TsinghuaAI/CPM-Generate) | [`CPM-Generate`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/CPM-Generate) |
+|     |nezha_gen|huawei_noah|[github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/NEZHA-Gen-TensorFlow), [`Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12`](https://huggingface.co/Tongjilibo/chinese_nezha_gpt_L-12_H-768_A-12)|
+|     | gpt2-chinese-cluecorpussmall|UER | [`uer/gpt2-chinese-cluecorpussmall`](https://huggingface.co/uer/gpt2-chinese-cluecorpussmall) | [`gpt2-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-chinese-cluecorpussmall)|
+|     | gpt2-ml|imcaspar | [tf](https://github.com/imcaspar/gpt2-ml), [torch](https://github.com/ghosthamlet/gpt2-ml-torch), [BaiduYun(84dh)](https://pan.baidu.com/s/16tL4Bmoh6jPy0cOND0YyeA) | [`gpt2-ml_15g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_15g_corpus), [`gpt2-ml_30g_corpus`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gpt2-ml_30g_corpus) |
+| bart| bart_base_chinese|复旦fnlp| [github](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [`fnlp/bart-base-chinese`](https://huggingface.co/fnlp/bart-base-chinese/tree/main)| [`bart-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese), [`bart-base-chinese-v1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bart-base-chinese-v1.0) |
+| t5  | t5| UER | [`uer/t5-small-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-small-chinese-cluecorpussmall), [`uer/t5-base-chinese-cluecorpussmall`](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall) | [`t5-base-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-base-chinese-cluecorpussmall), [`t5-small-chinese-cluecorpussmall`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/t5-small-chinese-cluecorpussmall)|
+|     | mt5 | 谷歌| [`google/mt5-base`](https://huggingface.co/google/mt5-base)| [`mt5-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/mt5-base)|
+|     | t5_pegasus| 追一科技| [github](https://github.com/ZhuiyiTechnology/t5-pegasus), [`Tongjilibo/chinese_t5_pegasus_small`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_small), [`Tongjilibo/chinese_t5_pegasus_base`](https://huggingface.co/Tongjilibo/chinese_t5_pegasus_base)| |
+|     | chatyuan v1&v2| clue-ai | [github](https://github.com/clue-ai/ChatYuan), [`ClueAI/ChatYuan-large-v1`](https://huggingface.co/ClueAI/ChatYuan-large-v1), [`ClueAI/ChatYuan-large-v2`](https://huggingface.co/ClueAI/ChatYuan-large-v2)| [`ChatYuan-large-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v1), [`ChatYuan-large-v2`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/ChatYuan-large-v2)|
+|     | PromptCLUE| clue-ai | [github](https://github.com/clue-ai/PromptCLUE), [`ClueAI/PromptCLUE-base`](https://huggingface.co/ClueAI/PromptCLUE-base) | [`PromptCLUE-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/PromptCLUE-base)|
+| chatglm   |chatglm-6b | THUDM | [github](https://github.com/THUDM/ChatGLM-6B), [`THUDM/chatglm-6b`](https://huggingface.co/THUDM/chatglm-6b), [`THUDM/chatglm-6b-int8`](https://huggingface.co/THUDM/chatglm-6b-int8), [`THUDM/chatglm-6b-int4`](https://huggingface.co/THUDM/chatglm-6b-int4), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0) | [`chatglm-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b), [`chatglm-6b-int8`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int8), [`chatglm-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-int4), [`chatglm-6b-v0.1.0`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm-6b-v0.1.0) |
+|       |chatglm2-6b | THUDM | [github](https://github.com/THUDM/ChatGLM2-6B), [`THUDM/chatglm2-6b`](https://huggingface.co/THUDM/chatglm2-6b), [`THUDM/chatglm2-6b-int4`](https://huggingface.co/THUDM/chatglm2-6b-int4), [`THUDM/chatglm2-6b-32k`](https://huggingface.co/THUDM/chatglm2-6b-32k) | [`chatglm2-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b), [`chatglm2-6b-int4`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-int4), [`chatglm2-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm2-6b-32k) |
+|       |chatglm3-6b | THUDM | [github](https://github.com/THUDM/ChatGLM3), [`THUDM/chatglm3-6b`](https://huggingface.co/THUDM/chatglm3-6b), [`THUDM/chatglm3-6b-32k`](https://huggingface.co/THUDM/chatglm3-6b-32k) | [`chatglm3-6b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b), [`chatglm3-6b-32k`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chatglm3-6b-32k) |
+| llama | llama | meta| [github](https://github.com/facebookresearch/llama) | [`llama-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-7b), [`llama-13b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/llama-13b)|
+|       | llama-2 | meta| [github](https://github.com/facebookresearch/llama), [meta-llama/Llama-2-7b-hf](https://huggingface.co/meta-llama/Llama-2-7b-hf), [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf), [meta-llama/Llama-2-13b-hf](https://huggingface.co/meta-llama/Llama-2-13b-hf), [meta-llama/Llama-2-13b-chat-hf](https://huggingface.co/meta-llama/Llama-2-13b-chat-hf) | [`Llama-2-7b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-hf), [`Llama-2-7b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-7b-chat-hf), [`Llama-2-13b-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-hf), [`Llama-2-13b-chat-hf`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Llama-2-13b-chat-hf)|
+|       | chinese_llama_alpaca|HFL|[github](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[`chinese_alpaca_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_alpaca_plus_7b), [`chinese_llama_plus_7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/chinese_llama_plus_7b)|
+|       | Belle_llama| LianjiaTech| [github](https://github.com/LianjiaTech/BELLE), [BelleGroup/BELLE-LLaMA-7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[`BELLE-LLaMA-7B-2M-enc`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/BELLE-LLaMA-7B-2M-enc)|
+|       | Ziya | IDEA-CCNL | [IDEA-CCNL/Ziya-LLaMA-13B-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [IDEA-CCNL/Ziya-LLaMA-13B-v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [`Ziya-LLaMA-13B-v1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1), [`Ziya-LLaMA-13B-v1.1`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Ziya-LLaMA-13B-v1.1) |
+|       | Baichuan | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan), [`baichuan-inc/Baichuan-7B`](https://huggingface.co/baichuan-inc/Baichuan-7B), [`baichuan-inc/Baichuan-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [`baichuan-inc/Baichuan-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [`Baichuan-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-7B), [`Baichuan-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Base), [`Baichuan-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan-13B-Chat) |
+|       | Baichuan2 | baichuan-inc | [github](https://github.com/baichuan-inc/Baichuan2), [`baichuan-inc/Baichuan2-7B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base), [`baichuan-inc/Baichuan2-7B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-7B-Chat), [`baichuan-inc/Baichuan2-13B-Base`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Base), [`baichuan-inc/Baichuan2-13B-Chat`](https://huggingface.co/baichuan-inc/Baichuan2-13B-Chat) | [`Baichuan2-7B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Base), [`Baichuan2-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-7B-Chat), [`Baichuan2-13B-Base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Base), [`Baichuan2-13B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Baichuan2-13B-Chat) |
+|       | vicuna | lmsys| [`lmsys/vicuna-7b-v1.5`](https://huggingface.co/lmsys/vicuna-7b-v1.5) | [`vicuna-7b-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/vicuna-7b-v1.5)|
+|       | Yi | 01-ai| [github](https://github.com/01-ai/Yi), [`01-ai/Yi-6B`](https://huggingface.co/01-ai/Yi-6B), [`01-ai/Yi-6B-200K`](https://huggingface.co/01-ai/Yi-6B-200K) | [`Yi-6B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B), [`Yi-6B-200K`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Yi-6B-200K)|
+| bloom |bloom | bigscience | [`bigscience/bloom-560m`](https://huggingface.co/bigscience/bloom-560m), [`bigscience/bloomz-560m`](https://huggingface.co/bigscience/bloomz-560m) | [`bloom-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloom-560m), [`bloomz-560m`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bloomz-560m) |
+| Qwen  |Qwen | 阿里云 | [github](https://github.com/QwenLM/Qwen-7B), [`Qwen/Qwen-1_8B`](https://huggingface.co/Qwen/Qwen-1_8B), [`Qwen/Qwen-1_8B-Chat`](https://huggingface.co/Qwen/Qwen-1_8B-Chat), [`Qwen/Qwen-7B`](https://huggingface.co/Qwen/Qwen-7B), [`Qwen/Qwen-7B-Chat`](https://huggingface.co/Qwen/Qwen-7B-Chat) | [`Qwen-1_8B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B), [`Qwen-1_8B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-1_8B-Chat), [`Qwen-7B`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B), [`Qwen-7B-Chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/Qwen-7B-Chat) |
+| InternLM|InternLM | 上海人工智能实验室 | [github](https://github.com/InternLM/InternLM), [`internlm/internlm-chat-7b`](https://huggingface.co/internlm/internlm-chat-7b), [`internlm/internlm-7b`](https://huggingface.co/internlm/internlm-7b) | [`internlm-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-7b), [`internlm-chat-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/internlm-chat-7b)|
+| Falcon|Falcon | tiiuae | [hf](https://huggingface.co/tiiuae), [`tiiuae/falcon-rw-1b`](https://huggingface.co/tiiuae/falcon-rw-1b), [`tiiuae/falcon-7b`](https://huggingface.co/tiiuae/falcon-7b), [`tiiuae/falcon-7b-instruct`](https://huggingface.co/tiiuae/falcon-7b-instruct) | [`falcon-rw-1b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-rw-1b), [`falcon-7b`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b), [`falcon-7b-instruct`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/falcon-7b-instruct) |
+|  moe  |deeoseek-moe|deepseek| [github](https://github.com/deepseek-ai/DeepSeek-MoE), [`deepseek-ai/deepseek-moe-16b-base`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-base), [`deepseek-ai/deepseek-moe-16b-chat`](https://huggingface.co/deepseek-ai/deepseek-moe-16b-chat) | [`deepseek-moe-16b-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-base), [`deepseek-moe-16b-chat`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/deepseek-moe-16b-chat) |
+| embedding| text2vec-base-chinese |shibing624| [`shibing624/text2vec-base-chinese`](https://huggingface.co/shibing624/text2vec-base-chinese) |[`text2vec-base-chinese`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/text2vec-base-chinese) |
+|          | m3e |moka-ai| [`moka-ai/m3e-base`](https://huggingface.co/moka-ai/m3e-base) |[`m3e-base`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/m3e-base)|
+|          | bge |BAAI| [`BAAI/bge-large-en-v1.5`](https://huggingface.co/BAAI/bge-large-en-v1.5), [`BAAI/bge-large-zh-v1.5`](https://huggingface.co/BAAI/bge-large-zh-v1.5) | [`bge-large-en-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-en-v1.5), [`bge-large-zh-v1.5`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/bge-large-zh-v1.5)|
+|          | gte |thenlper| [`thenlper/gte-large-zh`](https://huggingface.co/thenlper/gte-large-zh), [`thenlper/gte-base-zh`](https://huggingface.co/thenlper/gte-base-zh) |[`gte-base-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-base-zh), [`gte-large-zh`](https://huggingface.co/Tongjilibo/bert4torch_config/tree/main/gte-large-zh)|
+
+*注：
+1. `高亮格式`(如`bert-base-chinese`)的表示可直接`build_transformer_model()`联网下载
+2. 国内镜像网站加速下载
+   - `HF_ENDPOINT=https://hf-mirror.com python your_script.py`
+   - `export HF_ENDPOINT=https://hf-mirror.com`后再执行python代码
+   - 在python代码开头如下设置
+    ```python
+    import os
+    os.environ['HF_ENDPOINT'] = "https://hf-mirror.com"
+    ```
+
+## 6. 鸣谢
+
+- 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
+- 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
+
+## 7. 引用
+
+```
+@misc{bert4torch,
+  title={bert4torch},
+  author={Bo Li},
+  year={2022},
+  howpublished={\url{https://github.com/Tongjilibo/bert4torch}},
+}
+```
+
+## 8. 其他
+
+- Wechat & Star History Chart
+
+<table border="0">
+  <tbody>
+    <tr align="center" >
+      <td>
+         <a href="https://github.com/Tongjilibo"><img width="200" height="250" src="./docs/pics/wechat.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信号</a> 
+      </td>
+      <td>
+         <a href="https://github.com/Tongjilibo"><img width="190" height="250" src="./docs/pics/wechat_group.jpg" alt="pic"></a><br>
+         <a href="https://github.com/Tongjilibo">微信群</a> 
+      </td>
+      <td>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
+         <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
+      </td>    
+      </tr>
+  </tbody>
+</table>
```

### Comparing `bert4torch-0.4.9.post2/bert4torch.egg-info/SOURCES.txt` & `bert4torch-0.5.0/bert4torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/setup.py` & `bert4torch-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.4.9.post2',
+    version='v0.5.0',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['numpy', 'tqdm', 'torch>1.6', 'torch4keras==0.2.1.post2', 'six'],
+    install_requires=['numpy', 'tqdm', 'torch>1.6', 'torch4keras==0.2.2', 'six'],
     packages=find_packages()
 )
```

### Comparing `bert4torch-0.4.9.post2/test/test_entity_extract_rule.py` & `bert4torch-0.5.0/test/test_entity_extract_rule.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/test/test_fill_mask.py` & `bert4torch-0.5.0/test/test_fill_mask.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/test/test_generate_speed.py` & `bert4torch-0.5.0/test/test_generate_speed.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/test/test_hf_download.py` & `bert4torch-0.5.0/test/test_hf_download.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/test/test_save_pretrained.py` & `bert4torch-0.5.0/test/test_save_pretrained.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.4.9.post2/test/test_tokenizer.py` & `bert4torch-0.5.0/test/test_tokenizer.py`

 * *Files identical despite different names*

