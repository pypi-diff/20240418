# Comparing `tmp/vit_pytorch-1.6.6.tar.gz` & `tmp/vit_pytorch-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit_pytorch-1.6.6.tar", last modified: Wed Apr 17 16:40:45 2024, max compression
+gzip compressed data, was "vit_pytorch-1.6.7.tar", last modified: Thu Apr 18 16:45:11 2024, max compression
```

## Comparing `vit_pytorch-1.6.6.tar` & `vit_pytorch-1.6.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    65041 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.801581 vit_pytorch-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.809581 vit_pytorch-1.6.6/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/max_vit_with_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/na_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_qk_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_register_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vivit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/xcit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:11.148004 vit_pytorch-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-18 16:45:11.144004 vit_pytorch-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    65041 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:45:11.148004 vit_pytorch-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:11.136004 vit_pytorch-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:11.144004 vit_pytorch-1.6.7/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/max_vit_with_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/na_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_qk_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_register_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/vivit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-18 16:45:06.000000 vit_pytorch-1.6.7/vit_pytorch/xcit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:11.144004 vit_pytorch-1.6.7/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-18 16:45:11.000000 vit_pytorch-1.6.7/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-18 16:45:11.000000 vit_pytorch-1.6.7/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:45:11.000000 vit_pytorch-1.6.7/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:45:11.000000 vit_pytorch-1.6.7/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 16:45:11.000000 vit_pytorch-1.6.7/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit_pytorch-1.6.6/LICENSE` & `vit_pytorch-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/PKG-INFO` & `vit_pytorch-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.6.6
+Version: 1.6.7
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vit-pytorch Version: 1.6.6 Summary: Vision
+Metadata-Version: 2.1 Name: vit-pytorch Version: 1.6.7 Summary: Vision
 Transformer (ViT) - Pytorch Home-page: https://github.com/lucidrains/vit-
 pytorch Author: Phil Wang Author-email: lucidrains@gmail.com License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.6 Description-Content-Type: text/markdown
```

### Comparing `vit_pytorch-1.6.6/README.md` & `vit_pytorch-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/setup.py` & `vit_pytorch-1.6.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.6.6',
+  version = '1.6.7',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
```

### Comparing `vit_pytorch-1.6.6/vit_pytorch/ats_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/cait.py` & `vit_pytorch-1.6.7/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/cct.py` & `vit_pytorch-1.6.7/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/cct_3d.py` & `vit_pytorch-1.6.7/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/cross_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/cross_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/crossformer.py` & `vit_pytorch-1.6.7/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/cvt.py` & `vit_pytorch-1.6.7/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/deepvit.py` & `vit_pytorch-1.6.7/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/dino.py` & `vit_pytorch-1.6.7/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/distill.py` & `vit_pytorch-1.6.7/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/efficient.py` & `vit_pytorch-1.6.7/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/es_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/extractor.py` & `vit_pytorch-1.6.7/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/learnable_memory_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/levit.py` & `vit_pytorch-1.6.7/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/local_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/mae.py` & `vit_pytorch-1.6.7/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/max_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/max_vit_with_registers.py` & `vit_pytorch-1.6.7/vit_pytorch/max_vit_with_registers.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/mobile_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/mp3.py` & `vit_pytorch-1.6.7/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/mpp.py` & `vit_pytorch-1.6.7/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/na_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/na_vit.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
         self.calc_token_dropout = None
 
         if callable(token_dropout_prob):
             self.calc_token_dropout = token_dropout_prob
 
         elif isinstance(token_dropout_prob, (float, int)):
-            assert 0. < token_dropout_prob < 1.
+            assert 0. <= token_dropout_prob < 1.
             token_dropout_prob = float(token_dropout_prob)
             self.calc_token_dropout = lambda height, width: token_dropout_prob
 
         # calculate patching related stuff
 
         assert divisible_by(image_height, patch_size) and divisible_by(image_width, patch_size), 'Image dimensions must be divisible by the patch size.'
 
@@ -245,26 +245,26 @@
 
     def forward(
         self,
         batched_images: Union[List[Tensor], List[List[Tensor]]], # assume different resolution images already grouped correctly
         group_images = False,
         group_max_seq_len = 2048
     ):
-        p, c, device, has_token_dropout = self.patch_size, self.channels, self.device, exists(self.calc_token_dropout)
+        p, c, device, has_token_dropout = self.patch_size, self.channels, self.device, exists(self.calc_token_dropout) and self.training
 
         arange = partial(torch.arange, device = device)
         pad_sequence = partial(orig_pad_sequence, batch_first = True)
 
         # auto pack if specified
 
         if group_images:
             batched_images = group_images_by_max_seq_len(
                 batched_images,
                 patch_size = self.patch_size,
-                calc_token_dropout = self.calc_token_dropout,
+                calc_token_dropout = self.calc_token_dropout if self.training else None,
                 max_seq_len = group_max_seq_len
             )
 
         # process images into variable lengthed sequences with attention mask
 
         num_images = []
         batched_sequences = []
@@ -310,16 +310,16 @@
             batched_image_ids.append(image_ids)
             batched_sequences.append(torch.cat(sequences, dim = 0))
             batched_positions.append(torch.cat(positions, dim = 0))
 
         # derive key padding mask
 
         lengths = torch.tensor([seq.shape[-2] for seq in batched_sequences], device = device, dtype = torch.long)
-        max_length = arange(lengths.amax().item())
-        key_pad_mask = rearrange(lengths, 'b -> b 1') <= rearrange(max_length, 'n -> 1 n')
+        seq_arange = arange(lengths.amax().item())
+        key_pad_mask = rearrange(seq_arange, 'n -> 1 n') < rearrange(lengths, 'b -> b 1')
 
         # derive attention mask, and combine with key padding mask from above
 
         batched_image_ids = pad_sequence(batched_image_ids)
         attn_mask = rearrange(batched_image_ids, 'b i -> b 1 i 1') == rearrange(batched_image_ids, 'b j -> b 1 1 j')
         attn_mask = attn_mask & rearrange(key_pad_mask, 'b j -> b 1 1 j')
```

### Comparing `vit_pytorch-1.6.6/vit_pytorch/nest.py` & `vit_pytorch-1.6.7/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/parallel_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/pit.py` & `vit_pytorch-1.6.7/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/recorder.py` & `vit_pytorch-1.6.7/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/regionvit.py` & `vit_pytorch-1.6.7/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/rvt.py` & `vit_pytorch-1.6.7/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/scalable_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/sep_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simmim.py` & `vit_pytorch-1.6.7/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_flash_attn_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_1d.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_3d.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_fft.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_fft.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_qk_norm.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_qk_norm.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_register_tokens.py` & `vit_pytorch-1.6.7/vit_pytorch/simple_vit_with_register_tokens.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/t2t.py` & `vit_pytorch-1.6.7/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/twins_svt.py` & `vit_pytorch-1.6.7/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit.py` & `vit_pytorch-1.6.7/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit_1d.py` & `vit_pytorch-1.6.7/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit_3d.py` & `vit_pytorch-1.6.7/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit_for_small_dataset.py` & `vit_pytorch-1.6.7/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_dropout.py` & `vit_pytorch-1.6.7/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_merger.py` & `vit_pytorch-1.6.7/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/vivit.py` & `vit_pytorch-1.6.7/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch/xcit.py` & `vit_pytorch-1.6.7/vit_pytorch/xcit.py`

 * *Files identical despite different names*

### Comparing `vit_pytorch-1.6.6/vit_pytorch.egg-info/PKG-INFO` & `vit_pytorch-1.6.7/vit_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch
-Version: 1.6.6
+Version: 1.6.7
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/lucidrains/vit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vit-pytorch Version: 1.6.6 Summary: Vision
+Metadata-Version: 2.1 Name: vit-pytorch Version: 1.6.7 Summary: Vision
 Transformer (ViT) - Pytorch Home-page: https://github.com/lucidrains/vit-
 pytorch Author: Phil Wang Author-email: lucidrains@gmail.com License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3.6 Description-Content-Type: text/markdown
```

### Comparing `vit_pytorch-1.6.6/vit_pytorch.egg-info/SOURCES.txt` & `vit_pytorch-1.6.7/vit_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

