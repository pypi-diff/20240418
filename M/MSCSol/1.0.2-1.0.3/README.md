# Comparing `tmp/MSCSol-1.0.2.tar.gz` & `tmp/MSCSol-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MSCSol-1.0.2.tar", last modified: Thu Apr 18 08:46:46 2024, max compression
+gzip compressed data, last modified: Thu Apr 18 09:41:47 2024, from Unix, original size modulo 2^32 301404160 gzip compressed data, reserved method, ASCII, has comment, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `MSCSol-1.0.2.tar` & `MSCSol-1.0.3.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.225268 MSCSol-1.0.2/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       75 2024-04-18 08:45:47.000000 MSCSol-1.0.2/MANIFEST.in
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.211268 MSCSol-1.0.2/MSCSol/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     7731 2024-04-18 08:15:11.000000 MSCSol-1.0.2/MSCSol/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17465 2024-04-18 08:04:32.000000 MSCSol-1.0.2/MSCSol/data_process.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.214268 MSCSol-1.0.2/MSCSol/gvp/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    20501 2024-04-16 18:02:36.000000 MSCSol-1.0.2/MSCSol/gvp/MSCSolmodel.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.214268 MSCSol-1.0.2/MSCSol/gvp/SKANet/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3348 2024-04-16 16:18:09.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/SKAnet.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      215 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/__init__.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.215268 MSCSol-1.0.2/MSCSol/gvp/SKANet/config/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       24 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/config/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       91 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/config/constants.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    11726 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/features.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2883 2024-04-16 16:19:10.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/helpers.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.224268 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1823 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3306 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2529 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations_jit.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5339 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations_me.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3903 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2293 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/anti_aliasing.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2180 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/blur_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3337 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/cbam.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1616 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/classifier.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5129 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/cond_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3069 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/config.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1490 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/conv2d_same.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1466 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/conv_bn_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3599 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1222 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_attn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1399 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3327 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_norm_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6938 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/drop.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4701 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/eca.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3328 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/evo_norm.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      492 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/helpers.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3353 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/inplace_abn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2092 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/kerv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1737 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/median_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1844 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/mixed_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3774 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/mlp.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3444 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/norm_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2167 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/padding.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1408 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/patch_embed.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2969 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/pool2d_same.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1406 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/se.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    10500 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/selective_kernel.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2641 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/separable_conv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2768 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/shiftlution.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1750 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/space_to_depth.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3013 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/split_attn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3441 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/split_batchnorm.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6517 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/std_conv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4044 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/tbconv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3324 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/weight_init.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1447 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/registry.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     8051 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/SKANet/resnet.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17228 2024-04-15 17:45:43.000000 MSCSol-1.0.2/MSCSol/gvp/__init__.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 08:46:46.214268 MSCSol-1.0.2/MSCSol.egg-info/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1997 2024-04-18 08:46:46.000000 MSCSol-1.0.2/MSCSol.egg-info/PKG-INFO
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2052 2024-04-18 08:46:46.000000 MSCSol-1.0.2/MSCSol.egg-info/SOURCES.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        1 2024-04-18 08:46:46.000000 MSCSol-1.0.2/MSCSol.egg-info/dependency_links.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        7 2024-04-18 08:46:46.000000 MSCSol-1.0.2/MSCSol.egg-info/top_level.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1997 2024-04-18 08:46:46.224268 MSCSol-1.0.2/PKG-INFO
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1739 2024-04-18 08:46:33.000000 MSCSol-1.0.2/README.md
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       38 2024-04-18 08:46:46.225268 MSCSol-1.0.2/setup.cfg
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1098 2024-04-18 08:45:57.000000 MSCSol-1.0.2/setup.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:07:04.000000 ./MSCSol-1.0.3/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       38 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/setup.cfg
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol.egg-info/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        1 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol.egg-info/dependency_links.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2052 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol.egg-info/SOURCES.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2029 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol.egg-info/PKG-INFO
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        7 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol.egg-info/top_level.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       54 2024-04-18 08:54:26.000000 ./MSCSol-1.0.3/MANIFEST.in
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2029 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/PKG-INFO
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1139 2024-04-18 08:59:44.000000 ./MSCSol-1.0.3/setup.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1771 2024-04-18 09:01:10.000000 ./MSCSol-1.0.3/README.md
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:41:37.000000 ./MSCSol-1.0.3/MSCSol/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     7719 2024-04-18 09:39:43.000000 ./MSCSol-1.0.3/MSCSol/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17465 2024-04-18 08:04:32.000000 ./MSCSol-1.0.3/MSCSol/data_process.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004) 301127019 2024-04-18 09:06:44.000000 ./MSCSol-1.0.3/MSCSol/fingerprint.csv
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol/gvp/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17228 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/__init__.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3348 2024-04-16 16:18:10.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/SKAnet.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      215 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1447 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/registry.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2883 2024-04-16 16:19:10.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/helpers.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    11726 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/features.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     8051 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/resnet.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    10500 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/selective_kernel.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1823 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2529 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations_jit.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5129 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/cond_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1737 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/median_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3069 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/config.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4701 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/eca.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3599 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3353 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/inplace_abn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2768 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/shiftlution.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3327 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_norm_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1466 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/conv_bn_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3444 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/norm_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2969 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/pool2d_same.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1399 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2092 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/kerv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3013 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/split_attn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3903 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1222 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_attn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1750 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/space_to_depth.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2641 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/separable_conv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1844 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/mixed_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3774 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/mlp.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6938 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/drop.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2293 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/anti_aliasing.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      492 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/helpers.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1408 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/patch_embed.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3337 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/cbam.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1490 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/conv2d_same.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3324 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/weight_init.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1406 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/se.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3441 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/split_batchnorm.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2180 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/blur_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5339 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations_me.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3306 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4044 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/tbconv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3328 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/evo_norm.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6517 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/std_conv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1616 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/classifier.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2167 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/padding.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 09:01:36.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/config/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       24 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/config/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       91 2024-04-15 17:45:44.000000 ./MSCSol-1.0.3/MSCSol/gvp/SKANet/config/constants.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    20501 2024-04-16 18:02:36.000000 ./MSCSol-1.0.3/MSCSol/gvp/MSCSolmodel.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `MSCSol-1.0.2/MSCSol/__init__.py` & `./MSCSol-1.0.3/MSCSol/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     device = torch.device("cpu")
     test_smile = smiles
     drug = get_properties(test_smile)
     gg = GraphDataset()
     drug2 = gg._featurize_as_graph(drug)
 
     model = MSCSol.gvp.MSCSolmodel.Model((7, 2), (100, 16), (32, 1), (32, 1)).to(device)
-    model.load_state_dict(torch.load(current_path+'/trained.pt'))
+    model.load_state_dict(torch.load('./trained.pt'))
     model.eval()
     h_V = (drug2["node_s"], drug2["node_v"])
     h_E = (drug2["edge_s"], drug2["edge_v"])
     predictions = model(h_V, drug2["edge_index"], h_E, seq=drug2["seq"], batch33 = drug2["batch"],feature_molecule=drug2["feature_molecule"],picdata = drug2["picdata"])
     print("The predicted LogS is "+str(round(float(predictions[0][0]), 2)))
     import os
     os.unlink("./img_MSCSol.png")
```

### Comparing `MSCSol-1.0.2/MSCSol/data_process.py` & `./MSCSol-1.0.3/MSCSol/data_process.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/MSCSolmodel.py` & `./MSCSol-1.0.3/MSCSol/gvp/MSCSolmodel.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/SKAnet.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/SKAnet.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/features.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/features.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/helpers.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/helpers.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/__init__.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations_jit.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations_jit.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/activations_me.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/activations_me.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/anti_aliasing.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/anti_aliasing.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/blur_pool.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/blur_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/cbam.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/classifier.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/cond_conv2d.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/cond_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/config.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/config.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/conv2d_same.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/conv2d_same.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/conv_bn_act.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/conv_bn_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_act.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_attn.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_attn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_conv2d.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/create_norm_act.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/create_norm_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/drop.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/drop.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/eca.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/eca.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/evo_norm.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/evo_norm.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/inplace_abn.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/kerv2d.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/kerv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/median_pool.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/median_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/mixed_conv2d.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/mixed_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/mlp.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/norm_act.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/norm_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/padding.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/padding.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/patch_embed.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/pool2d_same.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/pool2d_same.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/se.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/se.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/selective_kernel.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/separable_conv.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/separable_conv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/shiftlution.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/shiftlution.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/space_to_depth.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/space_to_depth.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/split_attn.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/split_attn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/split_batchnorm.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/split_batchnorm.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/std_conv.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/std_conv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/tbconv.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/tbconv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/layers/weight_init.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/registry.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/registry.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/SKANet/resnet.py` & `./MSCSol-1.0.3/MSCSol/gvp/SKANet/resnet.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol/gvp/__init__.py` & `./MSCSol-1.0.3/MSCSol/gvp/__init__.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/MSCSol.egg-info/PKG-INFO` & `./MSCSol-1.0.3/MSCSol.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSCSol
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for predicting the solubility of small molecule drugs.
 Home-page: https://github.com/ZiyuFanCSU/MSCSol
 Author: Ziyu Fan
 Author-email: fzy_csu@qq.com
 Description-Content-Type: text/markdown
 
 
@@ -43,15 +43,17 @@
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
 In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
 
 ## Update log
 
-`1.0.2` Modifying files don't exist.
+`1.0.3` Modifying files don't exist.
+
+`1.0.1` Modifying path issues.
 
 `1.0.1` Modifying path issues.
 
 `1.0.0` First release.
 
 ## Contact
```

### Comparing `MSCSol-1.0.2/MSCSol.egg-info/SOURCES.txt` & `./MSCSol-1.0.3/MSCSol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.2/PKG-INFO` & `./MSCSol-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSCSol
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for predicting the solubility of small molecule drugs.
 Home-page: https://github.com/ZiyuFanCSU/MSCSol
 Author: Ziyu Fan
 Author-email: fzy_csu@qq.com
 Description-Content-Type: text/markdown
 
 
@@ -43,15 +43,17 @@
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
 In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
 
 ## Update log
 
-`1.0.2` Modifying files don't exist.
+`1.0.3` Modifying files don't exist.
+
+`1.0.1` Modifying path issues.
 
 `1.0.1` Modifying path issues.
 
 `1.0.0` First release.
 
 ## Contact
```

### Comparing `MSCSol-1.0.2/README.md` & `./MSCSol-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
 In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
 
 ## Update log
 
-`1.0.2` Modifying files don't exist.
+`1.0.3` Modifying files don't exist.
+
+`1.0.1` Modifying path issues.
 
 `1.0.1` Modifying path issues.
 
 `1.0.0` First release.
 
 ## Contact
```

### Comparing `MSCSol-1.0.2/setup.py` & `./MSCSol-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 # these things are needed for the README.md show on pypi
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'A tool for predicting the solubility of small molecule drugs.'
 LONG_DESCRIPTION = 'There is a specialized tool available for predicting the solubility of small molecule drugs. By analyzing molecular structures and computing various features, it provides accurate predictions crucial for drug discovery. It helps researchers efficiently select and optimize drug candidates. For more information, please refer to our paper.'
 
 # Setting up
 setup(
     name="MSCSol",
     version=VERSION,
     author="Ziyu Fan",
+    package_data={'mypkg': ['data/*'],},
     author_email="fzy_csu@qq.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/ZiyuFanCSU/MSCSol",
     packages=find_packages(),
     include_package_data=True,
```

