# Comparing `tmp/tokenizernltk-0.0.16.tar.gz` & `tmp/tokenizernltk-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizernltk-0.0.16.tar", last modified: Thu Apr 18 01:01:27 2024, max compression
+gzip compressed data, was "tokenizernltk-0.15.tar", last modified: Thu Apr 18 00:54:19 2024, max compression
```

## Comparing `tokenizernltk-0.0.16.tar` & `tokenizernltk-0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 01:01:27.913045 tokenizernltk-0.0.16/
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-18 01:01:27.913045 tokenizernltk-0.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1678 2024-04-18 01:00:01.000000 tokenizernltk-0.0.16/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 01:01:27.913045 tokenizernltk-0.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      813 2024-04-18 01:00:26.000000 tokenizernltk-0.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 01:01:27.912045 tokenizernltk-0.0.16/tokenizedinputblobs/
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-18 00:59:49.000000 tokenizernltk-0.0.16/tokenizedinputblobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-04-18 01:00:53.000000 tokenizernltk-0.0.16/tokenizedinputblobs/tokenized_vals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 01:01:27.913045 tokenizernltk-0.0.16/tokenizernltk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-18 01:01:27.000000 tokenizernltk-0.0.16/tokenizernltk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-18 01:01:27.000000 tokenizernltk-0.0.16/tokenizernltk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 01:01:27.000000 tokenizernltk-0.0.16/tokenizernltk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 01:01:27.000000 tokenizernltk-0.0.16/tokenizernltk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-18 01:01:27.000000 tokenizernltk-0.0.16/tokenizernltk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:54:19.164428 tokenizernltk-0.15/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-04-18 00:54:19.164428 tokenizernltk-0.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-04-18 00:49:18.000000 tokenizernltk-0.15/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 00:54:19.164428 tokenizernltk-0.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-18 00:52:45.000000 tokenizernltk-0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:54:19.163428 tokenizernltk-0.15/tokenizedinputblobs/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-18 00:50:36.000000 tokenizernltk-0.15/tokenizedinputblobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-18 00:50:40.000000 tokenizernltk-0.15/tokenizedinputblobs/tokenizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 00:54:19.164428 tokenizernltk-0.15/tokenizernltk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-04-18 00:54:19.000000 tokenizernltk-0.15/tokenizernltk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2024-04-18 00:54:19.000000 tokenizernltk-0.15/tokenizernltk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 00:54:19.000000 tokenizernltk-0.15/tokenizernltk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 00:54:19.000000 tokenizernltk-0.15/tokenizernltk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-18 00:54:19.000000 tokenizernltk-0.15/tokenizernltk.egg-info/top_level.txt
```

### Comparing `tokenizernltk-0.0.16/README.md` & `tokenizernltk-0.15/README.md`

 * *Files identical despite different names*

### Comparing `tokenizernltk-0.0.16/setup.py` & `tokenizernltk-0.15/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.16'
+VERSION = '0.15'
 DESCRIPTION = 'Tokenizer Data Values Via NLTK'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="tokenizernltk",
     version=VERSION,
     author="PyTorch",
-    author_email="<uts@uts.rf.gd>",
+    author_email="info@pytorch.io>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
         "transformers",
         "textblob"
```

### Comparing `tokenizernltk-0.0.16/tokenizedinputblobs/tokenized_vals.py` & `tokenizernltk-0.15/tokenizedinputblobs/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import torch
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 from textblob import TextBlob
 import logging
 import warnings
 
-class tokenizer_nltk:
+class tokenizerNLTK:
     def __init__(self, model_name = "humarin/chatgpt_paraphraser_on_T5_base", tokenizerSeq2SeqIntial = "bigscience/mt0-large"):
         self.tokenizer_default = None
         self.model_default = None
         self.secondary_tokenizer = None
         self.model_name = model_name
         self.tokenizerSeq2SeqIntial = tokenizerSeq2SeqIntial
         # Suppress warnings
```

