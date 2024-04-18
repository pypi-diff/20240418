# Comparing `tmp/konfuzio_sdk-0.3.3.dev20240415090556.tar.gz` & `tmp/konfuzio_sdk-0.3.3.dev20240416095414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.3.dev20240415090556.tar", last modified: Tue Apr 16 03:26:56 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.3.dev20240416095414.tar", last modified: Wed Apr 17 03:25:41 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.3.dev20240415090556.tar` & `konfuzio_sdk-0.3.3.dev20240416095414.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.614107 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.618106 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 03:26:56.000000 konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:26:56.622106 konfuzio_sdk-0.3.3.dev20240415090556/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:26:56.618106 konfuzio_sdk-0.3.3.dev20240415090556/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-16 03:26:46.000000 konfuzio_sdk-0.3.3.dev20240415090556/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 03:25:30.000000 konfuzio_sdk-0.3.3.dev20240416095414/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-17 03:25:30.000000 konfuzio_sdk-0.3.3.dev20240416095414/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.260363 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.264364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.264364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.268364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.268364 konfuzio_sdk-0.3.3.dev20240416095414/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/LICENSE.md` & `konfuzio_sdk-0.3.3.dev20240416095414/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/PKG-INFO` & `konfuzio_sdk-0.3.3.dev20240416095414/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240415090556
+Version: 0.3.3.dev20240416095414
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
@@ -63,40 +63,40 @@
 [Konfuzio Server](https://dev.konfuzio.com/index.html#konfuzio-server).
 
 ## Features
 
 The SDK allows you to retrieve visual and text features to build your own document models. Konfuzio Server serves as an
 UI to define the data structure, manage training/test data and to deploy your models as API.
 
-Function               | Public Host Free*                         | On-Site (Paid)      |
-:--------------------- | :---------------------------------------- | :-------------------|
-OCR Text               | :heavy_check_mark:                        |  :heavy_check_mark: |
-OCR Handwriting        | :heavy_check_mark:                        |  :heavy_check_mark: |
-Text Annotation        | :heavy_check_mark:                        |  :heavy_check_mark: |
-PDF Annotation         | :heavy_check_mark:                        |  :heavy_check_mark: |
-Image Annotation       | :heavy_check_mark:                        |  :heavy_check_mark: |
-Table Annotation       | :heavy_check_mark:                        |  :heavy_check_mark: |
-Download Images        | :heavy_check_mark:                        |  :heavy_check_mark: |
-Download PDF with OCR  | :heavy_check_mark:                        |  :heavy_check_mark: |
-Deploy AI models       | :heavy_multiplication_x:                  |  :heavy_check_mark: |
+Function               | Public Host Free* | On-Site (Paid) |
+:--------------------- |:------------------|:---------------|
+OCR Text               | ✔️                | ✔️             |
+OCR Handwriting        | ✔️                | ✔️             |
+Text Annotation        | ✔️                | ✔️             |
+PDF Annotation         | ✔️                | ✔️             |
+Image Annotation       | ✔️                | ✔️ ️            |
+Table Annotation       | ✔️                | ✔️             |
+Download Images        | ✔️                | ✔️             |
+Download PDF with OCR  | ✔️                | ✔️             |
+Deploy AI models       | ✖️                | ✔️             |
 
 `*` Under fair use policy: We will impose 10 pages/hour throttling eventually.
 
 
-|                                                                                               |                                                               |
-|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------|
-| :ledger: [Docs](https://dev.konfuzio.com/sdk/index.html)                                                    | Read the docs                                                 |
-| :floppy_disk: [Installation](https://github.com/konfuzio-ai/konfuzio-sdk#installation)        | How to install the Konfuzio SDK                               |
-| :mortar_board: [Tutorials](https://dev.konfuzio.com/sdk/examples/examples.html)               | See what the Konfuzio SDK can do with our Notebooks & Scripts |
-| :bulb: [Explanations](https://dev.konfuzio.com/sdk/explanations.html)                         | Here are links to teaching material about the Konfuzio SDK.   |
-| :gear: [API Reference](https://dev.konfuzio.com/sdk/sourcecode.html)                          | Python classes, methods, and functions                        |
-| :heart: [Contributing](https://dev.konfuzio.com/sdk/contribution.html)                        | Learn how to contribute!                                      |
-| :bug: [Issue Tracker](https://github.com/konfuzio-ai/konfuzio-sdk/issues)                     | Report and monitor Konfuzio SDK issues                        |
-| :telescope: [Changelog](https://github.com/konfuzio-ai/konfuzio-sdk/releases)                 | Review the release notes                                      |
-| :newspaper: [MIT License](https://github.com/konfuzio-ai/konfuzio-sdk/blob/master/LICENSE.md) | Review the license                                            |
+|                                                                                      |                                                            |
+|--------------------------------------------------------------------------------------|------------------------------------------------------------|
+| 📒 [Docs](https://dev.konfuzio.com/sdk/index.html)                                   | Read the docs                                              |
+| 💾 [Installation](https://github.com/konfuzio-ai/konfuzio-sdk#installation)          | How to install the Konfuzio SDK                            |
+| 🎓 [Tutorials](https://dev.konfuzio.com/sdk/tutorials.html)                          | See what the Konfuzio SDK can do with our tutorials        |
+| 💡 [Explanations](https://dev.konfuzio.com/sdk/explanations.html)                    | Here are links to teaching material about the Konfuzio SDK. |
+| ⚙️ [API Reference](https://dev.konfuzio.com/sdk/sourcecode.html)                     | Python classes, methods, and functions                     |
+| ❤️ [Contributing](https://dev.konfuzio.com/sdk/contribution.html)                    | Learn how to contribute!                                   |
+| 🐛 [Issue Tracker](https://github.com/konfuzio-ai/konfuzio-sdk/issues)               | Report and monitor Konfuzio SDK issues                     |
+| 🔭 [Changelog](https://github.com/konfuzio-ai/konfuzio-sdk/releases)                 | Review the release notes                                   |
+| 📰 [MIT License](https://github.com/konfuzio-ai/konfuzio-sdk/blob/master/LICENSE.md) | Review the license                                         |
 
 ## Installation
 
 As developer register on our [public HOST for free: https://app.konfuzio.com](https://app.konfuzio.com/accounts/signup/)
 
 Then you can use pip to install Konfuzio SDK and run init:
 
@@ -110,16 +110,16 @@
 By default, the SDK is installed without the AI-related dependencies like `torch` or `transformers` and allows for using 
 only the Data-related SDK concepts but not the AI models. To install the SDK with the AI components,
 run the following command:
   ```
   pip install konfuzio_sdk[ai]
   ```
 
-Find the full installation guide [here](https://dev.konfuzio.com/sdk/get_started.html#install-sdk)
-or setup PyCharm as described [here](https://dev.konfuzio.com/sdk/quickstart_pycharm.html).
+Find the full installation guide [here](https://dev.konfuzio.com/sdk/get_started.html#install-sdk).
+To configure a PyCharm setup, follow the instructions [here](https://dev.konfuzio.com/sdk/quickstart_pycharm.html).
 
 ## CLI
 
 We provide the basic function to create a new Project via CLI:
 
 `konfuzio_sdk create_project YOUR_PROJECT_NAME`
 
@@ -129,30 +129,30 @@
 
 `konfuzio_sdk export_project YOUR_PROJECT_ID`
 
 ## Tutorials
 
 You can find detailed examples about how to set up and run document AI pipelines in our 
 [Tutorials](https://dev.konfuzio.com/sdk/tutorials.html), including:
-- [Split a file into separate Documents](https://dev.konfuzio.com/sdk/tutorials.html#split-a-file-into-separate-documents)
-- [Document Categorization](https://dev.konfuzio.com/sdk/tutorials.html#document-categorization)
-- [Train a Konfuzio SDK Model to Extract Information From Payslip Documents](https://dev.konfuzio.com/sdk/tutorials.html#train-a-konfuzio-sdk-model-to-extract-information-from-payslip-documents)
+- [Split a file into separate Documents](https://dev.konfuzio.com/sdk/tutorials/context-aware-file-splitting-model/index.html)
+- [Document Categorization](https://dev.konfuzio.com/sdk/tutorials/document_categorization/index.html)
+- [Train a Konfuzio SDK model to get insights from annual reports](https://dev.konfuzio.com/sdk/tutorials/annual-reports/index.html)
 
 ### Basics
 
 Here we show how to use the Konfuzio SDK to retrieve data hosted on a Konfuzio Server instance.
 
 ```python
 from konfuzio_sdk.data import Project, Document
 
 # Initialize the Project
 YOUR_PROJECT_ID: int
 my_project = Project(id_=YOUR_PROJECT_ID)
 
-# Get any Document online
+# Get any online Document
 DOCUMENT_ID_ONLINE: int
 doc: Document = my_project.get_document_by_id(DOCUMENT_ID_ONLINE)
 
 # Get the Annotations in a Document
 doc.annotations()
 
 # Filter Annotations by Label
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240415090556
+Version: 0.3.3.dev20240416095414
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
@@ -63,40 +63,40 @@
 [Konfuzio Server](https://dev.konfuzio.com/index.html#konfuzio-server).
 
 ## Features
 
 The SDK allows you to retrieve visual and text features to build your own document models. Konfuzio Server serves as an
 UI to define the data structure, manage training/test data and to deploy your models as API.
 
-Function               | Public Host Free*                         | On-Site (Paid)      |
-:--------------------- | :---------------------------------------- | :-------------------|
-OCR Text               | :heavy_check_mark:                        |  :heavy_check_mark: |
-OCR Handwriting        | :heavy_check_mark:                        |  :heavy_check_mark: |
-Text Annotation        | :heavy_check_mark:                        |  :heavy_check_mark: |
-PDF Annotation         | :heavy_check_mark:                        |  :heavy_check_mark: |
-Image Annotation       | :heavy_check_mark:                        |  :heavy_check_mark: |
-Table Annotation       | :heavy_check_mark:                        |  :heavy_check_mark: |
-Download Images        | :heavy_check_mark:                        |  :heavy_check_mark: |
-Download PDF with OCR  | :heavy_check_mark:                        |  :heavy_check_mark: |
-Deploy AI models       | :heavy_multiplication_x:                  |  :heavy_check_mark: |
+Function               | Public Host Free* | On-Site (Paid) |
+:--------------------- |:------------------|:---------------|
+OCR Text               | ✔️                | ✔️             |
+OCR Handwriting        | ✔️                | ✔️             |
+Text Annotation        | ✔️                | ✔️             |
+PDF Annotation         | ✔️                | ✔️             |
+Image Annotation       | ✔️                | ✔️ ️            |
+Table Annotation       | ✔️                | ✔️             |
+Download Images        | ✔️                | ✔️             |
+Download PDF with OCR  | ✔️                | ✔️             |
+Deploy AI models       | ✖️                | ✔️             |
 
 `*` Under fair use policy: We will impose 10 pages/hour throttling eventually.
 
 
-|                                                                                               |                                                               |
-|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------|
-| :ledger: [Docs](https://dev.konfuzio.com/sdk/index.html)                                                    | Read the docs                                                 |
-| :floppy_disk: [Installation](https://github.com/konfuzio-ai/konfuzio-sdk#installation)        | How to install the Konfuzio SDK                               |
-| :mortar_board: [Tutorials](https://dev.konfuzio.com/sdk/examples/examples.html)               | See what the Konfuzio SDK can do with our Notebooks & Scripts |
-| :bulb: [Explanations](https://dev.konfuzio.com/sdk/explanations.html)                         | Here are links to teaching material about the Konfuzio SDK.   |
-| :gear: [API Reference](https://dev.konfuzio.com/sdk/sourcecode.html)                          | Python classes, methods, and functions                        |
-| :heart: [Contributing](https://dev.konfuzio.com/sdk/contribution.html)                        | Learn how to contribute!                                      |
-| :bug: [Issue Tracker](https://github.com/konfuzio-ai/konfuzio-sdk/issues)                     | Report and monitor Konfuzio SDK issues                        |
-| :telescope: [Changelog](https://github.com/konfuzio-ai/konfuzio-sdk/releases)                 | Review the release notes                                      |
-| :newspaper: [MIT License](https://github.com/konfuzio-ai/konfuzio-sdk/blob/master/LICENSE.md) | Review the license                                            |
+|                                                                                      |                                                            |
+|--------------------------------------------------------------------------------------|------------------------------------------------------------|
+| 📒 [Docs](https://dev.konfuzio.com/sdk/index.html)                                   | Read the docs                                              |
+| 💾 [Installation](https://github.com/konfuzio-ai/konfuzio-sdk#installation)          | How to install the Konfuzio SDK                            |
+| 🎓 [Tutorials](https://dev.konfuzio.com/sdk/tutorials.html)                          | See what the Konfuzio SDK can do with our tutorials        |
+| 💡 [Explanations](https://dev.konfuzio.com/sdk/explanations.html)                    | Here are links to teaching material about the Konfuzio SDK. |
+| ⚙️ [API Reference](https://dev.konfuzio.com/sdk/sourcecode.html)                     | Python classes, methods, and functions                     |
+| ❤️ [Contributing](https://dev.konfuzio.com/sdk/contribution.html)                    | Learn how to contribute!                                   |
+| 🐛 [Issue Tracker](https://github.com/konfuzio-ai/konfuzio-sdk/issues)               | Report and monitor Konfuzio SDK issues                     |
+| 🔭 [Changelog](https://github.com/konfuzio-ai/konfuzio-sdk/releases)                 | Review the release notes                                   |
+| 📰 [MIT License](https://github.com/konfuzio-ai/konfuzio-sdk/blob/master/LICENSE.md) | Review the license                                         |
 
 ## Installation
 
 As developer register on our [public HOST for free: https://app.konfuzio.com](https://app.konfuzio.com/accounts/signup/)
 
 Then you can use pip to install Konfuzio SDK and run init:
 
@@ -110,16 +110,16 @@
 By default, the SDK is installed without the AI-related dependencies like `torch` or `transformers` and allows for using 
 only the Data-related SDK concepts but not the AI models. To install the SDK with the AI components,
 run the following command:
   ```
   pip install konfuzio_sdk[ai]
   ```
 
-Find the full installation guide [here](https://dev.konfuzio.com/sdk/get_started.html#install-sdk)
-or setup PyCharm as described [here](https://dev.konfuzio.com/sdk/quickstart_pycharm.html).
+Find the full installation guide [here](https://dev.konfuzio.com/sdk/get_started.html#install-sdk).
+To configure a PyCharm setup, follow the instructions [here](https://dev.konfuzio.com/sdk/quickstart_pycharm.html).
 
 ## CLI
 
 We provide the basic function to create a new Project via CLI:
 
 `konfuzio_sdk create_project YOUR_PROJECT_NAME`
 
@@ -129,30 +129,30 @@
 
 `konfuzio_sdk export_project YOUR_PROJECT_ID`
 
 ## Tutorials
 
 You can find detailed examples about how to set up and run document AI pipelines in our 
 [Tutorials](https://dev.konfuzio.com/sdk/tutorials.html), including:
-- [Split a file into separate Documents](https://dev.konfuzio.com/sdk/tutorials.html#split-a-file-into-separate-documents)
-- [Document Categorization](https://dev.konfuzio.com/sdk/tutorials.html#document-categorization)
-- [Train a Konfuzio SDK Model to Extract Information From Payslip Documents](https://dev.konfuzio.com/sdk/tutorials.html#train-a-konfuzio-sdk-model-to-extract-information-from-payslip-documents)
+- [Split a file into separate Documents](https://dev.konfuzio.com/sdk/tutorials/context-aware-file-splitting-model/index.html)
+- [Document Categorization](https://dev.konfuzio.com/sdk/tutorials/document_categorization/index.html)
+- [Train a Konfuzio SDK model to get insights from annual reports](https://dev.konfuzio.com/sdk/tutorials/annual-reports/index.html)
 
 ### Basics
 
 Here we show how to use the Konfuzio SDK to retrieve data hosted on a Konfuzio Server instance.
 
 ```python
 from konfuzio_sdk.data import Project, Document
 
 # Initialize the Project
 YOUR_PROJECT_ID: int
 my_project = Project(id_=YOUR_PROJECT_ID)
 
-# Get any Document online
+# Get any online Document
 DOCUMENT_ID_ONLINE: int
 doc: Document = my_project.get_document_by_id(DOCUMENT_ID_ONLINE)
 
 # Get the Annotations in a Document
 doc.annotations()
 
 # Filter Annotations by Label
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/setup.py` & `konfuzio_sdk-0.3.3.dev20240416095414/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_api.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_cli.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_data.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_evaluate.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_extras.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_normalize.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_regex.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_samples.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_urls.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240415090556/tests/test_utils.py` & `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_utils.py`

 * *Files identical despite different names*

