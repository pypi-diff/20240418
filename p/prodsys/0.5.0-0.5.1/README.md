# Comparing `tmp/prodsys-0.5.0.tar.gz` & `tmp/prodsys-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.5.0.tar", max compression
+gzip compressed data, was "prodsys-0.5.1.tar", max compression
```

## Comparing `prodsys-0.5.0.tar` & `prodsys-0.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.5.0/LICENSE
--rw-r--r--   0        0        0      405 2024-04-14 17:14:53.846311 prodsys-0.5.0/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-01-07 23:00:16.870495 prodsys-0.5.0/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    51413 2024-04-14 17:14:53.846311 prodsys-0.5.0/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8314 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9028 2023-12-24 15:55:37.172880 prodsys-0.5.0/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2138 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/express/core.py
--rw-r--r--   0        0        0     6525 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/process.py
--rw-r--r--   0        0        0     2435 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/product.py
--rw-r--r--   0        0        0     6508 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8275 2024-04-07 17:13:56.260662 prodsys-0.5.0/prodsys/express/resources.py
--rw-r--r--   0        0        0     2558 2024-02-27 21:06:20.429295 prodsys-0.5.0/prodsys/express/sink.py
--rw-r--r--   0        0        0     3454 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/express/state.py
--rw-r--r--   0        0        0     4895 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3439 2024-04-07 17:13:56.261200 prodsys-0.5.0/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.5.0/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.5.0/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    10419 2024-04-12 11:17:17.974120 prodsys-0.5.0/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.5.0/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1436 2024-04-07 17:13:56.263212 prodsys-0.5.0/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     2971 2024-02-27 19:26:17.985971 prodsys-0.5.0/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0    11648 2024-04-14 17:14:53.855074 prodsys-0.5.0/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     6357 2024-04-14 17:14:53.857017 prodsys-0.5.0/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1931 2024-04-14 17:14:53.857017 prodsys-0.5.0/prodsys/models/queue_data.py
--rw-r--r--   0        0        0    12337 2024-04-14 17:14:53.862626 prodsys-0.5.0/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10730 2024-04-12 11:17:17.974120 prodsys-0.5.0/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     2846 2024-04-14 17:14:53.863598 prodsys-0.5.0/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     4059 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/source_data.py
--rw-r--r--   0        0        0    13852 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/state_data.py
--rw-r--r--   0        0        0     6642 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12476 2024-04-14 17:14:53.871089 prodsys-0.5.0/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28223 2024-04-14 17:14:53.874200 prodsys-0.5.0/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4640 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46564 2024-04-14 17:14:53.874200 prodsys-0.5.0/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9396 2024-04-14 17:14:53.879309 prodsys-0.5.0/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11646 2024-04-14 17:14:53.880630 prodsys-0.5.0/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    27915 2024-04-12 11:17:17.986645 prodsys-0.5.0/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/simulation/logger.py
--rw-r--r--   0        0        0     3763 2024-01-07 23:00:16.907148 prodsys-0.5.0/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9601 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0     9097 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/process.py
--rw-r--r--   0        0        0    11882 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/product.py
--rw-r--r--   0        0        0     4004 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/request.py
--rw-r--r--   0        0        0    17837 2024-04-12 11:17:17.986645 prodsys-0.5.0/prodsys/simulation/resources.py
--rw-r--r--   0        0        0     9574 2024-04-12 11:17:17.989996 prodsys-0.5.0/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     2260 2024-04-12 11:17:17.990877 prodsys-0.5.0/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     3809 2024-04-12 11:17:17.990877 prodsys-0.5.0/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29184 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.5.0/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7193 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.5.0/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30298 2023-12-24 15:40:41.082915 prodsys-0.5.0/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12118 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.5.0/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4260 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/util/util.py
--rw-r--r--   0        0        0     1313 2024-04-14 17:14:53.888155 prodsys-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6238 2023-10-11 11:05:21.946526 prodsys-0.5.0/README.md
--rw-r--r--   0        0        0     8509 1970-01-01 00:00:00.000000 prodsys-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.5.1/LICENSE
+-rw-r--r--   0        0        0      405 2024-04-18 15:23:00.783172 prodsys-0.5.1/prodsys/__init__.py
+-rw-r--r--   0        0        0     1289 2024-01-07 23:00:16.870495 prodsys-0.5.1/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    51413 2024-04-14 17:14:53.846311 prodsys-0.5.1/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8314 2024-04-07 17:13:56.244883 prodsys-0.5.1/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.5.1/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.5.1/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.5.1/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.5.1/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9028 2023-12-24 15:55:37.172880 prodsys-0.5.1/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.5.1/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2138 2024-04-07 17:13:56.244883 prodsys-0.5.1/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.5.1/prodsys/express/core.py
+-rw-r--r--   0        0        0     6525 2024-04-07 17:13:56.244883 prodsys-0.5.1/prodsys/express/process.py
+-rw-r--r--   0        0        0     2435 2024-04-07 17:13:56.244883 prodsys-0.5.1/prodsys/express/product.py
+-rw-r--r--   0        0        0     6508 2024-04-07 17:13:56.244883 prodsys-0.5.1/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8275 2024-04-07 17:13:56.260662 prodsys-0.5.1/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2558 2024-02-27 21:06:20.429295 prodsys-0.5.1/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3454 2024-01-07 23:00:16.874004 prodsys-0.5.1/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/express/state.py
+-rw-r--r--   0        0        0     4895 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-07 17:13:56.261200 prodsys-0.5.1/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.5.1/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.5.1/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    10419 2024-04-12 11:17:17.974120 prodsys-0.5.1/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.5.1/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1436 2024-04-07 17:13:56.263212 prodsys-0.5.1/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     2971 2024-02-27 19:26:17.985971 prodsys-0.5.1/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2023-10-11 11:05:22.089564 prodsys-0.5.1/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    11648 2024-04-14 17:14:53.855074 prodsys-0.5.1/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6357 2024-04-14 17:14:53.857017 prodsys-0.5.1/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1931 2024-04-14 17:14:53.857017 prodsys-0.5.1/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12337 2024-04-14 17:14:53.862626 prodsys-0.5.1/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10730 2024-04-12 11:17:17.974120 prodsys-0.5.1/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2846 2024-04-14 17:14:53.863598 prodsys-0.5.1/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     4059 2024-04-14 17:14:53.865574 prodsys-0.5.1/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13852 2024-04-14 17:14:53.865574 prodsys-0.5.1/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     6642 2024-04-14 17:14:53.865574 prodsys-0.5.1/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.5.1/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12476 2024-04-14 17:14:53.871089 prodsys-0.5.1/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28223 2024-04-14 17:14:53.874200 prodsys-0.5.1/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4642 2024-04-18 14:45:11.231208 prodsys-0.5.1/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46428 2024-04-18 09:38:08.351215 prodsys-0.5.1/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9577 2024-04-18 14:47:16.673364 prodsys-0.5.1/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11871 2024-04-18 14:51:26.265202 prodsys-0.5.1/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.5.1/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    27915 2024-04-12 11:17:17.986645 prodsys-0.5.1/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2023-10-11 11:05:22.105207 prodsys-0.5.1/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0     3763 2024-01-07 23:00:16.907148 prodsys-0.5.1/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9601 2024-04-07 17:13:56.267724 prodsys-0.5.1/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0     9097 2024-04-07 17:13:56.267724 prodsys-0.5.1/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    11882 2024-04-07 17:13:56.267724 prodsys-0.5.1/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     4004 2024-04-07 17:13:56.267724 prodsys-0.5.1/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    17837 2024-04-12 11:17:17.986645 prodsys-0.5.1/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0     9574 2024-04-12 11:17:17.989996 prodsys-0.5.1/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3199 2023-10-11 11:05:22.120833 prodsys-0.5.1/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2260 2024-04-12 11:17:17.990877 prodsys-0.5.1/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     3809 2024-04-12 11:17:17.990877 prodsys-0.5.1/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29184 2024-04-07 17:13:56.277897 prodsys-0.5.1/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.5.1/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7193 2024-04-07 17:13:56.277897 prodsys-0.5.1/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.5.1/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.5.1/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30298 2023-12-24 15:40:41.082915 prodsys-0.5.1/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12118 2024-04-07 17:13:56.277897 prodsys-0.5.1/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.5.1/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4379 2024-04-18 15:06:57.609972 prodsys-0.5.1/prodsys/util/util.py
+-rw-r--r--   0        0        0     1313 2024-04-18 15:22:58.531950 prodsys-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6318 2024-04-18 15:22:16.750446 prodsys-0.5.1/README.md
+-rw-r--r--   0        0        0     8587 1970-01-01 00:00:00.000000 prodsys-0.5.1/PKG-INFO
```

### Comparing `prodsys-0.5.0/LICENSE` & `prodsys-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/adapters/__init__.py` & `prodsys-0.5.1/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/adapters/adapter.py` & `prodsys-0.5.1/prodsys/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/adapters/json_adapter.py` & `prodsys-0.5.1/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/conf/logging.ini` & `prodsys-0.5.1/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/conf/logging_config.py` & `prodsys-0.5.1/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/control/routing_control_env.py` & `prodsys-0.5.1/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/control/sequencing_control_env.py` & `prodsys-0.5.1/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/__init__.py` & `prodsys-0.5.1/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/core.py` & `prodsys-0.5.1/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/process.py` & `prodsys-0.5.1/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/product.py` & `prodsys-0.5.1/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/production_system.py` & `prodsys-0.5.1/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/resources.py` & `prodsys-0.5.1/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/sink.py` & `prodsys-0.5.1/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/source.py` & `prodsys-0.5.1/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/state.py` & `prodsys-0.5.1/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/express/time_model.py` & `prodsys-0.5.1/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/__init__.py` & `prodsys-0.5.1/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/process_factory.py` & `prodsys-0.5.1/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/product_factory.py` & `prodsys-0.5.1/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/queue_factory.py` & `prodsys-0.5.1/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/resource_factory.py` & `prodsys-0.5.1/prodsys/factories/resource_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/sink_factory.py` & `prodsys-0.5.1/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/source_factory.py` & `prodsys-0.5.1/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/state_factory.py` & `prodsys-0.5.1/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/factories/time_model_factory.py` & `prodsys-0.5.1/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/__init__.py` & `prodsys-0.5.1/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/core_asset.py` & `prodsys-0.5.1/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/performance_data.py` & `prodsys-0.5.1/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/performance_indicators.py` & `prodsys-0.5.1/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/processes_data.py` & `prodsys-0.5.1/prodsys/models/processes_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/product_data.py` & `prodsys-0.5.1/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/queue_data.py` & `prodsys-0.5.1/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/resource_data.py` & `prodsys-0.5.1/prodsys/models/resource_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/scenario_data.py` & `prodsys-0.5.1/prodsys/models/scenario_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/sink_data.py` & `prodsys-0.5.1/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/source_data.py` & `prodsys-0.5.1/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/state_data.py` & `prodsys-0.5.1/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/models/time_model_data.py` & `prodsys-0.5.1/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/optimization/__init__.py` & `prodsys-0.5.1/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.5.1/prodsys/optimization/evolutionary_algorithm.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/optimization/math_opt.py` & `prodsys-0.5.1/prodsys/optimization/math_opt.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/optimization/optimization_analysis.py` & `prodsys-0.5.1/prodsys/optimization/optimization_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import pandas as pd
 from typing import List
 import json
 import plotly
 import plotly.graph_objects as go
 import numpy as np
 from copy import copy
```

### Comparing `prodsys-0.5.0/prodsys/optimization/optimization_util.py` & `prodsys-0.5.1/prodsys/optimization/optimization_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,18 +209,17 @@
     Returns:
         Tuple[float, ...]: Tuple of weights for the objectives.
     """
     weights = []
     for objective in adapter.scenario_data.objectives:
         kpi = parse_obj_as(performance_indicators.KPI_UNION, {"name": objective.name})
         if kpi.target != direction:
-            objective.weight *= -1
-        # if direction == "min":
-        #     objective.weight *= -1
-        weights.append(objective.weight)
+            weights.append(objective.weight * -1)
+        else:
+            weights.append(objective.weight)
     return tuple(weights)
 
 
 def crossover(ind1, ind2):
     ind1[0].ID = str(uuid1())
     ind2[0].ID = str(uuid1())
 
@@ -1051,16 +1050,15 @@
     if adapter_object_hash in solution_dict["hashes"]:
         evaluated_adapter_generation = solution_dict["hashes"][adapter_object_hash]["generation"]
         evaluated_adapter_id = solution_dict["hashes"][adapter_object_hash]["ID"]
         print(f"{adapter_object.ID}: adapter with equal hash already evaluated. Returning fitness of generation {evaluated_adapter_generation} and ID {evaluated_adapter_id}.")
         return performances[evaluated_adapter_generation][evaluated_adapter_id]["fitness"]
 
     if not check_valid_configuration(adapter_object, base_scenario):
-        # FIXME: check if this function is always correct, either max or min for all algorithms?
-        return [-100000 * weight for weight in get_weights(base_scenario, "max")]
+        return [-100000 / weight for weight in get_weights(base_scenario, "max")]
 
     fitness_values = []
 
     for seed in range(number_of_seeds):
         runner_object = runner.Runner(adapter=adapter_object) 
         if not adapter_object.scenario_data.info.time_range:
             raise ValueError("time_range is not defined in scenario_data")
```

### Comparing `prodsys-0.5.0/prodsys/optimization/simulated_annealing.py` & `prodsys-0.5.1/prodsys/optimization/simulated_annealing.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         performance = sum(
             [value * weight for value, weight in zip(values, self.weights)]
         )
         # print("\n\t########## Evaluted ind", self.counter, "for value:", performance)
         counter = len(self.performances["0"]) - 1
         document_individual(self.solution_dict, self.save_folder, [self.state])
-        self.performances["0"][str(counter)] = {
+        self.performances["0"][self.state.ID] = {
             "agg_fitness": performance,
             "fitness": [float(value) for value in values],
             "time_stamp": time.perf_counter() - self.start,
             "hash": self.state.hash(),
         }
         with open(f"{self.save_folder}/optimization_results.json", "w") as json_file:
             json.dump(self.performances, json_file)
@@ -145,18 +145,22 @@
         steps (int): Steps for annealing
         updates (int): Number of updates
         number_of_seeds (int): Number of seeds for optimization
         initial_solution_file_path (str, optional): File path to an initial solution. Defaults to "".
     """
     base_configuration = adapters.JsonProductionSystemAdapter()
     base_configuration.read_data(base_configuration_file_path, scenario_file_path)
+    if not base_configuration.ID:
+        base_configuration.ID = "base_configuration"
 
     if initial_solution_file_path:
         initial_solution = adapters.JsonProductionSystemAdapter()
         initial_solution.read_data(initial_solution_file_path, scenario_file_path)
+        if not initial_solution.ID:
+            initial_solution.ID = "initial_solution"
     else:
         initial_solution = base_configuration.copy(deep=True)
 
     hyper_parameters = SimulatedAnnealingHyperparameters(
         seed=seed, Tmax=Tmax, Tmin=Tmin, steps=steps, updates=updates, number_of_seeds=number_of_seeds)
 
     simulated_annealing_optimization(
```

### Comparing `prodsys-0.5.0/prodsys/optimization/tabu_search.py` & `prodsys-0.5.1/prodsys/optimization/tabu_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,18 +190,22 @@
         max_steps (int): Maximum number of steps.
         max_score (int): Maximum score to stop optimization.
         number_of_seeds (int, optional): Number of seeds for optimization. Defaults to 1.
         initial_solution_file_path (str, optional): File path to an initial solution. Defaults to "".
     """
     base_configuration = adapters.JsonProductionSystemAdapter()
     base_configuration.read_data(base_configuration_file_path, scenario_file_path)
+    if not base_configuration.ID:
+        base_configuration.ID = "base_configuration"
 
     if initial_solution_file_path:
         initial_solution = adapters.JsonProductionSystemAdapter()
         initial_solution.read_data(initial_solution_file_path, scenario_file_path)
+        if not initial_solution.ID:
+            initial_solution.ID = "initial_solution"
     else:
         initial_solution = base_configuration.copy(deep=True)
 
     hyper_parameters = TabuSearchHyperparameters(
         seed=seed, tabu_size=tabu_size, max_steps=max_steps, max_score=max_score, number_of_seeds=number_of_seeds
     )
     tabu_search_optimization(
@@ -262,15 +266,15 @@
             performance = sum(
                 [value * weight for value, weight in zip(values, weights)]
             )
             counter = len(performances["0"]) - 1
             print(counter, performance)
             document_individual(solution_dict, save_folder, [state])
 
-            performances["0"][str(counter)] = {
+            performances["0"][state.ID] = {
                 "agg_fitness": performance,
                 "fitness": [float(value) for value in values],
                 "time_stamp": time.perf_counter() - start,
                 "hash": state.hash()
             }
             with open(f"{save_folder}/optimization_results.json", "w") as json_file:
                 json.dump(performances, json_file)
@@ -293,15 +297,15 @@
     alg = Algorithm(
         initial_state=initial_solution,
         tabu_size=hyper_parameters.tabu_size,
         max_steps=hyper_parameters.max_steps,
         max_score=hyper_parameters.max_score,
     )
     best_solution, best_objective_value = alg.run()
-    print("Best solution: ", best_objective_value)
+    print(f"Best solution has ID {best_solution.ID} and objectives values: {best_objective_value}")
 
 
 
 def optimize_configuration(
     base_configuration_file_path: str,
     scenario_file_path: str,
     save_folder: str,
```

### Comparing `prodsys-0.5.0/prodsys/simulation/__init__.py` & `prodsys-0.5.1/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/control.py` & `prodsys-0.5.1/prodsys/simulation/control.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/logger.py` & `prodsys-0.5.1/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/observer.py` & `prodsys-0.5.1/prodsys/simulation/observer.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/proces_models.py` & `prodsys-0.5.1/prodsys/simulation/proces_models.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/process.py` & `prodsys-0.5.1/prodsys/simulation/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/product.py` & `prodsys-0.5.1/prodsys/simulation/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/request.py` & `prodsys-0.5.1/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/resources.py` & `prodsys-0.5.1/prodsys/simulation/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/router.py` & `prodsys-0.5.1/prodsys/simulation/router.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/sim.py` & `prodsys-0.5.1/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/sink.py` & `prodsys-0.5.1/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/source.py` & `prodsys-0.5.1/prodsys/simulation/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/state.py` & `prodsys-0.5.1/prodsys/simulation/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/store.py` & `prodsys-0.5.1/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/simulation/time_model.py` & `prodsys-0.5.1/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/util/kpi_visualization.py` & `prodsys-0.5.1/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/util/post_processing.py` & `prodsys-0.5.1/prodsys/util/post_processing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/util/runner.py` & `prodsys-0.5.1/prodsys/util/runner.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/util/statistical_functions.py` & `prodsys-0.5.1/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.0/prodsys/util/util.py` & `prodsys-0.5.1/prodsys/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,22 @@
         base_configuration (adapters.ProductionSystemAdapter): The base configuration for optimization containing the scenario data.
 
     Returns:
         List[adapters.ProductionSystemAdapter]: List of adapters of the initial solutions.
     """
     file_paths = [f for f in listdir(folder_path) if isfile(join(folder_path, f))]
     adapter_objects = []
-    for file_path in file_paths:
+    for counter, file_path in enumerate(file_paths):
         if ".json" not in file_path or file_path == "optimization_results.json":
             continue
         adapter = adapters.JsonProductionSystemAdapter()
         adapter.read_data(join(folder_path, file_path))
         adapter.scenario_data = base_configuration.scenario_data.copy()
+        if not adapter.ID:
+            adapter.ID = f"initial_solution_{counter}"
         adapter_objects.append(adapter)
     return adapter_objects
 
 def get_initial_solution_file_pth(
         folder_path: str
 ) -> str:
     """
@@ -123,15 +125,15 @@
     """
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from flatten(x)
         else:
             yield x
 
-def flatten_object(xs: list) -> list:
+def flatten_object(xs: list) -> list: # type: ignore
     """
     Flattens a nested list.
 
     Args:
         xs (list): The nested list.
 
     Yields:
```

### Comparing `prodsys-0.5.0/pyproject.toml` & `prodsys-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.5.0"
+version = "0.5.1"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `prodsys-0.5.0/README.md` & `prodsys-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# prodsys - modeling, simulating and optimizing production systems
+![Alt text](./resources/logo.svg)
+
+*prodsys - modeling, simulating and optimizing production systems*
 
 ![Build-sucess](https://img.shields.io/badge/build-success-green)
 ![PyPI](https://img.shields.io/pypi/v/prodsys)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
 ![Docu](https://img.shields.io/badge/docu-full-green)
 
-prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
+prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. For more information, have a look at the [documentation](https://sdm4fzi.github.io/prodsys/).
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
 ```
 
-Please note that the package is only compatible with Python 3.11 or higher.
+Please note that prodsys is currently only fully compatible with Python 3.11. Other versions might cause some errors.
 
 ## Getting started
 
 The package is designed to be easy to use. The following example shows how to model a simple production system and simulate it. The production system contains a single milling machine that performs milling processes on aluminium housings. The transport is thereby performed by a worker.  At first, just import the express API of `prodsys`:
 
 ```python
 import prodsys.express as psx
```

### Comparing `prodsys-0.5.0/PKG-INFO` & `prodsys-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.5.0
+Version: 0.5.1
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,32 +28,34 @@
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchaudio (>=2.0.2,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Requires-Dist: tqdm (>=4.65,<5.0)
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
-# prodsys - modeling, simulating and optimizing production systems
+![Alt text](./resources/logo.svg)
+
+*prodsys - modeling, simulating and optimizing production systems*
 
 ![Build-sucess](https://img.shields.io/badge/build-success-green)
 ![PyPI](https://img.shields.io/pypi/v/prodsys)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prodsys)
 ![Docu](https://img.shields.io/badge/docu-full-green)
 
-prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. Have a look at the [documentation](https://sdm4fzi.github.io/prodsys/) for more information.
+prodsys is a python package for modeling, simulating and optimizing production systems based on the product, process and resource (PPR) modelling principle. For more information, have a look at the [documentation](https://sdm4fzi.github.io/prodsys/).
 
 ## Installation
 
 To install the package, run the following command in the terminal:
 
 ```bash
 pip install prodsys
 ```
 
-Please note that the package is only compatible with Python 3.11 or higher.
+Please note that prodsys is currently only fully compatible with Python 3.11. Other versions might cause some errors.
 
 ## Getting started
 
 The package is designed to be easy to use. The following example shows how to model a simple production system and simulate it. The production system contains a single milling machine that performs milling processes on aluminium housings. The transport is thereby performed by a worker.  At first, just import the express API of `prodsys`:
 
 ```python
 import prodsys.express as psx
```

