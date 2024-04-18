# Comparing `tmp/MSCSol-1.0.0.tar.gz` & `tmp/MSCSol-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MSCSol-1.0.0.tar", last modified: Tue Apr 16 18:21:58 2024, max compression
+gzip compressed data, was "MSCSol-1.0.5.tar", last modified: Thu Apr 18 10:17:19 2024, max compression
```

## Comparing `MSCSol-1.0.0.tar` & `MSCSol-1.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.493170 MSCSol-1.0.0/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       64 2024-04-16 16:49:19.000000 MSCSol-1.0.0/MANIFEST.in
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.488170 MSCSol-1.0.0/MSCSol/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     7408 2024-04-16 18:13:17.000000 MSCSol-1.0.0/MSCSol/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17310 2024-04-16 18:05:22.000000 MSCSol-1.0.0/MSCSol/data_process.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.488170 MSCSol-1.0.0/MSCSol/gvp/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    20501 2024-04-16 18:02:36.000000 MSCSol-1.0.0/MSCSol/gvp/MSCSolmodel.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.489170 MSCSol-1.0.0/MSCSol/gvp/SKANet/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3348 2024-04-16 16:18:09.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/SKAnet.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      215 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/__init__.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.489170 MSCSol-1.0.0/MSCSol/gvp/SKANet/config/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       24 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/config/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       91 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/config/constants.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    11726 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/features.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2883 2024-04-16 16:19:10.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/helpers.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.493170 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1823 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/__init__.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3306 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2529 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations_jit.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5339 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations_me.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3903 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2293 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/anti_aliasing.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2180 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/blur_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3337 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/cbam.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1616 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/classifier.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5129 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/cond_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3069 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/config.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1490 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/conv2d_same.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1466 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/conv_bn_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3599 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1222 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_attn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1399 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3327 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_norm_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6938 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/drop.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4701 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/eca.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3328 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/evo_norm.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      492 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/helpers.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3353 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/inplace_abn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2092 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/kerv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1737 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/median_pool.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1844 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/mixed_conv2d.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3774 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/mlp.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3444 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/norm_act.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2167 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/padding.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1408 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/patch_embed.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2969 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/pool2d_same.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1406 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/se.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    10500 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/selective_kernel.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2641 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/separable_conv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2768 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/shiftlution.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1750 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/space_to_depth.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3013 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/split_attn.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3441 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/split_batchnorm.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6517 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/std_conv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4044 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/tbconv.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3324 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/weight_init.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1447 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/registry.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     8051 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/SKANet/resnet.py
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17228 2024-04-15 17:45:43.000000 MSCSol-1.0.0/MSCSol/gvp/__init__.py
-drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-16 18:21:58.488170 MSCSol-1.0.0/MSCSol.egg-info/
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1586 2024-04-16 18:21:58.000000 MSCSol-1.0.0/MSCSol.egg-info/PKG-INFO
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2052 2024-04-16 18:21:58.000000 MSCSol-1.0.0/MSCSol.egg-info/SOURCES.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        1 2024-04-16 18:21:58.000000 MSCSol-1.0.0/MSCSol.egg-info/dependency_links.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        7 2024-04-16 18:21:58.000000 MSCSol-1.0.0/MSCSol.egg-info/top_level.txt
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1586 2024-04-16 18:21:58.493170 MSCSol-1.0.0/PKG-INFO
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1328 2024-04-16 17:44:07.000000 MSCSol-1.0.0/README.md
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       38 2024-04-16 18:21:58.494170 MSCSol-1.0.0/setup.cfg
--rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1098 2024-04-16 17:57:39.000000 MSCSol-1.0.0/setup.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.286704 MSCSol-1.0.5/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       54 2024-04-18 08:54:26.000000 MSCSol-1.0.5/MANIFEST.in
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.249704 MSCSol-1.0.5/MSCSol/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     7719 2024-04-18 10:09:45.000000 MSCSol-1.0.5/MSCSol/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17453 2024-04-18 10:10:24.000000 MSCSol-1.0.5/MSCSol/data_process.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.250704 MSCSol-1.0.5/MSCSol/gvp/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    20501 2024-04-16 18:02:36.000000 MSCSol-1.0.5/MSCSol/gvp/MSCSolmodel.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.252704 MSCSol-1.0.5/MSCSol/gvp/SKANet/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3348 2024-04-16 16:18:09.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/SKAnet.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      215 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/__init__.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.254704 MSCSol-1.0.5/MSCSol/gvp/SKANet/config/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       24 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/config/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       91 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/config/constants.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    11726 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/features.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2883 2024-04-16 16:19:10.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/helpers.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.285704 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1823 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/__init__.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3306 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2529 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations_jit.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5339 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations_me.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3903 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2293 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/anti_aliasing.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2180 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/blur_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3337 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/cbam.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1616 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/classifier.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     5129 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/cond_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3069 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/config.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1490 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/conv2d_same.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1466 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/conv_bn_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3599 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1222 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_attn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1399 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3327 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_norm_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6938 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/drop.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4701 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/eca.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3328 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/evo_norm.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)      492 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/helpers.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3353 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/inplace_abn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2092 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/kerv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1737 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/median_pool.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1844 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/mixed_conv2d.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3774 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/mlp.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3444 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/norm_act.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2167 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/padding.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1408 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/patch_embed.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2969 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/pool2d_same.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1406 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/se.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    10500 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/selective_kernel.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2641 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/separable_conv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2768 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/shiftlution.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1750 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/space_to_depth.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3013 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/split_attn.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3441 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/split_batchnorm.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     6517 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/std_conv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     4044 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/tbconv.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     3324 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/weight_init.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1447 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/registry.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     8051 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/SKANet/resnet.py
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)    17228 2024-04-15 17:45:43.000000 MSCSol-1.0.5/MSCSol/gvp/__init__.py
+drwxrwxr-x   0 fanziyu   (1004) fanziyu   (1004)        0 2024-04-18 10:17:19.250704 MSCSol-1.0.5/MSCSol.egg-info/
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2140 2024-04-18 10:17:19.000000 MSCSol-1.0.5/MSCSol.egg-info/PKG-INFO
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2052 2024-04-18 10:17:19.000000 MSCSol-1.0.5/MSCSol.egg-info/SOURCES.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        1 2024-04-18 10:17:19.000000 MSCSol-1.0.5/MSCSol.egg-info/dependency_links.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)        7 2024-04-18 10:17:19.000000 MSCSol-1.0.5/MSCSol.egg-info/top_level.txt
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     2140 2024-04-18 10:17:19.285704 MSCSol-1.0.5/PKG-INFO
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1882 2024-04-18 10:17:09.000000 MSCSol-1.0.5/README.md
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)       38 2024-04-18 10:17:19.286704 MSCSol-1.0.5/setup.cfg
+-rw-rw-r--   0 fanziyu   (1004) fanziyu   (1004)     1098 2024-04-18 10:16:55.000000 MSCSol-1.0.5/setup.py
```

### Comparing `MSCSol-1.0.0/MSCSol/__init__.py` & `MSCSol-1.0.5/MSCSol/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import torch_geometric
 import torch_cluster
 from PIL import Image
 import random
 import numpy as np
 import torchvision.transforms as transforms
 from MSCSol.data_process import get_properties
+import os
+current_path = os.path.dirname(os.path.abspath(__file__))
 
 
 def _normalize(tensor, dim=-1):
     return torch.nan_to_num(
         torch.div(tensor, torch.norm(tensor, dim=dim, keepdim=True)))
 
 def _rbf(D, D_min=0., D_max=20., D_count=16, device='cpu'):
@@ -54,15 +56,15 @@
         img = Image.open(filename).convert('RGB')
         if self.type == 'train':
             return self._image_transformer_train(img)
         else:
             return self._image_transformer_test(img)
 
     def _featurize_as_graph(self, drug):
-        picdata = self.get_image("./0.png")
+        picdata = self.get_image("./img_MSCSol.png")
         if self.normalize is not None:
             picdata = self.normalize(picdata)
         feature_molecule = drug['features']
         with torch.no_grad():
             coords = torch.as_tensor(drug["xyz_1"],
                                      device=self.device, dtype=torch.float32)
             seq = torch.as_tensor([self.letter_to_num[a] for a in drug['atom_seq']],
@@ -165,20 +167,26 @@
         c, n = _normalize(c - origin), _normalize(n - origin)
         bisector = _normalize(c + n)
         perp = _normalize(torch.cross(c, n))
         vec = -bisector * math.sqrt(1 / 3) - perp * math.sqrt(2 / 3)
         return vec
 
 def pred(smiles):
+    print("This process will take a few minutes, please wait for a moment.")
     device = torch.device("cpu")
     test_smile = smiles
     drug = get_properties(test_smile)
     gg = GraphDataset()
     drug2 = gg._featurize_as_graph(drug)
 
     model = MSCSol.gvp.MSCSolmodel.Model((7, 2), (100, 16), (32, 1), (32, 1)).to(device)
-    model.load_state_dict(torch.load('./MSCSol/trained.pt'))
+    model.load_state_dict(torch.load('./trained.pt'))
     model.eval()
     h_V = (drug2["node_s"], drug2["node_v"])
     h_E = (drug2["edge_s"], drug2["edge_v"])
     predictions = model(h_V, drug2["edge_index"], h_E, seq=drug2["seq"], batch33 = drug2["batch"],feature_molecule=drug2["feature_molecule"],picdata = drug2["picdata"])
     print("The predicted LogS is "+str(round(float(predictions[0][0]), 2)))
+    import os
+    os.unlink("./img_MSCSol.png")
+    os.unlink("./shadow_MSCSol_1.png")
+    os.unlink("./shadow_MSCSol_2.png")
+    os.unlink("./shadow_MSCSol_3.png")
```

### Comparing `MSCSol-1.0.0/MSCSol/data_process.py` & `MSCSol-1.0.5/MSCSol/data_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 from mpl_toolkits.mplot3d import Axes3D
 import cv2 as cv
 import os
 import pandas as pd
+import os
+current_path = os.path.dirname(os.path.abspath(__file__))
+
 #number of points per atom
 number_points=1000
 #vdw radii
 radiiDict={'H': 1.2, 'He': 1.4, 'Li': 2.2, 'Be': 1.9, 'B': 2, 'C': 1.7, 'N': 1.55, 'O': 1.52, 'F': 1.47, 'Ne': 1.5,
   'Na': 2.4, 'Mg': 2.2, 'Al': 2.1, 'Si': 2.1, 'P': 1.8, 'S': 1.8, 'Cl': 1.75, 'Ar': 1.9, 'K': 2.8, 'Ca': 2.4,
     'Se': 1.9, 'Ti': 2.15, 'V': 2.05, 'Cr': 2.05, 'Mn': 2.05, 'Fe': 2.05, 'Co': 2.0, 'Ni': 2.0, 'Cu': 2.0, 'Zn': 2.1,
       'Ga': 2.1, 'Ge': 2.1, 'As': 2.05, 'Br': 1.85, 'Kr': 2.0, 'Rb': 2.9, 'Sr': 2.55, 'Y': 2.4, 'Zr': 2.3, 'Nb': 2.15,
@@ -407,27 +410,27 @@
     coords_list = data['atom_pos']
     df['atom_seq'] = atom_list
     df['xyz_1'] = coords_list
 
 
     x,y,z = get_points(coords_list,atom_list)
     graph(x,y,z,0,0)
-    plt.savefig("./i_1.png") #first angle
+    plt.savefig("./shadow_MSCSol_1.png") #first angle
     plt.close()
     graph(x,y,z,90,0)
-    plt.savefig("./i_2.png") #perpendicular
+    plt.savefig("./shadow_MSCSol_2.png") #perpendicular
     plt.close()
     graph(x,y,z,90,90)
-    plt.savefig("./i_3.png") #perpendicular again
+    plt.savefig("./shadow_MSCSol_3.png") #perpendicular again
     plt.close()
 
     #get for every molecule
-    results1=shadow_info("./i_1.png")
-    results2=shadow_info("./i_2.png")
-    results3=shadow_info("./i_3.png")
+    results1=shadow_info("./shadow_MSCSol_1.png")
+    results2=shadow_info("./shadow_MSCSol_2.png")
+    results3=shadow_info("./shadow_MSCSol_3.png")
     areas=sorted([results1[0],results2[0],results3[0]]) #get ascending areas
     asp_ratios=sorted([results1[1],results2[1],results3[1]]) #get ascending aspect ratios
 
     df["Area1"]=areas[0]
     df["Area2"]=areas[1]
     df["Area3"]=areas[2]
     df["Asp1"]=asp_ratios[0]
@@ -440,15 +443,15 @@
     columns_to_standardize = ['MW','logP','TPSA','hba','hbd','rob','aliRings','aroRings','sp3','LASA','chiral_center','qed',"Area1","Area2","Area3","Asp1","Asp2","Asp3"]
     ff = []
     num = 0
     for k in columns_to_standardize:
         ff.append(((df[k] - mean[num]) / std[num]))
         num += 1
 
-    df2 = pd.read_csv("./MSCSol/fingerprint.csv", quotechar='"')
+    df2 = pd.read_csv("./fingerprint.csv", quotechar='"')
     pca = PCA(n_components=101)
     concatenated_MACCS = pd.concat([df2['MACCS'],pd.DataFrame([str(df['MACCS'])])])
     MACCS_pca = pca.fit_transform([eval(i[0]) for i in np.array(concatenated_MACCS)])
     pca = PCA(n_components=300)
     concatenated_ECFP1 = pd.concat([df2['ECFP1'],pd.DataFrame([str(df['ECFP1'])])])
     ECFP6_1_pca = pca.fit_transform([eval(i[0]) for i in np.array(concatenated_ECFP1)])
     pca = PCA(n_components=300)
@@ -457,11 +460,11 @@
     pca = PCA(n_components=300)
     concatenated_ECFP3 = pd.concat([df2['ECFP2'],pd.DataFrame([str(df['ECFP3'])])])
     ECFP6_3_pca = pca.fit_transform([eval(i[0]) for i in np.array(concatenated_ECFP3)])
 
     df['features'] = [ff+ MACCS_pca[-1].tolist()+ECFP6_1_pca[-1].tolist()+ECFP6_2_pca[-1].tolist()+ECFP6_3_pca[-1].tolist()]
 
     mol = Chem.MolFromSmiles(test_smiles)
-    Draw.MolToFile(mol,f'./0.png',size=(224, 224))
+    Draw.MolToFile(mol,f'./img_MSCSol.png',size=(224, 224))
 
     return df
```

### Comparing `MSCSol-1.0.0/MSCSol/gvp/MSCSolmodel.py` & `MSCSol-1.0.5/MSCSol/gvp/MSCSolmodel.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/SKAnet.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/SKAnet.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/features.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/features.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/helpers.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/helpers.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/__init__.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations_jit.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations_jit.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/activations_me.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/activations_me.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/adaptive_avgmax_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/anti_aliasing.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/anti_aliasing.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/blur_pool.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/blur_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/cbam.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/cbam.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/classifier.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/cond_conv2d.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/cond_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/config.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/config.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/conv2d_same.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/conv2d_same.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/conv_bn_act.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/conv_bn_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_act.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_attn.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_attn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_conv2d.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/create_norm_act.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/create_norm_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/drop.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/drop.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/eca.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/eca.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/evo_norm.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/evo_norm.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/inplace_abn.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/inplace_abn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/kerv2d.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/kerv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/median_pool.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/median_pool.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/mixed_conv2d.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/mixed_conv2d.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/mlp.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/norm_act.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/norm_act.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/padding.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/padding.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/patch_embed.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/pool2d_same.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/pool2d_same.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/se.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/se.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/selective_kernel.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/selective_kernel.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/separable_conv.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/separable_conv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/shiftlution.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/shiftlution.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/space_to_depth.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/space_to_depth.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/split_attn.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/split_attn.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/split_batchnorm.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/split_batchnorm.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/std_conv.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/std_conv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/tbconv.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/tbconv.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/layers/weight_init.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/registry.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/registry.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/SKANet/resnet.py` & `MSCSol-1.0.5/MSCSol/gvp/SKANet/resnet.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol/gvp/__init__.py` & `MSCSol-1.0.5/MSCSol/gvp/__init__.py`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/MSCSol.egg-info/PKG-INFO` & `MSCSol-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-Metadata-Version: 2.1
-Name: MSCSol
-Version: 1.0.0
-Summary: A tool for predicting the solubility of small molecule drugs.
-Home-page: https://github.com/ZiyuFanCSU/MSCSol
-Author: Ziyu Fan
-Author-email: fzy_csu@qq.com
-Description-Content-Type: text/markdown
-
-
 ## Using MSCSol to predict moleculer solubility
 
 ### MSCSol
 
 [![Downloads](https://static.pepy.tech/badge/MSCSol)](https://pepy.tech/project/MSCSol)
 
 Our trained model has been uploaded to PyPI, accessible through this link (https://pypi.org/project/MSCSol/). We've included detailed installation instructions and usage guidelines, making it easy to obtain prediction results by inputting SMILES strings.
 
 
 ### Installation
 
 ```
-pip install MSCSol
+pip install MSCSol==1.0.5
 ```
 
+### Package needed
+
+see https://github.com/ZiyuFanCSU/MSCSol and you need to download the required data files for the program and place them in the directory where you are running MSCSol, including trained.pt and fingerprint.csv.
+
 ### Quick Start
 
 ```
 import MSCSol
 
 MSCSol.pred(<your_SMILES>)
 ```
@@ -35,12 +29,20 @@
 
 It will take some time to calculate the molecular signatures, so please be patient for a while. Also note that dipole moment features are not used here as they cannot be obtained directly by calling the code. 
 
 The training data was restricted to molecular weights less than or equal to 504, LogS values greater than or equal to -8, and experimental temperatures of 20-25 degrees Celsius, so if the molecule does not apply to the above conditions, the prediction results may have a large deviation. 
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
+In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
+
+## Update log
+
+`1.0.1--1.0.5` Modifying some bugs.
+
+`1.0.0` First release.
+
 ## Contact
 
 We thank all the researchers who contributed to this work.
 
-If you have any questions, please contact fzychina@csu.edu.cn.
+If you have any questions, please contact fzychina@csu.edu.cn.
```

### Comparing `MSCSol-1.0.0/MSCSol.egg-info/SOURCES.txt` & `MSCSol-1.0.5/MSCSol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MSCSol-1.0.0/PKG-INFO` & `MSCSol-1.0.5/MSCSol.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSCSol
-Version: 1.0.0
+Version: 1.0.5
 Summary: A tool for predicting the solubility of small molecule drugs.
 Home-page: https://github.com/ZiyuFanCSU/MSCSol
 Author: Ziyu Fan
 Author-email: fzy_csu@qq.com
 Description-Content-Type: text/markdown
 
 
@@ -16,17 +16,21 @@
 
 Our trained model has been uploaded to PyPI, accessible through this link (https://pypi.org/project/MSCSol/). We've included detailed installation instructions and usage guidelines, making it easy to obtain prediction results by inputting SMILES strings.
 
 
 ### Installation
 
 ```
-pip install MSCSol
+pip install MSCSol==1.0.5
 ```
 
+### Package needed
+
+see https://github.com/ZiyuFanCSU/MSCSol and you need to download the required data files for the program and place them in the directory where you are running MSCSol, including trained.pt and fingerprint.csv.
+
 ### Quick Start
 
 ```
 import MSCSol
 
 MSCSol.pred(<your_SMILES>)
 ```
@@ -35,12 +39,20 @@
 
 It will take some time to calculate the molecular signatures, so please be patient for a while. Also note that dipole moment features are not used here as they cannot be obtained directly by calling the code. 
 
 The training data was restricted to molecular weights less than or equal to 504, LogS values greater than or equal to -8, and experimental temperatures of 20-25 degrees Celsius, so if the molecule does not apply to the above conditions, the prediction results may have a large deviation. 
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
+In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
+
+## Update log
+
+`1.0.1--1.0.5` Modifying some bugs.
+
+`1.0.0` First release.
+
 ## Contact
 
 We thank all the researchers who contributed to this work.
 
 If you have any questions, please contact fzychina@csu.edu.cn.
```

### Comparing `MSCSol-1.0.0/README.md` & `MSCSol-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,36 @@
+Metadata-Version: 2.1
+Name: MSCSol
+Version: 1.0.5
+Summary: A tool for predicting the solubility of small molecule drugs.
+Home-page: https://github.com/ZiyuFanCSU/MSCSol
+Author: Ziyu Fan
+Author-email: fzy_csu@qq.com
+Description-Content-Type: text/markdown
+
+
 ## Using MSCSol to predict moleculer solubility
 
 ### MSCSol
 
 [![Downloads](https://static.pepy.tech/badge/MSCSol)](https://pepy.tech/project/MSCSol)
 
 Our trained model has been uploaded to PyPI, accessible through this link (https://pypi.org/project/MSCSol/). We've included detailed installation instructions and usage guidelines, making it easy to obtain prediction results by inputting SMILES strings.
 
 
 ### Installation
 
 ```
-pip install MSCSol
+pip install MSCSol==1.0.5
 ```
 
+### Package needed
+
+see https://github.com/ZiyuFanCSU/MSCSol and you need to download the required data files for the program and place them in the directory where you are running MSCSol, including trained.pt and fingerprint.csv.
+
 ### Quick Start
 
 ```
 import MSCSol
 
 MSCSol.pred(<your_SMILES>)
 ```
@@ -25,12 +39,20 @@
 
 It will take some time to calculate the molecular signatures, so please be patient for a while. Also note that dipole moment features are not used here as they cannot be obtained directly by calling the code. 
 
 The training data was restricted to molecular weights less than or equal to 504, LogS values greater than or equal to -8, and experimental temperatures of 20-25 degrees Celsius, so if the molecule does not apply to the above conditions, the prediction results may have a large deviation. 
 
 In addition, due to the computational requirements of the node vector feature of the GVP-GNN, the input molecule atom number must be greater than or equal to 3.
 
+In addition, four temporary files will be generated at runtime, named img_MSCSol.png, shadow_MSCSol_1.png, shadow_MSCSol_2.png and shadow_MSCSol_3.png. Please make sure not to have the same file name as yours to avoid accidental deletion.
+
+## Update log
+
+`1.0.1--1.0.5` Modifying some bugs.
+
+`1.0.0` First release.
+
 ## Contact
 
 We thank all the researchers who contributed to this work.
 
-If you have any questions, please contact fzychina@csu.edu.cn.
+If you have any questions, please contact fzychina@csu.edu.cn.
```

### Comparing `MSCSol-1.0.0/setup.py` & `MSCSol-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.5'
 DESCRIPTION = 'A tool for predicting the solubility of small molecule drugs.'
 LONG_DESCRIPTION = 'There is a specialized tool available for predicting the solubility of small molecule drugs. By analyzing molecular structures and computing various features, it provides accurate predictions crucial for drug discovery. It helps researchers efficiently select and optimize drug candidates. For more information, please refer to our paper.'
 
 # Setting up
 setup(
     name="MSCSol",
     version=VERSION,
```

