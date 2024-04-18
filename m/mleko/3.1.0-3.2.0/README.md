# Comparing `tmp/mleko-3.1.0.tar.gz` & `tmp/mleko-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-3.1.0.tar", max compression
+gzip compressed data, was "mleko-3.2.0.tar", max compression
```

## Comparing `mleko-3.1.0.tar` & `mleko-3.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10947 2024-04-12 11:13:42.978676 mleko-3.1.0/LICENSE
--rw-r--r--   0        0        0     4728 2024-04-12 11:13:42.978676 mleko-3.1.0/README.md
--rw-r--r--   0        0        0     1976 2024-04-12 11:14:14.766808 mleko-3.1.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1563 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1333 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/dict_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1360 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1508 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15173 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     6611 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0     1614 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7236 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0     1197 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     6118 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20008 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    12998 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6732 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1612 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4743 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11533 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    18804 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    10745 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3767 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    15426 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4497 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9723 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      874 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     6151 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2994 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2780 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     7816 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     2903 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5744 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3430 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/py.typed
--rw-r--r--   0        0        0      766 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9753 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      743 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1414 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     3641 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-04-12 11:14:14.766808 mleko-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-04-18 20:13:05.988194 mleko-3.2.0/LICENSE
+-rw-r--r--   0        0        0     4728 2024-04-18 20:13:05.988194 mleko-3.2.0/README.md
+-rw-r--r--   0        0        0     1976 2024-04-18 20:13:37.224223 mleko-3.2.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1563 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1222 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1360 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1508 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15173 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     6611 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0     1614 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7236 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0     1197 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     6188 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20008 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    12998 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6732 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1612 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4743 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11533 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    18964 2024-04-18 20:13:05.992194 mleko-3.2.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10756 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3767 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    16740 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4497 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9723 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      874 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     6151 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2994 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2780 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     7816 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     2903 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5744 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3430 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/py.typed
+-rw-r--r--   0        0        0      766 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      743 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1414 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     3641 2024-04-18 20:13:05.996194 mleko-3.2.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-04-18 20:13:37.224223 mleko-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.2.0/PKG-INFO
```

### Comparing `mleko-3.1.0/LICENSE` & `mleko-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/README.md` & `mleko-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/__init__.py` & `mleko-3.2.0/mleko/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
```

### Comparing `mleko-3.1.0/mleko/cache/__init__.py` & `mleko-3.2.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/cache_mixin.py` & `mleko-3.2.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/__init__.py` & `mleko-3.2.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/dict_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/dict_fingerprinter.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 
 from __future__ import annotations
 
 import hashlib
 import json
 from typing import Any
 
-from mleko.utils.custom_logger import CustomLogger
-
 from .base_fingerprinter import BaseFingerprinter
 
 
-logger = CustomLogger()
-"""The logger for the module."""
-
-
 class DictFingerprinter(BaseFingerprinter):
     """Class to generate unique fingerprints for dictionaries."""
 
     def fingerprint(self, data: dict[str, Any] | None) -> str:
         """Generate a fingerprint string for a given dictionary.
 
         Args:
```

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-3.2.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/handlers/__init__.py` & `mleko-3.2.0/mleko/cache/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-3.2.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-3.2.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-3.2.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-3.2.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/cache/lru_cache_mixin.py` & `mleko-3.2.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/__init__.py` & `mleko-3.2.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/convert/base_converter.py` & `mleko-3.2.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-3.2.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/data_schema.py` & `mleko-3.2.0/mleko/dataset/data_schema.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/__init__.py` & `mleko-3.2.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-3.2.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/filter/__init__.py` & `mleko-3.2.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/filter/base_filter.py` & `mleko-3.2.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/filter/expression_filter.py` & `mleko-3.2.0/mleko/dataset/filter/expression_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-3.2.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/ingest/__init__.py` & `mleko-3.2.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/ingest/base_ingester.py` & `mleko-3.2.0/mleko/dataset/ingest/base_ingester.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
     def _write_manifest(self, manifest_data: LocalManifest) -> None:
         """Writes the manifest to the manifest file.
 
         Args:
             manifest_data: Manifest data to write to the manifest file.
         """
+        self._manifest_path.parent.mkdir(parents=True, exist_ok=True)
         with open(self._manifest_path, "w") as manifest_file:
             json.dump(dataclasses.asdict(manifest_data), manifest_file, indent=2)
 
     def _deserialize_manifest(self, manifest_dict: dict) -> LocalManifest:
         """Deserializes the manifest from the manifest dictionary.
 
         Args:
```

### Comparing `mleko-3.1.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-3.2.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-3.2.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/split/__init__.py` & `mleko-3.2.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/split/base_splitter.py` & `mleko-3.2.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/split/expression_splitter.py` & `mleko-3.2.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/split/random_splitter.py` & `mleko-3.2.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/__init__.py` & `mleko-3.2.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/base_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/composite_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-3.2.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/model/base_model.py` & `mleko-3.2.0/mleko/model/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     specified DataFrame and transforms the specified features in the DataFrame.
     """
 
     def __init__(
         self,
         features: list[str] | tuple[str, ...] | None,
         ignore_features: list[str] | tuple[str, ...] | None,
+        verbosity: int,
         memoized_dataset_cache_size: int | None,
         cache_directory: str | Path,
         cache_size: int,
     ) -> None:
         """Initializes the model and ensures the destination directory exists.
 
         Note:
@@ -67,14 +68,15 @@
             clear the cache and free up memory.
 
         Args:
             features: List of feature names to be used by the model. If None, the default is all features
                 applicable to the model.
             ignore_features: List of feature names to be ignored by the model. If None, the default is to
                 ignore no features.
+            verbosity: The verbosity level of the logger, should be passed to the underlying model.
             memoized_dataset_cache_size: The number of datasets to keep in memory for speeding up repeated training.
                 When finished with the fitting and transforming, please call the `_clear_dataset_cache` method to clear
                 the cache and free up memory. Specify 0 to disable the cache.
             cache_directory: Directory where the cache will be stored locally.
             cache_size: The maximum number of entries to keep in the cache.
 
         Raises:
@@ -88,14 +90,15 @@
             logger.error(msg)
             raise ValueError(msg)
 
         self._model = None
         self._hyperparameters: HyperparametersType = {}
         self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
         self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
+        logger.set_level(verbosity)
 
         self._memoized_load_dataset = lru_cache(maxsize=self._memoized_dataset_cache_size)(self._memoized_load_dataset)
 
     def fit(
         self,
         data_schema: DataSchema,
         train_dataframe: vaex.DataFrame,
```

### Comparing `mleko-3.1.0/mleko/model/lgbm_model.py` & `mleko-3.2.0/mleko/model/lgbm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             ...     target="class_",
             ...     model=LGBMClassifier(n_estimators=100),
             ...     random_state=42,
             ...     features=["sepal_width", "petal_length", "petal_width"],
             ... )
             >>> booster, df_train_pred, df_test_pred = model.fit_transform(data_schema, df_train, df_test, {})
         """
-        super().__init__(features, ignore_features, memoized_dataset_cache_size, cache_directory, cache_size)
+        super().__init__(features, ignore_features, verbosity, memoized_dataset_cache_size, cache_directory, cache_size)
         lgb.register_logger(logger)
 
         self._target = target
         self._model = model
         self._eval_metric = eval_metric
         self._log_eval_period = log_eval_period
         self._random_state = random_state
```

### Comparing `mleko-3.1.0/mleko/model/tune/base_tuner.py` & `mleko-3.2.0/mleko/model/tune/base_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/model/tune/optuna_tuner.py` & `mleko-3.2.0/mleko/model/tune/optuna_tuner.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import getpass
 import inspect
 import logging
 import platform
+import random
 from datetime import datetime
 from pathlib import Path
 from typing import Callable, Hashable, Literal
 
 import optuna
 import vaex
 from optuna.samplers import (
@@ -21,22 +22,25 @@
     NSGAIISampler,
     PartialFixedSampler,
     QMCSampler,
     RandomSampler,
     TPESampler,
 )
 from optuna.samplers.nsgaii._child_generation_strategy import NSGAIIChildGenerationStrategy
+from optuna.storages import RDBStorage
 from optuna_dashboard import save_note
 from tqdm.auto import tqdm
 
+from mleko import __version__ as mleko_version
 from mleko.cache.fingerprinters import (
     CallableSourceFingerprinter,
     OptunaPrunerFingerprinter,
     OptunaSamplerFingerprinter,
 )
+from mleko.cache.fingerprinters.dict_fingerprinter import DictFingerprinter
 from mleko.dataset.data_schema import DataSchema
 from mleko.model.base_model import HyperparametersType
 from mleko.utils.custom_logger import CustomLogger
 
 from .base_tuner import BaseTuner
 
 
@@ -64,50 +68,54 @@
         ),
         direction: OptimizeDirection | list[OptimizeDirection],
         num_trials: int,
         cv_folds: Callable[[DataSchema, vaex.DataFrame], list[tuple[vaex.DataFrame, vaex.DataFrame]]] | None = None,
         sampler: BaseSampler | None = None,
         pruner: optuna.pruners.BasePruner | None = None,
         study_name: str | None = None,
-        storage_name: str | None = None,
+        storage: str | RDBStorage | None = None,
+        load_if_exists: bool = False,
         random_state: int | None = 42,
         cache_directory: str | Path = "data/optuna-tuner",
         cache_size: int = 1,
     ) -> None:
         """Initializes a new OptunaTuner instance.
 
         For more information about Optuna, please refer to the documentation:
         https://optuna.readthedocs.io/en/stable/.
 
         Note:
             To visualize the optimization process, you can use the `optuna-dashboard`
-            package. By specifying the `storage_name` parameter, the tuner will save
-            the study to the specified file, which can then be visualized using the
+            library. By specifying the `storage` parameter, the tuner will save
+            the study to the specified file or storage.
+
+            If a sqlite3 file path is defined, the optimization can be visualized using the
             `optuna-dashboard` command:
             ```bash
             optuna-dashboard sqlite:///PATH_TO_YOUR_OPTUNA_STORAGE.sqlite3
             ```
 
             The `study_name` parameter can be used to specify the name of the study,
             which will be displayed in the `optuna-dashboard` interface. If the
             `study_name` is not specified, the current date and time will be used.
+            It is also referred to as the `study_id` in Optuna.
 
         Warning:
-            The caching functionality of the obective function is implemented by
+            The caching functionality of the objective function is implemented by
             serializing the function source code itself. Ensure that all dependencies
             of the objective function are defined within the function itself. Otherwise,
             the dependencies will not be included in the fingerprint of the tuner and
             the results of the hyperparameter tuning will be unpredictable. For example,
-            if the objective function depends on a global variable, the cahing
+            if the objective function depends on a global variable, the caching
             functionality will not detect changes to the value itself and will not
             recompute the result.
 
             In addition, the objective function should preferably not use any cached
             methods, such as `BaseModel.fit_transform`. Instead, the objective
-            function should use the underscored methods (`BaseModell._fit_transform`)
+            function should use the underscored methods (`BaseModel._fit_transform`)
             to avoid caching the results of each trial.
 
         Args:
             objective_function: The objective function to optimize. The function must
                 accept three arguments: the Optuna trial, the data schema, and the
                 DataFrame or CV list of DataFrames to be tuned on. The function must
                 return either a single float value or a list/tuple of float values.
@@ -125,19 +133,22 @@
             sampler: The Optuna sampler to use, if None `TPESampler` is
                 used for single-objective optimization and `NSGAIISampler`
                 is used for multi-objective optimization.
             pruner: The Optuna pruner to use, if None `optuna.pruners.MedianPruner` is
                 used.
             study_name: The name of the study. If None, the current date and time will
                 be used.
-            storage_name: The name of the storage to save the study to. If None, the
-                study will not be saved to disk. Specify the name of the file to save
-                the study to. The file will be saved to the `cache_directory` directory
-                withe the `.sqlite3` extension. E.g. `storage_name="my-study"` will
-                save the study to `cache_directory/my-study.sqlite3`.
+            storage: The name of the storage to save the study to. If None, the
+                study will not be saved to a persistent storage. Refer to the Optuna
+                documentation for more information on the storage options.
+            load_if_exists: Flag to control the behavior to handle a conflict of study
+                names. In the case where a study named `study_name` already exists in
+                the storage, a `DuplicatedStudyError` is raised if `load_if_exists`
+                is set to `False`. Otherwise, the creation of the study is
+                skipped, and the existing one is returned.
             random_state: The random state to use for the Optuna sampler. If None, the
                 default random state of the sampler is used. Setting this will override
                 the random state of the sampler.
             cache_directory: The target directory where the output is to be saved.
             cache_size: The maximum number of cache entries.
 
         Examples:
@@ -179,100 +190,98 @@
         self._objective_function = objective_function
         self._direction = direction
         self._num_trials = num_trials
         self._cv_folds = cv_folds
         self._sampler = sampler or (TPESampler() if isinstance(direction, list) else NSGAIISampler())
         self._pruner = pruner or optuna.pruners.MedianPruner()
         self._study_name = study_name if study_name is not None else datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        self._storage_name = (
-            f"sqlite:///{self._cache_directory}/{storage_name}.sqlite3" if storage_name is not None else None
-        )
-        self._using_optuna_dashboard = True if self._storage_name is not None else False
+        self._storage = storage
+        self._load_if_exists = load_if_exists
+        self._using_optuna_dashboard = True if self._storage is not None else False
         self._random_state = random_state
 
         self._reset_sampler_rng(self._sampler)
 
         optuna_logger = logging.getLogger("optuna")
         for handler in optuna_logger.handlers:
             optuna_logger.removeHandler(handler)
         for handler in logger.handlers:
             optuna_logger.addHandler(handler)
 
-        if self._storage_name is not None:
-            logger.info(f"Optuna study is saved to {self._storage_name}, use optuna-dashboard to visualize it.")
+        if self._storage is not None:
+            storage_name = self._storage if isinstance(self._storage, str) else self._storage.url
+            logger.info(
+                f"Optuna study named {self._study_name!r} is stored in {storage_name}, use optuna-dashboard to view it."
+            )
 
     def _tune(
         self, data_schema: DataSchema, dataframe: vaex.DataFrame
     ) -> tuple[HyperparametersType, float | list[float] | tuple[float, ...], optuna.study.Study]:
         """Perform the hyperparameter tuning.
 
         Args:
             data_schema: Data schema for the DataFrame.
             dataframe: DataFrame to be tuned on.
 
         Returns:
             Tuple containing the best hyperparameters, the best score, and a the Optuna study.
         """
         self._reset_sampler_rng(self._sampler)
-
-        if isinstance(self._direction, list):
-            study = optuna.create_study(
-                sampler=self._sampler,
-                pruner=self._pruner,
-                directions=self._direction,
-                study_name=self._study_name,
-                storage=self._storage_name,
-            )
-        else:
-            study = optuna.create_study(
-                sampler=self._sampler,
-                pruner=self._pruner,
-                direction=self._direction,
-                study_name=self._study_name,
-                storage=self._storage_name,
-            )
-
+        study = optuna.create_study(
+            storage=self._storage,
+            sampler=self._sampler,
+            pruner=self._pruner,
+            study_name=self._study_name,
+            direction=self._direction if isinstance(self._direction, str) else None,
+            directions=self._direction if isinstance(self._direction, list) else None,
+            load_if_exists=self._load_if_exists,
+        )
         if self._using_optuna_dashboard:
             direction_str = (
                 self._direction if isinstance(self._direction, str) else ", ".join(self._direction)
             ).upper()
             save_note(
                 study,
                 f"""# Experiment Documentation
 
 ## Overview
 | | |
 |---|---|
 | **Study Name** | {self._study_name} |
+| **Load If Exists** | `{self._load_if_exists}` |
 | **Creation Date** | {datetime.now().strftime("%Y-%m-%d %H:%M:%S")} |
 | **Creator** | {getpass.getuser()} |
 ---
 
 ## Methodology
 
 ### Experimental Setup
 
 | | |
 |---|---|
 | **Python Version** | `{platform.python_version()}` |
 | **Optuna Version** | `{optuna.__version__}` |
+| **Mleko Version** | `{mleko_version}` |
 | **Random State** | `{self._random_state}` |
-| **Number of Trials** | `{self._num_trials}` |
 | **Sampler** | `{self._sampler.__class__.__name__}` |
 | **Pruner** | `{self._pruner.__class__.__name__}` |
 | **Optimization Direction** | {direction_str} |
 
 ## Notes
 > _Add any additional notes about the experiment here._
 
 ## Appendix
 ### Objective Function
 ```python
 {inspect.getsource(self._objective_function)}
 ```
+{"### Cross-Validation Folds Function" if self._cv_folds is not None else ""}
+{"```python" if self._cv_folds is not None else ""}
+{inspect.getsource(self._cv_folds) if self._cv_folds is not None else ""}
+{"```" if self._cv_folds is not None else ""}
                 """,
             )
 
         with tqdm(total=self._num_trials) as pbar:
 
             def tqdm_callback(study: optuna.study.Study, _trial: optuna.trial.FrozenTrial) -> None:
                 pbar.update(1)
@@ -312,24 +321,37 @@
 
     def _fingerprint(self) -> Hashable:
         """Generates a fingerprint for the tuner.
 
         Returns:
             The fingerprint of the tuner.
         """
+        if self._load_if_exists and self._storage is not None:  # pragma: no cover
+            logger.warning("The load_if_exists parameter is set to True, the caching functionality will be disabled.")
+            return random.random()
+
         return (
             super()._fingerprint(),
             CallableSourceFingerprinter().fingerprint(self._objective_function),
             self._direction,
             self._num_trials,
             CallableSourceFingerprinter().fingerprint(self._cv_folds) if self._cv_folds is not None else None,
             OptunaSamplerFingerprinter().fingerprint(self._sampler),
             OptunaPrunerFingerprinter().fingerprint(self._pruner),
             self._random_state,
-            self._storage_name,
+            (
+                self._storage
+                if isinstance(self._storage, str)
+                else (
+                    self._storage.url + DictFingerprinter().fingerprint(self._storage.engine_kwargs)
+                    if self._storage is not None
+                    else None
+                )
+            ),
+            self._load_if_exists,
         )
 
     def _reset_sampler_rng(self, sampler: BaseSampler) -> None:
         """Resets the random number generator of the given Optuna sampler.
 
         Args:
             sampler: The Optuna sampler to reset the random number generator of.
```

### Comparing `mleko-3.1.0/mleko/pipeline/__init__.py` & `mleko-3.2.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/data_container.py` & `mleko-3.2.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/pipeline.py` & `mleko-3.2.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/pipeline_step.py` & `mleko-3.2.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/__init__.py` & `mleko-3.2.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/convert_step.py` & `mleko-3.2.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-3.2.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/filter_step.py` & `mleko-3.2.0/mleko/pipeline/steps/filter_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/ingest_step.py` & `mleko-3.2.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/model_step.py` & `mleko-3.2.0/mleko/pipeline/steps/model_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/split_step.py` & `mleko-3.2.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/transform_step.py` & `mleko-3.2.0/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/pipeline/steps/tune_step.py` & `mleko-3.2.0/mleko/pipeline/steps/tune_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/__init__.py` & `mleko-3.2.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/custom_logger.py` & `mleko-3.2.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/decorators.py` & `mleko-3.2.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/file_helpers.py` & `mleko-3.2.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/tqdm_helpers.py` & `mleko-3.2.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/mleko/utils/vaex_helpers.py` & `mleko-3.2.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.1.0/pyproject.toml` & `mleko-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "3.1.0"
+version = "3.2.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-3.1.0/PKG-INFO` & `mleko-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 3.1.0
+Version: 3.2.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
```

