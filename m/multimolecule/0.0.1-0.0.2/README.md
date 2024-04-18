# Comparing `tmp/multimolecule-0.0.1.tar.gz` & `tmp/multimolecule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimolecule-0.0.1.tar", last modified: Tue Mar 26 14:47:00 2024, max compression
+gzip compressed data, was "multimolecule-0.0.2.tar", last modified: Thu Apr 18 13:35:04 2024, max compression
```

## Comparing `multimolecule-0.0.1.tar` & `multimolecule-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 14:46:56.000000 multimolecule-0.0.1/.codespell-whitelist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 14:46:56.000000 multimolecule-0.0.1/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-26 14:46:56.000000 multimolecule-0.0.1/.github/workflows/push.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6886 2024-03-26 14:46:56.000000 multimolecule-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-26 14:46:56.000000 multimolecule-0.0.1/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    34522 2024-03-26 14:46:56.000000 multimolecule-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41095 2024-03-26 14:47:00.131084 multimolecule-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 14:46:56.000000 multimolecule-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 14:46:59.000000 multimolecule-0.0.1/multimolecule/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule/models/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule/models/rnabert/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/models/rnabert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/models/rnabert/configuration_rnabert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/models/rnabert/convert_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/models/rnabert/modeling_rnabert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule/tokenizers/rna/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/tokenizers/rna/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1684 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/tokenizers/rna/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4867 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/tokenizers/rna/tokenization_rna.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-03-26 14:46:56.000000 multimolecule-0.0.1/multimolecule/tokenizers/rna/vocab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:47:00.131084 multimolecule-0.0.1/multimolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41095 2024-03-26 14:47:00.000000 multimolecule-0.0.1/multimolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-26 14:47:00.000000 multimolecule-0.0.1/multimolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:47:00.000000 multimolecule-0.0.1/multimolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 14:47:00.000000 multimolecule-0.0.1/multimolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-03-26 14:46:56.000000 multimolecule-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:47:00.131084 multimolecule-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-03-26 14:46:56.000000 multimolecule-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 14:46:56.000000 multimolecule-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.667251 multimolecule-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.codespell-whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.github/workflows/push.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-18 13:34:55.000000 multimolecule-0.0.2/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34522 2024-04-18 13:34:55.000000 multimolecule-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-18 13:35:04.667251 multimolecule-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:34:55.000000 multimolecule-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/rnabert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/configuration_rnabert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25725 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnabert/modeling_rnabert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.659251 multimolecule-0.0.2/multimolecule/models/rnafm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/configuration_rnafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/convert_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51027 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnafm/modeling_rnafm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/rnamsm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/configuration_rnamsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50103 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/rnamsm/modeling_rnamsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/splicebert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/configuration_splicebert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48169 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/splicebert/modeling_splicebert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/utrbert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/configuration_utrbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/convert_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46386 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrbert/modeling_utrbert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/models/utrlm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/configuration_utrlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/convert_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52324 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/models/utrlm/modeling_utrlm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule/tokenizers/rna/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5285 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/tokenization_rna.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2072 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/rna/vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 13:34:55.000000 multimolecule-0.0.2/multimolecule/tokenizers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:35:04.663251 multimolecule-0.0.2/multimolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41154 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:35:04.000000 multimolecule-0.0.2/multimolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 13:34:55.000000 multimolecule-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:35:04.667251 multimolecule-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-18 13:34:55.000000 multimolecule-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 13:34:55.000000 multimolecule-0.0.2/tox.ini
```

### Comparing `multimolecule-0.0.1/.github/workflows/push.yaml` & `multimolecule-0.0.2/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.1/.gitignore` & `multimolecule-0.0.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 [Aa][Rr][Mm]64/
 bld/
 [Bb]in/
 [Oo]bj/
 [Ll]og/
 [Ll]ogs/
 
+# Visual Studio Code cache/options directory
+.vscode/
+
 # Visual Studio 2015/2017 cache/options directory
 .vs/
 # Uncomment if you have tasks that create the project's static files in wwwroot
 #wwwroot/
 
 # Visual Studio 2017 auto generated files
 Generated\ Files/
@@ -395,7 +398,43 @@
 *.msp
 
 # JetBrains Rider
 *.sln.iml
 
 # version
 **/_version.py
+
+# Python Egg
+*.egg-info/
+
+# Tar
+**/*.tar
+**/*.tgz
+**/*.txz
+**/*.gz
+**/*.xz
+
+# Pickle
+**/*.pickle
+**/*.pkl
+
+# Checkpoints
+**/*.onnx
+**/*.ckpt
+**/*.safetensors
+**/*.pth
+**/*.pt
+**/*.bin
+**/*.msgpack
+**/*.h5
+**/*.ot
+
+# Data
+**/*.np
+**/*.npy
+**/*.npz
+**/*.numpy
+**/*.pd
+**/*.pandas
+
+# debug files
+**/*debug*
```

### Comparing `multimolecule-0.0.1/.pre-commit-config.yaml` & `multimolecule-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.1/LICENSE` & `multimolecule-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multimolecule-0.0.1/PKG-INFO` & `multimolecule-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimolecule
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Networks for RNA, DNA, and Protein.
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,7 +682,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chanfig>=0.0.99
+Requires-Dist: transformers
```

### Comparing `multimolecule-0.0.1/multimolecule/models/rnabert/configuration_rnabert.py` & `multimolecule-0.0.2/multimolecule/models/rnabert/configuration_rnabert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,109 @@
-from transformers.configuration_utils import PretrainedConfig
 from transformers.utils import logging
 
+from ..configuration_utils import HeadConfig, MaskedLMHeadConfig, PretrainedConfig
+
 logger = logging.get_logger(__name__)
 
 
 class RnaBertConfig(PretrainedConfig):
     r"""
     This is the configuration class to store the configuration of a [`RnaBertModel`]. It is used to instantiate a
     RnaBert model according to the specified arguments, defining the model architecture. Instantiating a configuration
     with the defaults will yield a similar configuration to that of the RnaBert
-    [mana438/RNABERT](https://github.com/mana438/RNABERT/blob/master/RNA_bert_config.json) architecture.
+    [mana438/RNABERT](https://github.com/mana438/RNABERT) architecture.
 
     Configuration objects inherit from [`PretrainedConfig`] and can be used to control the model outputs. Read the
     documentation from [`PretrainedConfig`] for more information.
 
 
     Args:
-        vocab_size (`int`, *optional*):
+        vocab_size (`int`, *optional*, defaults to 25):
             Vocabulary size of the RnaBert model. Defines the number of different tokens that can be represented by the
             `inputs_ids` passed when calling [`RnaBertModel`].
-        mask_token_id (`int`, *optional*):
-            The index of the mask token in the vocabulary. This must be included in the config because of the
-            "mask-dropout" scaling trick, which will scale the inputs depending on the number of masked tokens.
-        pad_token_id (`int`, *optional*):
-            The index of the padding token in the vocabulary. This must be included in the config because certain parts
-            of the RnaBert code use this instead of the attention mask.
-        hidden_size (`int`, *optional*, defaults to 768):
+        hidden_size (`int`, *optional*, defaults to 120):
             Dimensionality of the encoder layers and the pooler layer.
         num_hidden_layers (`int`, *optional*, defaults to 12):
             Number of hidden layers in the Transformer encoder.
-        num_attention_heads (`int`, *optional*, defaults to 12):
+        num_attention_heads (`int`, *optional*, defaults to 6):
             Number of attention heads for each attention layer in the Transformer encoder.
-        intermediate_size (`int`, *optional*, defaults to 3072):
+        intermediate_size (`int`, *optional*, defaults to 40):
             Dimensionality of the "intermediate" (often named feed-forward) layer in the Transformer encoder.
-        hidden_dropout_prob (`float`, *optional*, defaults to 0.1):
+        hidden_dropout (`float`, *optional*, defaults to 0.0):
             The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
-        attention_probs_dropout_prob (`float`, *optional*, defaults to 0.1):
+        attention_dropout (`float`, *optional*, defaults to 0.0):
             The dropout ratio for the attention probabilities.
-        max_position_embeddings (`int`, *optional*, defaults to 1026):
+        max_position_embeddings (`int`, *optional*, defaults to 440):
             The maximum sequence length that this model might ever be used with. Typically set this to something large
             just in case (e.g., 512 or 1024 or 2048).
         initializer_range (`float`, *optional*, defaults to 0.02):
             The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
         layer_norm_eps (`float`, *optional*, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
 
     Examples:
+        >>> from multimolecule import RnaBertModel, RnaBertConfig
 
-    ```python
-    >>> from multimolecule import RnaBertModel, RnaBertConfig
-
-    >>> # Initializing a RnaBert style configuration >>> configuration = RnaBertConfig()
+        >>> # Initializing a RNABERT multimolecule/rnabert style configuration
+        >>> configuration = RnaBertConfig()
 
-    >>> # Initializing a model from the configuration >>> model = RnaBertModel(configuration)
+        >>> # Initializing a model (with random weights) from the multimolecule/rnabert style configuration
+        >>> model = RnaBertModel(configuration)
 
-    >>> # Accessing the model configuration >>> configuration = model.config
-    ```"""
+        >>> # Accessing the model configuration
+        >>> configuration = model.config
+    """
 
     model_type = "rnabert"
 
     def __init__(
         self,
         vocab_size=25,
         ss_vocab_size=8,
         hidden_size=None,
         multiple=None,
         num_hidden_layers=6,
         num_attention_heads=12,
         intermediate_size=40,
         hidden_act="gelu",
-        hidden_dropout_prob=0.0,
-        attention_probs_dropout_prob=0.0,
+        hidden_dropout=0.0,
+        attention_dropout=0.0,
         max_position_embeddings=440,
         initializer_range=0.02,
         layer_norm_eps=1e-12,
-        pad_token_id=0,
         position_embedding_type="absolute",
         use_cache=True,
+        head=None,
+        lm_head=None,
         **kwargs,
     ):
-        super().__init__(pad_token_id=pad_token_id, **kwargs)
+        if hidden_size is None:
+            hidden_size = num_attention_heads * multiple if multiple is not None else 120
+        if head is None:
+            head = {}
+        head.setdefault("hidden_size", hidden_size)
+        if "problem_type" in kwargs:
+            head.setdefault("problem_type", kwargs["problem_type"])
+        if "num_labels" in kwargs:
+            head.setdefault("num_labels", kwargs["num_labels"])
+        if lm_head is None:
+            lm_head = {}
+        lm_head.setdefault("hidden_size", hidden_size)
+        super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
         self.ss_vocab_size = ss_vocab_size
-        if hidden_size is None:
-            hidden_size = num_attention_heads * multiple if multiple is not None else 120
+        self.type_vocab_size = 2
         self.hidden_size = hidden_size
         self.num_hidden_layers = num_hidden_layers
         self.num_attention_heads = num_attention_heads
         self.intermediate_size = intermediate_size
         self.hidden_act = hidden_act
-        self.hidden_dropout_prob = hidden_dropout_prob
-        self.attention_probs_dropout_prob = attention_probs_dropout_prob
+        self.hidden_dropout = hidden_dropout
+        self.attention_dropout = attention_dropout
         self.max_position_embeddings = max_position_embeddings
         self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
         self.position_embedding_type = position_embedding_type
         self.use_cache = use_cache
+        self.head = HeadConfig(**head)
+        self.lm_head = MaskedLMHeadConfig(**lm_head)
```

### Comparing `multimolecule-0.0.1/multimolecule/tokenizers/rna/config.py` & `multimolecule-0.0.2/multimolecule/tokenizers/rna/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,44 @@
-def get_vocab_list():
-    return VOCAB_LIST
+from ..utils import generate_kmer_vocabulary
+
+
+def get_vocab_list(nmers: int = 1, strameline: bool = False):
+    vocab_list = STRAMELINE_VOCAB_LIST if strameline else VOCAB_LIST
+    if nmers > 1:
+        return generate_kmer_vocabulary(vocab_list, nmers)
+    return vocab_list
 
 
 def get_special_tokens_map():
     return SPECIAL_TOKENS_MAP
 
 
 def get_tokenizer_config():
     config = TOKENIZER_CONFIG
     config.setdefault("added_tokens_decoder", {})
     for i, v in enumerate(SPECIAL_TOKENS_MAP.values()):
         config["added_tokens_decoder"][str(i)] = v
     return config
 
 
+STRAMELINE_VOCAB_LIST = [
+    "<pad>",
+    "<cls>",
+    "<eos>",
+    "<unk>",
+    "<mask>",
+    "<null>",
+    "A",
+    "C",
+    "G",
+    "U",
+    "N",
+]
+
+
 VOCAB_LIST = [
     "<pad>",
     "<cls>",
     "<eos>",
     "<unk>",
     "<mask>",
     "<null>",
```

### Comparing `multimolecule-0.0.1/multimolecule/tokenizers/rna/tokenization_rna.py` & `multimolecule-0.0.2/multimolecule/tokenizers/rna/tokenization_rna.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import os
 from typing import List, Optional
 
 from transformers.tokenization_utils import PreTrainedTokenizer
 from transformers.utils import logging
 
-from .config import VOCAB_LIST
+from .utils import get_vocab_list
 
 logger = logging.get_logger(__name__)
 
 
 class RnaTokenizer(PreTrainedTokenizer):
     """
     Constructs an RnaBert tokenizer.
     """
 
     model_input_names = ["input_ids", "attention_mask"]
 
     def __init__(
         self,
-        cls_token="<cls>",
-        pad_token="<pad>",
-        eos_token="<eos>",
-        sep_token="<eos>",
-        unk_token="<unk>",
-        mask_token="<mask>",
-        convert_to_uppercase=True,
-        convert_T_to_U=True,
+        bos_token: str = "<cls>",
+        cls_token: str = "<cls>",
+        pad_token: str = "<pad>",
+        eos_token: str = "<eos>",
+        sep_token: str = "<eos>",
+        unk_token: str = "<unk>",
+        mask_token: str = "<mask>",
+        convert_to_uppercase: bool = True,
+        convert_T_to_U: bool = True,
+        nmers: int = 1,
+        strameline: bool = False,
         **kwargs,
     ):
-        self.all_tokens = VOCAB_LIST
+        self.nmers = nmers
+        self.all_tokens = get_vocab_list(nmers, strameline)
         self._id_to_token = dict(enumerate(self.all_tokens))
         self._token_to_id = {tok: ind for ind, tok in enumerate(self.all_tokens)}
         self.convert_to_uppercase = convert_to_uppercase
         self.convert_T_to_U = convert_T_to_U
         super().__init__(
+            bos_token=bos_token,
             cls_token=cls_token,
             pad_token=pad_token,
             eos_token=eos_token,
             sep_token=sep_token,
             unk_token=unk_token,
             mask_token=mask_token,
             **kwargs,
@@ -49,30 +54,32 @@
         # self.unique_no_split_tokens = self.all_tokens
         # self._update_trie(self.unique_no_split_tokens)
 
     def _convert_id_to_token(self, index: int) -> str:
         return self._id_to_token.get(index, self.unk_token)
 
     def _convert_token_to_id(self, token: str) -> int:
-        return self._token_to_id.get(token, self._token_to_id.get(self.unk_token))
+        return self._token_to_id.get(token, self._token_to_id.get(self.unk_token))  # type: ignore[arg-type]
 
     def _tokenize(self, text: str, **kwargs):
         if self.convert_to_uppercase:
             text = text.upper()
         if self.convert_T_to_U:
             text = text.replace("T", "U")
+        if self.nmers > 1:
+            return [text[i : i + self.nmers] for i in range(len(text) - self.nmers + 1)]  # noqa: E203
         return list(text)
 
     def get_vocab(self):
         base_vocab = self._token_to_id.copy()
         base_vocab.update(self.added_tokens_encoder)
         return base_vocab
 
     def token_to_id(self, token: str) -> int:
-        return self._token_to_id.get(token, self._token_to_id.get(self.unk_token))
+        return self._token_to_id.get(token, self._token_to_id.get(self.unk_token))  # type: ignore[arg-type]
 
     def id_to_token(self, index: int) -> str:
         return self._id_to_token.get(index, self.unk_token)
 
     def build_inputs_with_special_tokens(
         self, token_ids_0: List[int], token_ids_1: Optional[List[int]] = None
     ) -> List[int]:
```

### Comparing `multimolecule-0.0.1/multimolecule.egg-info/PKG-INFO` & `multimolecule-0.0.2/multimolecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimolecule
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Networks for RNA, DNA, and Protein.
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,7 +682,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chanfig>=0.0.99
+Requires-Dist: transformers
```

### Comparing `multimolecule-0.0.1/multimolecule.egg-info/SOURCES.txt` & `multimolecule-0.0.2/multimolecule.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,42 @@
 .github/merge_rules.yaml
 .github/workflows/push.yaml
 multimolecule/__init__.py
 multimolecule/_version.py
 multimolecule.egg-info/PKG-INFO
 multimolecule.egg-info/SOURCES.txt
 multimolecule.egg-info/dependency_links.txt
+multimolecule.egg-info/requires.txt
 multimolecule.egg-info/top_level.txt
 multimolecule/models/__init__.py
+multimolecule/models/configuration_utils.py
+multimolecule/models/modeling_utils.py
 multimolecule/models/rnabert/__init__.py
 multimolecule/models/rnabert/configuration_rnabert.py
 multimolecule/models/rnabert/convert_checkpoint.py
 multimolecule/models/rnabert/modeling_rnabert.py
+multimolecule/models/rnafm/__init__.py
+multimolecule/models/rnafm/configuration_rnafm.py
+multimolecule/models/rnafm/convert_checkpoint.py
+multimolecule/models/rnafm/modeling_rnafm.py
+multimolecule/models/rnamsm/__init__.py
+multimolecule/models/rnamsm/configuration_rnamsm.py
+multimolecule/models/rnamsm/convert_checkpoint.py
+multimolecule/models/rnamsm/modeling_rnamsm.py
+multimolecule/models/splicebert/__init__.py
+multimolecule/models/splicebert/configuration_splicebert.py
+multimolecule/models/splicebert/convert_checkpoint.py
+multimolecule/models/splicebert/modeling_splicebert.py
+multimolecule/models/utrbert/__init__.py
+multimolecule/models/utrbert/configuration_utrbert.py
+multimolecule/models/utrbert/convert_checkpoint.py
+multimolecule/models/utrbert/modeling_utrbert.py
+multimolecule/models/utrlm/__init__.py
+multimolecule/models/utrlm/configuration_utrlm.py
+multimolecule/models/utrlm/convert_checkpoint.py
+multimolecule/models/utrlm/modeling_utrlm.py
 multimolecule/tokenizers/__init__.py
+multimolecule/tokenizers/utils.py
 multimolecule/tokenizers/rna/__init__.py
-multimolecule/tokenizers/rna/config.py
 multimolecule/tokenizers/rna/tokenization_rna.py
+multimolecule/tokenizers/rna/utils.py
 multimolecule/tokenizers/rna/vocab.txt
```

### Comparing `multimolecule-0.0.1/pyproject.toml` & `multimolecule-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,18 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = [
   "version",
 ]
+dependencies = [
+  "chanfig>=0.0.99",
+  "transformers",
+]
 [project.urls]
 documentation = "https://multimolecule.danling.org"
 homepage = "https://multimolecule.danling.org"
 repository = "https://github.com/DLS5-Omics/multimolecule"
 
 [tool.setuptools]
 packages = ["multimolecule"]
```

