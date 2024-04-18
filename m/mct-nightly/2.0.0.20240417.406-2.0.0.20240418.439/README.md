# Comparing `tmp/mct-nightly-2.0.0.20240417.406.tar.gz` & `tmp/mct-nightly-2.0.0.20240418.439.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240417.406.tar", last modified: Wed Apr 17 00:04:07 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240418.439.tar", last modified: Thu Apr 18 00:04:39 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240417.406.tar` & `mct-nightly-2.0.0.20240418.439.tar`

### file list

```diff
@@ -1,604 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.372760 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-17 00:04:07.000000 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37225 2024-04-17 00:04:07.000000 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:04:07.000000 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 00:04:07.000000 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 00:04:07.000000 mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.372760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-17 00:04:06.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.372760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.376760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.376760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.376760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.376760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.376760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38259 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    28492 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.380760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.380760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.380760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.380760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.384760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.388760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    27014 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.388760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.388760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.392760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.392760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.392760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.396760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.396760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.396760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29309 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.400760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.404760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.408760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.408760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.408760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.408760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27117 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.412760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.416761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.420760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.424760 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.428761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.432761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.436761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.440761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-17 00:03:31.000000 mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-17 00:04:07.444761 mct-nightly-2.0.0.20240417.406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-17 00:04:06.000000 mct-nightly-2.0.0.20240417.406/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19993 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.888596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38259 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28499 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.892596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.896596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.900596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.904596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.904596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27014 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.908596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.912596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29457 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.916597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.920596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.924596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.928596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.932597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.936596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.940596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.944596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.948597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.952597 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.956596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:04:39.960596 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-18 00:04:03.000000 mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 00:04:39.964597 mct-nightly-2.0.0.20240418.439/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-18 00:04:39.000000 mct-nightly-2.0.0.20240418.439/setup.py
```

### Comparing `mct-nightly-2.0.0.20240417.406/LICENSE.md` & `mct-nightly-2.0.0.20240418.439/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/PKG-INFO` & `mct-nightly-2.0.0.20240418.439/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240417.406
+Version: 2.0.0.20240418.439
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240417.406/README.md` & `mct-nightly-2.0.0.20240418.439/README.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240417.406
+Version: 2.0.0.20240418.439
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
```

### Comparing `mct-nightly-2.0.0.20240417.406/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240418.439/mct_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 model_compression_toolkit/core/common/substitutions/__init__.py
 model_compression_toolkit/core/common/substitutions/apply_substitutions.py
 model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
 model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
 model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
 model_compression_toolkit/core/common/substitutions/linear_collapsing.py
 model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+model_compression_toolkit/core/common/substitutions/remove_identity.py
 model_compression_toolkit/core/common/substitutions/residual_collapsing.py
 model_compression_toolkit/core/common/substitutions/scale_equalization.py
 model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/common/substitutions/softmax_shift.py
 model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/common/substitutions/weights_activation_split.py
 model_compression_toolkit/core/common/visualization/__init__.py
@@ -179,14 +180,15 @@
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
@@ -243,14 +245,15 @@
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240417.000406"
+__version__ = "2.0.0.20240418.000439"
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 DEFAULT_DEC_FACTOR = (1.02, 0.98)
 DEFAULT_TOL = 1e-11
 BOTTOM_FACTOR = 0.7
 UPPER_FACTOR = 1.2
 DEC_RANGE_BOTTOM = 0.97
 DEC_RANGE_UPPER = 1.03
 
+NUM_QPARAM_HESSIAN_SAMPLES = 16
+
 # Resource utilization computation parameters
 BITS_TO_BYTES = 8.0
 
 # Default threshold for Softmax layer
 SOFTMAX_THRESHOLD = 1
 
 # Substitutions node names
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import copy
-from typing import Dict, Any, Tuple, List, Type
+from typing import Dict, Any, Tuple, List, Type, Union
 
 import numpy as np
 
 from model_compression_toolkit.constants import WEIGHTS_NBITS_ATTRIBUTE, CORRECTED_BIAS_ATTRIBUTE, \
     ACTIVATION_NBITS_ATTRIBUTE, FP32_BYTES_PER_PARAMETER
 from model_compression_toolkit.core.common.quantization.node_quantization_config import WeightsAttrQuantizationConfig
 from model_compression_toolkit.logger import Logger
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 # ==============================================================================
 
 from functools import partial
 from typing import Callable, List
 
 from model_compression_toolkit.constants import HESSIAN_NUM_ITERATIONS
-from model_compression_toolkit.core.common import Graph
 from model_compression_toolkit.core.common.hessian.trace_hessian_request import TraceHessianRequest
 from model_compression_toolkit.logger import Logger
 
 
 class HessianInfoService:
     """
     A service to manage, store, and compute approximation of the Hessian-based information.
@@ -34,15 +33,15 @@
     Note:
     - The Hessian provides valuable information about the curvature of the loss function.
     - Computation can be computationally heavy and time-consuming.
     - The computed trace is an approximation.
     """
 
     def __init__(self,
-                 graph: Graph,
+                 graph,
                  representative_dataset: Callable,
                  fw_impl,
                  num_iterations_for_approximation: int = HESSIAN_NUM_ITERATIONS
                  ):
         """
 
         Args:
@@ -147,15 +146,15 @@
             The outer list is per image (thus, has the length as required_size).
             The inner list length dependent on the granularity (1 for per-tensor, 
             OC for per-output-channel when the requested node has OC output-channels, etc.)
         """
         if required_size==0:
             return []
 
-        Logger.info(f"Ensuring {required_size} Hessian-trace approximation for node {trace_hessian_request.target_node}.")
+        Logger.info(f"\nEnsuring {required_size} Hessian-trace approximation for node {trace_hessian_request.target_node}.")
 
         # Replace request of a reused target node with a request of the 'reuse group'.
         if trace_hessian_request.target_node.reuse_group:
             trace_hessian_request = self._get_request_of_reuse_group(trace_hessian_request)
 
         # Ensure the saved info has the required number of approximations
         self._populate_saved_info_to_size(trace_hessian_request, required_size)
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 from enum import Enum
 
-from model_compression_toolkit.core.common import BaseNode
-
 
 class HessianMode(Enum):
     """
     Enum representing the mode for Hessian information computation.
 
     This determines whether the Hessian's approximation is computed w.r.t weights or w.r.t activations.
     Note: This is not the actual Hessian but an approximation.
@@ -50,15 +48,15 @@
     It specifies the mode (weights/activations), granularity (element/channel/tensor), and the target node.
     Note: This does not compute the actual Hessian's trace but approximates it.
     """
 
     def __init__(self,
                  mode: HessianMode,
                  granularity: HessianInfoGranularity,
-                 target_node: BaseNode,
+                 target_node,
                  ):
         """
         Attributes:
             mode (HessianMode): Mode of Hessian's trace approximation (w.r.t weights or activations).
             granularity (HessianInfoGranularity): Granularity level for the approximation.
             target_node (BaseNode): The node in the float graph for which the Hessian's trace approximation is targeted.
         """
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,32 @@
 
 class QuantizationErrorMethod(Enum):
     """
     Method for quantization threshold selection:
 
     NOCLIPPING - Use min/max values as thresholds.
 
-    MSE - Use min square error for minimizing quantization noise.
+    MSE - Use mean square error for minimizing quantization noise.
 
-    MAE - Use min absolute error for minimizing quantization noise.
+    MAE - Use mean absolute error for minimizing quantization noise.
 
     KL - Use KL-divergence to make signals distributions to be similar as possible.
 
     Lp - Use Lp-norm to minimizing quantization noise.
 
+    HMSE - Use Hessian-based mean squared error for minimizing quantization noise. This method is using Hessian scores to factorize more valuable parameters when computing the error induced by quantization.
+
     """
 
     NOCLIPPING = 0
     MSE = 1
     MAE = 2
     KL = 4
     LP = 5
+    HMSE = 6
 
 
 class QuantizationConfig:
 
     def __init__(self,
                  activation_error_method: QuantizationErrorMethod = QuantizationErrorMethod.MSE,
                  weights_error_method: QuantizationErrorMethod = QuantizationErrorMethod.MSE,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from copy import deepcopy
-from typing import Tuple, Callable
+from typing import Tuple, Callable, List
 import numpy as np
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
+from model_compression_toolkit.core.common.hessian import TraceHessianRequest, HessianMode, HessianInfoGranularity, \
+    HessianInfoService
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse, compute_mae, compute_lp_norm
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.constants import FLOAT_32
-from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor
+from model_compression_toolkit.constants import FLOAT_32, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor, \
+    reshape_tensor_for_per_channel_search
 
 
 def _mse_error_histogram(q_bins: np.ndarray,
                          q_count: np.ndarray,
                          bins: np.ndarray,
                          counts: np.ndarray) -> np.float32:
     """
@@ -367,32 +370,85 @@
 
     bins_subset = deepcopy(bins[first_bin_idx:last_bin_idx + 1])
     counts_subset = deepcopy(counts[first_bin_idx:last_bin_idx])
 
     return bins_subset, counts_subset
 
 
+def _compute_hessian_for_hmse(node,
+                              hessian_info_service: HessianInfoService,
+                              num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> List[np.ndarray]:
+    """
+    Compute and retrieve Hessian-based scores for using during HMSE error computation.
+
+    Args:
+        node: The node to compute Hessian-based scores for.
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores.
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on.
+
+    Returns: A list with computed Hessian-based scores tensors for the given node.
+
+    """
+    _request = TraceHessianRequest(mode=HessianMode.WEIGHTS,
+                                   granularity=HessianInfoGranularity.PER_ELEMENT,
+                                   target_node=node)
+    _scores_for_node = hessian_info_service.fetch_hessian(_request,
+                                                          required_size=num_hessian_samples)
+
+    return _scores_for_node
+
+
+def _hmse_error_function_wrapper(float_tensor: np.ndarray,
+                                 fxp_tensor: np.ndarray,
+                                 axis: int,
+                                 norm: bool,
+                                 hessian_scores: np.ndarray):
+    """
+    This function wraps the HMSE error method to enable using it during parameters selection.
+
+    Args:
+        float_tensor: Float tensor.
+        fxp_tensor: Quantized tensor.
+        axis: Axis along which the operation has been performed. If not None, then per-channel computation is expected.
+        norm: Indicates whether to normalize the result of the error function.
+        hessian_scores: A tensor with Hessian-based scores to use for Hessian-based MSE (HMSE) error computation.
+
+    Returns: The HMSE error between the float and fixed-point tensors.
+
+    """
+    if axis is not None:
+        hessian_scores = reshape_tensor_for_per_channel_search(hessian_scores, 0)
+
+    return compute_mse(float_tensor, fxp_tensor, axis, norm, weights=hessian_scores)
+
+
 def get_threshold_selection_tensor_error_function(quantization_method: QuantizationMethod,
                                                   quant_error_method: qc.QuantizationErrorMethod,
                                                   p: int,
                                                   axis: int = None,
                                                   norm: bool = False,
                                                   n_bits: int = 8,
-                                                  signed: bool = True) -> Callable:
+                                                  signed: bool = True,
+                                                  node=None,
+                                                  hessian_info_service: HessianInfoService = None,
+                                                  num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Callable:
     """
     Returns the error function compatible to the provided threshold method,
     to be used in the threshold optimization search for tensor quantization.
     Args:
         quantization_method: Method used for selecting the quantization threshold.
         quant_error_method: Type of error function requested.
         p: P-norm to use for calculating the Lp-norm distance.
         axis: Axis along which the operation has been performed.
         norm: Indicates whether to normalize the result of the error function.
         n_bits: Number of bits used to quantize the tensor.
         signed: Indicates whether the input is signed.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns: a Callable method that calculates the error between a tensor and a quantized tensor.
     """
     if quant_error_method == qc.QuantizationErrorMethod.KL:
         if axis is None:
             # per-tensor
             if quantization_method == QuantizationMethod.UNIFORM:
@@ -414,14 +470,21 @@
                                                                           per_channel=True)
             else:
                 return lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=0 if not signed else -threshold,
                                                                           range_max=threshold,
                                                                           n_bits=n_bits,
                                                                           per_channel=True)
 
+    if quant_error_method == qc.QuantizationErrorMethod.HMSE:
+        node_hessian_scores = _compute_hessian_for_hmse(node, hessian_info_service, num_hessian_samples)
+        node_hessian_scores = np.sqrt(np.mean(node_hessian_scores, axis=0))
+
+        return lambda x, y, threshold: _hmse_error_function_wrapper(x, y, norm=norm, axis=axis,
+                                                                    hessian_scores=node_hessian_scores)
+
     quant_method_error_function_mapping = {
         qc.QuantizationErrorMethod.MSE: lambda x, y, threshold: compute_mse(x, y, norm=norm, axis=axis),
         qc.QuantizationErrorMethod.MAE: lambda x, y, threshold: compute_mae(x, y, norm=norm, axis=axis),
         qc.QuantizationErrorMethod.LP: lambda x, y, threshold: compute_lp_norm(x, y, p=p, norm=norm, axis=axis),
     }
 
     return quant_method_error_function_mapping[quant_error_method]
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # ==============================================================================
 
 import numpy as np
 from sklearn.cluster import KMeans
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
 from model_compression_toolkit.constants import LUT_VALUES, MIN_THRESHOLD, SCALE_PER_CHANNEL, \
-    LUT_VALUES_BITWIDTH, THRESHOLD
+    LUT_VALUES_BITWIDTH, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     max_power_of_two, int_quantization_with_threshold
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.symmetric_selection import \
     symmetric_selection_tensor
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.power_of_two_selection import \
     power_of_two_selection_tensor
 
@@ -33,15 +34,18 @@
                       p: int,
                       n_bits: int,
                       per_channel: bool = False,
                       channel_axis: int = 1,
                       n_iter: int = 10,
                       min_threshold: float = MIN_THRESHOLD,
                       quant_error_method: qc.QuantizationErrorMethod = None,
-                      is_symmetric=False) -> dict:
+                      is_symmetric=False,
+                      node=None,
+                      hessian_info_service: HessianInfoService = None,
+                      num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
     """
     The quantizer first finds the closest max value per channel of tensor_data.
     Now, we divide tensor_data with the threshold vector per channel. In addition, we scale the result to the range
     [-2^(LUT_VALUES_BITWIDTH-1), 2^(LUT_VALUES_BITWIDTH-1)-1].
     Next, we take the scaled tensor_data and perform k-means clustering with 2^nbit clusters.
     We return the rounded cluster centers, and threshold per channel. We use these to quantize the data.
     Args:
@@ -49,15 +53,18 @@
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search_methods for the optimal threshold.
         min_threshold: Minimal threshold to chose when the computed one is smaller.
         quant_error_method: an error function to optimize the parameters' selection accordingly (not used for this method).
-        is_symmetric (bool): Whether to apply symmetric weight quantization (default is False, meaning power of 2 quantization)
+        is_symmetric (bool): Whether to apply symmetric weight quantization (default is False, meaning power of 2 quantization).
+        node: The node for which the quantization error is computed (not used for this method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (not used for this method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (not used for this method).
 
     Returns:
         A dictionary containing the cluster assignments according to the k-means algorithm,
         the thresholds per channel and the multiplier num bits.
     """
     if n_bits >= LUT_VALUES_BITWIDTH:
         Logger.critical(f'Look-Up-Table (LUT) bit configuration exceeds maximum: {n_bits} bits provided, must be less than {LUT_VALUES_BITWIDTH} bits.')  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_selection_tensor_search, qparams_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import max_power_of_two, get_tensor_max
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
@@ -27,42 +28,51 @@
 def power_of_two_selection_tensor(tensor_data: np.ndarray,
                                   p: int,
                                   n_bits: int,
                                   per_channel: bool = False,
                                   channel_axis: int = 1,
                                   n_iter: int = 10,
                                   min_threshold: float = MIN_THRESHOLD,
-                                  quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                                  quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                                  node=None,
+                                  hessian_info_service: HessianInfoService = None,
+                                  num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES,
+                                  ) -> dict:
     """
     Compute the power of two threshold based on the provided QuantizationErrorMethod to quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Power of two threshold to quantize the tensor in a power of 2 manner.
     """
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits)
         threshold = max_power_of_two(tensor_max, min_threshold)
     else:
         signed = True  # weights are always signed
         axis = -1 if per_channel else None
         error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.POWER_OF_TWO,
-                                                                       quant_error_method, p, axis=axis, norm=False, n_bits=n_bits,
-                                                                       signed=signed)
+                                                                       quant_error_method, p, axis=axis, norm=False,
+                                                                       n_bits=n_bits, signed=signed, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         threshold = qparams_selection_tensor_search(error_function,
                                                     tensor_data,
                                                     n_bits,
                                                     per_channel=per_channel,
                                                     channel_axis=channel_axis,
                                                     n_iter=n_iter,
                                                     min_threshold=min_threshold,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,97 @@
-# Copyright 2021 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from tqdm import tqdm
-from typing import List
-
-from model_compression_toolkit.core.common import Graph, BaseNode
-from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_activations_computation \
-    import get_activations_qparams
-from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_weights_computation import \
-    get_weights_qparams
-from model_compression_toolkit.logger import Logger
-
-
-def calculate_quantization_params(graph: Graph,
-                                  nodes: List[BaseNode] = [],
-                                  specific_nodes: bool = False):
-    """
-    For a graph, go over its nodes, compute quantization params (for both weights and activations according
-    to the given framework info), and create and attach a NodeQuantizationConfig to each node (containing the
-    computed params).
-    By default, the function goes over all nodes in the graph. However, the specific_nodes flag enables
-    to compute quantization params for specific nodes if the default behavior is unnecessary. For that,
-    a list of nodes should be passed as well.
-
-    Args:
-        groups of layers by how they should be quantized, etc.)
-        graph: Graph to compute its nodes' thresholds.
-        nodes: List of nodes to compute their thresholds instead of computing it for all nodes in the graph.
-        specific_nodes: Flag to compute thresholds for only specific nodes.
-
-    """
-
-    Logger.info(f"\nRunning quantization parameters search. "
-                f"This process might take some time, "
-                f"depending on the model size and the selected quantization methods.\n")
-
-    # Create a list of nodes to compute their thresholds
-    nodes_list: List[BaseNode] = nodes if specific_nodes else graph.nodes()
-
-    for n in tqdm(nodes_list, "Calculating quantization parameters"):  # iterate only nodes that we should compute their thresholds
-        for candidate_qc in n.candidates_quantization_cfg:
-            for attr in n.get_node_weights_attributes():
-                if n.is_weights_quantization_enabled(attr):
-                    # If the node's weights attribute should be quantized, we compute its quantization parameters
-                    attr_cfg = candidate_qc.weights_quantization_cfg.get_attr_config(attr)
-                    channels_axis = attr_cfg.weights_channels_axis
-                    if channels_axis is not None:
-                        output_channels_axis = channels_axis[0]
-                    else:
-                        output_channels_axis = None
-                    weights_params = get_weights_qparams(n.get_weights_by_keys(attr),
-                                                         candidate_qc.weights_quantization_cfg,
-                                                         attr_cfg,
-                                                         output_channels_axis)
-                    attr_cfg.set_weights_quantization_param(weights_params)
-
-            if n.is_activation_quantization_enabled():
-                # If node's activations should be quantized as well, we compute its activation quantization parameters
-                activation_params = get_activations_qparams(
-                    activation_quant_cfg=candidate_qc.activation_quantization_cfg,
-                    nodes_prior_info=n.prior_info,
-                    out_stats_container=graph.get_out_stats_collector(n))
-                # Create a NodeQuantizationConfig containing all quantization params and attach it to the node
-                candidate_qc.activation_quantization_cfg.set_activation_quantization_param(activation_params)
+from abc import ABC
+from typing import Dict, List
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+
+
+class TrainableQuantizerCandidateConfig:
+
+    def __init__(self,
+                 n_bits: int,
+                 quantization_params: Dict,
+                 ):
+        """
+        Class for representing candidates of quantization configurations for trainable quantizer.
+        It can be used for weights and activation quantization configuration.
+
+        Args:
+            n_bits (int): Number of bits to use for quantization.
+            quantization_params (Dict): Dictionary that contains quantization params.
+        """
+
+        self.n_bits = n_bits
+        self.quantization_params = quantization_params
+
+
+class TrainableQuantizerActivationConfig:
+
+    def __init__(self,
+                 activation_quantization_method: QuantizationMethod,
+                 activation_n_bits: int,
+                 activation_quantization_params: Dict,
+                 enable_activation_quantization: bool,
+                 min_threshold: float,
+                 activation_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None,
+                 ):
+        """
+        Attributes for configuring activations trainable quantizer.
+
+        Args:
+            activation_quantization_method (QuantizationMethod): Which method to use from QuantizationMethod for activation quantization.
+            activation_n_bits (int): Number of bits to quantize the activations.
+            activation_quantization_params (Dict): Dictionary that contains activation quantization params.
+            enable_activation_quantization (bool): Whether to quantize the layer's activations or not.
+            min_threshold (float): Minimum threshold to use during thresholds selection.
+        """
+        self.activation_quantization_method = activation_quantization_method
+        self.activation_n_bits = activation_n_bits
+        self.activation_quantization_params = activation_quantization_params
+        self.enable_activation_quantization = enable_activation_quantization
+        self.min_threshold = min_threshold
+        self.activation_bits_candidates = activation_quantization_candidates
+
+
+class TrainableQuantizerWeightsConfig:
+    def __init__(self,
+                 weights_quantization_method: QuantizationMethod,
+                 weights_n_bits: int,
+                 weights_quantization_params: Dict,
+                 enable_weights_quantization: bool,
+                 weights_channels_axis: int,
+                 weights_per_channel_threshold: bool,
+                 min_threshold: float,
+                 weights_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None,
+                 ):
+        """
+        Attributes for configuring weights trainable quantizer.
+
+        Args:
+            weights_quantization_method (QuantizationMethod): Which method to use from QuantizationMethod for weights quantization.
+            weights_n_bits (int): Number of bits to quantize the coefficients.
+            weights_quantization_params (Dict): Dictionary that contains weights quantization params.
+            enable_weights_quantization (bool): Whether to quantize the layer's weights or not.
+            weights_channels_axis (int): Axis to quantize a node's kernel when quantizing per-channel.
+            weights_per_channel_threshold (bool): Whether to quantize the weights per-channel or not (per-tensor).
+            min_threshold (float): Minimum threshold to use during thresholds selection.
+        """
+        self.weights_quantization_method = weights_quantization_method
+        self.weights_n_bits = weights_n_bits
+        self.weights_quantization_params = weights_quantization_params
+        self.enable_weights_quantization = enable_weights_quantization
+        self.weights_channels_axis = weights_channels_axis
+        self.weights_per_channel_threshold = weights_per_channel_threshold
+        self.min_threshold = min_threshold
+        self.weights_bits_candidates = weights_quantization_candidates
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,54 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict, Any, Tuple
+from typing import Dict, Any
 
 import numpy as np
 
-from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeWeightsQuantizationConfig, \
     WeightsAttrQuantizationConfig
 
 # If the quantization config does not contain kernel channel mapping or the weights
 # quantization is not per-channel, we use a dummy channel mapping.
 dummy_channel_mapping = DefaultDict(default_value=(None, None))
 
 
-def get_weights_qparams(kernel: np.ndarray,
+def get_weights_qparams(weights_attr_values: np.ndarray,
                         weights_quant_config: NodeWeightsQuantizationConfig,
                         attr_quant_config: WeightsAttrQuantizationConfig,
-                        output_channels_axis: int) -> Dict[Any, Any]:
+                        output_channels_axis: int,
+                        node=None,
+                        hessian_info_service: HessianInfoService = None,
+                        num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Dict[Any, Any]:
     """
     Compute thresholds to quantize a kernel according to a NodeWeightsQuantizationConfig
     instance.
 
     Args:
-        kernel: Kernel to compute the quantization thresholds to.
+        weights_attr_values: Weights attribute parameter to compute the quantization thresholds for.
         weights_quant_config: Weights quantization configuration to define how the thresholds are computed.
         attr_quant_config: A specific weights attribute quantization configuration to get its params.
         output_channels_axis: Index of the kernel output channels dimension.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         A dictionary with the quantization threshold of the kernel.
     """
     if attr_quant_config.weights_quantization_params_fn is not None:
-        weights_params = attr_quant_config.weights_quantization_params_fn(kernel,
+        weights_params = attr_quant_config.weights_quantization_params_fn(weights_attr_values,
                                                                           p=attr_quant_config.l_p_value,
                                                                           n_bits=attr_quant_config.weights_n_bits,
                                                                           per_channel=attr_quant_config.weights_per_channel_threshold and output_channels_axis is not None,
                                                                           channel_axis=output_channels_axis,
                                                                           min_threshold=weights_quant_config.min_threshold,
-                                                                          quant_error_method=attr_quant_config.weights_error_method)
+                                                                          quant_error_method=attr_quant_config.weights_error_method,
+                                                                          node=node,
+                                                                          hessian_info_service=hessian_info_service,
+                                                                          num_hessian_samples=num_hessian_samples)
     else:
         weights_params = {}
 
     return weights_params
 
 
 def _get_kernel_channels_mapping(fw_info:FrameworkInfo,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function, _kl_error_histogram
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_symmetric_selection_tensor_search, \
     qparams_symmetric_selection_histogram_search, kl_qparams_symmetric_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     get_tensor_max
@@ -29,41 +30,51 @@
 def symmetric_selection_tensor(tensor_data: np.ndarray,
                                p: int,
                                n_bits: int,
                                per_channel: bool = False,
                                channel_axis: int = 1,
                                n_iter: int = 10,
                                min_threshold: float = MIN_THRESHOLD,
-                               quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                               quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                               node=None,
+                               hessian_info_service: HessianInfoService = None,
+                               num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
     """
     Compute the optimal threshold based on the provided QuantizationErrorMethod to quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Optimal threshold to quantize the tensor in a symmetric manner.
     """
 
     tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits)
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         threshold = get_init_threshold(min_threshold, tensor_max, per_channel)
     else:
         signed = True  # weights are always signed
         axis = -1 if per_channel else None
-        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.SYMMETRIC, quant_error_method, p, axis=axis, norm=False, n_bits=n_bits, signed=signed)
+        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.SYMMETRIC, quant_error_method,
+                                                                       p, axis=axis, norm=False, n_bits=n_bits,
+                                                                       signed=signed, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         threshold = qparams_symmetric_selection_tensor_search(error_function,
                                                               tensor_data,
                                                               tensor_max,
                                                               n_bits,
                                                               per_channel,
                                                               channel_axis,
                                                               min_threshold=min_threshold,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_uniform_selection_tensor_search, qparams_uniform_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import get_tensor_max, \
     get_tensor_min
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
@@ -27,41 +28,50 @@
 def uniform_selection_tensor(tensor_data: np.ndarray,
                              p: int,
                              n_bits: int,
                              per_channel: bool = False,
                              channel_axis: int = 1,
                              n_iter: int = 10,
                              min_threshold: float = MIN_THRESHOLD,
-                             quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                             quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                             node=None,
+                             hessian_info_service: HessianInfoService = None,
+                             num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
     """
     Compute the optimal quantization range based on the provided QuantizationErrorMethod
     to uniformly quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the range parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Optimal quantization range to quantize the tensor uniformly.
     """
     tensor_min = get_tensor_min(tensor_data, per_channel, channel_axis)
     tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits, is_uniform_quantization=True)
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         mm = tensor_min, tensor_max
     else:
         axis = -1 if per_channel else None
-        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.UNIFORM, quant_error_method, p, axis=axis, norm=False)
+        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.UNIFORM, quant_error_method,
+                                                                       p, axis=axis, norm=False, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         mm = qparams_uniform_selection_tensor_search(error_function,
                                                      tensor_data,
                                                      tensor_min,
                                                      tensor_max,
                                                      n_bits,
                                                      per_channel,
                                                      channel_axis)
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,39 +20,52 @@
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeActivationQuantizationConfig
-from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
+from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, \
+    QuantizationErrorMethod
 from model_compression_toolkit.core.common.quantization.quantization_params_fn_selection import \
     get_activation_quantization_params_fn, get_weights_quantization_params_fn
 from model_compression_toolkit.core.common.quantization.quantization_fn_selection import \
     get_weights_quantization_fn
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
     QuantizationConfigOptions
 
 
 def set_quantization_configuration_to_graph(graph: Graph,
                                             quant_config: QuantizationConfig,
-                                            mixed_precision_enable: bool = False) -> Graph:
+                                            mixed_precision_enable: bool = False,
+                                            running_gptq: bool = False) -> Graph:
     """
     Add quantization configuration for each graph node.
 
     Args:
         graph: Graph for which to add quantization info to each node.
         quant_config: Quantization configuration containing parameters for how the graph should be quantized.
-        mixed_precision_enable: is mixed precision enabled
+        mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns:
         The graph with quantization configurations attached to each node in it.
     """
 
+    if quant_config.weights_error_method == QuantizationErrorMethod.HMSE:
+        if not running_gptq:
+            Logger.warning(f"The HMSE error method for parameters selection is only supported when running GPTQ "
+                           f"optimization due to long execution time that is not suitable for basic PTQ. "
+                           f"Using the default MSE error method instead.")
+            quant_config.weights_error_method = QuantizationErrorMethod.MSE
+        else:
+            Logger.warning("Using the HMSE error method for weights quantization parameters search. "
+                           "Note: This method may significantly increase runtime during the parameter search process.")
+
     for n in graph.nodes:
         set_quantization_configs_to_node(node=n,
                                          quant_config=quant_config,
                                          fw_info=graph.fw_info,
                                          tpc=graph.tpc,
                                          mixed_precision_enable=mixed_precision_enable)
     return graph
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # ==============================================================================
 
 from typing import Any
 
 import numpy as np
 
 from model_compression_toolkit.constants import EPS
+from model_compression_toolkit.logger import Logger
+
 
 #########################
 #  Helpful functions
 #########################
 
 
 def validate_before_compute_similarity(float_tensor: Any, fxp_tensor: Any):
@@ -83,35 +85,45 @@
 
 
 def compute_mse(float_tensor: np.ndarray,
                 fxp_tensor: np.ndarray,
                 norm: bool = False,
                 norm_eps: float = 1e-8,
                 batch: bool = False,
-                axis: int = None) -> float:
+                axis: int = None,
+                weights: np.ndarray = None) -> float:
     """
     Compute the mean square error between two numpy arrays.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         norm: whether to normalize the error function result.
         norm_eps: epsilon value for error normalization stability.
         batch: Whether to run batch similarity analysis or not.
         axis: Axis along which the operator has been computed.
+        weights: Weights tensor to use for computing Weighted-MSE error computation.
 
     Returns:
         The MSE distance between the two tensors.
     """
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
     float_flat = flatten_tensor(float_tensor, batch, axis)
     fxp_flat = flatten_tensor(fxp_tensor, batch, axis)
 
-    error = ((float_flat - fxp_flat) ** 2).mean(axis=-1)
+    if weights is not None:
+        w_flat = flatten_tensor(weights, batch, axis)
+        if w_flat.shape != float_flat.shape:
+            Logger.critical(f"Shape mismatch: The shape of the weights tensor {weights.shape} does not match the shape "
+                            f"of the input tensors {float_flat.shape} for Weighted-MSE computation.")  # pragma: no cover
+        error = ((w_flat * (float_flat - fxp_flat)) ** 2).mean(axis=-1)
+    else:
+        error = ((float_flat - fxp_flat) ** 2).mean(axis=-1)
+
     if norm:
         error /= ((float_flat ** 2).mean(axis=-1) + norm_eps)
 
     return error
 
 
 def compute_mae(float_tensor: np.ndarray,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 def graph_preparation_runner(in_model: Any,
                              representative_data_gen: Callable,
                              quantization_config: QuantizationConfig,
                              fw_info: FrameworkInfo,
                              fw_impl: FrameworkImplementation,
                              tpc: TargetPlatformCapabilities,
                              tb_w: TensorboardWriter = None,
-                             mixed_precision_enable: bool = False) -> Graph:
+                             mixed_precision_enable: bool = False,
+                             running_gptq: bool = False) -> Graph:
     """
     Runs all required preparations in order to build a quantization graph from the given model,
     quantization configuration and target platform specifications.
     This runner include the following steps:
         - Reading and building a graph from the given model.
         - Setting quantization config to each relevant node in the graph.
         - Apply all necessary substitutions to finalize the graph for quantization.
@@ -55,14 +56,15 @@
         fw_info: Information needed for quantization about the specific framework (e.g., kernel channels indices,
             groups of layers by how they should be quantized, etc.).
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         tpc: TargetPlatformCapabilities object that models the inference target platform and
             the attached framework operator's information.
         tb_w: TensorboardWriter object for logging.
         mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns:
         An internal graph representation of the input model.
     """
 
     graph = read_model_to_graph(in_model,
                                 representative_data_gen,
@@ -75,40 +77,43 @@
 
     transformed_graph = get_finalized_graph(graph,
                                             tpc,
                                             quantization_config,
                                             fw_info,
                                             tb_w,
                                             fw_impl,
-                                            mixed_precision_enable=mixed_precision_enable)
+                                            mixed_precision_enable=mixed_precision_enable,
+                                            running_gptq=running_gptq)
 
     return transformed_graph
 
 
 def get_finalized_graph(initial_graph: Graph,
                         tpc: TargetPlatformCapabilities,
                         quant_config: QuantizationConfig = DEFAULTCONFIG,
                         fw_info: FrameworkInfo = None,
                         tb_w: TensorboardWriter = None,
                         fw_impl: FrameworkImplementation = None,
-                        mixed_precision_enable: bool = False) -> Graph:
+                        mixed_precision_enable: bool = False,
+                        running_gptq: bool = False) -> Graph:
     """
     Applies all edit operation (edit, substitutions, etc.) on the model's graph, to prepare it for the quantization
     process. All future graph substitutions and operations that change the graph should be added to this method.
 
     Args:
         initial_graph (Graph): Graph to apply the changes to.
         tpc (TargetPlatformCapabilities): TargetPlatformCapabilities object that describes the desired inference target platform (includes fusing patterns MCT should handle).
         quant_config (QuantizationConfig): QuantizationConfig containing parameters of how the model should be
             quantized.
         fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g.,
             kernel channels indices, groups of layers by how they should be quantized, etc.)
         tb_w (TensorboardWriter): TensorboardWriter object to use for logging events such as graphs, histograms, etc.
         fw_impl (FrameworkImplementation): FrameworkImplementation object with a specific framework methods implementation.
         mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns: Graph object that represents the model, after applying all required modifications to it.
     """
 
     ######################################
     # Graph substitution (prepare graph)
     ######################################
@@ -138,15 +143,16 @@
         tb_w.add_graph(transformed_graph, 'pre_statistics_collection_substitutions')
 
     ######################################
     # Add quantization configurations
     ######################################
     transformed_graph = set_quantization_configuration_to_graph(graph=transformed_graph,
                                                                 quant_config=quant_config,
-                                                                mixed_precision_enable=mixed_precision_enable)
+                                                                mixed_precision_enable=mixed_precision_enable,
+                                                                running_gptq=running_gptq)
 
     ######################################
     # Layer fusing
     ######################################
     transformed_graph = fusion(transformed_graph, tpc)
 
     ######################################
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import numpy as np
 import tensorflow as tf
 from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder
 from tensorflow.keras.models import Model
 
 from model_compression_toolkit.constants import HESSIAN_NUM_ITERATIONS
 from model_compression_toolkit.core.common.hessian import TraceHessianRequest, HessianMode, HessianInfoService
+from model_compression_toolkit.core.keras.graph_substitutions.substitutions.remove_identity import RemoveIdentity
 from model_compression_toolkit.core.keras.hessian.activation_trace_hessian_calculator_keras import \
     ActivationTraceHessianCalculatorKeras
 from model_compression_toolkit.core.keras.hessian.weights_trace_hessian_calculator_keras import WeightsTraceHessianCalculatorKeras
 from model_compression_toolkit.exporter.model_wrapper.fw_agnostic.get_inferable_quantizers import \
     get_inferable_quantizers
 from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizer import \
     get_weights_quantizer_for_node, get_activations_quantizer_for_node
@@ -242,15 +243,16 @@
         Returns: A list of the framework substitutions used to prepare the graph.
 
         """
         return [SeparableConvDecomposition(),
                 MatmulToDenseSubstitution(),
                 MultiHeadAttentionDecomposition(),
                 ActivationDecomposition(),
-                DwconvToConv()]
+                DwconvToConv(),
+                RemoveIdentity()]
 
     def get_substitutions_pre_statistics_collection(self, quant_config: QuantizationConfig) -> \
             List[common.BaseSubstitution]:
         """
         Return a list of the framework substitutions used before we collect statistics.
 
         Args:
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     import MultiHeadAttentionDecomposition
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.permute_call_method import \
     PermuteCallMethod
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.const_holder_conv import \
     FunctionalConvSubstitution
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.relu_bound_to_power_of_2 import \
     ReLUBoundToPowerOfTwo
+from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.remove_identity import RemoveIdentity
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.reshape_with_static_shapes import \
     ReshapeWithStaticShapes
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.residual_collapsing import \
     pytorch_residual_collapsing
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.scale_equalization import \
     ScaleEqualization, \
     ScaleEqualizationWithPad
@@ -234,15 +235,16 @@
 
         """
         return [ReshapeWithStaticShapes(),
                 MultiHeadAttentionDecomposition(),
                 PermuteCallMethod(),
                 FunctionalConvSubstitution(fw_info),
                 FunctionalBatchNorm(),
-                FunctionalLayerNorm()]
+                FunctionalLayerNorm(),
+                RemoveIdentity()]
 
     def get_substitutions_pre_statistics_collection(self,
                                                     quant_config: QuantizationConfig
                                                     ) -> List[common.BaseSubstitution]:
         """
         Args:
             quant_config: QuantizationConfig to determine which substitutions to return.
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import Callable
 
 from tqdm import tqdm
 
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.model_collector import ModelCollector
 from model_compression_toolkit.core.common.network_editors.edit_network import edit_network_graph
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_computation import \
     calculate_quantization_params
 from model_compression_toolkit.core.common.statistics_correction.statistics_correction import \
     statistics_correction_runner
@@ -34,15 +35,16 @@
 
 
 def quantization_preparation_runner(graph: Graph,
                                     representative_data_gen: Callable,
                                     core_config: CoreConfig,
                                     fw_info: FrameworkInfo,
                                     fw_impl: FrameworkImplementation,
-                                    tb_w: TensorboardWriter = None) -> Graph:
+                                    tb_w: TensorboardWriter = None,
+                                    hessian_info_service: HessianInfoService = None,) -> Graph:
     """
     Prepares a trained model for post-training quantization.
     First, the model graph is optimized using several transformations (e.g. folding BatchNormalization to preceding layers).
     Second, statistics (e.g. min/max, histogram, etc.) are collected for each layer's output
     (and input, depends on the quantization configuration) using a given representative dataset.
     Next, quantization parameters are calculated using the collected statistics.
     Finally, more transformations (based on the statistics) are applied to increase the model's performance.
@@ -51,14 +53,15 @@
         graph: A graph representation of the model to be quantized.
         representative_data_gen: Dataset used for calibration.
         core_config: CoreConfig containing parameters of how the model should be quantized
         fw_info: Information needed for quantization about the specific framework (e.g., kernel channels indices,
             groups of layers by how they should be quantized, etc.).
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         tb_w: TensorboardWriter object for logging
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores.
 
     Returns:
         Graph object that represents the model, contains thresholds, and ready for quantization.
     """
 
     ######################################
     # Statistic collection
@@ -82,15 +85,16 @@
     # there are no final configurations at this stage of the optimization). For this reason we edit the graph
     # again at the end of the optimization process.
     edit_network_graph(graph, fw_info, core_config.debug_config.network_editor)
 
     ######################################
     # Calculate quantization params
     ######################################
-    calculate_quantization_params(graph)
+
+    calculate_quantization_params(graph, hessian_info_service=hessian_info_service)
 
     if tb_w is not None:
         tb_w.add_graph(graph, 'thresholds_selection')
         tb_w.add_all_statistics(graph, 'thresholds_selection')
 
     ######################################
     # Graph substitution (post statistics collection)
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/core/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 def core_runner(in_model: Any,
                 representative_data_gen: Callable,
                 core_config: CoreConfig,
                 fw_info: FrameworkInfo,
                 fw_impl: FrameworkImplementation,
                 tpc: TargetPlatformCapabilities,
                 target_resource_utilization: ResourceUtilization = None,
+                running_gptq: bool = False,
                 tb_w: TensorboardWriter = None):
     """
     Quantize a trained model using post-training quantization.
     First, the model graph is optimized using several transformations (e.g. folding BatchNormalization to preceding
     layers).
     Second, statistics (e.g. min/max, histogram, etc.) are collected for each layer's output
     (and input, depends on the quantization configuration) using a given representative dataset.
@@ -93,26 +94,28 @@
     graph = graph_preparation_runner(in_model,
                                      representative_data_gen,
                                      core_config.quantization_config,
                                      fw_info,
                                      fw_impl,
                                      tpc,
                                      tb_w,
-                                     mixed_precision_enable=core_config.mixed_precision_enable)
+                                     mixed_precision_enable=core_config.mixed_precision_enable,
+                                     running_gptq=running_gptq)
 
     hessian_info_service = HessianInfoService(graph=graph,
                                               representative_dataset=representative_data_gen,
                                               fw_impl=fw_impl)
 
     tg = quantization_preparation_runner(graph=graph,
                                          representative_data_gen=representative_data_gen,
                                          core_config=core_config,
                                          fw_info=fw_info,
                                          fw_impl=fw_impl,
-                                         tb_w=tb_w)
+                                         tb_w=tb_w,
+                                         hessian_info_service=hessian_info_service)
 
     ######################################
     # Finalize bit widths
     ######################################
     if core_config.mixed_precision_enable:
         if core_config.mixed_precision_config.configuration_overwrite is None:
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,16 @@
         tg, bit_widths_config, hessian_info_service = core_runner(in_model=in_model,
                                                                   representative_data_gen=representative_data_gen,
                                                                   core_config=core_config,
                                                                   fw_info=DEFAULT_KERAS_INFO,
                                                                   fw_impl=fw_impl,
                                                                   tpc=target_platform_capabilities,
                                                                   target_resource_utilization=target_resource_utilization,
-                                                                  tb_w=tb_w)
+                                                                  tb_w=tb_w,
+                                                                  running_gptq=True)
 
         float_graph = copy.deepcopy(tg)
 
         tg_gptq = gptq_runner(tg,
                               core_config,
                               gptq_config,
                               representative_data_gen,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,17 @@
         graph, bit_widths_config, hessian_info_service = core_runner(in_model=model,
                                                                      representative_data_gen=representative_data_gen,
                                                                      core_config=core_config,
                                                                      fw_info=DEFAULT_PYTORCH_INFO,
                                                                      fw_impl=fw_impl,
                                                                      tpc=target_platform_capabilities,
                                                                      target_resource_utilization=target_resource_utilization,
-                                                                     tb_w=tb_w)
+                                                                     tb_w=tb_w,
+                                                                     running_gptq=True)
+
         float_graph = copy.deepcopy(graph)
 
         # ---------------------- #
         # GPTQ Runner
         # ---------------------- #
         graph_gptq = gptq_runner(graph,
                                  core_config,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/gptq/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     tg_bias = apply_statistics_correction(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
 
     if tb_w is not None:
         tb_w.add_graph(tg_bias, 'after_bias_correction')
     #############################################
     # Gradient Based Post Training Quantization
     #############################################
+    Logger.info("Running GPTQ optimization.")
     tg_gptq = _apply_gptq(gptq_config,
                           gptq_representative_data_gen,
                           tb_w,
                           tg,
                           tg_bias,
                           fw_info,
                           fw_impl,
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/metadata.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from model_compression_toolkit.constants import FOUND_TF, FOUND_TORCH
-from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tp_model import get_tp_model, generate_tp_model, \
+from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tp_model import get_tp_model, generate_tp_model, \
     get_op_quantization_configs
 if FOUND_TF:
-    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_keras import get_keras_tpc as get_keras_tpc_latest
-    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_keras import generate_keras_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_latest
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import generate_keras_tpc
 if FOUND_TORCH:
-    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_pytorch import get_pytorch_tpc as \
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import get_pytorch_tpc as \
         get_pytorch_tpc_latest
-    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_pytorch import generate_pytorch_tpc
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import generate_pytorch_tpc
```

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240418.439/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240417.406/setup.py` & `mct-nightly-2.0.0.20240418.439/setup.py`

 * *Files identical despite different names*

