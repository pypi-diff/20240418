# Comparing `tmp/trl-0.8.3.tar.gz` & `tmp/trl-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.8.3.tar", last modified: Fri Apr 12 10:19:08 2024, max compression
+gzip compressed data, was "trl-0.8.4.tar", last modified: Wed Apr 17 15:12:51 2024, max compression
```

## Comparing `trl-0.8.3.tar` & `trl-0.8.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.882650 trl-0.8.3/
--rw-rw-r--   0 younes   (150078) younes   (150078)     2507 2024-04-12 10:17:44.000000 trl-0.8.3/CONTRIBUTING.md
--rw-rw-r--   0 younes   (150078) younes   (150078)    11357 2023-06-01 10:19:35.000000 trl-0.8.3/LICENSE
--rw-rw-r--   0 younes   (150078) younes   (150078)      110 2024-04-12 10:17:44.000000 trl-0.8.3/MANIFEST.in
--rw-rw-r--   0 younes   (150078) younes   (150078)    10388 2024-04-12 10:19:08.882650 trl-0.8.3/PKG-INFO
--rw-rw-r--   0 younes   (150078) younes   (150078)     9273 2024-04-12 10:17:44.000000 trl-0.8.3/README.md
--rw-rw-r--   0 younes   (150078) younes   (150078)      509 2024-03-15 11:31:17.000000 trl-0.8.3/pyproject.toml
--rw-rw-r--   0 younes   (150078) younes   (150078)       73 2024-04-12 10:19:08.882650 trl-0.8.3/setup.cfg
--rw-rw-r--   0 younes   (150078) younes   (150078)     4547 2024-04-12 10:18:01.000000 trl-0.8.3/setup.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.874650 trl-0.8.3/tests/
--rw-rw-r--   0 younes   (150078) younes   (150078)        0 2023-06-01 10:19:35.000000 trl-0.8.3/tests/__init__.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.874650 trl-0.8.3/tests/slow/
--rw-rw-r--   0 younes   (150078) younes   (150078)        0 2024-01-30 06:55:37.000000 trl-0.8.3/tests/slow/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7757 2024-03-15 11:31:17.000000 trl-0.8.3/tests/slow/test_dpo_slow.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14741 2024-03-15 11:31:17.000000 trl-0.8.3/tests/slow/test_sft_slow.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1082 2024-01-30 06:55:37.000000 trl-0.8.3/tests/slow/testing_constants.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3158 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_best_of_n_sampler.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1723 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_cli.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1545 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_core.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6283 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_cpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5505 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_data_collator_completion_only.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6894 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_dataset_formatting.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4168 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_ddpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    22515 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_dpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)      152 2023-09-22 13:56:18.000000 trl-0.8.3/tests/test_e2e.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    11127 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_environments.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4597 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_iterative_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14983 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_kto_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    22746 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_modeling_value_head.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5560 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_no_peft.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6119 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_orpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     9122 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_peft_models.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    47392 2024-03-15 11:31:17.000000 trl-0.8.3/tests/test_ppo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    13419 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_reward_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1640 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_rich_progress_callback.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    43099 2024-04-12 10:17:44.000000 trl-0.8.3/tests/test_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)      799 2023-06-01 10:19:35.000000 trl-0.8.3/tests/testing_constants.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3342 2024-04-12 10:17:44.000000 trl-0.8.3/tests/testing_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.874650 trl-0.8.3/trl/
--rw-rw-r--   0 younes   (150078) younes   (150078)     3931 2024-04-12 10:18:05.000000 trl-0.8.3/trl/__init__.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/commands/
--rw-rw-r--   0 younes   (150078) younes   (150078)     1207 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     2367 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/cli.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    12965 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/cli_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/commands/scripts/
--rw-rw-r--   0 younes   (150078) younes   (150078)    12612 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/chat.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/commands/scripts/config/
--rw-rw-r--   0 younes   (150078) younes   (150078)      487 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/config/default_chat_config.yaml
--rw-rw-r--   0 younes   (150078) younes   (150078)     4003 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/cpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6500 2024-03-15 11:31:17.000000 trl-0.8.3/trl/commands/scripts/ddpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6054 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/dpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3729 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/kto.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4057 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/orpo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7646 2024-03-15 11:31:17.000000 trl-0.8.3/trl/commands/scripts/ppo.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5261 2024-03-15 11:31:17.000000 trl-0.8.3/trl/commands/scripts/ppo_multi_adapter.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4596 2024-03-15 11:31:17.000000 trl-0.8.3/trl/commands/scripts/reward_modeling.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4730 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/sft.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     7371 2024-04-12 10:17:44.000000 trl-0.8.3/trl/commands/scripts/vsft_llava.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    12148 2024-03-15 11:31:17.000000 trl-0.8.3/trl/core.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/environment/
--rw-rw-r--   0 younes   (150078) younes   (150078)      390 2024-03-15 11:31:17.000000 trl-0.8.3/trl/environment/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    17569 2024-03-15 11:31:17.000000 trl-0.8.3/trl/environment/base_environment.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/extras/
--rw-rw-r--   0 younes   (150078) younes   (150078)      971 2024-03-15 11:31:17.000000 trl-0.8.3/trl/extras/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5182 2024-03-15 11:31:17.000000 trl-0.8.3/trl/extras/best_of_n_sampler.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3646 2024-01-30 06:55:37.000000 trl-0.8.3/trl/extras/dataset_formatting.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6079 2024-04-12 10:17:44.000000 trl-0.8.3/trl/import_utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl/models/
--rw-rw-r--   0 younes   (150078) younes   (150078)     2208 2024-04-12 10:17:44.000000 trl-0.8.3/trl/models/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    28788 2024-03-15 11:31:17.000000 trl-0.8.3/trl/models/modeling_base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    27695 2024-03-15 11:31:17.000000 trl-0.8.3/trl/models/modeling_sd_base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    18933 2024-04-12 10:17:44.000000 trl-0.8.3/trl/models/modeling_value_head.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     5874 2024-03-15 11:31:17.000000 trl-0.8.3/trl/models/sd_utils.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     6026 2024-04-12 10:17:44.000000 trl-0.8.3/trl/models/utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.882650 trl-0.8.3/trl/trainer/
--rw-rw-r--   0 younes   (150078) younes   (150078)     3343 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/__init__.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1772 2023-06-01 10:19:35.000000 trl-0.8.3/trl/trainer/base.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3875 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/cpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    44118 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/cpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4891 2024-03-15 11:31:17.000000 trl-0.8.3/trl/trainer/ddpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    26796 2024-03-15 11:31:17.000000 trl-0.8.3/trl/trainer/ddpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    62510 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/dpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    16699 2024-03-15 11:31:17.000000 trl-0.8.3/trl/trainer/iterative_sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     4970 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/kto_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    63623 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/kto_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3297 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/model_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     3500 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/orpo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    45703 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/orpo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     8202 2024-01-30 06:55:37.000000 trl-0.8.3/trl/trainer/ppo_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    63097 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/ppo_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)     1623 2024-01-30 06:55:37.000000 trl-0.8.3/trl/trainer/reward_config.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    14097 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/reward_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    27414 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/sft_trainer.py
--rw-rw-r--   0 younes   (150078) younes   (150078)    35309 2024-04-12 10:17:44.000000 trl-0.8.3/trl/trainer/utils.py
-drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-12 10:19:08.878650 trl-0.8.3/trl.egg-info/
--rw-r--r--   0 younes   (150078) younes   (150078)    10388 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/PKG-INFO
--rw-rw-r--   0 younes   (150078) younes   (150078)     2346 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/SOURCES.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)        1 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/dependency_links.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)       46 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/entry_points.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)        1 2023-06-01 10:19:45.000000 trl-0.8.3/trl.egg-info/not-zip-safe
--rw-rw-r--   0 younes   (150078) younes   (150078)      519 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/requires.txt
--rw-rw-r--   0 younes   (150078) younes   (150078)       10 2024-04-12 10:19:08.000000 trl-0.8.3/trl.egg-info/top_level.txt
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.631469 trl-0.8.4/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2507 2024-04-12 10:22:24.000000 trl-0.8.4/CONTRIBUTING.md
+-rw-rw-r--   0 younes   (150078) younes   (150078)    11357 2023-06-01 10:19:35.000000 trl-0.8.4/LICENSE
+-rw-rw-r--   0 younes   (150078) younes   (150078)      110 2024-04-12 10:22:24.000000 trl-0.8.4/MANIFEST.in
+-rw-rw-r--   0 younes   (150078) younes   (150078)    10388 2024-04-17 15:12:51.631469 trl-0.8.4/PKG-INFO
+-rw-rw-r--   0 younes   (150078) younes   (150078)     9273 2024-04-12 10:22:24.000000 trl-0.8.4/README.md
+-rw-rw-r--   0 younes   (150078) younes   (150078)      509 2024-04-12 10:22:24.000000 trl-0.8.4/pyproject.toml
+-rw-rw-r--   0 younes   (150078) younes   (150078)       73 2024-04-17 15:12:51.631469 trl-0.8.4/setup.cfg
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4547 2024-04-17 15:12:08.000000 trl-0.8.4/setup.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/tests/
+-rw-rw-r--   0 younes   (150078) younes   (150078)        0 2023-06-01 10:19:35.000000 trl-0.8.4/tests/__init__.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/tests/slow/
+-rw-rw-r--   0 younes   (150078) younes   (150078)        0 2024-01-30 06:55:37.000000 trl-0.8.4/tests/slow/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7757 2024-04-12 10:22:24.000000 trl-0.8.4/tests/slow/test_dpo_slow.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14741 2024-04-12 10:22:24.000000 trl-0.8.4/tests/slow/test_sft_slow.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1082 2024-01-30 06:55:37.000000 trl-0.8.4/tests/slow/testing_constants.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3158 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_best_of_n_sampler.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1749 2024-04-17 15:11:50.000000 trl-0.8.4/tests/test_cli.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1545 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_core.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6283 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_cpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5505 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_data_collator_completion_only.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6894 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_dataset_formatting.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4168 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_ddpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    22515 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_dpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)      152 2023-09-22 13:56:18.000000 trl-0.8.4/tests/test_e2e.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    11127 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_environments.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4597 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_iterative_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14983 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_kto_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    22746 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_modeling_value_head.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5560 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_no_peft.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6119 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_orpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     9122 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_peft_models.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    49544 2024-04-17 15:11:50.000000 trl-0.8.4/tests/test_ppo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    13419 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_reward_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1640 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_rich_progress_callback.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    43099 2024-04-12 10:22:24.000000 trl-0.8.4/tests/test_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)      799 2023-06-01 10:19:35.000000 trl-0.8.4/tests/testing_constants.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3342 2024-04-12 10:22:24.000000 trl-0.8.4/tests/testing_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3931 2024-04-17 15:12:00.000000 trl-0.8.4/trl/__init__.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl/commands/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1207 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2367 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/cli.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    12963 2024-04-17 15:11:50.000000 trl-0.8.4/trl/commands/cli_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl/commands/scripts/
+-rw-rw-r--   0 younes   (150078) younes   (150078)    12612 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/chat.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl/commands/scripts/config/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      487 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/config/default_chat_config.yaml
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4003 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/cpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6500 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/ddpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6054 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/dpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3729 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/kto.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4057 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/orpo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7646 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/ppo.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5261 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/ppo_multi_adapter.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4596 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/reward_modeling.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4730 2024-04-12 10:22:24.000000 trl-0.8.4/trl/commands/scripts/sft.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     7657 2024-04-17 15:11:50.000000 trl-0.8.4/trl/commands/scripts/vsft_llava.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    12148 2024-04-12 10:22:24.000000 trl-0.8.4/trl/core.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl/environment/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      390 2024-04-12 10:22:24.000000 trl-0.8.4/trl/environment/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    17569 2024-04-12 10:22:24.000000 trl-0.8.4/trl/environment/base_environment.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.631469 trl-0.8.4/trl/extras/
+-rw-rw-r--   0 younes   (150078) younes   (150078)      971 2024-04-12 10:22:24.000000 trl-0.8.4/trl/extras/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5182 2024-04-12 10:22:24.000000 trl-0.8.4/trl/extras/best_of_n_sampler.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3646 2024-01-30 06:55:37.000000 trl-0.8.4/trl/extras/dataset_formatting.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6079 2024-04-12 10:22:24.000000 trl-0.8.4/trl/import_utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.631469 trl-0.8.4/trl/models/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2208 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    28788 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/modeling_base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    27695 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/modeling_sd_base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    18933 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/modeling_value_head.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     5874 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/sd_utils.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     6026 2024-04-12 10:22:24.000000 trl-0.8.4/trl/models/utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.631469 trl-0.8.4/trl/trainer/
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3343 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/__init__.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1772 2023-06-01 10:19:35.000000 trl-0.8.4/trl/trainer/base.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3875 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/cpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    44127 2024-04-17 15:11:50.000000 trl-0.8.4/trl/trainer/cpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4891 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/ddpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    26796 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/ddpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    62510 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/dpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    16699 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/iterative_sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     4970 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/kto_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    64532 2024-04-17 15:11:50.000000 trl-0.8.4/trl/trainer/kto_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3297 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/model_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     3500 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/orpo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    45703 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/orpo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     8202 2024-01-30 06:55:37.000000 trl-0.8.4/trl/trainer/ppo_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    63096 2024-04-17 15:11:50.000000 trl-0.8.4/trl/trainer/ppo_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)     1623 2024-01-30 06:55:37.000000 trl-0.8.4/trl/trainer/reward_config.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    14097 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/reward_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    27414 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/sft_trainer.py
+-rw-rw-r--   0 younes   (150078) younes   (150078)    35309 2024-04-12 10:22:24.000000 trl-0.8.4/trl/trainer/utils.py
+drwxrwxr-x   0 younes   (150078) younes   (150078)        0 2024-04-17 15:12:51.627469 trl-0.8.4/trl.egg-info/
+-rw-r--r--   0 younes   (150078) younes   (150078)    10388 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/PKG-INFO
+-rw-rw-r--   0 younes   (150078) younes   (150078)     2346 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/SOURCES.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)        1 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/dependency_links.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)       46 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/entry_points.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)        1 2023-06-01 10:19:45.000000 trl-0.8.4/trl.egg-info/not-zip-safe
+-rw-rw-r--   0 younes   (150078) younes   (150078)      519 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/requires.txt
+-rw-rw-r--   0 younes   (150078) younes   (150078)       10 2024-04-17 15:12:51.000000 trl-0.8.4/trl.egg-info/top_level.txt
```

### Comparing `trl-0.8.3/CONTRIBUTING.md` & `trl-0.8.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/LICENSE` & `trl-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/PKG-INFO` & `trl-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.3
+Version: 0.8.4
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.3 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.4 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
```

### Comparing `trl-0.8.3/README.md` & `trl-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/setup.py` & `trl-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    Then push the change with a message 'set dev version'
 """
 import os
 
 from setuptools import find_packages, setup
 
 
-__version__ = "0.8.3"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+__version__ = "0.8.4"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.31.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
```

### Comparing `trl-0.8.3/tests/slow/test_dpo_slow.py` & `trl-0.8.4/tests/slow/test_dpo_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/slow/test_sft_slow.py` & `trl-0.8.4/tests/slow/test_sft_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/slow/testing_constants.py` & `trl-0.8.4/tests/slow/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_best_of_n_sampler.py` & `trl-0.8.4/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_cli.py` & `trl-0.8.4/tests/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import unittest
 
 
 @unittest.skipIf(sys.platform.startswith("win"), "Skipping on Windows")
 def test_sft_cli():
     try:
         subprocess.run(
-            "trl sft --max_steps 1 --output_dir tmp-sft --model_name_or_path HuggingFaceM4/tiny-random-LlamaForCausalLM --dataset_name imdb --learning_rate 1e-4 --lr_scheduler_type cosine",
+            "trl sft --max_steps 1 --output_dir tmp-sft --model_name_or_path HuggingFaceM4/tiny-random-LlamaForCausalLM --dataset_name imdb --learning_rate 1e-4 --lr_scheduler_type cosine --dataset_text_field text",
             shell=True,
             check=True,
         )
     except BaseException as exc:
         raise AssertionError("An error occured while running the CLI, please double check") from exc
```

### Comparing `trl-0.8.3/tests/test_core.py` & `trl-0.8.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_cpo_trainer.py` & `trl-0.8.4/tests/test_cpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_data_collator_completion_only.py` & `trl-0.8.4/tests/test_data_collator_completion_only.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_dataset_formatting.py` & `trl-0.8.4/tests/test_dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_ddpo_trainer.py` & `trl-0.8.4/tests/test_ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_dpo_trainer.py` & `trl-0.8.4/tests/test_dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_environments.py` & `trl-0.8.4/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_iterative_sft_trainer.py` & `trl-0.8.4/tests/test_iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_kto_trainer.py` & `trl-0.8.4/tests/test_kto_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_modeling_value_head.py` & `trl-0.8.4/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_no_peft.py` & `trl-0.8.4/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_orpo_trainer.py` & `trl-0.8.4/tests/test_orpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_peft_models.py` & `trl-0.8.4/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_ppo_trainer.py` & `trl-0.8.4/tests/test_ppo_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1138,14 +1138,63 @@
         generations_batched = tokenizer.batch_decode(generations_batched)
 
         generations_single = [ppo_trainer.generate(inputs, **generation_kwargs).squeeze() for inputs in model_inputs]
         generations_single = tokenizer.batch_decode(generations_single)
 
         assert generations_single == generations_batched
 
+    def test_generation_with_ref_model(self):
+        dummy_dataset = self._init_dummy_dataset()
+        model = AutoModelForCausalLMWithValueHead.from_pretrained("gpt2")
+        tokenizer = AutoTokenizer.from_pretrained("gpt2")
+
+        # Negate the weights in the last layer of the ref model so it never
+        # outputs the same things as the primary model
+        ref_model = copy.deepcopy(model)
+        lm_head_weight = ref_model.pretrained_model.lm_head.weight
+        lm_head_weight.data = -lm_head_weight.data
+
+        ppo_trainer = PPOTrainer(
+            config=self.ppo_config,
+            model=model,
+            ref_model=ref_model,
+            tokenizer=tokenizer,
+            dataset=dummy_dataset,
+        )
+
+        input_texts = ["this is a test", "this is another, longer test"]
+
+        generation_kwargs = {"do_sample": False, "max_new_tokens": 4, "pad_token_id": tokenizer.eos_token_id}
+
+        tokenizer.pad_token = tokenizer.eos_token
+
+        model_inputs = [tokenizer(txt, return_tensors="pt").input_ids.squeeze() for txt in input_texts]
+
+        generations_batched, ref_generations_batched = ppo_trainer.generate(
+            model_inputs, batch_size=2, generate_ref_response=True, **generation_kwargs
+        )
+        generations_batched = tokenizer.batch_decode(generations_batched)
+        ref_generations_batched = tokenizer.batch_decode(ref_generations_batched)
+
+        generations_single = []
+        ref_generations_single = []
+        for inputs in model_inputs:
+            generation, ref_generation = ppo_trainer.generate(inputs, generate_ref_response=True, **generation_kwargs)
+            generations_single.append(generation.squeeze())
+            ref_generations_single.append(ref_generation.squeeze())
+
+        generations_single = tokenizer.batch_decode(generations_single)
+        ref_generations_single = tokenizer.batch_decode(ref_generations_single)
+
+        assert generations_single == generations_batched
+        assert ref_generations_single == ref_generations_batched
+
+        assert generations_batched != ref_generations_batched
+        assert generations_single != ref_generations_single
+
     def test_grad_accumulation(self):
         dummy_dataset = self._init_dummy_dataset()
 
         torch.manual_seed(0)
         gpt2_model = AutoModelForCausalLMWithValueHead.from_pretrained(self.model_id, summary_dropout_prob=0.0)
         gpt2_model_clone = copy.deepcopy(gpt2_model)
```

### Comparing `trl-0.8.3/tests/test_reward_trainer.py` & `trl-0.8.4/tests/test_reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_rich_progress_callback.py` & `trl-0.8.4/tests/test_rich_progress_callback.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/test_sft_trainer.py` & `trl-0.8.4/tests/test_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/testing_constants.py` & `trl-0.8.4/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/tests/testing_utils.py` & `trl-0.8.4/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/__init__.py` & `trl-0.8.4/trl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 from typing import TYPE_CHECKING
 from .import_utils import _LazyModule, is_diffusers_available, OptionalDependencyNotAvailable
 
 _import_structure = {
     "core": [
         "set_seed",
```

### Comparing `trl-0.8.3/trl/commands/__init__.py` & `trl-0.8.4/trl/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/cli.py` & `trl-0.8.4/trl/commands/cli.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/cli_utils.py` & `trl-0.8.4/trl/commands/cli_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     # Add the custom warning handler - we need to do that before importing anything to make sure the loggers work well
     warnings.showwarning = warning_handler
 
 
 @dataclass
 class SftScriptArguments:
     dataset_name: str = field(default="timdettmers/openassistant-guanaco", metadata={"help": "the dataset name"})
-    dataset_text_field: str = field(default="text", metadata={"help": "the text field of the dataset"})
+    dataset_text_field: str = field(default=None, metadata={"help": "the text field of the dataset"})
     max_seq_length: int = field(default=512, metadata={"help": "The maximum sequence length for SFT Trainer"})
     packing: bool = field(default=False, metadata={"help": "Whether to apply data packing or not during training"})
     config: str = field(default=None, metadata={"help": "Path to the optional config file"})
     gradient_checkpointing_use_reentrant: bool = field(
         default=False, metadata={"help": "Whether to apply `use_reentrant` for gradient_checkpointing"}
     )
```

### Comparing `trl-0.8.3/trl/commands/scripts/chat.py` & `trl-0.8.4/trl/commands/scripts/chat.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/cpo.py` & `trl-0.8.4/trl/commands/scripts/cpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/ddpo.py` & `trl-0.8.4/trl/commands/scripts/ddpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/dpo.py` & `trl-0.8.4/trl/commands/scripts/dpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/kto.py` & `trl-0.8.4/trl/commands/scripts/kto.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/orpo.py` & `trl-0.8.4/trl/commands/scripts/orpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/ppo.py` & `trl-0.8.4/trl/commands/scripts/ppo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/ppo_multi_adapter.py` & `trl-0.8.4/trl/commands/scripts/ppo_multi_adapter.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/reward_modeling.py` & `trl-0.8.4/trl/commands/scripts/reward_modeling.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/sft.py` & `trl-0.8.4/trl/commands/scripts/sft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/commands/scripts/vsft_llava.py` & `trl-0.8.4/trl/commands/scripts/vsft_llava.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     init_zero_verbose()
     FORMAT = "%(message)s"
 
     from rich.console import Console
     from rich.logging import RichHandler
 
 import torch
+from accelerate import Accelerator
 from datasets import load_dataset
 
 from tqdm.rich import tqdm
 from transformers import AutoTokenizer, AutoProcessor, TrainingArguments, LlavaForConditionalGeneration
 
 from trl import (
     ModelConfig,
@@ -107,15 +108,15 @@
     if TRL_USE_RICH:
         training_args.disable_tqdm = True
         console = Console()
 
     ################
     # Model, Tokenizer & Processor
     ################
-    LLAVA_CHAT_TEMPLATE = """A chat between a curious user and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the user's questions. {% for message in messages %}{% if message['role'] == 'user' %}USER: {% else %}ASSISTANT: {% endif %}{% for item in message['content'] %}{% if item['type'] == 'text' %}{{ item['text'] }}{% elif item['type'] == 'image' %}<image>{% endif %}{% endfor %}{% if message['role'] == 'user' %} {% else %}{{eos_token}}{% endif %}{% endfor %}"""
+    LLAVA_CHAT_TEMPLATE = """{% if not add_generation_prompt is defined %}{% set add_generation_prompt = false %}{% endif %}A chat between a curious user and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the user's questions. {% for message in messages %}{% if message['role'] == 'user' %}USER: {% else %}ASSISTANT: {% endif %}{% for item in message['content'] %}{% if item['type'] == 'text' %}{{ item['text'] }}{% elif item['type'] == 'image' %}<image>{% endif %}{% endfor %}{% if message['role'] == 'user' %} {% else %}{{eos_token}}{% endif %}{% endfor %}{% if add_generation_prompt %}ASSISTANT: {% endif %}"""
 
     torch_dtype = (
         model_config.torch_dtype
         if model_config.torch_dtype in ["auto", None]
         else getattr(torch, model_config.torch_dtype)
     )
     quantization_config = get_quantization_config(model_config)
@@ -201,7 +202,9 @@
         )
 
     trainer.train()
 
     with save_context:
         trainer.save_model(training_args.output_dir)
         trainer.push_to_hub()
+        if Accelerator().is_main_process:
+            processor.push_to_hub(training_args.hub_model_id)
```

### Comparing `trl-0.8.3/trl/core.py` & `trl-0.8.4/trl/core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/environment/base_environment.py` & `trl-0.8.4/trl/environment/base_environment.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/extras/__init__.py` & `trl-0.8.4/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/extras/best_of_n_sampler.py` & `trl-0.8.4/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/extras/dataset_formatting.py` & `trl-0.8.4/trl/extras/dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/import_utils.py` & `trl-0.8.4/trl/import_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/__init__.py` & `trl-0.8.4/trl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/modeling_base.py` & `trl-0.8.4/trl/models/modeling_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/modeling_sd_base.py` & `trl-0.8.4/trl/models/modeling_sd_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/modeling_value_head.py` & `trl-0.8.4/trl/models/modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/sd_utils.py` & `trl-0.8.4/trl/models/sd_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/models/utils.py` & `trl-0.8.4/trl/models/utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/__init__.py` & `trl-0.8.4/trl/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/base.py` & `trl-0.8.4/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/cpo_config.py` & `trl-0.8.4/trl/trainer/cpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/cpo_trainer.py` & `trl-0.8.4/trl/trainer/cpo_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,15 +734,15 @@
         metrics[f"{prefix}rewards/rejected"] = rejected_rewards.mean().cpu()
         metrics[f"{prefix}rewards/accuracies"] = reward_accuracies.mean().cpu()
         metrics[f"{prefix}rewards/margins"] = (chosen_rewards - rejected_rewards).mean().cpu()
         metrics[f"{prefix}logps/rejected"] = policy_rejected_logps.detach().mean().cpu()
         metrics[f"{prefix}logps/chosen"] = policy_chosen_logps.detach().mean().cpu()
         metrics[f"{prefix}logits/rejected"] = policy_rejected_logits.detach().mean().cpu()
         metrics[f"{prefix}logits/chosen"] = policy_chosen_logits.detach().mean().cpu()
-        metrics[f"{prefix}nll_loss"] = policy_nll_loss.cpu().mean()
+        metrics[f"{prefix}nll_loss"] = policy_nll_loss.detach().mean().cpu()
 
         return loss, metrics
 
     def compute_loss(
         self,
         model: Union[PreTrainedModel, nn.Module],
         inputs: Dict[str, Union[torch.Tensor, Any]],
```

### Comparing `trl-0.8.3/trl/trainer/ddpo_config.py` & `trl-0.8.4/trl/trainer/ddpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/ddpo_trainer.py` & `trl-0.8.4/trl/trainer/ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/dpo_trainer.py` & `trl-0.8.4/trl/trainer/dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/iterative_sft_trainer.py` & `trl-0.8.4/trl/trainer/iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/kto_config.py` & `trl-0.8.4/trl/trainer/kto_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/kto_trainer.py` & `trl-0.8.4/trl/trainer/kto_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 import random
 import warnings
 from collections import defaultdict
-from contextlib import nullcontext
+from contextlib import contextmanager, nullcontext
 from copy import deepcopy
 from functools import wraps
 from operator import itemgetter
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import torch
@@ -253,14 +253,18 @@
         peft_config (`Dict`, defaults to `None`):
             The PEFT configuration to use for training. If you pass a PEFT configuration, the model will be wrapped in a PEFT model.
         disable_dropout (`bool`, defaults to `True`):
             Whether or not to disable dropouts in `model` and `ref_model`.
         compute_metrics (`Callable[[EvalPrediction], Dict]`, *optional*):
             The function to use to compute the metrics. Must take a `EvalPrediction` and return
             a dictionary string to metric values.
+        model_adapter_name (`str`, defaults to `None`):
+            Name of the train target PEFT adapter, when using LoRA with multiple adapters.
+        ref_adapter_name (`str`, defaults to `None`):
+            Name of the reference PEFT adapter, when using LoRA with multiple adapters.
     """
 
     _tag_names = ["trl", "kto"]
 
     def __init__(
         self,
         model: Union[PreTrainedModel, nn.Module, str] = None,
@@ -272,14 +276,16 @@
         data_collator: Optional[DataCollator] = None,
         model_init: Optional[Callable[[], PreTrainedModel]] = None,
         callbacks: Optional[List[TrainerCallback]] = None,
         optimizers: Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR] = (None, None),
         preprocess_logits_for_metrics: Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]] = None,
         peft_config: Optional[Dict] = None,
         compute_metrics: Optional[Callable[[EvalLoopOutput], Dict]] = None,
+        model_adapter_name: Optional[str] = None,
+        ref_adapter_name: Optional[str] = None,
     ):
         if type(args) == TrainingArguments:
             raise ValueError("Please use `KTOConfig` instead TrainingArguments.")
 
         if args.model_init_kwargs is None:
             model_init_kwargs = {}
         elif not isinstance(model, str):
@@ -388,14 +394,16 @@
             self.is_encoder_decoder = model.config.is_encoder_decoder
         elif args.is_encoder_decoder is None:
             raise ValueError("When no model is provided, you need to pass the parameter is_encoder_decoder.")
         else:
             self.is_encoder_decoder = args.is_encoder_decoder
 
         self.is_peft_model = is_peft_available() and isinstance(model, PeftModel)
+        self.model_adapter_name = model_adapter_name
+        self.ref_adapter_name = ref_adapter_name
 
         if ref_model:
             self.ref_model = ref_model
         elif self.is_peft_model or args.precompute_ref_log_probs:
             # The `model` with adapters turned off will be used as the reference model
             self.ref_model = None
         else:
@@ -673,14 +681,26 @@
         # Otherwise, we assume the reference model fits in memory and is initialized on each device with ZeRO disabled (stage 0)
         if config_kwargs["zero_optimization"]["stage"] != 3:
             config_kwargs["zero_optimization"]["stage"] = 0
         model, *_ = deepspeed.initialize(model=model, config=config_kwargs)
         model.eval()
         return model
 
+    @contextmanager
+    def null_ref_context(self):
+        """Context manager for handling null reference model (that is, peft adapter manipulation)."""
+        with self.accelerator.unwrap_model(
+            self.model
+        ).disable_adapter() if self.is_peft_model and not self.ref_adapter_name else nullcontext():
+            if self.ref_adapter_name:
+                self.model.set_adapter(self.ref_adapter_name)
+            yield
+            if self.ref_adapter_name:
+                self.model.set_adapter(self.model_adapter_name or "default")
+
     def get_train_dataloader(self) -> DataLoader:
         """
         Returns the training [`~torch.utils.data.DataLoader`].
 
         Subclass of transformers.src.transformers.trainer.get_train_dataloader to precompute `ref_log_probs`.
         """
 
@@ -771,17 +791,15 @@
 
         return super().get_eval_dataloader(eval_dataset=eval_dataset)
 
     def compute_reference_log_probs(self, padded_batch: Dict) -> Dict:
         """Computes log probabilities of the reference model for a single padded batch of a KTO specific dataset."""
         with torch.no_grad():
             if self.ref_model is None:
-                with self.accelerator.unwrap_model(
-                    self.model
-                ).disable_adapter() if self.is_peft_model else nullcontext():
+                with self.null_ref_context():
                     if self.is_encoder_decoder:
                         completion_logits = self.model(
                             padded_batch["prompt_input_ids"],
                             attention_mask=padded_batch["prompt_attention_mask"],
                             decoder_input_ids=padded_batch.get("completion_decoder_input_ids"),
                             labels=padded_batch["completion_labels"],
                         ).logits
@@ -1025,15 +1043,15 @@
 
             reference_chosen_logps = batch["reference_logps"][chosen_idx, ...]
             reference_rejected_logps = batch["reference_logps"][rejected_idx, ...]
             reference_KL_logps = batch["reference_KL_logps"]
         else:
             with torch.no_grad():
                 if self.ref_model is None:
-                    with self.accelerator.unwrap_model(self.model).disable_adapter():
+                    with self.null_ref_context():
                         (
                             reference_chosen_logps,
                             reference_rejected_logps,
                             _,
                             _,
                             reference_KL_logps,
                         ) = self.forward(self.model, batch)
```

### Comparing `trl-0.8.3/trl/trainer/model_config.py` & `trl-0.8.4/trl/trainer/model_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/orpo_config.py` & `trl-0.8.4/trl/trainer/orpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/orpo_trainer.py` & `trl-0.8.4/trl/trainer/orpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/ppo_config.py` & `trl-0.8.4/trl/trainer/ppo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/ppo_trainer.py` & `trl-0.8.4/trl/trainer/ppo_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
                 generation_kwargs["max_new_tokens"] = length_sampler()
 
             with unwrap_model_for_generation(self.model, self.accelerator) as unwrapped_model:
                 response = unwrapped_model.generate(input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs)
 
             if generate_ref_response:
                 with unwrap_model_for_generation(
-                    self.model, self.accelerator, is_peft_model=self.is_peft_model
+                    ref_model, self.accelerator, is_peft_model=self.is_peft_model
                 ) as unwrapped_model:
                     ref_response = unwrapped_model.generate(
                         input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs
                     )
 
             if not return_prompt and not self.is_encoder_decoder:
                 response = response[:, query_tensor.shape[0] :]
```

### Comparing `trl-0.8.3/trl/trainer/reward_config.py` & `trl-0.8.4/trl/trainer/reward_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/reward_trainer.py` & `trl-0.8.4/trl/trainer/reward_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/sft_trainer.py` & `trl-0.8.4/trl/trainer/sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl/trainer/utils.py` & `trl-0.8.4/trl/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl.egg-info/PKG-INFO` & `trl-0.8.4/trl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.3
+Version: 0.8.4
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.3 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.4 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
```

### Comparing `trl-0.8.3/trl.egg-info/SOURCES.txt` & `trl-0.8.4/trl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trl-0.8.3/trl.egg-info/requires.txt` & `trl-0.8.4/trl.egg-info/requires.txt`

 * *Files identical despite different names*

