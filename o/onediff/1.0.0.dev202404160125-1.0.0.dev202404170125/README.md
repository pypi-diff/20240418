# Comparing `tmp/onediff-1.0.0.dev202404160125.tar.gz` & `tmp/onediff-1.0.0.dev202404170125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202404160125.tar", last modified: Tue Apr 16 01:25:13 2024, max compression
+gzip compressed data, was "onediff-1.0.0.dev202404170125.tar", last modified: Wed Apr 17 01:25:29 2024, max compression
```

## Comparing `onediff-1.0.0.dev202404160125.tar` & `onediff-1.0.0.dev202404170125.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.104905 onediff-1.0.0.dev202404160125/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.104905 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.108905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.112905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.112905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-16 01:25:13.000000 onediff-1.0.0.dev202404160125/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-16 01:25:13.000000 onediff-1.0.0.dev202404160125/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:25:13.000000 onediff-1.0.0.dev202404160125/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 01:25:13.000000 onediff-1.0.0.dev202404160125/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 01:25:13.000000 onediff-1.0.0.dev202404160125/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:25:13.116905 onediff-1.0.0.dev202404160125/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-16 01:25:05.000000 onediff-1.0.0.dev202404160125/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-17 01:25:21.000000 onediff-1.0.0.dev202404170125/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.426603 onediff-1.0.0.dev202404170125/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.426603 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.430603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.434603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.434603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.434603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/with_fx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/with_fx_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-04-17 01:25:29.000000 onediff-1.0.0.dev202404170125/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 01:25:29.000000 onediff-1.0.0.dev202404170125/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:25:29.000000 onediff-1.0.0.dev202404170125/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 01:25:29.000000 onediff-1.0.0.dev202404170125/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 01:25:29.000000 onediff-1.0.0.dev202404170125/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:29.438603 onediff-1.0.0.dev202404170125/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-17 01:25:22.000000 onediff-1.0.0.dev202404170125/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202404160125/PKG-INFO` & `onediff-1.0.0.dev202404170125/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202404160125
+Version: 1.0.0.dev202404170125
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,20 +25,22 @@
 Requires-Dist: torch
 
 <p align="center">
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
-<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community-green"></a>
-<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Github Stars"></a>
-[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
-<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip Downloads"></a>
+<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
+<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
 <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
+[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
 
+<a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
+<a href="https://github.com/siliconflow/onediff/issues" target="_blank"><img src="https://img.shields.io/github/issues/siliconflow/onediff?label=Issues"></a>
 [![Docker image build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml)
 [![CI testing](https://github.com/siliconflow/onediff/actions/workflows/examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/workflows/examples.yml?query=event%3Aschedule)
 
 
 ## OneDiff
 OneDiff is an out-of-the-box acceleration library for diffusion models, it provides:
 - PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion models
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404160125 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404170125 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 Requires-Dist: transformers>=4.27.1 Requires-Dist: diffusers>=0.19.3 Requires-
 Dist: accelerate Requires-Dist: torch
                             [imgs/onediff_logo.png]
---- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_G_i_t_h_u_b
-_S_t_a_r_s_][![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)]
-(https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/
-_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-
-_D_i_s_c_u_s_s_-_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![Docker image build](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml) [![CI testing](https://
-github.com/siliconflow/onediff/actions/workflows/examples.yml/
-badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/
-workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an out-of-
-the-box acceleration library for diffusion models, it provides: - PyTorch
-Module compilation tools and strong optimized GPU Kernels for diffusion models
-- Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF diffusers
-ð¤](https://github.com/siliconflow/onediff/tree/main/
+--- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
+_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![](https://dcbadge.vercel.app/api/server/
+RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_l_a_b_e_l_=_I_s_s_u_e_s_][![Docker image
+build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/
+badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml) [!
+[CI testing](https://github.com/siliconflow/onediff/actions/workflows/
+examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/
+actions/workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an
+out-of-the-box acceleration library for diffusion models, it provides: -
+PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion
+models - Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF
+diffusers ð¤](https://github.com/siliconflow/onediff/tree/main/
 onediff_diffusers_extensions) - [OneDiff for ComfyUI](https://github.com/
 siliconflow/onediff/tree/main/onediff_comfy_nodes) - [OneDiff for Stable
 Diffusion web UI](https://github.com/siliconflow/onediff/tree/main/
 onediff_sd_webui_extensions) For example: [imgs/replace_a100.png]## News
 OneDiff is the abbreviation of "**one** line of code to accelerate
 **diff**usion models". Here is the latest news: - :rocket:[Accelerating Stable
 Video Diffusion 3x faster with OneDiff DeepCache + Int8](https://
```

### Comparing `onediff-1.0.0.dev202404160125/README.md` & `onediff-1.0.0.dev202404170125/src/onediff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,46 @@
+Metadata-Version: 2.1
+Name: onediff
+Version: 1.0.0.dev202404170125
+Summary: an out-of-the-box acceleration library for diffusion models
+Home-page: https://github.com/siliconflow/onediff
+Author: OneDiff contributors
+Author-email: caishenghang@oneflow.org
+License: Apache
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Requires-Dist: transformers>=4.27.1
+Requires-Dist: diffusers>=0.19.3
+Requires-Dist: accelerate
+Requires-Dist: torch
+
 <p align="center">
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
-<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community-green"></a>
-<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Github Stars"></a>
-[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
-<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip Downloads"></a>
+<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
+<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
 <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
+[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
 
+<a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
+<a href="https://github.com/siliconflow/onediff/issues" target="_blank"><img src="https://img.shields.io/github/issues/siliconflow/onediff?label=Issues"></a>
 [![Docker image build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml)
 [![CI testing](https://github.com/siliconflow/onediff/actions/workflows/examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/workflows/examples.yml?query=event%3Aschedule)
 
 
 ## OneDiff
 OneDiff is an out-of-the-box acceleration library for diffusion models, it provides:
 - PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion models
```

#### html2text {}

```diff
@@ -1,23 +1,39 @@
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404170125 Summary: an
+out-of-the-box acceleration library for diffusion models Home-page: https://
+github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
+caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
+Requires-Dist: transformers>=4.27.1 Requires-Dist: diffusers>=0.19.3 Requires-
+Dist: accelerate Requires-Dist: torch
                             [imgs/onediff_logo.png]
---- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_G_i_t_h_u_b
-_S_t_a_r_s_][![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)]
-(https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/
-_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-
-_D_i_s_c_u_s_s_-_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![Docker image build](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml) [![CI testing](https://
-github.com/siliconflow/onediff/actions/workflows/examples.yml/
-badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/
-workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an out-of-
-the-box acceleration library for diffusion models, it provides: - PyTorch
-Module compilation tools and strong optimized GPU Kernels for diffusion models
-- Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF diffusers
-ð¤](https://github.com/siliconflow/onediff/tree/main/
+--- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
+_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![](https://dcbadge.vercel.app/api/server/
+RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_l_a_b_e_l_=_I_s_s_u_e_s_][![Docker image
+build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/
+badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml) [!
+[CI testing](https://github.com/siliconflow/onediff/actions/workflows/
+examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/
+actions/workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an
+out-of-the-box acceleration library for diffusion models, it provides: -
+PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion
+models - Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF
+diffusers ð¤](https://github.com/siliconflow/onediff/tree/main/
 onediff_diffusers_extensions) - [OneDiff for ComfyUI](https://github.com/
 siliconflow/onediff/tree/main/onediff_comfy_nodes) - [OneDiff for Stable
 Diffusion web UI](https://github.com/siliconflow/onediff/tree/main/
 onediff_sd_webui_extensions) For example: [imgs/replace_a100.png]## News
 OneDiff is the abbreviation of "**one** line of code to accelerate
 **diff**usion models". Here is the latest news: - :rocket:[Accelerating Stable
 Video Diffusion 3x faster with OneDiff DeepCache + Int8](https://
```

### Comparing `onediff-1.0.0.dev202404160125/setup.py` & `onediff-1.0.0.dev202404170125/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.0.0.dev202404170125/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/__init__.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/options.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/with_fx_graph.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/with_fx_graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/infer_compiler/with_fx_interpreter.py` & `onediff-1.0.0.dev202404170125/src/onediff/infer_compiler/with_fx_interpreter.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/optimization/attention_processor.py` & `onediff-1.0.0.dev202404170125/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/optimization/quant_optimizer.py` & `onediff-1.0.0.dev202404170125/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.0.0.dev202404170125/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.0.0.dev202404170125/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff/quantization/quantize_utils.py` & `onediff-1.0.0.dev202404170125/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/src/onediff.egg-info/PKG-INFO` & `onediff-1.0.0.dev202404170125/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,20 @@
-Metadata-Version: 2.1
-Name: onediff
-Version: 1.0.0.dev202404160125
-Summary: an out-of-the-box acceleration library for diffusion models
-Home-page: https://github.com/siliconflow/onediff
-Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Requires-Dist: transformers>=4.27.1
-Requires-Dist: diffusers>=0.19.3
-Requires-Dist: accelerate
-Requires-Dist: torch
-
 <p align="center">
 <img src="imgs/onediff_logo.png" height="100">
 </p>
 
 ---
-<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community-green"></a>
-<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Github Stars"></a>
-[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
-<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip Downloads"></a>
+<a href="https://pypistats.org/packages/onediff" target="_blank"><img src="https://img.shields.io/pypi/dw/onediff?style=square&label=Pip install"></a>
+<a href="https://github.com/siliconflow/onediff/stargazers" target="_blank"><img src="https://img.shields.io/github/stars/siliconflow/onediff?style=square&label=Stars&color=green"></a>
+<a href="https://github.com/siliconflow/onediff/wiki" target="_blank"><img src="https://img.shields.io/badge/OneDiff-Community wiki-green"></a>
 <a href="https://twitter.com/search?q=%22onediff%22&src=typed_query&f=live" target="_blank"><img src="https://img.shields.io/badge/Twitter-Discuss-green?logo=twitter&amp"></a>
+[![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ)
 
+<a href="https://github.com/siliconflow/onediff/milestone/3" target="_blank"><img src="https://img.shields.io/github/milestones/progress/siliconflow/onediff/3"></a>
+<a href="https://github.com/siliconflow/onediff/issues" target="_blank"><img src="https://img.shields.io/github/issues/siliconflow/onediff?label=Issues"></a>
 [![Docker image build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml)
 [![CI testing](https://github.com/siliconflow/onediff/actions/workflows/examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/workflows/examples.yml?query=event%3Aschedule)
 
 
 ## OneDiff
 OneDiff is an out-of-the-box acceleration library for diffusion models, it provides:
 - PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion models
```

#### html2text {}

```diff
@@ -1,37 +1,25 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404160125 Summary: an
-out-of-the-box acceleration library for diffusion models Home-page: https://
-github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
-caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
-Requires-Dist: transformers>=4.27.1 Requires-Dist: diffusers>=0.19.3 Requires-
-Dist: accelerate Requires-Dist: torch
                             [imgs/onediff_logo.png]
---- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_G_i_t_h_u_b
-_S_t_a_r_s_][![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=square)]
-(https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/
-_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _D_o_w_n_l_o_a_d_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-
-_D_i_s_c_u_s_s_-_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![Docker image build](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml/badge.svg)](https://github.com/
-siliconflow/onediff/actions/workflows/sd.yml) [![CI testing](https://
-github.com/siliconflow/onediff/actions/workflows/examples.yml/
-badge.svg?event=schedule)](https://github.com/siliconflow/onediff/actions/
-workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an out-of-
-the-box acceleration library for diffusion models, it provides: - PyTorch
-Module compilation tools and strong optimized GPU Kernels for diffusion models
-- Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF diffusers
-ð¤](https://github.com/siliconflow/onediff/tree/main/
+--- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_w_/_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_P_i_p_ _i_n_s_t_a_l_l_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_s_i_l_i_c_o_n_f_l_o_w_/
+_o_n_e_d_i_f_f_?_s_t_y_l_e_=_s_q_u_a_r_e_&_l_a_b_e_l_=_S_t_a_r_s_&_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_n_e_D_i_f_f_-_C_o_m_m_u_n_i_t_y_ _w_i_k_i_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_T_w_i_t_t_e_r_-_D_i_s_c_u_s_s_-
+_g_r_e_e_n_?_l_o_g_o_=_t_w_i_t_t_e_r_&_a_m_p_][![](https://dcbadge.vercel.app/api/server/
+RKJTjZMcPQ?style=square)](https://discord.gg/RKJTjZMcPQ) _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_m_i_l_e_s_t_o_n_e_s_/_p_r_o_g_r_e_s_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_/_3_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_s_i_l_i_c_o_n_f_l_o_w_/_o_n_e_d_i_f_f_?_l_a_b_e_l_=_I_s_s_u_e_s_][![Docker image
+build](https://github.com/siliconflow/onediff/actions/workflows/sd.yml/
+badge.svg)](https://github.com/siliconflow/onediff/actions/workflows/sd.yml) [!
+[CI testing](https://github.com/siliconflow/onediff/actions/workflows/
+examples.yml/badge.svg?event=schedule)](https://github.com/siliconflow/onediff/
+actions/workflows/examples.yml?query=event%3Aschedule) ## OneDiff OneDiff is an
+out-of-the-box acceleration library for diffusion models, it provides: -
+PyTorch Module compilation tools and strong optimized GPU Kernels for diffusion
+models - Out-of-the-box acceleration for popular UIs/libs - [OneDiff for HF
+diffusers ð¤](https://github.com/siliconflow/onediff/tree/main/
 onediff_diffusers_extensions) - [OneDiff for ComfyUI](https://github.com/
 siliconflow/onediff/tree/main/onediff_comfy_nodes) - [OneDiff for Stable
 Diffusion web UI](https://github.com/siliconflow/onediff/tree/main/
 onediff_sd_webui_extensions) For example: [imgs/replace_a100.png]## News
 OneDiff is the abbreviation of "**one** line of code to accelerate
 **diff**usion models". Here is the latest news: - :rocket:[Accelerating Stable
 Video Diffusion 3x faster with OneDiff DeepCache + Int8](https://
```

### Comparing `onediff-1.0.0.dev202404160125/src/onediff.egg-info/SOURCES.txt` & `onediff-1.0.0.dev202404170125/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/tests/test_dual_module_list.py` & `onediff-1.0.0.dev202404170125/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.0.0.dev202404170125/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/tests/test_quantitative_quality.py` & `onediff-1.0.0.dev202404170125/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404160125/tests/test_quantize_custom_model.py` & `onediff-1.0.0.dev202404170125/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

