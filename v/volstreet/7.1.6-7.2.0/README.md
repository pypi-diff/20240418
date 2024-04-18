# Comparing `tmp/volstreet-7.1.6.tar.gz` & `tmp/volstreet-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.1.6.tar", last modified: Mon Apr 15 03:33:35 2024, max compression
+gzip compressed data, was "volstreet-7.2.0.tar", last modified: Thu Apr 18 03:26:44 2024, max compression
```

## Comparing `volstreet-7.1.6.tar` & `volstreet-7.2.0.tar`

### file list

```diff
@@ -1,85 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.959763 volstreet-7.1.6/
--rw-rw-rw-   0        0        0     1293 2024-04-15 03:33:35.959763 volstreet-7.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.1.6/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-15 03:33:35.962484 volstreet-7.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.835030 volstreet-7.1.6/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.1.6/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.872396 volstreet-7.1.6/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.1.6/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.1.6/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2600 2024-04-03 08:06:51.000000 volstreet-7.1.6/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    13980 2024-04-06 06:31:33.000000 volstreet-7.1.6/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.1.6/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30608 2024-04-15 03:32:46.000000 volstreet-7.1.6/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.1.6/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.893208 volstreet-7.1.6/volstreet/backtests/
--rw-rw-rw-   0        0        0      157 2024-04-13 05:28:03.000000 volstreet-7.1.6/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.1.6/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    46315 2024-04-13 06:57:57.000000 volstreet-7.1.6/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.1.6/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0      972 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0       66 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/backtests/state.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.1.6/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.1.6/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.1.6/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20783 2024-04-09 13:24:35.000000 volstreet-7.1.6/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6134 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.912993 volstreet-7.1.6/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.1.6/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.1.6/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.1.6/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.1.6/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.1.6/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.915854 volstreet-7.1.6/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18674 2024-04-13 07:50:10.000000 volstreet-7.1.6/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.1.6/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.927567 volstreet-7.1.6/volstreet/strategies/
--rw-rw-rw-   0        0        0      155 2024-04-12 11:13:05.000000 volstreet-7.1.6/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0     5977 2024-04-12 11:27:31.000000 volstreet-7.1.6/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    28633 2024-04-15 03:32:46.000000 volstreet-7.1.6/volstreet/strategies/execution.py
--rw-rw-rw-   0        0        0    56299 2024-04-12 11:27:04.000000 volstreet-7.1.6/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.1.6/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    90364 2024-04-15 03:32:46.000000 volstreet-7.1.6/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.1.6/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.935863 volstreet-7.1.6/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      256 2024-04-03 08:06:51.000000 volstreet-7.1.6/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26301 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    10017 2024-04-12 11:27:04.000000 volstreet-7.1.6/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    11895 2024-04-09 12:18:28.000000 volstreet-7.1.6/volstreet/trade_interface/order_placement.py
--rw-rw-rw-   0        0        0    19897 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.947793 volstreet-7.1.6/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.1.6/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-04-15 03:04:16.000000 volstreet-7.1.6/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.1.6/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.955197 volstreet-7.1.6/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.1.6/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.1.6/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.1.6/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.1.6/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0      599 2024-03-28 11:16:14.000000 volstreet-7.1.6/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:33:35.957901 volstreet-7.1.6/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-15 03:33:35.000000 volstreet-7.1.6/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2473 2024-04-15 03:33:35.000000 volstreet-7.1.6/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:33:35.000000 volstreet-7.1.6/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-15 03:33:35.000000 volstreet-7.1.6/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 03:33:35.000000 volstreet-7.1.6/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.146103 volstreet-7.2.0/
+-rw-rw-rw-   0        0        0     1293 2024-04-18 03:26:44.146103 volstreet-7.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.0/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-18 03:26:44.146103 volstreet-7.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.036402 volstreet-7.2.0/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.0/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.067592 volstreet-7.2.0/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.0/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    17998 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.0/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30608 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.0/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.083283 volstreet-7.2.0/volstreet/backtests/
+-rw-rw-rw-   0        0        0      157 2024-04-13 05:28:03.000000 volstreet-7.2.0/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    46315 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0      972 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0       66 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/backtests/state.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.0/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.0/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20783 2024-04-09 13:24:35.000000 volstreet-7.2.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6134 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.0/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.0/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.0/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18674 2024-04-13 07:50:10.000000 volstreet-7.2.0/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.0/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.101845 volstreet-7.2.0/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.114848 volstreet-7.2.0/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56285 2024-04-18 03:26:14.000000 volstreet-7.2.0/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.0/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    90364 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.0/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26268 2024-04-18 03:26:18.000000 volstreet-7.2.0/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    18789 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    19897 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.0/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-04-17 11:49:46.000000 volstreet-7.2.0/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.2.0/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.0/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.0/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.0/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.0/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:26:44.130476 volstreet-7.2.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2024-04-18 03:26:44.000000 volstreet-7.2.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 03:26:43.000000 volstreet-7.2.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.1.6/PKG-INFO` & `volstreet-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.6
+Version: 7.2.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.6/setup.cfg` & `volstreet-7.2.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 312e 360d 0a61  rsion = 7.1.6..a
+00000020: 7273 696f 6e20 3d20 372e 322e 300d 0a61  rsion = 7.2.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.1.6/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.2.0/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/angel_interface/async_interface.py` & `volstreet-7.2.0/volstreet/angel_interface/async_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from collections import defaultdict
 import functools
 from volstreet.config import token_exchange_dict, logger
 from volstreet.angel_interface.active_session import ActiveSession
+from volstreet.angel_interface.interface import format_quote_response
 
 
 def retry_on_error(func):
     """Only for async functions. Retries the function 5 times with exponential backoff if an error occurs."""
 
     @functools.wraps(func)
     async def async_wrapped(*args, **kwargs):
@@ -47,16 +48,17 @@
             payload[exchange].append(token)
     payload = dict(payload)
     params = {"mode": mode, "exchangeTokens": payload}
     response = await ActiveSession.obj.async_get_quotes(params, session)
 
     # Formatting the response
     response = response["data"]["fetched"]
+    response = format_quote_response(response)
     if return_type.lower() == "dict":
-        return {entry["symbolToken"]: entry for entry in response}
+        return {entry["token"]: entry for entry in response}
     elif return_type.lower() == "list":
         return response
 
 
 @retry_on_error
 async def place_order_async(params: dict, session=None):
     response = await ActiveSession.obj.async_place_order(params, session)
```

### Comparing `volstreet-7.1.6/volstreet/angel_interface/base_websocket.py` & `volstreet-7.2.0/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/angel_interface/interface.py` & `volstreet-7.2.0/volstreet/angel_interface/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import functools
 from datetime import datetime
 import pandas as pd
 from SmartApi.smartExceptions import DataException
 from typing import Callable
 from multiprocessing import Manager, Process
 from volstreet.exceptions import APIFetchError
-from volstreet.utils import current_time
+from volstreet import config
 from volstreet.config import logger, token_exchange_dict, thread_local
 from volstreet.decorators import (
     classproperty,
     timeit,
 )
+from volstreet.utils import current_time, custom_round
 from volstreet.angel_interface.access_rate_handlers import access_rate_handler
 from volstreet.angel_interface.active_session import ActiveSession
 from volstreet.angel_interface.login import wait_for_login
 from volstreet.angel_interface.order_websocket import OrderWebsocket
 from volstreet.angel_interface.price_websocket import PriceWebsocket
 
 
@@ -171,25 +172,122 @@
             return func(*args, **kwargs)
         finally:
             thread_local.robust_handling = False
 
     return wrapper
 
 
+def generate_order_params(
+    symbol: str,
+    token: str,
+    qty: int,
+    action: str,
+    price: float | int,
+    order_tag: str = "",
+    stop_loss_order: bool = False,
+) -> dict:
+    """Price can be a str or a float because "market" is an acceptable value for price."""
+    action = action.upper()
+    order_tag = (
+        "Automated Order" if (order_tag == "" or order_tag is None) else order_tag
+    )
+    exchange = token_exchange_dict[token]
+    params = {
+        "tradingsymbol": symbol,
+        "symboltoken": token,
+        "transactiontype": action,
+        "exchange": exchange,
+        "producttype": "CARRYFORWARD",
+        "duration": "DAY",
+        "quantity": int(qty),
+        "ordertag": order_tag,
+    }
+
+    if stop_loss_order:
+        execution_price = (
+            price * 1.1
+        )  # Hardcoded 10% buffer for execution price in sl orders
+        params.update(
+            {
+                "variety": "STOPLOSS",
+                "ordertype": "STOPLOSS_LIMIT",
+                "triggerprice": round(price, 1),
+                "price": round(execution_price, 1),
+            }
+        )
+    else:
+        order_type, execution_price = (
+            ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
+        )
+        execution_price = custom_round(execution_price)
+        params.update(
+            {
+                "variety": "NORMAL",
+                "ordertype": order_type,
+                "price": max(execution_price, 0.05),
+            }
+        )
+
+    return params
+
+
+def update_order_params(
+    current_params: dict, quote_data: dict, additional_buffer: float = 0
+) -> dict:
+    """Additional buffer is a percentage value that can further modify the price of the order.
+    Additional buffer can be used when iteratively modifying orders to speed up the execution of persistently
+    open orders."""
+
+    action = current_params["transactiontype"]
+    target_price = "best_bid" if action == "SELL" else "best_ask"
+    market_price = quote_data[target_price]
+    modifier = (
+        (1 + config.LIMIT_PRICE_BUFFER + additional_buffer)
+        if action == "BUY"
+        else (1 - config.LIMIT_PRICE_BUFFER - additional_buffer)
+    )
+
+    new_price = market_price * modifier
+    new_price = max(0.05, new_price)
+    new_price = custom_round(new_price)
+
+    modified_params = current_params.copy()
+    modified_params["price"] = new_price
+    current_params["price"] = new_price
+    modified_params.pop("status")
+
+    return modified_params
+
+
 @retry_angel_api(data_type=lambda x: x)
 @access_rate_handler(max_requests=20, per_seconds=1.2)
 @timeit()
-def place_order_params(params: dict) -> str:
+def _place_order_params(params: dict) -> str:
     return ActiveSession.obj.placeOrder(params)
 
 
+def place_order(
+    symbol: str,
+    token: str,
+    qty: int,
+    action: str,
+    price: str | float,
+    order_tag: str = "",
+    stop_loss_order: bool = False,
+) -> str:
+    params = generate_order_params(
+        symbol, token, qty, action, price, order_tag, stop_loss_order
+    )
+    return _place_order_params(params)
+
+
 @retry_angel_api(data_type=lambda x: None)
 @access_rate_handler(max_requests=20, per_seconds=1.2)
 @timeit()
-def modify_order_params(params: dict) -> None:
+def modify_order(params: dict) -> None:
     return ActiveSession.obj.modifyOrder(params)
 
 
 @retry_angel_api(data_type=lambda x: x["data"]["fetched"])
 @access_rate_handler(max_requests=10, per_seconds=1.2)
 @timeit()
 def _fetch_quotes(tokens: list, mode: str = "FULL"):
@@ -199,19 +297,50 @@
         exchange = token_exchange_dict.get(token)
         if exchange:
             payload[exchange].append(token)
     payload = dict(payload)
     return ActiveSession.obj.getMarketData(mode, payload)
 
 
-def fetch_quotes(tokens: list | set, mode: str = "FULL", structure: str = "list"):
-    quote_data = _fetch_quotes(tokens, mode)
+def format_quote_response(response: list) -> list:
+    return [
+        {
+            "token": quote["symbolToken"],
+            "ltp": quote["ltp"],
+            "best_bid": quote["depth"]["buy"][0]["price"],
+            "best_bid_qty": quote["depth"]["buy"][0]["quantity"],
+            "best_ask": quote["depth"]["sell"][0]["price"],
+            "best_ask_qty": quote["depth"]["sell"][0]["quantity"],
+            "timestamp": datetime.strptime(quote["exchFeedTime"], "%d-%b-%Y %H:%M:%S"),
+            "last_traded_datetime": datetime.strptime(
+                quote["exchTradeTime"], "%d-%b-%Y %H:%M:%S"
+            ),
+        }
+        for quote in response
+    ]
+
+
+def fetch_quotes(
+    tokens: list | set,
+    mode: str = "FULL",
+    structure: str = "list",
+    from_source: bool = False,
+):
+    if (
+        not from_source
+        and LiveFeeds.price_feed_connected()
+        and all([token in LiveFeeds.price_feed.data_bank.copy() for token in tokens])
+    ):
+        quote_data = [LiveFeeds.price_feed.data_bank[token] for token in tokens]
+    else:
+        quote_data = _fetch_quotes(tokens, mode)
+        quote_data = format_quote_response(quote_data)
 
     if structure.lower() == "dict":
-        return {entry["symbolToken"]: entry for entry in quote_data}
+        return {entry["token"]: entry for entry in quote_data}
     elif structure.lower() == "list":
         return quote_data
     else:
         raise ValueError(f"Invalid structure '{structure}'.")
 
 
 @retry_angel_api(data_type="ltp")
```

### Comparing `volstreet-7.1.6/volstreet/angel_interface/login.py` & `volstreet-7.2.0/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/angel_interface/order_websocket.py` & `volstreet-7.2.0/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/angel_interface/price_websocket.py` & `volstreet-7.2.0/volstreet/angel_interface/price_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/angel_interface/smart_connect.py` & `volstreet-7.2.0/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/database.py` & `volstreet-7.2.0/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/delta_hedging.py` & `volstreet-7.2.0/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/delta_optimizer.py` & `volstreet-7.2.0/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/framework.py` & `volstreet-7.2.0/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.2.0/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/proxy_functions.py` & `volstreet-7.2.0/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/tools.py` & `volstreet-7.2.0/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/trend.py` & `volstreet-7.2.0/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/backtests/underlying_info.py` & `volstreet-7.2.0/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/blackscholes.py` & `volstreet-7.2.0/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/config.py` & `volstreet-7.2.0/volstreet/config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/database_connection.py` & `volstreet-7.2.0/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/analysis.py` & `volstreet-7.2.0/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/archive.py` & `volstreet-7.2.0/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/data_handling.py` & `volstreet-7.2.0/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/eod_client.py` & `volstreet-7.2.0/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/gambling.py` & `volstreet-7.2.0/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/intraday_data.py` & `volstreet-7.2.0/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/stockmock.py` & `volstreet-7.2.0/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/datamodule/trading_assistance.py` & `volstreet-7.2.0/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/dealingroom.py` & `volstreet-7.2.0/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/decorators.py` & `volstreet-7.2.0/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/discord_bot.py` & `volstreet-7.2.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/exceptions.py` & `volstreet-7.2.0/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.2.0/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/parallelization.py` & `volstreet-7.2.0/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/performance_tracking.py` & `volstreet-7.2.0/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/strategies/error_handling.py` & `volstreet-7.2.0/volstreet/strategies/error_handling.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 )
 from volstreet.angel_interface.interface import (
     fetch_book,
     fetch_quotes,
     lookup_and_return,
 )
 from volstreet.trade_interface import cancel_pending_orders, execute_orders
-from volstreet.strategies.tools import filter_orders_by_strategy
+from volstreet.strategies.monitoring import get_current_state_of_strategy
 
 
 def prepare_exit_params(
     positions: list[dict],
     max_lot_multiplier: int = 30,
     ltp_missing: bool = True,
 ) -> list[dict]:
+    positions = [position for position in positions if position["netqty"]]
     order_params_list = []
     if ltp_missing:
         prices = fetch_quotes(
-            [position["symboltoken"] for position in positions], structure="dict"
+            [position["symboltoken"] for position in positions],
+            structure="dict",
+            from_source=True,
         )
         positions = [
             {**position, "ltp": prices[position["symboltoken"]]["ltp"]}
             for position in positions
         ]
     for position in positions:
         net_qty = int(position["netqty"])
@@ -42,79 +45,41 @@
 
         if net_qty == 0:
             continue
         action = "SELL" if net_qty > 0 else "BUY"
         total_qty = abs(net_qty)
 
         execution_price = (
-            float(position["ltp"]) * 1 - config.LIMIT_PRICE_BUFFER
+            float(position["ltp"]) * (1 - config.LIMIT_PRICE_BUFFER)
             if action == "SELL"
-            else float(position["ltp"]) * 1 + config.LIMIT_PRICE_BUFFER
+            else float(position["ltp"]) * (1 + config.LIMIT_PRICE_BUFFER)
         )
         execution_price = custom_round(execution_price)
 
         while total_qty > 0:
             order_qty = min(total_qty, max_order_qty)
             params = {
-                "symbol": position["tradingsymbol"],
-                "token": position["symboltoken"],
-                "qty": order_qty,
-                "action": action,
-                "price": execution_price,
-                "ordertag": f"Error induced exit",
+                "variety": "NORMAL",
+                "ordertype": "LIMIT",
+                "price": max(execution_price, 0.05),
+                "tradingsymbol": position["tradingsymbol"],
+                "symboltoken": position["symboltoken"],
+                "transactiontype": action,
+                "exchange": config.token_exchange_dict[position["symboltoken"]],
+                "producttype": "CARRYFORWARD",
+                "duration": "DAY",
+                "quantity": int(order_qty),
+                "ordertag": "Error induced exit",
             }
             order_params_list.append(params)
             total_qty -= order_qty
 
     return order_params_list
 
 
-def get_current_state_of_strategy(
-    orderbook: list, index: str, order_tag: str, with_history: bool = False
-) -> list:
-    """
-    Returns the present state of a strategy. This is qty, tokens, and symbols for a given order tag.
-    Active quantity is increased for 'BUY' transactions and decreased for 'SELL' transactions.
-
-    :param orderbook: List of orderbook entries.
-    :param index: The index to search for.
-    :param order_tag: The order tag to search for.
-    :param with_history: If True, returns inactive positions taken earlier as well.
-    :return: A list of dictionaries, each containing the active quantity, symboltoken, and trading symbol.
-    """
-    active_quantities = {}
-    filtered_orders = filter_orders_by_strategy(orderbook, order_tag, index)
-    for order in filtered_orders:
-        symbol = order["tradingsymbol"]
-        filled_shares = (
-            int(order["filledshares"]) * -1
-            if order["transactiontype"] == "SELL"
-            else int(order["filledshares"])
-        )
-
-        if symbol not in active_quantities:
-            active_quantities[symbol] = {
-                "netqty": 0,
-                "symboltoken": order["symboltoken"],
-                "tradingsymbol": symbol,
-                "lotsize": int(order["lotsize"]),
-            }
-
-        active_quantities[symbol]["netqty"] += filled_shares
-
-    if with_history:
-        return [position for position in active_quantities.values()]
-
-    else:
-        active_positions = [
-            position for position in active_quantities.values() if position["netqty"]
-        ]
-        return active_positions
-
-
 @log_error(notify=True, raise_error=True)
 def exit_strategy(strategy: callable, execution_time: datetime, *args, **kwargs):
     sig = signature(strategy)
     bound = sig.bind_partial(*args, **kwargs)
     bound.apply_defaults()
     order_tag = bound.arguments.get("strategy_tag")
     index = bound.arguments.get("underlying").name
@@ -122,19 +87,32 @@
     order_book = filter_orderbook_by_time(order_book, start_time=execution_time)
     pending_orders = lookup_and_return(
         order_book, ["ordertag", "status"], [order_tag, "open"], "orderid"
     )
     if pending_orders:
         cancel_pending_orders(pending_orders, variety="NORMAL")
     active_positions = get_current_state_of_strategy(
-        order_book, index, order_tag, False
+        order_book, index, order_tag, with_pnl=False
     )
-    if not active_positions:
+
+    if active_positions.empty:
+        notifier(
+            f"No positions at all for strategy {strategy.__name__}",
+            webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
+        )
         return
+
+    active_positions = active_positions.to_dict(orient="records")
     exit_params = prepare_exit_params(active_positions, ltp_missing=True)
+    if not exit_params:
+        notifier(
+            f"No ACTIVE positions for strategy {strategy.__name__}",
+            webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
+        )
+        return
     asyncio.run(execute_orders(exit_params))
     user_prefix = config.ERROR_NOTIFICATION_SETTINGS.get("user")
     user_prefix = f"{user_prefix} - " if user_prefix else ""
     notifier(
         f"{user_prefix}Exited positions for strategy {strategy.__name__}",
         webhook_url=config.ERROR_NOTIFICATION_SETTINGS["url"],
         send_whatsapp=True,
```

### Comparing `volstreet-7.1.6/volstreet/strategies/execution.py` & `volstreet-7.2.0/volstreet/strategies/deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 from volstreet import config
 from volstreet.dealingroom import get_strangle_indices_to_trade
 from volstreet.angel_interface.login import login, wait_for_login
 from volstreet.angel_interface.interface import (
     LiveFeeds,
     fetch_book,
     lookup_and_return,
-    modify_order_params,
+    modify_order,
+    update_order_params,
     fetch_quotes,
 )
 from volstreet.angel_interface.active_session import ActiveSession
-from volstreet.trade_interface import Index, update_order_params, order_placement_lock
+from volstreet.trade_interface import Index, order_placement_lock
 from volstreet.strategies.strats import (
     intraday_strangle,
     intraday_trend,
     delta_hedged_strangle,
     overnight_straddle,
     biweekly_straddle,
     buy_weekly_hedge,
@@ -563,15 +564,26 @@
                 order_placement_lock.acquire()
                 order_book = fetch_book("orderbook", from_api=True)
                 if not order_book:
                     continue
                 open_orders = get_open_orders(order_book, statuses=["open"])
 
                 if open_orders.size > 0:
-                    logger.info(f"Modifying open orders at {current_time()}...")
+                    order_descriptions = [
+                        {
+                            "id": order["orderid"],
+                            "symbol": order["tradingsymbol"],
+                            "price": order["price"],
+                        }
+                        for order in open_orders
+                    ]
+                    logger.info(
+                        f"Modifying open orders {order_descriptions} "
+                        f"at {current_time()}"
+                    )
                     modify_orders(open_orders)
             except Exception as e:
                 logger.error(f"Error in continuously handling open orders: {e}")
             # In Python, the "finally" block is guaranteed to be executed regardless of how the try block is exited.
             # This includes situations where the try block is exited due to a return, break, or continue statement,
             # or even if an exception is raised. Hence, the lock gets released in the "finally" block.
             finally:
@@ -646,25 +658,26 @@
         [order_ids, statuses],
         config.modification_fields,
     )
     return open_orders_with_params
 
 
 def modify_orders(open_orders_params: list[dict] | np.ndarray[dict]):
-    ltp_cache = fetch_quotes(
+    quotes = fetch_quotes(
         [order["symboltoken"] for order in open_orders_params],
         structure="dict",
+        from_source=True,
     )
 
     for order in open_orders_params:
-        market_depth = ltp_cache[order["symboltoken"]]["depth"]
-        modified_params = update_order_params(order, market_depth)
+        quote_data = quotes[order["symboltoken"]]
+        modified_params = update_order_params(order, quote_data)
 
         try:
-            modify_order_params(modified_params)
+            modify_order(modified_params)
         except Exception as e:
             if isinstance(e, DataException):
                 logger.error(f"Error in modifying order: {e}")
                 sleep(1)
 
 
 def save_strategy_data(
```

### Comparing `volstreet-7.1.6/volstreet/strategies/helpers.py` & `volstreet-7.2.0/volstreet/strategies/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1038,15 +1038,15 @@
 
     all_quotes = [quote for quotes in all_quotes for quote in quotes]
 
     ltp_cache = {
         option: quote["ltp"]
         for quote in all_quotes
         for option in options
-        if option.token == quote["symbolToken"]
+        if option.token == quote["token"]
     }
 
     return ltp_cache
 
 
 def efficient_ltp_for_strangles(strangles: list[Strangle]) -> dict[Option, float]:
     """
@@ -1426,20 +1426,21 @@
         logger.error(f"Error in filter_out_illiquid_options: {e}", exc_info=True)
         return back_up_illiquid_filter(options, timedelta_minutes)
 
 
 def back_up_illiquid_filter(
     options: list[ActiveOption], timedelta_minutes: float | int = 3
 ):
-    quotes = fetch_quotes([option.token for option in options], structure="dict")
+    quotes = fetch_quotes(
+        [option.token for option in options], structure="dict", from_source=True
+    )
     return [
         option
         for option in options
-        if current_time()
-        - datetime.strptime(quotes[option.token]["exchTradeTime"], "%d-%b-%Y %H:%M:%S")
+        if current_time() - quotes[option.token]["last_traded_datetime"]
         < timedelta(minutes=timedelta_minutes)
     ]
 
 
 def process_stop_loss_order_statuses(
     order_book,
     order_ids,
```

### Comparing `volstreet-7.1.6/volstreet/strategies/optimization.py` & `volstreet-7.2.0/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/strategies/strats.py` & `volstreet-7.2.0/volstreet/strategies/strats.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/trade_interface/instruments.py` & `volstreet-7.2.0/volstreet/trade_interface/instruments.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 from volstreet.utils import (
     get_symbol_token,
     get_lot_size,
     time_to_expiry,
     splice_orders,
 )
 import volstreet.blackscholes as bs
-from volstreet.angel_interface.interface import fetch_ltp
-from volstreet.trade_interface.order_execution import place_order, generate_order_params
+from volstreet.angel_interface.interface import (
+    fetch_ltp,
+    place_order,
+    generate_order_params,
+)
 
 
 class OptionType(Enum):
     CALL = "CE"
     PUT = "PE"
```

### Comparing `volstreet-7.1.6/volstreet/trade_interface/underlyings.py` & `volstreet-7.2.0/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/utils/change_config.py` & `volstreet-7.2.0/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/utils/communication.py` & `volstreet-7.2.0/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/utils/core.py` & `volstreet-7.2.0/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/utils/data_io.py` & `volstreet-7.2.0/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/utils/scrip_processing.py` & `volstreet-7.2.0/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/vectorized_blackscholes.py` & `volstreet-7.2.0/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/vslogging/formatters.py` & `volstreet-7.2.0/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/vslogging/logging_config.json` & `volstreet-7.2.0/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet/vslogging/logging_setup.py` & `volstreet-7.2.0/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.1.6/volstreet.egg-info/PKG-INFO` & `volstreet-7.2.0/volstreet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.1.6
+Version: 7.2.0
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.1.6/volstreet.egg-info/SOURCES.txt` & `volstreet-7.2.0/volstreet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,25 +44,28 @@
 volstreet/datamodule/data_handling.py
 volstreet/datamodule/eod_client.py
 volstreet/datamodule/gambling.py
 volstreet/datamodule/intraday_data.py
 volstreet/datamodule/stockmock.py
 volstreet/datamodule/trading_assistance.py
 volstreet/historical_info/index_expiries.pkl
+volstreet/position_dashboard/__init__.py
+volstreet/position_dashboard/app.py
+volstreet/position_dashboard/formatting.py
 volstreet/strategies/__init__.py
+volstreet/strategies/deployment.py
 volstreet/strategies/error_handling.py
-volstreet/strategies/execution.py
 volstreet/strategies/helpers.py
+volstreet/strategies/monitoring.py
 volstreet/strategies/optimization.py
 volstreet/strategies/strats.py
 volstreet/strategies/tools.py
 volstreet/trade_interface/__init__.py
 volstreet/trade_interface/instruments.py
 volstreet/trade_interface/order_execution.py
-volstreet/trade_interface/order_placement.py
 volstreet/trade_interface/underlyings.py
 volstreet/utils/__init__.py
 volstreet/utils/change_config.py
 volstreet/utils/communication.py
 volstreet/utils/core.py
 volstreet/utils/data_io.py
 volstreet/utils/scrip_processing.py
```

