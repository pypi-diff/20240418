# Comparing `tmp/quickstats-0.7.0.2.1.tar.gz` & `tmp/quickstats-0.7.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.2.1.tar", last modified: Thu Apr  4 00:49:34 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.2.2.tar", last modified: Thu Apr 18 15:26:38 2024, max compression
```

## Comparing `quickstats-0.7.0.2.1.tar` & `quickstats-0.7.0.2.2.tar`

### file list

```diff
@@ -1,280 +1,285 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-02 17:25:02.000000 quickstats-0.7.0.2.1/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       26 2024-04-04 00:47:52.000000 quickstats-0.7.0.2.1/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats/algorithms/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.1/quickstats/algorithms/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:14.000000 quickstats-0.7.0.2.1/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-02 17:36:56.000000 quickstats-0.7.0.2.1/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-02 18:33:01.000000 quickstats-0.7.0.2.1/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-03 08:27:44.000000 quickstats-0.7.0.2.1/quickstats/analysis/config_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-02 22:44:19.000000 quickstats-0.7.0.2.1/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-02 23:14:17.000000 quickstats-0.7.0.2.1/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-02 22:05:57.000000 quickstats-0.7.0.2.1/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31730 2024-04-02 17:50:16.000000 quickstats-0.7.0.2.1/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:14.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:15.000000 quickstats-0.7.0.2.1/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23980 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/likelihood_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/clis/nuisance_parameter_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.1/quickstats/clis/processor_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/clis/stat_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:18.000000 quickstats-0.7.0.2.1/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1003 2024-03-24 11:50:51.000000 quickstats-0.7.0.2.1/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15200 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/caching_nll_wrapper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/discrete_nuisance.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-03-22 06:53:00.000000 quickstats-0.7.0.2.1/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14303 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:20.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:20.000000 quickstats-0.7.0.2.1/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-03-24 11:56:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:24.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1417 2024-03-24 12:41:51.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-03-23 11:42:51.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      286 2024-03-24 07:41:44.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/formatter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1152 2024-03-23 11:29:11.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2202 2024-03-24 09:53:39.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1870 2024-03-24 09:53:36.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1479 2024-03-24 09:53:33.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 21:34:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_awkward_array.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3684 2024-03-24 12:44:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-03-23 11:32:05.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      951 2024-03-23 11:31:01.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-03-24 12:37:44.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1245 2024-03-23 11:35:28.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-03-23 11:30:06.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-03-23 11:33:46.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-03-23 11:33:27.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-03-23 11:35:50.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-03-23 11:32:55.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:21.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-03-23 11:43:26.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:23.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2919 2024-03-24 09:15:48.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_output_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-03-24 11:10:08.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-03-23 11:36:26.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1751 2024-03-24 12:35:52.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1466 2024-03-23 11:30:31.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-03-23 11:36:37.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2208 2024-03-24 09:53:22.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-23 11:32:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:18.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-03-23 11:35:43.000000 quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-03-21 10:53:35.000000 quickstats-0.7.0.2.1/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9214 2024-03-24 12:10:07.000000 quickstats-0.7.0.2.1/quickstats/components/processors/roo_process_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10075 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.1/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:24.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-03-22 11:17:26.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:25.000000 quickstats-0.7.0.2.1/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.2.1/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5291 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10858 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7544 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_significance.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      412 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32263 2024-04-03 08:15:13.000000 quickstats-0.7.0.2.1/quickstats/core/configurations.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/constraints.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4325 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7523 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-02 20:40:30.000000 quickstats-0.7.0.2.1/quickstats/core/metaclasses.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7290 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/core/setup.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-03 08:23:27.000000 quickstats-0.7.0.2.1/quickstats/core/type_validation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-03-23 10:27:07.000000 quickstats-0.7.0.2.1/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/extensions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/extensions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/extensions/extension_dataframe.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:27.000000 quickstats-0.7.0.2.1/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-25 07:40:31.000000 quickstats-0.7.0.2.1/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:28.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/basic_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/ModelConfig.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8814 2024-03-23 12:52:37.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RDataFrame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsArg.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-03-21 09:25:52.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TChain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8389 2024-03-26 09:52:30.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5747 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TH3.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-03-23 12:51:24.000000 quickstats-0.7.0.2.1/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      656 2024-03-22 00:45:22.000000 quickstats-0.7.0.2.1/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.2.1/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.2.1/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.1/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       61 2024-03-25 07:59:30.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      386 2024-03-26 07:09:55.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      421 2024-03-25 07:29:55.000000 quickstats-0.7.0.2.1/quickstats/interface/xrootd/utils.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:11.000000 quickstats-0.7.0.2.1/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:29.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-03-22 22:59:46.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.2.1/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6638 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    39416 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.2.1/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:30.000000 quickstats-0.7.0.2.1/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.2.1/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/param_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/parsers/roo_param_setup_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:32.000000 quickstats-0.7.0.2.1/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15928 2024-03-26 14:28:15.000000 quickstats-0.7.0.2.1/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14143 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.2.1/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-03-26 13:58:38.000000 quickstats-0.7.0.2.1/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7671 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.1/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4078 2024-03-23 07:31:01.000000 quickstats-0.7.0.2.1/quickstats/plots/general_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22373 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17020 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.7.0.2.1/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25852 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10391 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28865 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.7.0.2.1/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/two_axis_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10197 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19306 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot_deprecated.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13196 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23332 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.1/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31327 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:32.000000 quickstats-0.7.0.2.1/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/default_workspace_extensions.json
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:33.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.2.1/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17249 2024-04-03 00:26:22.000000 quickstats-0.7.0.2.1/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.2.1/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18636 2024-04-02 22:21:53.000000 quickstats-0.7.0.2.1/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.2.1/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2891 2024-03-26 09:43:05.000000 quickstats-0.7.0.2.1/quickstats/utils/path_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-03-27 12:33:54.000000 quickstats-0.7.0.2.1/quickstats/utils/py_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27148 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14094 2024-03-24 08:17:19.000000 quickstats-0.7.0.2.1/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13830 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.1/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1440 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.1/quickstats/utils/sys_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-02 23:53:41.000000 quickstats-0.7.0.2.1/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-04 00:49:12.000000 quickstats-0.7.0.2.1/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-04 00:49:04.000000 quickstats-0.7.0.2.1/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10677 2024-04-04 00:49:07.000000 quickstats-0.7.0.2.1/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-04 00:49:04.000000 quickstats-0.7.0.2.1/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-04 00:49:05.000000 quickstats-0.7.0.2.1/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-04 00:49:05.000000 quickstats-0.7.0.2.1/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-04 00:49:34.000000 quickstats-0.7.0.2.1/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-03-22 21:08:00.000000 quickstats-0.7.0.2.1/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.2/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.2/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-02 17:25:02.000000 quickstats-0.7.0.2.2/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       26 2024-04-04 17:36:02.000000 quickstats-0.7.0.2.2/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/algorithms/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.2.2/quickstats/algorithms/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-02 17:36:56.000000 quickstats-0.7.0.2.2/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-02 18:33:01.000000 quickstats-0.7.0.2.2/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-03 08:27:44.000000 quickstats-0.7.0.2.2/quickstats/analysis/config_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-04 15:51:04.000000 quickstats-0.7.0.2.2/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-04 17:31:40.000000 quickstats-0.7.0.2.2/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-02 23:14:17.000000 quickstats-0.7.0.2.2/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-02 22:05:57.000000 quickstats-0.7.0.2.2/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33328 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23980 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/likelihood_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.2/quickstats/clis/nuisance_parameter_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.2.2/quickstats/clis/processor_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/clis/stat_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.2/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15200 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/caching_nll_wrapper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/discrete_nuisance.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.2/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-03-22 06:53:00.000000 quickstats-0.7.0.2.2/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14303 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-02 17:25:03.000000 quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-03-24 11:56:22.000000 quickstats-0.7.0.2.2/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1417 2024-03-24 12:41:51.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-03-23 11:42:51.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-13 09:49:34.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/formatter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1983 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1592 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-03-23 11:32:05.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-03-24 12:37:44.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1245 2024-04-13 10:01:31.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-03-23 11:30:06.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-03-23 11:33:46.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-03-23 11:33:27.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-03-23 11:35:50.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-03-23 11:32:55.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:21.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-14 19:01:04.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3237 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-03-24 11:10:08.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-03-23 11:36:26.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-13 10:01:38.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-14 19:28:40.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-03-23 11:36:37.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1774 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-23 11:32:35.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-03-23 11:43:18.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-03-23 11:35:43.000000 quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-03-21 10:53:35.000000 quickstats-0.7.0.2.2/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12425 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/roo_process_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12542 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-03-22 11:17:26.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.2.2/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.2.2/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-13 10:47:30.000000 quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-13 10:47:42.000000 quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7654 2024-04-14 20:40:15.000000 quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_significance.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-13 01:05:18.000000 quickstats-0.7.0.2.2/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-12 08:58:57.000000 quickstats-0.7.0.2.2/quickstats/core/configuration.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/core/constraints.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-12 08:59:45.000000 quickstats-0.7.0.2.2/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-12 09:01:06.000000 quickstats-0.7.0.2.2/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-02 20:40:30.000000 quickstats-0.7.0.2.2/quickstats/core/metaclasses.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-16 19:54:23.000000 quickstats-0.7.0.2.2/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-02 17:25:04.000000 quickstats-0.7.0.2.2/quickstats/core/setup.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-03 08:23:27.000000 quickstats-0.7.0.2.2/quickstats/core/type_validation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-03-23 10:27:07.000000 quickstats-0.7.0.2.2/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/extensions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/extensions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/extensions/extension_dataframe.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-25 07:40:31.000000 quickstats-0.7.0.2.2/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/basic_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/interface/kerberos/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/kerberos/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/kerberos/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/ModelConfig.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8814 2024-03-23 12:52:37.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RDataFrame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsArg.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-03-21 09:25:52.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TChain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11400 2024-04-16 20:39:08.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5747 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TH3.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-03-23 12:51:24.000000 quickstats-0.7.0.2.2/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.2.2/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.2.2/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.2.2/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:35.000000 quickstats-0.7.0.2.2/quickstats/interface/servicex/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       91 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/servicex/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1725 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/servicex/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/filesystem.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/path.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2563 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/interface/xrootd/xrd_helper.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.2.2/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.2.2/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-03-22 22:59:46.000000 quickstats-0.7.0.2.2/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.2.2/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.2.2/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.2.2/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:36.000000 quickstats-0.7.0.2.2/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.2.2/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6638 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    39416 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.2.2/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:37.000000 quickstats-0.7.0.2.2/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.2.2/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/parsers/param_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/parsers/roo_param_setup_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17250 2024-04-14 20:45:25.000000 quickstats-0.7.0.2.2/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-14 20:38:10.000000 quickstats-0.7.0.2.2/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.2.2/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-03-26 13:58:38.000000 quickstats-0.7.0.2.2/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.2.2/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7581 2024-04-14 20:21:01.000000 quickstats-0.7.0.2.2/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-14 20:22:17.000000 quickstats-0.7.0.2.2/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22281 2024-04-14 20:22:39.000000 quickstats-0.7.0.2.2/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-14 20:46:58.000000 quickstats-0.7.0.2.2/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.2/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-14 20:23:14.000000 quickstats-0.7.0.2.2/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.2/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25762 2024-04-14 20:28:12.000000 quickstats-0.7.0.2.2/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-14 20:36:47.000000 quickstats-0.7.0.2.2/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-14 20:27:52.000000 quickstats-0.7.0.2.2/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.2/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30174 2024-04-14 20:16:42.000000 quickstats-0.7.0.2.2/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-14 20:31:15.000000 quickstats-0.7.0.2.2/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.2.2/quickstats/plots/two_axis_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-14 20:23:29.000000 quickstats-0.7.0.2.2/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-14 20:19:27.000000 quickstats-0.7.0.2.2/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-14 20:23:59.000000 quickstats-0.7.0.2.2/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23314 2024-04-14 20:25:25.000000 quickstats-0.7.0.2.2/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31313 2024-04-14 20:26:10.000000 quickstats-0.7.0.2.2/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/resources/default_workspace_extensions.json
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/quickstats/resources/mpl_stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.2.2/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19071 2024-04-14 19:14:39.000000 quickstats-0.7.0.2.2/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.2.2/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-16 19:54:24.000000 quickstats-0.7.0.2.2/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.2.2/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2197 2024-04-16 19:54:25.000000 quickstats-0.7.0.2.2/quickstats/utils/path_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-03-27 12:33:54.000000 quickstats-0.7.0.2.2/quickstats/utils/py_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-12 09:09:41.000000 quickstats-0.7.0.2.2/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.2.2/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-13 09:21:41.000000 quickstats-0.7.0.2.2/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-16 19:54:25.000000 quickstats-0.7.0.2.2/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-13 01:30:48.000000 quickstats-0.7.0.2.2/quickstats/utils/sys_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-02 23:53:41.000000 quickstats-0.7.0.2.2/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:26:34.000000 quickstats-0.7.0.2.2/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4127 2024-04-18 15:26:28.000000 quickstats-0.7.0.2.2/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10761 2024-04-18 15:26:32.000000 quickstats-0.7.0.2.2/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-18 15:26:28.000000 quickstats-0.7.0.2.2/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-18 15:26:28.000000 quickstats-0.7.0.2.2/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-18 15:26:28.000000 quickstats-0.7.0.2.2/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-18 15:26:38.000000 quickstats-0.7.0.2.2/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-03-22 21:08:00.000000 quickstats-0.7.0.2.2/setup.py
```

### Comparing `quickstats-0.7.0.2.1/PKG-INFO` & `quickstats-0.7.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.2.1
+Version: 0.7.0.2.2
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.2.1/README.md` & `quickstats-0.7.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.2.2/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.2.2/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.2.2/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/config_templates.py` & `quickstats-0.7.0.2.2/quickstats/analysis/config_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.2.2/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.2.2/quickstats/analysis/data_preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 def fix_negative_weights(df, mode:Union[int, NegativeWeightMode, str]=0,
                          weight_col:str="weight"):
     mode = NegativeWeightMode.parse(mode)
     if mode == NegativeWeightMode.DONOTHING:
         return None
     mask = df[weight_col] < 0
     if mode == NegativeWeightMode.SETZERO:
-        df[weight_col][mask] = 0
+        df.loc[mask, weight_col] = 0
     elif mode == NegativeWeightMode.SETABS:
-        df[weight_col][mask] = abs(df[weight_col][mask])
+        df.loc[mask, weight_col] = abs(df[weight_col][mask])
         
 def shuffle_arrays(*arrays, random_state:Optional[int]=None):
     if random_state < 0:
         return arrays
     from sklearn.utils import shuffle
     return shuffle(*arrays, random_state=random_state)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.2.2/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.2.2/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.2.2/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.2.2/quickstats/analysis/ntuple_process_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             
         if process_flags is not None:
             self.process_flags = list(process_flags)
         else:
             self.process_flags = []
         
         self.cutflow_report = None
+        self.process_metadata = {}
         
     def load_sample_config(self, config_source:Union[Dict, str]):
         if isinstance(config_source, str):
             if not os.path.exists(config_source):
                 raise FileNotFoundError(f'config file "{config_source}" does not exist')
             config_path = os.path.abspath(config_source)
             self.path_manager.set_file("sample_config", config_path)
@@ -392,15 +393,24 @@
                     "type": sample_type
                 }
                 self.processor.global_variables['sample'] = sample
                 self.processor.global_variables['sample_type'] = sample_type
                 self.processor.global_variables['outdir'] = outdir
                 self.prerun_process(sample_config)
                 self.processor.run(sample_paths)
+                self.set_process_metadata(sample, sample_type,
+                                          self.processor.result_metadata.copy())
                 self.processor.clear_global_variables()
+
+    def set_process_metadata(self, sample:str,
+                             sample_type:str,
+                             metadata:Dict):
+        if sample not in self.process_metadata:
+            self.process_metadata[sample] = {}
+        self.process_metadata[sample][sample_type] = metadata
                 
     def merge_outputs(self, source_path_func:Callable,
                       target_path_func:Callable,
                       merge_func:Callable,
                       outdir:str,
                       samples:Optional[List[str]]=None,
                       syst_themes:Optional[List[str]]=None,
@@ -641,8 +651,31 @@
             
             # Culmulative efficiency bar chart 
             axs[2].bar(cut_labels, df["yield_cumulative_efficiency"], color=colors[2])
             axs[2].set_ylabel("Cumulative Efficiency [%]", fontsize=14)
 
             fig.suptitle(f"Sample: {sample}", fontsize=20, y=0.98)
             
-            plt.show()
+            plt.show()
+
+    def copy_remote_samples(self, samples:Optional[Union[List[str], str]]=None,
+                            sample_types:Optional[Union[List[str], str]]=None,
+                            cache:bool=True,
+                            cachedir:str='/tmp',
+                            parallel:bool=False):
+        if isinstance(samples, str):
+            samples = [samples]
+        if isinstance(sample_types, str):
+            sample_types = [sample_types]
+        paths = self.get_selected_paths(syst_themes=['Nominal'],
+                                        samples=samples,
+                                        sample_types=sample_types)
+        if not paths:
+            self.stdout.warning('No inputs matching the given conditions. Skipped.')
+        paths = paths['Nominal']
+        filenames = []
+        for sample in paths:
+            for sample_type in paths[sample]:
+                filenames.extend(paths[sample][sample_type])
+        from quickstats.interface.root import TFile
+        TFile.copy_remote_files(filenames, cache=cache,
+                                cachedir=cachedir, parallel=parallel)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.2.2/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.2.2/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.2.2/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.2.2/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.2.2/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/core.py` & `quickstats-0.7.0.2.2/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.2.2/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.2.2/quickstats/clis/likelihood_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.2.2/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.2.2/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.2.2/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.2.2/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.2.2/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/analysis_base.py` & `quickstats-0.7.0.2.2/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/analysis_object.py` & `quickstats-0.7.0.2.2/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.2.2/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.2.2/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/basics.py` & `quickstats-0.7.0.2.2/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.2.2/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.2.2/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.2.2/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/extended_model.py` & `quickstats-0.7.0.2.2/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.2.2/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/likelihood.py` & `quickstats-0.7.0.2.2/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.2.2/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.2.2/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from typing import Optional
-import re
 
-from .rooproc_rdf_action import RooProcRDFAction
+from .rooproc_helper_action import RooProcHelperAction
 from .auxiliary import register_action
 
+from quickstats.utils.root_utils import declare_expression
+
 @register_action
-class RooProcAlias(RooProcRDFAction):
+class RooProcDeclare(RooProcHelperAction):
     
-    NAME = "ALIAS"
+    NAME = "DECLARE"
     
-    def __init__(self, alias:str, column_name:str):
-        super().__init__(alias=alias, column_name=column_name)
+    def __init__(self, expression:str, name:Optional[str]=None):
+        super().__init__(expression=expression,
+                         name=name)
+        
+    @staticmethod
+    def allow_multiline():
+        return True
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        result = re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)\s*$", main_text)
-        if not result:
-            if re.search(r"^\s*(\w+)\s*=\s*([\w\.\${}]+)", main_text):
-                raise RuntimeError(f'can not alias an expression ("{main_text}"), '
-                                   'please use DEFINE instead')
-            raise RuntimeError(f"invalid expression {main_text}")
-        alias = result.group(1)
-        column_name = result.group(2)
-        return cls(alias=alias, column_name=column_name)        
-        
-    def _execute(self, rdf:"ROOT.RDataFrame", **params):
-        alias = params['alias']
-        column_name = params['column_name']
-        rdf_next = rdf.Alias(alias, column_name)
-        return rdf_next
+        return cls(expression=main_text)        
+    
+    def _execute(self, processor:"quickstats.RooProcessor", **params):
+        name = params.get("name", None)
+        expression = params['expression']
+        declare_expression(expression, name)
+        return processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,40 @@
 
 from quickstats import module_exist
 from quickstats.utils.common_utils import is_valid_file
 from quickstats.utils.data_conversion import ConversionMode
 from quickstats.interface.root import RDataFrameBackend
 
 @register_action
-class RooProcAsHDF(RooProcOutputAction):
+class RooProcAsNumpy(RooProcOutputAction):
     
-    NAME = "AS_HDF"
+    NAME = "AS_NUMPY"
     
-    def __init__(self, filename:str, key:str,
-                 columns:Optional[List[str]]):
-        super().__init__(filename=filename,
-                         columns=columns,
-                         key=key)
-
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         filename = params['filename']
-        key = params['key']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
-        import awkward as ak
-        import pandas as pd
         columns = params.get('columns', None)
-        columns = self.get_valid_columns(rdf, processor, columns=columns,
-                                         mode=ConversionMode.REMOVE_NON_STANDARD_TYPE)
+        exclude = params.get('exclude', None)
+        save_columns = self.get_save_columns(rdf, processor, columns=columns,
+                                             exclude=exclude,
+                                             mode="REMOVE_NON_STANDARD_TYPE")
         array = None
         if module_exist('awkward'):
             try:
                 import awkward as ak
                 # NB: RDF Dask/Spark does not support GetColumnType yet
                 if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
                     rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
-                array = ak.from_rdataframe(rdf, columns=columns)
+                array = ak.from_rdataframe(rdf, columns=save_columns)
                 array = ak.to_numpy(array)
             except:
                 array = None
                 processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
                                          "Falling back to use ROOT instead")
         if array is None:
-            array = rdf.AsNumpy(columns)
-        df = pd.DataFrame(array)
+            array = rdf.AsNumpy(save_columns)
         self.makedirs(filename)
-        df.to_hdf(filename, key=key)
+        np.save(filename, array)
         return rdf, processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,42 +3,54 @@
 import numpy as np
 
 from .rooproc_output_action import RooProcOutputAction
 from .auxiliary import register_action
 
 from quickstats import module_exist
 from quickstats.utils.common_utils import is_valid_file
-from quickstats.utils.data_conversion import ConversionMode
 from quickstats.interface.root import RDataFrameBackend
 
 @register_action
-class RooProcAsNumpy(RooProcOutputAction):
+class RooProcAsHDF(RooProcOutputAction):
     
-    NAME = "AS_NUMPY"
+    NAME = "AS_HDF"
     
+    def __init__(self, filename:str, key:str,
+                 columns:Optional[List[str]],
+                 exclude:Optional[List[str]]=None):
+        super().__init__(filename=filename,
+                         columns=columns,
+                         key=key)
+
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         filename = params['filename']
+        key = params['key']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
+        import awkward as ak
+        import pandas as pd
         columns = params.get('columns', None)
-        columns = self.get_valid_columns(rdf, processor, columns=columns,
-                                         mode=ConversionMode.REMOVE_NON_STANDARD_TYPE)
+        exclude = params.get('exclude', None)
+        save_columns = self.get_save_columns(rdf, processor, columns=columns,
+                                             exclude=exclude,
+                                             mode="REMOVE_NON_STANDARD_TYPE")
         array = None
         if module_exist('awkward'):
             try:
                 import awkward as ak
                 # NB: RDF Dask/Spark does not support GetColumnType yet
                 if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
                     rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
-                array = ak.from_rdataframe(rdf, columns=columns)
+                array = ak.from_rdataframe(rdf, columns=save_columns)
                 array = ak.to_numpy(array)
             except:
                 array = None
                 processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
                                          "Falling back to use ROOT instead")
         if array is None:
-            array = rdf.AsNumpy(columns)
+            array = rdf.AsNumpy(save_columns)
+        df = pd.DataFrame(array)
         self.makedirs(filename)
-        np.save(filename, array)
+        df.to_hdf(filename, key=key)
         return rdf, processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_export.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from typing import Optional, List
+from typing import Optional, List, Dict
+import os
+import json
 
-import numpy as np
-
-from .rooproc_output_action import RooProcOutputAction
+from .rooproc_helper_action import RooProcHelperAction
 from .auxiliary import register_action
 
 from quickstats.utils.common_utils import is_valid_file
-from quickstats.utils.data_conversion import ConversionMode
-from quickstats.interface.root import RDataFrameBackend
 
 @register_action
-class RooProcAsParquet(RooProcOutputAction):
+class RooProcExport(RooProcHelperAction):
     
-    NAME = "AS_PARQUET"
-
-    def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
+    NAME = "EXPORT"
+    
+    def __init__(self, filename:str):
+        super().__init__(filename=filename)
+        
+    @classmethod
+    def parse(cls, main_text:str, block_text:Optional[str]=None):
+        kwargs = cls.parse_as_kwargs(main_text)
+        return cls(**kwargs)
+    
+    def _execute(self, processor:"quickstats.RooProcessor", **params):
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
-            processor.stdout.info(f'Cached output from "{filename}".')
-            return rdf, processor
-        processor.stdout.info(f'Writing output to "{filename}".')
-        columns = params.get('columns', None)
-        columns = self.get_valid_columns(rdf, processor, columns=columns,
-                                         mode=ConversionMode.REMOVE_NON_STANDARD_TYPE)
-        import awkward as ak
-        try:
-            # NB: RDF Dask/Spark does not support GetColumnType yet
-            if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
-                rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
-            array = ak.from_rdataframe(rdf, columns=columns)
-        except:
-            array = ak.Array(rdf.AsNumpy(columns))
-        self.makedirs(filename)
-        ak.to_parquet(array, filename)
-        return rdf, processor
+            processor.stdout.info(f'Cached output "{filename}".')
+            return processor   
+        data = {k:v.GetValue() for k,v in processor.external_variables.items()}
+        dirname = os.path.dirname(filename)
+        if dirname and (not os.path.exists(dirname)):
+            os.makedirs(dirname)
+        with open(filename, 'w') as outfile:
+            processor.stdout.info(f'Writing auxiliary data to "{filename}".')
+            json.dump(data, outfile, indent=2)
+        return processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional, List, Dict
 import os
 import re
 
 from quickstats.utils.py_utils import get_required_args
 
+LITERAL_REGEX = re.compile(r"\${(\w+)}")
+
 class RooProcBaseAction(object):
     
     NAME = None
     PARAM_FORMATS = {}
 
     def __init__(self, **params):
         self._params = params
@@ -16,44 +18,59 @@
     
     @staticmethod
     def allow_multiline():
         return False
 
     @staticmethod
     def has_global_var(text:str):
-        return re.search(r"\${(\w+)}", text) is not None
+        if not isinstance(text, str):
+            text = str(text)
+        return LITERAL_REGEX.search(text) is not None
+
+    @staticmethod
+    def _get_literals(s:str):
+        return LITERAL_REGEX.findall(s)
     
-    def get_formatted_parameters(self, global_vars:Optional[Dict]=None):
+    def get_formatted_parameters(self, global_vars:Optional[Dict]=None, strict:bool=True):
         if global_vars is None:
             global_vars = {}
         formatted_parameters = {}
         for k,v in self._params.items():
             if v is None:
                 formatted_parameters[k] = None
                 continue
-            k_literals = re.findall(r"\${(\w+)}", k)
+            k_literals = self._get_literals(k)
             is_list = False
             if isinstance(v, list):
                 v = '__SEPARATOR__'.join(v)
                 is_list = True
-            v_literals = re.findall(r"\${(\w+)}", v)
+            elif not isinstance(v, str):
+                formatted_parameters[k] = v
+                continue
+            v_literals = self._get_literals(v)
             all_literals = set(k_literals).union(set(v_literals))
             for literal in all_literals:
-                if literal not in global_vars:
+                if strict and (literal not in global_vars):
                     raise RuntimeError(f"the global variable `{literal}` is undefined")
             for literal in k_literals:
+                if literal not in global_vars:
+                    continue
                 substitute = global_vars[literal]
                 k = k.replace("${" + literal + "}", str(substitute))
             for literal in v_literals:
+                if literal not in global_vars:
+                    continue                
                 substitute = global_vars[literal]
                 v = v.replace("${" + literal + "}", str(substitute))
             if is_list:
                 v = v.split("__SEPARATOR__")
             formatted_parameters[k] = v
         for key, value in formatted_parameters.items():
+            if not isinstance(value, str):
+                continue
             if key in self.PARAM_FORMATS:
                 formatter = self.PARAM_FORMATS[key]
                 formatted_parameters[key] = formatter(value)
         return formatted_parameters
     
     def makedirs(self, filename:str):
         dirname = os.path.dirname(filename)
@@ -96,8 +113,14 @@
     def _try_create(cls, **kwargs):
         try:
             return cls(**kwargs)
         except Exception:
             argnames = get_required_args(cls)
             missing_argnames = list(set(argnames) - set(kwargs))
             raise ValueError(f'missing keyword argument(s) for the action "{cls.NAME}": '
-                             f'{", ".join(missing_argnames)}')
+                             f'{", ".join(missing_argnames)}')
+
+    def get_referenced_columns(self, global_vars:Optional[Dict]=None):
+        return []
+
+    def get_defined_columns(self, global_vars:Optional[Dict]=None):
+        return []
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from typing import Optional
 
 from .rooproc_helper_action import RooProcHelperAction
 from .auxiliary import register_action
 
-from quickstats.utils.root_utils import declare_expression
-
 @register_action
-class RooProcDeclare(RooProcHelperAction):
+class RooProcSaveFrame(RooProcHelperAction):
     
-    NAME = "DECLARE"
+    NAME = "SAVE_FRAME"
     
-    def __init__(self, expression:str, name:Optional[str]=None):
-        super().__init__(expression=expression,
-                         name=name)
-        
-    @staticmethod
-    def allow_multiline():
-        return True
-        
+    def __init__(self, name:str):
+        super().__init__(name=name)
+
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        return cls(expression=main_text)        
+        return cls(name=main_text)
     
     def _execute(self, processor:"quickstats.RooProcessor", **params):
-        name = params.get("name", None)
-        expression = params['expression']
-        declare_expression(expression, name)
+        frame_name = params['name']
+        if frame_name in processor.rdf_frames:
+            processor.stdout.warning(f'Overriding existing rdf frame "{frame_name}"')
+        processor.rdf_frames[frame_name] = processor.rdf
         return processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 from typing import Optional
 import re
 
-from .rooproc_rdf_action import RooProcRDFAction
+from quickstats.utils.common_utils import in_notebook
+from .rooproc_hybrid_action import RooProcHybridAction
 from .auxiliary import register_action
 
 @register_action
-class RooProcDefine(RooProcRDFAction):
+class RooProcProgressBar(RooProcHybridAction):
     
-    NAME = "DEFINE"
-    
-    def __init__(self, name:str, expression:str):
-        super().__init__(name=name, expression=expression)
-        
-    @classmethod
-    def parse(cls, main_text:str, block_text:Optional[str]=None):
-        main_text = re.sub(' +', ' ', main_text)
-        result = re.search(r"^\s*(\w+)\s*=(.*)", main_text)
-        if not result:
-            raise RuntimeError(f"invalid expression {main_text}")
-        name = result.group(1)
-        expression = result.group(2)
-        return cls(name=name, expression=expression)        
+    NAME = "PROGRESSBAR"
         
-    def _execute(self, rdf:"ROOT.RDataFrame", **params):
-        name = params['name']
-        expression = params['expression']
-        rdf_next = rdf.Define(name, expression)
-        return rdf_next
+    def _execute(self, rdf:"ROOT.RDataFrame", processor, **params):
+        import ROOT
+        if not isinstance(rdf, ROOT.RDataFrame):
+            rdf_next = ROOT.RDF.AsRNode(rdf)
+        else:
+            rdf_next = rdf
+        if in_notebook():
+            processor.stdout.warning("ProgressBar does not work properly inside jupyter. Disabling for now.")
+        else:
+            ROOT.RDF.Experimental.AddProgressBar(rdf_next)
+        return rdf_next, processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         super().__init__(expression=expression,
                          name=name)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
         name_literals = re.findall(r"@{([^{}]+)}", main_text)
         if len(name_literals) == 0:
-            name = None
-            expression = main_text.strip()
+            name = main_text.strip()
+            expression = name
         elif len(name_literals) == 1:
             name = name_literals[0]
             expression = main_text.replace("@{" + name + "}", "").strip()
         else:
             raise RuntimeError(f"multiple filter names detected in the expression `{main_text}`")
         return cls(name=name, expression=expression)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing import Optional
 
 import pandas as pd
 
 from .rooproc_hybrid_action import RooProcHybridAction
 from .auxiliary import register_action
+from .formatter import BoolFormatter
 
 from quickstats.utils.common_utils import is_valid_file
 
 @register_action
 class RooProcReport(RooProcHybridAction):
     
     NAME = "REPORT"
+
+    PARAM_FORMATS = {
+        'display': BoolFormatter
+    }    
     
     def __init__(self, display:bool=False, filename:Optional[str]=None):
         super().__init__(display=display,
                          filename=filename)
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
         kwargs = cls.parse_as_kwargs(main_text)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_save.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,42 @@
 from typing import Optional, List
 import fnmatch
 
-from .rooproc_hybrid_action import RooProcHybridAction
+from .rooproc_output_action import RooProcOutputAction
 from .auxiliary import register_action
+from .formatter import ListFormatter
 
 from quickstats.utils.common_utils import is_valid_file, filter_by_wildcards
 
 @register_action
-class RooProcSave(RooProcHybridAction):
+class RooProcSave(RooProcOutputAction):
     
     NAME = "SAVE"
     
     def __init__(self, treename:str, filename:str, 
                  columns:Optional[List[str]]=None,
-                 exclude:Optional[List[str]]=None,
-                 frame:Optional[str]=None):
+                 exclude:Optional[List[str]]=None):
         super().__init__(treename=treename,
                          filename=filename,
                          columns=columns,
-                         exclude=exclude,
-                         frame=frame)
-        
-    @classmethod
-    def parse(cls, main_text:str, block_text:Optional[str]=None):
-        kwargs = cls.parse_as_kwargs(main_text)
-        return cls(**kwargs)
+                         exclude=exclude)
     
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         treename = params['treename']
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'INFO: Cached output from "{filename}".')
             return rdf, processor
-        all_columns = [str(c) for c in rdf.GetColumnNames()]
         columns = params.get('columns', None)
         exclude = params.get('exclude', None)
-        self.makedirs(filename)
-        if isinstance(columns, str):
-            columns = self.parse_as_list(columns)
-        if columns is None:
-            columns = list(all_columns)
-        if exclude is None:
-            exclude = []
-        save_columns = filter_by_wildcards(all_columns, columns)
-        save_columns = filter_by_wildcards(save_columns, exclude, exclusion=True)
-        save_columns = list(set(save_columns))
+        save_columns = self.get_save_columns(rdf, processor,
+                                             columns=columns,
+                                             exclude=exclude,
+                                             mode="ALL")
         processor.stdout.info(f'Writing output to "{filename}".')
+        self.makedirs(filename)
         if processor.use_template:
             from quickstats.utils.root_utils import templated_rdf_snapshot 
             rdf_next = templated_rdf_snapshot(rdf, save_columns)(treename, filename, save_columns)
         else:
             rdf_next = rdf.Snapshot(treename, filename, save_columns)
         return rdf_next, processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from typing import Optional
 
 from .rooproc_helper_action import RooProcHelperAction
 from .auxiliary import register_action
 
 @register_action
-class RooProcSaveFrame(RooProcHelperAction):
+class RooProcTreeName(RooProcHelperAction):
     
-    NAME = "SAVE_FRAME"
+    NAME = "TREENAME"
     
-    def __init__(self, name:str):
-        super().__init__(name=name)
-
+    def __init__(self, treename:str):
+        super().__init__(treename=treename)
+        
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        return cls(name=main_text)
+        return cls(treename=main_text)
     
     def _execute(self, processor:"quickstats.RooProcessor", **params):
-        frame_name = params['name']
-        if frame_name in processor.rdf_frames:
-            processor.stdout.warning(f'Overriding existing rdf frame "{frame_name}"')
-        processor.rdf_frames[frame_name] = processor.rdf
+        treename = params['treename']
+        processor.treename = treename
         return processor
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Dict
 import re
 
 from .rooproc_hybrid_action import RooProcHybridAction
 
 class RooProcStat(RooProcHybridAction):
     def __init__(self, ext_var_name:str, column_name:str):
         super().__init__(ext_var_name=ext_var_name,
@@ -20,8 +20,13 @@
     def _get_func(self, rdf:"ROOT.RDataFrame"):
         raise NotImplementedError
         
     def _execute(self, rdf:"ROOT.RDataFrame", processor:"quickstats.RooProcessor", **params):
         ext_var_name = params['ext_var_name']
         column_name = params['column_name']
         processor.external_variables[ext_var_name] = self._get_func(rdf)(column_name)
-        return rdf, processor
+        return rdf, processor
+
+    def get_referenced_columns(self, global_vars:Optional[Dict]=None):
+        params = self.get_formatted_parameters(global_vars, strict=False)
+        referenced_columns = [params['column_name']]
+        return referenced_columns
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.2.2/quickstats/components/processors/roo_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,21 +5,35 @@
 import time
 import ROOT
 
 from .builtin_methods import BUILTIN_METHODS
 from .actions import *
 from .roo_process_config import RooProcessConfig
 
-from quickstats import timer, AbstractObject, PathManager
+from quickstats import timer, AbstractObject, PathManager, GeneralEnum
 from quickstats.interface.root import TFile, RDataFrame, RDataFrameBackend
 from quickstats.interface.xrootd import get_cachedir, set_cachedir, switch_cachedir
-from quickstats.utils.root_utils import declare_expression, close_all_root_files
+from quickstats.utils.root_utils import declare_expression, close_all_root_files, set_multithread
 from quickstats.utils.path_utils import is_remote_path
 from quickstats.utils.common_utils import get_cpu_count
 
+class RDFVerbosity(GeneralEnum):
+    UNSET   = (0, 'kUnset')
+    FATAL   = (1, 'kFatal')
+    ERROR   = (2, 'kError')
+    WARNING = (3, 'kWarning')
+    INFO    = (4, 'kInfo')
+    DEBUG   = (5, 'kDebug')
+
+    def __new__(cls, value:int, key:str):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.key = key
+        return obj
+
 class RooProcessor(AbstractObject):
 
     @property
     def distributed(self):
         return self.backend != RDataFrameBackend.DEFAULT
         
     def __init__(self, config_source:Optional[Union[RooProcessConfig, str]]=None,
@@ -40,52 +54,60 @@
             self.flags = []
         self.rdf_frames = {}
         self.rdf = None
         self.global_variables = {}
         self.external_variables = {}
         self.default_treename = None
         self.use_template = use_template
-        self.multithread = multithread
+        self.rdf_verbosity = None
+        self.result_metadata = None
         if backend is None:
             self.backend = RDataFrameBackend.DEFAULT
         else:
             self.backend = RDataFrameBackend.parse(backend)
         self.backend_options = backend_options
         self.set_remote_file_options(localize=False,
                                      cachedir=get_cachedir())
-        
+        self.set_profile_options()
         self.load_buildin_functions()
-        
-        if multithread:            
-            if multithread > 1:
-                ROOT.EnableImplicitMT(multithread)
-                num_thread = multithread
-            else:
-                ROOT.EnableImplicitMT()
-                num_thread = get_cpu_count()
-            self.stdout.info(f'Enabled multithreading with {num_thread} threads.')
-        elif ROOT.IsImplicitMTEnabled():
-            ROOT.DisableImplicitMT()
+
+        self.set_multithread(multithread)
         
         if config_source is not None:
             self.load_config(config_source)
+
+    def set_multithread(self, num_threads:Optional[int]=None):
+        if num_threads is None:
+            num_threads = self.multithread
+        num_threads = set_multithread(num_threads)
+        if num_threads is None:
+            self.stdout.info("Disabled multithreading.")
+        else:
+            self.stdout.info(f"Enabled multithreading with {num_threads} threads.")
+        self.multithread = num_threads
             
     def set_cache(self, cache:bool=True):
         self.cache = cache
         
     def set_remote_file_options(self, localize:bool=False,
                                 cache:bool=True, cachedir:Optional[str]="/tmp",
                                 copy_options:Optional[Dict]=None):
         remote_file_options = {
             'localize': localize,
             'cache': cache,
             'cachedir': cachedir,
             'copy_options': copy_options
         }
         self.remote_file_options = remote_file_options
+
+    def set_profile_options(self, throughput:bool=False):
+        profile_options = {
+            "throughput": throughput
+        }
+        self.profile_options = profile_options
             
     def load_buildin_functions(self):
         # bug of redefining module from ROOT
         try:
             import ROOT
             Internal = ROOT.Internal
         except:
@@ -152,15 +174,17 @@
         return RooProcReturnCode.NORMAL
             
     def run_all_actions(self, consider_child:bool=True):
         if not self.action_tree:
             raise RuntimeError("action tree not initialized")
         node = self.action_tree.get_next(consider_child=consider_child)
         if node is not None:
-            self.stdout.debug(f'Executing node "{node.name}" defined at line {node.data["start_line_number"]}')
+            source = node.try_get_data("source", None)
+            self.stdout.debug(f'Executing node "{node.name}" defined at line {node.data["start_line_number"]}'
+                             f' (source {source})')
             action = node.action
             return_code = self.run_action(action)
             if return_code == RooProcReturnCode.NORMAL:
                 self.run_all_actions()
             elif return_code == RooProcReturnCode.SKIP_CHILD:
                 self.run_all_actions(consider_child=False)
             else:
@@ -182,45 +206,50 @@
     def list_files(self, filenames:List[str], resolve_cache:bool=True):
         cachedir = self.remote_file_options['cachedir']
         with switch_cachedir(cachedir):
             files = TFile.list_files(filenames, resolve_cache=resolve_cache,
                                      raise_on_error=False)
         return files
 
-    def _fetch_remote_files(self, filenames:List[str]):
+    def resolve_filenames(self, filenames:Union[List[str], str]):
+        filenames = self.list_files(filenames, resolve_cache=True)
+        if not filenames:
+            return []
+        has_remote_file = self._has_remote_files(filenames)
+        # copy remote files to local storage
+        if has_remote_file and self.remote_file_options['localize']:
+            remote_files = [filename for filename in filenames if is_remote_path(filename)]
+            self._copy_remote_files(remote_files)
+            filenames = self.list_files(filenames, resolve_cache=True)
+        return filenames
+
+    def _copy_remote_files(self, filenames:List[str]):
         opts = self.remote_file_options
         copy_options = opts.get('copy_options', None)
         if copy_options is None:
             copy_options = {}
-        TFile.fetch_remote_files(filenames, cache=opts['cache'],
+        TFile.copy_remote_files(filenames, cache=opts['cache'],
                                  cachedir=opts['cachedir'],
                                  **copy_options)
         
-    def load_rdataframe(self,
-                        filenames:Union[List[str], str],
-                        treename:Optional[str]=None):
-        
-        if treename is None:
-            treename = self.default_treename
+    def load_rdf(self,
+                 filenames:Union[List[str], str],
+                 treename:Optional[str]=None):
             
-        if treename is None:
-            raise RuntimeError("treename is undefined")
-            
-        filenames = self.list_files(filenames, resolve_cache=True)
-        
+        filenames = self.resolve_filenames(filenames)
         if not filenames:
-            self.stdout.info('No files to be processed. Skipped.')
+            self.stdout.info('No files to be processed. Skipping.')
             return None
-            
-        has_remote_file = self._has_remote_files(filenames)
-        # copy remote files to local storage
-        if has_remote_file and self.remote_file_options['localize']:
-            remote_files = [filename for filename in filenames if is_remote_path(filename)]
-            self._fetch_remote_files(remote_files)
-            filenames = self.list_files(filenames, resolve_cache=True)
+        self._filenames = filenames
+
+        if treename is None:
+            treename = self.default_treename
+        if treename is None:
+            treename = TFile._get_main_treename(filenames[0])
+            self.stdout.info(f"Using deduced treename: {treename}")
 
         if len(filenames) == 1:
             self.stdout.info(f'Processing file "{filenames[0]}".')
         else:
             self.stdout.info("Professing files")
             for filename in filenames:
                 self.stdout.info(f'  "{filename}"', bare=True)
@@ -232,23 +261,62 @@
         self.rdf = rdf
         return self
     
     def run(self, filenames:Optional[Union[List[str], str]]=None):
         self.sanity_check()
         with timer() as t:
             if filenames is not None:
-                self.load_rdataframe(filenames)
+                self.load_rdf(filenames)
             self.action_tree.reset()
             self.run_all_actions()
             self.shallow_cleanup()
         self.stdout.info(f"Task finished. Total time taken: {t.interval:.3f} s.")
+        result_metadata = {
+            "files": list(self._filenames),
+            "real_time": t.real_time_elapsed,
+            "cpu_time": t.cpu_time_elapsed
+        }
+        self.result_metadata = result_metadata
         return self
+
+    def get_rdf(self, frame:Optional[str]=None):
+        rdf = self.rdf if frame is None else self.rdf_frames.get(frame, None)
+        if rdf is None:
+            raise RuntimeError('RDataFrame instance not initialized')
+        return rdf
+
+    def get_referenced_columns(self):
+        action_tree = self.action_tree
+        return action_tree.get_referenced_columns(self.global_variables)
         
     def awkward_array(self, frame:Optional[str]=None,
-                       columns:Optional[List[str]]=None):
-        if frame is None:
-            rdf = self.rdf
+                      columns:Optional[List[str]]=None):
+        rdf = self.get_rdf(frame)
+        return RDataFrame._awkward_array(rdf, columns=columns)
+
+    def display(self, frame:Optional[str]=None,
+                columns:Union[str, List[str]]="",
+                n_rows:int=5, n_max_collection_elements:int=10,
+                lazy:bool=False):
+        rdf = self.get_rdf(frame)
+        result = self.rdf.Display(columns, n_rows, n_max_collection_elements)
+        if not lazy:
+            result.Print()
+            return None
+        return result
+
+    def save_graph(self, frame:Optional[str]=None,
+                   filename:Optional[str]=None):
+        rdf = self.get_rdf(frame)
+        if filename:
+            ROOT.RDF.SaveGraph(rdf, filename)
         else:
-            rdf = self.rdf_frames.get(frame, None)
-        if rdf is None:
-            raise RuntimeError('RDataFrame instance not initialized')
-        return RDataFrame._awkward_array(rdf, columns=columns)
+            ROOT.RDF.SaveGraph(rdf)
+
+    def set_rdf_verbosity(self, verbosity:str='INFO'):
+        if isinstance(verbosity, str):
+            verbosity = RDFVerbosity.parse(verbosity)
+            loglevel = getattr(ROOT.Experimental.ELogLevel, verbosity.key)
+        else:
+            loglevel = verbosity
+        verb = ROOT.Experimental.RLogScopedVerbosity(ROOT.Detail.RDF.RDFLogChannel(), loglevel)
+        self.rdf_verbosity = verb
```

### Comparing `quickstats-0.7.0.2.1/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.2.2/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.2.2/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/root_object.py` & `quickstats-0.7.0.2.2/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.2.2/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.2.2/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/logging.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from typing import Optional, Union, Dict, List, Any
 from itertools import repeat
 
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
-from quickstats.utils.common_utils import batch_makedirs, json_load, combine_dict, save_as_json
+from quickstats.utils.common_utils import batch_makedirs, json_load, combine_dict, save_json
 from quickstats.components import AsymptoticCLs
 
 class ParameterisedAsymptoticCLs(ParameterisedRunner):
     def __init__(self, input_path:str, config:Optional[Dict]=None,
                  file_expr:Optional[str]=None, param_expr:Optional[str]=None,
                  filter_expr:Optional[str]=None, exclude_expr:Optional[str]=None,
                  outdir:str="output", cachedir:str="cache", outname:str="limits.json",
@@ -113,8 +113,8 @@
 
         poi_name   = self.attributes['config'].get('poi_name', None)
         outdir     = self.attributes['outdir']
         outname    = self.attributes['outname'].format(poi_name=poi_name)
         
         if outname is not None:
             outpath = os.path.join(outdir, outname)
-            save_as_json(final_result, outpath)
+            save_json(final_result, outpath)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional, Union, Dict, List, Any
 from itertools import repeat
 
 import ROOT
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
-from quickstats.utils.common_utils import batch_makedirs, save_as_json
+from quickstats.utils.common_utils import batch_makedirs, save_json
 from quickstats.components import Likelihood
 
 class ParameterisedLikelihood(ParameterisedRunner):
     
     def __init__(self, input_path:str, param_expr:str, file_expr:Optional[str]=None,
                  filter_expr:Optional[str]=None, exclude_expr:Optional[str]=None,
                  data_name:str="combData", uncond_snapshot:Optional[str]=None,
@@ -231,8 +231,8 @@
         # backward compatibility
         if len(poi_names) == 1:
             poi_name = poi_names[0]
             data['mu'] = [v for v in data[poi_name]]
         outdir  = self.attributes['outdir']
         outname = self.attributes['outname'].format(poi_names="_".join(poi_names))
         outpath = os.path.join(outdir, outname.format(poi_name=poi_name))
-        save_as_json(data, outpath)
+        save_json(data, outpath)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.2.2/quickstats/concurrent/parameterised_significance.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import json
 from typing import Optional, Union, Dict, List, Any
 
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
-from quickstats.utils.common_utils import batch_makedirs, list_of_dict_to_dict_of_list, save_as_json, combine_dict
+from quickstats.utils.common_utils import batch_makedirs, list_of_dict_to_dict_of_list, save_json, combine_dict
 from quickstats.maths.numerics import pretty_value
 from quickstats.components import AnalysisBase, AsimovType, AsimovGenerator
 
 class ParameterisedSignificance(ParameterisedRunner):
     
     def __init__(self, input_path:str,
                  file_expr:Optional[str]=None,
@@ -80,17 +80,17 @@
             analysis = AnalysisBase(**config)
             if asimov_type is not None:
                 asimov_type = AsimovType.parse(asimov_type)
                 asimov_data = analysis.generate_standard_asimov(asimov_type, do_import=False)
                 asimov_snapshot = AsimovGenerator.ASIMOV_SETTINGS[asimov_type]['asimov_snapshot']
                 analysis.set_data(asimov_data)
                 result = analysis.nll_fit(poi_val=mu_exp, mode='hybrid',
-                                          snapshot_name=asimov_snapshot)
+                                          snapshot_name=asimov_snapshot, do_minos=config['minos'] if "minos" in config else False)
             else:
-                result = analysis.nll_fit(poi_val=mu_exp, mode='hybrid')
+                result = analysis.nll_fit(poi_val=mu_exp, mode='hybrid', do_minos=config['minos'] if "minos" in config else False)
             if outname:
                 with open(outname, 'w') as outfile:
                     json.dump(result, outfile, indent=2)
             return result
         except Exception as e:
             sys.stdout.write(f"{e}\n")
             return None
@@ -160,8 +160,8 @@
             data['pvalue'].append(result['pvalue'])
             data['status_muexp'].append(result['cond_fit']['status'])
             data['status_muhat'].append(result['uncond_fit']['status'])
             data['status'].append(result['status'])
         outdir  = self.attributes['outdir']
         outname = self.attributes['outname'].format(param_names="_".join(param_names))
         outpath = os.path.join(outdir, outname)
-        save_as_json(data, outpath)
+        save_json(data, outpath)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/core/abstract_object.py` & `quickstats-0.7.0.2.2/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/configurations.py` & `quickstats-0.7.0.2.2/quickstats/core/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .abstract_object import AbstractObject
 from .decorators import semistaticmethod
 from .metaclasses import MergeAnnotationsMeta
 from .type_validation import get_type_validator, get_type_hint_str
 from quickstats.utils.string_utils import format_dict_to_string
 
 
-__all__ = ['as_dict', 'ConfigComponent', 'ConfigScheme', 'ConfigFile', 'ConfigurableObject', 'ConfigUnit']
+__all__ = ['ConfigComponent', 'ConfigScheme', 'ConfigFile', 'ConfigurableObject', 'ConfigUnit']
 
 
 class MISSING_TYPE:
     pass
 
 MISSING = MISSING_TYPE()
```

### Comparing `quickstats-0.7.0.2.1/quickstats/core/constraints.py` & `quickstats-0.7.0.2.2/quickstats/core/constraints.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/decorators.py` & `quickstats-0.7.0.2.2/quickstats/core/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List
 from functools import partial
 import time
 import importlib
 
+__all__ = ["semistaticmethod", "cls_method_timer", "timer"]
+
 class semistaticmethod(object):
     """
     Descriptor to allow a staticmethod inside a class to use 'self' when called from an instance.
 
     This custom descriptor class `semistaticmethod` enables a static method defined inside a class 
     to access the instance (`self`) when called from an instance, similar to how regular instance 
     methods can access the instance attributes. By default, static methods do not have access to 
@@ -106,22 +108,26 @@
     def __enter__(self):
         """
         Records the start time when entering the context.
 
         Returns:
             timer: The timer instance itself.
         """
-        self.start = time.time()
+        self.start_real = time.time()
+        self.start_cpu = time.process_time()
         return self
 
     def __exit__(self, *args):
         """
         Calculates the time interval when exiting the context.
 
         Args:
             *args: Variable-length argument list.
 
         Returns:
             None
         """
-        self.end = time.time()
-        self.interval = self.end - self.start
+        self.end_cpu = time.process_time()
+        self.end_real = time.time()
+        self.interval = self.end_real - self.start_real
+        self.real_time_elapsed = self.interval
+        self.cpu_time_elapsed = self.end_cpu - self.start_cpu
```

### Comparing `quickstats-0.7.0.2.1/quickstats/core/enums.py` & `quickstats-0.7.0.2.2/quickstats/core/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Optional, Union, List, Dict
 from enum import Enum
 
+__all__ = ["GeneralEnum", "DescriptiveEnum"]
+
 class GeneralEnum(Enum):
     """
     Extended Enum class with additional parsing and lookup functionalities.
 
     Args:
         expr (Optional[Union[int, str, GeneralEnum]], optional): The expression to parse into an enum member. 
                         This can be an integer, a string representing the enum member name (case-insensitive),
```

### Comparing `quickstats-0.7.0.2.1/quickstats/core/io.py` & `quickstats-0.7.0.2.2/quickstats/core/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/metaclasses.py` & `quickstats-0.7.0.2.2/quickstats/core/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/methods.py` & `quickstats-0.7.0.2.2/quickstats/core/methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional, Dict
+from typing import List, Union, Optional, Dict, Callable
 import os
 import glob
 import json
 import shutil
 import importlib
 
 import quickstats
@@ -69,14 +69,17 @@
     try:
         root_config_cmd = ROOTChecker.get_root_config_cmd()
         root_version = ROOTChecker.get_installed_root_version(root_config_cmd)
     except Exception:
         root_version = ROOTVersion((0, 0, 0))
     return root_version
 
+def is_root_installed(name:str=None):
+    return get_root_version() > (0, 0, 0)
+
 def get_workspace_extensions():
     extension_config = get_workspace_extension_config()
     extensions = extension_config['required']
     if not extension_config['strict']:
         # deprecated extension
         if (quickstats.root_version >= (6, 26, 0)) and 'FlexibleInterpVarMkII' in extensions:
             extensions.remove('FlexibleInterpVarMkII')
@@ -158,9 +161,15 @@
         
 def load_processor_methods():
     from quickstats.components.processors.builtin_methods import BUILTIN_METHODS
     from quickstats.utils.root_utils import declare_expression
     for name, definition in BUILTIN_METHODS.items():
         declare_expression(definition, name)
         
-def module_exist(name:str):
-    return importlib.util.find_spec(name) is not None
+def module_exist(name: str) -> bool:
+    return importlib.util.find_spec(name) is not None
+
+def _require_module(name: str, fn:Optional[Callable]=None):
+    if fn is None:
+        fn = module_exist
+    if not fn(name):
+        raise ImportError(f"The module '{name}' is required but not found. Please install it to proceed.")
```

### Comparing `quickstats-0.7.0.2.1/quickstats/core/path_manager.py` & `quickstats-0.7.0.2.2/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/setup.py` & `quickstats-0.7.0.2.2/quickstats/core/setup.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/type_validation.py` & `quickstats-0.7.0.2.2/quickstats/core/type_validation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.2.2/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.2.2/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.2.2/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.2.2/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.2.2/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RDataFrame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TFile.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TFile.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import re
 import glob
 
 import numpy as np
 
 from quickstats import semistaticmethod
 from quickstats.utils.path_utils import (resolve_paths, is_remote_path, remote_glob,
-                                         remote_isdir, remote_dirlist, dirlist,
-                                         local_file_exist, split_url)
+                                         remote_isdir, remote_listdir, listdir,
+                                         local_file_exist, split_url,
+                                         remote_file_exist)
 from quickstats.utils.root_utils import is_corrupt
 from quickstats.utils.common_utils import in_notebook
-from quickstats.interface.xrootd import get_cachedir
+from quickstats.utils.sys_utils import bytes_to_readable
 from .TObject import TObject
 
 class TFile(TObject):
 
     FILE_PATTERN = re.compile(r"^.+\.root(?:\.\d+)?$")
 
     def __init__(self, source:Union[str, "ROOT.TFile"],
@@ -26,14 +27,47 @@
         self.obj = self._open(source)
         
     @staticmethod
     def is_corrupt(f:Union["ROOT.TFile", str]):
         return is_corrupt(f)
 
     @semistaticmethod
+    def _get_all_treenames(self, source:Union["ROOT.TFile", str]):
+        import ROOT
+        if isinstance(source, str):
+            source = ROOT.TFile.Open(source)
+        keys = [key.GetName() for key in source.GetListOfKeys()]
+        objs = [source.Get(key) for key in keys]
+        trees = [obj for obj in objs if isinstance(obj, ROOT.TTree)]
+        treenames = [tree.GetName() for tree in trees]
+        return treenames
+
+    @semistaticmethod
+    def _get_main_treename(self, source:Union["ROOT.TFile", str]):
+        import ROOT
+        if isinstance(source, str):
+            source = ROOT.TFile.Open(source)
+        keys = [key.GetName() for key in source.GetListOfKeys()]
+        objs = [source.Get(key) for key in keys]
+        trees = [obj for obj in objs if isinstance(obj, ROOT.TTree)]
+        if not trees:
+            raise RuntimeError('no tree found in the root file')
+        elif len(trees) == 1:
+            return trees[0].GetName()
+        main_trees = [tree for tree in trees if tree.GetEntriesFast() > 1]
+        main_treenames = [tree.GetName() for tree in main_trees]
+        if not main_trees:
+            raise RuntimeError('no tree found with entries > 1')
+        elif len(main_trees) > 1:
+            raise RuntimeError('found multiple trees with entries > 1 : {names}'.format(
+                names=", ".join(main_treenames)))
+        return main_treenames[0]
+                               
+
+    @semistaticmethod
     def _is_valid_filename(self, filename:str):
         return self.FILE_PATTERN.match(filename) is not None
     
     @semistaticmethod
     def _requires_protocol(self, filename:str):
         return "://" in filename
 
@@ -50,29 +84,30 @@
         return cache_path
     
     @semistaticmethod
     def _resolve_cached_remote_paths(self, paths:List[str],
                                      strict_format:Optional[bool]=True,
                                      cached_only:bool=False):
         import ROOT
+        from quickstats.interface.xrootd import get_cachedir
         cachedir = get_cachedir()
         if cachedir is None:
             return list(paths)
         resolved_paths = []
         for path in paths:
             url = ROOT.TUrl(path)
             # skip local file
             if url.GetProtocol() == "file":
                 resolved_paths.append(path)
                 continue
             filename = url.GetFile().lstrip("/")
             cache_path = os.path.join(cachedir, filename)
             if os.path.exists(cache_path):
                 if os.path.isdir(cache_path):
-                    cache_paths = dirlist(cache_path)
+                    cache_paths = listdir(cache_path)
                     if strict_format:
                         cache_paths = self._filter_valid_filenames(cache_paths)
                     if not cache_paths:
                         if not cached_only:
                             resolved_paths.append(path)
                         continue
                     resolved_paths.extend(cache_paths)
@@ -84,45 +119,47 @@
                 
     @semistaticmethod
     def list_files(self, paths:Union[List[str], str],
                    strict_format:Optional[bool]=True,
                    resolve_cache:bool=False,
                    expand_remote_files:bool=True,
                    raise_on_error:bool=True):
-        remote_flag = True
         paths = resolve_paths(paths)
         filenames = []
+
+        if resolve_cache:
+            paths = self._resolve_cached_remote_paths(paths)
         
         # expand directories if necessary
         for path in paths:
             if is_remote_path(path):
                 if local_file_exist(path):
                     host, path = split_url(path)
-                else:
-                    if remote_flag:
-                        self.stdout.info("Resolving remote files. Network traffic overhead might be expected.")
-                        remote_flag = False
+                elif remote_file_exist(path):
                     if expand_remote_files and remote_isdir(path):
-                        filenames.extend(remote_dirlist(path))
+                        filenames.extend(remote_listdir(path))
                     else:
                         filenames.append(path)
                     continue
+                else:
+                    self.stdout.warning(f'Remote file "{path}" does not exist')
             if os.path.isdir(path):
-                filenames.extend(dirlist(path))
-            else:
+                filenames.extend(listdir(path))
+            elif os.path.exists(path):
                 filenames.append(path)
+            else:
+                self.stdout.warning(f'Local file "{path}" does not exist')
         if strict_format:
             filenames = self._filter_valid_filenames(filenames)
         if not filenames:
             return []
         if resolve_cache:
             filenames = self._resolve_cached_remote_paths(filenames)
         import ROOT
-        invalid_filenames = []
-        valid_filenames = []
+        invalid_filenames, valid_filenames = [], []
         for filename in filenames:
             if is_remote_path(filename):
                 # delay the check of remote root file to when they are open
                 valid_filenames.append(filename)
                 continue
             try:
                 rfile = ROOT.TFile(filename)
@@ -134,16 +171,14 @@
                 invalid_filenames.append(filename)
         if invalid_filenames:
             fmt_str = "\n".join(invalid_filenames)
             if raise_on_error:
                 raise RuntimeError(f'Found empty/currupted file(s):\n{fmt_str}')
             else:
                 self.stdout.warning(f'Found empty/currupted file(s):\n{fmt_str}')
-        if not remote_flag:
-            self.stdout.info("Finished resolving remote files.")
         return valid_filenames
     
     @staticmethod
     def _open(source:Union[str, "ROOT.TFile"]):
         # source is path to a root file
         if isinstance(source, str):
             import ROOT
@@ -179,42 +214,80 @@
         tree = self.obj.Get(name)
         if not tree:
             if strict:
                 raise RuntimeError(f'In TFile.Get: Tree "{name}" does not exist')
             return None
         return tree
 
+    def get_tree_compression_summary(self, treename:Optional[str]=None):
+        file = self.obj
+        if treename is None:
+            treename = self._deduce_treename(file)
+        tree = file.Get(treename)
+        total_bytes = tree.GetTotBytes()
+        zip_bytes = tree.GetZipBytes()
+        summary = {
+            'total_bytes': total_bytes,
+            'total_bytes_s': bytes_to_readable(total_bytes),
+            'zip_bytes': zip_bytes,
+            'zip_bytes_s': bytes_to_readable(zip_bytes),
+            'comp_factor': total_bytes / zip_bytes
+        }
+        return summary
+
+    def get_compression_summary(self, treenames:Optional[List[str]]=None):
+        file = self.obj
+        comp_setting = file.GetCompressionSettings()
+        summary = {}
+        summary["comp_setting"] = comp_setting
+        summary["trees"] = {}
+        if treenames is None:
+            treenames = self._get_all_treenames(file)
+        for treename in treenames:
+            summary["trees"][treename] = self.get_tree_compression_summary(treename)
+        return summary
+        
     @semistaticmethod
-    def fetch_remote_files(self, paths:Union[str, List[str]],
+    def copy_remote_files(self, paths:Union[str, List[str]],
                           cache:bool=True,
                           cachedir:str="/tmp",
+                          parallel:bool=False,
                           **kwargs):
         if isinstance(paths, str):
             paths = [paths]
         remote_paths = []
         for path in paths:
             if not is_remote_path(path):
                 self.stdout.warning(f"Not a remote file: {path}. Skipped.")
                 continue
             if local_file_exist(path):
                 self.stdout.warning(f"Remote file {path} can be accessed locally. Skipped.")
                 continue
             remote_paths.append(path)
-        filenames = self.list_files(remote_paths, resolve_cache=cache,
-                                    expand_remote_files=True)
+        from quickstats.interface.xrootd import switch_cachedir
+        with switch_cachedir(cachedir):
+            filenames = self.list_files(remote_paths, resolve_cache=cache,
+                                        expand_remote_files=True)
         cached_files = [filename for filename in filenames if not is_remote_path(filename)]
         files_to_fetch = [filename for filename in filenames if is_remote_path(filename)]
         if cached_files:
             self.stdout.info(f'Cached remote file(s):\n' + '\n'.join(cached_files))
-        from quickstats.interface.xrootd.utils import copy_files
         src, dst = [], []
         for file in files_to_fetch:
             src.append(file)
-            dst.append(self._get_cache_path(file))
-        if src:
-            self.stdout.info(f'Fetching remote file(s):\n' + '\n'.join(src))
-            self.stdout.info(f'Destination(s):\n' + '\n'.join(dst))
-        copy_files(src, dst, force=not cache, **kwargs)
+            dst.append(self._get_cache_path(file, cachedir=cachedir))
+        if not src:
+            return None
+        from quickstats.interface.xrootd import XRDHelper
+        helper = XRDHelper(verbosity=self.stdout.verbosity)
+        if parallel:
+            helper.copy_files(src, dst, force=not cache, **kwargs)
+            return None
+        for src_i, dst_i in zip(src, dst):
+            helper.copy_files([src_i], [dst_i], force=not cache, **kwargs)
+
+    def get(self, key:str):
+        return self.obj.Get(key)
 
     def close(self):
         self.obj.Close()
         self.obj = None
```

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/TH3.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/helper.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/macros.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.2.2/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.2.2/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.2.2/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.2.2/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.2.2/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.2.2/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.2.2/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/maths/interpolation.py` & `quickstats-0.7.0.2.2/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/maths/numerics.py` & `quickstats-0.7.0.2.2/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/maths/statistics.py` & `quickstats-0.7.0.2.2/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.2.2/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/maths/symbolics.py` & `quickstats-0.7.0.2.2/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.2.2/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.2.2/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/__init__.py` & `quickstats-0.7.0.2.2/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/abstract_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import matplotlib
 
 from quickstats import AbstractObject, semistaticmethod
 from quickstats.plots import get_color_cycle, get_cmap
 from quickstats.plots.color_schemes import QUICKSTATS_PALETTES
 from quickstats.plots.template import (single_frame, parse_styles, format_axis_ticks,
                                        parse_analysis_label_options, centralize_axis,
-                                       create_transform, draw_multiline_text)
+                                       create_transform, draw_multiline_text,
+                                       CUSTOM_HANDLER_MAP)
 from quickstats.utils.common_utils import combine_dict, insert_periodic_substr
 from quickstats.maths.statistics import bin_center_to_bin_edge, get_hist_comparison_data
 from quickstats.maths.statistics import HistComparisonMode
 from .core import PlotFormat, ErrorDisplayFormat
 
 class AbstractPlot(AbstractObject):
     
@@ -317,39 +318,55 @@
             if mode == HistComparisonMode.RATIO:
                 ylabel = "Ratio"
             elif mode == HistComparisonMode.DIFFERENCE:
                 ylabel = "Difference"
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         
     def draw_binned_data(self, ax, data,
+                         remove_zero_entries:bool=False,
                          draw_data:bool=True,
                          draw_error:bool=True,
                          bin_edges:Optional[np.ndarray]=None,
                          plot_format:Union[PlotFormat, str]='errorbar',
                          error_format:Union[ErrorDisplayFormat, str]='errorbar',
                          styles:Optional[Dict]=None,
                          error_styles:Optional[Dict]=None):
         if styles is None:
             styles = {}
         if error_styles is None:
             error_styles = {}
-        plot_format = PlotFormat.parse(plot_format)
+        plot_format  = PlotFormat.parse(plot_format)
         error_format = ErrorDisplayFormat.parse(error_format)
         handle, error_handle = None, None
         
         x, y = data['x'], data['y']
         xerr, yerr = data.get('xerr', 0), data.get('yerr', 0)
+        if remove_zero_entries:
+            mask = y > 0
+            x, y = x[mask], y[mask]
+            if isinstance(xerr, tuple):
+                if isinstance(xerr[0], Sequence):
+                    xerr = (np.array(xerr[0])[mask],
+                            np.array(xerr[1])[mask])
+            elif isinstance(xerr, Sequence):
+                xerr = np.array(xerr)[mask]
+            if isinstance(yerr, tuple):
+                if isinstance(yerr[0], Sequence):
+                    yerr = (np.array(yerr[0])[mask],
+                            np.array(yerr[1])[mask])
+            elif isinstance(yerr, Sequence):
+                yerr = np.array(yerr)[mask]
         
         if draw_data:
             styles = combine_dict(self.styles['errorbar'], styles)
             if plot_format == PlotFormat.ERRORBAR:
                 if (not draw_error) or (error_format != ErrorDisplayFormat.ERRORBAR):
                     handle = ax.errorbar(x, y, **styles)
                 else:
-                    handle = ax.errorbar(**data, **styles)
+                    handle = ax.errorbar(x, y, xerr=xerr, yerr=yerr, **styles)
             else:
                 raise RuntimeError(f'unsupported plot format: {plot_format.name}')
                 
         if draw_error:
             if error_format == ErrorDisplayFormat.FILL:
                 if isinstance(yerr, tuple):
                     error_handle = ax.fill_between(x, y - yerr[0], y + yerr[1],
@@ -368,8 +385,20 @@
                 else:
                     error_handle = ax.bar(x=x, height=2*yerr,
                                           bottom=y - yerr, width=bin_widths,
                                           **error_styles, zorder=-1)
             elif error_format == ErrorDisplayFormat.ERRORBAR:
                 error_handle = ax.errorbar(**data, **error_styles)
         handles = tuple([h for h in [handle, error_handle] if h is not None])
-        return handles
+        return handles
+
+    def draw_legend(self, ax, handles=None, labels=None,
+                    handler_map=None, **kwargs):
+        if (handles is None) and (labels is None):
+            handles, labels = self.get_legend_handles_labels()
+        if handler_map is not None:
+            handler_map = {**CUSTOM_HANDLER_MAP, **handler_map}
+        else:
+            handler_map = CUSTOM_HANDLER_MAP
+        styles = {**self.styles['legend'], **kwargs}
+        styles['handler_map'] = handler_map
+        ax.legend(handles, labels, **styles)
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.2.2/quickstats/plots/bidirectional_bar_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                               if 'color' not in k and 'fill' not in k}
             primary_styles['color'] = 'k'
             secondary_styles = {k:v for k,v in self.config['secondary_up'].items() \
                               if 'color' not in k and 'fill' not in k}
             secondary_styles['color'] = 'k'
             target_handles = [lines.Line2D([0], [0], **primary_styles),
                               lines.Line2D([0], [0], **secondary_styles)]
-            ax.legend(target_handles, target_labels, **self.styles['legend'])
+            self.draw_legend(ax, handles=target_handles, labels=target_labels)
             ax.add_artist(legend_updown)
         """
         # legend for targets
         handles2 = [lines.Line2D([0], [0], color='k', lw=2.5),
                     patches.Patch(facecolor='k', edgecolor='none', alpha=0.5)]
         labels2  = analysisTitle
         # draw second legend
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.2.2/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/core.py` & `quickstats-0.7.0.2.2/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/general_1D_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,13 @@
                             handles[handle_name] = stat_handle
             legend_order.extend(handles.keys())
             self.update_legend_handles(handles)
         else:
             raise ValueError("invalid data format")
             
         self.legend_order = legend_order
-        handles, labels = self.get_legend_handles_labels()
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.draw_legend(ax)
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)
         
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/general_2D_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,19 @@
             self.pcm = pcm
             
         if draw_contour:
             handle = ax.contour(X, Y, Z, levels=contour_levels, **self.styles['contour'])
              
             if draw_clabel:
                 ax.clabel(handle, **self.styles['clabel'])
+                
         if draw_contourf:
             handle = ax.contourf(X, Y, Z, levels=contour_levels, **self.styles['contourf'])
+            
         if draw_scatter:
             handle = ax.scatter(x, y, **self.styles['scatter'])
-            ax.legend(**self.styles['legend'])
              
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel,
                                   title=title)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
         
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/general_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,17 +422,16 @@
                 self.update_legend_handles({name: handle})
                 if not handle.get_children():
                     self.colors[name] = handle.get_color()
                 else:
                     self.colors[name] = handle[0].get_color()
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)  
-        handles, labels = self.get_legend_handles_labels()
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)
+        self.draw_legend(ax)
         
         if comparison_options is not None:
             if not isinstance(comparison_options, list):
                 comparison_options = [comparison_options]
             for options in comparison_options:
                 reference = options['reference']
                 target    = options['target']
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/hypotest_inverter_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,9 +146,9 @@
             handles = handles[2:] + [handles[0], (handles[1], border_leg)]
             labels = labels[2:] + [labels[0], labels[1]]
         elif nsig == 2:
             handles[1].set_linewidth(1.0)
             handles[2].set_linewidth(1.0)
             handles = handles[3:] + [handles[0], handles[1], (handles[2], border_leg)]
             labels = labels[3:] + [labels[0], labels[1], labels[2]]
-        ax.legend(handles, labels, loc='upper right', frameon=False, **self.styles['legend'])
+        self.draw_legend(ax, handles, labels, loc=loc, frameon=frameon)
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/likelihood_2D_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,16 +359,15 @@
             ax.vlines(sm_x, ymin=0, ymax=1, zorder=0, transform=transform,
                       **self.config['sm_line_styles'])
             transform = create_transform(transform_x="axis", transform_y="data")
             ax.hlines(sm_y, xmin=0, xmax=1, zorder=0, transform=transform,
                       **self.config['sm_line_styles'])
 
         if draw_legend:
-            handles, labels = self.get_legend_handles_labels()
-            ax.legend(handles, labels, **self.styles['legend'])
+            self.draw_legend(ax)
 
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
 
         return ax
 
     def draw_highlight(self, ax, x, y, label:str,
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/pdf_distribution_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,16 +453,15 @@
                 self.legend_order.append(blind_target)
                 self.update_legend_handles({target: handle[0], blind_target: handle[1]})
             else:
                 self.update_legend_handles({target: handle})
 
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
         self.set_axis_range(ax, xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax, ypad=ypad)  
-        handles, labels = self.get_legend_handles_labels()
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.draw_legend(ax)
         
         if comparison_options is not None:
             if not isinstance(comparison_options, list):
                 comparison_options = [comparison_options]
             for options in comparison_options:
                 reference = options['reference']
                 target    = options['target']
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/sample_purity_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,17 @@
             text_color = self.get_text_color(*color)
             if add_text:
                 for y, (x, c) in enumerate(zip(xcenters, widths)):
                     if c < threshold:
                         continue
                     ax.text(x, y, to_string(c, precision), ha='center', va='center',
                             color=text_color)
-        legend_styles = combine_dict(self.styles['legend'])
-        if ('ncol' in legend_styles) and (legend_styles['ncol'] == 'auto'):
-            legend_styles['ncol'] = len(categories)
-        ax.legend(**legend_styles)
+        if (('ncol' in self.styles['legend']) and
+            (self.styles['legend']['ncol'] == 'auto')):
+            legend_styles = {"ncol": len(categories)}
+        else:
+            legend_styles = {}
+        
+        self.draw_legend(ax, **legend_styles)
         
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/score_distribution_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         if not logy:
             ax.yaxis.set_major_locator(MaxNLocator(prune='lower', steps=[10]))
             ax.xaxis.set_major_locator(MaxNLocator(steps=[10]))
 
         handles, labels = ax.get_legend_handles_labels()
         new_handles = [Line2D([], [], c=h.get_edgecolor(), linestyle=h.get_linestyle(),
                               **self.styles['legend_Line2D']) if isinstance(h, Polygon) else h for h in handles]
-        ax.legend(handles=new_handles, labels=labels, **self.styles['legend'])
+        self.draw_legend(ax, handles=new_handles, labels=labels)
         if boundaries is not None:
             for boundary in boundaries:
                 ax.axvline(x=boundary, **self.config["boundary_style"])
         return ax
 
 
 def score_distribution_plot(dfs:Dict[str, pd.DataFrame], hist_options:Dict[str, Dict], 
@@ -153,15 +153,15 @@
     ax.set_xlim(xmin, xmax)
     bin_width = 1/nbins
     ax.set_xlabel(xlabel, **styles['xlabel'])
     ax.set_ylabel(ylabel.format(bin_width=bin_width), **styles['ylabel'])
     handles, labels = ax.get_legend_handles_labels()
     new_handles = [Line2D([], [], c=h.get_edgecolor(), linestyle=h.get_linestyle(), **styles['legend_Line2D'])
                    if isinstance(h, Polygon) else h for h in handles]
-    ax.legend(handles=new_handles, labels=labels, **styles['legend'])
+    self.draw_legend(ax, new_handles, labels)
     if boundaries is not None:
         for boundary in boundaries:
             ax.axvline(x=boundary, ymin=0, ymax=0.5, linestyle='--', color='k')
     return ax
 
 def score_distribution_plot_2D(dfs:Dict[str, pd.DataFrame], hist_options:Dict[str, Dict], 
                             data_options:Optional[Dict[str, Dict]]=None,
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.2.2/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/template.py` & `quickstats-0.7.0.2.2/quickstats/plots/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from cycler import cycler
 from contextlib import contextmanager
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 from matplotlib.patches import Rectangle, Polygon
-from matplotlib.collections import PolyCollection
+from matplotlib.collections import (PolyCollection, LineCollection, PathCollection)
 from matplotlib.lines import Line2D
 from matplotlib.ticker import (MultipleLocator, FormatStrFormatter,
                                AutoMinorLocator, ScalarFormatter,
                                Locator, Formatter, AutoLocator,
                                LogFormatter, LogFormatterSciNotation,
                                MaxNLocator)
-
+from matplotlib.legend_handler import (HandlerLine2D,
+                                       HandlerLineCollection,
+                                       HandlerPathCollection)
 from quickstats.utils.common_utils import combine_dict
 from quickstats import DescriptiveEnum
 
 class ResultStatus(DescriptiveEnum):
     
     FINAL     = (0, "Finalised results", "")
     INT       = (1, "Internal results", "Internal")
@@ -63,14 +65,34 @@
         return result
     
 class LogNumericFormatter(LogFormatterSciNotation):
     def __call__(self, x, pos=None):
         result = super().__call__(x, pos)
         #result = result.replace('10^{1}', '10').replace('10^{0}', '1')
         return result
+        
+class CustomHandlerLineCollection(HandlerLineCollection):
+    def create_artists(self, legend, orig_handle, xdescent, ydescent, width, height, fontsize, trans):
+        artists = super().create_artists(legend, orig_handle, xdescent, ydescent, width, height, fontsize, trans)
+        # Adjust line height to center in legend
+        for artist in artists:
+            artist.set_ydata([height / 2.0, height / 2.0])
+        return artists
+
+class CustomHandlerPathCollection(HandlerPathCollection):
+    def create_artists(self, legend, orig_handle, xdescent, ydescent, width, height, fontsize, trans):
+        artists = super().create_artists(legend, orig_handle, xdescent, ydescent, width, height, fontsize, trans)
+        # Modify the path collection offsets to center the markers in the legend
+        for artist in artists:
+            offsets = np.array([[width / 2.0, height / 2.0]])
+            artist.set_offsets(offsets)
+        return artists
+
+CUSTOM_HANDLER_MAP = {LineCollection: CustomHandlerLineCollection(),
+                      PathCollection: CustomHandlerPathCollection()}
 
 TEMPLATE_STYLES = {
     'default': {
         'figure':{
             'figsize': (11.111, 8.333),
             'dpi': 72,
             'facecolor': "#FFFFFF"
@@ -661,15 +683,15 @@
     plt.sca(axis)
     yield
     plt.sca(current_axis)
 
 def draw_analysis_label(axis, loc=(0.05, 0.95), fontsize:float=25, status:str='int',
                         energy:Optional[str]=None, lumi:Optional[str]=None,
                         colab:Optional[str]='ATLAS', main_text:Optional[str]=None,
-                        extra_text:Optional[str]=None, dy:float=0.05, dy_main:float=0.02,
+                        extra_text:Optional[str]=None, dy:float=0.02, dy_main:float=0.01,
                         transform_x:str='axis', transform_y:str='axis',
                         vertical_align:str='top', horizontal_align:str='left',
                         text_options:Optional[Dict]=None):
     """
     Draw analysis label and additional texts on a given axis.
     
     Parameters
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,22 +167,24 @@
     
     def draw_legends(self, ax, primary_handles, secondary_handles=None, asymptotic_handles=None,
                      leg_loc:Tuple=(1.02, 0.75), sec_leg_loc:Tuple=(1.02, 0.5)):
         handles, labels = ax.get_legend_handles_labels()
         if asymptotic_handles is not None:
             primary_handles += asymptotic_handles
         primary_labels = [labels[handles.index(h)] for h in primary_handles]
-        primary_leg = ax.legend(primary_handles, primary_labels, 
-                                loc=leg_loc, ncol=2, **self.styles['legend'])
+        primary_leg = self.draw_legend(ax, handles=primary_handles,
+                                       labels=primary_labels,
+                                       loc=leg_loc, ncol=2)
         ax.add_artist(primary_leg)
         
         if secondary_handles is not None:
             secondary_labels = [labels[handles.index(h)] for h in secondary_handles]
-            primary_leg = ax.legend(secondary_handles, secondary_labels, 
-                                    loc=leg_loc, ncol=2, **self.styles['legend'])
+            primary_leg = self.draw_legend(ax, handles=secondary_handles,
+                                           labels=secondary_labels, 
+                                           loc=leg_loc, ncol=2)
             ax.add_artist(primary_leg)
         
         
     def draw(self, xlabel:str=r"$\~{q}_{\mu}$",
              nbins:int=75, xmax:Optional[float]=None, ymax:float=1e3,
              leg_loc:Tuple=(1.02, 0.7), sec_leg_loc:Tuple=(1.02, 0.45)):
         if self.sec_data is not None:
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/two_axis_1D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/two_axis_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/upper_limit_1D_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,55 +122,53 @@
             text_pos = {'observed': 0.775, 'expected': 0.925}
         if draw_stat:
             text_pos = {'expected': 0.775, 'stat': 0.925}
         if (not draw_observed) and (not draw_stat):
             text_pos = {'expected': 0.925}
         if draw_third_column:
             text_pos = {'observed': 0.725, 'expected': 0.825, 'third': 0.925}
-
+        text_styles = self.styles['text'].copy()
+        text_styles['verticalalignment']   = 'center'
+        text_styles['horizontalalignment'] = 'center'
         for i, category in enumerate(self.category_df):
             df = self.category_df[category]
             # draw observed
             if draw_observed:
                 observed_limit = df['obs']
                 handle_1 = ax.vlines(observed_limit, i, i+1, colors=self.color_pallete['observed'], linestyles='solid',
                                      zorder=1.1, label=self.labels['observed'] if i == 0 else '')
                 handle_2 = ax.scatter(observed_limit, i + 0.5, s=markersize, marker='o',
                                       color=self.color_pallete['observed'], zorder=1.1)
                 observed_handle = (handle_1, handle_2)
                 if add_text:
                     ax.text(text_pos['observed'], i + 0.5, f"{{:.{sig_fig}f}}".format(observed_limit),
-                            transform=transform,
-                            **self.styles['text'])
+                            transform=transform, **text_styles)
             else:
                 observed_handle = None
             # draw stat
             if draw_stat:
                 stat_limit = df['stat']
                 if add_text:
                     ax.text(text_pos['stat'], i + 0.5, f"({{:.{sig_fig}f}})".format(stat_limit),
-                            transform=transform,
-                            **self.styles['text'])
+                            transform=transform, **text_styles)
             # draw expected
             expected_limit = df['0']
             expected_handle = ax.vlines(expected_limit, i, i + 1, colors=self.color_pallete['expected'], linestyles='dotted',
                                         zorder=1.1, label=self.labels['expected'])
             if add_text:
                 ax.text(text_pos['expected'], i + 0.5, f"{{:.{sig_fig}f}}".format(expected_limit),
-                        transform=transform,
-                        **self.styles['text'])
+                        transform=transform, **text_styles)
             # draw third
             if draw_third_column:
                 third_limit = df['third']
                 third_handle = ax.vlines(third_limit, i, i + 1, colors=self.color_pallete['third'], linestyles='dashed',
                                          zorder=1.1, label=self.labels['third'])
                 if add_text:
                     ax.text(text_pos['third'], i + 0.5, f"{{:.{sig_fig}f}}".format(third_limit),
-                            transform=transform,
-                            **self.styles['text'])
+                            transform=transform, **text_styles)
             else:
                 third_handle = None
             # draw error band
             two_sigma_handle = ax.fill_betweenx([i, i + 1], df['-2'], df['2'], facecolor=self.color_pallete['2sigma'],
                                                 label=self.labels['2sigma'])
             
             one_sigma_handle = ax.fill_betweenx([i, i + 1], df['-1'], df['1'], facecolor=self.color_pallete['1sigma'],
@@ -204,30 +202,25 @@
                 if position.shape[0] != 1:
                     raise ValueError(
                         "category `{}` not found in dataframe".format(category))
                 ax.axhline(position[0], color='k', ls='--', lw=1)
         if add_text:
             if draw_observed:
                 ax.text(text_pos['observed'], n_category + 0.3, 'Obs.',
-                        transform=transform,
-                        **self.styles['text'])
+                        transform=transform, **text_styles)
             if draw_stat:
                 ax.text(text_pos['stat'], n_category + 0.3, '(Stat.)',
-                        transform=transform,
-                        **self.styles['text'])
+                        transform=transform, **text_styles)
             if draw_third_column:
                 ax.text(text_pos['third'], n_category + 0.3, draw_third_column,
-                        transform=transform,
-                        **self.styles['text'])
+                        transform=transform, **text_styles)
             ax.text(text_pos['expected'], n_category + 0.3, 'Exp.',
-                    transform=transform,
-                    **self.styles['text'])
+                    transform=transform, **text_styles)
         if self.curve_data is not None:
             self.draw_curve(ax, self.curve_data)
         if xlabel is not None:
             ax.set_xlabel(xlabel, **self.styles['xlabel'])
         # border for the legend
         border_leg = patches.Rectangle( (0, 0), 1, 1, facecolor='none', edgecolor='black', linewidth=1)
         self.add_legend_decoration(border_leg, targets=["one_sigma", "two_sigma", "curve"])
-        handles, labels = self.get_legend_handles_labels()
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.draw_legend(ax)
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/upper_limit_2D_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,10 +454,10 @@
                                  draw_expected=draw_expected,
                                  draw_observed=draw_observed,
                                  draw_interval=draw_interval,
                                  draw_length=draw_length)
 
         indices = sorted(self.legend_data_ext.keys())
         handles, labels = self.get_legend_handles_labels(idx=indices)
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.draw_legend(ax, handles, labels)
 
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/upper_limit_3D_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,11 +287,11 @@
             self.legend_data_sec['2sigma']['handle'] = (self.legend_data_sec['2sigma']['handle'], border_leg)
             
         handles, labels = self.get_legend_handles_labels()
         if self.data_sec is not None:
             handles_sec, labels_sec = self.get_legend_handles_labels(sec=True)
             handles = handles + handles_sec
             labels  = labels + labels_sec
-        ax.legend(handles, labels, **self.styles['legend'])
+        self.draw_legend(ax, handles, labels)
 
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,13 +521,13 @@
         ax.set_xticks(np.arange(nbenchmark))
         ax.set_xticklabels(xticklabels)
         
         handles, labels = self.get_legend_handles_labels()
         handles = remake_handles(handles, polygon_to_line=False, fill_border=True,
                                  border_styles=self.styles['legend_border'])
         handler_map = {ErrorbarContainer: HandlerErrorbar(xerr_size=1)}
-        ax.legend(handles, labels, **self.styles['legend'], handler_map=handler_map)
+        self.darw_legend(handles, labels, handler_map=handler_map)
         
         if comparison_options is not None:
             return ax, ax_ratio
         
         return ax
```

### Comparing `quickstats-0.7.0.2.1/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.2.2/quickstats/plots/variable_distribution_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,15 +590,15 @@
                 
         if not self.is_single_data():
             handles, labels = self.get_legend_handles_labels()
             box_legend_handle = self.config['box_legend_handle']
             if not box_legend_handle:
                 handles = remake_handles(handles, polygon_to_line=True,
                                          line2d_styles=self.styles['legend_Line2D'])
-            ax.legend(handles=handles, labels=labels, **self.styles['legend'])
+            self.draw_legend(ax, handles=handles, labels=labels)
         
         if comparison_options is not None:
             components = comparison_options.pop('components')
             for component in components:
                 reference = component.pop('reference')
                 target    = component.pop('target')
                 bin_edges = target_bin_edges[target]
```

### Comparing `quickstats-0.7.0.2.1/quickstats/root_checker.py` & `quickstats-0.7.0.2.2/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/common_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/common_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Optional, Union, Dict, List, Tuple, Callable
+from typing import Optional, Union, Dict, List, Tuple, Callable, Any
 import os
 import sys
 import copy
 import fnmatch
 import time
 import json
 import yaml
 import inspect
 import datetime
 import functools
 import collections.abc
 
 import numpy as np
 
-from .string_utils import split_str, parse_as_dict
-
 class disable_cout:    
     def __enter__(self):
         import cppyy
         cppyy.gbl.std.cout.setstate(cppyy.gbl.std.ios_base.failbit)
         return self
 
     def __exit__(self, *args):
@@ -423,14 +421,15 @@
     if isinstance(index_levels, (int, str)):
         index_levels = (index_levels,)
     for values, level in zip(index_values, index_levels):
         df = df.loc[df.index.get_level_values(level).isin(values)]
     return df
 
 def parse_config_dict(expr:Optional[Union[str, Dict]]=None):
+    from .string_utils import parse_as_dict
     if expr is None:
         return {}
     if isinstance(expr, str):
         return parse_as_dict(expr)
     if isinstance(expr, dict):
         return expr
     raise ValueError(f'expr of type "{type(expr)}" is not convertible to a config dict')
@@ -449,18 +448,37 @@
         return {k: [item[k] for item in source] for k in source[0]}
     common_keys = set.intersection(*map(set, source))
     return {k: [item[k] for item in source] for k in common_keys}
 
 def dict_of_list_to_list_of_dict(source:Dict[str, List]):
     return [dict(zip(source, t)) for t in zip(*source.values())]
 
-def save_as_json(data:Dict, outname:str,
+def save_json(data: Dict, outname: str, indent: int = 2, truncate: bool = False) -> None:
+    """
+    Serializes a dictionary to a JSON file.
+
+    Parameters:
+    data (Dict): The dictionary object to serialize to JSON.
+    outname (str): The file path where the JSON output will be saved.
+    indent (int): The number of spaces to use for indentation in the JSON file. Default is 2.
+    truncate (bool): If True, the file will be truncated at the end of the JSON data. Default is False.
+                     Typically not needed unless dealing with file updates where the new data might
+                     be shorter than the old data.
+    """
+    with open(outname, "w") as file:
+        json.dump(data, file, indent=indent)
+        # truncate the file if the flag is True; this might be useful in case the new JSON data is shorter
+        # than any existing data in the file to prevent old data from remaining at the end of the file.
+        if truncate:
+            file.truncate()
+
+def save_json(data:Dict, outname:str,
                  indent:int=2, truncate:bool=True):
     with open(outname, "w") as file:
-        json.dump(data, file, indent=2)
+        json.dump(data, file, indent=indent)
         if truncate:
             file.truncate()
         
 def filter_dataframe_by_column_values(df:"pd.DataFrame", attributes:Dict):
     for attribute, value in attributes.items():
         if (value is None):
             continue
@@ -472,18 +490,43 @@
         elif isinstance(value, str):
             df = df[df[attribute].str.fullmatch(value)]
         elif isinstance(value, Callable):
             df = df[df[attribute].apply(value)]
         else:
             df = df[df[attribute] == value]
     df = df.reset_index(drop=True)
-    return df      
+    return df
 
 class IndentDumper(yaml.Dumper):
-    def increase_indent(self, flow=False, indentless=False):
-        return super(IndentDumper, self).increase_indent(flow, False)
+    """
+    A custom YAML Dumper that allows for increased indentation control.
+    """
+
+    def increase_indent(self, flow: bool = False, indentless: bool = False) -> None:
+        super().increase_indent(flow, False)
 
-def save_yaml(obj, filename:str, indent:int=2):
+def save_yaml(obj: Any, filename: str, indent: int = 2) -> None:
+    """
+    Saves a Python object to a YAML file with custom indentation.
+
+    Parameters:
+    obj (Any): The Python object to serialize and save to YAML.
+    filename (str): The path to the file where the YAML output should be written.
+    indent (int): The number of spaces to use for indentation. Default is 2.
+    """
     with open(filename, 'w') as f:
         yaml.dump(obj, f, Dumper=IndentDumper,
                   default_flow_style=False,
-                  sort_keys=False, indent=indent)
+                  sort_keys=False, indent=indent)
+
+def remove_duplicates(lst):
+    """
+    Removes duplicates from a list while preserving the original order of elements.
+
+    Parameters:
+    lst (list): The list from which duplicates are to be removed.
+
+    Returns:
+    list: A new list containing the unique elements of the original list in the order they first appeared.
+    """
+    seen = set()
+    return [x for x in lst if not (x in seen or seen.add(x))]
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.2.2/quickstats/utils/data_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                   "double", "Double32_t", "Double_t", "float",
                   "Float16_t", "Float_t", "int", "Int_t", 
                   "long", "long long", "Long_t", "Long64_t",
                   "short", "Short_t", "Size_t", "UChar_t",
                   "UInt_t", "ULong64_t", "ULong_t",
                   "unsigned", "unsigned char", "unsigned int",
                   "unsigned long", "unsigned long long",
-                  "unsigned short", "UShort_t"]
+                  "unsigned short", "UShort_t", "ROOT::VecOps::RVec<Char_t>"]
 
 uproot_datatypes = ["bool", "double", "float", "int", "int8_t", "int64_t", "char*", "int32_t", "uint64_t", "uint32_t"]
 
 class ConversionMode(DescriptiveEnum):
     ALL = (0, "Convert all variable types")
     REMOVE_NON_STANDARD_TYPE = (1, "Remove variables of non-standard type (i.e. other than bool, int, float, str, etc.)")
     REMOVE_NON_ARRAY_TYPE = (2, "Remove variables of non-standard type or not convertible to array of standard type")
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/py_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/roofit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import uuid
 import fnmatch
 
 import numpy as np
 
 import ROOT
 
+from quickstats import root_version
 from .string_utils import remove_whitespace, split_str
 
 def copy_attributes(source:"ROOT.RooAbsArg", target:"ROOT.RooAbsArg"):
     if source is target:
         return
     for attrib in source.attributes():
         target.setAttribute(attrib)
@@ -380,40 +381,49 @@
         return result
     nominal = nominal_term.getVal()
     magnitude = resp_term.getVal()
     beta = beta_term.getVal()
     value = round(magnitude * beta, 8)
     return {"nominal": nominal, "low": value, "high": value, "type": "gaus"}
 
-def get_logn_response_variations(nuis:ROOT.RooRealVar, client:ROOT.RooFormulaVar):
+def _get_formula_str(formula_var:"ROOT.RooFormulaVar"):
+    if root_version > (6, 26, 0):
+        return formula_var.expression()
+    return formula_var.formula().formulaString()
+
+def _get_formula_dependents(formula_var:"ROOT.RooFormulaVar"):
+    if root_version > (6, 26, 0):
+        return formula_var.dependents()
+    return formula_var.formula().actualDependents()
+
+def get_logn_response_variations(nuis:"ROOT.RooRealVar", client:"ROOT.RooFormulaVar"):
     result = {"nominal": None, "low": None, "high": None, "type": None}
     if not isinstance(client, ROOT.RooFormulaVar):
         raise ValueError("lognormal response function must be an instance of RooFormulaVar")    
     nuis_name = nuis.GetName()
-    formula = client.formula()
-    formula_str = formula.formulaString()
+    formula_str = _get_formula_str(client)
     formula_str = remove_whitespace(formula_str)
     if not formula_str.startswith("exp("):
         return result
-    dependents = formula.actualDependents()
+    dependents = _get_formula_dependents(client)
     if dependents.size() != 2:
         return result
     beta_term, nuis_term, resp_term = None, None, None
     for dependent in dependents:
         if isinstance(dependent, ROOT.RooProduct):
             nuis_term, beta_term = get_nuis_beta_terms(nuis_name, dependent.components())
         elif isinstance(dependent, ROOT.RooFormulaVar):
             resp_term = dependent
     if any(term is None for term in [beta_term, nuis_term, resp_term]):
         return result
     beta = beta_term.getVal()
-    resp_formula_str = resp_term.formula().formulaString()
+    resp_formula_str = _get_formula_str(resp_term)
     resp_formula_str = remove_whitespace(resp_formula_str)
     if resp_formula_str == "log(1+x[0]/x[1])":
-        resp_dependents = resp_term.formula().actualDependents()
+        resp_dependents = _get_formula_dependents(resp_term)
         magnitude = resp_dependents[0].getVal()
         value = round(magnitude * beta, 8)
         nominal = resp_dependents[1].getVal()
         return {"nominal": nominal, "low": value, "high": value, "type": "logn"}
     return result
 
 def get_asym_response_variations(nuis:ROOT.RooRealVar, client):
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/root_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/root_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import glob
 import time
 
 import numpy as np
 
 import ROOT
 import quickstats
+from .common_utils import get_cpu_count
 
 root_type_str_maps = {
     'Char_t'    : 'char',
     'Bool_t'    : 'bool',
     'Float_t'   : 'float',
     'Double_t'  : 'double',
     'Int_t'     : 'int',
@@ -35,15 +36,15 @@
     rtypes = [rdf.GetColumnType(c) for c in columns]
     ctypes = tuple(rtype2ctype(rtypes))
     snapshot = rdf.Snapshot.__getitem__(ctypes)
     return snapshot
 
 def is_corrupt(f:Union[ROOT.TFile, str]):
     if isinstance(f, str):
-        f = ROOT.TFile(f)
+        f = ROOT.TFile.Open(f)
     if f.IsZombie():
         return True
     if f.TestBit(ROOT.TFile.kRecovered):
         return True
     if f.GetNkeys() == 0:
         return True
     return False
@@ -374,8 +375,49 @@
         forcecache = False
     ROOT.TFile.SetCacheFileDir(cachedir, True, forcecache)
     
 def get_cachedir():
     cachedir = ROOT.TFile.GetCacheFileDir()
     if (not cachedir) or (cachedir == "/"):
         return None
-    return cachedir
+    return cachedir
+
+def set_multithread(num_threads:Union[int, bool]=None):
+    if num_threads:
+        if num_threads > 1:
+            ROOT.EnableImplicitMT(num_threads)
+        else:
+            ROOT.EnableImplicitMT()
+            num_threads = get_cpu_count()
+    else:
+        num_threads = None
+        if ROOT.IsImplicitMTEnabled():
+            ROOT.DisableImplicitMT()
+    return num_threads
+
+def get_tree_perf_stats(tree):
+    # https://eguiraud.web.cern.ch/eguiraud/decks/root_io_perf_tooling/#/6
+    ps = ROOT.TTreePerfStats("ioperf", tree)
+    for i in range(tree.GetEntriesFast()):
+        tree.GetEntry(i)
+    ps.Print() # or ps.GetXXX(), or ps.Draw()
+
+def print_tree_clusters(tree):
+    tree.Print("clusters")
+
+def set_task_per_worker_hint(m:int):
+    ROOT.TTreeProcessorMT.SetTasksPerWorkerHint(m)
+
+def get_task_per_worker_hint():
+    return ROOT.TTreeProcessorMT.GetTasksPerWorkerHint()
+
+def get_opt_flag():
+    return ROOT.gSystem.GetFlagsOpt()
+
+def get_misc_summary():
+    summary = {
+        'opt_flag': get_opt_flag(),
+        'multithread': ROOT.IsImplicitMTEnabled(),
+        'task_per_worker_hint': get_task_per_worker_hint(),
+        'cachedir': get_cachedir()
+    }
+    return summary
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/string_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/string_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,20 +86,15 @@
     if remove_empty:
         items = [item for item in items if item]
     if cast is None:
         cast = lambda x: x
     items = [cast(item) if item else empty_value for item in items]
 
     return items
-
-def split_str_excl_paranthesis(s: str, sep: str = ",", strip: bool = True, remove_empty: bool = False) -> List:
-    regex = re.compile(sep + r'\s*(?![^()]*\))')
     
-
-
 whitespace_trans = str.maketrans('', '', " \t\r\n\v")
 newline_trans = str.maketrans('', '', "\r\n")
 
 def remove_whitespace(s: str) -> str:
     """
     Removes all whitespace characters from a string.
 
@@ -343,8 +338,73 @@
     indent_string = " " * indent_size
     for key, value in dictionary.items():
         cleaned_value = value.replace("\n", " ")
         wrapped_value = insert_breaks_preserving_words(cleaned_value, effective_text_width, indent_string)
         line = f"{' ' * left_margin}{key:{max_key_length}}{separator}{wrapped_value}"
         formatted_lines.append(line)
 
-    return "\n".join(formatted_lines) + "\n"
+    return "\n".join(formatted_lines) + "\n"
+
+
+def str_to_bool(s:str) -> bool:
+    """
+    Convert a string into a boolean value.
+    
+    Parameters:
+    s (str): The string to convert.
+
+    Returns:
+    bool: The boolean value of the string.
+
+    Raises:
+    ValueError: If the string does not represent a boolean value.
+    """
+    s = s.strip().lower()
+
+    true_values = {'true', '1'}
+    false_values = {'false', '0'}
+
+    if s in true_values:
+        return True
+    elif s in false_values:
+        return False
+    else:
+        raise ValueError(f"Invalid literal for boolean: '{s}'")
+
+def remove_cpp_type_casts(expression: str) -> str:
+    """
+    Removes type casts from a C++ expression based on general structure.
+
+    Parameters:
+    expression (str): A string containing a C++ expression.
+
+    Returns:
+    str: The expression with type casts removed.
+    """
+    # Matches a parenthetical that seems like a type (any word potentially followed by pointer/reference symbols),
+    # ensuring it's not preceded by an identifier character and is followed by a valid variable name.
+    type_cast_pattern = r'(?<![\w_])\(\s*[a-zA-Z_]\w*\s*[\*&]*\s*\)\s*(?=[a-zA-Z_]\w*|[+-]?\s*\d|\.)'
+    return re.sub(type_cast_pattern, '', expression)
+
+def extract_variable_names(expression:str)->List[str]:
+    """
+    Extracts variable names from a C++ expression.
+
+    Parameters:
+    expression (str): A string containing a C++ expression.
+
+    Returns:
+    list: A list of unique variable names found in the expression.
+    """
+
+    expression = remove_cpp_type_casts(expression)
+
+    # Match potential variable names which are not directly followed by a '(' which would indicate a 
+    # function call. Use negative lookaheads and positive lookbehinds to refine the match.
+    pattern = r'\b[a-zA-Z_]\w*(?:\.\w+)*\b(?!\s*\()'
+
+    matches = re.findall(pattern, expression)
+
+    from quickstats.utils.common_utils import remove_duplicates
+    unique_matches = remove_duplicates(matches)
+    
+    return unique_matches
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.2.2/quickstats/utils/sys_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,8 +37,38 @@
     - expandvars (bool, optional): Whether to expand environment variables in cmd. Defaults to False.
     """
     if expandvars:
         cmd = os.path.expandvars(cmd)
     # Use shlex.split to correctly parse the command line string into arguments,
     # handling cases with quotes and escaped characters appropriately.
     parsed_args = shlex.split(cmd)
-    sys.argv = parsed_args
+    sys.argv = parsed_args
+
+def bytes_to_readable(size_in_bytes, digits=2):
+    """
+    Convert the number of bytes to a human-readable string format.
+
+    Parameters:
+    size_in_bytes (int): The size in bytes that you want to convert.
+    digits (int, optional): The number of decimal places to format the output. Default is 2.
+
+    Returns:
+    str: A string representing the human-readable format of the size.
+
+    Examples:
+    >>> bytes_to_readable(123456789)
+    '117.74 MB'
+
+    >>> bytes_to_readable(9876543210)
+    '9.20 GB'
+
+    >>> bytes_to_readable(123456789, digits=4)
+    '117.7383 MB'
+
+    >>> bytes_to_readable(999, digits=1)
+    '999.0 B'
+    """
+    for unit in ['B', 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']:
+        if abs(size_in_bytes) < 1024.0:
+            return f"{size_in_bytes:.{digits}f} {unit}"
+        size_in_bytes /= 1024.0
+    return f"{size_in_bytes:.{digits}f} YB"
```

### Comparing `quickstats-0.7.0.2.1/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.2.2/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.2.1/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.2.2/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.2.1
+Version: 0.7.0.2.2
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.2.1/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.2.2/quickstats.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 quickstats/components/processors/actions/__init__.py
 quickstats/components/processors/actions/auxiliary.py
 quickstats/components/processors/actions/formatter.py
 quickstats/components/processors/actions/rooproc_alias.py
 quickstats/components/processors/actions/rooproc_as_hdf.py
 quickstats/components/processors/actions/rooproc_as_numpy.py
 quickstats/components/processors/actions/rooproc_as_parquet.py
-quickstats/components/processors/actions/rooproc_awkward_array.py
 quickstats/components/processors/actions/rooproc_base_action.py
 quickstats/components/processors/actions/rooproc_declare.py
 quickstats/components/processors/actions/rooproc_define.py
 quickstats/components/processors/actions/rooproc_export.py
 quickstats/components/processors/actions/rooproc_filter.py
 quickstats/components/processors/actions/rooproc_global_variables.py
 quickstats/components/processors/actions/rooproc_helper_action.py
@@ -127,15 +126,15 @@
 quickstats/concurrent/nuisance_parameter_ranking_runner.py
 quickstats/concurrent/parameterised_asymptotic_cls.py
 quickstats/concurrent/parameterised_likelihood.py
 quickstats/concurrent/parameterised_runner.py
 quickstats/concurrent/parameterised_significance.py
 quickstats/core/__init__.py
 quickstats/core/abstract_object.py
-quickstats/core/configurations.py
+quickstats/core/configuration.py
 quickstats/core/constraints.py
 quickstats/core/decorators.py
 quickstats/core/enums.py
 quickstats/core/io.py
 quickstats/core/metaclasses.py
 quickstats/core/methods.py
 quickstats/core/path_manager.py
@@ -146,14 +145,16 @@
 quickstats/extensions/extension_dataframe.py
 quickstats/interface/__init__.py
 quickstats/interface/cppyy/__init__.py
 quickstats/interface/cppyy/basic_methods.py
 quickstats/interface/cppyy/core.py
 quickstats/interface/cppyy/macros.py
 quickstats/interface/cppyy/vectorize.py
+quickstats/interface/kerberos/__init__.py
+quickstats/interface/kerberos/core.py
 quickstats/interface/root/ModelConfig.py
 quickstats/interface/root/RDataFrame.py
 quickstats/interface/root/RooAbsArg.py
 quickstats/interface/root/RooAbsData.py
 quickstats/interface/root/RooAbsPdf.py
 quickstats/interface/root/RooArgSet.py
 quickstats/interface/root/RooCategory.py
@@ -169,17 +170,21 @@
 quickstats/interface/root/TH3.py
 quickstats/interface/root/TObject.py
 quickstats/interface/root/__init__.py
 quickstats/interface/root/helper.py
 quickstats/interface/root/io.py
 quickstats/interface/root/macros.py
 quickstats/interface/root/roofit_extension.py
+quickstats/interface/servicex/__init__.py
+quickstats/interface/servicex/core.py
 quickstats/interface/xrootd/__init__.py
 quickstats/interface/xrootd/core.py
-quickstats/interface/xrootd/utils.py
+quickstats/interface/xrootd/filesystem.py
+quickstats/interface/xrootd/path.py
+quickstats/interface/xrootd/xrd_helper.py
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
 quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
 quickstats/macros/QuickStatsCore/QStringUtils.cxx
 quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
 quickstats/macros/QuickStatsCore/RooFitExt.cxx
@@ -207,26 +212,24 @@
 quickstats/plots/correlation_plot.py
 quickstats/plots/general_1D_plot.py
 quickstats/plots/general_2D_plot.py
 quickstats/plots/general_distribution_plot.py
 quickstats/plots/hypotest_inverter_plot.py
 quickstats/plots/likelihood_1D_plot.py
 quickstats/plots/likelihood_2D_plot.py
-quickstats/plots/likelihood_scan_plot.py
 quickstats/plots/np_ranking_plot.py
 quickstats/plots/pdf_distribution_plot.py
 quickstats/plots/sample_purity_plot.py
 quickstats/plots/score_distribution_plot.py
 quickstats/plots/stat_plot_config.py
 quickstats/plots/template.py
 quickstats/plots/test_statistic_distribution_plot.py
 quickstats/plots/two_axis_1D_plot.py
 quickstats/plots/upper_limit_1D_plot.py
 quickstats/plots/upper_limit_2D_plot.py
-quickstats/plots/upper_limit_2D_plot_deprecated.py
 quickstats/plots/upper_limit_3D_plot.py
 quickstats/plots/upper_limit_benchmark_plot.py
 quickstats/plots/variable_distribution_plot.py
 quickstats/resources/default_workspace_extensions.json
 quickstats/resources/mpl_stylesheets/hep.mplstyle
 quickstats/resources/mpl_stylesheets/no_latex.mplstyle
 quickstats/resources/mpl_stylesheets/science.mplstyle
```

### Comparing `quickstats-0.7.0.2.1/setup.py` & `quickstats-0.7.0.2.2/setup.py`

 * *Files identical despite different names*

