# Comparing `tmp/TorchFix-0.4.0.tar.gz` & `tmp/torchfix-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchFix-0.4.0.tar", last modified: Wed Feb  7 19:06:42 2024, max compression
+gzip compressed data, was "torchfix-0.5.0.tar", last modified: Thu Apr 18 18:15:29 2024, max compression
```

## Comparing `TorchFix-0.4.0.tar` & `torchfix-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.818054 TorchFix-0.4.0/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1535 2024-02-07 19:04:52.000000 TorchFix-0.4.0/LICENSE
--rw-r--r--   0 sdym      (1000) sdym      (1000)     6611 2024-02-07 19:06:42.817054 TorchFix-0.4.0/PKG-INFO
--rw-r--r--   0 sdym      (1000) sdym      (1000)     4302 2024-02-07 19:04:52.000000 TorchFix-0.4.0/README.md
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.817054 TorchFix-0.4.0/TorchFix.egg-info/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     6611 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/PKG-INFO
--rw-r--r--   0 sdym      (1000) sdym      (1000)      873 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/SOURCES.txt
--rw-r--r--   0 sdym      (1000) sdym      (1000)        1 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/dependency_links.txt
--rw-r--r--   0 sdym      (1000) sdym      (1000)      109 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/entry_points.txt
--rw-r--r--   0 sdym      (1000) sdym      (1000)       42 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/requires.txt
--rw-r--r--   0 sdym      (1000) sdym      (1000)        9 2024-02-07 19:06:42.000000 TorchFix-0.4.0/TorchFix.egg-info/top_level.txt
--rw-r--r--   0 sdym      (1000) sdym      (1000)      950 2024-02-07 19:04:52.000000 TorchFix-0.4.0/pyproject.toml
--rw-r--r--   0 sdym      (1000) sdym      (1000)       38 2024-02-07 19:06:42.818054 TorchFix-0.4.0/setup.cfg
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.815054 TorchFix-0.4.0/tests/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     2613 2024-02-07 19:04:52.000000 TorchFix-0.4.0/tests/test_torchfix.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.815054 TorchFix-0.4.0/torchfix/
--rw-r--r--   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/__init__.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     4022 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/__main__.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     4876 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/common.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     2204 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/deprecated_symbols.yaml
--rw-r--r--   0 sdym      (1000) sdym      (1000)     7690 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/torchfix.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.813054 TorchFix-0.4.0/torchfix/visitors/
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.816054 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     4154 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/__init__.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)      880 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/chain_matmul.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1230 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/cholesky.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1160 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/qr.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     4259 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/range.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.816054 TorchFix-0.4.0/torchfix/visitors/internal/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1099 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/internal/__init__.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.816054 TorchFix-0.4.0/torchfix/visitors/misc/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     3207 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/misc/__init__.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.817054 TorchFix-0.4.0/torchfix/visitors/performance/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1479 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/performance/__init__.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.817054 TorchFix-0.4.0/torchfix/visitors/security/
--rw-r--r--   0 sdym      (1000) sdym      (1000)     2318 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/security/__init__.py
-drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-02-07 19:06:42.817054 TorchFix-0.4.0/torchfix/visitors/vision/
--rw-r--r--   0 sdym      (1000) sdym      (1000)      151 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/vision/__init__.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)    16086 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/vision/pretrained.py
--rw-r--r--   0 sdym      (1000) sdym      (1000)     1713 2024-02-07 19:04:52.000000 TorchFix-0.4.0/torchfix/visitors/vision/to_tensor.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.812606 torchfix-0.5.0/
+-rw-rw-r--   0 sdym      (1000) sdym      (1000)     1535 2023-11-23 01:16:48.000000 torchfix-0.5.0/LICENSE
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     6629 2024-04-18 18:15:29.812606 torchfix-0.5.0/PKG-INFO
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     4320 2024-03-14 21:35:36.000000 torchfix-0.5.0/README.md
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.812606 torchfix-0.5.0/TorchFix.egg-info/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     6629 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/PKG-INFO
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      955 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/SOURCES.txt
+-rw-r--r--   0 sdym      (1000) sdym      (1000)        1 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/dependency_links.txt
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      109 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/entry_points.txt
+-rw-r--r--   0 sdym      (1000) sdym      (1000)       42 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/requires.txt
+-rw-r--r--   0 sdym      (1000) sdym      (1000)        9 2024-04-18 18:15:29.000000 torchfix-0.5.0/TorchFix.egg-info/top_level.txt
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      950 2024-02-01 01:48:04.000000 torchfix-0.5.0/pyproject.toml
+-rw-r--r--   0 sdym      (1000) sdym      (1000)       38 2024-04-18 18:15:29.812606 torchfix-0.5.0/setup.cfg
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.808606 torchfix-0.5.0/tests/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     2731 2024-03-15 17:37:55.000000 torchfix-0.5.0/tests/test_torchfix.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.809606 torchfix-0.5.0/torchfix/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)        0 2023-11-23 00:37:50.000000 torchfix-0.5.0/torchfix/__init__.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     4022 2024-03-08 02:07:27.000000 torchfix-0.5.0/torchfix/__main__.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     5507 2024-03-15 19:44:02.000000 torchfix-0.5.0/torchfix/common.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     2310 2024-03-19 01:16:18.000000 torchfix-0.5.0/torchfix/deprecated_symbols.yaml
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     7818 2024-04-18 18:07:18.000000 torchfix-0.5.0/torchfix/torchfix.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.807606 torchfix-0.5.0/torchfix/visitors/
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.810606 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     4873 2024-04-17 23:49:15.000000 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/__init__.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      880 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/chain_matmul.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1228 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/cholesky.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1158 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/qr.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     4260 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/deprecated_symbols/range.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.810606 torchfix-0.5.0/torchfix/visitors/internal/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      641 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/internal/__init__.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.810606 torchfix-0.5.0/torchfix/visitors/misc/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     2512 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/misc/__init__.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.811606 torchfix-0.5.0/torchfix/visitors/nonpublic/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     3761 2024-04-17 23:49:15.000000 torchfix-0.5.0/torchfix/visitors/nonpublic/__init__.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.811606 torchfix-0.5.0/torchfix/visitors/performance/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1011 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/performance/__init__.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.811606 torchfix-0.5.0/torchfix/visitors/security/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1949 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/security/__init__.py
+drwxr-xr-x   0 sdym      (1000) sdym      (1000)        0 2024-04-18 18:15:29.811606 torchfix-0.5.0/torchfix/visitors/vision/
+-rw-r--r--   0 sdym      (1000) sdym      (1000)      223 2024-03-06 00:45:59.000000 torchfix-0.5.0/torchfix/visitors/vision/__init__.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1222 2024-04-17 23:49:15.000000 torchfix-0.5.0/torchfix/visitors/vision/models_import.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)    15719 2024-03-15 22:08:01.000000 torchfix-0.5.0/torchfix/visitors/vision/pretrained.py
+-rw-r--r--   0 sdym      (1000) sdym      (1000)     1331 2024-03-15 23:16:00.000000 torchfix-0.5.0/torchfix/visitors/vision/to_tensor.py
```

### Comparing `TorchFix-0.4.0/LICENSE` & `torchfix-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TorchFix-0.4.0/PKG-INFO` & `torchfix-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchFix
-Version: 0.4.0
+Version: 0.5.0
 Summary: TorchFix - a linter for PyTorch-using code with autofix support
 License: BSD License
         
         For TorchFix software
         
         Copyright (c) Facebook, Inc. and its affiliates. All rights reserved.
         
@@ -55,15 +55,16 @@
 TorchFix is built upon https://github.com/Instagram/LibCST - a library to manipulate
 Python concrete syntax trees. LibCST enables "codemods" (autofixes) in addition to
 reporting issues.
 
 TorchFix can be used as a Flake8 plugin (linting only) or as a standalone
 program (with autofix available for a subset of the lint violations).
 
-Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
+> [!WARNING]
+> Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
 edges and many things can and will change.
 
 ## Installation
 
 To install the latest code from GitHub, clone/download
 https://github.com/pytorch-labs/torchfix and run `pip install .`
 inside the directory.
@@ -78,15 +79,16 @@
 To see only TorchFix warnings without the rest of the Flake8 linters, you can run
 `flake8 --isolated --select=TOR0,TOR1,TOR2`
 
 TorchFix can also be run as a standalone program: `torchfix .`
 Add `--fix` parameter to try to autofix some of the issues (the files will be overwritten!)
 To see some additional debug info, add `--show-stderr` parameter.
 
-Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
+> [!CAUTION]
+> Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
 and especially the beta version status of TorchFix, it's very difficult to have
 certainty when making changes to code, even for the seemingly trivial fixes.
 
 Warnings for issues with codes starting with TOR0, TOR1, and TOR2 are enabled by default.
 Warnings with other codes may be too noisy, so not enabled by default.
 To enable them, use standard flake8 configuration options for the plugin mode or use
 `torchfix --select=ALL .` for the standalone mode.
@@ -125,17 +127,17 @@
 See this [forum post](https://dev-discuss.pytorch.org/t/bc-breaking-update-to-torch-utils-checkpoint-not-passing-in-use-reentrant-flag-will-raise-an-error/1745)
 for details.
 
 ### TOR101 Use of deprecated function
 
 #### torch.nn.utils.weight_norm
 
-This function is deprecated. Use :func:`torch.nn.utils.parametrizations.weight_norm`
-which uses the modern parametrization API. The new ``weight_norm`` is compatible
-with ``state_dict`` generated from old ``weight_norm``.
+This function is deprecated. Use `torch.nn.utils.parametrizations.weight_norm`
+which uses the modern parametrization API. The new `weight_norm` is compatible
+with `state_dict` generated from old `weight_norm`.
 
 Migration guide:
 
 * The magnitude (``weight_g``) and direction (``weight_v``) are now expressed
     as ``parametrizations.weight.original0`` and ``parametrizations.weight.original1``
     respectively.
```

### Comparing `TorchFix-0.4.0/README.md` & `torchfix-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 TorchFix is built upon https://github.com/Instagram/LibCST - a library to manipulate
 Python concrete syntax trees. LibCST enables "codemods" (autofixes) in addition to
 reporting issues.
 
 TorchFix can be used as a Flake8 plugin (linting only) or as a standalone
 program (with autofix available for a subset of the lint violations).
 
-Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
+> [!WARNING]
+> Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
 edges and many things can and will change.
 
 ## Installation
 
 To install the latest code from GitHub, clone/download
 https://github.com/pytorch-labs/torchfix and run `pip install .`
 inside the directory.
@@ -32,15 +33,16 @@
 To see only TorchFix warnings without the rest of the Flake8 linters, you can run
 `flake8 --isolated --select=TOR0,TOR1,TOR2`
 
 TorchFix can also be run as a standalone program: `torchfix .`
 Add `--fix` parameter to try to autofix some of the issues (the files will be overwritten!)
 To see some additional debug info, add `--show-stderr` parameter.
 
-Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
+> [!CAUTION]
+> Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
 and especially the beta version status of TorchFix, it's very difficult to have
 certainty when making changes to code, even for the seemingly trivial fixes.
 
 Warnings for issues with codes starting with TOR0, TOR1, and TOR2 are enabled by default.
 Warnings with other codes may be too noisy, so not enabled by default.
 To enable them, use standard flake8 configuration options for the plugin mode or use
 `torchfix --select=ALL .` for the standalone mode.
@@ -79,17 +81,17 @@
 See this [forum post](https://dev-discuss.pytorch.org/t/bc-breaking-update-to-torch-utils-checkpoint-not-passing-in-use-reentrant-flag-will-raise-an-error/1745)
 for details.
 
 ### TOR101 Use of deprecated function
 
 #### torch.nn.utils.weight_norm
 
-This function is deprecated. Use :func:`torch.nn.utils.parametrizations.weight_norm`
-which uses the modern parametrization API. The new ``weight_norm`` is compatible
-with ``state_dict`` generated from old ``weight_norm``.
+This function is deprecated. Use `torch.nn.utils.parametrizations.weight_norm`
+which uses the modern parametrization API. The new `weight_norm` is compatible
+with `state_dict` generated from old `weight_norm`.
 
 Migration guide:
 
 * The magnitude (``weight_g``) and direction (``weight_v``) are now expressed
     as ``parametrizations.weight.original0`` and ``parametrizations.weight.original1``
     respectively.
```

### Comparing `TorchFix-0.4.0/TorchFix.egg-info/PKG-INFO` & `torchfix-0.5.0/TorchFix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchFix
-Version: 0.4.0
+Version: 0.5.0
 Summary: TorchFix - a linter for PyTorch-using code with autofix support
 License: BSD License
         
         For TorchFix software
         
         Copyright (c) Facebook, Inc. and its affiliates. All rights reserved.
         
@@ -55,15 +55,16 @@
 TorchFix is built upon https://github.com/Instagram/LibCST - a library to manipulate
 Python concrete syntax trees. LibCST enables "codemods" (autofixes) in addition to
 reporting issues.
 
 TorchFix can be used as a Flake8 plugin (linting only) or as a standalone
 program (with autofix available for a subset of the lint violations).
 
-Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
+> [!WARNING]
+> Currently TorchFix is in a **beta version** stage, so there are still a lot of rough
 edges and many things can and will change.
 
 ## Installation
 
 To install the latest code from GitHub, clone/download
 https://github.com/pytorch-labs/torchfix and run `pip install .`
 inside the directory.
@@ -78,15 +79,16 @@
 To see only TorchFix warnings without the rest of the Flake8 linters, you can run
 `flake8 --isolated --select=TOR0,TOR1,TOR2`
 
 TorchFix can also be run as a standalone program: `torchfix .`
 Add `--fix` parameter to try to autofix some of the issues (the files will be overwritten!)
 To see some additional debug info, add `--show-stderr` parameter.
 
-Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
+> [!CAUTION]
+> Please keep in mind that autofix is a best-effort mechanism. Given the dynamic nature of Python,
 and especially the beta version status of TorchFix, it's very difficult to have
 certainty when making changes to code, even for the seemingly trivial fixes.
 
 Warnings for issues with codes starting with TOR0, TOR1, and TOR2 are enabled by default.
 Warnings with other codes may be too noisy, so not enabled by default.
 To enable them, use standard flake8 configuration options for the plugin mode or use
 `torchfix --select=ALL .` for the standalone mode.
@@ -125,17 +127,17 @@
 See this [forum post](https://dev-discuss.pytorch.org/t/bc-breaking-update-to-torch-utils-checkpoint-not-passing-in-use-reentrant-flag-will-raise-an-error/1745)
 for details.
 
 ### TOR101 Use of deprecated function
 
 #### torch.nn.utils.weight_norm
 
-This function is deprecated. Use :func:`torch.nn.utils.parametrizations.weight_norm`
-which uses the modern parametrization API. The new ``weight_norm`` is compatible
-with ``state_dict`` generated from old ``weight_norm``.
+This function is deprecated. Use `torch.nn.utils.parametrizations.weight_norm`
+which uses the modern parametrization API. The new `weight_norm` is compatible
+with `state_dict` generated from old `weight_norm`.
 
 Migration guide:
 
 * The magnitude (``weight_g``) and direction (``weight_v``) are now expressed
     as ``parametrizations.weight.original0`` and ``parametrizations.weight.original1``
     respectively.
```

### Comparing `TorchFix-0.4.0/TorchFix.egg-info/SOURCES.txt` & `torchfix-0.5.0/TorchFix.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,14 @@
 torchfix/visitors/deprecated_symbols/__init__.py
 torchfix/visitors/deprecated_symbols/chain_matmul.py
 torchfix/visitors/deprecated_symbols/cholesky.py
 torchfix/visitors/deprecated_symbols/qr.py
 torchfix/visitors/deprecated_symbols/range.py
 torchfix/visitors/internal/__init__.py
 torchfix/visitors/misc/__init__.py
+torchfix/visitors/nonpublic/__init__.py
 torchfix/visitors/performance/__init__.py
 torchfix/visitors/security/__init__.py
 torchfix/visitors/vision/__init__.py
+torchfix/visitors/vision/models_import.py
 torchfix/visitors/vision/pretrained.py
 torchfix/visitors/vision/to_tensor.py
```

### Comparing `TorchFix-0.4.0/pyproject.toml` & `torchfix-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TorchFix-0.4.0/tests/test_torchfix.py` & `torchfix-0.5.0/tests/test_torchfix.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 def _codemod_results(source_path):
     with open(source_path) as source:
         code = source.read()
     config = TorchCodemodConfig(select=list(GET_ALL_ERROR_CODES()))
     context = TorchCodemod(codemod.CodemodContext(filename=source_path), config)
     new_module = codemod.transform_module(context, code)
+    if isinstance(new_module, codemod.TransformFailure):
+        raise new_module.error
     return new_module.code
 
 
 def test_empty():
     assert _checker_results([""]) == []
 
 
@@ -69,12 +71,12 @@
 def test_parse_error_code_str():
     exclude_set = expand_error_codes(tuple(DISABLED_BY_DEFAULT))
     cases = [
         ("ALL", GET_ALL_ERROR_CODES()),
         ("ALL,TOR102", GET_ALL_ERROR_CODES()),
         ("TOR102", {"TOR102"}),
         ("TOR102,TOR101", {"TOR102", "TOR101"}),
-        ("TOR1,TOR102", {"TOR102", "TOR101"}),
+        ("TOR1,TOR102", {"TOR102", "TOR101", "TOR103", "TOR104", "TOR105"}),
         (None, GET_ALL_ERROR_CODES() - exclude_set),
     ]
     for case, expected in cases:
         assert expected == process_error_code_str(case)
```

### Comparing `TorchFix-0.4.0/torchfix/__main__.py` & `torchfix-0.5.0/torchfix/__main__.py`

 * *Files identical despite different names*

### Comparing `TorchFix-0.4.0/torchfix/common.py` & `torchfix-0.5.0/torchfix/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,35 @@
                 if curr_pos == arg_pos:
                     return arg
                 curr_pos += 1
             elif arg.keyword.value == arg_name:
                 return arg
         return None
 
+    def add_violation(
+        self,
+        node: cst.CSTNode,
+        error_code: str,
+        message: str,
+        replacement: Optional[cst.CSTNode] = None,
+    ) -> None:
+        position_metadata = self.get_metadata(
+            cst.metadata.WhitespaceInclusivePositionProvider, node
+        )
+        self.violations.append(
+            LintViolation(
+                error_code=error_code,
+                message=message,
+                line=position_metadata.start.line,
+                column=position_metadata.start.column,
+                node=node,
+                replacement=replacement,
+            )
+        )
+
     def get_qualified_name_for_call(self, node: cst.Call) -> Optional[str]:
         # Guard against situations like `vmap(a)(b)`:
         #
         # Call(
         #   func=Call(
         #       func=Name(
         #         value='vmap',
```

### Comparing `TorchFix-0.4.0/torchfix/deprecated_symbols.yaml` & `torchfix-0.5.0/torchfix/deprecated_symbols.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 - name: torch.nn.UpsamplingBilinear2d
   deprecate_pr: TBA
   remove_pr:
 
 - name: torch.testing.assert_allclose
   deprecate_pr: TBA
   remove_pr:
+  replacement: torch.testing.assert_allclose
+  reference: https://github.com/pytorch/pytorch/issues/61844
 
 - name: torch.nn.utils.weight_norm
   deprecate_pr: https://github.com/pytorch/pytorch/pull/103001
   remove_pr:
   reference: https://github.com/pytorch-labs/torchfix#torchnnutilsweight_norm
 
 # functorch
```

### Comparing `TorchFix-0.4.0/torchfix/torchfix.py` & `torchfix-0.5.0/torchfix/torchfix.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,36 +11,40 @@
     _UpdateFunctorchImports,
 )
 
 from .visitors.internal import TorchScopedLibraryVisitor
 
 from .visitors.performance import TorchSynchronizedDataLoaderVisitor
 from .visitors.misc import (TorchRequireGradVisitor, TorchReentrantCheckpointVisitor)
+from .visitors.nonpublic import TorchNonPublicAliasVisitor
 
 from .visitors.vision import (
     TorchVisionDeprecatedPretrainedVisitor,
     TorchVisionDeprecatedToTensorVisitor,
+    TorchVisionModelsImportVisitor,
 )
 from .visitors.security import TorchUnsafeLoadVisitor
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
-DEPRECATED_CONFIG_PATH = Path(__file__).absolute().parent / "deprecated_symbols.yaml"
+DEPRECATED_CONFIG_PATH = "deprecated_symbols.yaml"
 
 DISABLED_BY_DEFAULT = ["TOR3", "TOR4", "TOR9"]
 
 ALL_VISITOR_CLS = [
     TorchDeprecatedSymbolsVisitor,
     TorchRequireGradVisitor,
     TorchScopedLibraryVisitor,
     TorchSynchronizedDataLoaderVisitor,
     TorchVisionDeprecatedPretrainedVisitor,
     TorchVisionDeprecatedToTensorVisitor,
+    TorchVisionModelsImportVisitor,
     TorchUnsafeLoadVisitor,
     TorchReentrantCheckpointVisitor,
+    TorchNonPublicAliasVisitor,
 ]
 
 
 @functools.cache
 def GET_ALL_ERROR_CODES():
     codes = set()
     for cls in ALL_VISITOR_CLS:
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/__init__.py` & `torchfix-0.5.0/torchfix/visitors/deprecated_symbols/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import libcst as cst
+import pkgutil
 import yaml
 from typing import Optional
 from collections.abc import Sequence
 
 from ...common import (
     TorchVisitor,
     call_with_name_changes,
-    LintViolation,
 )
 
 from .range import call_replacement_range
 from .cholesky import call_replacement_cholesky
 from .chain_matmul import call_replacement_chain_matmul
 from .qr import call_replacement_qr
 
 
 class TorchDeprecatedSymbolsVisitor(TorchVisitor):
-    ERROR_CODE = ["TOR001", "TOR101"]
+    ERROR_CODE = ["TOR001", "TOR101", "TOR004", "TOR103"]
 
     def __init__(self, deprecated_config_path=None):
         def read_deprecated_config(path=None):
             deprecated_config = {}
             if path is not None:
-                with open(path) as f:
-                    for item in yaml.load(f, yaml.SafeLoader):
-                        deprecated_config[item["name"]] = item
+                data = pkgutil.get_data("torchfix", path)
+                for item in yaml.load(data, yaml.SafeLoader):
+                    deprecated_config[item["name"]] = item
             return deprecated_config
 
         super().__init__()
         self.deprecated_config = read_deprecated_config(deprecated_config_path)
 
     def _call_replacement(
         self, node: cst.Call, qualified_name: str
@@ -53,44 +53,56 @@
                     node, qualified_name, function_name_replacement
                 )
                 if replacement_and_imports is not None:
                     replacement, imports = replacement_and_imports
                     self.needed_imports.update(imports)
         return replacement
 
-    def visit_Call(self, node):
+    def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
+        if node.module is None:
+            return
+
+        module = cst.helpers.get_full_name_for_node(node.module)
+        if isinstance(node.names, Sequence):
+            for name in node.names:
+                qualified_name = f"{module}.{name.name.value}"
+                if qualified_name in self.deprecated_config:
+                    if self.deprecated_config[qualified_name]["remove_pr"] is None:
+                        error_code = self.ERROR_CODE[3]
+                        message = f"Import of deprecated function {qualified_name}"
+                    else:
+                        error_code = self.ERROR_CODE[2]
+                        message = f"Import of removed function {qualified_name}"
+
+                    reference = self.deprecated_config[qualified_name].get("reference")
+                    if reference is not None:
+                        message = f"{message}: {reference}"
+
+                    self.add_violation(node, error_code=error_code, message=message)
+
+    def visit_Call(self, node) -> None:
         qualified_name = self.get_qualified_name_for_call(node)
         if qualified_name is None:
             return
 
         if qualified_name in self.deprecated_config:
-            position_metadata = self.get_metadata(
-                cst.metadata.WhitespaceInclusivePositionProvider, node
-            )
             if self.deprecated_config[qualified_name]["remove_pr"] is None:
                 error_code = self.ERROR_CODE[1]
                 message = f"Use of deprecated function {qualified_name}"
             else:
                 error_code = self.ERROR_CODE[0]
                 message = f"Use of removed function {qualified_name}"
             replacement = self._call_replacement(node, qualified_name)
 
             reference = self.deprecated_config[qualified_name].get("reference")
             if reference is not None:
                 message = f"{message}: {reference}"
 
-            self.violations.append(
-                LintViolation(
-                    error_code=error_code,
-                    message=message,
-                    line=position_metadata.start.line,
-                    column=position_metadata.start.column,
-                    node=node,
-                    replacement=replacement,
-                )
+            self.add_violation(
+                node, error_code=error_code, message=message, replacement=replacement
             )
 
 
 # TODO: refactor/generalize this.
 class _UpdateFunctorchImports(cst.CSTTransformer):
     REPLACEMENTS = {
         "vmap",
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/chain_matmul.py` & `torchfix-0.5.0/torchfix/visitors/deprecated_symbols/chain_matmul.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,12 +16,12 @@
             out_arg = arg
     matrices_arg = cst.Arg(value=cst.List(elements=matrices))
 
     if out_arg is None:
         replacement_args = [matrices_arg]
     else:
         replacement_args = [matrices_arg, out_arg]
-    module_name = get_module_name(node, 'torch')
+    module_name = get_module_name(node, "torch")
     replacement = cst.parse_expression(f"{module_name}.linalg.multi_dot(args)")
     replacement = replacement.with_changes(args=replacement_args)
 
     return replacement
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/cholesky.py` & `torchfix-0.5.0/torchfix/visitors/deprecated_symbols/cholesky.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import libcst as cst
-from ...common import (TorchVisitor, get_module_name)
+from ...common import TorchVisitor, get_module_name
 
 
 def call_replacement_cholesky(node: cst.Call) -> cst.CSTNode:
     """
     Replace `torch.cholesky(A)` with `torch.linalg.cholesky(A)` and
     `torch.cholesky(A, upper=True)` with `torch.linalg.cholesky(A).mH`.
     """
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/qr.py` & `torchfix-0.5.0/torchfix/visitors/deprecated_symbols/qr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import libcst as cst
 from typing import Optional
-from ...common import (TorchVisitor, get_module_name)
+from ...common import TorchVisitor, get_module_name
 
 
 def call_replacement_qr(node: cst.Call) -> Optional[cst.CSTNode]:
     """
     Replace `torch.qr(A)` with `torch.linalg.qr(A)` and
     `torch.qr(A, some=False)` with `torch.linalg.qr(A, mode="complete")`.
     """
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/deprecated_symbols/range.py` & `torchfix-0.5.0/torchfix/visitors/deprecated_symbols/range.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, Tuple
 
 
 def call_replacement_range(node: cst.Call) -> Optional[cst.Call]:
     """Replace `range` with `arange`.
     Add `step` to the `end` argument as `arange` has the interval `[start, end)`.
     """
+
     # `torch.range` documented signature is not a valid Python signature,
     # so it's hard to generalize this.
     def _get_range_args(node: cst.Call) -> Tuple[cst.Arg, Optional[cst.Arg]]:
         "Return (`end`, `step`) from a `range` call"
         end_arg = None
         step_arg = None
         non_kw_args = []
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/misc/__init__.py` & `torchfix-0.5.0/torchfix/visitors/misc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import libcst as cst
 import libcst.matchers as m
 
 
-from ...common import TorchVisitor, LintViolation
+from ...common import TorchVisitor
 
 
 class TorchRequireGradVisitor(TorchVisitor):
     """
     Find and fix common misspelling `require_grad` (instead of `requires_grad`).
     """
 
@@ -27,28 +27,19 @@
                     )
                 ],
             ),
         ):
             replacement = node.with_deep_changes(
                 old_node=node.targets[0].target.attr, value="requires_grad"
             )
-
-            position_metadata = self.get_metadata(
-                cst.metadata.WhitespaceInclusivePositionProvider, node
-            )
-
-            self.violations.append(
-                LintViolation(
-                    error_code=self.ERROR_CODE,
-                    message=self.MESSAGE,
-                    line=position_metadata.start.line,
-                    column=position_metadata.start.column,
-                    node=node,
-                    replacement=replacement,
-                )
+            self.add_violation(
+                node,
+                error_code=self.ERROR_CODE,
+                message=self.MESSAGE,
+                replacement=replacement,
             )
 
 
 class TorchReentrantCheckpointVisitor(TorchVisitor):
     """
     Find and fix common misuse of reentrant checkpoints.
     """
@@ -61,29 +52,20 @@
     )
 
     def visit_Call(self, node):
         qualified_name = self.get_qualified_name_for_call(node)
         if qualified_name == "torch.utils.checkpoint.checkpoint":
             use_reentrant_arg = self.get_specific_arg(node, "use_reentrant", -1)
             if use_reentrant_arg is None:
-                position_metadata = self.get_metadata(
-                    cst.metadata.WhitespaceInclusivePositionProvider, node
-                )
-
                 # This codemod maybe  unsafe correctness-wise
                 # if reentrant behavior is actually needed,
                 # so the changes need to be verified/tested.
                 use_reentrant_arg = cst.ensure_type(
                     cst.parse_expression("f(use_reentrant=False)"), cst.Call
                 ).args[0]
                 replacement = node.with_changes(args=node.args + (use_reentrant_arg,))
-
-                self.violations.append(
-                    LintViolation(
-                        error_code=self.ERROR_CODE,
-                        message=self.MESSAGE,
-                        line=position_metadata.start.line,
-                        column=position_metadata.start.column,
-                        node=node,
-                        replacement=replacement,
-                    )
+                self.add_violation(
+                    node,
+                    error_code=self.ERROR_CODE,
+                    message=self.MESSAGE,
+                    replacement=replacement,
                 )
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/performance/__init__.py` & `torchfix-0.5.0/torchfix/visitors/performance/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import libcst as cst
 import libcst.matchers as m
 
 
-from ...common import TorchVisitor, LintViolation
+from ...common import TorchVisitor
 
 
 class TorchSynchronizedDataLoaderVisitor(TorchVisitor):
     """
     Reimplementation of SynchronizedDataLoaderPattern from
     https://github.com/pytorch/pytorch/blob/main/torch/profiler/_pattern_matcher.py
     """
@@ -21,21 +20,10 @@
     def visit_Call(self, node):
         qualified_name = self.get_qualified_name_for_call(node)
         if qualified_name == "torch.utils.data.DataLoader":
             num_workers_arg = self.get_specific_arg(node, "num_workers", 5)
             if num_workers_arg is None or m.matches(
                 num_workers_arg.value, m.Integer(value="0")
             ):
-                position_metadata = self.get_metadata(
-                    cst.metadata.WhitespaceInclusivePositionProvider, node
-                )
-
-                self.violations.append(
-                    LintViolation(
-                        error_code=self.ERROR_CODE,
-                        message=self.MESSAGE,
-                        line=position_metadata.start.line,
-                        column=position_metadata.start.column,
-                        node=node,
-                        replacement=None,
-                    )
+                self.add_violation(
+                    node, error_code=self.ERROR_CODE, message=self.MESSAGE
                 )
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/security/__init__.py` & `torchfix-0.5.0/torchfix/visitors/security/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import libcst as cst
-from ...common import TorchVisitor, LintViolation
+from ...common import TorchVisitor
 
 
 class TorchUnsafeLoadVisitor(TorchVisitor):
     """
     Warn on `torch.load` not having explicit `weights_only`.
     See https://github.com/pytorch/pytorch/issues/31875.
     """
@@ -17,18 +17,14 @@
     )
 
     def visit_Call(self, node):
         qualified_name = self.get_qualified_name_for_call(node)
         if qualified_name == "torch.load":
             weights_only_arg = self.get_specific_arg(node, "weights_only", -1)
             if weights_only_arg is None:
-                position_metadata = self.get_metadata(
-                    cst.metadata.WhitespaceInclusivePositionProvider, node
-                )
-
                 # Add `weights_only=True` if there is no `pickle_module`.
                 # (do not add `weights_only=False` with `pickle_module`, as it
                 # needs to be an explicit choice).
                 #
                 # This codemod is somewhat unsafe correctness-wise
                 # because full pickling functionality may still be needed
                 # even without `pickle_module`,
@@ -38,18 +34,13 @@
                 if pickle_module_arg is None:
                     weights_only_arg = cst.ensure_type(
                         cst.parse_expression("f(weights_only=True)"), cst.Call
                     ).args[0]
                     replacement = node.with_changes(
                         args=node.args + (weights_only_arg,)
                     )
-
-                self.violations.append(
-                    LintViolation(
-                        error_code=self.ERROR_CODE,
-                        message=self.MESSAGE,
-                        line=position_metadata.start.line,
-                        column=position_metadata.start.column,
-                        node=node,
-                        replacement=replacement,
-                    )
+                self.add_violation(
+                    node,
+                    error_code=self.ERROR_CODE,
+                    message=self.MESSAGE,
+                    replacement=replacement,
                 )
```

### Comparing `TorchFix-0.4.0/torchfix/visitors/vision/pretrained.py` & `torchfix-0.5.0/torchfix/visitors/vision/pretrained.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import libcst as cst
 from libcst.codemod.visitors import ImportItem
 
-from ...common import LintViolation, TorchVisitor
+from ...common import TorchVisitor
 
 
 class TorchVisionDeprecatedPretrainedVisitor(TorchVisitor):
     """
     Find and fix deprecated `pretrained` parameters in TorchVision models.
 
     Both `pretrained` and `pretrained_backbone` parameters are supported.
@@ -244,20 +244,13 @@
                 replacement_args[pos] = new_pretrained_backbone_arg
                 has_replacement = True
 
             replacement = (
                 node.with_changes(args=replacement_args) if has_replacement else None
             )
             if message is not None:
-                position_metadata = self.get_metadata(
-                    cst.metadata.WhitespaceInclusivePositionProvider, node
-                )
-                self.violations.append(
-                    LintViolation(
-                        error_code=self.ERROR_CODE,
-                        message=message,
-                        line=position_metadata.start.line,
-                        column=position_metadata.start.column,
-                        node=node,
-                        replacement=replacement,
-                    )
+                self.add_violation(
+                    node,
+                    error_code=self.ERROR_CODE,
+                    message=message,
+                    replacement=replacement,
                 )
```

