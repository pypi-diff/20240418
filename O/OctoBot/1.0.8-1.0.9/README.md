# Comparing `tmp/OctoBot-1.0.8.tar.gz` & `tmp/OctoBot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-1.0.8.tar", last modified: Fri Feb 16 10:02:56 2024, max compression
+gzip compressed data, was "OctoBot-1.0.9.tar", last modified: Thu Apr 18 07:16:04 2024, max compression
```

## Comparing `OctoBot-1.0.8.tar` & `OctoBot-1.0.9.tar`

### file list

```diff
@@ -1,203 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.803684 OctoBot-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    64685 2024-02-16 10:01:43.000000 OctoBot-1.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-02-16 10:01:43.000000 OctoBot-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-16 10:01:43.000000 OctoBot-1.0.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/OctoBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-16 10:02:56.000000 OctoBot-1.0.8/OctoBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-02-16 10:02:56.803684 OctoBot-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13337 2024-02-16 10:01:43.000000 OctoBot-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.739683 OctoBot-1.0.8/octobot/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.739683 OctoBot-1.0.8/octobot/api/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/api/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/api/strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.739683 OctoBot-1.0.8/octobot/automation/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/automation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.743683 OctoBot-1.0.8/octobot/automation/bases/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/bases/abstract_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/bases/abstract_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/bases/abstract_trigger_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-16 10:01:43.000000 OctoBot-1.0.8/octobot/automation/bases/automation_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.743683 OctoBot-1.0.8/octobot/backtesting/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/backtesting/abstract_backtesting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/backtesting/independent_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/backtesting/octobot_backtesting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.743683 OctoBot-1.0.8/octobot/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/channels/octobot_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.743683 OctoBot-1.0.8/octobot/community/
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26243 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/community_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/community_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.747683 OctoBot-1.0.8/octobot/community/errors_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors_upload/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors_upload/errors_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors_upload/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/errors_upload/sentry_aiohttp_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.747683 OctoBot-1.0.8/octobot/community/feeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/feeds/abstract_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/feeds/community_supabase_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/feeds/community_ws_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/feeds/feed_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/graphql_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/identifiers_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.747683 OctoBot-1.0.8/octobot/community/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_donation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_public_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_supports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_tentacles_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/community_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/startup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/models/strategy_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.751683 OctoBot-1.0.8/octobot/community/supabase_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28284 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/community_supabase_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/configuration_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/postgres_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/supabase_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.751683 OctoBot-1.0.8/octobot/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/config/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/config/default_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/config/logging_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/config/profile_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/databases_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/octobot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/octobot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/octobot_backtesting_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.751683 OctoBot-1.0.8/octobot/producers/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/producers/evaluator_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/producers/exchange_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/producers/interface_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/producers/service_feed_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.751683 OctoBot-1.0.8/octobot/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/storage/db_databases_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/storage/trading_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.755683 OctoBot-1.0.8/octobot/strategy_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/fitness_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.791684 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/
--rw-r--r--   0 runner    (1001) docker     (127)   950272 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data
--rw-r--r--   0 runner    (1001) docker     (127)   937984 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data
--rw-r--r--   0 runner    (1001) docker     (127)   942080 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data
--rw-r--r--   0 runner    (1001) docker     (127)   958464 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data
--rw-r--r--   0 runner    (1001) docker     (127)   876544 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data
--rw-r--r--   0 runner    (1001) docker     (127)   978944 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data
--rw-r--r--   0 runner    (1001) docker     (127)   946176 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data
--rw-r--r--   0 runner    (1001) docker     (127)   913408 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data
--rw-r--r--   0 runner    (1001) docker     (127)  3764224 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data
--rw-r--r--   0 runner    (1001) docker     (127)  3129344 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data
--rw-r--r--   0 runner    (1001) docker     (127)  2822144 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data
--rw-r--r--   0 runner    (1001) docker     (127)  2547712 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data
--rw-r--r--   0 runner    (1001) docker     (127)  3735552 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data
--rw-r--r--   0 runner    (1001) docker     (127)  3551232 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data
--rw-r--r--   0 runner    (1001) docker     (127)   983040 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data
--rw-r--r--   0 runner    (1001) docker     (127)   937984 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/scored_run_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    45758 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/strategy_design_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/strategy_design_optimizer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/strategy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/strategy_optimizer/test_suite_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/task_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/octobot/updater/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/updater/binary_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/updater/python_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/updater/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-16 10:01:44.000000 OctoBot-1.0.8/octobot/updater/updater_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-16 10:01:44.000000 OctoBot-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-16 10:02:56.803684 OctoBot-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-16 10:01:44.000000 OctoBot-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-16 10:01:44.000000 OctoBot-1.0.8/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.731683 OctoBot-1.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/automations/
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/automations/test_automation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/backtesting_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/backtesting_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/backtesting_tests/backtesting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/evaluators_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/evaluators_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/evaluators_tests/abstract_TA_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/launch_test/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/launch_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/launch_test/launch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.795684 OctoBot-1.0.8/tests/functional_tests/strategy_evaluators_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/strategy_evaluators_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/bot_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/data_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/memory_check_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/test_utils/trading_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/community/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_errors_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_sentry_aiohttp_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/test_community_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/test_community_supabase_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/community/test_community_ws_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_design_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/trading_modes_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/trading_modes_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:02:56.799684 OctoBot-1.0.8/tests/unit_tests/updater/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-16 10:01:44.000000 OctoBot-1.0.8/tests/unit_tests/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.600824 OctoBot-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    65618 2024-04-18 07:14:55.000000 OctoBot-1.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-18 07:14:55.000000 OctoBot-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-18 07:14:55.000000 OctoBot-1.0.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/OctoBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 07:16:04.000000 OctoBot-1.0.9/OctoBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-18 07:16:04.600824 OctoBot-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-04-18 07:14:55.000000 OctoBot-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/api/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/api/strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/automation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/automation/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/bases/abstract_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/bases/abstract_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/bases/abstract_trigger_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/automation/bases/automation_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/backtesting/abstract_backtesting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/backtesting/independent_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/backtesting/octobot_backtesting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.540824 OctoBot-1.0.9/octobot/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/channels/octobot_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.544824 OctoBot-1.0.9/octobot/community/
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26318 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/community_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/community_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.544824 OctoBot-1.0.9/octobot/community/errors_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors_upload/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors_upload/errors_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors_upload/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/errors_upload/sentry_aiohttp_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.544824 OctoBot-1.0.9/octobot/community/feeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/feeds/abstract_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/feeds/community_supabase_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/feeds/community_ws_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/feeds/feed_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/graphql_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/identifiers_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.548824 OctoBot-1.0.9/octobot/community/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_donation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_public_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_supports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_tentacles_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/community_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/startup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/models/strategy_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.548824 OctoBot-1.0.9/octobot/community/supabase_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29331 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/community_supabase_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/configuration_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/postgres_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/supabase_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.548824 OctoBot-1.0.9/octobot/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/config/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/config/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/config/logging_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/config/profile_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/databases_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/octobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/octobot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/octobot_backtesting_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.548824 OctoBot-1.0.9/octobot/producers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/producers/evaluator_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/producers/exchange_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/producers/interface_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/producers/service_feed_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.548824 OctoBot-1.0.9/octobot/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/storage/db_databases_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/storage/trading_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.552824 OctoBot-1.0.9/octobot/strategy_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/fitness_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.588824 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   950272 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data
+-rw-r--r--   0 runner    (1001) docker     (127)   937984 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data
+-rw-r--r--   0 runner    (1001) docker     (127)   942080 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data
+-rw-r--r--   0 runner    (1001) docker     (127)   958464 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data
+-rw-r--r--   0 runner    (1001) docker     (127)   876544 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data
+-rw-r--r--   0 runner    (1001) docker     (127)   978944 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data
+-rw-r--r--   0 runner    (1001) docker     (127)   946176 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data
+-rw-r--r--   0 runner    (1001) docker     (127)   913408 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data
+-rw-r--r--   0 runner    (1001) docker     (127)  3764224 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data
+-rw-r--r--   0 runner    (1001) docker     (127)  3129344 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data
+-rw-r--r--   0 runner    (1001) docker     (127)  2822144 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data
+-rw-r--r--   0 runner    (1001) docker     (127)  2547712 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data
+-rw-r--r--   0 runner    (1001) docker     (127)  3735552 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data
+-rw-r--r--   0 runner    (1001) docker     (127)  3551232 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data
+-rw-r--r--   0 runner    (1001) docker     (127)   983040 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data
+-rw-r--r--   0 runner    (1001) docker     (127)   937984 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data
+-rw-r--r--   0 runner    (1001) docker     (127)   360448 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/ExchangeHistoryDataCollector_1711122002.311132.data
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/scored_run_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45758 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/strategy_design_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/strategy_design_optimizer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/strategy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/strategy_optimizer/test_suite_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/task_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/octobot/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/updater/binary_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/updater/python_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/updater/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-18 07:14:55.000000 OctoBot-1.0.9/octobot/updater/updater_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 07:14:55.000000 OctoBot-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 07:16:04.600824 OctoBot-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-18 07:14:55.000000 OctoBot-1.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-18 07:14:55.000000 OctoBot-1.0.9/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.532824 OctoBot-1.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/automations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/automations/test_automation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/backtesting_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/backtesting_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/backtesting_tests/backtesting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/evaluators_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/evaluators_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/evaluators_tests/abstract_TA_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/launch_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/launch_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/launch_test/launch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/functional_tests/strategy_evaluators_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/strategy_evaluators_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.592824 OctoBot-1.0.9/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/bot_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/data_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/memory_check_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/test_utils/trading_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/community/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_errors_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_sentry_aiohttp_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/test_community_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/test_community_supabase_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/community/test_community_ws_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_design_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/trading_modes_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/trading_modes_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:16:04.596824 OctoBot-1.0.9/tests/unit_tests/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 07:14:55.000000 OctoBot-1.0.9/tests/unit_tests/updater/test_updater.py
```

### Comparing `OctoBot-1.0.8/CHANGELOG.md` & `OctoBot-1.0.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 *It is strongly advised to perform an update of your tentacles after updating OctoBot. (start.py tentacles --install --all)*
 
+## [1.0.9] - 2024-04-18
+### Added
+- [DigitalOcean] Added in marketplace and handle one click deployment
+- [IndexTradingMode] Add the Index Trading Mode enabling to follow custom indexes
+- [TradingViewTradingMode] Add quote and offsets from the current price
+- [DCATradingMode] Add max holding ratio to cap the maximum exposure to an asset
+- [Coinbase] Handle new API key format
+### Updated
+- [CCXT] Update to CCXT 4.2.95
+### Fixed
+- [ChainedOrders] Fix chained orders quantity computation when handling fees
+- [ChainedOrders] Fix chained orders backtesting fill price to adapt to current candles
+- [StopLoss] Now always recreate stop losses when restarting on real trading
+- [Orders] Fixes rare order creation issues
+- [Coinbase] Fix order fetch issues
+- [BinanceUS] Fix permissions checks
+- [Kucoin] Fix a rare order creation issue
+- [MEXC] Fix order cancel issues
+- [WebInterface] Add robots.txt to prevent search engine indexing
+
 ## [1.0.8] - 2024-02-14
 ### Added
 - [TradingView] Support standalone stop loss and order tags
 ### Updated
 - [Tentacles] Improved docs
 - [WebInterface] Fix exchange credentials check when using futures accounts
 - [Exchanges] Increase base maximum candles count and make it customizable via env variable
```

### Comparing `OctoBot-1.0.8/LICENSE` & `OctoBot-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/OctoBot.egg-info/PKG-INFO` & `OctoBot-1.0.9/OctoBot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: OctoBot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Cryptocurrencies alert / trading bot
 Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: OctoBot-Commons==1.9.40
-Requires-Dist: OctoBot-Trading==2.4.55
-Requires-Dist: OctoBot-Evaluators==1.9.4
+Requires-Dist: OctoBot-Commons==1.9.43
+Requires-Dist: OctoBot-Trading==2.4.78
+Requires-Dist: OctoBot-Evaluators==1.9.5
 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
-Requires-Dist: OctoBot-Services==1.6.10
+Requires-Dist: OctoBot-Services==1.6.13
 Requires-Dist: OctoBot-Backtesting==1.9.7
 Requires-Dist: Async-Channel==2.2.1
-Requires-Dist: trading-backend==1.2.14
+Requires-Dist: trading-backend==1.2.19
 Requires-Dist: colorlog==6.8.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3
 Requires-Dist: packaging==23.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: setuptools==69.0.3
 Requires-Dist: websockets
@@ -34,20 +34,19 @@
 Requires-Dist: gotrue==1.0.3
 Requires-Dist: supafunc==0.2.3
 Requires-Dist: postgrest==0.10.8
 Requires-Dist: realtime==1.0.0
 Requires-Dist: httpcore==0.17.3
 Requires-Dist: anyio==4.0.0
 
-# OctoBot [1.0.8](https://octobot.click/gh-changelog)
+# OctoBot [1.0.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi)
 [![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
-[![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
 
 #### Octobot Community
 [![OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]()
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram)
 [![Discord](https://img.shields.io/discord/530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-discord)
 [![Telegram News](https://img.shields.io/badge/telegram-news-blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project)
 [![Twitter](https://img.shields.io/twitter/follow/DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-twitter)
@@ -85,20 +84,25 @@
 - [Install](https://www.octobot.cloud/en/guides/octobot-advanced-usage/tentacle-manager?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=install_tentacles), [modify](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=modify_tentacles) and even [create](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=create_tentacles) new tentacles to build your ideal cryptocurrency trading robot.
 - [Contribute](https://www.octobot.cloud/en/guides/octobot-developers-environment/setup-your-environment?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=contribute) to improve OctoBot core repositories and tentacles.
 
 [OctoBot is AI ready](https://www.octobot.cloud/features/ai-trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=ai-ready): Python being the main language for OctoBot, it's easy to integrate machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/tensorflow) or any other libraries and take advantage of all the available data and create a very powerful trading strategy.
 
 Looking for more info ? Check out our Octobot guides at [octobot.cloud/en/guides/octobot](https://www.octobot.cloud/en/guides/octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
 
-## Installation  
-OctoBot's installation is **very simple**, you can either:
-- [Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud). With OctoBot cloud, experience hassle-free installation, updates, and maintenance - leave it all to us! Your robot will also benefit from cloud only features.
-- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server and enjoy all features for free.
-- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/with-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
-
+## Installation
+### One click deployment using DigitalOcean
+OctoBot can be easily launched on the cloud from the [DigitalOcean Marketplace](https://digitalocean.pxf.io/octobot-app).
+
+[![Deploy on DO](https://mp-assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://digitalocean.pxf.io/start-octobot)
+
+### Manual installations
+To install OctoBot, you can either:
+- [Deploy your OctoBot on the cloud using DigitalOcean](https://octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud) and have your OctoBot automating your strategies 24/7.
+- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-your-computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server.
+- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
     Docker install in one line summary:
     ```
     docker run -itd --name OctoBot -p 80:5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $(pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable
     ```
     Your OctoBot will be accessible on [http://localhost](http://localhost).
 
 ## Exchanges
@@ -120,14 +124,32 @@
 To trade on any exchange, just activate the exchange in your OctoBot. This enables you to trade with [simulated money](https://www.octobot.cloud/en/guides/octobot-usage/simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-trading) on this exchange.
 
 No exchange credential is required.
 
 ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as described [on the exchange guides](https://www.octobot.cloud/en/guides/exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides). 
 
+## Follow your investments
+
+You can follow your OctoBots portfolio, orders, trades and historical performance from your phone with our [Android application](https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp). You can also install the [web application](https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments) to have the same experience on any smartphone or computer.
+
+<p align="middle">
+<a href='https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png' height="50px"/></a>
+</p>
+
+<p align="middle">
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bots-en.png" height="414" alt="Follow your bots from your mobile">
+  </a>  
+  &nbsp;&nbsp;&nbsp;&nbsp;    
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bot-view-pf-en.png" height="414" alt="Follow each trade and profits of your OctoBot from your mobile">
+  </a>  
+</p>
+
 ## Testing trading strategies
 
 OctoBot comes with its [built-in backtesting engine](https://www.octobot.cloud/en/guides/octobot-usage/backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting) which enables you to trade with simulated money using historical exchange data.
 
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/blob/assets/backtesting_report.jpg)  
 
 Backtesting will give you accurate insights on the past performance and behavior of trading strategies.
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: OctoBot Version: 1.0.8 Summary: Cryptocurrencies
+Metadata-Version: 2.1 Name: OctoBot Version: 1.0.9 Summary: Cryptocurrencies
 alert / trading bot Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software Author-email: contact@drakkar.software License: GPL-
 3.0 Classifier: Development Status :: 4 - Beta Classifier: Operating System ::
 OS Independent Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-OctoBot-Commons==1.9.40 Requires-Dist: OctoBot-Trading==2.4.55 Requires-Dist:
-OctoBot-Evaluators==1.9.4 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
-Requires-Dist: OctoBot-Services==1.6.10 Requires-Dist: OctoBot-
+OctoBot-Commons==1.9.43 Requires-Dist: OctoBot-Trading==2.4.78 Requires-Dist:
+OctoBot-Evaluators==1.9.5 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
+Requires-Dist: OctoBot-Services==1.6.13 Requires-Dist: OctoBot-
 Backtesting==1.9.7 Requires-Dist: Async-Channel==2.2.1 Requires-Dist: trading-
-backend==1.2.14 Requires-Dist: colorlog==6.8.0 Requires-Dist: requests==2.31.0
+backend==1.2.19 Requires-Dist: colorlog==6.8.0 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3 Requires-Dist: packaging==23.2 Requires-Dist: python-
 dotenv==1.0.0 Requires-Dist: setuptools==69.0.3 Requires-Dist: websockets
 Requires-Dist: supabase==1.0.4 Requires-Dist: gotrue==1.0.3 Requires-Dist:
 supafunc==0.2.3 Requires-Dist: postgrest==0.10.8 Requires-Dist: realtime==1.0.0
-Requires-Dist: httpcore==0.17.3 Requires-Dist: anyio==4.0.0 # OctoBot [1.0.8]
+Requires-Dist: httpcore==0.17.3 Requires-Dist: anyio==4.0.0 # OctoBot [1.0.9]
 (https://octobot.click/gh-changelog) [![PyPI](https://img.shields.io/pypi/v/
 OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi) [![Downloads](https://
 pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot) [!
 [Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/
 octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub) [![OctoBot-CI]
 (https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)]
-(https://github.com/Drakkar-Software/OctoBot/actions) [![UptimeRobot](https://
-img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)]
-(https://octobot.click/gh-status) #### Octobot Community [![OctoBot](https://
-img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/
-community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [!
-[Telegram Chat](https://img.shields.io/badge/telegram-chat-
+(https://github.com/Drakkar-Software/OctoBot/actions) #### Octobot Community [!
+[OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://
+dev.octobot.cloud/api/community/
+stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [![Telegram
+Chat](https://img.shields.io/badge/telegram-chat-
 green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram) [!
 [Discord](https://img.shields.io/discord/
 530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-
 discord) [![Telegram News](https://img.shields.io/badge/telegram-news-
 blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project) [!
 [Twitter](https://img.shields.io/twitter/follow/
 DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-
@@ -85,26 +84,29 @@
 ready): Python being the main language for OctoBot, it's easy to integrate
 machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/
 tensorflow) or any other libraries and take advantage of all the available data
 and create a very powerful trading strategy. Looking for more info ? Check out
 our Octobot guides at [octobot.cloud/en/guides/octobot](https://
 www.octobot.cloud/en/guides/
 octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
-## Installation OctoBot's installation is **very simple**, you can either: -
-[Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-
-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud).
-With OctoBot cloud, experience hassle-free installation, updates, and
-maintenance - leave it all to us! Your robot will also benefit from cloud only
-features. - [Download and install](https://www.octobot.cloud/en/guides/octobot-
-installation/
-local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
-OctoBot on your computer or server and enjoy all features for free. - Install
-OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-
-installation/with-
-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
+## Installation ### One click deployment using DigitalOcean OctoBot can be
+easily launched on the cloud from the [DigitalOcean Marketplace](https://
+digitalocean.pxf.io/octobot-app). [![Deploy on DO](https://mp-
+assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://
+digitalocean.pxf.io/start-octobot) ### Manual installations To install OctoBot,
+you can either: - [Deploy your OctoBot on the cloud using DigitalOcean](https:/
+/octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-
+digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud)
+and have your OctoBot automating your strategies 24/7. - [Download and install]
+(https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-
+your-
+computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
+OctoBot on your computer or server. - Install OctoBot [using docker](https://
+www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-
+video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
 Docker install in one line summary: ``` docker run -itd --name OctoBot -p 80:
 5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $
 (pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable ``` Your OctoBot will
 be accessible on [http://localhost](http://localhost). ## Exchanges [![Binance
 supported exchange partnership](../assets/binance-logo.png)](https://
 www.octobot.cloud/en/guides/octobot-partner-exchanges/
 binance?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=binance)
@@ -143,14 +145,24 @@
 OctoBot. This enables you to trade with [simulated money](https://
 www.octobot.cloud/en/guides/octobot-usage/
 simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-
 trading) on this exchange. No exchange credential is required. ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as
 described [on the exchange guides](https://www.octobot.cloud/en/guides/
 exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides).
+## Follow your investments You can follow your OctoBots portfolio, orders,
+trades and historical performance from your phone with our [Android
+application](https://play.google.com/store/apps/
+details?id=com.drakkarsoftware.octobotapp). You can also install the [web
+application](https://mobile.octobot.cloud/
+?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments)
+to have the same experience on any smartphone or computer.
+_[_G_e_t_ _i_t_ _o_n_ _G_o_o_g_l_e_ _P_l_a_y_]
+_[_F_o_l_l_o_w_ _y_o_u_r_ _b_o_t_s_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]    _[_F_o_l_l_o_w_ _e_a_c_h_ _t_r_a_d_e_ _a_n_d_ _p_r_o_f_i_t_s_ _o_f_ _y_o_u_r
+_O_c_t_o_B_o_t_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]
 ## Testing trading strategies OctoBot comes with its [built-in backtesting
 engine](https://www.octobot.cloud/en/guides/octobot-usage/
 backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting)
 which enables you to trade with simulated money using historical exchange data.
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../
 assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/
 blob/assets/backtesting_report.jpg) Backtesting will give you accurate insights
```

### Comparing `OctoBot-1.0.8/OctoBot.egg-info/SOURCES.txt` & `OctoBot-1.0.9/OctoBot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data
 octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data
+octobot/strategy_optimizer/optimizer_data_files/ExchangeHistoryDataCollector_1711122002.311132.data
 octobot/updater/__init__.py
 octobot/updater/binary_updater.py
 octobot/updater/python_updater.py
 octobot/updater/updater.py
 octobot/updater/updater_factory.py
 tests/functional_tests/__init__.py
 tests/functional_tests/automations/__init__.py
```

### Comparing `OctoBot-1.0.8/PKG-INFO` & `OctoBot-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: OctoBot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Cryptocurrencies alert / trading bot
 Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: OctoBot-Commons==1.9.40
-Requires-Dist: OctoBot-Trading==2.4.55
-Requires-Dist: OctoBot-Evaluators==1.9.4
+Requires-Dist: OctoBot-Commons==1.9.43
+Requires-Dist: OctoBot-Trading==2.4.78
+Requires-Dist: OctoBot-Evaluators==1.9.5
 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
-Requires-Dist: OctoBot-Services==1.6.10
+Requires-Dist: OctoBot-Services==1.6.13
 Requires-Dist: OctoBot-Backtesting==1.9.7
 Requires-Dist: Async-Channel==2.2.1
-Requires-Dist: trading-backend==1.2.14
+Requires-Dist: trading-backend==1.2.19
 Requires-Dist: colorlog==6.8.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3
 Requires-Dist: packaging==23.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: setuptools==69.0.3
 Requires-Dist: websockets
@@ -34,20 +34,19 @@
 Requires-Dist: gotrue==1.0.3
 Requires-Dist: supafunc==0.2.3
 Requires-Dist: postgrest==0.10.8
 Requires-Dist: realtime==1.0.0
 Requires-Dist: httpcore==0.17.3
 Requires-Dist: anyio==4.0.0
 
-# OctoBot [1.0.8](https://octobot.click/gh-changelog)
+# OctoBot [1.0.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi)
 [![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
-[![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
 
 #### Octobot Community
 [![OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]()
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram)
 [![Discord](https://img.shields.io/discord/530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-discord)
 [![Telegram News](https://img.shields.io/badge/telegram-news-blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project)
 [![Twitter](https://img.shields.io/twitter/follow/DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-twitter)
@@ -85,20 +84,25 @@
 - [Install](https://www.octobot.cloud/en/guides/octobot-advanced-usage/tentacle-manager?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=install_tentacles), [modify](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=modify_tentacles) and even [create](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=create_tentacles) new tentacles to build your ideal cryptocurrency trading robot.
 - [Contribute](https://www.octobot.cloud/en/guides/octobot-developers-environment/setup-your-environment?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=contribute) to improve OctoBot core repositories and tentacles.
 
 [OctoBot is AI ready](https://www.octobot.cloud/features/ai-trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=ai-ready): Python being the main language for OctoBot, it's easy to integrate machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/tensorflow) or any other libraries and take advantage of all the available data and create a very powerful trading strategy.
 
 Looking for more info ? Check out our Octobot guides at [octobot.cloud/en/guides/octobot](https://www.octobot.cloud/en/guides/octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
 
-## Installation  
-OctoBot's installation is **very simple**, you can either:
-- [Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud). With OctoBot cloud, experience hassle-free installation, updates, and maintenance - leave it all to us! Your robot will also benefit from cloud only features.
-- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server and enjoy all features for free.
-- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/with-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
-
+## Installation
+### One click deployment using DigitalOcean
+OctoBot can be easily launched on the cloud from the [DigitalOcean Marketplace](https://digitalocean.pxf.io/octobot-app).
+
+[![Deploy on DO](https://mp-assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://digitalocean.pxf.io/start-octobot)
+
+### Manual installations
+To install OctoBot, you can either:
+- [Deploy your OctoBot on the cloud using DigitalOcean](https://octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud) and have your OctoBot automating your strategies 24/7.
+- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-your-computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server.
+- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
     Docker install in one line summary:
     ```
     docker run -itd --name OctoBot -p 80:5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $(pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable
     ```
     Your OctoBot will be accessible on [http://localhost](http://localhost).
 
 ## Exchanges
@@ -120,14 +124,32 @@
 To trade on any exchange, just activate the exchange in your OctoBot. This enables you to trade with [simulated money](https://www.octobot.cloud/en/guides/octobot-usage/simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-trading) on this exchange.
 
 No exchange credential is required.
 
 ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as described [on the exchange guides](https://www.octobot.cloud/en/guides/exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides). 
 
+## Follow your investments
+
+You can follow your OctoBots portfolio, orders, trades and historical performance from your phone with our [Android application](https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp). You can also install the [web application](https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments) to have the same experience on any smartphone or computer.
+
+<p align="middle">
+<a href='https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png' height="50px"/></a>
+</p>
+
+<p align="middle">
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bots-en.png" height="414" alt="Follow your bots from your mobile">
+  </a>  
+  &nbsp;&nbsp;&nbsp;&nbsp;    
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bot-view-pf-en.png" height="414" alt="Follow each trade and profits of your OctoBot from your mobile">
+  </a>  
+</p>
+
 ## Testing trading strategies
 
 OctoBot comes with its [built-in backtesting engine](https://www.octobot.cloud/en/guides/octobot-usage/backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting) which enables you to trade with simulated money using historical exchange data.
 
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/blob/assets/backtesting_report.jpg)  
 
 Backtesting will give you accurate insights on the past performance and behavior of trading strategies.
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: OctoBot Version: 1.0.8 Summary: Cryptocurrencies
+Metadata-Version: 2.1 Name: OctoBot Version: 1.0.9 Summary: Cryptocurrencies
 alert / trading bot Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software Author-email: contact@drakkar.software License: GPL-
 3.0 Classifier: Development Status :: 4 - Beta Classifier: Operating System ::
 OS Independent Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-OctoBot-Commons==1.9.40 Requires-Dist: OctoBot-Trading==2.4.55 Requires-Dist:
-OctoBot-Evaluators==1.9.4 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
-Requires-Dist: OctoBot-Services==1.6.10 Requires-Dist: OctoBot-
+OctoBot-Commons==1.9.43 Requires-Dist: OctoBot-Trading==2.4.78 Requires-Dist:
+OctoBot-Evaluators==1.9.5 Requires-Dist: OctoBot-Tentacles-Manager==2.9.10
+Requires-Dist: OctoBot-Services==1.6.13 Requires-Dist: OctoBot-
 Backtesting==1.9.7 Requires-Dist: Async-Channel==2.2.1 Requires-Dist: trading-
-backend==1.2.14 Requires-Dist: colorlog==6.8.0 Requires-Dist: requests==2.31.0
+backend==1.2.19 Requires-Dist: colorlog==6.8.0 Requires-Dist: requests==2.31.0
 Requires-Dist: urllib3 Requires-Dist: packaging==23.2 Requires-Dist: python-
 dotenv==1.0.0 Requires-Dist: setuptools==69.0.3 Requires-Dist: websockets
 Requires-Dist: supabase==1.0.4 Requires-Dist: gotrue==1.0.3 Requires-Dist:
 supafunc==0.2.3 Requires-Dist: postgrest==0.10.8 Requires-Dist: realtime==1.0.0
-Requires-Dist: httpcore==0.17.3 Requires-Dist: anyio==4.0.0 # OctoBot [1.0.8]
+Requires-Dist: httpcore==0.17.3 Requires-Dist: anyio==4.0.0 # OctoBot [1.0.9]
 (https://octobot.click/gh-changelog) [![PyPI](https://img.shields.io/pypi/v/
 OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi) [![Downloads](https://
 pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot) [!
 [Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/
 octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub) [![OctoBot-CI]
 (https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)]
-(https://github.com/Drakkar-Software/OctoBot/actions) [![UptimeRobot](https://
-img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)]
-(https://octobot.click/gh-status) #### Octobot Community [![OctoBot](https://
-img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/
-community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [!
-[Telegram Chat](https://img.shields.io/badge/telegram-chat-
+(https://github.com/Drakkar-Software/OctoBot/actions) #### Octobot Community [!
+[OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://
+dev.octobot.cloud/api/community/
+stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [![Telegram
+Chat](https://img.shields.io/badge/telegram-chat-
 green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram) [!
 [Discord](https://img.shields.io/discord/
 530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-
 discord) [![Telegram News](https://img.shields.io/badge/telegram-news-
 blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project) [!
 [Twitter](https://img.shields.io/twitter/follow/
 DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-
@@ -85,26 +84,29 @@
 ready): Python being the main language for OctoBot, it's easy to integrate
 machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/
 tensorflow) or any other libraries and take advantage of all the available data
 and create a very powerful trading strategy. Looking for more info ? Check out
 our Octobot guides at [octobot.cloud/en/guides/octobot](https://
 www.octobot.cloud/en/guides/
 octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
-## Installation OctoBot's installation is **very simple**, you can either: -
-[Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-
-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud).
-With OctoBot cloud, experience hassle-free installation, updates, and
-maintenance - leave it all to us! Your robot will also benefit from cloud only
-features. - [Download and install](https://www.octobot.cloud/en/guides/octobot-
-installation/
-local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
-OctoBot on your computer or server and enjoy all features for free. - Install
-OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-
-installation/with-
-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
+## Installation ### One click deployment using DigitalOcean OctoBot can be
+easily launched on the cloud from the [DigitalOcean Marketplace](https://
+digitalocean.pxf.io/octobot-app). [![Deploy on DO](https://mp-
+assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://
+digitalocean.pxf.io/start-octobot) ### Manual installations To install OctoBot,
+you can either: - [Deploy your OctoBot on the cloud using DigitalOcean](https:/
+/octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-
+digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud)
+and have your OctoBot automating your strategies 24/7. - [Download and install]
+(https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-
+your-
+computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
+OctoBot on your computer or server. - Install OctoBot [using docker](https://
+www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-
+video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
 Docker install in one line summary: ``` docker run -itd --name OctoBot -p 80:
 5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $
 (pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable ``` Your OctoBot will
 be accessible on [http://localhost](http://localhost). ## Exchanges [![Binance
 supported exchange partnership](../assets/binance-logo.png)](https://
 www.octobot.cloud/en/guides/octobot-partner-exchanges/
 binance?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=binance)
@@ -143,14 +145,24 @@
 OctoBot. This enables you to trade with [simulated money](https://
 www.octobot.cloud/en/guides/octobot-usage/
 simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-
 trading) on this exchange. No exchange credential is required. ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as
 described [on the exchange guides](https://www.octobot.cloud/en/guides/
 exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides).
+## Follow your investments You can follow your OctoBots portfolio, orders,
+trades and historical performance from your phone with our [Android
+application](https://play.google.com/store/apps/
+details?id=com.drakkarsoftware.octobotapp). You can also install the [web
+application](https://mobile.octobot.cloud/
+?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments)
+to have the same experience on any smartphone or computer.
+_[_G_e_t_ _i_t_ _o_n_ _G_o_o_g_l_e_ _P_l_a_y_]
+_[_F_o_l_l_o_w_ _y_o_u_r_ _b_o_t_s_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]    _[_F_o_l_l_o_w_ _e_a_c_h_ _t_r_a_d_e_ _a_n_d_ _p_r_o_f_i_t_s_ _o_f_ _y_o_u_r
+_O_c_t_o_B_o_t_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]
 ## Testing trading strategies OctoBot comes with its [built-in backtesting
 engine](https://www.octobot.cloud/en/guides/octobot-usage/
 backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting)
 which enables you to trade with simulated money using historical exchange data.
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../
 assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/
 blob/assets/backtesting_report.jpg) Backtesting will give you accurate insights
```

### Comparing `OctoBot-1.0.8/README.md` & `OctoBot-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# OctoBot [1.0.8](https://octobot.click/gh-changelog)
+# OctoBot [1.0.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi)
 [![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
-[![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
 
 #### Octobot Community
 [![OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]()
 [![Telegram Chat](https://img.shields.io/badge/telegram-chat-green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram)
 [![Discord](https://img.shields.io/discord/530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-discord)
 [![Telegram News](https://img.shields.io/badge/telegram-news-blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project)
 [![Twitter](https://img.shields.io/twitter/follow/DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-twitter)
@@ -45,20 +44,25 @@
 - [Install](https://www.octobot.cloud/en/guides/octobot-advanced-usage/tentacle-manager?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=install_tentacles), [modify](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=modify_tentacles) and even [create](https://www.octobot.cloud/en/guides/octobot-tentacles-development/create-a-tentacle?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=create_tentacles) new tentacles to build your ideal cryptocurrency trading robot.
 - [Contribute](https://www.octobot.cloud/en/guides/octobot-developers-environment/setup-your-environment?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=contribute) to improve OctoBot core repositories and tentacles.
 
 [OctoBot is AI ready](https://www.octobot.cloud/features/ai-trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=ai-ready): Python being the main language for OctoBot, it's easy to integrate machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/tensorflow) or any other libraries and take advantage of all the available data and create a very powerful trading strategy.
 
 Looking for more info ? Check out our Octobot guides at [octobot.cloud/en/guides/octobot](https://www.octobot.cloud/en/guides/octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
 
-## Installation  
-OctoBot's installation is **very simple**, you can either:
-- [Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud). With OctoBot cloud, experience hassle-free installation, updates, and maintenance - leave it all to us! Your robot will also benefit from cloud only features.
-- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server and enjoy all features for free.
-- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/with-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
-
+## Installation
+### One click deployment using DigitalOcean
+OctoBot can be easily launched on the cloud from the [DigitalOcean Marketplace](https://digitalocean.pxf.io/octobot-app).
+
+[![Deploy on DO](https://mp-assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://digitalocean.pxf.io/start-octobot)
+
+### Manual installations
+To install OctoBot, you can either:
+- [Deploy your OctoBot on the cloud using DigitalOcean](https://octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud) and have your OctoBot automating your strategies 24/7.
+- [Download and install](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-your-computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation) OctoBot on your computer or server.
+- Install OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
     Docker install in one line summary:
     ```
     docker run -itd --name OctoBot -p 80:5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $(pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable
     ```
     Your OctoBot will be accessible on [http://localhost](http://localhost).
 
 ## Exchanges
@@ -80,14 +84,32 @@
 To trade on any exchange, just activate the exchange in your OctoBot. This enables you to trade with [simulated money](https://www.octobot.cloud/en/guides/octobot-usage/simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-trading) on this exchange.
 
 No exchange credential is required.
 
 ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as described [on the exchange guides](https://www.octobot.cloud/en/guides/exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides). 
 
+## Follow your investments
+
+You can follow your OctoBots portfolio, orders, trades and historical performance from your phone with our [Android application](https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp). You can also install the [web application](https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments) to have the same experience on any smartphone or computer.
+
+<p align="middle">
+<a href='https://play.google.com/store/apps/details?id=com.drakkarsoftware.octobotapp'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png' height="50px"/></a>
+</p>
+
+<p align="middle">
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bots-en.png" height="414" alt="Follow your bots from your mobile">
+  </a>  
+  &nbsp;&nbsp;&nbsp;&nbsp;    
+  <a href="https://mobile.octobot.cloud/?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments_image">
+    <img src="../assets/mobile/bot-view-pf-en.png" height="414" alt="Follow each trade and profits of your OctoBot from your mobile">
+  </a>  
+</p>
+
 ## Testing trading strategies
 
 OctoBot comes with its [built-in backtesting engine](https://www.octobot.cloud/en/guides/octobot-usage/backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting) which enables you to trade with simulated money using historical exchange data.
 
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/blob/assets/backtesting_report.jpg)  
 
 Backtesting will give you accurate insights on the past performance and behavior of trading strategies.
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-# OctoBot [1.0.8](https://octobot.click/gh-changelog) [![PyPI](https://
+# OctoBot [1.0.9](https://octobot.click/gh-changelog) [![PyPI](https://
 img.shields.io/pypi/v/OctoBot.svg?logo=pypi)](https://octobot.click/gh-pypi) [!
 [Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/
 octobot) [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/
 octobot.svg?logo=docker)](https://octobot.click/gh-dockerhub) [![OctoBot-CI]
 (https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)]
-(https://github.com/Drakkar-Software/OctoBot/actions) [![UptimeRobot](https://
-img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)]
-(https://octobot.click/gh-status) #### Octobot Community [![OctoBot](https://
-img.shields.io/badge/dynamic/json.svg?&url=https://dev.octobot.cloud/api/
-community/stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [!
-[Telegram Chat](https://img.shields.io/badge/telegram-chat-
+(https://github.com/Drakkar-Software/OctoBot/actions) #### Octobot Community [!
+[OctoBot](https://img.shields.io/badge/dynamic/json.svg?&url=https://
+dev.octobot.cloud/api/community/
+stats&query=$.total_bots&color=blue&label=Installed%20OctoBots)]() [![Telegram
+Chat](https://img.shields.io/badge/telegram-chat-
 green.svg?logo=telegram&label=Telegram)](https://octobot.click/gh-telegram) [!
 [Discord](https://img.shields.io/discord/
 530629985661222912.svg?logo=discord&label=Discord)](https://octobot.click/gh-
 discord) [![Telegram News](https://img.shields.io/badge/telegram-news-
 blue.svg?logo=telegram&label=Telegram)](https://t.me/OctoBot_Project) [!
 [Twitter](https://img.shields.io/twitter/follow/
 DrakkarsOctobot.svg?label=twitter&style=social)](https://octobot.click/gh-
@@ -67,26 +66,29 @@
 ready): Python being the main language for OctoBot, it's easy to integrate
 machine-learning libraries such as [Tensorflow](https://github.com/tensorflow/
 tensorflow) or any other libraries and take advantage of all the available data
 and create a very powerful trading strategy. Looking for more info ? Check out
 our Octobot guides at [octobot.cloud/en/guides/octobot](https://
 www.octobot.cloud/en/guides/
 octobot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=checkout_guides)
-## Installation OctoBot's installation is **very simple**, you can either: -
-[Deploy your OctoBot on OctoBot Cloud](https://octobot.cloud/trading-
-bot?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud).
-With OctoBot cloud, experience hassle-free installation, updates, and
-maintenance - leave it all to us! Your robot will also benefit from cloud only
-features. - [Download and install](https://www.octobot.cloud/en/guides/octobot-
-installation/
-local?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
-OctoBot on your computer or server and enjoy all features for free. - Install
-OctoBot [using docker](https://www.octobot.cloud/en/guides/octobot-
-installation/with-
-docker?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
+## Installation ### One click deployment using DigitalOcean OctoBot can be
+easily launched on the cloud from the [DigitalOcean Marketplace](https://
+digitalocean.pxf.io/octobot-app). [![Deploy on DO](https://mp-
+assets1.sfo2.digitaloceanspaces.com/deploy-to-do/do-btn-blue.svg)](https://
+digitalocean.pxf.io/start-octobot) ### Manual installations To install OctoBot,
+you can either: - [Deploy your OctoBot on the cloud using DigitalOcean](https:/
+/octobot.cloud/en/guides/octobot-installation/cloud-install-octobot-on-
+digitalocean?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_deploy_on_cloud)
+and have your OctoBot automating your strategies 24/7. - [Download and install]
+(https://www.octobot.cloud/en/guides/octobot-installation/install-octobot-on-
+your-
+computer?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_local_installation)
+OctoBot on your computer or server. - Install OctoBot [using docker](https://
+www.octobot.cloud/en/guides/octobot-installation/install-octobot-with-docker-
+video?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=readme_docker_installation).
 Docker install in one line summary: ``` docker run -itd --name OctoBot -p 80:
 5001 -v $(pwd)/user:/octobot/user -v $(pwd)/tentacles:/octobot/tentacles -v $
 (pwd)/logs:/octobot/logs drakkarsoftware/octobot:stable ``` Your OctoBot will
 be accessible on [http://localhost](http://localhost). ## Exchanges [![Binance
 supported exchange partnership](../assets/binance-logo.png)](https://
 www.octobot.cloud/en/guides/octobot-partner-exchanges/
 binance?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=binance)
@@ -125,14 +127,24 @@
 OctoBot. This enables you to trade with [simulated money](https://
 www.octobot.cloud/en/guides/octobot-usage/
 simulator?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=paper-
 trading) on this exchange. No exchange credential is required. ### Real trading
 To use your real exchange account with OctoBot, enter your exchange API keys as
 described [on the exchange guides](https://www.octobot.cloud/en/guides/
 exchanges?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=exchanges_guides).
+## Follow your investments You can follow your OctoBots portfolio, orders,
+trades and historical performance from your phone with our [Android
+application](https://play.google.com/store/apps/
+details?id=com.drakkarsoftware.octobotapp). You can also install the [web
+application](https://mobile.octobot.cloud/
+?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=follow_your_investments)
+to have the same experience on any smartphone or computer.
+_[_G_e_t_ _i_t_ _o_n_ _G_o_o_g_l_e_ _P_l_a_y_]
+_[_F_o_l_l_o_w_ _y_o_u_r_ _b_o_t_s_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]    _[_F_o_l_l_o_w_ _e_a_c_h_ _t_r_a_d_e_ _a_n_d_ _p_r_o_f_i_t_s_ _o_f_ _y_o_u_r
+_O_c_t_o_B_o_t_ _f_r_o_m_ _y_o_u_r_ _m_o_b_i_l_e_]
 ## Testing trading strategies OctoBot comes with its [built-in backtesting
 engine](https://www.octobot.cloud/en/guides/octobot-usage/
 backtesting?utm_source=github&utm_medium=dk&utm_campaign=regular_open_source_content&utm_content=backtesting)
 which enables you to trade with simulated money using historical exchange data.
 [![Backtesting report using grid trading on eth btc with 8 percent profit](../
 assets/backtesting_report.jpg)](https://github.com/Drakkar-Software/OctoBot/
 blob/assets/backtesting_report.jpg) Backtesting will give you accurate insights
```

### Comparing `OctoBot-1.0.8/octobot/__init__.py` & `OctoBot-1.0.9/octobot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public
 #  License along with OctoBot. If not, see <https://www.gnu.org/licenses/>.
 
 PROJECT_NAME = "OctoBot"
 AUTHOR = "Drakkar-Software"
-VERSION = "1.0.8"  # major.minor.revision
+VERSION = "1.0.9"  # major.minor.revision
 LONG_VERSION = f"{VERSION}"
```

### Comparing `OctoBot-1.0.8/octobot/api/__init__.py` & `OctoBot-1.0.9/octobot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/api/backtesting.py` & `OctoBot-1.0.9/octobot/api/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/api/strategy_optimizer.py` & `OctoBot-1.0.9/octobot/api/strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/api/updater.py` & `OctoBot-1.0.9/octobot/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/__init__.py` & `OctoBot-1.0.9/octobot/automation/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/automation.py` & `OctoBot-1.0.9/octobot/automation/automation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/bases/__init__.py` & `OctoBot-1.0.9/octobot/automation/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/bases/abstract_action.py` & `OctoBot-1.0.9/octobot/automation/bases/abstract_action.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/bases/abstract_condition.py` & `OctoBot-1.0.9/octobot/automation/bases/abstract_condition.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/bases/abstract_trigger_event.py` & `OctoBot-1.0.9/octobot/automation/bases/abstract_trigger_event.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/automation/bases/automation_step.py` & `OctoBot-1.0.9/octobot/automation/bases/automation_step.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/backtesting/__init__.py` & `OctoBot-1.0.9/octobot/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/backtesting/abstract_backtesting_test.py` & `OctoBot-1.0.9/octobot/backtesting/abstract_backtesting_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,18 @@
                          "AbstractExchangeHistoryCollector_1581775018.2658834.data"),
     "POWR/BTC": path.join(constants.OPTIMIZER_DATA_FILES_FOLDER,
                           "AbstractExchangeHistoryCollector_1581776404.9679003.data"),
     "2020ADA/USDT": path.join(TEST_DATA_FILES_FOLDER, "ExchangeHistoryDataCollector_1587769859.9278197.data"),
     "2020ADA/BTC": path.join(TEST_DATA_FILES_FOLDER, "ExchangeHistoryDataCollector_1588110698.1060486.data")
 }
 
+MULTI_ASSETS_DATA_FILE = path.join(
+    constants.OPTIMIZER_DATA_FILES_FOLDER, "ExchangeHistoryDataCollector_1711122002.311132.data"
+)
+
 EXTENDED_DATA_FILES = {
     "ADA/BTC": path.join(constants.OPTIMIZER_DATA_FILES_FOLDER,
                          "AbstractExchangeHistoryCollector_1581775117.1713624.data"),
     "ETC/BTC": path.join(constants.OPTIMIZER_DATA_FILES_FOLDER,
                          "AbstractExchangeHistoryCollector_1581775133.1533682.data"),
     "NEO/BTC": path.join(constants.OPTIMIZER_DATA_FILES_FOLDER,
                          "AbstractExchangeHistoryCollector_1581775139.0332782.data"),
```

### Comparing `OctoBot-1.0.8/octobot/backtesting/independent_backtesting.py` & `OctoBot-1.0.9/octobot/backtesting/independent_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/backtesting/octobot_backtesting.py` & `OctoBot-1.0.9/octobot/backtesting/octobot_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/channels/__init__.py` & `OctoBot-1.0.9/octobot/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/channels/octobot_channel.py` & `OctoBot-1.0.9/octobot/channels/octobot_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/cli.py` & `OctoBot-1.0.9/octobot/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/commands.py` & `OctoBot-1.0.9/octobot/commands.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/__init__.py` & `OctoBot-1.0.9/octobot/community/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/authentication.py` & `OctoBot-1.0.9/octobot/community/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,23 +36,25 @@
 import octobot_commons.authentication as authentication
 import octobot_commons.configuration as commons_configuration
 import octobot_commons.profiles as commons_profiles
 import octobot_trading.enums as trading_enums
 
 
 def _bot_data_update(func):
-    async def wrapper(*args, **kwargs):
+    async def wrapper(*args, raise_errors=False, **kwargs):
         self = args[0]
         if not self.is_logged_in_and_has_selected_bot():
             self.logger.debug(f"Skipping {func.__name__} update: no user selected bot.")
             return
         try:
             self.logger.debug(f"bot_data_update: {func.__name__} initiated.")
             return await func(*args, **kwargs)
         except Exception as err:
+            if raise_errors:
+                raise err
             self.logger.exception(err, True, f"Error when calling {func.__name__} {err}")
         finally:
             self.logger.debug(f"bot_data_update: {func.__name__} completed.")
     return wrapper
 
 
 class CommunityAuthentication(authentication.Authenticator):
```

### Comparing `OctoBot-1.0.8/octobot/community/community_analysis.py` & `OctoBot-1.0.9/octobot/community/community_analysis.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/community_manager.py` & `OctoBot-1.0.9/octobot/community/community_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors.py` & `OctoBot-1.0.9/octobot/community/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors_upload/__init__.py` & `OctoBot-1.0.9/octobot/community/errors_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors_upload/error_model.py` & `OctoBot-1.0.9/octobot/community/errors_upload/error_model.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors_upload/errors_uploader.py` & `OctoBot-1.0.9/octobot/community/errors_upload/errors_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors_upload/initializer.py` & `OctoBot-1.0.9/octobot/community/errors_upload/initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/errors_upload/sentry_aiohttp_transport.py` & `OctoBot-1.0.9/octobot/community/errors_upload/sentry_aiohttp_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  OctoBot is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public
 #  License along with OctoBot. If not, see <https://www.gnu.org/licenses/>.
+import logging
 import typing
 import asyncio
 import aiohttp
 import io
 import gzip
 
 try:
@@ -77,15 +78,16 @@
                         sentry_sdk.utils.logger.error(
                             "Unexpected status code: %s (body: %s)",
                             response.status,
                             await response.text(),
                         )
                         self.on_dropped_event("status_{}".format(response.status))
                         record_loss("network_error")
-            except Exception:
+            except BaseException as err:
+                logging.getLogger(self.__class__.__name__).warning(f"Sentry post error: {err} {err.__class__.__name__}")
                 self.on_dropped_event("network")
                 record_loss("network_error")
                 raise
 
         async def _async_send_event(
             self, event  # type: sentry_sdk._types.Event
         ) -> None:
```

### Comparing `OctoBot-1.0.8/octobot/community/feeds/__init__.py` & `OctoBot-1.0.9/octobot/community/feeds/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/feeds/abstract_feed.py` & `OctoBot-1.0.9/octobot/community/feeds/abstract_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/feeds/community_supabase_feed.py` & `OctoBot-1.0.9/octobot/community/feeds/community_supabase_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/feeds/community_ws_feed.py` & `OctoBot-1.0.9/octobot/community/feeds/community_ws_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/feeds/feed_factory.py` & `OctoBot-1.0.9/octobot/community/feeds/feed_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/graphql_requests.py` & `OctoBot-1.0.9/octobot/community/graphql_requests.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/identifiers_provider.py` & `OctoBot-1.0.9/octobot/community/identifiers_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/__init__.py` & `OctoBot-1.0.9/octobot/community/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_donation.py` & `OctoBot-1.0.9/octobot/community/models/community_donation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_fields.py` & `OctoBot-1.0.9/octobot/community/models/community_fields.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_public_data.py` & `OctoBot-1.0.9/octobot/community/models/community_public_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_supports.py` & `OctoBot-1.0.9/octobot/community/models/community_supports.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_tentacles_package.py` & `OctoBot-1.0.9/octobot/community/models/community_tentacles_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/community_user_account.py` & `OctoBot-1.0.9/octobot/community/models/community_user_account.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/formatters.py` & `OctoBot-1.0.9/octobot/community/models/formatters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/startup_info.py` & `OctoBot-1.0.9/octobot/community/models/startup_info.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/models/strategy_data.py` & `OctoBot-1.0.9/octobot/community/models/strategy_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/__init__.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/community_supabase_client.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/community_supabase_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 
 class CommunitySupabaseClient(supabase_client.AuthenticatedAsyncSupabaseClient):
     """
     Octobot Community layer added to supabase_client.AuthenticatedSupabaseClient
     """
     MAX_PAGINATED_REQUESTS_COUNT = 100
+    MAX_UUID_PER_COMMUNITY_REQUEST_FILTERS = 150
 
     def __init__(
         self,
         supabase_url: str,
         supabase_key: str,
         storage: configuration_storage.SyncConfigurationStorage,
         options: supabase.lib.client_options.ClientOptions = supabase.lib.client_options.ClientOptions(),
@@ -236,17 +237,18 @@
             await self.table("products").select(
                 "*,"
                 "category:product_categories!inner(slug, name_translations, type, metadata),"
                 "results:product_results!products_current_result_id_fkey("
                 "  profitability,"
                 "  reference_market_profitability"
                 ")"
-            ).eq(
-                enums.ProductKeys.VISIBILITY.value, "public"
-            )
+            ).match({
+                enums.ProductKeys.VISIBILITY.value: "public",
+                "category.type": "profile",
+            })
             .execute()
         ).data
 
     async def fetch_subscribed_products_urls(self) -> list:
         return json.loads(
             (await self.postgres_functions().invoke("get_subscribed_products_urls", {}))["data"]
         ) or []
@@ -319,31 +321,52 @@
             if trading_api.is_usd_like_coin(profile_data.trading.reference_market):
                 usd_like_asset = profile_data.trading.reference_market
             else:
                 usd_like_asset = "USDT"  # todo use dynamic value when exchange is not supporting USDT
             profile_data.trader_simulator.starting_portfolio = formatters.get_adapted_portfolio(
                 usd_like_asset, portfolio
             )
-        exchanges_config = (
-            # use product config exchanges when no exchange is set in bot_config and when in simulator mode
-            bot_config["product_config"][enums.ProfileConfigKeys.CONFIG.value]["exchanges"]
-            if profile_data.trader_simulator.enabled
-            # otherwise use botconfig exchange id
-            else bot_config[enums.BotConfigKeys.EXCHANGES.value] if bot_config[enums.BotConfigKeys.EXCHANGES.value]
-            else []
-        )
+        if profile_data.trader_simulator.enabled:
+            # attempt 1: set exchange using exchange_id when set in bot_config
+            exchange_ids = [
+                config["exchange_id"]
+                for config in bot_config["exchanges"]
+                if config.get("exchange_id", None)
+            ]
+            if exchange_ids:
+                exchanges = await self.fetch_exchanges(exchange_ids)
+                exchanges_config = [
+                    {enums.ExchangeKeys.INTERNAL_NAME.value: exchange[enums.ExchangeKeys.INTERNAL_NAME.value]}
+                    for exchange in exchanges
+                ]
+            else:
+                # attempt 2: fallback to exchange_internal_name in product config
+                exchanges_config = bot_config["product_config"][enums.ProfileConfigKeys.CONFIG.value]["exchanges"]
+        else:
+            # real trading: use bot_config and its exchange_credential_id
+            exchanges_config = (
+                bot_config[enums.BotConfigKeys.EXCHANGES.value]
+                if bot_config[enums.BotConfigKeys.EXCHANGES.value]
+                else []
+            )
         profile_data.exchanges = [
             commons_profiles.ExchangeData.from_dict(exchange_data)
             for exchange_data in exchanges_config
         ]
         if options := bot_config.get(enums.BotConfigKeys.OPTIONS.value):
             profile_data.options = commons_profiles.OptionsData.from_dict(options)
         profile_data.profile_details.id = bot_config_id
         return profile_data
 
+    async def fetch_exchanges(self, exchange_ids: list) -> list:
+        return (await self.table("exchanges").select(
+            f"{enums.ExchangeKeys.ID.value}, "
+            f"{enums.ExchangeKeys.INTERNAL_NAME.value}"
+        ).in_(enums.ExchangeKeys.ID.value, exchange_ids).execute()).data
+
     async def fetch_product_config(self, product_id: str) -> commons_profiles.ProfileData:
         if not product_id:
             raise errors.MissingProductConfigError(f"product_id is '{product_id}'")
         try:
             product = (await self.table("products").select(
                 "slug, "
                 "product_config:product_configs!current_config_id(config, version)"
```

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/configuration_storage.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/configuration_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/enums.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,33 @@
 
 
 class BotDeploymentErrorsStatuses(enum.Enum):
     NO_ERROR = None
     INTERNAL_SERVER_ERROR = "internal_server_error"
     INVALID_CONFIG = "invalid_config"
     INVALID_EXCHANGE_CREDENTIALS = "invalid_exchange_credentials"
+    INCOMPATIBLE_USER_EXCHANGE_ACCOUNT_WITH_CONFIG = "incompatible_user_exchange_account_with_config"
     ALREADY_USED_EXCHANGE_ACCOUNT = "already_used_exchange_account"
     MISSING_MINIMAL_FUNDS = "missing_minimal_funds"
     MISSING_CONFIG = "missing_config"
     EXPIRED_BOT = "expired_bot"
     MAX_SIMULATORS_REACHED = "max_simulators_reached"
 
 
 class ExchangeAccountStatuses(enum.Enum):
     NO_STATUS = None
     PENDING_PORTFOLIO_REFRESH = "pending_portfolio_refresh"
     NO_PENDING_ACTION = "no_pending_action"
 
 
+class ExchangeKeys(enum.Enum):
+    ID = "id"
+    INTERNAL_NAME = "internal_name"
+
+
 class SignalKeys(enum.Enum):
     ID = "id"
     TIME = "time"
     PRODUCT_ID = "product_id"
     SIGNAL = "signal"
```

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/postgres_functions.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/postgres_functions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/supabase_client.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/supabase_client.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_channel.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_client.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_client.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/community/supabase_backend/supabase_realtime_socket.py` & `OctoBot-1.0.9/octobot/community/supabase_backend/supabase_realtime_socket.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/config/config_schema.json` & `OctoBot-1.0.9/octobot/config/config_schema.json`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/config/logging_config.ini` & `OctoBot-1.0.9/octobot/config/logging_config.ini`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/config/profile_schema.json` & `OctoBot-1.0.9/octobot/config/profile_schema.json`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/configuration_manager.py` & `OctoBot-1.0.9/octobot/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/constants.py` & `OctoBot-1.0.9/octobot/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/databases_util.py` & `OctoBot-1.0.9/octobot/databases_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/disclaimer.py` & `OctoBot-1.0.9/octobot/disclaimer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/enums.py` & `OctoBot-1.0.9/octobot/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/errors.py` & `OctoBot-1.0.9/octobot/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/initializer.py` & `OctoBot-1.0.9/octobot/initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/limits.py` & `OctoBot-1.0.9/octobot/limits.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/logger.py` & `OctoBot-1.0.9/octobot/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,21 +274,21 @@
         f"MARK PRICE : EXCHANGE = {exchange} || CRYPTOCURRENCY = {cryptocurrency} "
         f"|| SYMBOL = {symbol} || MARK PRICE = {mark_price}"
     )
 
 
 def _filter_balance(balance: dict):
     if not balance:
-        return balance
+        return balance, 0
     first_value = next(iter(balance.values()))
     if isinstance(first_value, dict):
         filtered_balance = {
             key: values
             for key, values in balance.items()
-            if values[commons_constants.PORTFOLIO_TOTAL]
+            if values.get(commons_constants.PORTFOLIO_TOTAL)
         }
         removed_count = len(balance) - len(filtered_balance)
         return trading_api.parse_decimal_portfolio(filtered_balance, False), removed_count
     return balance, 0
 
 
 async def balance_callback(exchange: str, exchange_id: str, balance):
```

### Comparing `OctoBot-1.0.8/octobot/octobot.py` & `OctoBot-1.0.9/octobot/octobot.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/octobot_api.py` & `OctoBot-1.0.9/octobot/octobot_api.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/octobot_backtesting_factory.py` & `OctoBot-1.0.9/octobot/octobot_backtesting_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/octobot_channel_consumer.py` & `OctoBot-1.0.9/octobot/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/producers/__init__.py` & `OctoBot-1.0.9/octobot/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/producers/evaluator_producer.py` & `OctoBot-1.0.9/octobot/producers/evaluator_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/producers/exchange_producer.py` & `OctoBot-1.0.9/octobot/producers/exchange_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/producers/interface_producer.py` & `OctoBot-1.0.9/octobot/producers/interface_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/producers/service_feed_producer.py` & `OctoBot-1.0.9/octobot/producers/service_feed_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/storage/__init__.py` & `OctoBot-1.0.9/octobot/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/storage/db_databases_pruning.py` & `OctoBot-1.0.9/octobot/storage/db_databases_pruning.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/storage/trading_metadata.py` & `OctoBot-1.0.9/octobot/storage/trading_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/__init__.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/fitness_parameter.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/fitness_parameter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_constraint.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_constraint.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_filter.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/optimizer_settings.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/optimizer_settings.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/scored_run_result.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/scored_run_result.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/strategy_design_optimizer.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/strategy_design_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/strategy_design_optimizer_factory.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/strategy_design_optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/strategy_optimizer.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/strategy_test_suite.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/strategy_test_suite.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/strategy_optimizer/test_suite_result.py` & `OctoBot-1.0.9/octobot/strategy_optimizer/test_suite_result.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/task_manager.py` & `OctoBot-1.0.9/octobot/task_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/updater/__init__.py` & `OctoBot-1.0.9/octobot/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/updater/binary_updater.py` & `OctoBot-1.0.9/octobot/updater/binary_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/updater/python_updater.py` & `OctoBot-1.0.9/octobot/updater/python_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/updater/updater.py` & `OctoBot-1.0.9/octobot/updater/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/octobot/updater/updater_factory.py` & `OctoBot-1.0.9/octobot/updater/updater_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/requirements.txt` & `OctoBot-1.0.9/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Drakkar-Software requirements
-OctoBot-Commons==1.9.40
-OctoBot-Trading==2.4.55
-OctoBot-Evaluators==1.9.4
+OctoBot-Commons==1.9.43
+OctoBot-Trading==2.4.78
+OctoBot-Evaluators==1.9.5
 OctoBot-Tentacles-Manager==2.9.10
-OctoBot-Services==1.6.10
+OctoBot-Services==1.6.13
 OctoBot-Backtesting==1.9.7
 Async-Channel==2.2.1
-trading-backend==1.2.14
+trading-backend==1.2.19
 
 ## Others
 colorlog==6.8.0
 requests==2.31.0
 urllib3 # required by requests, used in imports: make sure it's always available
 packaging==23.2
 python-dotenv==1.0.0
```

### Comparing `OctoBot-1.0.8/setup.py` & `OctoBot-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/start.py` & `OctoBot-1.0.9/start.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/automations/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/automations/test_automation.py` & `OctoBot-1.0.9/tests/functional_tests/automations/test_automation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/backtesting_tests/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/backtesting_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/backtesting_tests/backtesting_test.py` & `OctoBot-1.0.9/tests/functional_tests/backtesting_tests/backtesting_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/evaluators_tests/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/evaluators_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/evaluators_tests/abstract_TA_test.py` & `OctoBot-1.0.9/tests/functional_tests/evaluators_tests/abstract_TA_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/launch_test/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/launch_test/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/launch_test/launch_test.py` & `OctoBot-1.0.9/tests/functional_tests/launch_test/launch_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/strategy_evaluators_tests/__init__.py` & `OctoBot-1.0.9/tests/functional_tests/strategy_evaluators_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py` & `OctoBot-1.0.9/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/__init__.py` & `OctoBot-1.0.9/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/bot_management.py` & `OctoBot-1.0.9/tests/test_utils/bot_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/config.py` & `OctoBot-1.0.9/tests/test_utils/config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/data_bank.py` & `OctoBot-1.0.9/tests/test_utils/data_bank.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/logging.py` & `OctoBot-1.0.9/tests/test_utils/logging.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/memory_check_util.py` & `OctoBot-1.0.9/tests/test_utils/memory_check_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,40 +15,43 @@
 #  License along with OctoBot. If not, see <https://www.gnu.org/licenses/>.
 import asyncio
 
 import octobot_commons.constants as commons_constants
 from octobot.api.backtesting import create_independent_backtesting, initialize_and_run_independent_backtesting, \
     check_independent_backtesting_remaining_objects, stop_independent_backtesting, join_independent_backtesting, \
     get_independent_backtesting_exchange_manager_ids
-from octobot.backtesting.abstract_backtesting_test import DATA_FILES
+from octobot.backtesting.abstract_backtesting_test import DATA_FILES, MULTI_ASSETS_DATA_FILE
 from octobot_commons.asyncio_tools import ErrorContainer
 from octobot_trading.api.exchange import get_exchange_manager_from_exchange_id
 from octobot_trading.api.orders import get_open_orders
 from octobot_trading.api.trades import get_trade_history
 
 
-async def run_independent_backtestings_with_memory_check(config, tentacles_setup_config, backtesting_count=3):
+async def run_independent_backtestings_with_memory_check(
+    config, tentacles_setup_config, backtesting_count=3, use_multiple_asset_data_file=False
+):
     """
     Will raise an error of an object is not deleted by garbage collector at the end of the backtesting process
     :param config: the global config to use in backtesting
     :param tentacles_setup_config: the tentacles setup config to use (with the tentacles to be tested)
     :param backtesting_count: number of backtestings to run to ensure no side effects, default is 3
+    :param use_multiple_asset_data_file: when True, a multi symbol data file will be used
     :return:
     """
     backtesting = None
     try:
         config[commons_constants.CONFIG_SIMULATOR][commons_constants.CONFIG_STARTING_PORTFOLIO]["USDT"] = 10000
         config[commons_constants.CONFIG_SIMULATOR][commons_constants.CONFIG_STARTING_PORTFOLIO]["ETH"] = 20
         for _ in range(backtesting_count):
             error_container = ErrorContainer()
             asyncio.get_event_loop().set_exception_handler(error_container.exception_handler)
             # enabling loggers is slowing down backtesting but can display useful debug info
             # from octobot.logger import init_logger
             # init_logger()
-            backtesting = await _run_backtesting(config, tentacles_setup_config)
+            backtesting = await _run_backtesting(config, tentacles_setup_config, use_multiple_asset_data_file)
             exchange_manager = get_exchange_manager_from_exchange_id(
                 get_independent_backtesting_exchange_manager_ids(backtesting)[0])
             trades = get_trade_history(exchange_manager)
             open_orders = get_open_orders(exchange_manager)
             # ensure at least one order is either open or got filled
             assert trades + open_orders
             trades = open_orders = exchange_manager = None  # prevent memory leak
@@ -60,13 +63,15 @@
         if backtesting is not None:
             # do not get stuck in running backtesting
             await stop_independent_backtesting(backtesting, memory_check=False)
             await asyncio.wait_for(backtesting.post_backtesting_task, 5)
         raise e
 
 
-async def _run_backtesting(config, tentacles_setup_config):
-    backtesting = create_independent_backtesting(config, tentacles_setup_config, [DATA_FILES["ETH/USDT"]], "",
-                                                 enable_storage=False)
+async def _run_backtesting(config, tentacles_setup_config, use_multiple_asset_data_file):
+    data_file = MULTI_ASSETS_DATA_FILE if use_multiple_asset_data_file else DATA_FILES["ETH/USDT"]
+    backtesting = create_independent_backtesting(
+        config, tentacles_setup_config, [data_file], "", enable_storage=False
+    )
     await initialize_and_run_independent_backtesting(backtesting, log_errors=False)
     await join_independent_backtesting(backtesting)
     return backtesting
```

### Comparing `OctoBot-1.0.8/tests/test_utils/order_util.py` & `OctoBot-1.0.9/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/test_exchanges.py` & `OctoBot-1.0.9/tests/test_utils/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/test_utils/trading_modes.py` & `OctoBot-1.0.9/tests/test_utils/trading_modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/__init__.py` & `OctoBot-1.0.9/tests/unit_tests/community/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/errors_upload/__init__.py` & `OctoBot-1.0.9/tests/unit_tests/community/errors_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_error_model.py` & `OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_error_model.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_errors_uploader.py` & `OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_errors_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_initializer.py` & `OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/errors_upload/test_sentry_aiohttp_transport.py` & `OctoBot-1.0.9/tests/unit_tests/community/errors_upload/test_sentry_aiohttp_transport.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/test_authentication.py` & `OctoBot-1.0.9/tests/unit_tests/community/test_authentication.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/test_community_data.py` & `OctoBot-1.0.9/tests/unit_tests/community/test_community_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/test_community_supabase_feed.py` & `OctoBot-1.0.9/tests/unit_tests/community/test_community_supabase_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/community/test_community_ws_feed.py` & `OctoBot-1.0.9/tests/unit_tests/community/test_community_ws_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/__init__.py` & `OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_design_optimizer.py` & `OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_design_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py` & `OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py` & `OctoBot-1.0.9/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/test_configuration_manager.py` & `OctoBot-1.0.9/tests/unit_tests/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/trading_modes_tests/__init__.py` & `OctoBot-1.0.9/tests/unit_tests/trading_modes_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py` & `OctoBot-1.0.9/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/updater/__init__.py` & `OctoBot-1.0.9/tests/unit_tests/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-1.0.8/tests/unit_tests/updater/test_updater.py` & `OctoBot-1.0.9/tests/unit_tests/updater/test_updater.py`

 * *Files identical despite different names*

