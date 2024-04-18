# Comparing `tmp/aaanalysis-0.1.4.tar.gz` & `tmp/aaanalysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaanalysis-0.1.4.tar", max compression
+gzip compressed data, was "aaanalysis-0.1.5.tar", max compression
```

## Comparing `aaanalysis-0.1.4.tar` & `aaanalysis-0.1.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     1083 2023-09-11 12:49:07.633445 aaanalysis-0.1.4/LICENSE
--rw-r--r--   0        0        0     5101 2024-04-09 16:28:34.864556 aaanalysis-0.1.4/README.rst
--rw-r--r--   0        0        0     2274 2024-04-05 06:31:42.471141 aaanalysis-0.1.4/aaanalysis/__init__.py
--rw-r--r--   0        0        0        1 2023-08-10 12:46:09.110177 aaanalysis-0.1.4/aaanalysis/_data/__init__.py
--rw-r--r--   0        0        0       90 2023-12-07 17:03:17.995192 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/.~lock.AA_CASPASE3.tsv#
--rw-r--r--   0        0        0   559990 2022-09-06 18:44:41.884459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_CASPASE3.tsv
--rw-r--r--   0        0        0   177731 2022-09-06 18:44:41.987459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_FURIN.tsv
--rw-r--r--   0        0        0   357735 2022-09-06 18:44:42.980459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_LDR.tsv
--rw-r--r--   0        0        0   944571 2022-09-06 18:44:42.548459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_MMP2.tsv
--rw-r--r--   0        0        0   167789 2022-09-06 18:44:42.993459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_RNABIND.tsv
--rw-r--r--   0        0        0   558592 2022-09-06 18:44:42.950459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_SA.tsv
--rw-r--r--   0        0        0   101063 2023-09-12 14:33:54.138616 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/DOM_GSEC.tsv
--rw-r--r--   0        0        0   538923 2023-09-12 14:37:19.635623 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/DOM_GSEC_PU.tsv
--rw-r--r--   0        0        0     7131 2023-12-16 15:45:13.684099 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/Overview.xlsx
--rw-r--r--   0        0        0    27194 2022-09-06 18:44:40.472459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_AMYLO.tsv
--rw-r--r--   0        0        0  3482619 2022-09-06 18:44:40.724459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_CAPSID.tsv
--rw-r--r--   0        0        0   659230 2022-09-06 18:44:41.001459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_DISULFIDE.tsv
--rw-r--r--   0        0        0   762507 2022-09-19 14:45:15.221053 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_LOCATION.tsv
--rw-r--r--   0        0        0  4717120 2022-09-06 18:44:41.560459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_SOLUBLE.tsv
--rw-r--r--   0        0        0  2757288 2022-09-06 18:44:40.933459 aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_TAIL.tsv
--rw-r--r--   0        0        0    24478 2024-02-05 11:03:54.156274 aaanalysis-0.1.4/aaanalysis/_data/features/FEATURES_DOM_GSEC.xlsx
--rw-r--r--   0        0        0    87752 2023-08-11 09:49:26.000000 aaanalysis-0.1.4/aaanalysis/_data/scales.xlsx
--rw-r--r--   0        0        0    32294 2024-02-05 11:05:10.688275 aaanalysis-0.1.4/aaanalysis/_data/scales_cat.xlsx
--rw-r--r--   0        0        0    13485 2023-08-11 09:51:34.000000 aaanalysis-0.1.4/aaanalysis/_data/scales_pc.xlsx
--rw-r--r--   0        0        0    94142 2023-08-11 09:49:44.000000 aaanalysis-0.1.4/aaanalysis/_data/scales_raw.xlsx
--rw-r--r--   0        0        0   103201 2023-08-12 13:18:14.728092 aaanalysis-0.1.4/aaanalysis/_data/top60.xlsx
--rw-r--r--   0        0        0    13622 2023-12-03 13:50:16.966507 aaanalysis-0.1.4/aaanalysis/_data/top60_eval.xlsx
--rw-r--r--   0        0        0        1 2023-09-23 15:20:19.447974 aaanalysis-0.1.4/aaanalysis/_utils/__init__.py
--rw-r--r--   0        0        0      348 2024-04-05 05:50:33.508120 aaanalysis-0.1.4/aaanalysis/_utils/_utils.py
--rw-r--r--   0        0        0    13988 2024-04-05 14:56:45.762398 aaanalysis-0.1.4/aaanalysis/_utils/check_data.py
--rw-r--r--   0        0        0     3905 2024-04-05 14:54:21.075397 aaanalysis-0.1.4/aaanalysis/_utils/check_models.py
--rw-r--r--   0        0        0     9010 2024-04-05 16:56:57.220459 aaanalysis-0.1.4/aaanalysis/_utils/check_plots.py
--rw-r--r--   0        0        0     8519 2024-04-05 14:56:45.752398 aaanalysis-0.1.4/aaanalysis/_utils/check_type.py
--rw-r--r--   0        0        0     6228 2024-04-05 14:54:21.065397 aaanalysis-0.1.4/aaanalysis/_utils/decorators.py
--rw-r--r--   0        0        0     3953 2023-12-29 11:00:10.286094 aaanalysis-0.1.4/aaanalysis/_utils/metrics.py
--rw-r--r--   0        0        0    11753 2024-04-05 05:50:33.501120 aaanalysis-0.1.4/aaanalysis/_utils/plotting.py
--rw-r--r--   0        0        0     1699 2024-04-05 14:56:45.756398 aaanalysis-0.1.4/aaanalysis/_utils/utils_output.py
--rw-r--r--   0        0        0     9253 2024-02-02 08:40:14.645222 aaanalysis-0.1.4/aaanalysis/_utils/utils_plot_elements.py
--rw-r--r--   0        0        0     1194 2024-01-23 17:23:27.556401 aaanalysis-0.1.4/aaanalysis/_utils/utils_types.py
--rw-r--r--   0        0        0     7056 2024-02-13 18:33:05.447066 aaanalysis-0.1.4/aaanalysis/config.py
--rw-r--r--   0        0        0      250 2023-12-07 17:18:12.605229 aaanalysis-0.1.4/aaanalysis/data_handling/__init__.py
--rw-r--r--   0        0        0     1942 2024-02-02 17:40:03.085548 aaanalysis-0.1.4/aaanalysis/data_handling/_data_read_write.py
--rw-r--r--   0        0        0     9907 2024-01-02 09:26:37.096214 aaanalysis-0.1.4/aaanalysis/data_handling/_load_dataset.py
--rw-r--r--   0        0        0     1434 2024-01-11 01:09:05.219552 aaanalysis-0.1.4/aaanalysis/data_handling/_load_features.py
--rw-r--r--   0        0        0     8063 2024-02-08 18:33:47.296941 aaanalysis-0.1.4/aaanalysis/data_handling/_load_scales.py
--rw-r--r--   0        0        0      130 2024-01-15 21:21:22.713712 aaanalysis-0.1.4/aaanalysis/explainable_ai/__init__.py
--rw-r--r--   0        0        0    37015 2024-01-23 20:07:17.374716 aaanalysis-0.1.4/aaanalysis/explainable_ai/_shap_explainer.py
--rw-r--r--   0        0        0    25172 2024-02-04 23:55:25.444350 aaanalysis-0.1.4/aaanalysis/explainable_ai/_tree_model.py
--rw-r--r--   0        0        0        0 2023-10-05 16:24:11.422218 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/__init__.py
--rw-r--r--   0        0        0     1620 2024-01-23 16:48:02.778333 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/check_models.py
--rw-r--r--   0        0        0        0 2024-01-10 15:56:54.875489 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/__init__.py
--rw-r--r--   0        0        0     4909 2024-01-23 13:23:02.448938 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/se_add_feat_impact.py
--rw-r--r--   0        0        0     1638 2024-01-23 20:17:43.288736 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/se_add_sample_mean_dif.py
--rw-r--r--   0        0        0     6476 2024-04-05 07:35:50.481174 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/shap_explainer_fit.py
--rw-r--r--   0        0        0        0 2024-01-11 14:07:40.208586 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/__init__.py
--rw-r--r--   0        0        0     2258 2024-01-14 20:41:53.257430 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_eval.py
--rw-r--r--   0        0        0     5455 2024-01-20 21:04:30.937447 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_fit.py
--rw-r--r--   0        0        0     1355 2024-01-12 19:22:27.233408 aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_predict_proba.py
--rw-r--r--   0        0        0      340 2024-04-05 14:54:21.070397 aaanalysis-0.1.4/aaanalysis/feature_engineering/__init__.py
--rw-r--r--   0        0        0    27351 2024-02-13 12:31:16.722882 aaanalysis-0.1.4/aaanalysis/feature_engineering/_aaclust.py
--rw-r--r--   0        0        0    24647 2024-02-03 16:42:49.884539 aaanalysis-0.1.4/aaanalysis/feature_engineering/_aaclust_plot.py
--rw-r--r--   0        0        0        0 2023-10-05 16:24:11.422218 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/__init__.py
--rw-r--r--   0        0        0        0 2023-10-03 09:25:23.718916 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/__init__.py
--rw-r--r--   0        0        0     2328 2023-12-17 16:08:27.477890 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/_utils_aaclust.py
--rw-r--r--   0        0        0     1368 2024-01-02 11:20:27.261433 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_eval.py
--rw-r--r--   0        0        0     9076 2024-01-02 23:47:01.850730 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_fit.py
--rw-r--r--   0        0        0     5766 2024-01-11 18:08:59.002051 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_methods.py
--rw-r--r--   0        0        0     7342 2024-02-01 19:29:44.535604 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_plot.py
--rw-r--r--   0        0        0      338 2023-12-08 09:31:10.406780 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/check_aaclust.py
--rw-r--r--   0        0        0     2869 2024-01-30 17:50:36.267183 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/check_cpp_plot.py
--rw-r--r--   0        0        0    22627 2024-01-28 02:08:36.737688 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/check_feature.py
--rw-r--r--   0        0        0        0 2023-10-03 09:25:23.732916 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/__init__.py
--rw-r--r--   0        0        0     2517 2023-12-12 10:31:18.428773 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_part.py
--rw-r--r--   0        0        0     9632 2024-02-01 07:50:40.743182 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_split.py
--rw-r--r--   0        0        0     5035 2024-02-03 13:30:31.945423 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_elements.py
--rw-r--r--   0        0        0    11776 2024-02-03 14:56:02.114475 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_map.py
--rw-r--r--   0        0        0    18652 2024-02-03 15:00:15.085477 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_positions.py
--rw-r--r--   0        0        0     3804 2024-01-21 12:28:12.342998 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_feature_stat.py
--rw-r--r--   0        0        0     4974 2024-01-26 12:36:24.546376 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_eval.py
--rw-r--r--   0        0        0     7465 2024-01-26 19:10:09.211614 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_eval.py
--rw-r--r--   0        0        0     9226 2024-01-26 12:36:24.560376 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature.py
--rw-r--r--   0        0        0    11127 2024-02-03 14:37:13.373463 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature_map.py
--rw-r--r--   0        0        0     4095 2024-02-03 13:30:31.928423 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_heatmap.py
--rw-r--r--   0        0        0     9223 2024-02-02 17:21:27.869536 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_profile.py
--rw-r--r--   0        0        0    12158 2024-02-04 23:55:25.438350 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_ranking.py
--rw-r--r--   0        0        0     2612 2024-01-31 19:50:03.982361 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_update_seq_size.py
--rw-r--r--   0        0        0     9283 2024-01-26 12:36:24.576376 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_run.py
--rw-r--r--   0        0        0     4828 2024-01-26 12:36:24.566376 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/sequence_feature.py
--rw-r--r--   0        0        0    13718 2024-01-28 14:16:30.803839 aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/utils_feature.py
--rw-r--r--   0        0        0    22781 2024-02-13 12:41:44.006887 aaanalysis-0.1.4/aaanalysis/feature_engineering/_cpp.py
--rw-r--r--   0        0        0    81430 2024-04-05 12:46:41.587332 aaanalysis-0.1.4/aaanalysis/feature_engineering/_cpp_plot.py
--rw-r--r--   0        0        0     3793 2024-02-02 17:40:03.081548 aaanalysis-0.1.4/aaanalysis/feature_engineering/_numerical_feature.py
--rw-r--r--   0        0        0    37397 2024-02-13 12:33:35.982883 aaanalysis-0.1.4/aaanalysis/feature_engineering/_sequence_feature.py
--rw-r--r--   0        0        0      141 2023-12-17 16:40:03.164864 aaanalysis-0.1.4/aaanalysis/metrics/__init__.py
--rw-r--r--   0        0        0     8630 2024-01-23 17:42:06.095437 aaanalysis-0.1.4/aaanalysis/metrics/_metrics.py
--rw-r--r--   0        0        0      202 2023-11-06 14:15:44.451534 aaanalysis-0.1.4/aaanalysis/pertubation/__init__.py
--rw-r--r--   0        0        0      724 2024-02-02 17:40:03.062548 aaanalysis-0.1.4/aaanalysis/pertubation/_aamut.py
--rw-r--r--   0        0        0      563 2024-01-02 11:01:12.069396 aaanalysis-0.1.4/aaanalysis/pertubation/_aamut_plot.py
--rw-r--r--   0        0        0        0 2024-01-23 14:05:30.899020 aaanalysis-0.1.4/aaanalysis/pertubation/_backend/__init__.py
--rw-r--r--   0        0        0        0 2023-10-03 09:25:23.723916 aaanalysis-0.1.4/aaanalysis/pertubation/_backend/aamut/__init__.py
--rw-r--r--   0        0        0        0 2023-11-10 19:37:15.983276 aaanalysis-0.1.4/aaanalysis/pertubation/_backend/seqmut/__init__.py
--rw-r--r--   0        0        0      652 2024-02-02 17:40:03.070547 aaanalysis-0.1.4/aaanalysis/pertubation/_seqmut.py
--rw-r--r--   0        0        0      531 2024-03-06 15:49:24.733399 aaanalysis-0.1.4/aaanalysis/pertubation/_seqmut_plot.py
--rw-r--r--   0        0        0      382 2024-04-05 06:28:29.859140 aaanalysis-0.1.4/aaanalysis/plotting/__init__.py
--rw-r--r--   0        0        0     1030 2024-02-13 19:07:20.227083 aaanalysis-0.1.4/aaanalysis/plotting/_plot_gcfs.py
--rw-r--r--   0        0        0     1172 2024-02-08 13:59:43.227090 aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_cdict.py
--rw-r--r--   0        0        0     1390 2024-02-08 13:59:43.233090 aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_clist.py
--rw-r--r--   0        0        0     1984 2024-02-08 13:59:43.238090 aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_cmap.py
--rw-r--r--   0        0        0     7630 2024-02-08 13:59:43.243090 aaanalysis-0.1.4/aaanalysis/plotting/_plot_legend.py
--rw-r--r--   0        0        0     8220 2024-02-08 13:59:43.250090 aaanalysis-0.1.4/aaanalysis/plotting/_plot_settings.py
--rw-r--r--   0        0        0      123 2023-12-17 19:30:13.383726 aaanalysis-0.1.4/aaanalysis/pu_learning/__init__.py
--rw-r--r--   0        0        0        0 2023-11-10 19:37:15.977276 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/__init__.py
--rw-r--r--   0        0        0        0 2023-10-03 09:25:23.723916 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/__init__.py
--rw-r--r--   0        0        0     1403 2023-12-23 15:08:32.398502 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_compare_sets_neg.py
--rw-r--r--   0        0        0     5260 2024-01-02 11:20:27.257434 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_eval.py
--rw-r--r--   0        0        0     3627 2023-12-25 09:56:18.290882 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_fit.py
--rw-r--r--   0        0        0     5838 2024-01-26 19:10:44.243614 aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_plot.py
--rw-r--r--   0        0        0    19832 2024-02-08 19:24:10.419967 aaanalysis-0.1.4/aaanalysis/pu_learning/_dpulearn.py
--rw-r--r--   0        0        0    13005 2024-02-03 16:42:49.871539 aaanalysis-0.1.4/aaanalysis/pu_learning/_dpulearn_plot.py
--rw-r--r--   0        0        0       70 2024-04-05 06:28:29.839140 aaanalysis-0.1.4/aaanalysis/show_html/__init__.py
--rw-r--r--   0        0        0     5972 2024-04-05 05:50:33.518120 aaanalysis-0.1.4/aaanalysis/show_html/_display_df.py
--rw-r--r--   0        0        0     1552 2024-01-10 19:13:38.151868 aaanalysis-0.1.4/aaanalysis/template_classes.py
--rw-r--r--   0        0        0    29225 2024-02-04 23:26:34.210332 aaanalysis-0.1.4/aaanalysis/utils.py
--rw-r--r--   0        0        0     2834 2024-04-09 16:53:03.272603 aaanalysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7460 1970-01-01 00:00:00.000000 aaanalysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-04-18 06:54:11.381366 aaanalysis-0.1.5/LICENSE
+-rw-r--r--   0        0        0     5095 2024-04-09 17:07:07.630630 aaanalysis-0.1.5/README.rst
+-rw-r--r--   0        0        0     2274 2024-04-05 06:31:42.471141 aaanalysis-0.1.5/aaanalysis/__init__.py
+-rw-r--r--   0        0        0        1 2023-08-10 12:46:09.110177 aaanalysis-0.1.5/aaanalysis/_data/__init__.py
+-rw-r--r--   0        0        0       90 2023-12-07 17:03:17.995192 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/.~lock.AA_CASPASE3.tsv#
+-rw-r--r--   0        0        0   559990 2022-09-06 18:44:41.884459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_CASPASE3.tsv
+-rw-r--r--   0        0        0   177731 2022-09-06 18:44:41.987459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_FURIN.tsv
+-rw-r--r--   0        0        0   357735 2022-09-06 18:44:42.980459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_LDR.tsv
+-rw-r--r--   0        0        0   944571 2022-09-06 18:44:42.548459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_MMP2.tsv
+-rw-r--r--   0        0        0   167789 2022-09-06 18:44:42.993459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_RNABIND.tsv
+-rw-r--r--   0        0        0   558592 2022-09-06 18:44:42.950459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_SA.tsv
+-rw-r--r--   0        0        0   101063 2023-09-12 14:33:54.138616 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/DOM_GSEC.tsv
+-rw-r--r--   0        0        0   538923 2023-09-12 14:37:19.635623 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/DOM_GSEC_PU.tsv
+-rw-r--r--   0        0        0     7131 2023-12-16 15:45:13.684099 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/Overview.xlsx
+-rw-r--r--   0        0        0    27194 2022-09-06 18:44:40.472459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_AMYLO.tsv
+-rw-r--r--   0        0        0  3482619 2022-09-06 18:44:40.724459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_CAPSID.tsv
+-rw-r--r--   0        0        0   659230 2022-09-06 18:44:41.001459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_DISULFIDE.tsv
+-rw-r--r--   0        0        0   762507 2022-09-19 14:45:15.221053 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_LOCATION.tsv
+-rw-r--r--   0        0        0  4717120 2022-09-06 18:44:41.560459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_SOLUBLE.tsv
+-rw-r--r--   0        0        0  2757288 2022-09-06 18:44:40.933459 aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_TAIL.tsv
+-rw-r--r--   0        0        0    24478 2024-02-05 11:03:54.156274 aaanalysis-0.1.5/aaanalysis/_data/features/FEATURES_DOM_GSEC.xlsx
+-rw-r--r--   0        0        0    87752 2023-08-11 09:49:26.000000 aaanalysis-0.1.5/aaanalysis/_data/scales.xlsx
+-rw-r--r--   0        0        0    32294 2024-02-05 11:05:10.688275 aaanalysis-0.1.5/aaanalysis/_data/scales_cat.xlsx
+-rw-r--r--   0        0        0    13485 2023-08-11 09:51:34.000000 aaanalysis-0.1.5/aaanalysis/_data/scales_pc.xlsx
+-rw-r--r--   0        0        0    94142 2023-08-11 09:49:44.000000 aaanalysis-0.1.5/aaanalysis/_data/scales_raw.xlsx
+-rw-r--r--   0        0        0   103201 2023-08-12 13:18:14.728092 aaanalysis-0.1.5/aaanalysis/_data/top60.xlsx
+-rw-r--r--   0        0        0    13622 2023-12-03 13:50:16.966507 aaanalysis-0.1.5/aaanalysis/_data/top60_eval.xlsx
+-rw-r--r--   0        0        0        1 2023-09-23 15:20:19.447974 aaanalysis-0.1.5/aaanalysis/_utils/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-05 05:50:33.508120 aaanalysis-0.1.5/aaanalysis/_utils/_utils.py
+-rw-r--r--   0        0        0    14265 2024-04-17 14:19:23.304327 aaanalysis-0.1.5/aaanalysis/_utils/check_data.py
+-rw-r--r--   0        0        0     3905 2024-04-05 14:54:21.075397 aaanalysis-0.1.5/aaanalysis/_utils/check_models.py
+-rw-r--r--   0        0        0     9010 2024-04-05 16:56:57.220459 aaanalysis-0.1.5/aaanalysis/_utils/check_plots.py
+-rw-r--r--   0        0        0     8519 2024-04-05 14:56:45.752398 aaanalysis-0.1.5/aaanalysis/_utils/check_type.py
+-rw-r--r--   0        0        0     6228 2024-04-05 14:54:21.065397 aaanalysis-0.1.5/aaanalysis/_utils/decorators.py
+-rw-r--r--   0        0        0     3953 2023-12-29 11:00:10.286094 aaanalysis-0.1.5/aaanalysis/_utils/metrics.py
+-rw-r--r--   0        0        0    11753 2024-04-05 05:50:33.501120 aaanalysis-0.1.5/aaanalysis/_utils/plotting.py
+-rw-r--r--   0        0        0     1699 2024-04-05 14:56:45.756398 aaanalysis-0.1.5/aaanalysis/_utils/utils_output.py
+-rw-r--r--   0        0        0     9253 2024-02-02 08:40:14.645222 aaanalysis-0.1.5/aaanalysis/_utils/utils_plot_elements.py
+-rw-r--r--   0        0        0     1194 2024-01-23 17:23:27.556401 aaanalysis-0.1.5/aaanalysis/_utils/utils_types.py
+-rw-r--r--   0        0        0     7057 2024-04-18 10:00:33.194081 aaanalysis-0.1.5/aaanalysis/config.py
+-rw-r--r--   0        0        0      250 2023-12-07 17:18:12.605229 aaanalysis-0.1.5/aaanalysis/data_handling/__init__.py
+-rw-r--r--   0        0        0     1942 2024-02-02 17:40:03.085548 aaanalysis-0.1.5/aaanalysis/data_handling/_data_read_write.py
+-rw-r--r--   0        0        0     9907 2024-01-02 09:26:37.096214 aaanalysis-0.1.5/aaanalysis/data_handling/_load_dataset.py
+-rw-r--r--   0        0        0     1434 2024-01-11 01:09:05.219552 aaanalysis-0.1.5/aaanalysis/data_handling/_load_features.py
+-rw-r--r--   0        0        0     8063 2024-02-08 18:33:47.296941 aaanalysis-0.1.5/aaanalysis/data_handling/_load_scales.py
+-rw-r--r--   0        0        0      130 2024-01-15 21:21:22.713712 aaanalysis-0.1.5/aaanalysis/explainable_ai/__init__.py
+-rw-r--r--   0        0        0    37015 2024-01-23 20:07:17.374716 aaanalysis-0.1.5/aaanalysis/explainable_ai/_shap_explainer.py
+-rw-r--r--   0        0        0    25172 2024-02-04 23:55:25.444350 aaanalysis-0.1.5/aaanalysis/explainable_ai/_tree_model.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:24:11.422218 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/__init__.py
+-rw-r--r--   0        0        0     1620 2024-01-23 16:48:02.778333 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/check_models.py
+-rw-r--r--   0        0        0        0 2024-01-10 15:56:54.875489 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/__init__.py
+-rw-r--r--   0        0        0     4909 2024-01-23 13:23:02.448938 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/se_add_feat_impact.py
+-rw-r--r--   0        0        0     1638 2024-01-23 20:17:43.288736 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/se_add_sample_mean_dif.py
+-rw-r--r--   0        0        0     6476 2024-04-05 07:35:50.481174 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/shap_explainer_fit.py
+-rw-r--r--   0        0        0        0 2024-01-11 14:07:40.208586 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/__init__.py
+-rw-r--r--   0        0        0     2258 2024-01-14 20:41:53.257430 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_eval.py
+-rw-r--r--   0        0        0     5455 2024-01-20 21:04:30.937447 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_fit.py
+-rw-r--r--   0        0        0     1355 2024-01-12 19:22:27.233408 aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_predict_proba.py
+-rw-r--r--   0        0        0      340 2024-04-05 14:54:21.070397 aaanalysis-0.1.5/aaanalysis/feature_engineering/__init__.py
+-rw-r--r--   0        0        0    27323 2024-04-16 19:59:06.546676 aaanalysis-0.1.5/aaanalysis/feature_engineering/_aaclust.py
+-rw-r--r--   0        0        0    24647 2024-02-03 16:42:49.884539 aaanalysis-0.1.5/aaanalysis/feature_engineering/_aaclust_plot.py
+-rw-r--r--   0        0        0        0 2023-10-05 16:24:11.422218 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-03 09:25:23.718916 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/__init__.py
+-rw-r--r--   0        0        0     2328 2023-12-17 16:08:27.477890 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/_utils_aaclust.py
+-rw-r--r--   0        0        0     1368 2024-01-02 11:20:27.261433 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_eval.py
+-rw-r--r--   0        0        0     9076 2024-01-02 23:47:01.850730 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_fit.py
+-rw-r--r--   0        0        0     5766 2024-01-11 18:08:59.002051 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_methods.py
+-rw-r--r--   0        0        0     7342 2024-02-01 19:29:44.535604 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_plot.py
+-rw-r--r--   0        0        0      338 2023-12-08 09:31:10.406780 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/check_aaclust.py
+-rw-r--r--   0        0        0     2869 2024-01-30 17:50:36.267183 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/check_cpp_plot.py
+-rw-r--r--   0        0        0    22627 2024-01-28 02:08:36.737688 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/check_feature.py
+-rw-r--r--   0        0        0        0 2023-10-03 09:25:23.732916 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/__init__.py
+-rw-r--r--   0        0        0     2517 2023-12-12 10:31:18.428773 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_part.py
+-rw-r--r--   0        0        0     9632 2024-02-01 07:50:40.743182 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_split.py
+-rw-r--r--   0        0        0     5035 2024-02-03 13:30:31.945423 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_elements.py
+-rw-r--r--   0        0        0    11776 2024-02-03 14:56:02.114475 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_map.py
+-rw-r--r--   0        0        0    18652 2024-02-03 15:00:15.085477 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_positions.py
+-rw-r--r--   0        0        0     3804 2024-01-21 12:28:12.342998 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_feature_stat.py
+-rw-r--r--   0        0        0     4974 2024-01-26 12:36:24.546376 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_eval.py
+-rw-r--r--   0        0        0     7465 2024-01-26 19:10:09.211614 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_eval.py
+-rw-r--r--   0        0        0     9226 2024-01-26 12:36:24.560376 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature.py
+-rw-r--r--   0        0        0    11127 2024-02-03 14:37:13.373463 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature_map.py
+-rw-r--r--   0        0        0     4095 2024-02-03 13:30:31.928423 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_heatmap.py
+-rw-r--r--   0        0        0     9223 2024-02-02 17:21:27.869536 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_profile.py
+-rw-r--r--   0        0        0    12158 2024-02-04 23:55:25.438350 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_ranking.py
+-rw-r--r--   0        0        0     2612 2024-01-31 19:50:03.982361 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_update_seq_size.py
+-rw-r--r--   0        0        0     9314 2024-04-17 14:01:47.306354 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_run.py
+-rw-r--r--   0        0        0     4828 2024-01-26 12:36:24.566376 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/sequence_feature.py
+-rw-r--r--   0        0        0    13721 2024-04-17 13:46:49.727377 aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/utils_feature.py
+-rw-r--r--   0        0        0    22781 2024-02-13 12:41:44.006887 aaanalysis-0.1.5/aaanalysis/feature_engineering/_cpp.py
+-rw-r--r--   0        0        0    81430 2024-04-05 12:46:41.587332 aaanalysis-0.1.5/aaanalysis/feature_engineering/_cpp_plot.py
+-rw-r--r--   0        0        0     3793 2024-02-02 17:40:03.081548 aaanalysis-0.1.5/aaanalysis/feature_engineering/_numerical_feature.py
+-rw-r--r--   0        0        0    37395 2024-04-17 12:51:28.858461 aaanalysis-0.1.5/aaanalysis/feature_engineering/_sequence_feature.py
+-rw-r--r--   0        0        0      141 2023-12-17 16:40:03.164864 aaanalysis-0.1.5/aaanalysis/metrics/__init__.py
+-rw-r--r--   0        0        0     8630 2024-01-23 17:42:06.095437 aaanalysis-0.1.5/aaanalysis/metrics/_metrics.py
+-rw-r--r--   0        0        0      202 2023-11-06 14:15:44.451534 aaanalysis-0.1.5/aaanalysis/pertubation/__init__.py
+-rw-r--r--   0        0        0      724 2024-02-02 17:40:03.062548 aaanalysis-0.1.5/aaanalysis/pertubation/_aamut.py
+-rw-r--r--   0        0        0      563 2024-01-02 11:01:12.069396 aaanalysis-0.1.5/aaanalysis/pertubation/_aamut_plot.py
+-rw-r--r--   0        0        0        0 2024-01-23 14:05:30.899020 aaanalysis-0.1.5/aaanalysis/pertubation/_backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-03 09:25:23.723916 aaanalysis-0.1.5/aaanalysis/pertubation/_backend/aamut/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-10 19:37:15.983276 aaanalysis-0.1.5/aaanalysis/pertubation/_backend/seqmut/__init__.py
+-rw-r--r--   0        0        0      652 2024-02-02 17:40:03.070547 aaanalysis-0.1.5/aaanalysis/pertubation/_seqmut.py
+-rw-r--r--   0        0        0      531 2024-03-06 15:49:24.733399 aaanalysis-0.1.5/aaanalysis/pertubation/_seqmut_plot.py
+-rw-r--r--   0        0        0      382 2024-04-05 06:28:29.859140 aaanalysis-0.1.5/aaanalysis/plotting/__init__.py
+-rw-r--r--   0        0        0     1030 2024-02-13 19:07:20.227083 aaanalysis-0.1.5/aaanalysis/plotting/_plot_gcfs.py
+-rw-r--r--   0        0        0     1172 2024-02-08 13:59:43.227090 aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_cdict.py
+-rw-r--r--   0        0        0     1390 2024-02-08 13:59:43.233090 aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_clist.py
+-rw-r--r--   0        0        0     1984 2024-02-08 13:59:43.238090 aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_cmap.py
+-rw-r--r--   0        0        0     7630 2024-02-08 13:59:43.243090 aaanalysis-0.1.5/aaanalysis/plotting/_plot_legend.py
+-rw-r--r--   0        0        0     8220 2024-02-08 13:59:43.250090 aaanalysis-0.1.5/aaanalysis/plotting/_plot_settings.py
+-rw-r--r--   0        0        0      123 2023-12-17 19:30:13.383726 aaanalysis-0.1.5/aaanalysis/pu_learning/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-10 19:37:15.977276 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-03 09:25:23.723916 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/__init__.py
+-rw-r--r--   0        0        0     1403 2023-12-23 15:08:32.398502 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_compare_sets_neg.py
+-rw-r--r--   0        0        0     5260 2024-01-02 11:20:27.257434 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_eval.py
+-rw-r--r--   0        0        0     3627 2023-12-25 09:56:18.290882 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_fit.py
+-rw-r--r--   0        0        0     5838 2024-01-26 19:10:44.243614 aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_plot.py
+-rw-r--r--   0        0        0    19832 2024-02-08 19:24:10.419967 aaanalysis-0.1.5/aaanalysis/pu_learning/_dpulearn.py
+-rw-r--r--   0        0        0    13005 2024-02-03 16:42:49.871539 aaanalysis-0.1.5/aaanalysis/pu_learning/_dpulearn_plot.py
+-rw-r--r--   0        0        0       70 2024-04-05 06:28:29.839140 aaanalysis-0.1.5/aaanalysis/show_html/__init__.py
+-rw-r--r--   0        0        0     5972 2024-04-05 05:50:33.518120 aaanalysis-0.1.5/aaanalysis/show_html/_display_df.py
+-rw-r--r--   0        0        0     1552 2024-01-10 19:13:38.151868 aaanalysis-0.1.5/aaanalysis/template_classes.py
+-rw-r--r--   0        0        0    29220 2024-04-18 10:00:33.204081 aaanalysis-0.1.5/aaanalysis/utils.py
+-rw-r--r--   0        0        0     2834 2024-04-18 15:12:02.060605 aaanalysis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7454 1970-01-01 00:00:00.000000 aaanalysis-0.1.5/PKG-INFO
```

### Comparing `aaanalysis-0.1.4/README.rst` & `aaanalysis-0.1.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 ..
     Missing badges
     |Conda Version|
 
 .. list-table::
-   :widths: 25 75
+   :widths: 20 80
    :header-rows: 1
 
    * - **Package**
      - |PyPI Status| |PyPI Version| |Supported Python Versions| |Downloads| |License|
    * - **Testing**
      - |Unit Tests| |CodeQL| |Codecov| |Documentation Status|
 
@@ -86,21 +86,21 @@
 
 Install
 =======
 **AAanalysis** can be installed from `PyPi <https://pypi.org/project/aaanalysis>`_:
 
 .. code-block:: bash
 
-   pip install -u aaanalysis
+   pip install aaanalysis
 
 For extended features, including our explainable AI module, please use the 'professional' version:
 
 .. code-block:: bash
 
-   pip install -u aaanalysis[pro]
+   pip install aaanalysis[pro]
 
 Contributing
 ============
 We appreciate bug reports, feature requests, or updates on documentation and code. For details, please refer to
 `Contributing Guidelines <CONTRIBUTING.rst>`_. These include specifics about AAanalysis and also notes on Test
 Guided Development (TGD) using ChatGPT. For further questions or suggestions, please email stephanbreimann@gmail.com.
```

### Comparing `aaanalysis-0.1.4/aaanalysis/__init__.py` & `aaanalysis-0.1.5/aaanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_CASPASE3.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_CASPASE3.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_FURIN.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_FURIN.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_LDR.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_LDR.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_MMP2.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_MMP2.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_RNABIND.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_RNABIND.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/AA_SA.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/AA_SA.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/DOM_GSEC.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/DOM_GSEC.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/DOM_GSEC_PU.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/DOM_GSEC_PU.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/Overview.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/Overview.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_AMYLO.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_AMYLO.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_CAPSID.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_CAPSID.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_DISULFIDE.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_DISULFIDE.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_LOCATION.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_LOCATION.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_SOLUBLE.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_SOLUBLE.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/benchmarks/SEQ_TAIL.tsv` & `aaanalysis-0.1.5/aaanalysis/_data/benchmarks/SEQ_TAIL.tsv`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/features/FEATURES_DOM_GSEC.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/features/FEATURES_DOM_GSEC.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/scales.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/scales.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/scales_cat.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/scales_cat.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/scales_pc.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/scales_pc.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/scales_raw.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/scales_raw.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/top60.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/top60.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_data/top60_eval.xlsx` & `aaanalysis-0.1.5/aaanalysis/_data/top60_eval.xlsx`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/check_data.py` & `aaanalysis-0.1.5/aaanalysis/_utils/check_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,7 +272,13 @@
                                 str_add=str_add)
             raise ValueError(str_error)
     if cols_nan_check is not None:
         if df[cols_nan_check].isna().sum().sum() > 0:
             str_error = add_str(str_error=f"NaN values are not allowed in '{cols_nan_check}'.",
                                 str_add=str_add)
             raise ValueError(str_error)
+    columns = list(df)
+    cols_duplicated = [x for x in columns if columns.count(x) > 1]
+    if len(cols_duplicated) > 0:
+        str_error = add_str(str_error=f"The following columns are duplicated '{cols_duplicated}'.", str_add=str_add)
+        raise ValueError(str_error)
+
```

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/check_models.py` & `aaanalysis-0.1.5/aaanalysis/_utils/check_models.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/check_plots.py` & `aaanalysis-0.1.5/aaanalysis/_utils/check_plots.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/check_type.py` & `aaanalysis-0.1.5/aaanalysis/_utils/check_type.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/decorators.py` & `aaanalysis-0.1.5/aaanalysis/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/metrics.py` & `aaanalysis-0.1.5/aaanalysis/_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/plotting.py` & `aaanalysis-0.1.5/aaanalysis/_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/utils_output.py` & `aaanalysis-0.1.5/aaanalysis/_utils/utils_output.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/utils_plot_elements.py` & `aaanalysis-0.1.5/aaanalysis/_utils/utils_plot_elements.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/_utils/utils_types.py` & `aaanalysis-0.1.5/aaanalysis/_utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/config.py` & `aaanalysis-0.1.5/aaanalysis/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,9 +162,10 @@
         """Check if a key is in the settings."""
         return key in self._settings
 
     def __str__(self) -> str:
         """Return a string representation of the settings dictionary."""
         return str(self._settings)
 
+
 # Global settings instance
 options = Settings()
```

### Comparing `aaanalysis-0.1.4/aaanalysis/data_handling/_data_read_write.py` & `aaanalysis-0.1.5/aaanalysis/data_handling/_data_read_write.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/data_handling/_load_dataset.py` & `aaanalysis-0.1.5/aaanalysis/data_handling/_load_dataset.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/data_handling/_load_features.py` & `aaanalysis-0.1.5/aaanalysis/data_handling/_load_features.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/data_handling/_load_scales.py` & `aaanalysis-0.1.5/aaanalysis/data_handling/_load_scales.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/_shap_explainer.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/_shap_explainer.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/_tree_model.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/_tree_model.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/check_models.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/check_models.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/se_add_feat_impact.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/se_add_feat_impact.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/se_add_sample_mean_dif.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/se_add_sample_mean_dif.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/shap_explainer/shap_explainer_fit.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/shap_explainer/shap_explainer_fit.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_eval.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_eval.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_fit.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_fit.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/explainable_ai/backend/tree_model/tree_model_predict_proba.py` & `aaanalysis-0.1.5/aaanalysis/explainable_ai/backend/tree_model/tree_model_predict_proba.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_aaclust.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_aaclust.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,29 +251,29 @@
             self.model = self._model_class(n_clusters=n_clusters, **self._model_kwargs)
             labels = self.model.fit(X).labels_.tolist()
 
         # Clustering using AAclust algorithm
         else:
             # 1. Step: Estimation of lower bound of k (number of clusters)
             if self._verbose:
-                ut.print_out("1. Estimation of lower bound of k (number of clusters)", end="")
+                ut.print_out("1. Estimation of lower bound of k (number of clusters)")
             n_clusters_lb = estimate_lower_bound_n_clusters(X, **args)
             # 2. Step: Optimization of k by recursive clustering
             if self._verbose:
                 objective_fct = "min_cor_center" if on_center else "min_cor_all"
-                ut.print_out(f"2. Optimization of k by recursive clustering ({objective_fct}, min_th={min_th}, k={n_clusters_lb})", end="")
+                ut.print_out(f"2. Optimization of k by recursive clustering ({objective_fct}, min_th={min_th}, k={n_clusters_lb})")
             n_clusters = optimize_n_clusters(X, n_clusters=n_clusters_lb, **args)
             self.model = self._model_class(n_clusters=n_clusters, **self._model_kwargs)
             labels = self.model.fit(X).labels_.tolist()
             # 3. Step: Cluster merging (optional)
             if metric is not None:
-                if self._verbose:
-                    ut.print_out(f"3. Cluster merging (k={len(labels)})", end="")
                 labels = merge_clusters(X, labels=labels, min_th=min_th, on_center=on_center, metric=metric)
                 n_clusters = len(set(labels))
+                if self._verbose:
+                    ut.print_out(f"3. Cluster merging (k={n_clusters})")
 
         # Obtain cluster centers and medoids
         medoids, medoid_labels, medoid_ind = compute_medoids(X, labels=labels)
         centers, center_labels = compute_centers(X, labels=labels)
 
         # Save results in output parameters
         post_check_n_clusters(n_clusters_actual=len(set(labels)), n_clusters=n_clusters)
@@ -545,17 +545,17 @@
         # Get correlations
         df_corr, labels_sorted = compute_correlation(X, X_ref=X_ref,
                                                      labels=labels, labels_ref=labels_ref,
                                                      names=names, names_ref=names_ref)
         return df_corr, labels_sorted
 
     @staticmethod
-    def comp_coverage(names : List[str] = None,
-                      names_ref : List[str] = None
-                      ) -> float :
+    def comp_coverage(names: List[str] = None,
+                      names_ref: List[str] = None
+                      ) -> float:
         """
         Computes the percentage of unique names from ``names`` that are present in ``names_ref``.
 
         This method helps in understanding the coverage of a particular set of names (subset)
         within a reference set of names (universal set). Each name from both ``names`` and ``names_ref``
         are considered only once, regardless of repetition.
```

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_aaclust_plot.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_aaclust_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/_utils_aaclust.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/_utils_aaclust.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_eval.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_eval.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_fit.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_fit.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_methods.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_methods.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/aaclust/aaclust_plot.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/aaclust/aaclust_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/check_cpp_plot.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/check_cpp_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/check_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/check_feature.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_part.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_part.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_split.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_split.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_elements.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_elements.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_map.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_map.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_positions.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_cpp_plot_positions.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/_utils_feature_stat.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/_utils_feature_stat.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_eval.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_eval.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_eval.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_eval.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature_map.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_feature_map.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_heatmap.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_profile.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_profile.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_ranking.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_ranking.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_update_seq_size.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_plot_update_seq_size.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/cpp_run.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/cpp_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 This is a script for the backend of the CPP.run() method.
 
 This is the key algorithm of CPP and for AAanalysis.
 """
 import os
 import numpy as np
 import pandas as pd
-import multiprocessing as mp
-from itertools import repeat
+from joblib import Parallel, delayed
 import warnings
 
 import aaanalysis.utils as ut
 from .utils_feature import get_vf_scale, get_feature_matrix_, post_check_vf_scale
 from ._utils_feature_stat import add_stat_
 from ._split import SplitRange
 
@@ -94,43 +93,51 @@
         dict_c = dict()
     dict_p = dict(zip(df[ut.COL_FEATURE], [set(x) for x in df["positions"]]))
     df_cor = df_scales.corr()
     return dict_c, dict_p, df_cor
 
 
 # II Main functions
+
+
 # Filtering methods
 def pre_filtering_info(df_parts=None, split_kws=None, df_scales=None, labels=None, label_test=1, label_ref=0,
                        accept_gaps=False, verbose=True, n_jobs=None):
     """Get n best features in descending order based on the abs(mean(group1) - mean(group0),
     where group 1 is the target group"""
     # Input (df_parts, split_kws, df_scales, y) checked in main method (CPP.run())
     mask_ref = [x == label_ref for x in labels]
     mask_test = [x == label_test for x in labels]
+    # Initial splitting
     part_split, labels_ps = _splitting(split_kws=split_kws, df_parts=df_parts)
     list_scales = list(df_scales)
     dict_all_scales = {col: dict(zip(df_scales.index.to_list(), df_scales[col])) for col in list_scales}
+
+    # Function to be parallelized
+    def compute_pre_filtering_info(scales_chunk):
+        args = [scales_chunk, dict_all_scales, labels_ps, part_split, accept_gaps, mask_ref, mask_test, verbose]
+        return _pre_filtering_info(*args)
+
     # Feature filtering
     if n_jobs == 1:
         # Run in a single process
-        args = [list_scales, dict_all_scales, labels_ps, part_split, accept_gaps, mask_ref, mask_test, verbose]
-        abs_mean_dif, std_test, feat_names = _pre_filtering_info(*args)
+        abs_mean_dif, std_test, feat_names = compute_pre_filtering_info(list_scales)
     else:
         # Run in multiple processes
-        n_jobs = min([os.cpu_count(), len(list_scales)])
-        scale_chunks = np.array_split(list_scales, n_jobs)
-        args = zip(scale_chunks, repeat(dict_all_scales), repeat(labels_ps), repeat(part_split), repeat(accept_gaps),
-                   repeat(mask_ref), repeat(mask_test), repeat(verbose))
-        with mp.get_context("spawn").Pool(processes=n_jobs) as pool:
-            result = pool.starmap(_pre_filtering_info, args)
-        abs_mean_dif = np.concatenate([x[0] for x in result])
-        std_test = np.concatenate([x[1] for x in result])
-        feat_names = np.concatenate([x[2] for x in result])
+        if n_jobs is None:
+            n_jobs = min([os.cpu_count(), len(list_scales)])  # Parallel processing
+        results = Parallel(n_jobs=n_jobs)(
+            delayed(compute_pre_filtering_info)(scales_chunk) for scales_chunk in np.array_split(list_scales, n_jobs))
+        # Concatenate results from all jobs
+        abs_mean_dif = np.concatenate([x[0] for x in results])
+        std_test = np.concatenate([x[1] for x in results])
+        feat_names = np.concatenate([x[2] for x in results])
     return abs_mean_dif, std_test, feat_names
 
+
 def pre_filtering(features=None, abs_mean_dif=None, std_test=None, max_std_test=0.2, n=10000):
     """CPP pre-filtering based on thresholds."""
     df = pd.DataFrame(zip(features, abs_mean_dif, std_test),
                       columns=[ut.COL_FEATURE, ut.COL_ABS_MEAN_DIF, ut.COL_STD_TEST])
     df = df[df[ut.COL_STD_TEST] <= max_std_test]
     df = df.sort_values(by=ut.COL_ABS_MEAN_DIF, ascending=False).head(n)
     return df
```

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/sequence_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/sequence_feature.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_backend/cpp/utils_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_backend/cpp/utils_feature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 This is a script for utility feature functions for CPP and SequenceFeature objects and backend.
 """
 import os
 import numpy as np
-from itertools import repeat
-import multiprocessing as mp
 import pandas as pd
+from joblib import Parallel, delayed
 
 from ._part import create_parts
 from ._split import Split
 import aaanalysis.utils as ut
 
 
 # I Helper Functions
@@ -18,14 +17,15 @@
     """Check for the presence of a specific gap string in the sequence."""
     # Join the elements of part_split into a single string
     combined_string = "".join(part_split)
     # Check if ut.STR_AA_GAP is in the combined string
     if ut.STR_AA_GAP in combined_string:
         raise ValueError("Some input sequences contain gaps ('-').")
 
+
 def post_check_vf_scale(feature_values=None):
     """Check if feature_values/X does contain nans due to gaps"""
     if np.isnan(feature_values).any():
         raise ValueError("Some input sequences result in NaN feature values most likely due to gaps ('-').")
 
 
 def get_vf_scale(dict_scale=None, accept_gaps=False):
@@ -215,32 +215,34 @@
     f_pat = lambda x: "-".join([seq[int(p)] for p in x.split(",")])
     feat_aa = [f_seg(pos) if "Segment" in feat else f_pat(pos) for feat, pos in zip(features, pos)]
     return feat_aa
 
 
 def get_feature_matrix_(features=None, df_parts=None, df_scales=None, accept_gaps=False, n_jobs=None):
     """Create feature matrix for given feature ids and sequence parts."""
-    features = [features] if type(features) is str else features
+    features = [features] if isinstance(features, str) else features
     dict_all_scales = _get_dict_all_scales(df_scales=df_scales)
-    # Convert features to list if needed
     features = features.to_list() if isinstance(features, pd.Series) else features
+
+    # Function to be parallelized
+    def compute_feature_matrix(features_subset):
+        return _feature_matrix(features_subset, dict_all_scales, df_parts, accept_gaps)
+
     # Feature creation
     if n_jobs == 1:
-        # Run in a single process
-        feat_matrix = _feature_matrix(features, dict_all_scales, df_parts, accept_gaps)
+        # Process in a single thread/process
+        feat_matrix = compute_feature_matrix(features)
     else:
-        # Run in multiple processes
+        # If n_jobs is not specified, decide it dynamically based on the number of features
         if n_jobs is None:
-            # Optimize n_jobs that each core processes a minimum of 10 features
-            n_jobs = min([os.cpu_count(), max([int(len(features)/10), 1])])
-        feat_chunks = np.array_split(features, n_jobs)
-        args = zip(feat_chunks, repeat(dict_all_scales), repeat(df_parts), repeat(accept_gaps))
-        with mp.get_context("spawn").Pool(processes=n_jobs) as pool:
-            result = pool.starmap(_feature_matrix, args)
-        feat_matrix = np.concatenate(result, axis=1)
+            n_jobs = min(os.cpu_count(), max(int(len(features) / 10), 1))
+        # Use joblib to parallelize the computation
+        results = Parallel(n_jobs=n_jobs)(
+            delayed(compute_feature_matrix)(features_chunk) for features_chunk in np.array_split(features, n_jobs))
+        feat_matrix = np.concatenate(results, axis=1)
     return feat_matrix
 
 
 def get_df_pos_(df_feat=None, col_cat="category", col_val=None, value_type="count", start=None, stop=None):
     """Get df with aggregated values for each combination of column values and positions"""
     df_feat = df_feat.copy()
     list_y_cat = sorted(set(df_feat[col_cat]))
```

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_cpp.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_cpp.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_cpp_plot.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_cpp_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_numerical_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_numerical_feature.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/feature_engineering/_sequence_feature.py` & `aaanalysis-0.1.5/aaanalysis/feature_engineering/_sequence_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,16 @@
         return split_kws
 
     # Feature methods
     def get_df_feat(self,
                     features: ut.ArrayLike1D = None,
                     df_parts: pd.DataFrame = None,
                     labels: ut.ArrayLike1D = None,
-                    label_test : int = 1,
-                    label_ref : int = 0,
+                    label_test: int = 1,
+                    label_ref: int = 0,
                     df_scales: Optional[pd.DataFrame] = None,
                     df_cat: Optional[pd.DataFrame] = None,
                     start: int = 1,
                     tmd_len: int = 20,
                     jmd_c_len: int = 10,
                     jmd_n_len: int = 10,
                     accept_gaps: bool = False,
```

### Comparing `aaanalysis-0.1.4/aaanalysis/metrics/_metrics.py` & `aaanalysis-0.1.5/aaanalysis/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pertubation/_aamut.py` & `aaanalysis-0.1.5/aaanalysis/pertubation/_aamut.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pertubation/_aamut_plot.py` & `aaanalysis-0.1.5/aaanalysis/pertubation/_aamut_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pertubation/_seqmut.py` & `aaanalysis-0.1.5/aaanalysis/pertubation/_seqmut.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pertubation/_seqmut_plot.py` & `aaanalysis-0.1.5/aaanalysis/pertubation/_seqmut_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_gcfs.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_gcfs.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_cdict.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_cdict.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_clist.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_clist.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_get_cmap.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_get_cmap.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_legend.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_legend.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/plotting/_plot_settings.py` & `aaanalysis-0.1.5/aaanalysis/plotting/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_compare_sets_neg.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_compare_sets_neg.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_eval.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_eval.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_fit.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_fit.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_backend/dpulearn/dpul_plot.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_backend/dpulearn/dpul_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_dpulearn.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_dpulearn.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/pu_learning/_dpulearn_plot.py` & `aaanalysis-0.1.5/aaanalysis/pu_learning/_dpulearn_plot.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/show_html/_display_df.py` & `aaanalysis-0.1.5/aaanalysis/show_html/_display_df.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/template_classes.py` & `aaanalysis-0.1.5/aaanalysis/template_classes.py`

 * *Files identical despite different names*

### Comparing `aaanalysis-0.1.4/aaanalysis/utils.py` & `aaanalysis-0.1.5/aaanalysis/utils.py`

 * *Files identical despite different names*

```diff
@@ -294,15 +294,14 @@
 # Parameter options for cmaps and color dicts
 STR_CMAP_CPP = "CPP"
 STR_CMAP_SHAP = "SHAP"
 STR_DICT_COLOR = "DICT_COLOR"
 STR_DICT_CAT = "DICT_CAT"
 
 
-
 # I Helper functions
 def _retrieve_string_starting_at_end(seq, start=None, end=None):
     """Reverse_string_start_end"""
     def reverse_string(s):
         return s[::-1]
     reversed_seq = reverse_string(seq)
     reversed_seq_part = reversed_seq[start:end]
@@ -326,17 +325,14 @@
                      'ext_n': ext_n, 'ext_c': ext_c,
                      'tmd_jmd': jmd_n + tmd + jmd_c,
                      'jmd_n_tmd_n': jmd_n + tmd_n, 'tmd_c_jmd_c': tmd_c + jmd_c,
                      'ext_n_tmd_n': ext_n + tmd_n, 'tmd_c_ext_c': tmd_c + ext_c}
     return part_seq_dict
 
 
-
-
-
 # II Main functions
 # Caching for data loading for better performance (data loaded ones)
 @lru_cache(maxsize=None)
 def read_excel_cached(name, index_col=None):
     """Load cached dataframe to save loading time"""
     df = pd.read_excel(name, index_col=index_col)
     return df.copy()
@@ -439,15 +435,15 @@
 def plot_get_cmap_(cmap="CPP", n_colors=101, facecolor_dark=None, only_pos=False, only_neg=False):
     """Get colormap for CPP or CPP-SHAP plots"""
     args = dict(n_colors=n_colors, facecolor_dark=facecolor_dark,
                 only_neg=only_neg, only_pos=only_pos)
     if cmap == STR_CMAP_CPP:
         cmap = _get_diverging_cmap("RdBu_r", **args)
     elif cmap == STR_CMAP_SHAP:
-        cmap =  _get_shap_cmap(**args)
+        cmap = _get_shap_cmap(**args)
     else:
         cmap = _get_diverging_cmap(cmap=cmap, **args)
     return cmap
 
 
 # Check df_seq
 def check_df_seq(df_seq=None, accept_none=False):
```

### Comparing `aaanalysis-0.1.4/pyproject.toml` & `aaanalysis-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aaanalysis"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python framework for interpretable protein prediction"
 authors = ["Stephan Breimann <stephanbreimann@gmail.de>"]
 license = "MIT"
 readme = "README.rst"
 include = ["data/*.xlsx", "data/benchmarks/*.tsv", "data/benchmarks/*.xlsx"]
 
 # Add classifiers to provide more details about the package (used by PyPI)
@@ -51,15 +51,15 @@
 Pillow = "^10.0.1"
 pip = "^23.2.01"
 pyparsing = "^3.0.9"
 python-dateutil = "^2.8.2"
 pytz = "^2022.2.1"
 scikit-learn = "^1.4"
 scipy = "^1.10.0"
-seaborn = "^0.11.2"
+seaborn = "^0.13.2"
 six = "^1.16.0"
 statsmodels = "^0.13.2"
 threadpoolctl = "^3.1.0"
 # Optional professional dependencies (via pip install aaanalysis[pro])
 shap = { version = "^0.44.0", optional = true }
 ipython = { version = "^8.16.1", optional = true }
 hypothesis = { version = "^6.86.2", optional = true }
```

### Comparing `aaanalysis-0.1.4/PKG-INFO` & `aaanalysis-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaanalysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python framework for interpretable protein prediction
 License: MIT
 Author: Stephan Breimann
 Author-email: stephanbreimann@gmail.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,15 @@
 Requires-Dist: pip (>=23.2.01,<24.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0) ; extra == "pro"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
 Requires-Dist: scikit-learn (>=1.4,<2.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: shap (>=0.44.0,<0.45.0) ; extra == "pro"
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: threadpoolctl (>=3.1.0,<4.0.0)
 Project-URL: Documentation, https://aaanalysis.readthedocs.io
 Project-URL: Repository, https://github.com/breimanntools/aaanalysis
 Description-Content-Type: text/x-rst
@@ -106,15 +106,15 @@
 
 
 ..
     Missing badges
     |Conda Version|
 
 .. list-table::
-   :widths: 25 75
+   :widths: 20 80
    :header-rows: 1
 
    * - **Package**
      - |PyPI Status| |PyPI Version| |Supported Python Versions| |Downloads| |License|
    * - **Testing**
      - |Unit Tests| |CodeQL| |Codecov| |Documentation Status|
 
@@ -141,21 +141,21 @@
 
 Install
 =======
 **AAanalysis** can be installed from `PyPi <https://pypi.org/project/aaanalysis>`_:
 
 .. code-block:: bash
 
-   pip install -u aaanalysis
+   pip install aaanalysis
 
 For extended features, including our explainable AI module, please use the 'professional' version:
 
 .. code-block:: bash
 
-   pip install -u aaanalysis[pro]
+   pip install aaanalysis[pro]
 
 Contributing
 ============
 We appreciate bug reports, feature requests, or updates on documentation and code. For details, please refer to
 `Contributing Guidelines <CONTRIBUTING.rst>`_. These include specifics about AAanalysis and also notes on Test
 Guided Development (TGD) using ChatGPT. For further questions or suggestions, please email stephanbreimann@gmail.com.
```

