# Comparing `tmp/pyprocessors-opennre-0.5.74.tar.gz` & `tmp/pyprocessors_opennre-0.5.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-opennre-0.5.74.tar", last modified: Thu Dec 15 22:28:51 2022, max compression
+gzip compressed data, was "pyprocessors_opennre-0.5.98.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors-opennre-0.5.74.tar` & `pyprocessors_opennre-0.5.98.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      496 2022-10-04 08:09:00.159523 pyprocessors-opennre-0.5.74/.bumpversion.cfg
--rw-r--r--   0        0        0     1760 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/.gitignore
--rw-r--r--   0        0        0      419 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/.readthedocs.yml
--rw-r--r--   0        0        0      116 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/AUTHORS.md
--rw-r--r--   0        0        0      268 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/CHANGELOG.md
--rw-r--r--   0        0        0      476 2022-10-04 08:09:00.162523 pyprocessors-opennre-0.5.74/Dockerfile
--rw-r--r--   0        0        0    10797 2022-12-15 21:54:08.900935 pyprocessors-opennre-0.5.74/Jenkinsfile
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:00.163523 pyprocessors-opennre-0.5.74/LICENSE
--rw-r--r--   0        0        0     1533 2022-10-04 08:09:00.163523 pyprocessors-opennre-0.5.74/README.md
--rw-r--r--   0        0        0      939 2022-10-04 08:09:00.163523 pyprocessors-opennre-0.5.74/RELEASE.md
--rw-r--r--   0        0        0     1563 2022-10-04 08:09:00.163523 pyprocessors-opennre-0.5.74/bumpversion.py
--rw-r--r--   0        0        0       62 2022-10-04 08:09:00.163523 pyprocessors-opennre-0.5.74/docs/.gitignore
--rw-r--r--   0        0        0      268 2022-10-04 08:09:00.164523 pyprocessors-opennre-0.5.74/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2022-10-04 08:09:00.164523 pyprocessors-opennre-0.5.74/docs/LICENSE
--rw-r--r--   0        0        0        0 2022-10-04 08:09:00.164523 pyprocessors-opennre-0.5.74/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-10-04 08:09:00.165523 pyprocessors-opennre-0.5.74/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2874 2022-10-04 08:09:00.166523 pyprocessors-opennre-0.5.74/docs/conf.py
--rw-r--r--   0        0        0      141 2022-10-04 08:09:00.166523 pyprocessors-opennre-0.5.74/docs/index.rst
--rw-r--r--   0        0        0       98 2022-10-04 08:09:00.166523 pyprocessors-opennre-0.5.74/mypy.ini
--rw-r--r--   0        0        0     2318 2022-10-04 08:09:00.166523 pyprocessors-opennre-0.5.74/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-04 08:09:00.167523 pyprocessors-opennre-0.5.74/src/__init__.py
--rw-r--r--   0        0        0      107 2022-12-15 22:28:44.867637 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/__init__.py
--rw-r--r--   0        0        0      625 2022-10-04 08:09:00.169523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/__init__.py
--rw-r--r--   0        0        0      335 2022-10-04 08:09:00.169523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/__init__.py
--rw-r--r--   0        0        0     6052 2022-10-04 08:09:00.170523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/base_encoder.py
--rw-r--r--   0        0        0     8458 2022-10-04 08:09:00.170523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/bert_encoder.py
--rw-r--r--   0        0        0     2555 2022-10-04 08:09:00.170523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/cnn_encoder.py
--rw-r--r--   0        0        0     6986 2022-10-04 08:09:00.170523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/pcnn_encoder.py
--rw-r--r--   0        0        0      606 2022-10-04 08:09:00.170523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/__init__.py
--rw-r--r--   0        0        0     6819 2022-10-04 08:09:00.171523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/bag_re.py
--rw-r--r--   0        0        0    19369 2022-10-04 08:09:00.171523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/data_loader.py
--rw-r--r--   0        0        0     6619 2022-10-04 08:09:00.171523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/multi_label_sentence_re.py
--rw-r--r--   0        0        0     6410 2022-10-04 08:09:00.171523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/sentence_re.py
--rw-r--r--   0        0        0      721 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/utils.py
--rw-r--r--   0        0        0      481 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/__init__.py
--rw-r--r--   0        0        0     8279 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_attention.py
--rw-r--r--   0        0        0     5012 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_average.py
--rw-r--r--   0        0        0     6269 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_one.py
--rw-r--r--   0        0        0     1878 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/base_model.py
--rw-r--r--   0        0        0     1165 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/sigmoid_nn.py
--rw-r--r--   0        0        0     1615 2022-10-04 08:09:00.172523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/softmax_nn.py
--rw-r--r--   0        0        0      109 2022-10-04 08:09:00.173523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/__init__.py
--rw-r--r--   0        0        0      223 2022-10-04 08:09:00.173523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/__init__.py
--rw-r--r--   0        0        0     1059 2022-10-04 08:09:00.173523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/cnn.py
--rw-r--r--   0        0        0     1327 2022-10-04 08:09:00.173523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/lstm.py
--rw-r--r--   0        0        0     1320 2022-10-04 08:09:00.173523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/rnn.py
--rw-r--r--   0        0        0      213 2022-10-04 08:09:00.174523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/pool/__init__.py
--rw-r--r--   0        0        0     1811 2022-10-04 08:09:00.174523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/pool/avg_pool.py
--rw-r--r--   0        0        0     2277 2022-10-04 08:09:00.175523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/pool/max_pool.py
--rw-r--r--   0        0        0    11530 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/pretrain.py
--rw-r--r--   0        0        0      752 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/__init__.py
--rw-r--r--   0        0        0     2633 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/basic_tokenizer.py
--rw-r--r--   0        0        0     2192 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/bert_tokenizer.py
--rw-r--r--   0        0        0     8627 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/utils.py
--rw-r--r--   0        0        0     3862 2022-10-04 08:09:00.176524 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/word_piece_tokenizer.py
--rw-r--r--   0        0        0     2709 2022-10-04 08:09:00.177523 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/word_tokenizer.py
--rw-r--r--   0        0        0     8245 2022-11-04 08:54:05.457224 pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre_proc.py
--rw-r--r--   0        0        0    39344 2022-10-04 08:09:00.180523 pyprocessors-opennre-0.5.74/tests/data/bel_entities.json
--rw-r--r--   0        0        0    41750 2022-12-15 22:28:37.607446 pyprocessors-opennre-0.5.74/tests/data/bel_entities_rel0.json
--rw-r--r--   0        0        0     6689 2022-11-04 09:11:08.742652 pyprocessors-opennre-0.5.74/tests/test_opennre.py
--rw-r--r--   0        0        0     1204 2022-10-04 08:09:00.186524 pyprocessors-opennre-0.5.74/tox.ini
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 pyprocessors-opennre-0.5.74/setup.py
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 pyprocessors-opennre-0.5.74/PKG-INFO
+-rw-r--r--   0        0        0      496 2023-08-21 14:19:06.628221 pyprocessors_opennre-0.5.98/.bumpversion.cfg
+-rw-r--r--   0        0        0     1802 2023-08-21 14:19:06.628221 pyprocessors_opennre-0.5.98/.gitignore
+-rw-r--r--   0        0        0      419 2023-08-21 14:19:06.629221 pyprocessors_opennre-0.5.98/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2023-08-21 14:19:06.629221 pyprocessors_opennre-0.5.98/.readthedocs.yml
+-rw-r--r--   0        0        0      116 2023-08-21 14:19:06.629221 pyprocessors_opennre-0.5.98/AUTHORS.md
+-rw-r--r--   0        0        0      268 2023-08-21 14:19:06.629221 pyprocessors_opennre-0.5.98/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2023-08-21 14:19:06.629221 pyprocessors_opennre-0.5.98/Dockerfile
+-rw-r--r--   0        0        0    13917 2023-08-25 23:48:28.998148 pyprocessors_opennre-0.5.98/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2023-08-21 14:19:06.630221 pyprocessors_opennre-0.5.98/LICENSE
+-rw-r--r--   0        0        0     1533 2023-08-21 14:19:06.630221 pyprocessors_opennre-0.5.98/README.md
+-rw-r--r--   0        0        0      939 2023-08-21 14:19:06.630221 pyprocessors_opennre-0.5.98/RELEASE.md
+-rw-r--r--   0        0        0     1563 2023-08-21 14:19:06.630221 pyprocessors_opennre-0.5.98/bumpversion.py
+-rw-r--r--   0        0        0       62 2023-08-21 14:19:06.632221 pyprocessors_opennre-0.5.98/docs/.gitignore
+-rw-r--r--   0        0        0      268 2023-08-21 14:19:06.633221 pyprocessors_opennre-0.5.98/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-08-21 14:19:06.634221 pyprocessors_opennre-0.5.98/docs/LICENSE
+-rw-r--r--   0        0        0        0 2023-08-21 14:19:06.634221 pyprocessors_opennre-0.5.98/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-08-21 14:19:06.634221 pyprocessors_opennre-0.5.98/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2874 2023-08-21 14:19:06.635221 pyprocessors_opennre-0.5.98/docs/conf.py
+-rw-r--r--   0        0        0      141 2023-08-21 14:19:06.636221 pyprocessors_opennre-0.5.98/docs/index.rst
+-rw-r--r--   0        0        0       98 2023-08-21 14:19:06.636221 pyprocessors_opennre-0.5.98/mypy.ini
+-rw-r--r--   0        0        0     2326 2023-08-28 09:34:47.553569 pyprocessors_opennre-0.5.98/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-21 14:19:06.637221 pyprocessors_opennre-0.5.98/src/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-28 09:44:43.267435 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/__init__.py
+-rw-r--r--   0        0        0      625 2023-08-21 14:19:06.639221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/__init__.py
+-rw-r--r--   0        0        0      335 2023-08-21 14:19:06.639221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/__init__.py
+-rw-r--r--   0        0        0     6052 2023-08-21 14:19:06.639221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/base_encoder.py
+-rw-r--r--   0        0        0     8458 2023-08-21 14:19:06.640221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/bert_encoder.py
+-rw-r--r--   0        0        0     2555 2023-08-21 14:19:06.640221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/cnn_encoder.py
+-rw-r--r--   0        0        0     6986 2023-08-21 14:19:06.640221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/pcnn_encoder.py
+-rw-r--r--   0        0        0      606 2023-08-21 14:19:06.640221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/__init__.py
+-rw-r--r--   0        0        0     6819 2023-08-21 14:19:06.640221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/bag_re.py
+-rw-r--r--   0        0        0    19369 2023-08-21 14:19:06.641221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/data_loader.py
+-rw-r--r--   0        0        0     6619 2023-08-21 14:19:06.642221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/multi_label_sentence_re.py
+-rw-r--r--   0        0        0     6410 2023-08-21 14:19:06.643221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/sentence_re.py
+-rw-r--r--   0        0        0      721 2023-08-21 14:19:06.643221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/utils.py
+-rw-r--r--   0        0        0      481 2023-08-21 14:19:06.643221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/__init__.py
+-rw-r--r--   0        0        0     8279 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_attention.py
+-rw-r--r--   0        0        0     5012 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_average.py
+-rw-r--r--   0        0        0     6269 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_one.py
+-rw-r--r--   0        0        0     1878 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/base_model.py
+-rw-r--r--   0        0        0     1165 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/sigmoid_nn.py
+-rw-r--r--   0        0        0     1615 2023-08-21 14:19:06.644221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/softmax_nn.py
+-rw-r--r--   0        0        0      109 2023-08-21 14:19:06.645221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/__init__.py
+-rw-r--r--   0        0        0      223 2023-08-21 14:19:06.645221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/__init__.py
+-rw-r--r--   0        0        0     1059 2023-08-21 14:19:06.645221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/cnn.py
+-rw-r--r--   0        0        0     1327 2023-08-21 14:19:06.645221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/lstm.py
+-rw-r--r--   0        0        0     1320 2023-08-21 14:19:06.645221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/rnn.py
+-rw-r--r--   0        0        0      213 2023-08-21 14:19:06.646221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/pool/__init__.py
+-rw-r--r--   0        0        0     1811 2023-08-21 14:19:06.647221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/pool/avg_pool.py
+-rw-r--r--   0        0        0     2277 2023-08-21 14:19:06.647221 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/pool/max_pool.py
+-rw-r--r--   0        0        0    11530 2023-08-21 14:19:06.648222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/pretrain.py
+-rw-r--r--   0        0        0      752 2023-08-21 14:19:06.648222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/__init__.py
+-rw-r--r--   0        0        0     2633 2023-08-21 14:19:06.648222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/basic_tokenizer.py
+-rw-r--r--   0        0        0     2192 2023-08-21 14:19:06.649222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/bert_tokenizer.py
+-rw-r--r--   0        0        0     8627 2023-08-21 14:19:06.649222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/utils.py
+-rw-r--r--   0        0        0     3862 2023-08-21 14:19:06.649222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/word_piece_tokenizer.py
+-rw-r--r--   0        0        0     2709 2023-08-21 14:19:06.650222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/word_tokenizer.py
+-rw-r--r--   0        0        0     8245 2023-08-21 14:19:06.651222 pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre_proc.py
+-rw-r--r--   0        0        0    39344 2023-08-21 14:19:06.652222 pyprocessors_opennre-0.5.98/tests/data/bel_entities.json
+-rw-r--r--   0        0        0    41750 2023-08-28 09:44:39.759341 pyprocessors_opennre-0.5.98/tests/data/bel_entities_rel0.json
+-rw-r--r--   0        0        0     6689 2023-08-21 14:19:06.654222 pyprocessors_opennre-0.5.98/tests/test_opennre.py
+-rw-r--r--   0        0        0     1204 2023-08-21 14:19:06.655222 pyprocessors_opennre-0.5.98/tox.ini
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 pyprocessors_opennre-0.5.98/setup.py
+-rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 pyprocessors_opennre-0.5.98/PKG-INFO
```

### Comparing `pyprocessors-opennre-0.5.74/.gitignore` & `pyprocessors_opennre-0.5.98/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -122,9 +122,12 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
+# Specific
 .idea/
 models/
+.groovylintrc.json
+.emailNotif
```

### Comparing `pyprocessors-opennre-0.5.74/LICENSE` & `pyprocessors_opennre-0.5.98/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/README.md` & `pyprocessors_opennre-0.5.98/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/RELEASE.md` & `pyprocessors_opennre-0.5.98/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/bumpversion.py` & `pyprocessors_opennre-0.5.98/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/docs/LICENSE` & `pyprocessors_opennre-0.5.98/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/docs/conf.py` & `pyprocessors_opennre-0.5.98/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/pyproject.toml` & `pyprocessors_opennre-0.5.98/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3.8",
 ]
 requires = [
     "pymultirole-plugins>=0.5.0,<0.6.0",
     "collections-extended",
-    "torch==1.7.1",
+    "torch==1.8.1",
 #    "opennre"
-    "transformers",
+    "transformers==4.12.0",
     "scikit-learn",
     "scipy",
     "nltk",
     "pybel"
 ]
 dist-name = "pyprocessors-opennre"
```

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/__init__.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/base_encoder.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/base_encoder.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/bert_encoder.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/bert_encoder.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/cnn_encoder.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/encoder/pcnn_encoder.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/encoder/pcnn_encoder.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/__init__.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/bag_re.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/bag_re.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/data_loader.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/data_loader.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/multi_label_sentence_re.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/multi_label_sentence_re.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/sentence_re.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/sentence_re.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/framework/utils.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/framework/utils.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_attention.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_attention.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_average.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_average.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/bag_one.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/bag_one.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/base_model.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/base_model.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/sigmoid_nn.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/sigmoid_nn.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/model/softmax_nn.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/model/softmax_nn.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/cnn.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/cnn.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/lstm.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/lstm.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/nn/rnn.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/nn/rnn.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/pool/avg_pool.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/module/pool/max_pool.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/module/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/pretrain.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/pretrain.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/__init__.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/basic_tokenizer.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/basic_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/bert_tokenizer.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/utils.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/word_piece_tokenizer.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/word_piece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre/tokenization/word_tokenizer.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre/tokenization/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/src/pyprocessors_opennre/opennre_proc.py` & `pyprocessors_opennre-0.5.98/src/pyprocessors_opennre/opennre_proc.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/tests/data/bel_entities.json` & `pyprocessors_opennre-0.5.98/tests/data/bel_entities.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/tests/data/bel_entities_rel0.json` & `pyprocessors_opennre-0.5.98/tests/data/bel_entities_rel0.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/tests/test_opennre.py` & `pyprocessors_opennre-0.5.98/tests/test_opennre.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/tox.ini` & `pyprocessors_opennre-0.5.98/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-opennre-0.5.74/setup.py` & `pyprocessors_opennre-0.5.98/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 package_dir = \
 {'': 'src'}
 
 install_requires = \
 ['pymultirole-plugins>=0.5.0,<0.6.0',
  'collections-extended',
- 'torch==1.7.1',
- 'transformers',
+ 'torch==1.8.1',
+ 'transformers==4.12.0',
  'scikit-learn',
  'scipy',
  'nltk',
  'pybel']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
@@ -47,15 +47,15 @@
           'openpyxl==3.0.7']}
 
 entry_points = \
 {'pyprocessors.plugins': ['opennre = '
                           'pyprocessors_opennre.opennre_proc:OpenNREProcessor']}
 
 setup(name='pyprocessors-opennre',
-      version='0.5.74',
+      version='0.5.98',
       description='Processor based on Huggingface transformers zero-shot classification pipeline',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_opennre/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors-opennre-0.5.74/PKG-INFO` & `pyprocessors_opennre-0.5.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-opennre
-Version: 0.5.74
+Version: 0.5.98
 Summary: Processor based on Huggingface transformers zero-shot classification pipeline
 Home-page: https://github.com/oterrier/pyprocessors_opennre/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -17,16 +17,16 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pymultirole-plugins>=0.5.0,<0.6.0
 Requires-Dist: collections-extended
-Requires-Dist: torch==1.7.1
-Requires-Dist: transformers
+Requires-Dist: torch==1.8.1
+Requires-Dist: transformers==4.12.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: nltk
 Requires-Dist: pybel
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
```

