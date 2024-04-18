# Comparing `tmp/snowflake_cli_labs-2.1.2.tar.gz` & `tmp/snowflake_cli_labs-2.2.0rc0.tar.gz`

## Comparing `snowflake_cli_labs-2.1.2.tar` & `snowflake_cli_labs-2.2.0rc0.tar`

### file list

```diff
@@ -1,512 +1,562 @@
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/LEGAL.md
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/RELEASE-NOTES.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/SECURITY.md
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/performance_history_analysis.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/snowcli.spec
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/docs/images/coverage_5.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/__init__.py
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/cli_global_context.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/config.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/constants.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/exceptions.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/secure_path.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/secure_utils.py
--rw-r--r--   0        0        0     6661 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/sql_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/alias.py
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/decorators.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/experimental_behaviour.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/flags.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/project_initialisation.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/snow_typer.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/abc.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/console.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/output/formats.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/output/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/plugins/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/plugins/plugin_config.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/plugins/command/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/__init__.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/definition.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/definition_manager.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/native_app.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/project_definition.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/relaxed_map.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/snowpark.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/schemas/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/cursor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/error_handling.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/path_utils.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/rendering.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/__main__.py
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/cli_app.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/loggers.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/main_typer.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/printing.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/snow_connector.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/api_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/api_impl/plugin/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/builtin_plugins.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/exception_logging.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/threadsafe.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/typer_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/commands_structure.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/pycharm_remote_debug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/generator.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/__init__.py
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/commands.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/plugin_spec.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/__init__.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/artifacts.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/commands.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/common_flags.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/constants.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/exceptions.py
--rw-r--r--   0        0        0    11486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/init.py
--rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/policy.py
--rw-r--r--   0        0        0    16573 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/run_processor.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/version/__init__.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/version/commands.py
--rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/__init__.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/commands.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/common.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/stage/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/stage/commands.py
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/stage/diff.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/stage/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/render/__init__.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/render/commands.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/render/plugin_spec.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/__init__.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/commands.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/common.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/manager.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/models.py
--rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/package_utils.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/plugin_spec.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/venv.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/zipper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/package/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/package/commands.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/package/manager.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/package/utils.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/__init__.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/common.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_registry/commands.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_registry/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_repository/commands.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_repository/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/jobs/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/jobs/commands.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/jobs/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/services/__init__.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/services/commands.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/services/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/__init__.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/commands.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/manager.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/__init__.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/commands.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/plugin_spec.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/streamlit_utils.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/environment.yml.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/.gitignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/app/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/app/common.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/app/functions.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/app/procedures.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/.gitignore
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/environment.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/snowflake.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/common/hello.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/broken_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/failing_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/override_build_in_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/empty_config.toml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_cli.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_command_registration.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_common_decorators.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_common_global_context.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_config.py
--rw-r--r--   0        0        0    21713 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_connection.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_experimental_behaviour.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_help_messages.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_loaded_modules.py
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_logs.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_main.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_performance.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_project_initialisation.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_render.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_snow_connector.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_sql.py
--rw-r--r--   0        0        0    12490 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_zipper.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0   391720 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/__snapshots__/test_help_messages.ambr
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/__init__.py
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/test_secure_path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/commands/__init__.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/commands/test_flags.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/commands/test_snow_typer.py
--rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/commands/__snapshots__/test_snow_typer.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/console/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/console/test_cli_console_output.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/console/test_console_abc.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/api/console/test_intermediate_output.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/app/test_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/patch_utils.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_artifacts.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_commands.py
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_init.py
--rw-r--r--   0        0        0    16732 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_manager.py
--rw-r--r--   0        0        0     6242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_package_scripts.py
--rw-r--r--   0        0        0    49759 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_run_processor.py
--rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_teardown_processor.py
--rw-r--r--   0        0        0    22208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_version_create_processor.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/test_version_drop_processor.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/utils.py
--rw-r--r--   0        0        0    15171 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/__snapshots__/test_commands.ambr
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/nativeapp/__snapshots__/test_init.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/__init__.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/test_common.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/test_object.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/__snapshots__/test_object.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/stage/__init__.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/stage/test_diff.py
--rw-r--r--   0        0        0    16323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/stage/test_stage.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/object/stage/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/output/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/output/test_format_silent_enforcement.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/output/test_printing.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/output/test_silent_output.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/plugin/test_broken_plugin.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/plugin/test_failing_plugin.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/plugin/test_override_by_external_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/project/__init__.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/project/fixtures.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/project/test_config.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/project/test_definition_manager.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/project/test_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/test_common.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/test_function.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/test_package.py
--rw-r--r--   0        0        0    13771 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/test_procedure.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/test_snowpark_shared.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_procedure.ambr
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_common.py
--rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_image_repository.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_jobs.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_registry.py
--rw-r--r--   0        0        0    21119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/test_services.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/spcs/__snapshots__/test_registry.ambr
--rw-r--r--   0        0        0    23093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/streamlit/test_commands.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/streamlit/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/test_data.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/configs/broken_plugin_config.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/configs/disabled_override_plugin_config.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/configs/failing_plugin_config.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/configs/override_plugin_config.toml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure/core/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
--rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
--rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/empty_project/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit/environment.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit/pages/my_page.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_defaults/main.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_stage/environment.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/snowflake.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/package/002-shared.sql
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/snowflake.local.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/snowflake.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/package/002-shared.sql
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/minimal/snowflake.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/setup.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_1/app/streamlit/main.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/no_definition_version/snowflake.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_external_access/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_external_access/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_external_access/requirements.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_functions/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_functions/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_functions/requirements.txt
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_functions/snowflake.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_external_access/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_external_access/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/requirements.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures_coverage/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures_coverage/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/streamlit_full_definition/environment.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/streamlit_full_definition/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/streamlit_full_definition/utils/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/underspecified/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/projects/unknown_fields/snowflake.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/streamlit/another_file_with_list.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/streamlit/another_file_with_single_item.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/streamlit/with_list_in_source_file.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/test_data/streamlit/with_single_item.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/testing_utils/conversion.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/testing_utils/files_and_dirs.py
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/testing_utils/fixtures.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/conftest.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/test_error_handling.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/test_installation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/test_snowpark_examples.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/__snapshots__/test_installation.ambr
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/config/config.toml
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_e2e/config/malformatted_config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/__init__.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/conftest.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_external_plugins.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_nativeapp.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_object.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_package.py
--rw-r--r--   0        0        0    19050 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_snowpark.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_snowpark_external_access.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_sql.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_stage.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_streamlit.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_temporary_connection.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_utils.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/__snapshots__/test_sql.ambr
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/config/config_with_enabled_all_external_plugins.toml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/scripts/integration_account_setup.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/test_image_repository.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/test_jobs.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/test_registry.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/test_services.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/docker/Dockerfile
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/docker/bootstrap_containers_setup.sh
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/docker/echo_service.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/spec/spec.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/spec/spec_upgrade.yml
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/testing_utils/compute_pool_utils.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/spcs/testing_utils/spcs_services_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/sql_multi_queries.sql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/requirements.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_external_access/.gitignore
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_external_access/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_package/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_package/requirements.txt
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_package/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_package/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_package/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/streamlit/environment.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/streamlit/snowflake.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/streamlit/pages/my_page.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/streamlit/utils/utils.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/naming_utils.py
--rw-r--r--   0        0        0    11449 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/snowpark_utils.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/sql_utils.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/working_directory_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/assertions/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/assertions/test_file_assertions.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/tests_integration/testing_utils/assertions/test_result_assertions.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/LICENSE
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/README.md
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    15679 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    16098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/SECURITY.md
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/dependency-sync.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py
+-rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/feature_flags.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/alias.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/experimental_behaviour.py
+-rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/flags.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/formats.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/plugin_config.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/__init__.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/errors.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/error_handling.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/naming_utils.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/path_utils.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__main__.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/snow_connector.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/__init__.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/exception_logging.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/__init__.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/plugin_spec.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/commands.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/manager.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/__init__.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py
+-rw-r--r--   0        0        0    16830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py
+-rw-r--r--   0        0        0    13227 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/__init__.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/plugin_spec.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/__init__.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/commands.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/plugin_spec.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/__init__.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/models.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/venv.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/__init__.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/utils.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/__init__.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/manager.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/__init__.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/commands.py
+-rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py
+-rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/manager.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/__init__.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/environment.yml.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/.gitignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/common.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/functions.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/.gitignore
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/environment.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/common/hello.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/empty_config.toml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_cli.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_config.py
+-rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_connection.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_loaded_modules.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_logs.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_main.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_performance.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_render.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py
+-rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_sql.py
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0   529299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_feature_flags.py
+-rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__init__.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_flags.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_flags.ambr
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/utils/test_naming_utils.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/app/test_telemetry.py
+-rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/git/test_git_commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py
+-rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py
+-rw-r--r--   0        0        0    43760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py
+-rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_utils.py
+-rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_stage.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_failing_plugin.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_config.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py
+-rw-r--r--   0        0        0    19709 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/mocks.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_anaconda.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_build.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_common.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_models.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_package.py
+-rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py
+-rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py
+-rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__init__.py
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py
+-rw-r--r--   0        0        0    29844 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_stage.py
+-rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/broken_plugin_config.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/disabled_override_plugin_config.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/failing_plugin_config.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/override_plugin_config.toml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/core/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/empty_project/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/environment.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/main.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/snowflake.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/002-shared.sql
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.local.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/002-shared.sql
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/minimal/snowflake.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/setup.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/no_definition_version/snowflake.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/requirements.txt
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/snowflake.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/environment.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/underspecified/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/unknown_fields/snowflake.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_list.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_single_item.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_list_in_source_file.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_single_item.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/conversion.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_error_handling.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/config.toml
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/malformatted_config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__init__.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_config.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_connection.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_git.py
+-rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_package.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_session_token.py
+-rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_git.ambr
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_all_external_plugins.toml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/scripts/integration_account_setup.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/Dockerfile
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec_upgrade.yml
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/sql_multi_queries.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/requirements.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script3.sql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script_template.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/environment.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/snowflake.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/utils/utils.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/README.md
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    16123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/PKG-INFO
```

### Comparing `snowflake_cli_labs-2.1.2/CONTRIBUTING.md` & `snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contributing to SnowCLI
+# Contributing to Snowflake CLI
 
 There are two ways to contribute code to the repository: directly or by use of forks. For best practices for the second approach, refer to the section on forks below. Right now, there is limited access to contributing to the repository directly, and hence using forks is the recommended approach.
 
 ## Setup a development environment
 If you are interested in contributing, you will need to instantiate dev virtual environments and the pre-commit logic to help with formatting and linting of commits.
 
 We use [hatch](https://hatch.pypa.io/latest/) to manage and created development environments.
@@ -119,22 +119,22 @@
     * If a connection cannot be established, you will see some exception about it.
     * If you want to use other host or port you can use `--pycharm-debug-server-host` and `--pycharm-debug-server-port` options.
     * The code execution will be paused before execution of your command.
       You will see the exact line in the IDE's debug view.
       You can resume code execution, add breakpoints, evaluate variables, do all the things you usually do when debugging locally.
 
 ## Using Forks
-Create your own fork from the `snowcli` repo. As a heads up, all `snowcli` forks are publicly accessible on Github.
+Create your own fork from the `snowflake-cli` repo. As a heads up, all `snowflake-cli` forks are publicly accessible on Github.
 
-Syncing forks with the upstream `snowcli` repo can be a hassle when trying to resolve merge conflicts. To avoid issues with this approach, we recommend always rebasing to the upstream `snowcli` branch.
+Syncing forks with the upstream `snowflake-cli` repo can be a hassle when trying to resolve merge conflicts. To avoid issues with this approach, we recommend always rebasing to the upstream `snowflake-cli` branch.
 
 In the cloned copy of your fork, perform the following steps.
 
 ```bash
-git remote add sfcli https://github.com/Snowflake-Labs/snowcli.git
+git remote add sfcli https://github.com/snowflakedb/snowflake-cli.git
 git fetch sfcli
 git checkout <your-branch>
 git rebase sfcli/main
 ```
 
 ## Presenting intermediate output to users
```

### Comparing `snowflake_cli_labs-2.1.2/RELEASE-NOTES.md` & `snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,85 @@
+# v2.2.0
+
+## Backward incompatibility
+
+## Deprecations
+* `snow snowpark package lookup` no longer performs check against PyPi. Using `--pypi-download` or `--yes`
+  has no effect and will cause a warning. In this way the command has single responsibility - check if package is
+  available in Snowflake Anaconda channel.
+* `snow snowpark package create`:
+  * `--pypi-download` or `--yes` flags are deprecated, have no effect and will cause a warning.
+    `create` command always checks against PyPi.
+  * `--allow-native-libraries` is deprecated in favour of boolean flag `--allow-shared-libraries`.
+    Using old flag will cause a warning.
+* `snow snowpark build`:
+  * `--pypi-download` flag is deprecated, have no effect and will cause a warning. Create command always check against PyPi.
+  * `--check-anaconda-for-pypi-depts` is deprecated and using it will cause warning, the functionality is replaced by `--ignore-anaconda`
+  * `--package-native-libraries` is deprecated and using it will cause warning, the functionality is replaced by `--allow-shared-libraries`
+* `snow object stage` commands are deprecated and using them will cause a warning.
+   Functionality is replaced by `snow stage` commands.
+
+## New additions
+* Added support for fully qualified name (`database.schema.name`) in `name` parameter in streamlit project definition
+* Added support for fully qualified image repository names in `spcs image-repository` commands.
+* Added `--if-not-exists` option to `create` commands for `service`, and `compute-pool`. Added `--replace` and `--if-not-exists` options for `image-repository create`.
+* Added support for python connector diagnostic report.
+* Added `snow app deploy` command that creates an application package and syncs the local changes to the stage without creating or updating the application.
+* Added `is_default` column to `snow connection list` output to highlight default connection.
+* `snow snowpark package create`:
+  * new `--ignore-anaconda` flag disables package lookup in Snowflake Anaconda channel.
+    All dependencies will be downloaded from PyPi.
+  * new `--skip-version-check` skips comparing versions of dependencies between requirements and Anaconda.
+  * new `--index-url` flag sets up Base URL of the Python Package Index to use for package lookup.
+* `snow snowpark build`:
+  * new `--skip-version-check` skips comparing versions of dependencies between requirements and Anaconda.
+  * new `--index-url` flag sets up Base URL of the Python Package Index to use for package lookup.
+* Added `--recursive` flag for copy from stage, it will reproduce the directory structure locally.
+* Added support for snowgit. New commands:
+  * `snow git setup` - wizard setting up a git repository stage and creating all necessary objects
+  * `snow git fetch` - fetches latest changes from the origin repository into Snowflake repository
+  * `snow git list-brahces` - lists all branches in the repository
+  * `snow git list-tags` - lists all tags in the repository
+  * `snow git list-files` - lists all files on provided branch/tag/commit
+  * `snow git copy` - copies files from provided branch/tag/commit into stage or local directory
+  * `snow git execute` - execute immediate files from repository
+* Added command for execute immediate `snow object stage execute`
+* Fetching available packages list from Snowflake instead of directly from Anaconda with fallback to the old method (for backward compatibility).
+  As the new method requires a connection to Snowflake, it adds connection options to the following commands:
+  * `snow snowpark build`
+  * `snow snowpark package lookup`
+  * `snow snowpark package create`
+
+## Fixes and improvements
+* Adding `--image-name` option for image name argument in `spcs image-repository list-tags` for consistency with other commands.
+* Fixed errors during `spcs image-registry login` not being formatted correctly.
+* Project definition no longer accept extra fields. Any extra field will cause an error.
+* Changing imports in function/procedure section in `snowflake.yml` will cause the definition update on replace
+* Adding `--pattern` flag to `stage list` command for filtering out results with regex.
+* Fixed snowpark build paths for builds with --project option (fixed empty zip issue).
+* More clear error messages in `snow snowpark build` command
+* Adding support for any source supported by `pip` in `snow snowpark`.
+* Fixed version parsing for packages lookup on Snowflake Anaconda Channel
+* Fix handling database/schema/role identifiers containing dashes
+* Fix schema override bug in `snow connection test`
+* Hidden incorrectly working config permissions warning on Windows
+
 # v2.1.2
 
 ## Fixes and improvements
- * Add `pip` as Snowflake-cli dependency
- * Optimize `connection test` command
- * Fix venv creation issues in `snowpark package create` and `snowpark build` command
+* Add `pip` as Snowflake-cli dependency
+* Optimize `connection test` command
+* Fix venv creation issues in `snowpark package create` and `snowpark build` command
 
 # v2.1.1
 
 ## Fixes and improvements
 * Improved security of printing connection details in `snow connection list`.
 * Improved parsing of non-quoted scalar values within square brackets in `manifest.yml` in Native App projects.
+
 # v2.1.0
 
 ## Backward incompatibility
 
 ## New additions
 * Added ability to specify scope of the `object list` command with the `--in <scope_type> <scope_name>` option.
 * Introduced `snowflake.cli.api.console.cli_console` object with helper methods for intermediate output.
@@ -22,14 +88,17 @@
 * New commands for `spcs`
   * Added `image-registry url` command to get the URL for your account image registry.
   * Added `image-registry login` command to fetch authentication token and log in to image registry in one command.
   * Added `image-repository url <repo_name>` command to get the URL for specified image repository.
   * Added `create` command for `image-repository`.
   * Added `status`, `set (property)`, `unset (property)`, `suspend` and `resume` commands for `compute-pool`.
   * Added `set (property)`, `unset (property)`,`upgrade` and `list-endpoints` commands for `service`.
+* You can now use github repo link in `snow snowpark package create` to prepare your code for upload
+* Added `allow-native-libraries` option to `snow snowpark package create` command
+* Added alias `--install-from-pip` for `-y` option in `snow snowpark package create` command
 * Connections parameters are also supported by generic environment variables:
   * `SNOWFLAKE_ACCOUNT`
   * `SNOWFLAKE_USER`
   * `SNOWFLAKE_PASSWORD`
   * `SNOWFLAKE_DATABASE`
   * `SNOWFLAKE_SCHEMA`
   * `SNOWFLAKE_ROLE`
@@ -43,14 +112,15 @@
 * Testing connection using `snow connection test` validates also access to database, schema, role and warehouse
   specified in the connection details.
 * Added `snow connection set-default` command for changing default connection.
 
 ## Fixes and improvements
 * Restricted permissions of automatically created files
 * Fixed bug where `spcs service create` would not throw error if service with specified name already exists.
+* Improved package lookup, to avoid unnecessary uploads
 * Logging into the file by default (INFO level)
 * Added validation that service, compute pool, and image repository names are unqualified identifiers.
 * `spcs service` commands now accept qualified names.
 * Updated help messages for `spcs` commands.
 
 # v2.0.0
 
@@ -147,15 +217,15 @@
 ## Fixes and improvements
 * Fix homebrew installation
 
 
 # v1.2.0
 
 ## Backward incompatibility
-* Removed `snow streamlit create` command. Streamlit can be deployd using `snow streamlit deploy`
+* Removed `snow streamlit create` command. Streamlit can be deployed using `snow streamlit deploy`
 * Removed short option names in compute pool commands:
   * `-n` for `--name`, name of compute pool
   * `-d` for `--num`, number of pool's instances
   * `-f` for `--family`, instance family
 * Renamed long options in Snowpark services commands:
   * `--compute_pool` is now `--compute-pool`
   * `--num_instances` is now `--num-instances`
```

### Comparing `snowflake_cli_labs-2.1.2/performance_history_analysis.py` & `snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,25 @@
 
 
 def _print_summary_performance_descending(
     commits_with_results: List[Tuple[Commit, float]]
 ) -> None:
     commits_with_diffs: List[Tuple[Commit, Decimal]] = []
     last_result: Optional[Decimal] = None
-    for (commit, result) in reversed(commits_with_results):
+    for commit, result in reversed(commits_with_results):
         if last_result:
             result_diff = Decimal(result) - last_result
             if result_diff > 0:
                 commits_with_diffs.append((commit, result_diff))
         last_result = Decimal(result)
     sorted_list_of_diffs: List[Tuple[Commit, Decimal]] = sorted(
         commits_with_diffs, key=lambda e: e[1], reverse=True
     )
     print("\nCommits causing performance descending:")
-    for (commit, diff) in sorted_list_of_diffs:
+    for commit, diff in sorted_list_of_diffs:
         print(
             f"Diff [{diff}] after commit {commit} ({commit.authored_datetime}) -> {commit.message.splitlines()[0]}"
         )
 
 
 def _analyse_performance_history(
     rev: str, limit_commits: int, sample_amount: int, print_all_results: bool
```

### Comparing `snowflake_cli_labs-2.1.2/docs/images/coverage_1.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/docs/images/coverage_2.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/docs/images/coverage_3.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/docs/images/coverage_4.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/docs/images/coverage_5.png` & `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/cli_global_context.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,20 @@
         self._schema: Optional[str] = None
         self._user: Optional[str] = None
         self._password: Optional[str] = None
         self._authenticator: Optional[str] = None
         self._private_key_path: Optional[str] = None
         self._warehouse: Optional[str] = None
         self._mfa_passcode: Optional[str] = None
+        self._enable_diag: Optional[bool] = False
+        self._diag_log_path: Optional[Path] = None
+        self._diag_allowlist_path: Optional[Path] = None
         self._temporary_connection: bool = False
+        self._session_token: Optional[str] = None
+        self._master_token: Optional[str] = None
 
     def __setattr__(self, key, value):
         """
         We invalidate connection cache every time connection attributes change.
         """
         super().__setattr__(key, value)
         if key != "_cached_connection":
@@ -115,21 +120,56 @@
     def mfa_passcode(self) -> Optional[str]:
         return self._mfa_passcode
 
     def set_mfa_passcode(self, value: Optional[str]):
         self._mfa_passcode = value
 
     @property
+    def enable_diag(self) -> Optional[bool]:
+        return self._enable_diag
+
+    def set_enable_diag(self, value: Optional[bool]):
+        self._enable_diag = value
+
+    @property
+    def diag_log_path(self) -> Optional[Path]:
+        return self._diag_log_path
+
+    def set_diag_log_path(self, value: Optional[Path]):
+        self._diag_log_path = value
+
+    @property
+    def diag_allowlist_path(self) -> Optional[Path]:
+        return self._diag_allowlist_path
+
+    def set_diag_allowlist_path(self, value: Optional[Path]):
+        self._diag_allowlist_path = value
+
+    @property
     def temporary_connection(self) -> bool:
         return self._temporary_connection
 
     def set_temporary_connection(self, value: bool):
         self._temporary_connection = value
 
     @property
+    def session_token(self) -> Optional[str]:
+        return self._session_token
+
+    def set_session_token(self, value: Optional[str]):
+        self._session_token = value
+
+    @property
+    def master_token(self) -> Optional[str]:
+        return self._master_token
+
+    def set_master_token(self, value: Optional[str]):
+        self._master_token = value
+
+    @property
     def connection(self) -> SnowflakeConnection:
         if not self._cached_connection:
             self._cached_connection = self._build_connection()
         return self._cached_connection
 
     def _collect_not_empty_connection_attributes(self):
         return {
@@ -138,22 +178,27 @@
             "password": self.password,
             "authenticator": self.authenticator,
             "private_key_path": self.private_key_path,
             "database": self.database,
             "schema": self.schema,
             "role": self.role,
             "warehouse": self.warehouse,
+            "session_token": self.session_token,
+            "master_token": self.master_token,
         }
 
     def _build_connection(self):
         from snowflake.cli.app.snow_connector import connect_to_snowflake
 
         return connect_to_snowflake(
             temporary_connection=self.temporary_connection,
             mfa_passcode=self._mfa_passcode,
+            enable_diag=self._enable_diag,
+            diag_log_path=self._diag_log_path,
+            diag_allowlist_path=self._diag_allowlist_path,
             connection_name=self.connection_name,
             **self._collect_not_empty_connection_attributes(),
         )
 
 
 class _CliGlobalContextManager:
     def __init__(self):
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/config.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import logging
 import os
+import warnings
 from contextlib import contextmanager
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import tomlkit
+from click import ClickException
 from snowflake.cli.api.exceptions import (
     ConfigFileTooWidePermissionsError,
     MissingConfiguration,
     UnsupportedConfigSectionTypeError,
 )
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.api.secure_utils import file_permissions_are_strict
@@ -34,14 +36,15 @@
 CONNECTIONS_SECTION = "connections"
 CLI_SECTION = "cli"
 LOGS_SECTION = "logs"
 PLUGINS_SECTION = "plugins"
 
 LOGS_SECTION_PATH = [CLI_SECTION, LOGS_SECTION]
 PLUGINS_SECTION_PATH = [CLI_SECTION, PLUGINS_SECTION]
+FEATURE_FLAGS_SECTION_PATH = [CLI_SECTION, "features"]
 
 CONFIG_MANAGER.add_option(
     name=CLI_SECTION,
     parse_str=tomlkit.parse,
     default=dict(),
 )
 
@@ -98,15 +101,15 @@
     """
     if config_file:
         CONFIG_MANAGER.file_path = config_file
     else:
         _check_default_config_files_permissions()
     if not CONFIG_MANAGER.file_path.exists():
         _initialise_config(CONFIG_MANAGER.file_path)
-    CONFIG_MANAGER.read_config()
+    _read_config_file()
 
 
 def add_connection(name: str, connection_config: ConnectionConfig):
     set_config_value(
         section=CONNECTIONS_SECTION,
         key=name,
         value=connection_config.to_dict_of_all_non_empty_values(),
@@ -120,20 +123,31 @@
 }
 
 _DEFAULT_CLI_CONFIG = {LOGS_SECTION: _DEFAULT_LOGS_CONFIG}
 
 
 @contextmanager
 def _config_file():
-    CONFIG_MANAGER.read_config()
+    _read_config_file()
     conf_file_cache = CONFIG_MANAGER.conf_file_cache
     yield conf_file_cache
     _dump_config(conf_file_cache)
 
 
+def _read_config_file():
+    with warnings.catch_warnings():
+        if IS_WINDOWS:
+            warnings.filterwarnings(
+                action="ignore",
+                message="Bad owner or permissions.*",
+                module="snowflake.connector.config_manager",
+            )
+        CONFIG_MANAGER.read_config()
+
+
 def _initialise_logs_section():
     with _config_file() as conf_file_cache:
         if conf_file_cache.get(CLI_SECTION) is None:
             conf_file_cache[CLI_SECTION] = _DEFAULT_CLI_CONFIG
         if conf_file_cache[CLI_SECTION].get(LOGS_SECTION) is None:
             conf_file_cache[CLI_SECTION][LOGS_SECTION] = _DEFAULT_LOGS_CONFIG
 
@@ -184,54 +198,77 @@
 def get_connection_dict(connection_name: str) -> dict:
     try:
         return get_config_section(CONNECTIONS_SECTION, connection_name)
     except KeyError:
         raise MissingConfiguration(f"Connection {connection_name} is not configured")
 
 
+def get_default_connection_name() -> str:
+    return CONFIG_MANAGER["default_connection_name"]
+
+
 def get_default_connection_dict() -> dict:
-    def_connection_name = CONFIG_MANAGER["default_connection_name"]
-    return get_connection_dict(def_connection_name)
+    return get_connection_dict(get_default_connection_name())
 
 
 def get_config_section(*path) -> dict:
     section = _find_section(*path)
     if isinstance(section, Container):
         return {s: _merge_section_with_env(section[s], *path, s) for s in section}
     if isinstance(section, dict):
         return _merge_section_with_env(section, *path)
     raise UnsupportedConfigSectionTypeError(type(section))
 
 
 def get_config_value(*path, key: str, default: Optional[Any] = Empty) -> Any:
     """Looks for given key under nested path in toml file."""
-    env_variable = _get_env_value(*path, key=key)
+    env_variable = get_env_value(*path, key=key)
     if env_variable:
         return env_variable
     try:
         return get_config_section(*path)[key]
     except (KeyError, NonExistentKey, MissingConfigOptionError):
         if default is not Empty:
             return default
         raise
 
 
+def get_config_bool_value(*path, key: str, default: Optional[Any] = Empty) -> bool:
+    value = get_config_value(*path, key=key, default=default)
+    # If we get bool then we can return
+    if isinstance(value, bool):
+        return value
+
+    # Now if value is not string then cast it to str. Simplifies logic for 1 and 0
+    if not isinstance(value, str):
+        value = str(value)
+
+    know_booleans_mapping = {"true": True, "false": False, "1": True, "0": False}
+
+    if value.lower() not in know_booleans_mapping:
+        raise ClickException(
+            f"Expected boolean value for {'.'.join((*path, key))} option."
+        )
+    return know_booleans_mapping[value.lower()]
+
+
 def _initialise_config(config_file: Path) -> None:
     config_file = SecurePath(config_file)
     config_file.parent.mkdir(parents=True, exist_ok=True)
     config_file.touch()
     _initialise_logs_section()
     log.info("Created Snowflake configuration file at %s", CONFIG_MANAGER.file_path)
 
 
-def _get_env_value(*path, key: str) -> str | None:
-    env_variable_name = (
-        "SNOWFLAKE_" + "_".join(p.upper() for p in path) + f"_{key.upper()}"
-    )
-    return os.environ.get(env_variable_name)
+def get_env_variable_name(*path, key: str) -> str:
+    return "SNOWFLAKE_" + "_".join(p.upper() for p in path) + f"_{key.upper()}"
+
+
+def get_env_value(*path, key: str) -> str | None:
+    return os.environ.get(get_env_variable_name(*path, key=key))
 
 
 def _find_section(*path) -> TOMLDocument:
     section = CONFIG_MANAGER
     idx = 0
     while idx < len(path):
         section = section[path[idx]]
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/constants.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     TASK = ObjectNames("task", "task", "tasks")
     USER = ObjectNames("user", "user", "users")
     WAREHOUSE = ObjectNames("warehouse", "warehouse", "warehouses")
     VIEW = ObjectNames("view", "view", "views")
     IMAGE_REPOSITORY = ObjectNames(
         "image-repository", "image repository", "image repositories"
     )
+    GIT_REPOSITORY = ObjectNames("git-repository", "git repository", "git repositories")
 
     def __str__(self):
         """This makes using this Enum easier in formatted string"""
         return self.value.cli_name
 
 
 OBJECT_TO_NAMES = {o.value.cli_name: o.value for o in ObjectType}
 SUPPORTED_OBJECTS = sorted(OBJECT_TO_NAMES.keys())
 
 # Scope names here must replace spaces with '-'. For example 'compute pool' is 'compute-pool'.
 VALID_SCOPES = ["database", "schema", "compute-pool"]
 
-PACKAGES_DIR = Path(".packages")
 DEFAULT_SIZE_LIMIT_MB = 128
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/exceptions.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/secure_path.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         """
         When the path points to a directory, yield path objects of the directory contents.
         Otherwise, NotADirectoryError is raised.
         If the locartion does not exists, FileNotFoundError is raised.
 
         For details, check pathlib.Path.iterdir()
         """
-        self._assert_exists()
-        self._assert_is_directory()
+        self.assert_exists()
+        self.assert_is_directory()
         return (SecurePath(p) for p in self._path.iterdir())
 
     def exists(self) -> bool:
         """
         Return True if the path points to an existing file or directory.
         """
         return self._path.exists()
@@ -130,15 +130,15 @@
             assert (
                 read_file_limit_mb is not None
             ), "For reading mode ('r') read_file_limit_mb must be provided"
             self._assert_exists_and_is_file()
             self._assert_file_size_limit(read_file_limit_mb)
 
         if self.exists():
-            self._assert_is_file()
+            self.assert_is_file()
         else:
             self.touch()  # makes sure permissions of freshly-created file are strict
 
         log.info("Opening file %s in mode '%s'", self._path, mode)
         with self._path.open(mode=mode, **open_kwargs) as fd:
             yield fd
         log.info("Closing file %s", self._path)
@@ -151,15 +151,15 @@
         """
         destination = Path(destination)
         if destination.is_dir():
             destination = destination / self._path.name
         if destination.exists():
             _raise_file_exists_error(destination)
         log.info("Moving %s to %s", str(self._path), destination.resolve())
-        return SecurePath(shutil.move(self._path, destination))
+        return SecurePath(shutil.move(str(self._path), destination))
 
     def copy(
         self, destination: Union[Path, str], dirs_exist_ok: bool = False
     ) -> "SecurePath":
         """
         Copy the file/directory into the destination.
         If source is a directory, its whole content is copied recursively.
@@ -171,15 +171,15 @@
         Otherwise, the copied file/base directory will be renamed to match destination.
         If dirs_exist_ok is false (the default) and dst already exists,
         a FileExistsError is raised. If dirs_exist_ok is true,
         the copying operation will continue if it encounters existing directories,
         and files within the destination tree will be overwritten by corresponding
         files from the src tree.
         """
-        self._assert_exists()
+        self.assert_exists()
 
         destination = Path(destination)
         if destination.exists():
             if destination.is_dir() and (
                 destination.name != self._path.name or self.path.is_file()
             ):
                 destination = destination / self._path.name
@@ -222,36 +222,36 @@
         Remove this file or symbolic link.
         If the path points to a directory, use SecurePath.rmdir() instead.
 
         Check pathlib.Path.unlink() for details.
         """
         if not self.exists():
             if not missing_ok:
-                self._assert_exists()
+                self.assert_exists()
             return
 
-        self._assert_is_file()
+        self.assert_is_file()
         log.info("Removing file %s", self._path)
         self._path.unlink()
 
     def rmdir(self, recursive=False, missing_ok=False):
         """
         Remove this directory.
         If the path points to a file, use SecurePath.unlink() instead.
 
         If path points to a file, NotADirectoryError will be raised.
         If directory does not exist, FileNotFoundError will be raised unless [missing_ok] is True.
         If the directory is not empty, DirectoryNotEmpty will be raised unless [recursive] is True.
         """
         if not self.exists():
             if not missing_ok:
-                self._assert_exists()
+                self.assert_exists()
             return
 
-        self._assert_is_directory()
+        self.assert_is_directory()
 
         if not recursive and any(self._path.iterdir()):
             raise DirectoryIsNotEmptyError(self._path.resolve())
 
         log.info("Removing directory %s", self._path)
         shutil.rmtree(str(self._path))
 
@@ -267,28 +267,28 @@
         """
         with tempfile.TemporaryDirectory(prefix="snowflake-cli") as tmpdir:
             log.info("Created temporary directory %s", tmpdir)
             yield SecurePath(tmpdir)
             log.info("Removing temporary directory %s", tmpdir)
 
     def _assert_exists_and_is_file(self) -> None:
-        self._assert_exists()
-        self._assert_is_file()
+        self.assert_exists()
+        self.assert_is_file()
 
-    def _assert_exists(self) -> None:
+    def assert_exists(self) -> None:
         if not self.exists():
             raise FileNotFoundError(
                 errno.ENOENT, os.strerror(errno.ENOENT), self._path.resolve()
             )
 
-    def _assert_is_file(self) -> None:
+    def assert_is_file(self) -> None:
         if not self._path.is_file():
             _raise_is_a_directory_error(self._path.resolve())
 
-    def _assert_is_directory(self) -> None:
+    def assert_is_directory(self) -> None:
         if not self._path.is_dir():
             _raise_not_a_directory_error(self._path.resolve())
 
     def _assert_file_size_limit(self, size_limit_in_mb):
         if (
             size_limit_in_mb != UNLIMITED
             and self._path.stat().st_size > size_limit_in_mb * 1024 * 1024
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/secure_utils.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/sql_execution.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import logging
 from contextlib import contextmanager
 from functools import cached_property
 from io import StringIO
 from textwrap import dedent
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Tuple
 
-from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.exceptions import (
     DatabaseNotProvidedError,
     SchemaNotProvidedError,
     SnowflakeSQLExecutionError,
 )
 from snowflake.cli.api.project.util import (
     identifier_to_show_like_pattern,
     unquote_identifier,
 )
 from snowflake.cli.api.utils.cursor import find_first_row
+from snowflake.cli.api.utils.naming_utils import from_qualified_name
 from snowflake.connector.cursor import DictCursor, SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
 
 
 class SqlExecutionMixin:
     def __init__(self):
         pass
@@ -82,95 +82,145 @@
             self._execute_query(f"use role {new_role}")
         try:
             yield
         finally:
             if is_different_role:
                 self._execute_query(f"use role {prev_role}")
 
-    def _execute_schema_query(self, query: str, **kwargs):
-        self.check_database_and_schema()
-        return self._execute_query(query, **kwargs)
+    def create_password_secret(
+        self, name: str, username: str, password: str
+    ) -> SnowflakeCursor:
+        return self._execute_query(
+            f"""
+            create secret {name}
+            type = password
+            username = '{username}'
+            password = '{password}'
+            """
+        )
+
+    def create_api_integration(
+        self, name: str, api_provider: str, allowed_prefix: str, secret: Optional[str]
+    ) -> SnowflakeCursor:
+        return self._execute_query(
+            f"""
+            create api integration {name}
+            api_provider = {api_provider}
+            api_allowed_prefixes = ('{allowed_prefix}')
+            allowed_authentication_secrets = ({secret if secret else ''})
+            enabled = true
+            """
+        )
 
-    def check_database_and_schema(self) -> None:
+    def _execute_schema_query(self, query: str, name: Optional[str] = None, **kwargs):
         """
-        Checks if the connection database and schema are set and that they actually exist in Snowflake.
+        Check that a database and schema are provided before executing the query. Useful for operating on schema level objects.
         """
-        self.check_schema_exists(self._conn.database, self._conn.schema)
+        self.check_database_and_schema_provided(name)
+        return self._execute_query(query, **kwargs)
 
-    def check_database_exists(self, database: str) -> None:
+    def check_database_and_schema_provided(self, name: Optional[str] = None) -> None:
         """
-        Checks that database is provided and that it is a valid database in
-        Snowflake. Note that this could fail for a variety of reasons,
-        including not authorized to use database, database doesn't exist,
-        database is not a valid identifier, and more.
+        Checks if a database and schema are provided, either through the connection context or a qualified name.
         """
+        if name:
+            _, schema, database = from_qualified_name(name)
+        else:
+            schema, database = None, None
+        schema = schema or self._conn.schema
+        database = database or self._conn.database
         if not database:
             raise DatabaseNotProvidedError()
-        try:
-            self._execute_query(f"USE DATABASE {database}")
-        except ProgrammingError as e:
-            raise ClickException(f"Exception occurred: {e}.") from e
-
-    def check_schema_exists(self, database: str, schema: str) -> None:
-        """
-        Checks that schema is provided and that it is a valid schema in Snowflake.
-        Note that this could fail for a variety of reasons,
-        including not authorized to use schema, schema doesn't exist,
-        schema is not a valid identifier, and more.
-        """
-        self.check_database_exists(database)
         if not schema:
             raise SchemaNotProvidedError()
-        try:
-            self._execute_query(f"USE {database}.{schema}")
-        except ProgrammingError as e:
-            raise ClickException(f"Exception occurred: {e}.") from e
 
     def to_fully_qualified_name(
         self, name: str, database: Optional[str] = None, schema: Optional[str] = None
     ):
         current_parts = name.split(".")
         if len(current_parts) == 3:
             # already fully qualified name
             return name.upper()
 
         if not database:
             if not self._conn.database:
-                raise ClickException(
-                    "Default database not specified in connection details."
-                )
+                raise DatabaseNotProvidedError()
             database = self._conn.database
 
         if len(current_parts) == 2:
             # we assume name is in form of `schema.object`
             return f"{database}.{name}".upper()
 
         schema = schema or self._conn.schema or "public"
         database = database or self._conn.database
         return f"{database}.{schema}.{name}".upper()
 
+    @staticmethod
+    def get_name_from_fully_qualified_name(name):
+        """
+        Returns name of the object from the fully-qualified name.
+        Assumes that [name] is in format [[database.]schema.]name
+        """
+        return from_qualified_name(name)[0]
+
+    @staticmethod
+    def _qualified_name_to_in_clause(name: str) -> Tuple[str, Optional[str]]:
+        unqualified_name, schema, database = from_qualified_name(name)
+        if database:
+            in_clause = f"in schema {database}.{schema}"
+        elif schema:
+            in_clause = f"in schema {schema}"
+        else:
+            in_clause = None
+        return unqualified_name, in_clause
+
+    class InClauseWithQualifiedNameError(ValueError):
+        def __init__(self):
+            super().__init__("non-empty 'in_clause' passed with qualified 'name'")
+
     def show_specific_object(
         self,
         object_type_plural: str,
-        unqualified_name: str,
+        name: str,
         name_col: str = "name",
         in_clause: str = "",
         check_schema: bool = False,
     ) -> Optional[dict]:
         """
         Executes a "show <objects> like" query for a particular entity with a
-        given (unqualified) name. This command is useful when the corresponding
+        given (optionally qualified) name. This command is useful when the corresponding
         "describe <object>" query does not provide the information you seek.
+
+        Note that this command is analogous to describe and should only return a single row.
+        If the target object type is a schema level object, then check_schema should be set to True
+        so that the function will verify that a database and schema are provided, either through
+        the connection or a qualified name, before executing the query.
         """
-        if check_schema:
-            self.check_database_and_schema()
+
+        unqualified_name, name_in_clause = self._qualified_name_to_in_clause(name)
+        if in_clause and name_in_clause:
+            raise self.InClauseWithQualifiedNameError()
+        elif name_in_clause:
+            in_clause = name_in_clause
         show_obj_query = f"show {object_type_plural} like {identifier_to_show_like_pattern(unqualified_name)} {in_clause}".strip()
-        show_obj_cursor = self._execute_query(  # type: ignore
-            show_obj_query, cursor_class=DictCursor
-        )
+
+        if check_schema:
+            show_obj_cursor = self._execute_schema_query(  # type: ignore
+                show_obj_query, name=name, cursor_class=DictCursor
+            )
+        else:
+            show_obj_cursor = self._execute_query(  # type: ignore
+                show_obj_query, cursor_class=DictCursor
+            )
+
         if show_obj_cursor.rowcount is None:
             raise SnowflakeSQLExecutionError(show_obj_query)
+        elif show_obj_cursor.rowcount > 1:
+            raise ProgrammingError(
+                f"Received multiple rows from result of SQL statement: {show_obj_query}. Usage of 'show_specific_object' may not be properly scoped."
+            )
+
         show_obj_row = find_first_row(
             show_obj_cursor,
             lambda row: row[name_col] == unquote_identifier(unqualified_name),
         )
         return show_obj_row
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/decorators.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.flags import (
     AccountOption,
     AuthenticatorOption,
     ConnectionOption,
     DatabaseOption,
     DebugOption,
+    DiagAllowlistPathOption,
+    DiagLogPathOption,
+    EnableDiagOption,
+    MasterTokenOption,
     MfaPasscodeOption,
     OutputFormatOption,
     PasswordOption,
     PrivateKeyPathOption,
     RoleOption,
     SchemaOption,
+    SessionTokenOption,
     SilentOption,
     TemporaryConnectionOption,
     UserOption,
     VerboseOption,
     WarehouseOption,
     experimental_option,
     project_definition_option,
@@ -203,14 +208,26 @@
     inspect.Parameter(
         "private_key_path",
         inspect.Parameter.KEYWORD_ONLY,
         annotation=Optional[str],
         default=PrivateKeyPathOption,
     ),
     inspect.Parameter(
+        "session_token",
+        inspect.Parameter.KEYWORD_ONLY,
+        annotation=Optional[str],
+        default=SessionTokenOption,
+    ),
+    inspect.Parameter(
+        "master_token",
+        inspect.Parameter.KEYWORD_ONLY,
+        annotation=Optional[str],
+        default=MasterTokenOption,
+    ),
+    inspect.Parameter(
         "database",
         inspect.Parameter.KEYWORD_ONLY,
         annotation=Optional[str],
         default=DatabaseOption,
     ),
     inspect.Parameter(
         "schema",
@@ -238,14 +255,32 @@
     ),
     inspect.Parameter(
         "mfa_passcode",
         inspect.Parameter.KEYWORD_ONLY,
         annotation=Optional[str],
         default=MfaPasscodeOption,
     ),
+    inspect.Parameter(
+        "enable_diag",
+        inspect.Parameter.KEYWORD_ONLY,
+        annotation=Optional[bool],
+        default=EnableDiagOption,
+    ),
+    inspect.Parameter(
+        "diag_log_path",
+        inspect.Parameter.KEYWORD_ONLY,
+        annotation=Optional[str],
+        default=DiagLogPathOption,
+    ),
+    inspect.Parameter(
+        "diag_allowlist_path",
+        inspect.Parameter.KEYWORD_ONLY,
+        annotation=Optional[str],
+        default=DiagAllowlistPathOption,
+    ),
 ]
 
 GLOBAL_OPTIONS = [
     inspect.Parameter(
         "format",
         inspect.Parameter.KEYWORD_ONLY,
         annotation=OutputFormat,
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/project_initialisation.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from __future__ import annotations
 
+from typing import Optional
+
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.constants import TEMPLATES_PATH
 from snowflake.cli.api.output.types import CommandResult, MessageResult
 from snowflake.cli.api.secure_path import SecurePath
 from typer import Argument
 
 
 def _create_project_template(template_name: str, project_directory: str):
     SecurePath(TEMPLATES_PATH / template_name).copy(
         project_directory, dirs_exist_ok=True
     )
 
 
-def add_init_command(app: SnowTyper, project_type: str, template: str):
+def add_init_command(
+    app: SnowTyper, project_type: str, template: str, help_message: Optional[str] = None
+):
     @app.command()
     def init(
         project_name: str = Argument(
             f"example_{project_type.lower()}",
-            help=f"Name of the {project_type} project you want to create.",
+            help=(
+                help_message
+                if help_message is not None
+                else f"Name of the {project_type} project you want to create."
+            ),
         ),
         **options,
     ) -> CommandResult:
         _create_project_template(template, project_directory=project_name)
         return MessageResult(f"Initialized the new project in {project_name}/")
 
+    project_type_doc = (
+        project_type if project_type.lower() != "streamlit" else "Streamlit app"
+    )
+
     init.__doc__ = (
         f"Initializes this directory with a sample set "
-        f"of files for creating a {project_type} project."
+        f"of files for creating a {project_type_doc} project."
     )
 
     return init
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/commands/snow_typer.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from functools import wraps
-from typing import Optional
+from typing import Callable, Optional
 
 import typer
 from snowflake.cli.api.commands.decorators import (
     global_options,
     global_options_with_connection,
 )
 from snowflake.cli.api.commands.flags import DEFAULT_CONTEXT_SETTINGS
@@ -26,21 +26,24 @@
 
     @wraps(typer.Typer.command)
     def command(
         self,
         name: Optional[str] = None,
         requires_global_options: bool = True,
         requires_connection: bool = False,
+        is_enabled: Callable[[], bool] | None = None,
         **kwargs,
     ):
         """
         Custom implementation of Typer.command that adds ability to execute additional
         logic before and after execution as well as process the result and act on possible
         errors.
         """
+        if is_enabled is not None and not is_enabled():
+            return lambda func: func
 
         def custom_command(command_callable):
             """Custom command wrapper similar to Typer.command."""
             if requires_connection:
                 command_callable = global_options_with_connection(command_callable)
             elif requires_global_options:
                 command_callable = global_options(command_callable)
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/abc.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from snowflake.cli.api.cli_global_context import _CliGlobalContextAccess, cli_context
 
 
 class AbstractConsole(ABC):
     """Interface for cli console implementation.
 
     Each console should have three methods implemented:
-    - `step` - for more detailed informations on steps
+    - `step` - for more detailed information on steps
     - `warning` - for displaying messages in a style that makes it
       visually stand out from other output
     - `phase` a context manager for organising steps into logical group
     """
 
     _print_fn: Callable[[str], None]
     _cli_context: _CliGlobalContextAccess
@@ -58,8 +58,8 @@
     def message(self, _message: str):
         """Displays an informational message to output."""
 
     @abstractmethod
     def warning(self, message: str):
         """Displays message in a style that makes it visually stand out from other output.
 
-        Intended for diplaying messeges related to important messages."""
+        Intended for displaying messages related to important messages."""
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/console/console.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 class CliConsoleNestingProhibitedError(RuntimeError):
     """CliConsole phase nesting not allowed."""
 
 
 class CliConsole(AbstractConsole):
     """An utility for displaying intermediate output.
 
-    Provides following methods for handling displying messages:
-    - `step` - for more detailed informations on steps
+    Provides following methods for handling displaying messages:
+    - `step` - for more detailed information on steps
     - `warning` - for displaying messages in a style that makes it
       visually stand out from other output
     - `phase` a context manager for organising steps into logical group
     """
 
     _indentation_level: int = INDENTATION_LEVEL
     _styles: dict = {
@@ -35,15 +35,15 @@
         Output.PHASE: PHASE_STYLE,
         Output.STEP: STEP_STYLE,
         Output.INFO: INFO_STYLE,
         Output.IMPORTANT: IMPORTANT_STYLE,
     }
 
     def _format_message(self, message: str, output: Output) -> Text:
-        """Wraps message in rich Text object and applys formatting."""
+        """Wraps message in rich Text object and applies formatting."""
         style = self._styles.get(output, "default")
         text = Text(message, style=style)
 
         if self.in_phase and output in {Output.STEP, Output.INFO, Output.IMPORTANT}:
             text.pad_left(self._indentation_level)
 
         return text
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/output/types.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import typing as t
 
+from snowflake.connector import DictCursor
 from snowflake.connector.cursor import SnowflakeCursor
 
 
 class CommandResult:
     @property
     def result(self):
         raise NotImplementedError()
@@ -39,20 +40,22 @@
 
     @property
     def result(self):
         return (element for element in self._elements)
 
 
 class QueryResult(CollectionResult):
-    def __init__(self, cursor: SnowflakeCursor):
+    def __init__(self, cursor: SnowflakeCursor | DictCursor):
         self.column_names = [col.name for col in cursor.description]
         super().__init__(elements=self._prepare_payload(cursor))
         self._query = cursor.query
 
-    def _prepare_payload(self, cursor):
+    def _prepare_payload(self, cursor: SnowflakeCursor | DictCursor):
+        if isinstance(cursor, DictCursor):
+            return (k for k in cursor)
         return ({k: v for k, v in zip(self.column_names, row)} for row in cursor)
 
     @property
     def query(self):
         return self._query
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/plugins/command/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/definition.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,97 @@
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List
 
+import yaml.loader
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
-from snowflake.cli.api.project.schemas.project_definition import (
-    project_override_schema,
-    project_schema,
-)
+from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 from snowflake.cli.api.project.util import (
     append_to_identifier,
     clean_identifier,
     get_env_username,
     to_identifier,
 )
 from snowflake.cli.api.secure_path import SecurePath
-from strictyaml import (
-    YAML,
-    as_document,
-    load,
-)
+from yaml import load
 
 DEFAULT_USERNAME = "unknown_user"
 
 
-def merge_left(target: Union[Dict, YAML], source: Union[Dict, YAML]) -> None:
+def merge_left(target: Dict, source: Dict) -> None:
     """
     Recursively merges key/value pairs from source into target.
     Modifies the original dict-like "target".
     """
     for k, v in source.items():
-        if k in target and (
-            isinstance(v, dict) or (isinstance(v, YAML) and v.is_mapping())
-        ):
+        if k in target and isinstance(target[k], dict):
             # assumption: all inputs have been validated.
-            assert isinstance(target[k], dict) or isinstance(target[k], YAML)
             merge_left(target[k], v)
         else:
             target[k] = v
 
 
-def load_project_definition(paths: List[Path]) -> dict:
+def load_project_definition(paths: List[Path]) -> ProjectDefinition:
     """
     Loads project definition, optionally overriding values. Definition values
     are merged in left-to-right order (increasing precedence).
     """
     spaths: List[SecurePath] = [SecurePath(p) for p in paths]
     if len(spaths) == 0:
         raise ValueError("Need at least one definition file.")
 
     with spaths[0].open("r", read_file_limit_mb=DEFAULT_SIZE_LIMIT_MB) as base_yml:
-        definition = load(base_yml.read(), project_schema)
+        definition = load(base_yml.read(), Loader=yaml.loader.BaseLoader)
 
     for override_path in spaths[1:]:
         with override_path.open(
             "r", read_file_limit_mb=DEFAULT_SIZE_LIMIT_MB
         ) as override_yml:
-            overrides = load(override_yml.read(), project_override_schema)
+            overrides = load(override_yml.read(), Loader=yaml.loader.BaseLoader)
             merge_left(definition, overrides)
 
         # TODO: how to show good error messages here?
-        definition.revalidate(project_schema)
 
-    return definition.data
+    return ProjectDefinition(**definition)
 
 
-def generate_local_override_yml(project: Union[Dict, YAML]) -> YAML:
+def generate_local_override_yml(
+    project: ProjectDefinition,
+) -> ProjectDefinition:
     """
     Generates defaults for optional keys in the same YAML structure as the project
     schema. The returned YAML object can be saved directly to a file, if desired.
     A connection is made using global context to resolve current role and warehouse.
     """
     conn = cli_context.connection
     user = clean_identifier(get_env_username() or DEFAULT_USERNAME)
     role = conn.role
     warehouse = conn.warehouse
 
     local: dict = {}
-    if "native_app" in project:
-        name = clean_identifier(project["native_app"]["name"])
+    if project.native_app:
+        name = clean_identifier(project.native_app.name)
         app_identifier = to_identifier(name)
         user_app_identifier = append_to_identifier(app_identifier, f"_{user}")
         package_identifier = append_to_identifier(app_identifier, f"_pkg_{user}")
         local["native_app"] = {
             "application": {
                 "name": user_app_identifier,
                 "role": role,
                 "debug": True,
                 "warehouse": warehouse,
             },
             "package": {"name": package_identifier, "role": role},
         }
+    # TODO: this is an ugly workaround, because pydantics BaseModel.model_copy(update=) doesn't work properly
+    # After fixing UpdatableModel.update_from_dict it should be used here
+    target_definition = project.model_dump()
+    merge_left(target_definition, local)
 
-    return as_document(local, project_override_schema)
+    return ProjectDefinition(**target_definition)
 
 
 def default_app_package(project_name: str):
     user = clean_identifier(get_env_username() or DEFAULT_USERNAME)
     return append_to_identifier(to_identifier(project_name), f"_pkg_{user}")
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/definition_manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import functools
 import os
 from pathlib import Path
 from typing import List, Optional
 
 from snowflake.cli.api.exceptions import MissingConfiguration
 from snowflake.cli.api.project.definition import load_project_definition
+from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
 
 
 def _compat_is_mount(path: Path):
     try:
         return path.is_mount()
     except NotImplementedError:
         # If we can't figure out if path is mount then let's assume it is
@@ -96,9 +97,9 @@
     @staticmethod
     def _user_definition_file_if_available(project_path: Path) -> Optional[Path]:
         return DefinitionManager._definition_if_available(
             DefinitionManager.USER_DEFINITION_FILENAME, project_path
         )
 
     @functools.cached_property
-    def project_definition(self) -> dict:
+    def project_definition(self) -> ProjectDefinition:
         return load_project_definition(self._project_config_paths)
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/project/util.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import codecs
 import os
 import re
 from typing import Optional
 
 IDENTIFIER = r'((?:"[^"]*(?:""[^"]*)*")|(?:[A-Za-z_][\w$]{0,254}))'
+IDENTIFIER_NO_LENGTH = r'((?:"[^"]*(?:""[^"]*)*")|(?:[A-Za-z_][\w$]*))'
 DB_SCHEMA_AND_NAME = f"{IDENTIFIER}[.]{IDENTIFIER}[.]{IDENTIFIER}"
 SCHEMA_AND_NAME = f"{IDENTIFIER}[.]{IDENTIFIER}"
 GLOB_REGEX = r"^[a-zA-Z0-9_\-./*?**\p{L}\p{N}]+$"
 RELATIVE_PATH = r"^[^/][\p{L}\p{N}_\-.][^/]*$"
 
 SINGLE_QUOTED_STRING_LITERAL_REGEX = r"'((?:\\.|''|[^'\n])+?)'"
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/cursor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/api/utils/rendering.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/cli_app.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from snowflake.cli.app.dev.pycharm_remote_debug import (
     setup_pycharm_remote_debugger_if_provided,
 )
 from snowflake.cli.app.main_typer import SnowCliMainTyper
 from snowflake.cli.app.printing import MessageResult, print_result
 from snowflake.connector.config_manager import CONFIG_MANAGER
 
-app: SnowCliMainTyper = SnowCliMainTyper()
 log = logging.getLogger(__name__)
 
 _api = Api(plugin_config_provider=PluginConfigProviderImpl())
 api_provider.register_api(_api)
 
 _commands_registration = CommandsRegistrationWithCallbacks(_api.plugin_config_provider)
 
@@ -122,97 +121,102 @@
                 {"key": "system_info", "value": platform.platform()},
             ],
         )
         print_result(result, output_format=OutputFormat.JSON)
         _exit_with_cleanup()
 
 
-@app.callback()
-def default(
-    version: bool = typer.Option(
-        None,
-        "--version",
-        help="Shows version of the Snowflake CLI",
-        callback=_version_callback,
-        is_eager=True,
-    ),
-    docs: bool = typer.Option(
-        None,
-        "--docs",
-        hidden=True,
-        help="Generates Snowflake CLI documentation",
-        callback=_docs_callback,
-        is_eager=True,
-    ),
-    structure: bool = typer.Option(
-        None,
-        "--structure",
-        hidden=True,
-        help="Prints Snowflake CLI structure of commands",
-        callback=_commands_structure_callback,
-        is_eager=True,
-    ),
-    info: bool = typer.Option(
-        None,
-        "--info",
-        help="Shows information about the Snowflake CLI",
-        callback=_info_callback,
-    ),
-    configuration_file: Path = typer.Option(
-        None,
-        "--config-file",
-        help="Specifies Snowflake CLI configuration file that should be used",
-        exists=True,
-        dir_okay=False,
-        is_eager=True,
-        callback=_config_init_callback,
-    ),
-    pycharm_debug_library_path: str = typer.Option(
-        None,
-        "--pycharm-debug-library-path",
-        hidden=True,
-    ),
-    pycharm_debug_server_host: str = typer.Option(
-        "localhost",
-        "--pycharm-debug-server-host",
-        hidden=True,
-    ),
-    pycharm_debug_server_port: int = typer.Option(
-        12345,
-        "--pycharm-debug-server-port",
-        hidden=True,
-    ),
-    disable_external_command_plugins: bool = typer.Option(
-        None,
-        "--disable-external-command-plugins",
-        help="Disable external command plugins",
-        callback=_disable_external_command_plugins_callback,
-        is_eager=True,
-        hidden=True,
-    ),
-    # THIS OPTION SHOULD BE THE LAST OPTION IN THE LIST!
-    # ---
-    # This is a hidden artificial option used only to guarantee execution of commands registration
-    # and make this guaranty not dependent on other callbacks.
-    # Commands registration is invoked as soon as all callbacks
-    # decorated with "_commands_registration.before" are executed
-    # but if there are no such callbacks (at the result of possible future changes)
-    # then we need to invoke commands registration manually.
-    #
-    # This option is also responsible for resetting registration state for test purposes.
-    commands_registration: bool = typer.Option(
-        True,
-        "--commands-registration",
-        help="Commands registration",
-        hidden=True,
-        is_eager=True,
-        callback=_commands_registration_callback,
-    ),
-) -> None:
-    """
-    Snowflake CLI tool for developers.
-    """
-    setup_pycharm_remote_debugger_if_provided(
-        pycharm_debug_library_path=pycharm_debug_library_path,
-        pycharm_debug_server_host=pycharm_debug_server_host,
-        pycharm_debug_server_port=pycharm_debug_server_port,
-    )
+def app_factory() -> SnowCliMainTyper:
+    app = SnowCliMainTyper()
+
+    @app.callback()
+    def default(
+        version: bool = typer.Option(
+            None,
+            "--version",
+            help="Shows version of the Snowflake CLI",
+            callback=_version_callback,
+            is_eager=True,
+        ),
+        docs: bool = typer.Option(
+            None,
+            "--docs",
+            hidden=True,
+            help="Generates Snowflake CLI documentation",
+            callback=_docs_callback,
+            is_eager=True,
+        ),
+        structure: bool = typer.Option(
+            None,
+            "--structure",
+            hidden=True,
+            help="Prints Snowflake CLI structure of commands",
+            callback=_commands_structure_callback,
+            is_eager=True,
+        ),
+        info: bool = typer.Option(
+            None,
+            "--info",
+            help="Shows information about the Snowflake CLI",
+            callback=_info_callback,
+        ),
+        configuration_file: Path = typer.Option(
+            None,
+            "--config-file",
+            help="Specifies Snowflake CLI configuration file that should be used",
+            exists=True,
+            dir_okay=False,
+            is_eager=True,
+            callback=_config_init_callback,
+        ),
+        pycharm_debug_library_path: str = typer.Option(
+            None,
+            "--pycharm-debug-library-path",
+            hidden=True,
+        ),
+        pycharm_debug_server_host: str = typer.Option(
+            "localhost",
+            "--pycharm-debug-server-host",
+            hidden=True,
+        ),
+        pycharm_debug_server_port: int = typer.Option(
+            12345,
+            "--pycharm-debug-server-port",
+            hidden=True,
+        ),
+        disable_external_command_plugins: bool = typer.Option(
+            None,
+            "--disable-external-command-plugins",
+            help="Disable external command plugins",
+            callback=_disable_external_command_plugins_callback,
+            is_eager=True,
+            hidden=True,
+        ),
+        # THIS OPTION SHOULD BE THE LAST OPTION IN THE LIST!
+        # ---
+        # This is a hidden artificial option used only to guarantee execution of commands registration
+        # and make this guaranty not dependent on other callbacks.
+        # Commands registration is invoked as soon as all callbacks
+        # decorated with "_commands_registration.before" are executed
+        # but if there are no such callbacks (at the result of possible future changes)
+        # then we need to invoke commands registration manually.
+        #
+        # This option is also responsible for resetting registration state for test purposes.
+        commands_registration: bool = typer.Option(
+            True,
+            "--commands-registration",
+            help="Commands registration",
+            hidden=True,
+            is_eager=True,
+            callback=_commands_registration_callback,
+        ),
+    ) -> None:
+        """
+        Snowflake CLI tool for developers.
+        """
+        setup_pycharm_remote_debugger_if_provided(
+            pycharm_debug_library_path=pycharm_debug_library_path,
+            pycharm_debug_server_host=pycharm_debug_server_host,
+            pycharm_debug_server_port=pycharm_debug_server_port,
+        )
+
+    return app
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/loggers.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             },
         },
     )
     loggers: Dict[str, Any] = field(
         default_factory=lambda: {
             "snowflake.cli": LoggerConfig(handlers=["console", "file"]),
             "snowflake": LoggerConfig(),
+            "snowflake.connector.telemetry": LoggerConfig(level=logging.CRITICAL),
         }
     )
 
 
 def _remove_underscore_prefixes_from_keys(d: Dict[str, Any]) -> None:
     for k, v in list(d.items()):
         if k.startswith("_"):
@@ -121,14 +122,16 @@
     if verbose and debug:
         raise typer.BadParameter("Only one parameter `verbose` or `debug` is possible")
     elif debug:
         config.handlers["console"].update(
             level=logging.DEBUG,
             formatter="detailed_formatter",
         )
+        # In debug mode we also want to get snowflake connector logs
+        config.loggers["snowflake"].handlers = ["file", "console"]
     elif verbose:
         config.handlers["console"].update(level=logging.INFO)
 
     global_log_level = config.handlers["console"]["level"]
 
     file_logs_config = FileLogsConfig(debug=debug)
     if file_logs_config.save_logs:
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/main_typer.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/printing.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/telemetry.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/builtin_plugins.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from snowflake.cli.plugins.connection import plugin_spec as connection_plugin_spec
+from snowflake.cli.plugins.git import plugin_spec as git_plugin_spec
 from snowflake.cli.plugins.nativeapp import plugin_spec as nativeapp_plugin_spec
 from snowflake.cli.plugins.object import plugin_spec as object_plugin_spec
 from snowflake.cli.plugins.render import plugin_spec as render_plugin_spec
 from snowflake.cli.plugins.snowpark import plugin_spec as snowpark_plugin_spec
 from snowflake.cli.plugins.spcs import plugin_spec as spcs_plugin_spec
 from snowflake.cli.plugins.sql import plugin_spec as sql_plugin_spec
+from snowflake.cli.plugins.stage import plugin_spec as stage_plugin_spec
 from snowflake.cli.plugins.streamlit import plugin_spec as streamlit_plugin_spec
 
+
 # plugin name to plugin spec
-builtin_plugin_name_to_plugin_spec = {
-    "connection": connection_plugin_spec,
-    "spcs": spcs_plugin_spec,
-    "nativeapp": nativeapp_plugin_spec,
-    "object": object_plugin_spec,
-    "render": render_plugin_spec,
-    "snowpark": snowpark_plugin_spec,
-    "sql": sql_plugin_spec,
-    "streamlit": streamlit_plugin_spec,
-}
+def get_builtin_plugin_name_to_plugin_spec():
+    plugin_specs = {
+        "connection": connection_plugin_spec,
+        "spcs": spcs_plugin_spec,
+        "nativeapp": nativeapp_plugin_spec,
+        "object": object_plugin_spec,
+        "render": render_plugin_spec,
+        "snowpark": snowpark_plugin_spec,
+        "stage": stage_plugin_spec,
+        "sql": sql_plugin_spec,
+        "streamlit": streamlit_plugin_spec,
+        "git": git_plugin_spec,
+    }
+
+    return plugin_specs
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/command_plugins_loader.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from snowflake.cli.app.commands_registration import (
     LoadedBuiltInCommandPlugin,
     LoadedCommandPlugin,
     LoadedExternalCommandPlugin,
 )
 from snowflake.cli.app.commands_registration.builtin_plugins import (
-    builtin_plugin_name_to_plugin_spec,
+    get_builtin_plugin_name_to_plugin_spec,
 )
 from snowflake.cli.app.commands_registration.exception_logging import exception_logging
 
 log = logging.getLogger(__name__)
 log_exception = exception_logging(log)
 
 
@@ -27,15 +27,15 @@
         plugin_manager = pluggy.PluginManager(SNOWCLI_COMMAND_PLUGIN_NAMESPACE)
         plugin_manager.add_hookspecs(plugin_hook_specs)
         self._plugin_manager = plugin_manager
         self._loaded_plugins: Dict[str, LoadedCommandPlugin] = {}
         self._loaded_command_paths: Dict[CommandPath, LoadedCommandPlugin] = {}
 
     def register_builtin_plugins(self) -> None:
-        for (plugin_name, plugin) in builtin_plugin_name_to_plugin_spec.items():
+        for plugin_name, plugin in get_builtin_plugin_name_to_plugin_spec().items():
             try:
                 self._plugin_manager.register(plugin=plugin, name=plugin_name)
             except Exception as ex:
                 log_exception(
                     f"Cannot register plugin [{plugin_name}]: {ex.__str__()}", ex
                 )
 
@@ -47,15 +47,15 @@
                 )
             except Exception as ex:
                 log_exception(
                     f"Cannot register plugin [{plugin_name}]: {ex.__str__()}", ex
                 )
 
     def load_all_registered_plugins(self) -> List[LoadedCommandPlugin]:
-        for (plugin_name, plugin) in self._plugin_manager.list_name_plugin():
+        for plugin_name, plugin in self._plugin_manager.list_name_plugin():
             self._load_plugin(plugin_name, plugin)
         return list(self._loaded_plugins.values())
 
     def _load_plugin(self, plugin_name: str, plugin) -> Optional[LoadedCommandPlugin]:
         already_loaded_plugin = self._loaded_plugins.get(plugin_name)
         if already_loaded_plugin:
             return already_loaded_plugin
@@ -85,15 +85,15 @@
             loaded_plugin.command_spec.full_command_path
         ] = loaded_plugin
         return loaded_plugin
 
     def _load_plugin_spec(
         self, plugin_name: str, plugin
     ) -> Optional[LoadedCommandPlugin]:
-        if plugin_name in builtin_plugin_name_to_plugin_spec.keys():
+        if plugin_name in get_builtin_plugin_name_to_plugin_spec().keys():
             return self._load_builtin_plugin_spec(plugin_name, plugin)
         else:
             return self._load_external_plugin_spec(plugin_name, plugin)
 
     def _load_builtin_plugin_spec(
         self, plugin_name: str, plugin
     ) -> Optional[LoadedCommandPlugin]:
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/threadsafe.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/commands_registration/typer_registration.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/commands_structure.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/pycharm_remote_debug.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/generator.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 from click import ClickException, Context, Parameter  # type: ignore
 from click.core import ParameterSource  # type: ignore
 from click.types import StringParamType
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.flags import (
     PLAIN_PASSWORD_MSG,
     ConnectionOption,
+    DiagAllowlistPathOption,
+    DiagLogPathOption,
+    EnableDiagOption,
     MfaPasscodeOption,
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.config import (
     ConnectionConfig,
     add_connection,
     connection_exists,
     get_all_connections,
     get_connection_dict,
+    get_default_connection_name,
     set_config_value,
 )
 from snowflake.cli.api.console import cli_console
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.output.types import (
     CollectionResult,
     CommandResult,
@@ -58,20 +62,22 @@
 
 @app.command(name="list")
 def list_connections(**options) -> CommandResult:
     """
     Lists configured connections.
     """
     connections = get_all_connections()
+    default_connection = get_default_connection_name()
     result = (
         {
             "connection_name": connection_name,
             "parameters": _mask_password(
                 connection_config.to_dict_of_known_non_empty_values()
             ),
+            "is_default": connection_name == default_connection,
         }
         for connection_name, connection_config in connections.items()
     )
     return CollectionResult(result)
 
 
 def require_integer(field_name: str):
@@ -229,48 +235,63 @@
     return MessageResult(
         f"Wrote new connection {connection_name} to {CONFIG_MANAGER.file_path}"
     )
 
 
 @app.command(requires_connection=False)
 def test(
-    connection: str = ConnectionOption, mfa_passcode: str = MfaPasscodeOption, **options
+    connection: str = ConnectionOption,
+    mfa_passcode: str = MfaPasscodeOption,
+    enable_diag: bool = EnableDiagOption,
+    diag_log_path: str = DiagLogPathOption,
+    diag_allowlist_path: str = DiagAllowlistPathOption,
+    **options,
 ) -> CommandResult:
     """
     Tests the connection to Snowflake.
     """
 
     # Test connection
     conn = cli_context.connection
 
     # Test session attributes
     om = ObjectManager()
     try:
+        # "use database" operation changes schema to default "public",
+        # so to test schema set up by user we need to copy it here:
+        schema = conn.schema
+
         if conn.role:
-            om.use(object_type=ObjectType.ROLE, name=conn.role)
+            om.use(object_type=ObjectType.ROLE, name=f'"{conn.role}"')
         if conn.database:
-            om.use(object_type=ObjectType.DATABASE, name=conn.database)
-        if conn.schema:
-            om.use(object_type=ObjectType.SCHEMA, name=conn.schema)
+            om.use(object_type=ObjectType.DATABASE, name=f'"{conn.database}"')
+        if schema:
+            om.use(object_type=ObjectType.SCHEMA, name=f'"{schema}"')
         if conn.warehouse:
-            om.use(object_type=ObjectType.WAREHOUSE, name=conn.warehouse)
+            om.use(object_type=ObjectType.WAREHOUSE, name=f'"{conn.warehouse}"')
+
     except ProgrammingError as err:
         raise ClickException(str(err))
 
     result = {
         "Connection name": connection,
         "Status": "OK",
         "Host": conn.host,
         "Account": conn.account,
         "User": conn.user,
         "Role": f'{conn.role or "not set"}',
         "Database": f'{conn.database or "not set"}',
         "Warehouse": f'{conn.warehouse or "not set"}',
     }
 
+    if enable_diag:
+        result[
+            "Diag Report Location"
+        ] = f"{diag_log_path}/SnowflakeConnectionTestReport.txt"
+
     return ObjectResult(result)
 
 
 @app.command(requires_connection=False)
 def set_default(
     name: str = typer.Argument(
         help="Name of the connection, as defined in your `config.toml`"
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/connection/util.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/artifacts.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 from click import ClickException
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
+from snowflake.cli.api.project.schemas.native_app.path_mapping import PathMapping
 from snowflake.cli.api.secure_path import SecurePath
 from yaml import safe_load
 
 
 class DeployRootError(ClickException):
     """
     The deploy root was incorrectly specified.
@@ -149,16 +150,16 @@
 
 def translate_artifact(item: Union[dict, str]) -> ArtifactMapping:
     """
     Builds an artifact mapping from a project definition value.
     Validation is done later when we actually resolve files / folders.
     """
 
-    if isinstance(item, dict):
-        return ArtifactMapping(item["src"], item.get("dest", item["src"]))
+    if isinstance(item, PathMapping):
+        return ArtifactMapping(item.src, item.dest if item.dest else item.src)
 
     elif isinstance(item, str):
         return ArtifactMapping(item, item)
 
     # XXX: validation should have caught this
     raise ArtifactError("Item is not a valid artifact!")
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,40 @@
 
 import typer
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_project_definition,
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
-from snowflake.cli.api.output.types import CommandResult, MessageResult
+from snowflake.cli.api.output.types import (
+    CollectionResult,
+    CommandResult,
+    MessageResult,
+)
+from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.plugins.nativeapp.common_flags import ForceOption, InteractiveOption
-from snowflake.cli.plugins.nativeapp.init import nativeapp_init
+from snowflake.cli.plugins.nativeapp.init import (
+    OFFICIAL_TEMPLATES_GITHUB_URL,
+    nativeapp_init,
+)
 from snowflake.cli.plugins.nativeapp.manager import NativeAppManager
 from snowflake.cli.plugins.nativeapp.policy import (
     AllowAlwaysPolicy,
     AskAlwaysPolicy,
     DenyAlwaysPolicy,
 )
 from snowflake.cli.plugins.nativeapp.run_processor import NativeAppRunProcessor
 from snowflake.cli.plugins.nativeapp.teardown_processor import (
     NativeAppTeardownProcessor,
 )
-from snowflake.cli.plugins.nativeapp.utils import is_tty_interactive
+from snowflake.cli.plugins.nativeapp.utils import (
+    get_first_paragraph_from_markdown_file,
+    is_tty_interactive,
+    shallow_git_clone,
+)
 from snowflake.cli.plugins.nativeapp.version.commands import app as versions_app
 
 app = SnowTyper(
     name="app",
     help="Manages a Snowflake Native App",
 )
 app.add_typer(versions_app)
@@ -65,14 +77,47 @@
         path=path, name=name, git_url=template_repo, template=template
     )
     return MessageResult(
         f"Snowflake Native App project {project.name} has been created at: {path}"
     )
 
 
+@app.command("list-templates", hidden=True)
+def app_list_templates(**options) -> CommandResult:
+    """
+    Prints information regarding the official templates that can be used with snow app init.
+    """
+    with SecurePath.temporary_directory() as temp_path:
+        repo = shallow_git_clone(OFFICIAL_TEMPLATES_GITHUB_URL, temp_path.path)
+
+        # Mark a directory as a template if a project definition jinja template is inside
+        template_directories = [
+            entry.name
+            for entry in repo.head.commit.tree
+            if (temp_path / entry.name / "snowflake.yml.jinja").exists()
+        ]
+
+        # get the template descriptions from the README.md in its directory
+        template_descriptions = [
+            get_first_paragraph_from_markdown_file(
+                (temp_path / directory / "README.md").path
+            )
+            for directory in template_directories
+        ]
+
+        result = (
+            {"template": directory, "description": description}
+            for directory, description in zip(
+                template_directories, template_descriptions
+            )
+        )
+
+        return CollectionResult(result)
+
+
 @app.command("bundle", hidden=True)
 @with_project_definition("native_app")
 def app_bundle(
     **options,
 ) -> CommandResult:
     """
     Prepares a local folder with configured app artifacts.
@@ -175,7 +220,26 @@
     """
     processor = NativeAppTeardownProcessor(
         project_definition=cli_context.project_definition,
         project_root=cli_context.project_root,
     )
     processor.process(force)
     return MessageResult(f"Teardown is now complete.")
+
+
+@app.command("deploy", requires_connection=True)
+@with_project_definition("native_app")
+def app_deploy(
+    **options,
+) -> CommandResult:
+    """
+    Creates an application package in your Snowflake account and syncs the local changes to the stage without creating or updating the application.
+    """
+    manager = NativeAppManager(
+        project_definition=cli_context.project_definition,
+        project_root=cli_context.project_root,
+    )
+
+    manager.build_bundle()
+    manager.deploy()
+
+    return MessageResult(f"Deployed successfully.")
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/common_flags.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/constants.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/exceptions.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, name: str):
         super().__init__(
             f"An Application Package {name} already exists in account that may have been created without Snowflake CLI."
         )
 
 
 class ApplicationPackageDoesNotExistError(ClickException):
-    """An application package of the specified name does not exist in the Snowflake acccount."""
+    """An application package of the specified name does not exist in the Snowflake account."""
 
     def __init__(self, name: str):
         super().__init__(
             f"Application Package {name} does not exist in the Snowflake account."
         )
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/init.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,26 +218,18 @@
     """
     use_whole_repo_as_template = git_url and not template
     if not use_whole_repo_as_template:
         git_url = git_url if git_url else OFFICIAL_TEMPLATES_GITHUB_URL
 
     try:
         with SecurePath.temporary_directory() as temp_path:
-            from git import Repo
             from git import rmtree as git_rmtree
+            from snowflake.cli.plugins.nativeapp.utils import shallow_git_clone
 
-            # Clone the repository in the temporary directory with options.
-            repo = Repo.clone_from(
-                url=git_url,
-                to_path=temp_path.path,
-                filter=["tree:0"],
-                depth=1,
-            )
-            # Close repo to avoid issues with permissions on Windows
-            repo.close()
+            shallow_git_clone(git_url, temp_path.path)
 
             if use_whole_repo_as_template:
                 # the template is the entire git repository
                 template_root = temp_path
                 # Remove all git history before we move the repo
                 git_rmtree((template_root / ".git").path)
             else:
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict, List, Optional
+from typing import List, Optional
 
+import jinja2
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
 from snowflake.cli.api.project.definition import (
     default_app_package,
     default_application,
     default_role,
 )
+from snowflake.cli.api.project.schemas.native_app.native_app import NativeApp
 from snowflake.cli.api.project.util import (
     extract_schema,
     to_identifier,
     unquote_identifier,
 )
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import make_snowsight_url
 from snowflake.cli.plugins.nativeapp.artifacts import (
     ArtifactMapping,
     build_bundle,
     translate_artifact,
 )
 from snowflake.cli.plugins.nativeapp.constants import (
+    ALLOWED_SPECIAL_COMMENTS,
+    COMMENT_COL,
     ERROR_MESSAGE_606,
     ERROR_MESSAGE_2043,
+    INTERNAL_DISTRIBUTION,
     NAME_COL,
     OWNER_COL,
+    SPECIAL_COMMENT,
 )
-from snowflake.cli.plugins.nativeapp.exceptions import UnexpectedOwnerError
-from snowflake.cli.plugins.object.stage.diff import (
+from snowflake.cli.plugins.nativeapp.exceptions import (
+    ApplicationPackageAlreadyExistsError,
+    InvalidPackageScriptError,
+    MissingPackageScriptError,
+    UnexpectedOwnerError,
+)
+from snowflake.cli.plugins.stage.diff import (
     DiffResult,
     stage_diff,
     sync_local_diff_with_stage,
 )
 from snowflake.connector import ProgrammingError
+from snowflake.connector.cursor import DictCursor
 
 
 def generic_sql_error_handler(
     err: ProgrammingError, role: Optional[str] = None, warehouse: Optional[str] = None
 ):
     # Potential refactor: If moving away from Python 3.8 and 3.9 to >= 3.10, use match ... case
     if err.errno == 2043 or err.msg.__contains__(ERROR_MESSAGE_2043):
@@ -95,101 +107,127 @@
 
 
 class NativeAppManager(SqlExecutionMixin):
     """
     Base class with frequently used functionality already implemented and ready to be used by related subclasses.
     """
 
-    def __init__(self, project_definition: Dict, project_root: Path):
+    def __init__(self, project_definition: NativeApp, project_root: Path):
         super().__init__()
         self._project_root = project_root
         self._project_definition = project_definition
 
     @property
     def project_root(self) -> Path:
         return self._project_root
 
     @property
-    def definition(self) -> Dict:
+    def definition(self) -> NativeApp:
         return self._project_definition
 
     @cached_property
     def artifacts(self) -> List[ArtifactMapping]:
-        return [translate_artifact(item) for item in self.definition["artifacts"]]
+        return [translate_artifact(item) for item in self.definition.artifacts]
 
     @cached_property
     def deploy_root(self) -> Path:
-        return Path(self.project_root, self.definition["deploy_root"])
+        return Path(self.project_root, self.definition.deploy_root)
 
     @cached_property
     def package_scripts(self) -> List[str]:
         """
         Relative paths to package scripts from the project root.
         """
-        return self.definition.get("package", {}).get("scripts", [])
+        if self.definition.package and self.definition.package.scripts:
+            return self.definition.package.scripts
+        else:
+            return []
 
     @cached_property
     def stage_fqn(self) -> str:
-        return f'{self.package_name}.{self.definition["source_stage"]}'
+        return f"{self.package_name}.{self.definition.source_stage}"
 
     @cached_property
     def stage_schema(self) -> Optional[str]:
         return extract_schema(self.stage_fqn)
 
     @cached_property
     def package_warehouse(self) -> Optional[str]:
-        return self.definition.get("package", {}).get("warehouse", self._conn.warehouse)
+        if self.definition.package and self.definition.package.warehouse:
+            return self.definition.package.warehouse
+        else:
+            return self._conn.warehouse
 
     @cached_property
     def application_warehouse(self) -> Optional[str]:
-        return self.definition.get("application", {}).get(
-            "warehouse", self._conn.warehouse
-        )
+        if self.definition.application and self.definition.application.warehouse:
+            return self.definition.application.warehouse
+        else:
+            return self._conn.warehouse
 
     @cached_property
     def project_identifier(self) -> str:
         # name is expected to be a valid Snowflake identifier, but PyYAML
         # will sometimes strip out double quotes so we try to get them back here.
-        return to_identifier(self.definition["name"])
+        return to_identifier(self.definition.name)
 
     @cached_property
     def package_name(self) -> str:
-        return to_identifier(
-            self.definition.get("package", {}).get(
-                "name", default_app_package(self.project_identifier)
-            )
-        )
+        if self.definition.package and self.definition.package.name:
+            return to_identifier(self.definition.package.name)
+        else:
+            return to_identifier(default_app_package(self.project_identifier))
 
     @cached_property
     def package_role(self) -> str:
-        return self.definition.get("package", {}).get("role", None) or default_role()
+        if self.definition.package and self.definition.package.role:
+            return self.definition.package.role
+        else:
+            return self._default_role
 
     @cached_property
     def package_distribution(self) -> str:
-        return (
-            self.definition.get("package", {}).get("distribution", "internal").lower()
-        )
+        if self.definition.package and self.definition.package.distribution:
+            return self.definition.package.distribution.lower()
+        else:
+            return "internal"
 
     @cached_property
     def app_name(self) -> str:
-        return to_identifier(
-            self.definition.get("application", {}).get(
-                "name", default_application(self.project_identifier)
-            )
-        )
+        if self.definition.application and self.definition.application.name:
+            return to_identifier(self.definition.application.name)
+        else:
+            return to_identifier(default_application(self.project_identifier))
 
     @cached_property
     def app_role(self) -> str:
-        return (
-            self.definition.get("application", {}).get("role", None) or default_role()
-        )
+        if self.definition.application and self.definition.application.role:
+            return self.definition.application.role
+        else:
+            return self._default_role
+
+    @cached_property
+    def _default_role(self) -> str:
+        role = default_role()
+        if role is None:
+            role = self._get_current_role()
+        return role
+
+    def _get_current_role(self) -> str:
+        role_result = self._execute_query(
+            "select current_role()", cursor_class=DictCursor
+        ).fetchone()
+        return role_result["CURRENT_ROLE()"]
 
     @cached_property
     def debug_mode(self) -> bool:
-        return self.definition.get("application", {}).get("debug", True)
+        if self.definition.application:
+            return self.definition.application.debug
+        else:
+            return True
 
     @cached_property
     def get_app_pkg_distribution_in_snowflake(self) -> str:
         """
         Returns the 'distribution' attribute of a 'describe application package' SQL query, in lowercase.
         """
         with self.use_role(self.package_role):
@@ -309,7 +347,105 @@
                 "application packages", self.package_name, name_col=NAME_COL
             )
 
     def get_snowsight_url(self) -> str:
         """Returns the URL that can be used to visit this app via Snowsight."""
         name = unquote_identifier(self.app_name)
         return make_snowsight_url(self._conn, f"/#/apps/application/{name}")
+
+    def create_app_package(self) -> None:
+        """
+        Creates the application package with our up-to-date stage if none exists.
+        """
+
+        # 1. Check for existing existing application package
+        show_obj_row = self.get_existing_app_pkg_info()
+
+        if show_obj_row:
+            # 1. Check for the right owner role
+            ensure_correct_owner(
+                row=show_obj_row, role=self.package_role, obj_name=self.package_name
+            )
+
+            # 2. Check distribution of the existing application package
+            actual_distribution = self.get_app_pkg_distribution_in_snowflake
+            if not self.verify_project_distribution(actual_distribution):
+                cc.warning(
+                    f"Continuing to execute `snow app run` on application package {self.package_name} with distribution '{actual_distribution}'."
+                )
+
+            # 3. If actual_distribution is external, skip comment check
+            if actual_distribution == INTERNAL_DISTRIBUTION:
+                row_comment = show_obj_row[COMMENT_COL]
+
+                if row_comment not in ALLOWED_SPECIAL_COMMENTS:
+                    raise ApplicationPackageAlreadyExistsError(self.package_name)
+
+            return
+
+        # If no application package pre-exists, create an application package, with the specified distribution in the project definition file.
+        with self.use_role(self.package_role):
+            cc.step(f"Creating new application package {self.package_name} in account.")
+            self._execute_query(
+                dedent(
+                    f"""\
+                    create application package {self.package_name}
+                        comment = {SPECIAL_COMMENT}
+                        distribution = {self.package_distribution}
+                """
+                )
+            )
+
+    def _apply_package_scripts(self) -> None:
+        """
+        Assuming the application package exists and we are using the correct role,
+        applies all package scripts in-order to the application package.
+        """
+        env = jinja2.Environment(
+            loader=jinja2.loaders.FileSystemLoader(self.project_root),
+            keep_trailing_newline=True,
+            undefined=jinja2.StrictUndefined,
+        )
+
+        queued_queries = []
+        for relpath in self.package_scripts:
+            try:
+                template = env.get_template(relpath)
+                result = template.render(dict(package_name=self.package_name))
+                queued_queries.append(result)
+
+            except jinja2.TemplateNotFound as e:
+                raise MissingPackageScriptError(e.name)
+
+            except jinja2.TemplateSyntaxError as e:
+                raise InvalidPackageScriptError(e.name, e)
+
+            except jinja2.UndefinedError as e:
+                raise InvalidPackageScriptError(relpath, e)
+
+        # once we're sure all the templates expanded correctly, execute all of them
+        try:
+            if self.package_warehouse:
+                self._execute_query(f"use warehouse {self.package_warehouse}")
+
+            for i, queries in enumerate(queued_queries):
+                cc.step(f"Applying package script: {self.package_scripts[i]}")
+                self._execute_queries(queries)
+        except ProgrammingError as err:
+            generic_sql_error_handler(
+                err, role=self.package_role, warehouse=self.package_warehouse
+            )
+
+    def deploy(self) -> DiffResult:
+        """app deploy process"""
+
+        # 1. Create an empty application package, if none exists
+        self.create_app_package()
+
+        with self.use_role(self.package_role):
+            # 2. now that the application package exists, create shared data
+            self._apply_package_scripts()
+
+            # 3. Upload files from deploy root local folder to the above stage
+            diff = self.sync_deploy_root_with_stage(self.package_role)
+
+        return diff
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/policy.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Optional
 
 import typer
 
 
 class PolicyBase(ABC):
-    """Abtract Class for various policies that govern if a Snowflake CLI command can continue execution when it asks for a decision."""
+    """Abstract Class for various policies that govern if a Snowflake CLI command can continue execution when it asks for a decision."""
 
     @abstractmethod
     def should_proceed(self, user_prompt: Optional[str]) -> bool:
         pass
 
 
 class AllowAlwaysPolicy(PolicyBase):
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/run_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,133 +1,46 @@
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict, Optional
+from typing import Optional
 
-import jinja2
 import typer
 from click import UsageError
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
+from snowflake.cli.api.project.schemas.native_app.native_app import NativeApp
 from snowflake.cli.plugins.nativeapp.constants import (
     ALLOWED_SPECIAL_COMMENTS,
     COMMENT_COL,
-    INTERNAL_DISTRIBUTION,
     LOOSE_FILES_MAGIC_VERSION,
     SPECIAL_COMMENT,
     VERSION_COL,
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationAlreadyExistsError,
-    ApplicationPackageAlreadyExistsError,
     ApplicationPackageDoesNotExistError,
-    InvalidPackageScriptError,
-    MissingPackageScriptError,
 )
 from snowflake.cli.plugins.nativeapp.manager import (
     NativeAppCommandProcessor,
     NativeAppManager,
     ensure_correct_owner,
     generic_sql_error_handler,
 )
 from snowflake.cli.plugins.nativeapp.policy import PolicyBase
-from snowflake.cli.plugins.object.stage.diff import DiffResult
-from snowflake.cli.plugins.object.stage.manager import StageManager
+from snowflake.cli.plugins.stage.diff import DiffResult
+from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import SnowflakeCursor
 
 UPGRADE_RESTRICTION_CODES = {93044, 93055, 93045, 93046}
 
 
 class NativeAppRunProcessor(NativeAppManager, NativeAppCommandProcessor):
-    def __init__(self, project_definition: Dict, project_root: Path):
+    def __init__(self, project_definition: NativeApp, project_root: Path):
         super().__init__(project_definition, project_root)
 
-    def create_app_package(self) -> None:
-        """
-        Creates the application package with our up-to-date stage if none exists.
-        """
-
-        # 1. Check for existing existing application package
-        show_obj_row = self.get_existing_app_pkg_info()
-
-        if show_obj_row:
-            # 1. Check for the right owner role
-            ensure_correct_owner(
-                row=show_obj_row, role=self.package_role, obj_name=self.package_name
-            )
-
-            # 2. Check distribution of the existing application package
-            actual_distribution = self.get_app_pkg_distribution_in_snowflake
-            if not self.verify_project_distribution(actual_distribution):
-                cc.warning(
-                    f"Continuing to execute `snow app run` on application package {self.package_name} with distribution '{actual_distribution}'."
-                )
-
-            # 3. If actual_distribution is external, skip comment check
-            if actual_distribution == INTERNAL_DISTRIBUTION:
-                row_comment = show_obj_row[COMMENT_COL]
-
-                if row_comment not in ALLOWED_SPECIAL_COMMENTS:
-                    raise ApplicationPackageAlreadyExistsError(self.package_name)
-
-            return
-
-        # If no application package pre-exists, create an application package, with the specified distribution in the project definition file.
-        with self.use_role(self.package_role):
-            cc.step(f"Creating new application package {self.package_name} in account.")
-            self._execute_query(
-                dedent(
-                    f"""\
-                    create application package {self.package_name}
-                        comment = {SPECIAL_COMMENT}
-                        distribution = {self.package_distribution}
-                """
-                )
-            )
-
-    def _apply_package_scripts(self) -> None:
-        """
-        Assuming the application package exists and we are using the correct role,
-        applies all package scripts in-order to the application package.
-        """
-        env = jinja2.Environment(
-            loader=jinja2.loaders.FileSystemLoader(self.project_root),
-            keep_trailing_newline=True,
-            undefined=jinja2.StrictUndefined,
-        )
-
-        queued_queries = []
-        for relpath in self.package_scripts:
-            try:
-                template = env.get_template(relpath)
-                result = template.render(dict(package_name=self.package_name))
-                queued_queries.append(result)
-
-            except jinja2.TemplateNotFound as e:
-                raise MissingPackageScriptError(e.name)
-
-            except jinja2.TemplateSyntaxError as e:
-                raise InvalidPackageScriptError(e.name, e)
-
-            except jinja2.UndefinedError as e:
-                raise InvalidPackageScriptError(relpath, e)
-
-        # once we're sure all the templates expanded correctly, execute all of them
-        try:
-            if self.package_warehouse:
-                self._execute_query(f"use warehouse {self.package_warehouse}")
-
-            for i, queries in enumerate(queued_queries):
-                cc.step(f"Applying package script: {self.package_scripts[i]}")
-                self._execute_queries(queries)
-        except ProgrammingError as err:
-            generic_sql_error_handler(
-                err, role=self.package_role, warehouse=self.package_warehouse
-            )
-
     def _create_dev_app(self, diff: DiffResult) -> None:
         """
         (Re-)creates the application object with our up-to-date stage.
         """
         with self.use_role(self.app_role):
 
             # 1. Need to use a warehouse to create an application object
@@ -380,19 +293,9 @@
                 policy=policy,
                 version=version,
                 patch=patch,
                 is_interactive=is_interactive,
             )
             return
 
-        # 1. Create an empty application package, if none exists
-        self.create_app_package()
-
-        with self.use_role(self.package_role):
-            # 2. now that the application package exists, create shared data
-            self._apply_package_scripts()
-
-            # 3. Upload files from deploy root local folder to the above stage
-            diff = self.sync_deploy_root_with_stage(self.package_role)
-
-        # 4. Create an application if none exists, else upgrade the application
+        diff = self.deploy()
         self._create_dev_app(diff)
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/teardown_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self.drop_generic_object(
             object_type="application", object_name=self.app_name, role=self.app_role
         )
         return  # The application object was successfully dropped, therefore exit gracefully
 
     def drop_package(self, auto_yes: bool):
         """
-        Attemps to drop application package unless user specifies otherwise.
+        Attempts to drop application package unless user specifies otherwise.
         """
         needs_confirm = True
 
         # 1. If existing application package is not found, exit gracefully
         show_obj_row = self.get_existing_app_pkg_info()
         if show_obj_row is None:
             cc.warning(
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/version/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/nativeapp/version/version_processor.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from textwrap import dedent
 from typing import Dict, List, Optional
 
 import typer
 from click import BadOptionUsage, ClickException
 from snowflake.cli.api.console import cli_console as cc
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
+from snowflake.cli.api.project.schemas.native_app.native_app import NativeApp
 from snowflake.cli.api.project.util import unquote_identifier
 from snowflake.cli.api.utils.cursor import (
     find_all_rows,
     find_first_row,
 )
 from snowflake.cli.plugins.nativeapp.artifacts import find_version_info_in_manifest_file
 from snowflake.cli.plugins.nativeapp.constants import VERSION_COL
@@ -236,15 +237,15 @@
             return  # A new version created automatically has patch 0, we do not need to further increment the patch.
 
         # Add a new patch to an existing (old) version
         self.add_new_patch_to_version(version=version, patch=patch)
 
 
 class NativeAppVersionDropProcessor(NativeAppManager, NativeAppCommandProcessor):
-    def __init__(self, project_definition: Dict, project_root: Path):
+    def __init__(self, project_definition: NativeApp, project_root: Path):
         super().__init__(project_definition, project_root)
 
     def process(
         self,
         version: Optional[str],
         policy: PolicyBase,
         is_interactive: bool,
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from __future__ import annotations
 
 from typing import Tuple
 
 import typer
 from click import ClickException
+from snowflake.cli.api.commands.flags import like_option
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.constants import SUPPORTED_OBJECTS, VALID_SCOPES
 from snowflake.cli.api.output.types import QueryResult
 from snowflake.cli.api.project.util import is_valid_identifier
 from snowflake.cli.plugins.object.manager import ObjectManager
-from snowflake.cli.plugins.object.stage.commands import app as stage_app
+from snowflake.cli.plugins.object.stage_deprecated.commands import app as stage_app
 
 app = SnowTyper(
     name="object",
     help="Manages Snowflake objects like warehouses and stages",
 )
 app.add_typer(stage_app)
 
 
 NameArgument = typer.Argument(help="Name of the object")
 ObjectArgument = typer.Argument(
     help="Type of object. For example table, procedure, streamlit.",
     case_sensitive=False,
 )
-LikeOption = typer.Option(
-    "%%",
-    "--like",
-    "-l",
-    help='SQL LIKE pattern for filtering objects by name. For example, `list function --like "my%"` lists '
-    "all functions that begin with “my”.",
+LikeOption = like_option(
+    help_example='`list function --like "my%"` lists all functions that begin with “my”',
 )
 
 
 def _scope_validate(object_type: str, scope: Tuple[str, str]):
     if scope[1] is not None and not is_valid_identifier(scope[1]):
         raise ClickException("scope name must be a valid identifier")
     if scope[0] is not None and scope[0].lower() not in VALID_SCOPES:
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dataclasses import dataclass
 from typing import Optional
 
 from click import ClickException
 from snowflake.cli.api.commands.flags import OverrideableOption
 from snowflake.cli.api.project.util import (
-    QUOTED_IDENTIFIER_REGEX,
-    UNQUOTED_IDENTIFIER_REGEX,
+    VALID_IDENTIFIER_REGEX,
     is_valid_identifier,
     to_string_literal,
 )
 
 
 @dataclass
 class Tag:
@@ -30,19 +29,17 @@
             "tag must be in the format <name>=<value> where 'name' is a valid identifier and value is a string"
         )
 
 
 def _parse_tag(tag: str) -> Tag:
     import re
 
-    identifier_pattern = re.compile(
-        f"(?P<tag_name>{UNQUOTED_IDENTIFIER_REGEX}|{QUOTED_IDENTIFIER_REGEX})"
-    )
-    value_pattern = re.compile(f"(?P<tag_value>.+)")
-    result = re.fullmatch(f"{identifier_pattern.pattern}={value_pattern.pattern}", tag)
+    identifier_pattern = rf"(?P<tag_name>{VALID_IDENTIFIER_REGEX})"
+    value_pattern = r"(?P<tag_value>.+)"
+    result = re.fullmatch(rf"{identifier_pattern}={value_pattern}", tag)
     if result is not None:
         try:
             return Tag(result.group("tag_name"), result.group("tag_value"))
         except ValueError:
             raise TagError()
     else:
         raise TagError()
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Optional, Tuple, Union
 
 from click import ClickException
 from snowflake.cli.api.constants import OBJECT_TO_NAMES, ObjectNames
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
+from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import SnowflakeCursor
 
 
 def _get_object_names(object_type: str) -> ObjectNames:
     object_type = object_type.lower()
     if object_type.lower() not in OBJECT_TO_NAMES:
         raise ClickException(f"Object of type {object_type} is not supported.")
@@ -40,7 +41,14 @@
         # Image repository is the only supported object that does not have a DESCRIBE command.
         if object_type == "image-repository":
             raise ClickException(
                 f"Describe is currently not supported for object of type image-repository"
             )
         object_name = _get_object_names(object_type).sf_name
         return self._execute_query(f"describe {object_name} {name}")
+
+    def object_exists(self, *, object_type: str, name: str):
+        try:
+            self.describe(object_type=object_type, name=name)
+            return True
+        except ProgrammingError:
+            return False
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/object/stage/diff.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     Could the provided hexadecimal checksum represent a valid md5sum?
     """
     return re.match(MD5SUM_REGEX, checksum) is not None
 
 
 def compute_md5sum(file: Path) -> str:
     """
-    Returns a hexidecimal checksum for the file located at the given path.
+    Returns a hexadecimal checksum for the file located at the given path.
     """
     if not file.is_file():
         raise ValueError(
             "The provided file does not exist or not a (symlink to a) regular file"
         )
 
     # FIXME: there are two cases in which this will fail to provide a matching
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/render/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,115 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
-from pathlib import Path
 from typing import Dict, List, Optional, Set
 
 import typer
 from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_project_definition,
 )
 from snowflake.cli.api.commands.flags import (
+    ReplaceOption,
+    deprecated_flag_callback_enum,
     execution_identifier_argument,
 )
 from snowflake.cli.api.commands.project_initialisation import add_init_command
 from snowflake.cli.api.commands.snow_typer import SnowTyper
-from snowflake.cli.api.constants import DEPLOYMENT_STAGE, ObjectType
+from snowflake.cli.api.constants import (
+    DEFAULT_SIZE_LIMIT_MB,
+    DEPLOYMENT_STAGE,
+    ObjectType,
+)
 from snowflake.cli.api.exceptions import (
     SecretsWithoutExternalAccessIntegrationError,
 )
 from snowflake.cli.api.output.types import (
     CollectionResult,
     CommandResult,
     MessageResult,
     SingleQueryResult,
 )
+from snowflake.cli.api.project.schemas.snowpark.callable import (
+    Callable,
+    FunctionSchema,
+    ProcedureSchema,
+)
+from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.plugins.object.manager import ObjectManager
-from snowflake.cli.plugins.object.stage.manager import StageManager
+from snowflake.cli.plugins.snowpark import package_utils
 from snowflake.cli.plugins.snowpark.common import (
     build_udf_sproc_identifier,
     check_if_replace_is_required,
 )
 from snowflake.cli.plugins.snowpark.manager import FunctionManager, ProcedureManager
-from snowflake.cli.plugins.snowpark.models import PypiOption
-from snowflake.cli.plugins.snowpark.package_utils import get_snowflake_packages
+from snowflake.cli.plugins.snowpark.models import YesNoAsk
+from snowflake.cli.plugins.snowpark.package.anaconda_packages import (
+    AnacondaPackages,
+    AnacondaPackagesManager,
+)
+from snowflake.cli.plugins.snowpark.snowpark_package_paths import SnowparkPackagePaths
 from snowflake.cli.plugins.snowpark.snowpark_shared import (
-    CheckAnacondaForPyPiDependencies,
-    PackageNativeLibrariesOption,
-    PyPiDownloadOption,
-    snowpark_package,
+    AllowSharedLibrariesOption,
+    DeprecatedCheckAnacondaForPyPiDependencies,
+    IgnoreAnacondaOption,
+    IndexUrlOption,
+    SkipVersionCheckOption,
+    deprecated_allow_native_libraries_option,
+    resolve_allow_shared_libraries_yes_no_ask,
 )
+from snowflake.cli.plugins.snowpark.zipper import zip_dir
+from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector import DictCursor, ProgrammingError
 
 log = logging.getLogger(__name__)
 
 app = SnowTyper(
     name="snowpark",
     help="Manages procedures and functions.",
 )
 
-ReplaceOption = typer.Option(
-    False,
-    "--replace",
-    help="Replaces procedure or function, even if no detected changes to metadata",
-)
-
 ObjectTypeArgument = typer.Argument(
     help="Type of Snowpark object",
     case_sensitive=False,
 )
 
 add_init_command(app, project_type="Snowpark", template="default_snowpark")
 
 
 @app.command("deploy", requires_connection=True)
 @with_project_definition("snowpark")
 def deploy(
-    replace: bool = ReplaceOption,
+    replace: bool = ReplaceOption(
+        help="Replaces procedure or function, even if no detected changes to metadata"
+    ),
     **options,
 ) -> CommandResult:
     """
     Deploys procedures and functions defined in project. Deploying the project alters all objects defined in it.
     By default, if any of the objects exist already the commands will fail unless `--replace` flag is provided.
     All deployed objects use the same artifact which is deployed only once.
     """
     snowpark = cli_context.project_definition
+    paths = SnowparkPackagePaths.for_snowpark_project(
+        project_root=SecurePath(cli_context.project_root),
+        snowpark_project_definition=snowpark,
+    )
 
-    procedures = snowpark.get("procedures", [])
-    functions = snowpark.get("functions", [])
+    procedures = snowpark.procedures
+    functions = snowpark.functions
 
     if not procedures and not functions:
         raise ClickException(
             "No procedures or functions were specified in the project definition."
         )
 
-    build_artifact_path = _get_snowpark_artifact_path(snowpark)
-
-    if not build_artifact_path.exists():
+    if not paths.artifact_file.exists():
         raise ClickException(
             "Artifact required for deploying the project does not exist in this directory. "
             "Please use build command to create it."
         )
 
     pm = ProcedureManager()
     fm = FunctionManager()
@@ -108,65 +126,71 @@
         msg = "Following objects already exists. Consider using --replace.\n"
         msg += "\n".join(f"function: {n}" for n in existing_functions)
         msg += "\n" if existing_functions and existing_procedures else ""
         msg += "\n".join(f"procedure: {n}" for n in existing_procedures)
         raise ClickException(msg)
 
     # Create stage
-    stage_name = snowpark.get("stage_name", DEPLOYMENT_STAGE)
+    stage_name = snowpark.stage_name
     stage_manager = StageManager()
     stage_name = stage_manager.to_fully_qualified_name(stage_name)
     stage_manager.create(
         stage_name=stage_name, comment="deployments managed by Snowflake CLI"
     )
 
-    packages = get_snowflake_packages()
+    snowflake_dependencies = _read_snowflake_requrements_file(
+        paths.snowflake_requirements_file
+    )
 
-    artifact_stage_directory = get_app_stage_path(stage_name, snowpark["project_name"])
-    artifact_stage_target = f"{artifact_stage_directory}/{build_artifact_path.name}"
+    artifact_stage_directory = get_app_stage_path(stage_name, snowpark.project_name)
+    artifact_stage_target = (
+        f"{artifact_stage_directory}/{paths.artifact_file.path.name}"
+    )
 
     stage_manager.put(
-        local_path=build_artifact_path,
+        local_path=paths.artifact_file.path,
         stage_path=artifact_stage_directory,
         overwrite=True,
     )
 
     deploy_status = []
     # Procedures
     for procedure in procedures:
         operation_result = _deploy_single_object(
             manager=pm,
             object_type=ObjectType.PROCEDURE,
             object_definition=procedure,
             existing_objects=existing_procedures,
-            packages=packages,
+            snowflake_dependencies=snowflake_dependencies,
             stage_artifact_path=artifact_stage_target,
         )
         deploy_status.append(operation_result)
 
     # Functions
     for function in functions:
         operation_result = _deploy_single_object(
             manager=fm,
             object_type=ObjectType.FUNCTION,
             object_definition=function,
             existing_objects=existing_functions,
-            packages=packages,
+            snowflake_dependencies=snowflake_dependencies,
             stage_artifact_path=artifact_stage_target,
         )
         deploy_status.append(operation_result)
 
     return CollectionResult(deploy_status)
 
 
-def _assert_object_definitions_are_correct(object_type, object_definitions):
+def _assert_object_definitions_are_correct(
+    object_type, object_definitions: List[Callable]
+):
     for definition in object_definitions:
-        database = definition.get("database")
-        schema = definition.get("schema")
-        name = definition["name"]
+        database = definition.database
+        schema = definition.schema_name
+        name = definition.name
         fqn_parts = len(name.split("."))
         if fqn_parts == 3 and database:
             raise ClickException(
                 f"database of {object_type} {name} is redefined in its name"
             )
         if fqn_parts >= 2 and schema:
             raise ClickException(
@@ -192,32 +216,32 @@
             existing_objects[identifier] = current_state
         except ProgrammingError:
             pass
     return existing_objects
 
 
 def _check_if_all_defined_integrations_exists(
-    om: ObjectManager, functions: List[Dict], procedures: List[Dict]
+    om: ObjectManager,
+    functions: List[FunctionSchema],
+    procedures: List[ProcedureSchema],
 ):
     existing_integrations = {
         i["name"].lower()
         for i in om.show(object_type="integration", cursor_class=DictCursor, like=None)
         if i["type"] == "EXTERNAL_ACCESS"
     }
     declared_integration: Set[str] = set()
     for object_definition in [*functions, *procedures]:
         external_access_integrations = {
-            s.lower() for s in object_definition.get("external_access_integrations", [])
+            s.lower() for s in object_definition.external_access_integrations
         }
-        secrets = [s.lower() for s in object_definition.get("secrets", [])]
+        secrets = [s.lower() for s in object_definition.secrets]
 
         if not external_access_integrations and secrets:
-            raise SecretsWithoutExternalAccessIntegrationError(
-                object_definition["name"]
-            )
+            raise SecretsWithoutExternalAccessIntegrationError(object_definition.name)
 
         declared_integration = declared_integration | external_access_integrations
 
     missing = declared_integration - existing_integrations
     if missing:
         raise ClickException(
             f"Following external access integration does not exists in Snowflake: {', '.join(missing)}"
@@ -228,109 +252,184 @@
     artifact_stage_directory = f"@{(stage_name or DEPLOYMENT_STAGE)}/{project_name}"
     return artifact_stage_directory
 
 
 def _deploy_single_object(
     manager: FunctionManager | ProcedureManager,
     object_type: ObjectType,
-    object_definition: Dict,
+    object_definition: Callable,
     existing_objects: Dict[str, Dict],
-    packages: List[str],
+    snowflake_dependencies: List[str],
     stage_artifact_path: str,
 ):
     identifier = build_udf_sproc_identifier(
         object_definition, manager, include_parameter_names=False
     )
     identifier_with_default_values = build_udf_sproc_identifier(
         object_definition,
         manager,
         include_parameter_names=True,
         include_default_values=True,
     )
     log.info("Deploying %s: %s", object_type, identifier_with_default_values)
 
-    handler = object_definition["handler"]
-    returns = object_definition["returns"]
+    handler = object_definition.handler
+    returns = object_definition.returns
+    imports = object_definition.imports
     replace_object = False
 
     object_exists = identifier in existing_objects
     if object_exists:
         replace_object = check_if_replace_is_required(
-            object_type,
-            existing_objects[identifier],
-            handler,
-            returns,
+            object_type=object_type,
+            current_state=existing_objects[identifier],
+            handler=handler,
+            return_type=returns,
+            snowflake_dependencies=snowflake_dependencies,
+            imports=imports,
+            stage_artifact_file=stage_artifact_path,
         )
 
     if object_exists and not replace_object:
         return {
             "object": identifier_with_default_values,
             "type": str(object_type),
             "status": "packages updated",
         }
 
     create_or_replace_kwargs = {
         "identifier": identifier_with_default_values,
         "handler": handler,
         "return_type": returns,
         "artifact_file": stage_artifact_path,
-        "packages": packages,
-        "runtime": object_definition.get("runtime"),
-        "external_access_integrations": object_definition.get(
-            "external_access_integrations"
-        ),
-        "secrets": object_definition.get("secrets"),
-        "imports": object_definition.get("imports", []),
+        "packages": snowflake_dependencies,
+        "runtime": object_definition.runtime,
+        "external_access_integrations": object_definition.external_access_integrations,
+        "secrets": object_definition.secrets,
+        "imports": imports,
     }
     if object_type == ObjectType.PROCEDURE:
-        create_or_replace_kwargs["execute_as_caller"] = object_definition.get(
+        create_or_replace_kwargs[
             "execute_as_caller"
-        )
-
+        ] = object_definition.execute_as_caller
     manager.create_or_replace(**create_or_replace_kwargs)
 
     status = "created" if not object_exists else "definition updated"
     return {
         "object": identifier_with_default_values,
         "type": str(object_type),
         "status": status,
     }
 
 
-def _get_snowpark_artifact_path(snowpark_definition: Dict):
-    source = Path(snowpark_definition["src"])
-    artifact_file = Path.cwd() / (source.name + ".zip")
-    return artifact_file
+deprecated_pypi_download_option = typer.Option(
+    YesNoAsk.NO.value,
+    "--pypi-download",
+    help="Whether to download non-Anaconda packages from PyPi.",
+    hidden=True,
+    callback=deprecated_flag_callback_enum(
+        "--pypi-download flag is deprecated. Snowpark build command"
+        " always tries to download non-Anaconda packages from external index (PyPi by default)."
+    ),
+)
 
 
-@app.command("build")
+def _read_snowflake_requrements_file(file_path: SecurePath):
+    if not file_path.exists():
+        return []
+    return file_path.read_text(file_size_limit_mb=DEFAULT_SIZE_LIMIT_MB).splitlines()
+
+
+@app.command("build", requires_connection=True)
 @with_project_definition("snowpark")
 def build(
-    pypi_download: PypiOption = PyPiDownloadOption,
-    check_anaconda_for_pypi_deps: bool = CheckAnacondaForPyPiDependencies,
-    package_native_libraries: PypiOption = PackageNativeLibrariesOption,
+    ignore_anaconda: bool = IgnoreAnacondaOption,
+    allow_shared_libraries: bool = AllowSharedLibrariesOption,
+    index_url: Optional[str] = IndexUrlOption,
+    skip_version_check: bool = SkipVersionCheckOption,
+    deprecated_package_native_libraries: YesNoAsk = deprecated_allow_native_libraries_option(
+        "--package-native-libraries"
+    ),
+    deprecated_check_anaconda_for_pypi_deps: bool = DeprecatedCheckAnacondaForPyPiDependencies,
+    _deprecated_pypi_download: YesNoAsk = deprecated_pypi_download_option,
     **options,
 ) -> CommandResult:
     """
     Builds the Snowpark project as a `.zip` archive that can be used by `deploy` command.
     The archive is built using only the `src` directory specified in the project file.
     """
-    snowpark = cli_context.project_definition
-    source = Path(snowpark.get("src"))
-    artifact_file = _get_snowpark_artifact_path(snowpark)
-    log.info("Building package using sources from: %s", source.resolve())
-
-    snowpark_package(
-        source=source,
-        artifact_file=artifact_file,
-        pypi_download=pypi_download,  # type: ignore[arg-type]
-        check_anaconda_for_pypi_deps=check_anaconda_for_pypi_deps,
-        package_native_libraries=package_native_libraries,  # type: ignore[arg-type]
+    if not deprecated_check_anaconda_for_pypi_deps:
+        ignore_anaconda = True
+    snowpark_paths = SnowparkPackagePaths.for_snowpark_project(
+        project_root=SecurePath(cli_context.project_root),
+        snowpark_project_definition=cli_context.project_definition,
+    )
+    log.info("Building package using sources from: %s", snowpark_paths.source.path)
+
+    anaconda_packages_manager = AnacondaPackagesManager()
+
+    with SecurePath.temporary_directory() as packages_dir:
+        if snowpark_paths.defined_requirements_file.exists():
+            log.info("Resolving any requirements from requirements.txt...")
+            requirements = package_utils.parse_requirements(
+                requirements_file=snowpark_paths.defined_requirements_file,
+            )
+            anaconda_packages = (
+                AnacondaPackages.empty()
+                if ignore_anaconda
+                else anaconda_packages_manager.find_packages_available_in_snowflake_anaconda()
+            )
+            download_result = package_utils.download_unavailable_packages(
+                requirements=requirements,
+                target_dir=packages_dir,
+                anaconda_packages=anaconda_packages,
+                skip_version_check=skip_version_check,
+                pip_index_url=index_url,
+            )
+            if not download_result.succeeded:
+                raise ClickException(download_result.error_message)
+
+            log.info("Checking to see if packages have shared (.so/.dll) libraries...")
+            if package_utils.detect_and_log_shared_libraries(
+                download_result.downloaded_packages_details
+            ):
+                # TODO: yes/no/ask logic should be removed in 3.0
+                if not (
+                    allow_shared_libraries
+                    or resolve_allow_shared_libraries_yes_no_ask(
+                        deprecated_package_native_libraries
+                    )
+                ):
+                    raise ClickException(
+                        "Some packages contain shared (.so/.dll) libraries. "
+                        "Try again with --allow-shared-libraries."
+                    )
+            if download_result.anaconda_packages:
+                anaconda_packages.write_requirements_file_in_snowflake_format(  # type: ignore
+                    file_path=snowpark_paths.snowflake_requirements_file,
+                    requirements=download_result.anaconda_packages,
+                )
+
+        zip_dir(
+            source=snowpark_paths.source.path,
+            dest_zip=snowpark_paths.artifact_file.path,
+        )
+        if any(packages_dir.iterdir()):
+            # if any packages were generated, append them to the .zip
+            zip_dir(
+                source=packages_dir.path,
+                dest_zip=snowpark_paths.artifact_file.path,
+                mode="a",
+            )
+
+    log.info("Package now ready: %s", snowpark_paths.artifact_file.path)
+
+    return MessageResult(
+        f"Build done. Artifact path: {snowpark_paths.artifact_file.path}"
     )
-    return MessageResult(f"Build done. Artifact path: {artifact_file}")
 
 
 class _SnowparkObject(Enum):
     """This clas is used only for Snowpark execute where choice is limited."""
 
     PROCEDURE = str(ObjectType.PROCEDURE)
     FUNCTION = str(ObjectType.FUNCTION)
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional
+import re
+from typing import Dict, List, Optional, Set
 
-from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB, ObjectType
-from snowflake.cli.api.secure_path import SecurePath
+from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.api.project.schemas.snowpark.argument import Argument
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
-from snowflake.cli.plugins.snowpark.package_utils import generate_deploy_stage_name
+from snowflake.cli.plugins.snowpark.models import Requirement
+from snowflake.cli.plugins.snowpark.package_utils import (
+    generate_deploy_stage_name,
+)
 from snowflake.connector.cursor import SnowflakeCursor
 
 DEFAULT_RUNTIME = "3.8"
 
 
 def check_if_replace_is_required(
     object_type: ObjectType,
     current_state,
     handler: str,
     return_type: str,
+    snowflake_dependencies: List[str],
+    imports: List[str],
+    stage_artifact_file: str,
 ) -> bool:
     import logging
 
     log = logging.getLogger(__name__)
     resource_json = _convert_resource_details_to_dict(current_state)
-    anaconda_packages = resource_json["packages"]
+    old_dependencies = resource_json["packages"]
     log.info(
-        "Found %s defined Anaconda packages in deployed %s...",
-        len(anaconda_packages),
+        "Found %d defined Anaconda packages in deployed %s...",
+        len(old_dependencies),
         object_type,
     )
     log.info("Checking if app configuration has changed...")
-    updated_package_list = _get_snowflake_packages_delta(
-        anaconda_packages,
-    )
 
-    if updated_package_list:
-        diff = len(updated_package_list) - len(anaconda_packages)
+    if _snowflake_dependencies_differ(old_dependencies, snowflake_dependencies):
         log.info(
-            "Found difference of %s packages. Replacing the %s.", diff, object_type
+            "Found difference of package requirements. Replacing the %s.", object_type
         )
         return True
 
     if (
         resource_json["handler"].lower() != handler.lower()
         or _sql_to_python_return_type_mapper(resource_json["returns"]).lower()
         != return_type.lower()
     ):
         log.info(
             "Return type or handler types do not match. Replacing the %s.", object_type
         )
         return True
 
+    if _compare_imports(resource_json, imports, stage_artifact_file):
+        return True
+
     return False
 
 
 def _convert_resource_details_to_dict(function_details: SnowflakeCursor) -> dict:
     import json
 
     function_dict = {}
@@ -63,29 +69,23 @@
                 function[1].replace("'", '"'),
             )
         else:
             function_dict[function[0]] = function[1]
     return function_dict
 
 
-def _get_snowflake_packages_delta(anaconda_packages) -> List[str]:
-    updated_package_list = []
-    requirements_file = SecurePath("requirements.snowflake.txt")
-    if requirements_file.exists():
-        with requirements_file.open(
-            "r", read_file_limit_mb=DEFAULT_SIZE_LIMIT_MB, encoding="utf-8"
-        ) as f:
-            # for each line, check if it exists in anaconda_packages. If it
-            # doesn't, add it to the return string
-            for line in f:
-                if line.strip() not in anaconda_packages:
-                    updated_package_list.append(line.strip())
-        return updated_package_list
-    else:
-        return updated_package_list
+def _snowflake_dependencies_differ(
+    old_dependencies: List[str], new_dependencies: List[str]
+) -> bool:
+    def _standardize(packages: List[str]) -> Set[str]:
+        return set(
+            Requirement.parse_line(package).name_and_version for package in packages
+        )
+
+    return _standardize(old_dependencies) != _standardize(new_dependencies)
 
 
 def _sql_to_python_return_type_mapper(resource_return_type: str) -> str:
     """
     Some of the Python data types get converted to SQL types, when function/procedure is created.
     So, to properly compare types, we use mapping based on:
     https://docs.snowflake.com/en/developer-guide/udf-stored-procedure-data-type-mapping#sql-python-data-type-mappings
@@ -169,30 +169,52 @@
 
 
 def _is_signature_type_a_string(sig_type: str) -> bool:
     return sig_type.lower() in ["string", "varchar"]
 
 
 def build_udf_sproc_identifier(
-    udf_sproc_dict,
+    udf_sproc,
     slq_exec_mixin,
     include_parameter_names,
     include_default_values=False,
 ):
-    def format_arg(arg):
-        result = f"{arg['type']}"
+    def format_arg(arg: Argument):
+        result = f"{arg.arg_type}"
         if include_parameter_names:
-            result = f"{arg['name']} {result}"
-        if include_default_values and "default" in arg:
-            val = f"{arg['default']}"
-            if _is_signature_type_a_string(arg["type"]):
+            result = f"{arg.name} {result}"
+        if include_default_values and arg.default:
+            val = f"{arg.default}"
+            if _is_signature_type_a_string(arg.arg_type):
                 val = f"'{val}'"
             result += f" default {val}"
         return result
 
-    arguments = ", ".join(format_arg(arg) for arg in udf_sproc_dict["signature"])
+    arguments = ", ".join(format_arg(arg) for arg in udf_sproc.signature)
     name = slq_exec_mixin.to_fully_qualified_name(
-        udf_sproc_dict["name"],
-        database=udf_sproc_dict.get("database"),
-        schema=udf_sproc_dict.get("schema"),
+        udf_sproc.name,
+        database=udf_sproc.database,
+        schema=udf_sproc.schema_name,
     )
     return f"{name}({arguments})"
+
+
+def _compare_imports(
+    resource_json: dict, imports: List[str], artifact_file: str
+) -> bool:
+    pattern = re.compile(r"(?:\[@?\w+_\w+\.)?(\w+(?:/\w+)+\.\w+)(?:\])?")
+
+    project_imports = {
+        imp
+        for import_string in [*imports, artifact_file]
+        for imp in pattern.findall(import_string.lower())
+    }
+
+    if "imports" not in resource_json.keys():
+        object_imports = set()
+    else:
+        object_imports = {
+            imp.lower()
+            for imp in pattern.findall(resource_json.get("imports", "").lower())
+        }
+
+    return project_imports != object_imports
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/snowpark/zipper.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/__init__.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/common.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,20 +62,24 @@
         raise ClickException(
             f"max_{instance_name} must be greater or equal to min_{instance_name}"
         )
     return max_instances
 
 
 def handle_object_already_exists(
-    error: ProgrammingError, object_type: ObjectType, object_name: str
+    error: ProgrammingError,
+    object_type: ObjectType,
+    object_name: str,
+    replace_available: bool = False,
 ):
     if error.errno == 2002:
         raise ObjectAlreadyExistsError(
             object_type=object_type,
             name=unquote_identifier(object_name),
+            replace_available=replace_available,
         )
     else:
         raise error
 
 
 class NoPropertiesProvidedError(ClickException):
     pass
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/compute_pool/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Optional
 
 import typer
 from click import ClickException
-from snowflake.cli.api.commands.flags import (
-    OverrideableOption,
-)
+from snowflake.cli.api.commands.flags import IfNotExistsOption, OverrideableOption
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.output.types import CommandResult, SingleQueryResult
 from snowflake.cli.api.project.util import is_valid_object_name
 from snowflake.cli.plugins.object.common import CommentOption
 from snowflake.cli.plugins.spcs.common import (
     validate_and_set_instances,
 )
@@ -86,14 +84,15 @@
     initially_suspended: bool = typer.Option(
         False,
         "--init-suspend/--no-init-suspend",
         help="Starts the compute pool in a suspended state.",
     ),
     auto_suspend_secs: int = AutoSuspendSecsOption(),
     comment: Optional[str] = CommentOption(help=_COMMENT_HELP),
+    if_not_exists: bool = IfNotExistsOption(),
     **options,
 ) -> CommandResult:
     """
     Creates a new compute pool.
     """
     max_nodes = validate_and_set_instances(min_nodes, max_nodes, "nodes")
     cursor = ComputePoolManager().create(
@@ -101,14 +100,15 @@
         min_nodes=min_nodes,
         max_nodes=max_nodes,
         instance_family=instance_family,
         auto_resume=auto_resume,
         initially_suspended=initially_suspended,
         auto_suspend_secs=auto_suspend_secs,
         comment=comment,
+        if_not_exists=if_not_exists,
     )
     return SingleQueryResult(cursor)
 
 
 @app.command("stop-all", requires_connection=True)
 def stop_all(name: str = ComputePoolNameArgument, **options) -> CommandResult:
     """
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/compute_pool/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,21 @@
         min_nodes: int,
         max_nodes: int,
         instance_family: str,
         auto_resume: bool,
         initially_suspended: bool,
         auto_suspend_secs: int,
         comment: Optional[str],
+        if_not_exists: bool,
     ) -> SnowflakeCursor:
+        create_statement = "CREATE COMPUTE POOL"
+        if if_not_exists:
+            create_statement = f"{create_statement} IF NOT EXISTS"
         query = f"""\
-            CREATE COMPUTE POOL {pool_name}
+            {create_statement} {pool_name}
             MIN_NODES = {min_nodes}
             MAX_NODES = {max_nodes}
             INSTANCE_FAMILY = {instance_family}
             AUTO_RESUME = {auto_resume}
             INITIALLY_SUSPENDED = {initially_suspended}
             AUTO_SUSPEND_SECS = {auto_suspend_secs}
             """.splitlines()
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_registry/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_registry/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,10 +78,12 @@
             "login",
             "--username",
             "0sessiontoken",
             "--password-stdin",
             registry_url,
         ]
         try:
-            return subprocess.check_output(command, input=json.dumps(token), text=True)
+            return subprocess.check_output(
+                command, input=json.dumps(token), text=True, stderr=subprocess.PIPE
+            )
         except subprocess.CalledProcessError as e:
             raise ClickException(f"Login Failed: {e.stderr}".strip())
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_repository/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import Optional
 
 import requests
 import typer
 from click import ClickException
+from snowflake.cli.api.commands.flags import IfNotExistsOption, ReplaceOption
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.console import cli_console
 from snowflake.cli.api.output.types import (
     CollectionResult,
     MessageResult,
     SingleQueryResult,
 )
@@ -19,15 +20,15 @@
     name="image-repository",
     help="Manages Snowpark Container Services image repositories.",
     short_help="Manages image repositories.",
 )
 
 
 def _repo_name_callback(name: str):
-    if not is_valid_object_name(name, max_depth=0, allow_quoted=True):
+    if not is_valid_object_name(name, max_depth=2, allow_quoted=False):
         raise ClickException(
             f"'{name}' is not a valid image repository name. Note that image repository names must be unquoted identifiers. The same constraint also applies to database and schema names where you create an image repository."
         )
     return name
 
 
 REPO_NAME_ARGUMENT = typer.Argument(
@@ -35,20 +36,26 @@
     callback=_repo_name_callback,
 )
 
 
 @app.command(requires_connection=True)
 def create(
     name: str = REPO_NAME_ARGUMENT,
+    replace: bool = ReplaceOption(),
+    if_not_exists: bool = IfNotExistsOption(),
     **options,
 ):
     """
     Creates a new image repository in the current schema.
     """
-    return SingleQueryResult(ImageRepositoryManager().create(name=name))
+    return SingleQueryResult(
+        ImageRepositoryManager().create(
+            name=name, replace=replace, if_not_exists=if_not_exists
+        )
+    )
 
 
 @app.command("list-images", requires_connection=True)
 def list_images(
     name: str = REPO_NAME_ARGUMENT,
     **options,
 ) -> CollectionResult:
@@ -91,14 +98,15 @@
 
 
 @app.command("list-tags", requires_connection=True)
 def list_tags(
     name: str = REPO_NAME_ARGUMENT,
     image_name: str = typer.Option(
         ...,
+        "--image-name",
         "--image_name",
         "-i",
         help="Fully qualified name of the image as shown in the output of list-images",
     ),
     **options,
 ) -> CollectionResult:
     """Lists tags for the given image in a repository."""
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/image_repository/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from urllib.parse import urlparse
 
-from click import ClickException
 from snowflake.cli.api.constants import ObjectType
-from snowflake.cli.api.project.util import (
-    is_valid_unquoted_identifier,
-)
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.spcs.common import handle_object_already_exists
 from snowflake.connector.errors import ProgrammingError
 
 
 class ImageRepositoryManager(SqlExecutionMixin):
     def get_database(self):
@@ -17,25 +13,21 @@
     def get_schema(self):
         return self._conn.schema
 
     def get_role(self):
         return self._conn.role
 
     def get_repository_url(self, repo_name: str, with_scheme: bool = True):
-        if not is_valid_unquoted_identifier(repo_name):
-            raise ValueError(
-                f"repo_name '{repo_name}' is not a valid unquoted Snowflake identifier"
-            )
-        # we explicitly do not allow this function to be used without connection database and schema set
+
         repo_row = self.show_specific_object(
             "image repositories", repo_name, check_schema=True
         )
         if repo_row is None:
-            raise ClickException(
-                f"Image repository '{repo_name}' does not exist in database '{self.get_database()}' and schema '{self.get_schema()}' or not authorized."
+            raise ProgrammingError(
+                f"Image repository '{self.to_fully_qualified_name(repo_name)}' does not exist or not authorized."
             )
         if with_scheme:
             return f"https://{repo_row['repository_url']}"
         else:
             return repo_row["repository_url"]
 
     def get_repository_api_url(self, repo_url):
@@ -47,12 +39,30 @@
 
         scheme = parsed_url.scheme
         host = parsed_url.netloc
         path = parsed_url.path
 
         return f"{scheme}://{host}/v2{path}"
 
-    def create(self, name: str):
+    def create(
+        self,
+        name: str,
+        if_not_exists: bool,
+        replace: bool,
+    ):
+        if if_not_exists and replace:
+            raise ValueError(
+                "'replace' and 'if_not_exists' options are mutually exclusive for ImageRepositoryManager.create"
+            )
+        elif replace:
+            create_statement = "create or replace image repository"
+        elif if_not_exists:
+            create_statement = "create image repository if not exists"
+        else:
+            create_statement = "create image repository"
+
         try:
-            return self._execute_schema_query(f"create image repository {name}")
+            return self._execute_schema_query(f"{create_statement} {name}", name=name)
         except ProgrammingError as e:
-            handle_object_already_exists(e, ObjectType.IMAGE_REPOSITORY, name)
+            handle_object_already_exists(
+                e, ObjectType.IMAGE_REPOSITORY, name, replace_available=True
+            )
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/jobs/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/jobs/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/services/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import sys
 from pathlib import Path
 from typing import List, Optional
 
 import typer
 from click import ClickException
-from snowflake.cli.api.commands.flags import (
-    OverrideableOption,
-)
+from snowflake.cli.api.commands.flags import IfNotExistsOption, OverrideableOption
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.output.types import (
     CommandResult,
     QueryJsonValueResult,
     QueryResult,
     SingleQueryResult,
 )
@@ -91,14 +89,15 @@
         None,
         "--eai-name",
         help="Identifies External Access Integrations(EAI) that the service can access. This option may be specified multiple times for multiple EAIs.",
     ),
     query_warehouse: Optional[str] = QueryWarehouseOption(),
     tags: Optional[List[Tag]] = TagOption(help="Tag for the service."),
     comment: Optional[str] = CommentOption(help=_COMMENT_HELP),
+    if_not_exists: bool = IfNotExistsOption(),
     **options,
 ) -> CommandResult:
     """
     Creates a new service in the current schema.
     """
     max_instances = validate_and_set_instances(
         min_instances, max_instances, "instances"
@@ -110,14 +109,15 @@
         compute_pool=compute_pool,
         spec_path=spec_path,
         external_access_integrations=external_access_integrations,
         auto_resume=auto_resume,
         query_warehouse=query_warehouse,
         tags=tags,
         comment=comment,
+        if_not_exists=if_not_exists,
     )
     return SingleQueryResult(cursor)
 
 
 @app.command(requires_connection=True)
 def status(name: str = ServiceNameArgument, **options) -> CommandResult:
     """
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/spcs/services/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
 from pathlib import Path
 from typing import List, Optional
 
+import yaml
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB, ObjectType
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.object.common import Tag
 from snowflake.cli.plugins.spcs.common import (
     NoPropertiesProvidedError,
     handle_object_already_exists,
@@ -23,19 +25,22 @@
         min_instances: int,
         max_instances: int,
         auto_resume: bool,
         external_access_integrations: Optional[List[str]],
         query_warehouse: Optional[str],
         tags: Optional[List[Tag]],
         comment: Optional[str],
+        if_not_exists: bool,
     ) -> SnowflakeCursor:
         spec = self._read_yaml(spec_path)
-
+        create_statement = "CREATE SERVICE"
+        if if_not_exists:
+            create_statement = f"{create_statement} IF NOT EXISTS"
         query = f"""\
-            CREATE SERVICE {service_name}
+            {create_statement} {service_name}
             IN COMPUTE POOL {compute_pool}
             FROM SPECIFICATION $$
             {spec}
             $$
             MIN_INSTANCES = {min_instances}
             MAX_INSTANCES = {max_instances}
             AUTO_RESUME = {auto_resume}
@@ -62,18 +67,14 @@
         try:
             return self._execute_query(strip_empty_lines(query))
         except ProgrammingError as e:
             handle_object_already_exists(e, ObjectType.SERVICE, service_name)
 
     def _read_yaml(self, path: Path) -> str:
         # TODO(aivanou): Add validation towards schema
-        import json
-
-        import yaml
-
         with SecurePath(path).open("r", read_file_limit_mb=DEFAULT_SIZE_LIMIT_MB) as fh:
             data = yaml.safe_load(fh)
         return json.dumps(data)
 
     def status(self, service_name: str) -> SnowflakeCursor:
         return self._execute_query(f"CALL SYSTEM$GET_SERVICE_STATUS('{service_name}')")
 
@@ -116,15 +117,15 @@
         ]
 
         # Check if all provided properties are set to None (no properties are being set)
         if all([value is None for property_name, value in property_pairs]):
             raise NoPropertiesProvidedError(
                 f"No properties specified for service '{service_name}'. Please provide at least one property to set."
             )
-        query: list[str] = [f"alter service {service_name} set"]
+        query: List[str] = [f"alter service {service_name} set"]
         for property_name, value in property_pairs:
             if value is not None:
                 query.append(f"{property_name} = {value}")
         return self._execute_query(strip_empty_lines(query))
 
     def unset_property(
         self,
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ),
     std_in: Optional[bool] = typer.Option(
         False,
         "--stdin",
         "-i",
         help="Read the query from standard input. Use it when piping input to this command.",
     ),
-    **options
+    **options,
 ) -> CommandResult:
     """
     Executes Snowflake query.
 
     Query to execute can be specified using query option, filename option (all queries from file will be executed)
     or via stdin by piping output from other command. For example `cat my.sql | snow sql -i`.
     """
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/sql/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/commands.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 import logging
 from pathlib import Path
-from typing import Optional
 
 import click
 import typer
 from click import ClickException
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_experimental_behaviour,
     with_project_definition,
 )
+from snowflake.cli.api.commands.flags import ReplaceOption
 from snowflake.cli.api.commands.project_initialisation import add_init_command
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.output.types import (
     CommandResult,
     MessageResult,
     SingleQueryResult,
 )
+from snowflake.cli.api.project.schemas.streamlit.streamlit import Streamlit
 from snowflake.cli.plugins.streamlit.manager import StreamlitManager
 
 app = SnowTyper(
     name="streamlit",
-    help="Manages Streamlit in Snowflake.",
+    help="Manages a Streamlit app in Snowflake.",
 )
 log = logging.getLogger(__name__)
 
 
 StageNameOption: str = typer.Option(
     "streamlit",
     "--stage",
-    help="Stage name where Streamlit files will be uploaded.",
+    help="Name of the stage where you want to upload Streamlit app files.",
+)
+
+OpenOption = typer.Option(
+    False,
+    "--open",
+    help="Whether to open the Streamlit app in a browser.",
+    is_flag=True,
 )
 
 
-add_init_command(app, project_type="Streamlit", template="default_streamlit")
+add_init_command(
+    app,
+    project_type="Streamlit",
+    template="default_streamlit",
+    help_message="Name of the Streamlit app project directory you want to create. Defaults to `example_streamlit`.",
+)
 
 
 @app.command("share", requires_connection=True)
 def streamlit_share(
-    name: str = typer.Argument(..., help="Name of streamlit to share."),
+    name: str = typer.Argument(..., help="Name of the Streamlit app to share."),
     to_role: str = typer.Argument(
-        ..., help="Role that streamlit should be shared with."
+        ..., help="Role with which to share the Streamlit app."
     ),
     **options,
 ) -> CommandResult:
     """
     Shares a Streamlit app with another role.
     """
     cursor = StreamlitManager().share(streamlit_name=name, to_role=to_role)
@@ -66,70 +79,63 @@
     return _check_file_exists_if_not_default
 
 
 @app.command("deploy", requires_connection=True)
 @with_project_definition("streamlit")
 @with_experimental_behaviour()
 def streamlit_deploy(
-    replace: Optional[bool] = typer.Option(
-        False,
-        "--replace",
-        help="Replace the Streamlit if it already exists.",
-        is_flag=True,
-    ),
-    open_: bool = typer.Option(
-        False, "--open", help="Whether to open Streamlit in a browser.", is_flag=True
+    replace: bool = ReplaceOption(
+        help="Replace the Streamlit app if it already exists."
     ),
+    open_: bool = OpenOption,
     **options,
 ) -> CommandResult:
     """
-    Deploys a Streamlit dashboard defined in project definition file (snowflake.yml). By default, the command will
-    upload environment.yml and pages/ folder if present. If stage name is not specified then 'streamlit' stage
-    will be used. If stage does not exist it will be created by this command.
+    Deploys a Streamlit app defined in the project definition file (snowflake.yml). By default, the command uploads
+    environment.yml and any other pages or folders, if present. If you don’t specify a stage name, the `streamlit`
+    stage is used. If the specified stage does not exist, the command creates it.
     """
-    streamlit = cli_context.project_definition
+    streamlit: Streamlit = cli_context.project_definition
     if not streamlit:
         return MessageResult("No streamlit were specified in project definition.")
 
-    environment_file = streamlit.get("env_file", None)
+    environment_file = streamlit.env_file
     if environment_file and not Path(environment_file).exists():
         raise ClickException(f"Provided file {environment_file} does not exist")
     elif environment_file is None:
         environment_file = "environment.yml"
 
-    pages_dir = streamlit.get("pages_dir", None)
+    pages_dir = streamlit.pages_dir
     if pages_dir and not Path(pages_dir).exists():
         raise ClickException(f"Provided file {pages_dir} does not exist")
     elif pages_dir is None:
         pages_dir = "pages"
 
     url = StreamlitManager().deploy(
-        streamlit_name=streamlit["name"],
+        streamlit_name=streamlit.name,
         environment_file=Path(environment_file),
         pages_dir=Path(pages_dir),
-        stage_name=streamlit["stage"],
-        main_file=Path(streamlit["main_file"]),
+        stage_name=streamlit.stage,
+        main_file=Path(streamlit.main_file),
         replace=replace,
-        query_warehouse=streamlit["query_warehouse"],
-        additional_source_files=streamlit.get("additional_source_files"),
+        query_warehouse=streamlit.query_warehouse,
+        additional_source_files=streamlit.additional_source_files,
         **options,
     )
 
     if open_:
         typer.launch(url)
 
     return MessageResult(f"Streamlit successfully deployed and available under {url}")
 
 
 @app.command("get-url", requires_connection=True)
 def get_url(
     name: str = typer.Argument(..., help="Name of the Streamlit app."),
-    open_: bool = typer.Option(
-        False, "--open", help="Whether to open Streamlit in a browser.", is_flag=True
-    ),
+    open_: bool = OpenOption,
     **options,
 ):
-    """Returns url to provided streamlit app"""
+    """Returns a URL to the specified Streamlit app"""
     url = StreamlitManager().get_url(streamlit_name=name)
     if open_:
         typer.launch(url)
     return MessageResult(url)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/plugins/streamlit/manager.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import logging
 from pathlib import Path
 from typing import List, Optional
 
 from snowflake.cli.api.commands.experimental_behaviour import (
     experimental_behaviour_enabled,
 )
+from snowflake.cli.api.feature_flags import FeatureFlag
 from snowflake.cli.api.project.util import unquote_identifier
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import (
     MissingConnectionHostError,
     make_snowsight_url,
 )
-from snowflake.cli.plugins.object.stage.manager import StageManager
+from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
 
 log = logging.getLogger(__name__)
 
 
 class StreamlitManager(SqlExecutionMixin):
@@ -53,32 +54,32 @@
                     if "/" in file
                     else root_location
                 )
                 stage_manager.put(file, destination, 4, True)
 
     def _create_streamlit(
         self,
-        streamlit_name: str,
+        fully_qualified_name: str,
         main_file: Path,
         replace: Optional[bool] = None,
         experimental: Optional[bool] = None,
         query_warehouse: Optional[str] = None,
         from_stage_name: Optional[str] = None,
     ):
         query = []
         if replace:
-            query.append(f"CREATE OR REPLACE STREAMLIT {streamlit_name}")
+            query.append(f"CREATE OR REPLACE STREAMLIT {fully_qualified_name}")
         elif experimental:
             # For experimental behaviour, we need to use CREATE STREAMLIT IF NOT EXISTS
             # for a streamlit app with an embedded stage
             # because this is analogous to the behavior for non-experimental
             # deploy which does CREATE STAGE IF NOT EXISTS
-            query.append(f"CREATE STREAMLIT IF NOT EXISTS {streamlit_name}")
+            query.append(f"CREATE STREAMLIT IF NOT EXISTS {fully_qualified_name}")
         else:
-            query.append(f"CREATE STREAMLIT {streamlit_name}")
+            query.append(f"CREATE STREAMLIT {fully_qualified_name}")
 
         if from_stage_name:
             query.append(f"ROOT_LOCATION = '{from_stage_name}'")
 
         query.append(f"MAIN_FILE = '{main_file.name}'")
 
         if query_warehouse:
@@ -95,32 +96,42 @@
         stage_name: Optional[str] = None,
         query_warehouse: Optional[str] = None,
         replace: Optional[bool] = False,
         additional_source_files: Optional[List[str]] = None,
         **options,
     ):
         stage_manager = StageManager()
-        if experimental_behaviour_enabled():
+        # for backwards compatibility - quoted stage path might be case-sensitive
+        # https://docs.snowflake.com/en/sql-reference/identifiers-syntax#double-quoted-identifiers
+        streamlit_name_for_root_location = self.get_name_from_fully_qualified_name(
+            streamlit_name
+        )
+        fully_qualified_name = stage_manager.to_fully_qualified_name(streamlit_name)
+        streamlit_name = self.get_name_from_fully_qualified_name(fully_qualified_name)
+        if (
+            experimental_behaviour_enabled()
+            or FeatureFlag.ENABLE_STREAMLIT_EMBEDDED_STAGE.is_enabled()
+        ):
             """
             1. Create streamlit object
             2. Upload files to embedded stage
             """
             # TODO: Support from_stage
             # from_stage_stmt = f"FROM_STAGE = '{stage_name}'" if stage_name else ""
             self._create_streamlit(
-                streamlit_name,
+                fully_qualified_name,
                 main_file,
                 replace=replace,
                 query_warehouse=query_warehouse,
                 experimental=True,
             )
             try:
-                self._execute_query(f"ALTER streamlit {streamlit_name} CHECKOUT")
+                self._execute_query(f"ALTER streamlit {fully_qualified_name} CHECKOUT")
             except ProgrammingError as e:
-                # If an error is raised because a CHECKOUT has already occured,
+                # If an error is raised because a CHECKOUT has already occurred,
                 # simply skip it and continue
                 if "Checkout already exists" in str(e):
                     log.info("Checkout already exists, continuing")
                 else:
                     raise
             stage_path = stage_manager.to_fully_qualified_name(streamlit_name)
             embedded_stage_name = f"snow://streamlit/{stage_path}"
@@ -142,48 +153,44 @@
             stage_manager = StageManager()
 
             stage_name = stage_name or "streamlit"
             stage_name = stage_manager.to_fully_qualified_name(stage_name)
 
             stage_manager.create(stage_name=stage_name)
 
-            root_location = stage_manager.get_standard_stage_name(
-                f"{stage_name}/{streamlit_name}"
+            root_location = stage_manager.get_standard_stage_prefix(
+                f"{stage_name}/{streamlit_name_for_root_location}"
             )
 
             self._put_streamlit_files(
                 root_location,
                 main_file,
                 environment_file,
                 pages_dir,
                 additional_source_files,
             )
 
             self._create_streamlit(
-                streamlit_name,
+                fully_qualified_name,
                 main_file,
                 replace=replace,
                 query_warehouse=query_warehouse,
                 from_stage_name=root_location,
                 experimental=False,
             )
 
-        return self.get_url(streamlit_name)
+        return self.get_url(fully_qualified_name)
 
-    def get_url(self, streamlit_name: str) -> str:
+    def get_url(self, streamlit_name: str, database=None, schema=None) -> str:
         try:
             return make_snowsight_url(
                 self._conn,
-                f"/#/streamlit-apps/{self.qualified_name_for_url(streamlit_name)}",
+                f"/#/streamlit-apps/{self.qualified_name_for_url(streamlit_name, database=database, schema=schema)}",
             )
         except MissingConnectionHostError as e:
             return "https://app.snowflake.com"
 
-    def qualified_name(self, object_name: str):
-        return f"{self._conn.database}.{self._conn.schema}.{object_name}"
-
-    def qualified_name_for_url(self, object_name: str):
-        return (
-            f"{unquote_identifier(self._conn.database)}."
-            f"{unquote_identifier(self._conn.schema)}."
-            f"{unquote_identifier(object_name)}"
+    def qualified_name_for_url(self, object_name: str, database=None, schema=None):
+        fqn = self.to_fully_qualified_name(
+            object_name, database=database, schema=schema
         )
+        return ".".join(unquote_identifier(part) for part in fqn.split("."))
```

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/src/snowflake/cli/templates/default_snowpark/app/procedures.py` & `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py` & `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import pytest
 from snowflake.cli.api.cli_global_context import cli_context_manager
 from snowflake.cli.api.commands.decorators import global_options, with_output
 from snowflake.cli.api.config import config_init
 from snowflake.cli.api.console import cli_console
 from snowflake.cli.api.output.types import QueryResult
 from snowflake.cli.app import loggers
-from snowflake.cli.app.cli_app import app
-
 
 pytest_plugins = ["tests.testing_utils.fixtures", "tests.project.fixtures"]
 
 
 @pytest.fixture(autouse=True)
 # Global context and logging levels reset is required.
 # Without it, state from previous tests is visible in following tests.
@@ -69,15 +67,17 @@
             ("string", 42, ["array"], {"k": "object"}, datetime(2022, 3, 21)),
             ("string", 43, ["array"], {"k": "object"}, datetime(2022, 3, 21)),
         ],
     )
 
 
 @pytest.fixture(name="faker_app")
-def make_faker_app(_create_mock_cursor):
+def make_faker_app(runner, _create_mock_cursor):
+    app = runner.app
+
     @app.command("Faker")
     @with_output
     @global_options
     def faker_app(**options):
         """Faker app"""
         with cli_console.phase("Enter", "Exit") as step:
             step("Faker. Teeny Tiny step: UNO UNO")
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_cli.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-from tests.testing_utils.fixtures import *
+from __future__ import annotations
 
+import pytest
+from snowflake.cli.api.cli_global_context import cli_context
 
-def test_global(runner):
-    result = runner.invoke(["-h"])
 
-    assert result.exit_code == 0
+@pytest.mark.parametrize(
+    "command, expected_value",
+    (
+        pytest.param(("sql",), False, id="silent is False"),
+        pytest.param(("sql", "--silent"), True, id="silent is True"),
+    ),
+)
+def test_silent_in_global_context(
+    command: tuple[str, ...],
+    expected_value: bool,
+    runner,
+):
+    runner.invoke(command)
 
-    assert "Snowflake CLI tool for developers" in result.output
+    assert cli_context.silent is expected_value
 
 
-@pytest.mark.parametrize(
-    "namespace, expected",
-    [
-        ("object", "Manages Snowflake objects"),
-        ("snowpark", "Manages procedures and functions."),
-        ("streamlit", " Manages Streamlit in Snowflake."),
-    ],
-)
-def test_namespace(namespace, expected, runner):
-    result = runner.invoke([namespace, "-h"])
+def test_silent_output_help(runner):
+    result = runner.invoke(["streamlit", "get-url", "--help"], catch_exceptions=False)
+
+    assert result.exit_code == 0, result.output
+    expected_message = "Turns off intermediate output to console"
+    assert expected_message in result.output, result.output
+
 
-    assert result.exit_code == 0
+def test_proper_context_values_for_silent(runner):
+    result = runner.invoke(["streamlit", "get-url", "--silent", "--help"])
+    assert runner.app is not None
+    assert runner.app
 
-    assert expected in result.output
+    assert result.exit_code == 0, result.output
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_command_registration.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
+from unittest import mock
+
 from snowflake.cli.api.plugins.command import (
     SNOWCLI_ROOT_COMMAND_PATH,
     CommandPath,
     CommandSpec,
     CommandType,
 )
 from snowflake.cli.plugins.connection import plugin_spec as connection_plugin_spec
 from snowflake.cli.plugins.streamlit import plugin_spec as streamlit_plugin_spec
 from typer import Typer
 
-from tests.testing_utils.fixtures import *
-
 
 def test_builtin_plugins_registration(runner):
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("Manages connections to Snowflake") == 1
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
     assert result.output.count("Executes Snowflake query") == 1
 
 
 def test_multiple_use_of_test_runner(runner):
     def assert_result_is_correct(result):
         assert result.exit_code == 0
         assert result.output.count("Manages connections to Snowflake") == 1
-        assert result.output.count("Manages Streamlit in Snowflake") == 1
+        assert result.output.count("Manages a Streamlit app in Snowflake") == 1
         assert result.output.count("Manages Snowflake objects") == 1
         assert result.output.count("Executes Snowflake query") == 1
 
     assert_result_is_correct(runner.invoke(["-h"]))
     assert_result_is_correct(runner.invoke(["-h"]))
 
 
@@ -71,15 +71,15 @@
         parent_command_path=SNOWCLI_ROOT_COMMAND_PATH,
         command_type=CommandType.SINGLE_COMMAND,
         typer_instance=typer_instance,
     )
 
     result = runner.invoke(["-h"])
     assert result.output.count("Manages connections to Snowflake") == 0
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch("snowflake.cli.plugins.connection.plugin_spec.command_spec")
 def test_exception_handling_if_single_command_has_multiple_commands(
     connection_command_spec_mock, runner
 ):
     typer_instance = Typer(name="connection", help="Manages connections to Snowflake")
@@ -89,20 +89,20 @@
         parent_command_path=SNOWCLI_ROOT_COMMAND_PATH,
         command_type=CommandType.SINGLE_COMMAND,
         typer_instance=typer_instance,
     )
 
     result = runner.invoke(["-h"])
     assert result.output.count("Manages connections to Snowflake") == 0
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch(
-    "snowflake.cli.app.commands_registration.command_plugins_loader.builtin_plugin_name_to_plugin_spec",
-    {
+    "snowflake.cli.app.commands_registration.command_plugins_loader.get_builtin_plugin_name_to_plugin_spec",
+    lambda: {
         "connection": connection_plugin_spec,
         "connection2": connection_plugin_spec,
     },
 )
 def test_duplicated_plugin_handling(runner):
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
@@ -115,15 +115,15 @@
     connection_command_spec_mock, runner
 ):
     connection_command_spec_mock.return_value = streamlit_plugin_spec.command_spec()
 
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("Manages connections to Snowflake") == 0
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch("snowflake.cli.plugins.streamlit.plugin_spec.command_spec")
 def test_conflicting_commands_handling(streamlit_command_spec_mock, runner):
     streamlit_command_spec_mock.return_value = CommandSpec(
         parent_command_path=CommandPath(["connection"]),
         command_type=CommandType.COMMAND_GROUP,
@@ -151,37 +151,37 @@
         typer_instance=Typer(name="list", callback=lambda: None),
     )
 
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("xyz123") == 0
     assert result.output.count("Manages connections to Snowflake") == 0
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch("snowflake.cli.plugins.connection.plugin_spec.command_spec")
 def test_broken_command_spec_handling(connection_command_spec_mock, runner):
     connection_command_spec_mock.side_effect = RuntimeError("Test exception")
 
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("Manages connections to Snowflake") == 0
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch(
     "snowflake.cli.app.api_impl.plugin.plugin_config_provider_impl.PluginConfigProviderImpl.get_enabled_plugin_names"
 )
 def test_not_existing_external_entrypoint_handling(enabled_plugin_names_mock, runner):
     enabled_plugin_names_mock.return_value = ["xyz123"]
 
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("Manages connections to Snowflake") == 1
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
 
 
 @mock.patch("pluggy.PluginManager.load_setuptools_entrypoints")
 @mock.patch(
     "snowflake.cli.app.api_impl.plugin.plugin_config_provider_impl.PluginConfigProviderImpl.get_enabled_plugin_names"
 )
 def test_broken_external_entrypoint_handling(
@@ -189,8 +189,8 @@
 ):
     enabled_plugin_names_mock.return_value = ["xyz123"]
     load_setuptools_entrypoints_mock.side_effect = RuntimeError("Test exception")
 
     result = runner.invoke(["-h"])
     assert result.exit_code == 0
     assert result.output.count("Manages connections to Snowflake") == 1
-    assert result.output.count("Manages Streamlit in Snowflake") == 1
+    assert result.output.count("Manages a Streamlit app in Snowflake") == 1
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_common_decorators.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 _KNOWN_SIG_GLOBAL_PARAMETERS_WITH_CONNECTION = [
     "connection",
     "account",
     "user",
     "password",
     "authenticator",
     "private_key_path",
+    "session_token",
+    "master_token",
     "database",
     "schema",
     "role",
     "warehouse",
     "temporary_connection",
     "mfa_passcode",
+    "enable_diag",
+    "diag_log_path",
+    "diag_allowlist_path",
     "format",
     "verbose",
     "debug",
     "silent",
 ]
 
 _KNOWN_SIG_GLOBAL_PARAMETERS = ["format", "verbose", "debug", "silent"]
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_common_global_context.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,34 +55,44 @@
     assert mock_connect.call_count == 2
 
     mock_connect.assert_has_calls(
         [
             call(
                 temporary_connection=False,
                 mfa_passcode=None,
+                enable_diag=False,
+                diag_log_path=None,
+                diag_allowlist_path=None,
                 connection_name=None,
                 account=None,
                 user=None,
                 password=None,
                 authenticator=None,
                 private_key_path=None,
+                session_token=None,
+                master_token=None,
                 database=None,
                 schema=None,
                 role="newValue",
                 warehouse="newValue2",
             ),
             call(
                 temporary_connection=False,
                 mfa_passcode=None,
+                enable_diag=False,
+                diag_log_path=None,
+                diag_allowlist_path=None,
                 connection_name=None,
                 account=None,
                 user="newValue3",
                 password=None,
                 authenticator=None,
                 private_key_path=None,
+                session_token=None,
+                master_token=None,
                 database=None,
                 schema=None,
                 role="newValue",
                 warehouse="newValue2",
             ),
         ]
     )
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     config_init,
     get_config_section,
     get_connection_dict,
     get_default_connection_dict,
 )
 from snowflake.cli.api.exceptions import MissingConfiguration
 
-from tests.testing_utils.fixtures import *
 from tests.testing_utils.files_and_dirs import assert_file_permissions_are_strict
 
 
 def test_empty_config_file_is_created_if_not_present():
     with TemporaryDirectory() as tmp_dir:
         config_file = Path(tmp_dir) / "sub" / "config.toml"
         assert config_file.exists() is False
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_connection.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,15 +157,17 @@
                 "account1",
             ],
         )
     assert result.exit_code == 1, result.output
     assert "Connection conn2 already exists  " in result.output
 
 
-def test_lists_connection_information(runner):
+@mock.patch("snowflake.cli.plugins.connection.commands.get_default_connection_name")
+def test_lists_connection_information(mock_get_default_conn_name, runner):
+    mock_get_default_conn_name.return_value = "empty"
     result = runner.invoke(["connection", "list", "--format", "json"])
     assert result.exit_code == 0, result.output
     payload = json.loads(result.output)
     assert payload == [
         {
             "connection_name": "full",
             "parameters": {
@@ -174,41 +176,51 @@
                 "host": "dev_host",
                 "port": 8000,
                 "role": "dev_role",
                 "schema": "dev_schema",
                 "user": "dev_user",
                 "warehouse": "dev_warehouse",
             },
+            "is_default": False,
         },
         {
             "connection_name": "default",
             "parameters": {
                 "database": "db_for_test",
                 "password": "****",  # masked
                 "role": "test_role",
                 "schema": "test_public",
                 "warehouse": "xs",
             },
+            "is_default": False,
+        },
+        {"connection_name": "empty", "parameters": {}, "is_default": True},
+        {
+            "connection_name": "test_connections",
+            "parameters": {"user": "python"},
+            "is_default": False,
         },
-        {"connection_name": "empty", "parameters": {}},
-        {"connection_name": "test_connections", "parameters": {"user": "python"}},
     ]
 
 
 @mock.patch.dict(
     os.environ,
     {
         # connection not existing in config.toml but with a name starting with connection from config.toml ("empty")
         "SNOWFLAKE_CONNECTIONS_EMPTYABC_PASSWORD": "abc123",
         # connection existing in config.toml but key not used by CLI
         "SNOWFLAKE_CONNECTIONS_EMPTY_PW": "abc123",
     },
     clear=True,
 )
-def test_connection_list_does_not_print_too_many_env_variables(runner):
+@mock.patch("snowflake.cli.plugins.connection.commands.get_default_connection_name")
+def test_connection_list_does_not_print_too_many_env_variables(
+    mock_get_default_conn_name, runner
+):
+    mock_get_default_conn_name.return_value = "empty"
     result = runner.invoke(["connection", "list", "--format", "json"])
     assert result.exit_code == 0, result.output
     payload = json.loads(result.output)
     assert payload == [
         {
             "connection_name": "full",
             "parameters": {
@@ -217,27 +229,33 @@
                 "host": "dev_host",
                 "port": 8000,
                 "role": "dev_role",
                 "schema": "dev_schema",
                 "user": "dev_user",
                 "warehouse": "dev_warehouse",
             },
+            "is_default": False,
         },
         {
             "connection_name": "default",
             "parameters": {
                 "database": "db_for_test",
                 "password": "****",  # masked
                 "role": "test_role",
                 "schema": "test_public",
                 "warehouse": "xs",
             },
+            "is_default": False,
+        },
+        {"connection_name": "empty", "parameters": {}, "is_default": True},
+        {
+            "connection_name": "test_connections",
+            "parameters": {"user": "python"},
+            "is_default": False,
         },
-        {"connection_name": "empty", "parameters": {}},
-        {"connection_name": "test_connections", "parameters": {"user": "python"}},
     ]
 
 
 def test_second_connection_not_update_default_connection(runner, snapshot):
     with NamedTemporaryFile("w+", suffix=".toml") as tmp_file:
         tmp_file.write(
             dedent(
@@ -273,41 +291,48 @@
         assert result.exit_code == 0, result.output
         assert content == snapshot
 
 
 @mock.patch("snowflake.cli.plugins.connection.commands.ObjectManager")
 @mock.patch("snowflake.cli.app.snow_connector.connect_to_snowflake")
 def test_connection_test(mock_connect, mock_om, runner):
-    result = runner.invoke(["connection", "test", "-c", "full"])
+    result = runner.invoke(
+        ["connection", "test", "-c", "full", "--diag-log-path", "/tmp"]
+    )
     assert result.exit_code == 0, result.output
     assert "Host" in result.output
     assert "Password" not in result.output
     assert "password" not in result.output
 
     mock_connect.assert_called_with(
         temporary_connection=False,
         mfa_passcode=None,
+        enable_diag=False,
+        diag_log_path="/tmp",
+        diag_allowlist_path=None,
         connection_name="full",
         account=None,
         user=None,
         password=None,
         authenticator=None,
         private_key_path=None,
+        session_token=None,
+        master_token=None,
         database=None,
         schema=None,
         role=None,
         warehouse=None,
     )
 
     conn = mock_connect.return_value
     assert mock_om.return_value.use.mock_calls == [
-        mock.call(object_type=ObjectType.ROLE, name=conn.role),
-        mock.call(object_type=ObjectType.DATABASE, name=conn.database),
-        mock.call(object_type=ObjectType.SCHEMA, name=conn.schema),
-        mock.call(object_type=ObjectType.WAREHOUSE, name=conn.warehouse),
+        mock.call(object_type=ObjectType.ROLE, name=f'"{conn.role}"'),
+        mock.call(object_type=ObjectType.DATABASE, name=f'"{conn.database}"'),
+        mock.call(object_type=ObjectType.SCHEMA, name=f'"{conn.schema}"'),
+        mock.call(object_type=ObjectType.WAREHOUSE, name=f'"{conn.warehouse}"'),
     ]
 
 
 @mock.patch("snowflake.connector.connect")
 @pytest.mark.parametrize("option", ["--temporary-connection", "-x"])
 def test_temporary_connection(mock_connector, mock_ctx, option, runner):
     ctx = mock_ctx()
@@ -420,14 +445,61 @@
         authenticator="SNOWFLAKE_JWT",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
     )
 
 
+@mock.patch("snowflake.connector.connect")
+def test_session_and_master_tokens(mock_connector, mock_ctx, runner):
+    ctx = mock_ctx()
+    mock_connector.return_value = ctx
+
+    session_token = "dummy-session-token"
+    master_token = "dummy-master-token"
+    result = runner.invoke(
+        [
+            "object",
+            "list",
+            "warehouse",
+            "--temporary-connection",
+            "--account",
+            "test_account",
+            "--user",
+            "snowcli_test",
+            "--authenticator",
+            "SNOWFLAKE_JWT",
+            "--session-token",
+            session_token,
+            "--master-token",
+            master_token,
+            "--warehouse",
+            "xsmall",
+            "--database",
+            "test_dv",
+            "--schema",
+            "PUBLIC",
+        ]
+    )
+
+    assert result.exit_code == 0
+    mock_connector.assert_called_once_with(
+        application="SNOWCLI.OBJECT.LIST",
+        session_token=session_token,
+        master_token=master_token,
+        account="test_account",
+        user="snowcli_test",
+        authenticator="SNOWFLAKE_JWT",
+        database="test_dv",
+        schema="PUBLIC",
+        warehouse="xsmall",
+        server_session_keep_alive=True,
+    )
+
+
 @mock.patch.dict(
     os.environ,
     {
         "PRIVATE_KEY_PASSPHRASE": "password",
     },
     clear=True,
 )
@@ -711,7 +783,38 @@
         tmp_file.flush()
 
         config = _change_connection(tmp_file, "conn1")
         assert config["default_connection_name"] == "conn1"
 
         config = _change_connection(tmp_file, "conn2")
         assert config["default_connection_name"] == "conn2"
+
+
+@mock.patch("snowflake.cli.plugins.connection.commands.ObjectManager")
+@mock.patch("snowflake.cli.app.snow_connector.connect_to_snowflake")
+def test_connection_test_diag_report(mock_connect, mock_om, runner):
+    result = runner.invoke(
+        ["connection", "test", "-c", "full", "--enable-diag", "--diag-log-path", "/tmp"]
+    )
+    assert result.exit_code == 0, result.output
+    print(result.output)
+    assert "Host" in result.output
+    assert "Diag Report" in result.output
+    mock_connect.assert_called_once_with(
+        temporary_connection=False,
+        mfa_passcode=None,
+        enable_diag=True,
+        diag_log_path="/tmp",
+        diag_allowlist_path=None,
+        connection_name="full",
+        account=None,
+        user=None,
+        password=None,
+        authenticator=None,
+        private_key_path=None,
+        session_token=None,
+        master_token=None,
+        database=None,
+        schema=None,
+        role=None,
+        warehouse=None,
+    )
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_experimental_behaviour.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from unittest import mock
 
 import typer
 from snowflake.cli.api.commands.decorators import (
     global_options,
     with_experimental_behaviour,
     with_output,
 )
@@ -13,16 +14,14 @@
 from snowflake.cli.api.plugins.command import (
     SNOWCLI_ROOT_COMMAND_PATH,
     CommandSpec,
     CommandType,
     plugin_hook_impl,
 )
 
-from tests.testing_utils.fixtures import *
-
 _test_experimental_typer = typer.Typer(name="test")
 
 
 @_test_experimental_typer.command("hello")
 @with_output
 @with_experimental_behaviour()
 @global_options
@@ -42,16 +41,16 @@
     )
 
 
 def _mock_test_plugin():
     from . import test_experimental_behaviour as plugin_spec
 
     return mock.patch(
-        "snowflake.cli.app.commands_registration.command_plugins_loader.builtin_plugin_name_to_plugin_spec",
-        {"test-plugin": plugin_spec},
+        "snowflake.cli.app.commands_registration.command_plugins_loader.get_builtin_plugin_name_to_plugin_spec",
+        lambda: {"test-plugin": plugin_spec},
     )
 
 
 @_mock_test_plugin()
 def test_experimental_invocation(runner):
     result_of_help = runner.invoke(["test", "hello", "--help"])
     assert "username" in result_of_help.output
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_help_messages.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+import pytest
 from snowflake.cli.app.commands_registration.command_plugins_loader import (
     load_only_builtin_command_plugins,
 )
-import pytest
 
 
 def iter_through_all_commands_paths():
     """
     Generator iterating through all commands.
     Paths are yielded as List[str]
     """
-    IGNORE_PLUGINS = ["render"]
+    ignore_plugins = ["render"]
 
     def _iter_through_commands(command, path):
         yield list(path)
         for subpath, subcommand in getattr(command, "commands", {}).items():
             path.append(subpath)
             yield from _iter_through_commands(subcommand, path)
             path.pop()
 
+    yield []  # "snow" with no commands
     builtin_plugins = load_only_builtin_command_plugins()
     for plugin in builtin_plugins:
         spec = plugin.command_spec
-        if not plugin.plugin_name in IGNORE_PLUGINS:
+        if not plugin.plugin_name in ignore_plugins:
             yield from _iter_through_commands(
                 spec.command, spec.full_command_path.path_segments
             )
 
 
 @pytest.mark.parametrize(
     "command",
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_logs.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import shutil
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Optional
 
 import pytest
-from snowflake.cli.app import loggers
 from snowflake.cli.api.config import config_init
 from snowflake.cli.api.exceptions import InvalidLogsConfiguration
+from snowflake.cli.app import loggers
 
 from tests.conftest import clean_logging_handlers
 from tests.testing_utils.files_and_dirs import assert_file_permissions_are_strict
 
 
 @pytest.fixture
 def setup_config_and_logs(snowflake_home):
@@ -33,17 +33,19 @@
             "\n".join(
                 x
                 for x in [
                     "[connections]",
                     "",
                     "[cli.logs]",
                     f'path = "{logs_path}"' if use_custom_logs_path else None,
-                    f"save_logs = {str(save_logs).lower()}"
-                    if save_logs is not None
-                    else None,
+                    (
+                        f"save_logs = {str(save_logs).lower()}"
+                        if save_logs is not None
+                        else None
+                    ),
                     f'level = "{level}"' if level else None,
                 ]
                 if x is not None
             )
         )
         config_path.chmod(0o700)
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_main.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """These tests verify that the CLI runs work as expected."""
+
 from __future__ import annotations
 
 import json
+import os
 import platform
 import sys
 import typing as t
+from pathlib import Path
+from unittest import mock
 
+import pytest
 from click import Command
 from snowflake.cli.__about__ import VERSION
 from snowflake.cli.app.cli_app import app_context_holder
 from snowflake.connector.config_manager import CONFIG_MANAGER
 from typer.core import TyperArgument, TyperOption
 
-from tests.testing_utils.fixtures import *
-
 
 def test_help_option(runner):
     result = runner.invoke(["--help"])
     assert result.exit_code == 0
 
 
 def test_streamlit_help(runner):
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_project_initialisation.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from unittest import mock
 
-from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.api.commands.project_initialisation import add_init_command
-from typer import Typer
-from typer.testing import CliRunner
-
 from snowflake.cli.api.commands.snow_typer import SnowTyper
+from snowflake.cli.api.secure_path import SecurePath
+from typer.testing import CliRunner
 
 
 @mock.patch.object(SecurePath, "copy")
 def test_adds_init_command(mock_copy):
     app = SnowTyper()
     runner = CliRunner()
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_render.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import json
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
-from tests.testing_utils.fixtures import *
-
 
 def test_render_template(runner):
     with NamedTemporaryFile("r") as tmp_file, NamedTemporaryFile("r") as json_file:
         Path(tmp_file.name).write_text(
             "This is my template {{ data.name }} and {{ toBeUpdated }}"
         )
         Path(json_file.name).write_text(
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_snow_connector.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from tests.testing_utils.fixtures import *
+import os
+from unittest import mock
+
+import pytest
 
 
 # Used as a solution to syrupy having some problems with comparing multilines string
 class CustomStr(str):
     def __repr__(self):
         return str(self)
 
@@ -23,16 +26,16 @@
     ],
 )
 @mock.patch("snowflake.connector.connect")
 @mock.patch("snowflake.cli.app.snow_connector.command_info")
 def test_command_context_is_passed_to_snowflake_connection(
     mock_command_info, mock_connect, cmd, expected, test_snowcli_config
 ):
-    from snowflake.cli.app.snow_connector import connect_to_snowflake
     from snowflake.cli.api.config import config_init
+    from snowflake.cli.app.snow_connector import connect_to_snowflake
 
     config_init(test_snowcli_config)
 
     mock_ctx = mock.Mock()
     mock_ctx.command_path = cmd
     mock_command_info.return_value = expected
 
@@ -64,7 +67,59 @@
         print(funny_text)
         return mock.MagicMock()
 
     mock_connect.connect = _mock
 
     result = runner.invoke(["sql", "-q", "select 1"])
     assert funny_text not in result.output
+
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_returns_nice_error_in_case_of_master_token_without_temporary_connection(
+    runner,
+):
+    result = runner.invoke(
+        ["sql", "-q", "select 1", "--master-token", "dummy-master-token"]
+    )
+    assert result.exit_code == 1
+    assert (
+        "When using a session or master token, you must use a temporary connection"
+        in result.output
+    )
+
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_returns_nice_error_in_case_of_session_token_without_temporary_connection(
+    runner,
+):
+    result = runner.invoke(
+        ["sql", "-q", "select 1", "--session-token", "dummy-session-token"]
+    )
+    assert result.exit_code == 1
+    assert (
+        "When using a session or master token, you must use a temporary connection"
+        in result.output
+    )
+
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_returns_nice_error_in_case_of_missing_session_token(runner):
+    result = runner.invoke(
+        ["sql", "-q", "select 1", "--master-token", "dummy-master-token", "-x"]
+    )
+    assert result.exit_code == 1
+    assert (
+        "When using a master token, you must provide the corresponding session token"
+        in result.output
+    )
+
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_returns_nice_error_in_case_of_missing_master_token(runner):
+    result = runner.invoke(
+        ["sql", "-q", "select 1", "--session-token", "dummy-session-token", "-x"]
+    )
+    assert result.exit_code == 1
+    assert (
+        "When using a session token, you must provide the corresponding master token"
+        in result.output
+    )
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_zipper.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import os
+from pathlib import Path
 from zipfile import ZipFile
 
 from snowflake.cli.plugins.snowpark.zipper import add_file_to_existing_zip, zip_dir
 
-from tests.testing_utils.fixtures import *
-
 
 def test_zip_current_dir(temp_dir):
     zip_name = Path("zip_name.zip")
     files = [
         Path(".DS_Store"),
         Path(".git/config"),
         Path(".gitignore"),
```

### Comparing `snowflake_cli_labs-2.1.2/tests/__snapshots__/test_connection.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/__snapshots__/test_help_messages.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,39 @@
 # serializer version: 1
+# name: test_help_messages[]
+  '''
+                                                                                  
+   Usage: default [OPTIONS] COMMAND [ARGS]...                                     
+                                                                                  
+   Snowflake CLI tool for developers.                                             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --version                    Shows version of the Snowflake CLI              │
+  │ --info                       Shows information about the Snowflake CLI       │
+  │ --config-file          FILE  Specifies Snowflake CLI configuration file that │
+  │                              should be used                                  │
+  │                              [default: None]                                 │
+  │ --help         -h            Show this message and exit.                     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ app          Manages a Snowflake Native App                                  │
+  │ connection   Manages connections to Snowflake.                               │
+  │ git          Manages git repositories in Snowflake.                          │
+  │ object       Manages Snowflake objects like warehouses and stages            │
+  │ snowpark     Manages procedures and functions.                               │
+  │ spcs         Manages Snowpark Container Services compute pools, services,    │
+  │              image registries, and image repositories.                       │
+  │ sql          Executes Snowflake query.                                       │
+  │ stage        Manages stages.                                                 │
+  │ streamlit    Manages a Streamlit app in Snowflake.                           │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[app.bundle]
   '''
                                                                                   
    Usage: default app bundle [OPTIONS]                                            
                                                                                   
    Prepares a local folder with configured app artifacts.                         
                                                                                   
@@ -21,14 +52,82 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[app.deploy]
+  '''
+                                                                                  
+   Usage: default app deploy [OPTIONS]                                            
+                                                                                  
+   Creates an application package in your Snowflake account and syncs the local   
+   changes to the stage without creating or updating the application.             
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --project  -p      TEXT  Path where the Snowflake Native App project         │
+  │                          resides. Defaults to current working directory.     │
+  │ --help     -h            Show this message and exit.                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[app.init]
   '''
                                                                                   
    Usage: default app init [OPTIONS] PATH                                         
                                                                                   
    Initializes a Snowflake Native App project.                                    
                                                                                   
@@ -82,14 +181,39 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[app.list-templates]
+  '''
+                                                                                  
+   Usage: default app list-templates [OPTIONS]                                    
+                                                                                  
+   Prints information regarding the official templates that can be used with snow 
+   app init.                                                                      
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[app.open]
   '''
                                                                                   
    Usage: default app open [OPTIONS]                                              
                                                                                   
    Opens the Snowflake Native App inside of your browser, once it has been        
    installed in your account.                                                     
@@ -130,14 +254,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -233,14 +362,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -301,14 +435,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -391,14 +530,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -470,14 +614,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -532,14 +681,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -558,21 +712,21 @@
                                                                                   
    Manages versions defined in an application package                             
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ create  Adds a new patch to the provided version defined in your application │
-  │         package. If the version does not exist, creates a version with patch │
-  │         0.                                                                   │
-  │ drop    Drops a version defined in your application package. Versions can    │
-  │         either be passed in as an argument to the command or read from the   │
-  │         `manifest.yml` file. Dropping patches is not allowed.                │
-  │ list    Lists all versions defined in an application package.                │
+  │ create   Adds a new patch to the provided version defined in your            │
+  │          application package. If the version does not exist, creates a       │
+  │          version with patch 0.                                               │
+  │ drop     Drops a version defined in your application package. Versions can   │
+  │          either be passed in as an argument to the command or read from the  │
+  │          `manifest.yml` file. Dropping patches is not allowed.               │
+  │ list     Lists all versions defined in an application package.               │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[app]
   '''
@@ -581,23 +735,26 @@
                                                                                   
    Manages a Snowflake Native App                                                 
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ init      Initializes a Snowflake Native App project.                        │
-  │ open      Opens the Snowflake Native App inside of your browser, once it has │
-  │           been installed in your account.                                    │
-  │ run       Creates an application package in your Snowflake account, uploads  │
-  │           code files to its stage, then creates or upgrades an application   │
-  │           object from the application package.                               │
-  │ teardown  Attempts to drop both the application object and application       │
-  │           package as defined in the project definition file.                 │
-  │ version   Manages versions defined in an application package                 │
+  │ deploy     Creates an application package in your Snowflake account and      │
+  │            syncs the local changes to the stage without creating or updating │
+  │            the application.                                                  │
+  │ init       Initializes a Snowflake Native App project.                       │
+  │ open       Opens the Snowflake Native App inside of your browser, once it    │
+  │            has been installed in your account.                               │
+  │ run        Creates an application package in your Snowflake account, uploads │
+  │            code files to its stage, then creates or upgrades an application  │
+  │            object from the application package.                              │
+  │ teardown   Attempts to drop both the application object and application      │
+  │            package as defined in the project definition file.                │
+  │ version    Manages versions defined in an application package                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[connection.add]
   '''
@@ -716,14 +873,19 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -742,32 +904,597 @@
                                                                                   
    Manages connections to Snowflake.                                              
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ add              Adds a connection to configuration file.                    │
-  │ list             Lists configured connections.                               │
-  │ set-default      Changes default connection to provided value.               │
-  │ test             Tests the connection to Snowflake.                          │
+  │ add           Adds a connection to configuration file.                       │
+  │ list          Lists configured connections.                                  │
+  │ set-default   Changes default connection to provided value.                  │
+  │ test          Tests the connection to Snowflake.                             │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.copy]
+  '''
+                                                                                  
+   Usage: default git copy [OPTIONS] REPOSITORY_PATH DESTINATION_PATH             
+                                                                                  
+   Copies all files from given state of repository to local directory or stage.   
+   If the source path ends with '/', the command copies contents of specified     
+   directory. Otherwise, it creates a new directory or file in the destination    
+   directory.                                                                     
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_path       TEXT  Path to git repository stage with scope     │
+  │                                  provided. Path to the repository root must  │
+  │                                  end with '/'. For example:                  │
+  │                                  @my_repo/branches/main/                     │
+  │                                  [default: None]                             │
+  │                                  [required]                                  │
+  │ *    destination_path      TEXT  Target path for copy operation. Should be a │
+  │                                  path to a directory on remote stage or      │
+  │                                  local file system.                          │
+  │                                  [default: None]                             │
+  │                                  [required]                                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --parallel          INTEGER  Number of parallel threads to use when          │
+  │                              downloading files.                              │
+  │                              [default: 4]                                    │
+  │ --help      -h               Show this message and exit.                     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.execute]
+  '''
+                                                                                  
+   Usage: default git execute [OPTIONS] REPOSITORY_PATH                           
+                                                                                  
+   Execute immediate all files from the repository path. Files can be filtered    
+   with glob like pattern, e.g. `@my_repo/branches/main/*.sql`,                   
+   `@my_repo/branches/main/dev/*`. Only files with `.sql` extension will be       
+   executed.                                                                      
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_path      TEXT  Path to git repository stage with scope      │
+  │                                 provided. Path to the repository root must   │
+  │                                 end with '/'. For example:                   │
+  │                                 @my_repo/branches/main/                      │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --on-error          [break|continue]  What to do when an error occurs.       │
+  │                                       Defaults to break.                     │
+  │                                       [default: break]                       │
+  │ --help      -h                        Show this message and exit.            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.fetch]
+  '''
+                                                                                  
+   Usage: default git fetch [OPTIONS] REPOSITORY_NAME                             
+                                                                                  
+   Fetch changes from origin to snowflake repository.                             
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_name      TEXT  Identifier of the git repository. For        │
+  │                                 example: my_repo                             │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.list-branches]
+  '''
+                                                                                  
+   Usage: default git list-branches [OPTIONS] REPOSITORY_NAME                     
+                                                                                  
+   List all branches in the repository.                                           
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_name      TEXT  Identifier of the git repository. For        │
+  │                                 example: my_repo                             │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT  SQL LIKE pattern for filtering objects by name. For    │
+  │                       example, `list-branches --like "%_test"` lists all     │
+  │                       branches that end with "_test".                        │
+  │                       [default: %%]                                          │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.list-files]
+  '''
+                                                                                  
+   Usage: default git list-files [OPTIONS] REPOSITORY_PATH                        
+                                                                                  
+   List files from given state of git repository.                                 
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_path      TEXT  Path to git repository stage with scope      │
+  │                                 provided. Path to the repository root must   │
+  │                                 end with '/'. For example:                   │
+  │                                 @my_repo/branches/main/                      │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --pattern          TEXT  Regex pattern for filtering files by name. For      │
+  │                          example --pattern ".*\.txt" will filter only files  │
+  │                          with .txt extension.                                │
+  │ --help     -h            Show this message and exit.                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.list-tags]
+  '''
+                                                                                  
+   Usage: default git list-tags [OPTIONS] REPOSITORY_NAME                         
+                                                                                  
+   List all tags in the repository.                                               
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_name      TEXT  Identifier of the git repository. For        │
+  │                                 example: my_repo                             │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --like  -l      TEXT  SQL LIKE pattern for filtering objects by name. For    │
+  │                       example, `list-tags --like "v2.0%"` lists all tags     │
+  │                       that start with "v2.0".                                │
+  │                       [default: %%]                                          │
+  │ --help  -h            Show this message and exit.                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git.setup]
+  '''
+                                                                                  
+   Usage: default git setup [OPTIONS] REPOSITORY_NAME                             
+                                                                                  
+   Sets up a git repository object.                                               
+   You will be prompted for:                                                      
+   * url - address of repository to be used for git clone operation               
+   * secret - Snowflake secret containing authentication credentials. Not needed  
+   if origin repository does not require authentication for RO operations (clone, 
+   fetch)                                                                         
+   * API integration - object allowing Snowflake to interact with git repository. 
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    repository_name      TEXT  Identifier of the git repository. For        │
+  │                                 example: my_repo                             │
+  │                                 [default: None]                              │
+  │                                 [required]                                   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[git]
+  '''
+                                                                                  
+   Usage: default git [OPTIONS] COMMAND [ARGS]...                                 
+                                                                                  
+   Manages git repositories in Snowflake.                                         
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ copy            Copies all files from given state of repository to local     │
+  │                 directory or stage.                                          │
+  │ execute         Execute immediate all files from the repository path. Files  │
+  │                 can be filtered with glob like pattern, e.g.                 │
+  │                 `@my_repo/branches/main/*.sql`,                              │
+  │                 `@my_repo/branches/main/dev/*`. Only files with `.sql`       │
+  │                 extension will be executed.                                  │
+  │ fetch           Fetch changes from origin to snowflake repository.           │
+  │ list-branches   List all branches in the repository.                         │
+  │ list-files      List files from given state of git repository.               │
+  │ list-tags       List all tags in the repository.                             │
+  │ setup           Sets up a git repository object.                             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.describe]
   '''
                                                                                   
    Usage: default object describe [OPTIONS] OBJECT_TYPE OBJECT_NAME               
                                                                                   
    Provides description of an object of given type.                               
-   Supported types: compute-pool, database, function, integration, network-rule,  
-   procedure, role, schema, secret, service, stage, stream, streamlit, table,     
-   task, user, view, warehouse                                                    
+   Supported types: compute-pool, database, function, git-repository,             
+   integration, network-rule, procedure, role, schema, secret, service, stage,    
+   stream, streamlit, table, task, user, view, warehouse                          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   │ *    object_name      TEXT  Name of the object [default: None] [required]    │
@@ -806,14 +1533,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -827,17 +1559,17 @@
 # ---
 # name: test_help_messages[object.drop]
   '''
                                                                                   
    Usage: default object drop [OPTIONS] OBJECT_TYPE OBJECT_NAME                   
                                                                                   
    Drops Snowflake object of given name and type.                                 
-   Supported types: compute-pool, database, function, image-repository,           
-   integration, network-rule, procedure, role, schema, secret, service, stage,    
-   stream, streamlit, table, task, user, view, warehouse                          
+   Supported types: compute-pool, database, function, git-repository,             
+   image-repository, integration, network-rule, procedure, role, schema, secret,  
+   service, stage, stream, streamlit, table, task, user, view, warehouse          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   │ *    object_name      TEXT  Name of the object [default: None] [required]    │
@@ -876,14 +1608,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -897,17 +1634,17 @@
 # ---
 # name: test_help_messages[object.list]
   '''
                                                                                   
    Usage: default object list [OPTIONS] OBJECT_TYPE                               
                                                                                   
    Lists all available Snowflake objects of given type.                           
-   Supported types: compute-pool, database, function, image-repository,           
-   integration, network-rule, procedure, role, schema, secret, service, stage,    
-   stream, streamlit, table, task, user, view, warehouse                          
+   Supported types: compute-pool, database, function, git-repository,             
+   image-repository, integration, network-rule, procedure, role, schema, secret,  
+   service, stage, stream, streamlit, table, task, user, view, warehouse          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    object_type      TEXT  Type of object. For example table, procedure,    │
   │                             streamlit.                                       │
   │                             [default: None]                                  │
   │                             [required]                                       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -956,14 +1693,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -973,17 +1715,20 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.stage.copy]
   '''
+  DeprecationWarning: The command 'stage' is deprecated.
+  `snow object stage` command group is deprecated. Please use `snow stage` instead.
                                                                                   
    Usage: default object stage copy [OPTIONS] SOURCE_PATH DESTINATION_PATH        
                                                                                   
+   (deprecated)                                                                   
    Copies all files from target path to target directory. This works for both     
    uploading to and downloading files from the stage.                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    source_path           TEXT  Source path for copy operation. Can be      │
   │                                  either stage path or local.                 │
   │                                  [default: None]                             │
@@ -997,14 +1742,17 @@
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --overwrite      --no-overwrite             Overwrites existing files in the │
   │                                             target path.                     │
   │                                             [default: no-overwrite]          │
   │ --parallel                         INTEGER  Number of parallel threads to    │
   │                                             use when uploading files.        │
   │                                             [default: 4]                     │
+  │ --recursive      --no-recursive             Copy files recursively with      │
+  │                                             directory structure.             │
+  │                                             [default: no-recursive]          │
   │ --help       -h                             Show this message and exit.      │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -1034,14 +1782,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1051,21 +1804,24 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.stage.create]
   '''
+  DeprecationWarning: The command 'stage' is deprecated.
+  `snow object stage` command group is deprecated. Please use `snow stage` instead.
                                                                                   
    Usage: default object stage create [OPTIONS] STAGE_NAME                        
                                                                                   
+   (deprecated)                                                                   
    Creates a named stage if it does not already exist.                            
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    stage_name      TEXT  Name of the stage. [default: None] [required]     │
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -1097,14 +1853,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1114,17 +1875,20 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.stage.diff]
   '''
+  DeprecationWarning: The command 'stage' is deprecated.
+  `snow object stage` command group is deprecated. Please use `snow stage` instead.
                                                                                   
    Usage: default object stage diff [OPTIONS] [STAGE_NAME] [FOLDER_NAME]          
                                                                                   
+   (deprecated)                                                                   
    Diffs a stage with a local folder.                                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │   stage_name       [STAGE_NAME]   Fully qualified name of a stage            │
   │                                   [default: None]                            │
   │   folder_name      [FOLDER_NAME]  Path to local folder [default: None]       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -1162,14 +1926,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1179,24 +1948,30 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.stage.list]
   '''
+  DeprecationWarning: The command 'stage' is deprecated.
+  `snow object stage` command group is deprecated. Please use `snow stage` instead.
                                                                                   
    Usage: default object stage list [OPTIONS] STAGE_NAME                          
                                                                                   
+   (deprecated)                                                                   
    Lists the stage contents.                                                      
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    stage_name      TEXT  Name of the stage. [default: None] [required]     │
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --help  -h        Show this message and exit.                                │
+  │ --pattern          TEXT  Regex pattern for filtering files by name. For      │
+  │                          example --pattern ".*\.txt" will filter only files  │
+  │                          with .txt extension.                                │
+  │ --help     -h            Show this message and exit.                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -1225,14 +2000,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1242,21 +2022,24 @@
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object.stage.remove]
   '''
+  DeprecationWarning: The command 'stage' is deprecated.
+  `snow object stage` command group is deprecated. Please use `snow stage` instead.
                                                                                   
    Usage: default object stage remove [OPTIONS] STAGE_NAME FILE_NAME              
                                                                                   
+   (deprecated)                                                                   
    Removes a file from a stage.                                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    stage_name      TEXT  Name of the stage. [default: None] [required]     │
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
   │ *    file_name       TEXT  Name of the file to remove. [default: None]       │
   │                            [required]                                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
@@ -1290,14 +2073,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1310,25 +2098,27 @@
   '''
 # ---
 # name: test_help_messages[object.stage]
   '''
                                                                                   
    Usage: default object stage [OPTIONS] COMMAND [ARGS]...                        
                                                                                   
+   (deprecated)                                                                   
    Manages stages.                                                                
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ copy    Copies all files from target path to target directory. This works    │
-  │         for both uploading to and downloading files from the stage.          │
-  │ create  Creates a named stage if it does not already exist.                  │
-  │ list    Lists the stage contents.                                            │
-  │ remove  Removes a file from a stage.                                         │
+  │ copy     Copies all files from target path to target           (deprecated)  │
+  │          directory. This works for both uploading to and                     │
+  │          downloading files from the stage.                                   │
+  │ create   Creates a named stage if it does not already exist.   (deprecated)  │
+  │ list     Lists the stage contents.                             (deprecated)  │
+  │ remove   Removes a file from a stage.                          (deprecated)  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[object]
   '''
@@ -1337,18 +2127,19 @@
                                                                                   
    Manages Snowflake objects like warehouses and stages                           
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ describe     Provides description of an object of given type.                │
-  │ drop         Drops Snowflake object of given name and type.                  │
-  │ list         Lists all available Snowflake objects of given type.            │
-  │ stage        Manages stages.                                                 │
+  │ describe   Provides description of an object of given type.                  │
+  │ drop       Drops Snowflake object of given name and type.                    │
+  │ list       Lists all available Snowflake objects of given                    │
+  │            type.                                                             │
+  │ stage      Manages stages.                                     (deprecated)  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[snowpark.build]
   '''
@@ -1356,46 +2147,73 @@
    Usage: default snowpark build [OPTIONS]                                        
                                                                                   
    Builds the Snowpark project as a `.zip` archive that can be used by `deploy`   
    command. The archive is built using only the `src` directory specified in the  
    project file.                                                                  
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --pypi-download                              [yes|no|ask]  Whether to        │
-  │                                                            download          │
-  │                                                            non-Anaconda      │
-  │                                                            packages from     │
-  │                                                            PyPi.             │
-  │                                                            [default: ask]    │
-  │ --check-anaconda-…  -a  --no-check-anaco…                  Checks if any of  │
-  │                                                            missing Anaconda  │
-  │                                                            packages          │
-  │                                                            dependencies can  │
-  │                                                            be imported       │
-  │                                                            directly from     │
-  │                                                            Anaconda. Valid   │
-  │                                                            values include:   │
-  │                                                            `true`, `false`,  │
-  │                                                            Default: `true`.  │
-  │                                                            [default:         │
-  │                                                            check-anaconda-f… │
-  │ --package-native-…                           [yes|no|ask]  Allows native     │
-  │                                                            libraries, when   │
-  │                                                            using packages    │
-  │                                                            installed through │
-  │                                                            PIP               │
-  │                                                            [default: no]     │
-  │ --project           -p                       TEXT          Path where the    │
-  │                                                            Snowpark project  │
-  │                                                            resides. Defaults │
-  │                                                            to current        │
-  │                                                            working           │
-  │                                                            directory.        │
-  │ --help              -h                                     Show this message │
-  │                                                            and exit.         │
+  │ --ignore-anaconda                       Does not lookup packages on          │
+  │                                         Snowflake Anaconda channel.          │
+  │ --allow-shared-libraries                Allows shared (.so) libraries, when  │
+  │                                         using packages installed through     │
+  │                                         PIP.                                 │
+  │ --index-url                       TEXT  Base URL of the Python Package Index │
+  │                                         to use for package lookup. This      │
+  │                                         should point to  a repository        │
+  │                                         compliant with PEP 503 (the simple   │
+  │                                         repository API) or a local directory │
+  │                                         laid out in the same format.         │
+  │ --skip-version-check                    Skip comparing versions of           │
+  │                                         dependencies between requirements    │
+  │                                         and Anaconda.                        │
+  │ --project                 -p      TEXT  Path where the Snowpark project      │
+  │                                         resides. Defaults to current working │
+  │                                         directory.                           │
+  │ --help                    -h            Show this message and exit.          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1455,14 +2273,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1529,14 +2352,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1587,17 +2415,29 @@
    imported for a Snowpark Python app.                                            
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    name      TEXT  Name of the package to create. [default: None]          │
   │                      [required]                                              │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --pypi-download            Installs packages that are not available on the   │
-  │                            Snowflake Anaconda channel.                       │
-  │ --help           -h        Show this message and exit.                       │
+  │ --ignore-anaconda                       Does not lookup packages on          │
+  │                                         Snowflake Anaconda channel.          │
+  │ --index-url                       TEXT  Base URL of the Python Package Index │
+  │                                         to use for package lookup. This      │
+  │                                         should point to  a repository        │
+  │                                         compliant with PEP 503 (the simple   │
+  │                                         repository API) or a local directory │
+  │                                         laid out in the same format.         │
+  │ --skip-version-check                    Skip comparing versions of           │
+  │                                         dependencies between requirements    │
+  │                                         and Anaconda.                        │
+  │ --allow-shared-libraries                Allows shared (.so) libraries, when  │
+  │                                         using packages installed through     │
+  │                                         PIP.                                 │
+  │ --help                    -h            Show this message and exit.          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -1626,14 +2466,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1644,27 +2489,23 @@
   
   
   '''
 # ---
 # name: test_help_messages[snowpark.package.lookup]
   '''
                                                                                   
-   Usage: default snowpark package lookup [OPTIONS] NAME                          
+   Usage: default snowpark package lookup [OPTIONS] PACKAGE_NAME                  
                                                                                   
-   Checks if a package is available on the Snowflake Anaconda channel. If the     
-   `--pypi-download` flag is provided, this command checks all dependencies of    
-   the packages outside Snowflake channel.                                        
+   Checks if a package is available on the Snowflake Anaconda channel.            
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name      TEXT  Name of the package. [default: None] [required]         │
+  │ *    package_name      TEXT  Name of the package. [required]                 │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --pypi-download            Installs packages that are not available on the   │
-  │                            Snowflake Anaconda channel.                       │
-  │ --help           -h        Show this message and exit.                       │
+  │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -1693,14 +2534,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1761,14 +2607,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1787,21 +2638,19 @@
                                                                                   
    Manages custom Python packages for Snowpark                                    
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ create  Creates a Python package as a zip file that can be uploaded to a     │
-  │         stage and imported for a Snowpark Python app.                        │
-  │ lookup  Checks if a package is available on the Snowflake Anaconda channel.  │
-  │         If the `--pypi-download` flag is provided, this command checks all   │
-  │         dependencies of the packages outside Snowflake channel.              │
-  │ upload  Uploads a Python package zip file to a Snowflake stage so it can be  │
-  │         referenced in the imports of a procedure or function.                │
+  │ create   Creates a Python package as a zip file that can be uploaded to a    │
+  │          stage and imported for a Snowpark Python app.                       │
+  │ lookup   Checks if a package is available on the Snowflake Anaconda channel. │
+  │ upload   Uploads a Python package zip file to a Snowflake stage so it can be │
+  │          referenced in the imports of a procedure or function.               │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[snowpark]
   '''
@@ -1810,26 +2659,26 @@
                                                                                   
    Manages procedures and functions.                                              
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ build    Builds the Snowpark project as a `.zip` archive that can be used by │
-  │          `deploy` command. The archive is built using only the `src`         │
-  │          directory specified in the project file.                            │
-  │ deploy   Deploys procedures and functions defined in project. Deploying the  │
-  │          project alters all objects defined in it. By default, if any of the │
-  │          objects exist already the commands will fail unless `--replace`     │
-  │          flag is provided. All deployed objects use the same artifact which  │
-  │          is deployed only once.                                              │
-  │ execute  Executes a procedure or function in a specified environment.        │
-  │ init     Initializes this directory with a sample set of files for creating  │
-  │          a Snowpark project.                                                 │
-  │ package  Manages custom Python packages for Snowpark                         │
+  │ build     Builds the Snowpark project as a `.zip` archive that can be used   │
+  │           by `deploy` command. The archive is built using only the `src`     │
+  │           directory specified in the project file.                           │
+  │ deploy    Deploys procedures and functions defined in project. Deploying the │
+  │           project alters all objects defined in it. By default, if any of    │
+  │           the objects exist already the commands will fail unless            │
+  │           `--replace` flag is provided. All deployed objects use the same    │
+  │           artifact which is deployed only once.                              │
+  │ execute   Executes a procedure or function in a specified environment.       │
+  │ init      Initializes this directory with a sample set of files for creating │
+  │           a Snowpark project.                                                │
+  │ package   Manages custom Python packages for Snowpark                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs.compute-pool.create]
   '''
@@ -1884,14 +2733,19 @@
   │                                                             automatically    │
   │                                                             suspend the      │
   │                                                             compute pool.    │
   │                                                             [default: 3600]  │
   │    --comment                               TEXT             Comment for the  │
   │                                                             compute pool.    │
   │                                                             [default: None]  │
+  │    --if-not-exists                                          Only apply this  │
+  │                                                             operation if the │
+  │                                                             specified object │
+  │                                                             does not already │
+  │                                                             exist.           │
   │    --help           -h                                      Show this        │
   │                                                             message and      │
   │                                                             exit.            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -1923,14 +2777,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -1986,14 +2845,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2074,14 +2938,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2138,14 +3007,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2201,14 +3075,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2265,14 +3144,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2337,14 +3221,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2363,24 +3252,24 @@
                                                                                   
    Manages Snowpark Container Services compute pools.                             
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ create    Creates a new compute pool.                                        │
-  │ resume    Resumes the compute pool from a SUSPENDED state.                   │
-  │ set       Sets one or more properties for the compute pool.                  │
-  │ status    Retrieves the status of a compute pool along with a relevant       │
-  │           message, if one exists.                                            │
-  │ stop-all  Deletes all services running on the compute pool.                  │
-  │ suspend   Suspends the compute pool by suspending all currently running      │
-  │           services and then releasing compute pool nodes.                    │
-  │ unset     Resets one or more properties for the compute pool to their        │
-  │           default value(s).                                                  │
+  │ create     Creates a new compute pool.                                       │
+  │ resume     Resumes the compute pool from a SUSPENDED state.                  │
+  │ set        Sets one or more properties for the compute pool.                 │
+  │ status     Retrieves the status of a compute pool along with a relevant      │
+  │            message, if one exists.                                           │
+  │ stop-all   Deletes all services running on the compute pool.                 │
+  │ suspend    Suspends the compute pool by suspending all currently running     │
+  │            services and then releasing compute pool nodes.                   │
+  │ unset      Resets one or more properties for the compute pool to their       │
+  │            default value(s).                                                 │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs.image-registry.login]
   '''
@@ -2426,14 +3315,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2488,14 +3382,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2557,14 +3456,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2583,19 +3487,19 @@
                                                                                   
    Manages Snowpark Container Services image registries.                          
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ login  Logs in to the account image registry with the current user's         │
-  │        credentials through Docker.                                           │
-  │ token  Retrieves a registry authentication token based on your current       │
-  │        connection.                                                           │
-  │ url    Gets the image registry URL for the current account.                  │
+  │ login   Logs in to the account image registry with the current user's        │
+  │         credentials through Docker.                                          │
+  │ token   Retrieves a registry authentication token based on your current      │
+  │         connection.                                                          │
+  │ url     Gets the image registry URL for the current account.                 │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs.image-repository.create]
   '''
@@ -2605,15 +3509,18 @@
    Creates a new image repository in the current schema.                          
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    name      TEXT  Name of the image repository. [default: None]           │
   │                      [required]                                              │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --help  -h        Show this message and exit.                                │
+  │ --replace                  Replace this object if it already exists.         │
+  │ --if-not-exists            Only apply this operation if the specified object │
+  │                            does not already exist.                           │
+  │ --help           -h        Show this message and exit.                       │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -2642,14 +3549,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2706,14 +3618,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2733,19 +3650,20 @@
    Lists tags for the given image in a repository.                                
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    name      TEXT  Name of the image repository. [default: None]           │
   │                      [required]                                              │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ *  --image_name  -i      TEXT  Fully qualified name of the image as shown in │
-  │                                the output of list-images                     │
-  │                                [default: None]                               │
-  │                                [required]                                    │
-  │    --help        -h            Show this message and exit.                   │
+  │ *  --image-name,--image_name  -i      TEXT  Fully qualified name of the      │
+  │                                             image as shown in the output of  │
+  │                                             list-images                      │
+  │                                             [default: None]                  │
+  │                                             [required]                       │
+  │    --help                     -h            Show this message and exit.      │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -2774,14 +3692,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2838,14 +3761,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2864,18 +3792,18 @@
                                                                                   
    Manages Snowpark Container Services image repositories.                        
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ create         Creates a new image repository in the current schema.         │
-  │ list-images    Lists images in the given repository.                         │
-  │ list-tags      Lists tags for the given image in a repository.               │
-  │ url            Returns the URL for the given repository.                     │
+  │ create        Creates a new image repository in the current schema.          │
+  │ list-images   Lists images in the given repository.                          │
+  │ list-tags     Lists tags for the given image in a repository.                │
+  │ url           Returns the URL for the given repository.                      │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs.job.create]
   '''
@@ -2925,14 +3853,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -2990,14 +3923,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3053,14 +3991,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3155,14 +4098,19 @@
   │                                                             [default: None]  │
   │    --tag                                   NAME=VALUE       Tag for the      │
   │                                                             service.         │
   │                                                             [default: None]  │
   │    --comment                               TEXT             Comment for the  │
   │                                                             service.         │
   │                                                             [default: None]  │
+  │    --if-not-exists                                          Only apply this  │
+  │                                                             operation if the │
+  │                                                             specified object │
+  │                                                             does not already │
+  │                                                             exist.           │
   │    --help           -h                                      Show this        │
   │                                                             message and      │
   │                                                             exit.            │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
@@ -3194,14 +4142,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3257,14 +4210,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3328,14 +4286,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3391,14 +4354,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3483,14 +4451,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3546,14 +4519,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3609,14 +4587,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3685,14 +4668,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3751,14 +4739,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3777,25 +4770,25 @@
                                                                                   
    Manages Snowpark Container Services services.                                  
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ create          Creates a new service in the current schema.                 │
-  │ list-endpoints  Lists the endpoints in a service.                            │
-  │ logs            Retrieves local logs from a service container.               │
-  │ resume          Resumes the service from a SUSPENDED state.                  │
-  │ set             Sets one or more properties for the service.                 │
-  │ status          Retrieves the status of a service.                           │
-  │ suspend         Suspends the service, shutting down and deleting all its     │
-  │                 containers.                                                  │
-  │ unset           Resets one or more properties for the service to their       │
-  │                 default value(s).                                            │
-  │ upgrade         Updates an existing service with a new specification file.   │
+  │ create           Creates a new service in the current schema.                │
+  │ list-endpoints   Lists the endpoints in a service.                           │
+  │ logs             Retrieves local logs from a service container.              │
+  │ resume           Resumes the service from a SUSPENDED state.                 │
+  │ set              Sets one or more properties for the service.                │
+  │ status           Retrieves the status of a service.                          │
+  │ suspend          Suspends the service, shutting down and deleting all its    │
+  │                  containers.                                                 │
+  │ unset            Resets one or more properties for the service to their      │
+  │                  default value(s).                                           │
+  │ upgrade          Updates an existing service with a new specification file.  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[spcs]
   '''
@@ -3805,18 +4798,18 @@
    Manages Snowpark Container Services compute pools, services, image registries, 
    and image repositories.                                                        
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ compute-pool                  Manages compute pools.                         │
-  │ image-registry                Manages image registries.                      │
-  │ image-repository              Manages image repositories.                    │
-  │ service                       Manages services.                              │
+  │ compute-pool       Manages compute pools.                                    │
+  │ image-registry     Manages image registries.                                 │
+  │ image-repository   Manages image repositories.                               │
+  │ service            Manages services.                                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_help_messages[sql]
   '''
@@ -3866,14 +4859,316 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.copy]
+  '''
+                                                                                  
+   Usage: default stage copy [OPTIONS] SOURCE_PATH DESTINATION_PATH               
+                                                                                  
+   Copies all files from target path to target directory. This works for both     
+   uploading to and downloading files from the stage.                             
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    source_path           TEXT  Source path for copy operation. Can be      │
+  │                                  either stage path or local.                 │
+  │                                  [required]                                  │
+  │ *    destination_path      TEXT  Target directory path for copy operation.   │
+  │                                  Should be stage if source is local or local │
+  │                                  if source is stage.                         │
+  │                                  [required]                                  │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --overwrite      --no-overwrite             Overwrites existing files in the │
+  │                                             target path.                     │
+  │                                             [default: no-overwrite]          │
+  │ --parallel                         INTEGER  Number of parallel threads to    │
+  │                                             use when uploading files.        │
+  │                                             [default: 4]                     │
+  │ --recursive      --no-recursive             Copy files recursively with      │
+  │                                             directory structure.             │
+  │                                             [default: no-recursive]          │
+  │ --help       -h                             Show this message and exit.      │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.create]
+  '''
+                                                                                  
+   Usage: default stage create [OPTIONS] STAGE_NAME                               
+                                                                                  
+   Creates a named stage if it does not already exist.                            
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.diff]
+  '''
+                                                                                  
+   Usage: default stage diff [OPTIONS] [STAGE_NAME] [FOLDER_NAME]                 
+                                                                                  
+   Diffs a stage with a local folder.                                             
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   stage_name       [STAGE_NAME]   Fully qualified name of a stage            │
+  │                                   [default: None]                            │
+  │   folder_name      [FOLDER_NAME]  Path to local folder [default: None]       │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.execute]
+  '''
+                                                                                  
+   Usage: default stage execute [OPTIONS] STAGE_PATH                              
+                                                                                  
+   Execute immediate all files from the stage path. Files can be filtered with    
+   glob like pattern, e.g. `@stage/*.sql`, `@stage/dev/*`. Only files with `.sql` 
+   extension will be executed.                                                    
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    stage_path      TEXT  Stage path with files to be execute. For example  │
+  │                            `@stage/dev/*`.                                   │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --on-error          [break|continue]  What to do when an error occurs.       │
+  │                                       Defaults to break.                     │
+  │                                       [default: break]                       │
+  │ --help      -h                        Show this message and exit.            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3881,30 +5176,197 @@
   │                                  information.                                │
   │ --silent                         Turns off intermediate output to console.   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[stage.list-files]
+  '''
+                                                                                  
+   Usage: default stage list-files [OPTIONS] STAGE_NAME                           
+                                                                                  
+   Lists the stage contents.                                                      
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --pattern          TEXT  Regex pattern for filtering files by name. For      │
+  │                          example --pattern ".*\.txt" will filter only files  │
+  │                          with .txt extension.                                │
+  │ --help     -h            Show this message and exit.                         │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage.remove]
+  '''
+                                                                                  
+   Usage: default stage remove [OPTIONS] STAGE_NAME FILE_NAME                     
+                                                                                  
+   Removes a file from a stage.                                                   
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    stage_name      TEXT  Name of the stage. [required]                     │
+  │ *    file_name       TEXT  Name of the file to remove. [default: None]       │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[stage]
+  '''
+                                                                                  
+   Usage: default stage [OPTIONS] COMMAND [ARGS]...                               
+                                                                                  
+   Manages stages.                                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ copy         Copies all files from target path to target directory. This     │
+  │              works for both uploading to and downloading files from the      │
+  │              stage.                                                          │
+  │ create       Creates a named stage if it does not already exist.             │
+  │ execute      Execute immediate all files from the stage path. Files can be   │
+  │              filtered with glob like pattern, e.g. `@stage/*.sql`,           │
+  │              `@stage/dev/*`. Only files with `.sql` extension will be        │
+  │              executed.                                                       │
+  │ list-files   Lists the stage contents.                                       │
+  │ remove       Removes a file from a stage.                                    │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[streamlit.deploy]
   '''
                                                                                   
    Usage: default streamlit deploy [OPTIONS]                                      
                                                                                   
-   Deploys a Streamlit dashboard defined in project definition file               
-   (snowflake.yml). By default, the command will upload environment.yml and       
-   pages/ folder if present. If stage name is not specified then 'streamlit'      
-   stage will be used. If stage does not exist it will be created by this         
-   command.                                                                       
+   Deploys a Streamlit app defined in the project definition file                 
+   (snowflake.yml). By default, the command uploads environment.yml and any other 
+   pages or folders, if present. If you don’t specify a stage name, the           
+   `streamlit` stage is used. If the specified stage does not exist, the command  
+   creates it.                                                                    
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --replace                Replace the Streamlit if it already exists.         │
-  │ --open                   Whether to open Streamlit in a browser.             │
-  │ --project  -p      TEXT  Path where the Streamlit project resides. Defaults  │
-  │                          to current working directory.                       │
+  │ --replace                Replace the Streamlit app if it already exists.     │
+  │ --open                   Whether to open the Streamlit app in a browser.     │
+  │ --project  -p      TEXT  Path where the Streamlit app project resides.       │
+  │                          Defaults to current working directory.              │
   │ --help     -h            Show this message and exit.                         │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -3934,14 +5396,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -3954,21 +5421,21 @@
   '''
 # ---
 # name: test_help_messages[streamlit.get-url]
   '''
                                                                                   
    Usage: default streamlit get-url [OPTIONS] NAME                                
                                                                                   
-   Returns url to provided streamlit app                                          
+   Returns a URL to the specified Streamlit app                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    name      TEXT  Name of the Streamlit app. [default: None] [required]   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --open            Whether to open Streamlit in a browser.                    │
+  │ --open            Whether to open the Streamlit app in a browser.            │
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -3998,14 +5465,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -4019,19 +5491,20 @@
 # ---
 # name: test_help_messages[streamlit.init]
   '''
                                                                                   
    Usage: default streamlit init [OPTIONS] [PROJECT_NAME]                         
                                                                                   
    Initializes this directory with a sample set of files for creating a Streamlit 
-   project.                                                                       
+   app project.                                                                   
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │   project_name      [PROJECT_NAME]  Name of the Streamlit project you want   │
-  │                                     to create.                               │
+  │   project_name      [PROJECT_NAME]  Name of the Streamlit app project        │
+  │                                     directory you want to create. Defaults   │
+  │                                     to `example_streamlit`.                  │
   │                                     [default: example_streamlit]             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
@@ -4051,17 +5524,17 @@
   '''
                                                                                   
    Usage: default streamlit share [OPTIONS] NAME TO_ROLE                          
                                                                                   
    Shares a Streamlit app with another role.                                      
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │ *    name         TEXT  Name of streamlit to share. [default: None]          │
+  │ *    name         TEXT  Name of the Streamlit app to share. [default: None]  │
   │                         [required]                                           │
-  │ *    to_role      TEXT  Role that streamlit should be shared with.           │
+  │ *    to_role      TEXT  Role with which to share the Streamlit app.          │
   │                         [default: None]                                      │
   │                         [required]                                           │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
@@ -4095,14 +5568,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -4115,27 +5593,27 @@
   '''
 # ---
 # name: test_help_messages[streamlit]
   '''
                                                                                   
    Usage: default streamlit [OPTIONS] COMMAND [ARGS]...                           
                                                                                   
-   Manages Streamlit in Snowflake.                                                
+   Manages a Streamlit app in Snowflake.                                          
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ deploy   Deploys a Streamlit dashboard defined in project definition file    │
-  │          (snowflake.yml). By default, the command will upload                │
-  │          environment.yml and pages/ folder if present. If stage name is not  │
-  │          specified then 'streamlit' stage will be used. If stage does not    │
-  │          exist it will be created by this command.                           │
-  │ get-url  Returns url to provided streamlit app                               │
-  │ init     Initializes this directory with a sample set of files for creating  │
-  │          a Streamlit project.                                                │
-  │ share    Shares a Streamlit app with another role.                           │
+  │ deploy    Deploys a Streamlit app defined in the project definition file     │
+  │           (snowflake.yml). By default, the command uploads environment.yml   │
+  │           and any other pages or folders, if present. If you don’t specify a │
+  │           stage name, the `streamlit` stage is used. If the specified stage  │
+  │           does not exist, the command creates it.                            │
+  │ get-url   Returns a URL to the specified Streamlit app                       │
+  │ init      Initializes this directory with a sample set of files for creating │
+  │           a Streamlit app project.                                           │
+  │ share     Shares a Streamlit app with another role.                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
```

### Comparing `snowflake_cli_labs-2.1.2/tests/api/test_secure_path.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
+import re
+import shutil
 import stat
+from pathlib import Path
 
 import pytest
-
 from snowflake.cli.api import secure_path
-from snowflake.cli.api.exceptions import FileTooLargeError, DirectoryIsNotEmptyError
-from snowflake.cli.api.secure_path import SecurePath
-from pathlib import Path
 from snowflake.cli.api.config import config_init
+from snowflake.cli.api.exceptions import DirectoryIsNotEmptyError, FileTooLargeError
+from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.app import loggers
 
 from tests.testing_utils.files_and_dirs import assert_file_permissions_are_strict
 
-import shutil
-import re
-
 
 @pytest.fixture()
 def save_logs(snowflake_home):
     config = snowflake_home / "config.toml"
     logs_path = snowflake_home / "logs"
     config.write_text(
         "\n".join(["[cli.logs]", "save_logs = true", f'path = "{logs_path}"'])
@@ -208,20 +206,20 @@
 def test_move(temp_dir, save_logs):
     def _get_new_file():
         file = Path(temp_dir) / "file.txt"
         file.touch()
         return file
 
     def _get_new_dir():
-        dir = Path(temp_dir) / "dir"
-        (dir / "subdir").mkdir(parents=True)
-        (dir / "empty").mkdir()
-        (dir / "file1.txt").touch()
-        (dir / "subdir" / "file2.txt").touch()
-        return dir
+        dir_ = Path(temp_dir) / "dir"
+        (dir_ / "subdir").mkdir(parents=True)
+        (dir_ / "empty").mkdir()
+        (dir_ / "file1.txt").touch()
+        (dir_ / "subdir" / "file2.txt").touch()
+        return dir_
 
     def _check_dir_moved(dst):
         for filename in ["file1.txt", "empty", "subdir/file2.txt"]:
             path = Path(dst) / filename
             assert path.exists()
             if filename.endswith(".txt"):
                 assert path.is_file()
@@ -238,47 +236,47 @@
     )
 
     file = SecurePath(_get_new_file())
     with pytest.raises(FileExistsError):
         file.move("moved_file.txt")
     assert file.exists()
 
-    dir = _get_new_dir()
-    moved_file = file.move(dir)
+    dir_ = _get_new_dir()
+    moved_file = file.move(dir_)
     assert moved_file.exists() and not file.exists()
     assert moved_file.path.resolve() == (Path("dir") / "file.txt").resolve()
     _assert_count_matching_logs(
         save_logs, 1, "Moving", "file.txt", " to \S+dir[\/]file.txt"
     )
 
     file = SecurePath(_get_new_file())
     with pytest.raises(FileExistsError):
-        file.move(dir)
+        file.move(dir_)
     assert file.exists()
 
     # moving directory
-    dir = SecurePath(dir)
-    moved_dir = dir.move("moved_dir")
-    assert moved_dir.exists() and not dir.exists()
+    dir_ = SecurePath(dir_)
+    moved_dir = dir_.move("moved_dir")
+    assert moved_dir.exists() and not dir_.exists()
     assert moved_dir.path == Path("moved_dir")
     _check_dir_moved("moved_dir")
     _assert_count_matching_logs(save_logs, 1, "Moving", "dir", " to \S+moved_dir")
 
-    dir = SecurePath(_get_new_dir())
-    moved_dir = dir.move("moved_dir")
-    assert moved_dir.exists() and not dir.exists()
+    dir_ = SecurePath(_get_new_dir())
+    moved_dir = dir_.move("moved_dir")
+    assert moved_dir.exists() and not dir_.exists()
     assert moved_dir.path == Path("moved_dir") / "dir"
     _check_dir_moved(Path("moved_dir") / "dir")
     _assert_count_matching_logs(
         save_logs, 1, "Moving", "dir", " to \S+moved_dir[\/]dir"
     )
 
-    dir = SecurePath(_get_new_dir())
+    dir_ = SecurePath(_get_new_dir())
     with pytest.raises(FileExistsError):
-        dir.move("moved_dir")
+        dir_.move("moved_dir")
 
 
 def test_copy_file(temp_dir, save_logs):
     file = SecurePath(temp_dir) / "file.txt"
     file.touch()
     file.chmod(permissions_mask=0o660)
 
@@ -354,67 +352,67 @@
         assert_file_permissions_are_strict(path)
 
     _assert_count_matching_logs(save_logs, 10, "Copying file", ".txt")
     _assert_count_matching_logs(save_logs, 8, "Creating directory", "")
 
 
 def test_copy_dir_onto_existing_dir(temp_dir, save_logs):
-    DIR, FILE = "DIR", "FILE"
+    dir_, file = "DIR", "FILE"
     original = [
-        (DIR, "dir"),
-        (FILE, "dir/subfile"),
-        (DIR, "dir/subdir"),
-        (FILE, "dir/subdir/subfile"),
-        (DIR, "dir/newdir/"),
+        (dir_, "dir"),
+        (file, "dir/subfile"),
+        (dir_, "dir/subdir"),
+        (file, "dir/subdir/subfile"),
+        (dir_, "dir/newdir/"),
     ]
     file_instead_of_dir = [
-        (DIR, "dir"),
-        (FILE, "dir/subfile"),
-        (FILE, "dir/subdir"),
+        (dir_, "dir"),
+        (file, "dir/subfile"),
+        (file, "dir/subdir"),
     ]
     dir_instead_of_file = [
-        (DIR, "dir"),
-        (DIR, "dir/subfile"),
-        (DIR, "dir/subdir"),
-        (FILE, "dir/subdir/subfile"),
+        (dir_, "dir"),
+        (dir_, "dir/subfile"),
+        (dir_, "dir/subdir"),
+        (file, "dir/subdir/subfile"),
     ]
     proper_destination = [
-        (DIR, "dir"),
-        (FILE, "dir/subfile"),
-        (DIR, "dir/subdir"),
-        (FILE, "dir/subdir/subfile2"),
+        (dir_, "dir"),
+        (file, "dir/subfile"),
+        (dir_, "dir/subdir"),
+        (file, "dir/subdir/subfile2"),
     ]
     expected_result = [
-        (DIR, "dir"),
-        (FILE, "dir/subfile"),
-        (DIR, "dir/subdir"),
-        (FILE, "dir/subdir/subfile"),
-        (FILE, "dir/subdir/subfile2"),
-        (DIR, "dir/newdir/"),
+        (dir_, "dir"),
+        (file, "dir/subfile"),
+        (dir_, "dir/subdir"),
+        (file, "dir/subdir/subfile"),
+        (file, "dir/subdir/subfile2"),
+        (dir_, "dir/newdir/"),
     ]
     should_be_overridden = [("dir/subfile"), ("dir/subdir/subfile"), ("dir/newdir/")]
 
     def _check_result_tree(root):
         readable_by_group = stat.S_IRGRP
 
         for filetype, filename in expected_result:
             file = root / filename
             assert file.exists()
             if filename in should_be_overridden:
                 assert_file_permissions_are_strict(root / filename)
-                if filetype == FILE:
+                if filetype == file:
                     assert file.read_text() == "new"
             else:
                 assert file.stat().st_mode & readable_by_group == readable_by_group
-                if filetype == FILE:
+                if filetype == file:
                     assert file.read_text() == "old"
 
     def _create_tree(root, tree, file_content):
         for filetype, filename in tree:
-            if filetype == DIR:
+            if filetype == dir_:
                 (root / filename).mkdir(parents=True)
                 (root / filename).chmod(0o750)
             else:
                 (root / filename).write_text(file_content)
                 (root / filename).chmod(0o660)
 
     tmpdir = Path(temp_dir)
```

### Comparing `snowflake_cli_labs-2.1.2/tests/api/commands/test_snow_typer.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from functools import partial
 from unittest import mock
 from unittest.mock import MagicMock
 
 import pytest
 import typer
-
 from snowflake.cli.api.commands.snow_typer import SnowTyper
 from snowflake.cli.api.output.types import MessageResult
-
 from typer.testing import CliRunner
 
 
 def class_factory(
     pre_execute=None,
     result_handler=None,
     exception_handler=None,
@@ -37,14 +35,17 @@
         def exception_handler(err):
             if exception_handler:
                 exception_handler(err)
 
     return _CustomTyper
 
 
+_ENABLED_FLAG = False
+
+
 def app_factory(typer_cls):
     app = typer_cls(name="snow")
 
     @app.command("simple_cmd", requires_global_options=False, requires_connection=False)
     def simple_cmd(name: str = typer.Argument()):
         return MessageResult(f"hello {name}")
 
@@ -60,14 +61,18 @@
     def cmd_with_global_options(name: str = typer.Argument()):
         return MessageResult(f"hello {name}")
 
     @app.command("cmd_with_connection_options", requires_connection=True)
     def cmd_with_connection_options(name: str = typer.Argument()):
         return MessageResult(f"hello {name}")
 
+    @app.command("switchable_cmd", is_enabled=lambda: _ENABLED_FLAG)
+    def cmd_witch_enabled_switch():
+        return MessageResult("Enabled")
+
     return app
 
 
 @pytest.fixture
 def cli():
     def mock_cli(app):
         return partial(CliRunner().invoke, app)
@@ -145,14 +150,30 @@
 
 
 def test_command_with_connection_options(cli, snapshot):
     result = cli(app_factory(SnowTyper))(["cmd_with_connection_options", "--help"])
     assert result.output == snapshot
 
 
+def test_enabled_command_is_visible(cli, snapshot):
+    global _ENABLED_FLAG
+    _ENABLED_FLAG = True
+    result = cli(app_factory(SnowTyper))(["switchable_cmd", "--help"])
+    assert result.exit_code == 0
+    assert result.output == snapshot
+
+
+def test_enabled_command_is_not_visible(cli, snapshot):
+    global _ENABLED_FLAG
+    _ENABLED_FLAG = False
+    result = cli(app_factory(SnowTyper))(["switchable_cmd", "--help"])
+    assert result.exit_code == 2
+    assert result.output == snapshot
+
+
 @mock.patch("snowflake.cli.app.telemetry.log_command_usage")
 def test_snow_typer_pre_execute_sends_telemetry(mock_log_command_usage, cli):
     result = cli(app_factory(SnowTyper))(["simple_cmd", "Norma"])
     assert result.exit_code == 0
     mock_log_command_usage.assert_called_once_with()
```

### Comparing `snowflake_cli_labs-2.1.2/tests/api/commands/__snapshots__/test_snow_typer.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,19 @@
   │                                           value specified for the            │
   │                                           connection.                        │
   │ --temporary-connection      -x            Uses connection defined with       │
   │                                           command line parameters, instead   │
   │                                           of one defined in config           │
   │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
   │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Global configuration ───────────────────────────────────────────────────────╮
   │ --format           [TABLE|JSON]  Specifies the output format.                │
   │                                  [default: TABLE]                            │
   │ --verbose  -v                    Displays log entries for log levels `info`  │
   │                                  and higher.                                 │
   │ --debug                          Displays log entries for log levels `debug` │
@@ -96,7 +101,39 @@
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_enabled_command_is_not_visible
+  '''
+  Usage: snow [OPTIONS] COMMAND [ARGS]...
+  Try 'snow --help' for help.
+  ╭─ Error ──────────────────────────────────────────────────────────────────────╮
+  │ No such command 'switchable_cmd'.                                            │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  '''
+# ---
+# name: test_enabled_command_is_visible
+  '''
+                                                                                  
+   Usage: snow switchable_cmd [OPTIONS]                                           
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
```

### Comparing `snowflake_cli_labs-2.1.2/tests/api/console/test_cli_console_output.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/api/console/test_console_abc.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/api/console/test_intermediate_output.py` & `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/app/test_telemetry.py` & `snowflake_cli_labs-2.2.0rc0/tests/app/test_telemetry.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     mock_platform.return_value = "FancyOS"
     mock_version.return_value = "2.3.4"
 
     result = runner.invoke(["connection", "test"], catch_exceptions=False)
     assert result.exit_code == 0, result.output
 
     # The method is called with a TelemetryData type, so we cast it to dict for simpler comparison
-    assert mock_conn.return_value._telemetry.try_add_log_to_batch.call_args.args[
+    assert mock_conn.return_value._telemetry.try_add_log_to_batch.call_args.args[  # noqa: SLF001
         0
     ].to_dict() == {
         "message": {
             "driver_type": "PythonConnector",
             "driver_version": ".".join(str(s) for s in DRIVER_VERSION[:3]),
             "source": "snowcli",
             "version_cli": VERSION,
             "version_os": "FancyOS",
             "version_python": "2.3.4",
             "command": ["connection", "test"],
             "command_group": "connection",
-            "command_flags": {"format": "DEFAULT"},
+            "command_flags": {"diag_log_path": "DEFAULT", "format": "DEFAULT"},
             "command_output_type": "TABLE",
             "type": "executing_command",
         },
         "timestamp": "123",
     }
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/patch_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_artifacts.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from typing import Optional
-from unittest import mock
+from pathlib import Path
+from typing import List, Optional
 
 import pytest
+from snowflake.cli.api.project.definition import load_project_definition
 from snowflake.cli.plugins.nativeapp.artifacts import (
     ArtifactMapping,
     DeployRootError,
     GlobMatchedNothingError,
     NotInDeployRootError,
     SourceNotFoundError,
     TooManyFilesError,
     build_bundle,
     translate_artifact,
 )
-from snowflake.cli.api.project.definition import load_project_definition
-
-from tests.project.fixtures import *
-from tests.testing_utils.fixtures import *
 
 
 def trimmed_contents(path: Path) -> Optional[str]:
     if not path.is_file():
         return None
     with open(path, "r") as handle:
         return handle.read().strip()
@@ -38,18 +35,18 @@
 
     return parts
 
 
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
 def test_napp_project_1_artifacts(project_definition_files):
     project_root = project_definition_files[0].parent
-    native_app = load_project_definition(project_definition_files)["native_app"]
+    native_app = load_project_definition(project_definition_files).native_app
 
-    deploy_root = Path(project_root, native_app["deploy_root"])
-    artifacts = [translate_artifact(item) for item in native_app["artifacts"]]
+    deploy_root = Path(project_root, native_app.deploy_root)
+    artifacts = [translate_artifact(item) for item in native_app.artifacts]
     build_bundle(project_root, deploy_root, artifacts)
 
     assert dir_structure(deploy_root) == [
         "app/README.md",
         "setup.sql",
         "ui/config.py",
         "ui/main.py",
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_commands.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from unittest import mock
 
 import pytest
 
-from tests.testing_utils.fixtures import *
-
 PROJECT_PATH = "demo_na_project"
 
 
 @pytest.mark.parametrize(
-    "id,init_args",
+    "id_,init_args",
     [
         # with implicit name
         ["all_upper", ["DEMO_NA_PROJECT"]],
         ["snake_case", ["demo_na_project"]],
         ["camel_case", ["DemoNAProject"]],
         ["with_dashes", ["demo-na-project"]],
         ["with_spaces", ["demo na project"]],
@@ -62,26 +60,26 @@
         ],
     ],
 )
 @mock.patch(
     "snowflake.cli.plugins.nativeapp.init._init_from_template", return_value=None
 )
 def test_init_no_template_success(
-    mock_init_from_template, runner, temp_dir, snapshot, id, init_args
+    mock_init_from_template, runner, temp_dir, snapshot, id_, init_args
 ):
     args = ["app", "init"]
     args.extend(init_args)
     result = runner.invoke(args)
 
     assert result.exit_code == 0
     assert result.output == snapshot
 
 
 @pytest.mark.parametrize(
-    "id,init_args",
+    "id_,init_args",
     [
         # with implicit name
         ["with_unterminated_id", ['"demo_na_project']],
         ["with_trailing_double_quote", ['demo_na_project"']],
         ["with_invalid_id", ['"demo"na_project']],
         ["with_unquoted_inner_quote", ['"demo"na_project"']],
         ["empty_path", [""]],
@@ -99,15 +97,23 @@
         ["empty_name", [PROJECT_PATH, "--name", ""]],
     ],
 )
 @mock.patch(
     "snowflake.cli.plugins.nativeapp.init._init_from_template", return_value=None
 )
 def test_init_no_template_failure(
-    mock_init_from_template, runner, temp_dir, snapshot, id, init_args
+    mock_init_from_template, runner, temp_dir, snapshot, id_, init_args
 ):
     args = ["app", "init"]
     args.extend(init_args)
     result = runner.invoke(args)
 
     assert result.exit_code == 1
     assert result.output == snapshot
+
+
+def test_list_templates_no_options_success(runner, temp_dir, snapshot):
+    args = ["app", "list-templates"]
+    result = runner.invoke(args)
+
+    assert result.exit_code == 0
+    assert result.output == snapshot
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_init.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from pathlib import Path
 from textwrap import dedent
+from unittest import mock
 
+import pytest
 from snowflake.cli.api.exceptions import MissingConfiguration
 from snowflake.cli.plugins.nativeapp.init import (
     CannotInitializeAnExistingProjectError,
     DirectoryAlreadyExistsError,
     InitError,
     ProjectNameInvalidError,
     RenderingFromJinjaError,
@@ -11,15 +14,15 @@
     _render_snowflake_yml,
     _replace_snowflake_yml_name_with_project,
     _to_yaml_string,
     _validate_and_update_snowflake_yml,
     nativeapp_init,
 )
 
-from tests.testing_utils.fixtures import *
+from tests.testing_utils.files_and_dirs import create_named_file
 
 PROJECT_PATH = "demo-na-project"
 PROJECT_NAME = "demo_na_project"
 CUSTOM_GIT_REPO_URL = "https://testing.com/my-native-app-template"
 
 
 SNOWFLAKE_YML = dedent(
@@ -44,73 +47,79 @@
 
 # --------------------------------------
 # ----- Test Harness Helpers -------
 # --------------------------------------
 
 
 def fake_clone_template_with_files(files: dict):
-    def fake_clone_mock(url: str, to_path: str, filter: list, depth: int):
+    def fake_clone_mock(url: str, to_path: str, filter: list, depth: int):  # noqa: A002
         repo_path = Path(to_path)
         repo_path.mkdir(parents=True, exist_ok=True)
 
         # create a fake .git directory
         git_dir_path = repo_path / ".git"
         git_dir_path.mkdir()
 
         for file_name in files:
             file_contents = files[file_name]
             create_named_file(
                 file_name=file_name,
-                dir=str(repo_path),
+                dir_name=str(repo_path),
                 contents=[file_contents],
             )
         return mock.MagicMock()
 
     return fake_clone_mock
 
 
 def fake_clone_template_with_file(file_name: str, file_contents: str):
     return fake_clone_template_with_files({file_name: file_contents})
 
 
-def fake_clone_default_repo(url: str, to_path: str, filter: list, depth: int):
+def fake_clone_default_repo(
+    url: str, to_path: str, filter: list, depth: int  # noqa: A002
+):
     assert url == "https://github.com/snowflakedb/native-apps-templates"
     repo_path = Path(to_path)
     repo_path.mkdir(parents=True, exist_ok=True)
 
     # create a fake .git directory
     git_dir_path = repo_path / ".git"
     git_dir_path.mkdir()
 
     # create a fake basic template
     basic_template_dir = repo_path / "basic"
     basic_template_dir.mkdir()
     create_named_file(
         file_name="snowflake.yml.jinja",
-        dir=str(basic_template_dir),
+        dir_name=str(basic_template_dir),
         contents=[TEMPLATED_SNOWFLAKE_YML],
     )
 
     # create a fake python-streamlit template
     py_template_dir = repo_path / "python-streamlit"
     py_template_dir.mkdir()
     create_named_file(
         file_name="snowflake.yml.jinja",
-        dir=str(py_template_dir),
+        dir_name=str(py_template_dir),
         contents=[TEMPLATED_SNOWFLAKE_YML],
     )
     return mock.MagicMock()
 
 
-def fake_clone_jinja_template_repo(url: str, to_path: str, filter: list, depth: int):
+def fake_clone_jinja_template_repo(
+    url: str, to_path: str, filter: list, depth: int  # noqa: A002
+):
     fn = fake_clone_template_with_file("snowflake.yml.jinja", TEMPLATED_SNOWFLAKE_YML)
     return fn(url=url, to_path=to_path, filter=filter, depth=depth)
 
 
-def fake_clone_template_repo(url: str, to_path: str, filter: list, depth: int):
+def fake_clone_template_repo(
+    url: str, to_path: str, filter: list, depth: int  # noqa: A002
+):
     fn = fake_clone_template_with_file("snowflake.yml", SNOWFLAKE_YML)
     return fn(url=url, to_path=to_path, filter=filter, depth=depth)
 
 
 # --------------------------------------
 # ----- Tests for Helper Methods -------
 # --------------------------------------
@@ -129,15 +138,15 @@
     assert _to_yaml_string(python_string) == yaml_string
 
 
 def test_render_snowflake_yml(other_directory):
     temp_dir = Path(other_directory)
     create_named_file(
         file_name="snowflake.yml.jinja",
-        dir=str(temp_dir),
+        dir_name=str(temp_dir),
         contents=[
             dedent(
                 """\
             native_app:
                 name: {{project_name}}
                 artifacts:
                     - app/setup_script.sql
@@ -162,15 +171,15 @@
     assert temp_dir.joinpath("snowflake.yml").read_text() == expected
 
 
 def test_render_snowflake_yml_raises_exception(other_directory):
     temp_dir = Path(other_directory)
     create_named_file(
         file_name="snowflake.yml.jinja",
-        dir=str(temp_dir),
+        dir_name=str(temp_dir),
         contents=[
             dedent(
                 """\
             native_app:
                 name: {{project_name}}
                 artifacts:
                     - {{one_more_variable}}
@@ -184,15 +193,15 @@
         )
 
 
 def test_replace_snowflake_yml_name_with_project_populated_file(other_directory):
     temp_dir = Path(other_directory)
     create_named_file(
         file_name="snowflake.yml",
-        dir=str(temp_dir),
+        dir_name=str(temp_dir),
         contents=[
             dedent(
                 """\
             native_app:
                 name: old_value
                 artifacts:
                     - app/setup_script.sql
@@ -216,15 +225,15 @@
     assert path_to_snowflake_yml.read_text() == expected
 
 
 def test_replace_snowflake_yml_name_with_project_empty_file(other_directory):
     temp_dir = Path(other_directory)
     create_named_file(
         file_name="snowflake.yml",
-        dir=str(temp_dir),
+        dir_name=str(temp_dir),
         contents=[""],
     )
     expected = dedent(
         f"""\
         native_app:
           name: {PROJECT_NAME}
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_manager.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,45 @@
+import os
 from textwrap import dedent
+from unittest import mock
+
+import pytest
+from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.constants import (
     LOOSE_FILES_MAGIC_VERSION,
     NAME_COL,
     SPECIAL_COMMENT,
+    SPECIAL_COMMENT_OLD,
+)
+from snowflake.cli.plugins.nativeapp.exceptions import (
+    ApplicationPackageAlreadyExistsError,
+    UnexpectedOwnerError,
 )
-from snowflake.cli.plugins.nativeapp.exceptions import UnexpectedOwnerError
 from snowflake.cli.plugins.nativeapp.manager import (
     NativeAppManager,
     SnowflakeSQLExecutionError,
     ensure_correct_owner,
 )
-from snowflake.cli.plugins.object.stage.diff import DiffResult
-from snowflake.cli.api.project.definition_manager import DefinitionManager
+from snowflake.cli.plugins.stage.diff import DiffResult
+from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
 from tests.nativeapp.patch_utils import (
     mock_connection,
     mock_get_app_pkg_distribution_in_sf,
 )
 from tests.nativeapp.utils import (
     NATIVEAPP_MANAGER_EXECUTE,
+    NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO,
+    NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME,
     NATIVEAPP_MODULE,
     mock_execute_helper,
     mock_snowflake_yml_file,
 )
-from tests.testing_utils.fixtures import *
+from tests.testing_utils.files_and_dirs import create_named_file
 
 mock_project_definition_override = {
     "native_app": {
         "application": {
             "name": "sample_application_name",
             "role": "sample_application_role",
         },
@@ -39,15 +50,15 @@
     }
 }
 
 
 def _get_na_manager():
     dm = DefinitionManager()
     return NativeAppManager(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock.patch(f"{NATIVEAPP_MODULE}.stage_diff")
 @mock.patch(f"{NATIVEAPP_MODULE}.sync_local_diff_with_stage")
@@ -57,15 +68,15 @@
     mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
     mock_diff_result = DiffResult(different=["setup.sql"])
     mock_stage_diff.return_value = mock_diff_result
     mock_local_diff_with_stage.return_value = None
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     assert mock_diff_result.has_changes()
     native_app_manager.sync_deploy_root_with_stage("new_role")
 
@@ -118,15 +129,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     actual_distribution = native_app_manager.get_app_pkg_distribution_in_snowflake
     assert actual_distribution == "external"
     assert mock_execute.mock_calls == expected
@@ -154,15 +165,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     with pytest.raises(ProgrammingError):
         native_app_manager.get_app_pkg_distribution_in_snowflake
 
@@ -186,15 +197,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     with pytest.raises(SnowflakeSQLExecutionError):
         native_app_manager.get_app_pkg_distribution_in_snowflake
 
@@ -221,15 +232,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     with pytest.raises(ProgrammingError):
         native_app_manager.get_app_pkg_distribution_in_snowflake
 
@@ -238,21 +249,21 @@
 
 @mock_get_app_pkg_distribution_in_sf()
 def test_is_app_pkg_distribution_same_in_sf_w_arg(mock_mismatch, temp_dir):
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     create_named_file(
         file_name="snowflake.local.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[
             dedent(
                 """\
                     native_app:
                         package:
                             distribution: >-
                                 EXTERNAL
@@ -269,21 +280,21 @@
 @mock_get_app_pkg_distribution_in_sf()
 def test_is_app_pkg_distribution_same_in_sf_no_mismatch(mock_mismatch, temp_dir):
     mock_mismatch.return_value = "external"
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     create_named_file(
         file_name="snowflake.local.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[
             dedent(
                 """\
                     native_app:
                         package:
                             distribution: >-
                                 EXTERNAL
@@ -302,15 +313,15 @@
     mock_warning, mock_mismatch, temp_dir
 ):
     mock_mismatch.return_value = "external"
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     assert native_app_manager.verify_project_distribution() is False
     mock_warning.assert_called_once_with(
         "Application package app_pkg in your Snowflake account has distribution property external,\nwhich does not match the value specified in project definition file: internal.\n"
@@ -344,15 +355,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     show_obj_row = native_app_manager.get_existing_app_info()
     assert show_obj_row is not None
     assert show_obj_row[NAME_COL] == "MYAPP"
@@ -376,15 +387,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     show_obj_row = native_app_manager.get_existing_app_info()
     assert show_obj_row is None
     assert mock_execute.mock_calls == expected
@@ -420,15 +431,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     show_obj_row = native_app_manager.get_existing_app_pkg_info()
     assert show_obj_row is not None
     assert show_obj_row[NAME_COL] == "APP_PKG"
@@ -457,15 +468,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     show_obj_row = native_app_manager.get_existing_app_pkg_info()
     assert show_obj_row is None
     assert mock_execute.mock_calls == expected
@@ -482,15 +493,15 @@
     mock_snowsight_host.return_value = "https://host"
     mock_context.return_value = "organization"
     mock_account.return_value = "account"
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     assert (
         native_app_manager.get_snowsight_url()
         == "https://host/organization/account/#/apps/application/MYAPP"
@@ -505,7 +516,203 @@
     )
 
 
 def test_is_correct_owner_bad_owner():
     test_row = {"name": "some_name", "owner": "wrong_role", "comment": "some_comment"}
     with pytest.raises(UnexpectedOwnerError):
         ensure_correct_owner(row=test_row, role="right_role", obj_name="some_name")
+
+
+# Test create_app_package() with no existing package available
+@mock.patch(NATIVEAPP_MANAGER_EXECUTE)
+@mock.patch(NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO, return_value=None)
+def test_create_app_pkg_no_existing_package(
+    mock_get_existing_app_pkg_info, mock_execute, temp_dir, mock_cursor
+):
+    side_effects, expected = mock_execute_helper(
+        [
+            (
+                mock_cursor([{"CURRENT_ROLE()": "old_role"}], []),
+                mock.call("select current_role()", cursor_class=DictCursor),
+            ),
+            (None, mock.call("use role package_role")),
+            (
+                None,
+                mock.call(
+                    dedent(
+                        f"""\
+                        create application package app_pkg
+                            comment = {SPECIAL_COMMENT}
+                            distribution = internal
+                    """
+                    )
+                ),
+            ),
+            (None, mock.call("use role old_role")),
+        ]
+    )
+    mock_execute.side_effect = side_effects
+
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+
+    native_app_manager = _get_na_manager()
+    native_app_manager.create_app_package()
+    assert mock_execute.mock_calls == expected
+    mock_get_existing_app_pkg_info.assert_called_once()
+
+
+# Test create_app_package() with incorrect owner
+@mock.patch(NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO)
+def test_create_app_pkg_incorrect_owner(mock_get_existing_app_pkg_info, temp_dir):
+    mock_get_existing_app_pkg_info.return_value = {
+        "name": "APP_PKG",
+        "comment": SPECIAL_COMMENT,
+        "version": LOOSE_FILES_MAGIC_VERSION,
+        "owner": "wrong_owner",
+    }
+
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+
+    with pytest.raises(UnexpectedOwnerError):
+        native_app_manager = _get_na_manager()
+        native_app_manager.create_app_package()
+
+
+# Test create_app_package() with distribution external AND variable mismatch
+@mock.patch(NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO)
+@mock_get_app_pkg_distribution_in_sf()
+@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
+@mock.patch(f"{NATIVEAPP_MODULE}.cc.warning")
+@pytest.mark.parametrize(
+    "is_pkg_distribution_same",
+    [False, True],
+)
+def test_create_app_pkg_external_distribution(
+    mock_warning,
+    mock_is_distribution_same,
+    mock_get_distribution,
+    mock_get_existing_app_pkg_info,
+    is_pkg_distribution_same,
+    temp_dir,
+):
+    mock_is_distribution_same.return_value = is_pkg_distribution_same
+    mock_get_distribution.return_value = "external"
+    mock_get_existing_app_pkg_info.return_value = {
+        "name": "APP_PKG",
+        "comment": "random",
+        "version": LOOSE_FILES_MAGIC_VERSION,
+        "owner": "PACKAGE_ROLE",
+    }
+
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+
+    native_app_manager = _get_na_manager()
+    native_app_manager.create_app_package()
+    if not is_pkg_distribution_same:
+        mock_warning.assert_called_once_with(
+            "Continuing to execute `snow app run` on application package app_pkg with distribution 'external'."
+        )
+
+
+# Test create_app_package() with distribution internal AND variable mismatch AND special comment is True
+@mock.patch(NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO)
+@mock_get_app_pkg_distribution_in_sf()
+@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
+@mock.patch(f"{NATIVEAPP_MODULE}.cc.warning")
+@pytest.mark.parametrize(
+    "is_pkg_distribution_same, special_comment",
+    [
+        (False, SPECIAL_COMMENT),
+        (False, SPECIAL_COMMENT_OLD),
+        (True, SPECIAL_COMMENT),
+        (True, SPECIAL_COMMENT_OLD),
+    ],
+)
+def test_create_app_pkg_internal_distribution_special_comment(
+    mock_warning,
+    mock_is_distribution_same,
+    mock_get_distribution,
+    mock_get_existing_app_pkg_info,
+    is_pkg_distribution_same,
+    special_comment,
+    temp_dir,
+):
+    mock_is_distribution_same.return_value = is_pkg_distribution_same
+    mock_get_distribution.return_value = "internal"
+    mock_get_existing_app_pkg_info.return_value = {
+        "name": "APP_PKG",
+        "comment": special_comment,
+        "version": LOOSE_FILES_MAGIC_VERSION,
+        "owner": "PACKAGE_ROLE",
+    }
+
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+
+    native_app_manager = _get_na_manager()
+    native_app_manager.create_app_package()
+    if not is_pkg_distribution_same:
+        mock_warning.assert_called_once_with(
+            "Continuing to execute `snow app run` on application package app_pkg with distribution 'internal'."
+        )
+
+
+# Test create_app_package() with distribution internal AND variable mismatch AND special comment is False
+@mock.patch(NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO)
+@mock_get_app_pkg_distribution_in_sf()
+@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
+@mock.patch(f"{NATIVEAPP_MODULE}.cc.warning")
+@pytest.mark.parametrize(
+    "is_pkg_distribution_same",
+    [False, True],
+)
+def test_create_app_pkg_internal_distribution_no_special_comment(
+    mock_warning,
+    mock_is_distribution_same,
+    mock_get_distribution,
+    mock_get_existing_app_pkg_info,
+    is_pkg_distribution_same,
+    temp_dir,
+):
+    mock_is_distribution_same.return_value = is_pkg_distribution_same
+    mock_get_distribution.return_value = "internal"
+    mock_get_existing_app_pkg_info.return_value = {
+        "name": "APP_PKG",
+        "comment": "dummy",
+        "version": LOOSE_FILES_MAGIC_VERSION,
+        "owner": "PACKAGE_ROLE",
+    }
+
+    current_working_directory = os.getcwd()
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=current_working_directory,
+        contents=[mock_snowflake_yml_file],
+    )
+
+    native_app_manager = _get_na_manager()
+    with pytest.raises(ApplicationPackageAlreadyExistsError):
+        native_app_manager.create_app_package()
+
+    if not is_pkg_distribution_same:
+        mock_warning.assert_called_once_with(
+            "Continuing to execute `snow app run` on application package app_pkg with distribution 'internal'."
+        )
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_package_scripts.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
 import pytest
+from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.exceptions import (
     InvalidPackageScriptError,
     MissingPackageScriptError,
 )
 from snowflake.cli.plugins.nativeapp.run_processor import NativeAppRunProcessor
-from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.connector import ProgrammingError
 
 from tests.nativeapp.patch_utils import mock_connection
 from tests.nativeapp.utils import (
     NATIVEAPP_MANAGER_EXECUTE,
     NATIVEAPP_MANAGER_EXECUTE_QUERIES,
 )
-from tests.project.fixtures import *
-from tests.testing_utils.fixtures import *
+from tests.testing_utils.fixtures import MockConnectionCtx
 
 
 def _get_na_manager(working_dir):
     dm = DefinitionManager(working_dir)
     return NativeAppRunProcessor(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
@@ -44,15 +44,15 @@
     mock_execute_queries,
     project_definition_files,
     expected_call,
 ):
     mock_conn.return_value = MockConnectionCtx()
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
-    native_app_manager._apply_package_scripts()
+    native_app_manager._apply_package_scripts()  # noqa: SLF001
     assert mock_execute_query.mock_calls == [
         mock.call(expected_call),
     ]
     assert mock_execute_queries.mock_calls == [
         mock.call(
             dedent(
                 f"""\
@@ -84,45 +84,45 @@
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
 def test_missing_package_script(mock_execute, project_definition_files):
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
     with pytest.raises(MissingPackageScriptError):
         (working_dir / "002-shared.sql").unlink()
-        native_app_manager._apply_package_scripts()
+        native_app_manager._apply_package_scripts()  # noqa: SLF001
 
     # even though the second script was the one missing, nothing should be executed
     assert mock_execute.mock_calls == []
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
 def test_invalid_package_script(mock_execute, project_definition_files):
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
     with pytest.raises(InvalidPackageScriptError):
         second_file = working_dir / "002-shared.sql"
         second_file.unlink()
         second_file.write_text("select * from {{ package_name")
-        native_app_manager._apply_package_scripts()
+        native_app_manager._apply_package_scripts()  # noqa: SLF001
 
     # even though the second script was the one missing, nothing should be executed
     assert mock_execute.mock_calls == []
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
 def test_undefined_var_package_script(mock_execute, project_definition_files):
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
     with pytest.raises(InvalidPackageScriptError):
         second_file = working_dir / "001-shared.sql"
         second_file.unlink()
         second_file.write_text("select * from {{ abc }}")
-        native_app_manager._apply_package_scripts()
+        native_app_manager._apply_package_scripts()  # noqa: SLF001
 
     assert mock_execute.mock_calls == []
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
@@ -140,15 +140,15 @@
         msg="No active warehouse selected in the current session.", errno=606
     )
 
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
 
     with pytest.raises(ProgrammingError) as err:
-        native_app_manager._apply_package_scripts()
+        native_app_manager._apply_package_scripts()  # noqa: SLF001
 
     assert "Please provide a warehouse for the active session role" in err.value.msg
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
 @pytest.mark.parametrize("project_definition_files", ["napp_project_1"], indirect=True)
@@ -162,10 +162,10 @@
         msg="Object does not exist, or operation cannot be performed.", errno=2043
     )
 
     working_dir: Path = project_definition_files[0].parent
     native_app_manager = _get_na_manager(str(working_dir))
 
     with pytest.raises(ProgrammingError) as err:
-        native_app_manager._apply_package_scripts()
+        native_app_manager._apply_package_scripts()  # noqa: SLF001
 
     assert "Please grant usage privilege on warehouse to this role." in err.value.msg
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_run_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-import unittest
+import os
 from textwrap import dedent
+from unittest import mock
 
+import pytest
 import typer
 from click import UsageError
+from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.constants import (
     LOOSE_FILES_MAGIC_VERSION,
     SPECIAL_COMMENT,
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationAlreadyExistsError,
-    ApplicationPackageAlreadyExistsError,
     ApplicationPackageDoesNotExistError,
     UnexpectedOwnerError,
 )
 from snowflake.cli.plugins.nativeapp.policy import (
     AllowAlwaysPolicy,
     AskAlwaysPolicy,
     DenyAlwaysPolicy,
 )
 from snowflake.cli.plugins.nativeapp.run_processor import NativeAppRunProcessor
-from snowflake.cli.plugins.object.stage.diff import DiffResult
-from snowflake.cli.api.project.definition_manager import DefinitionManager
+from snowflake.cli.plugins.stage.diff import DiffResult
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
 from src.snowflake.cli.plugins.nativeapp.constants import SPECIAL_COMMENT_OLD
 from tests.nativeapp.patch_utils import (
     mock_connection,
-    mock_get_app_pkg_distribution_in_sf,
 )
-from tests.nativeapp.utils import *
-from tests.testing_utils.fixtures import *
+from tests.nativeapp.utils import (
+    NATIVEAPP_MANAGER_EXECUTE,
+    NATIVEAPP_MANAGER_EXECUTE_QUERIES,
+    RUN_PROCESSOR_GET_EXISTING_APP_INFO,
+    TYPER_CONFIRM,
+    mock_execute_helper,
+    mock_snowflake_yml_file,
+    quoted_override_yml_file,
+)
+from tests.testing_utils.files_and_dirs import create_named_file
+from tests.testing_utils.fixtures import MockConnectionCtx
 
 mock_project_definition_override = {
     "native_app": {
         "application": {
             "name": "sample_application_name",
             "role": "sample_application_role",
         },
@@ -49,215 +58,19 @@
 ask_always_policy = AskAlwaysPolicy()
 deny_always_policy = DenyAlwaysPolicy()
 
 
 def _get_na_run_processor():
     dm = DefinitionManager()
     return NativeAppRunProcessor(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
-# Test create_app_package() with no existing package available
-@mock.patch(NATIVEAPP_MANAGER_EXECUTE)
-@mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO, return_value=None)
-def test_create_app_pkg_no_existing_package(
-    mock_get_existing_app_pkg_info, mock_execute, temp_dir, mock_cursor
-):
-    side_effects, expected = mock_execute_helper(
-        [
-            (
-                mock_cursor([{"CURRENT_ROLE()": "old_role"}], []),
-                mock.call("select current_role()", cursor_class=DictCursor),
-            ),
-            (None, mock.call("use role package_role")),
-            (
-                None,
-                mock.call(
-                    dedent(
-                        f"""\
-                        create application package app_pkg
-                            comment = {SPECIAL_COMMENT}
-                            distribution = internal
-                    """
-                    )
-                ),
-            ),
-            (None, mock.call("use role old_role")),
-        ]
-    )
-    mock_execute.side_effect = side_effects
-
-    current_working_directory = os.getcwd()
-    create_named_file(
-        file_name="snowflake.yml",
-        dir=current_working_directory,
-        contents=[mock_snowflake_yml_file],
-    )
-
-    run_processor = _get_na_run_processor()
-    run_processor.create_app_package()
-    assert mock_execute.mock_calls == expected
-    mock_get_existing_app_pkg_info.assert_called_once()
-
-
-# Test create_app_package() with incorrect owner
-@mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO)
-def test_create_app_pkg_incorrect_owner(mock_get_existing_app_pkg_info, temp_dir):
-    mock_get_existing_app_pkg_info.return_value = {
-        "name": "APP_PKG",
-        "comment": SPECIAL_COMMENT,
-        "version": LOOSE_FILES_MAGIC_VERSION,
-        "owner": "wrong_owner",
-    }
-
-    current_working_directory = os.getcwd()
-    create_named_file(
-        file_name="snowflake.yml",
-        dir=current_working_directory,
-        contents=[mock_snowflake_yml_file],
-    )
-
-    with pytest.raises(UnexpectedOwnerError):
-        run_processor = _get_na_run_processor()
-        run_processor.create_app_package()
-
-
-# Test create_app_package() with distribution external AND variable mismatch
-@mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO)
-@mock_get_app_pkg_distribution_in_sf()
-@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
-@mock.patch(f"{RUN_MODULE}.cc.warning")
-@pytest.mark.parametrize(
-    "is_pkg_distribution_same",
-    [False, True],
-)
-def test_create_app_pkg_external_distribution(
-    mock_warning,
-    mock_is_distribution_same,
-    mock_get_distribution,
-    mock_get_existing_app_pkg_info,
-    is_pkg_distribution_same,
-    temp_dir,
-):
-    mock_is_distribution_same.return_value = is_pkg_distribution_same
-    mock_get_distribution.return_value = "external"
-    mock_get_existing_app_pkg_info.return_value = {
-        "name": "APP_PKG",
-        "comment": "random",
-        "version": LOOSE_FILES_MAGIC_VERSION,
-        "owner": "PACKAGE_ROLE",
-    }
-
-    current_working_directory = os.getcwd()
-    create_named_file(
-        file_name="snowflake.yml",
-        dir=current_working_directory,
-        contents=[mock_snowflake_yml_file],
-    )
-
-    run_processor = _get_na_run_processor()
-    run_processor.create_app_package()
-    if not is_pkg_distribution_same:
-        mock_warning.assert_called_once_with(
-            "Continuing to execute `snow app run` on application package app_pkg with distribution 'external'."
-        )
-
-
-# Test create_app_package() with distribution internal AND variable mismatch AND special comment is True
-@mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO)
-@mock_get_app_pkg_distribution_in_sf()
-@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
-@mock.patch(f"{RUN_MODULE}.cc.warning")
-@pytest.mark.parametrize(
-    "is_pkg_distribution_same, special_comment",
-    [
-        (False, SPECIAL_COMMENT),
-        (False, SPECIAL_COMMENT_OLD),
-        (True, SPECIAL_COMMENT),
-        (True, SPECIAL_COMMENT_OLD),
-    ],
-)
-def test_create_app_pkg_internal_distribution_special_comment(
-    mock_warning,
-    mock_is_distribution_same,
-    mock_get_distribution,
-    mock_get_existing_app_pkg_info,
-    is_pkg_distribution_same,
-    special_comment,
-    temp_dir,
-):
-    mock_is_distribution_same.return_value = is_pkg_distribution_same
-    mock_get_distribution.return_value = "internal"
-    mock_get_existing_app_pkg_info.return_value = {
-        "name": "APP_PKG",
-        "comment": special_comment,
-        "version": LOOSE_FILES_MAGIC_VERSION,
-        "owner": "PACKAGE_ROLE",
-    }
-
-    current_working_directory = os.getcwd()
-    create_named_file(
-        file_name="snowflake.yml",
-        dir=current_working_directory,
-        contents=[mock_snowflake_yml_file],
-    )
-
-    run_processor = _get_na_run_processor()
-    run_processor.create_app_package()
-    if not is_pkg_distribution_same:
-        mock_warning.assert_called_once_with(
-            "Continuing to execute `snow app run` on application package app_pkg with distribution 'internal'."
-        )
-
-
-# Test create_app_package() with distribution internal AND variable mismatch AND special comment is False
-@mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO)
-@mock_get_app_pkg_distribution_in_sf()
-@mock.patch(NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME)
-@mock.patch(f"{RUN_MODULE}.cc.warning")
-@pytest.mark.parametrize(
-    "is_pkg_distribution_same",
-    [False, True],
-)
-def test_create_app_pkg_internal_distribution_no_special_comment(
-    mock_warning,
-    mock_is_distribution_same,
-    mock_get_distribution,
-    mock_get_existing_app_pkg_info,
-    is_pkg_distribution_same,
-    temp_dir,
-):
-    mock_is_distribution_same.return_value = is_pkg_distribution_same
-    mock_get_distribution.return_value = "internal"
-    mock_get_existing_app_pkg_info.return_value = {
-        "name": "APP_PKG",
-        "comment": "dummy",
-        "version": LOOSE_FILES_MAGIC_VERSION,
-        "owner": "PACKAGE_ROLE",
-    }
-
-    current_working_directory = os.getcwd()
-    create_named_file(
-        file_name="snowflake.yml",
-        dir=current_working_directory,
-        contents=[mock_snowflake_yml_file],
-    )
-
-    run_processor = _get_na_run_processor()
-    with pytest.raises(ApplicationPackageAlreadyExistsError):
-        run_processor.create_app_package()
-
-    if not is_pkg_distribution_same:
-        mock_warning.assert_called_once_with(
-            "Continuing to execute `snow app run` on application package app_pkg with distribution 'internal'."
-        )
-
-
 # Test create_dev_app with exception thrown trying to use the warehouse
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
 def test_create_dev_app_w_warehouse_access_exception(
     mock_conn, mock_execute, temp_dir, mock_cursor
 ):
     side_effects, expected = mock_execute_helper(
@@ -280,23 +93,23 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
 
     with pytest.raises(ProgrammingError) as err:
-        run_processor._create_dev_app(mock_diff_result)
+        run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
 
     assert mock_execute.mock_calls == expected
     assert "Please grant usage privilege on warehouse to this role." in err.value.msg
 
 
 # Test create_dev_app with no existing application AND create succeeds AND app role == package role
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO, return_value=None)
@@ -333,21 +146,21 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file.replace("package_role", "app_role")],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with no existing application AND create succeeds AND app role != package role
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO, return_value=None)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE_QUERIES)
@@ -407,21 +220,21 @@
     ]
     mock_execute_queries.side_effect = [None, None, None]
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute_query.mock_calls == mock_execute_query_expected
     assert mock_execute_queries.mock_calls == mock_execute_queries_expected
 
 
 # Test create_dev_app with no existing application AND create throws an exception
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO, return_value=None)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
@@ -460,23 +273,23 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file.replace("package_role", "app_role")],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
 
     with pytest.raises(ProgrammingError) as err:
-        run_processor._create_dev_app(mock_diff_result)
+        run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
 
     assert "Please provide a warehouse for the active session role" in err.value.msg
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with existing application AND bad comment AND good version
 # Test create_dev_app with existing application AND bad comment AND bad version
@@ -522,22 +335,22 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     with pytest.raises(ApplicationAlreadyExistsError):
         run_processor = _get_na_run_processor()
         assert not mock_diff_result.has_changes()
-        run_processor._create_dev_app(mock_diff_result)
+        run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
 
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with existing application AND incorrect owner
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
@@ -565,22 +378,22 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     with pytest.raises(UnexpectedOwnerError):
         run_processor = _get_na_run_processor()
         assert not mock_diff_result.has_changes()
-        run_processor._create_dev_app(mock_diff_result)
+        run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
 
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with existing application AND diff has no changes
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
@@ -609,21 +422,21 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with existing application AND diff has changes
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
@@ -657,21 +470,21 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult(different=["setup.sql"])
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with existing application AND alter throws an error
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
@@ -706,23 +519,23 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult(different=["setup.sql"])
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert mock_diff_result.has_changes()
 
     with pytest.raises(ProgrammingError) as err:
-        run_processor._create_dev_app(mock_diff_result)
+        run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
 
     assert mock_execute.mock_calls == expected
     assert "Please provide a warehouse for the active session role" in err.value.msg
 
 
 # Test create_dev_app with no existing application AND quoted name scenario 1
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO, return_value=None)
@@ -759,30 +572,31 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[
             dedent(
                 """\
             definition_version: 1
             native_app:
                 name: '"My Native Application"'
-
+            
                 source_stage:
                     app_src.stage
-
+            
                 artifacts:
                 - setup.sql
                 - app/README.md
                 - src: app/streamlit/*.py
-                dest: ui/
+                  dest: ui/
+
 
                 application:
                     name: >-
                         "My Application"
                     role: app_role
                     warehouse: app_warehouse
                     debug: true
@@ -796,15 +610,15 @@
         """
             )
         ],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute.mock_calls == expected
 
 
 # Test create_dev_app with no existing application AND quoted name scenario 2
 @mock.patch(RUN_PROCESSOR_GET_EXISTING_APP_INFO, return_value=None)
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
@@ -839,26 +653,26 @@
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     mock_diff_result = DiffResult()
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file.replace("package_role", "app_role")],
     )
     create_named_file(
         file_name="snowflake.local.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[quoted_override_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     assert not mock_diff_result.has_changes()
-    run_processor._create_dev_app(mock_diff_result)
+    run_processor._create_dev_app(mock_diff_result)  # noqa: SLF001
     assert mock_execute.mock_calls == expected
 
 
 # Test upgrade app method for release directives AND throws warehouse error
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 @mock_connection()
 @pytest.mark.parametrize(
@@ -886,15 +700,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(ProgrammingError):
         run_processor.upgrade_app(policy_param, is_interactive=True)
     assert mock_execute.mock_calls == expected
@@ -933,15 +747,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(UnexpectedOwnerError):
         run_processor.upgrade_app(policy=policy_param, is_interactive=True)
     assert mock_execute.mock_calls == expected
@@ -981,15 +795,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     run_processor.upgrade_app(policy=policy_param, is_interactive=True)
     assert mock_execute.mock_calls == expected
 
@@ -1034,15 +848,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(ProgrammingError):
         run_processor.upgrade_app(policy=policy_param, is_interactive=True)
     assert mock_execute.mock_calls == expected
@@ -1097,15 +911,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(typer.Exit):
         result = run_processor.upgrade_app(
             policy_param, is_interactive=is_interactive_param
@@ -1169,15 +983,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(ProgrammingError):
         run_processor.upgrade_app(policy_param, is_interactive=is_interactive_param)
     assert mock_execute.mock_calls == expected
@@ -1250,15 +1064,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     run_processor.upgrade_app(policy_param, is_interactive=True)
     assert mock_execute.mock_calls == expected
 
@@ -1274,15 +1088,15 @@
 def test_upgrade_app_from_version_throws_usage_error_one(
     mock_existing, policy_param, temp_dir
 ):
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(UsageError):
         run_processor.process(policy=policy_param, version="v1", is_interactive=True)
 
@@ -1298,15 +1112,15 @@
 def test_upgrade_app_from_version_throws_usage_error_two(
     mock_existing, policy_param, temp_dir
 ):
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     with pytest.raises(UsageError):
         run_processor.process(policy=policy_param, version="v1", is_interactive=True)
 
@@ -1390,15 +1204,15 @@
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     run_processor = _get_na_run_processor()
     run_processor.process(policy=policy_param, version="v1", is_interactive=True)
     assert mock_execute.mock_calls == expected
 
@@ -1435,15 +1249,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_na_run_processor()
     result = processor.get_existing_version_info(version)
     assert mock_execute.mock_calls == expected
     assert result["version"] == version
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_teardown_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 )
 from tests.testing_utils.files_and_dirs import create_named_file
 
 
 def _get_na_teardown_processor():
     dm = DefinitionManager()
     return NativeAppTeardownProcessor(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 # Test drop_generic_object() with success
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 def test_drop_generic_object_success(mock_execute, temp_dir, mock_cursor):
@@ -58,15 +58,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_generic_object(
         object_type="application", object_name="myapp", role="app_role"
     )
@@ -94,15 +94,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     with pytest.raises(SnowflakeSQLExecutionError):
         teardown_processor.drop_generic_object(
             object_type="application package",
@@ -121,15 +121,15 @@
 )
 def test_drop_application_no_existing_application(
     mock_warning, mock_get_existing_app_info, auto_yes_param, temp_dir
 ):
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes_param)
     mock_get_existing_app_info.assert_called_once()
     mock_warning.assert_called_once_with(
@@ -151,15 +151,15 @@
         "owner": "different_owner",
         "comment": "some_comment",
     }
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     with pytest.raises(UnexpectedOwnerError):
         teardown_processor.drop_application(auto_yes_param)
     mock_get_existing_app_info.assert_called_once()
@@ -191,15 +191,15 @@
         "owner": "app_role",
         "comment": special_comment,
     }
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes_param)
     mock_get_existing_app_info.assert_called_once()
     mock_is_correct_owner.assert_called_once()
@@ -260,20 +260,20 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
     create_named_file(
         file_name="snowflake.local.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[quoted_override_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes_param)
     mock_execute.mock_calls == expected
 
@@ -301,15 +301,15 @@
         "version": "dummy",
         "patch": "dummy",
     }
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes=False)
     mock_get_existing_app_info.assert_called_once()
     mock_is_correct_owner.assert_called_once()
@@ -358,15 +358,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes_param)
     mock_get_existing_app_info.assert_called_once()
     mock_is_correct_owner.assert_called_once()
@@ -395,15 +395,15 @@
         None,
     ]
     mock_get_existing_app_info.side_effect = side_effects_for_get_existing_app_info
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_application(auto_yes_param)
     teardown_processor.drop_application(auto_yes_param)
     teardown_processor.drop_application(auto_yes_param)
@@ -426,15 +426,15 @@
 def test_drop_package_no_existing_application(
     mock_warning, mock_get_existing_app_pkg_info, auto_yes_param, temp_dir
 ):
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     mock_get_existing_app_pkg_info.assert_called_once()
     mock_warning.assert_called_once_with(
@@ -456,15 +456,15 @@
         "owner": "different_owner",
         "comment": "some_comment",
     }
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     with pytest.raises(UnexpectedOwnerError):
         teardown_processor.drop_package(auto_yes_param)
     mock_get_existing_app_pkg_info.assert_called_once()
@@ -506,15 +506,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     with pytest.raises(CouldNotDropApplicationPackageWithVersions):
         teardown_processor.drop_package(auto_yes_param)
     mock_is_correct_owner.assert_called_once()
@@ -561,15 +561,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes=False)
     mock_execute.mock_calls == expected
 
@@ -628,15 +628,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     mock_execute.mock_calls == expected
     if not is_pkg_distribution_same:
@@ -701,15 +701,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     mock_execute.mock_calls == expected
     mock_drop_generic_object.assert_called_once()
@@ -791,20 +791,20 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
     create_named_file(
         file_name="snowflake.local.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[quoted_override_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     mock_execute.mock_calls == expected
 
@@ -856,15 +856,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes=False)
     mock_execute.mock_calls == expected
     if not is_pkg_distribution_same:
@@ -926,15 +926,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     mock_execute.mock_calls == expected
     mock_drop_generic_object.assert_called_once()
@@ -987,15 +987,15 @@
     mock_get_existing_app_pkg_info.side_effect = (
         side_effects_for_get_existing_app_pkg_info
     )
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     teardown_processor = _get_na_teardown_processor()
     teardown_processor.drop_package(auto_yes_param)
     teardown_processor.drop_package(auto_yes_param)
     teardown_processor.drop_package(auto_yes_param)
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_version_create_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-import unittest
+import os
 from textwrap import dedent
+from unittest import mock
 
+import pytest
 import typer
 from click import BadOptionUsage, ClickException
+from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.constants import SPECIAL_COMMENT
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationPackageDoesNotExistError,
 )
 from snowflake.cli.plugins.nativeapp.policy import (
     AllowAlwaysPolicy,
     AskAlwaysPolicy,
     DenyAlwaysPolicy,
 )
 from snowflake.cli.plugins.nativeapp.version.version_processor import (
     NativeAppVersionCreateProcessor,
 )
-from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.connector.cursor import DictCursor
 
-from tests.nativeapp.utils import *
-from tests.testing_utils.fixtures import *
+from tests.nativeapp.utils import (
+    FIND_VERSION_FROM_MANIFEST,
+    NATIVEAPP_MANAGER_EXECUTE,
+    TYPER_CONFIRM,
+    VERSION_MODULE,
+    mock_execute_helper,
+    mock_snowflake_yml_file,
+)
+from tests.testing_utils.files_and_dirs import create_named_file
 
 CREATE_PROCESSOR = "NativeAppVersionCreateProcessor"
 
 allow_always_policy = AllowAlwaysPolicy()
 ask_always_policy = AskAlwaysPolicy()
 deny_always_policy = DenyAlwaysPolicy()
 
 
 def _get_version_create_processor():
     dm = DefinitionManager()
     return NativeAppVersionCreateProcessor(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 # Test get_existing_release_directive_info_for_version returns release directives info correctly
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 def test_get_existing_release_direction_info(mock_execute, temp_dir, mock_cursor):
@@ -65,15 +74,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     result = processor.get_existing_release_directive_info_for_version(version)
     assert mock_execute.mock_calls == expected
     assert len(result) == 2
@@ -107,15 +116,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.add_new_version(version)
     assert mock_execute.mock_calls == expected
 
@@ -148,15 +157,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.add_new_patch_to_version(version)
     assert mock_execute.mock_calls == expected
 
@@ -189,15 +198,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.add_new_patch_to_version(version, "12")
     assert mock_execute.mock_calls == expected
 
@@ -209,15 +218,15 @@
 )
 def test_process_no_version_from_user_no_version_in_manifest(
     mock_version_info_in_manifest, policy_param, temp_dir
 ):
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     with pytest.raises(ClickException):
         processor.process(
             version=None,
@@ -238,15 +247,15 @@
 )
 def test_process_no_version_exists_throws_bad_option_exception_one(
     mock_existing_version_info, policy_param, temp_dir
 ):
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     with pytest.raises(BadOptionUsage):
         processor.process(
             version="v1",
@@ -267,15 +276,15 @@
 )
 def test_process_no_version_exists_throws_bad_option_exception_two(
     mock_existing_version_info, policy_param, temp_dir
 ):
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     with pytest.raises(BadOptionUsage):
         processor.process(
             version="v1",
@@ -337,15 +346,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.process(
         version=version,
         patch=None,
@@ -425,15 +434,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.process(
         version=version,
         patch=12,
@@ -516,15 +525,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     with pytest.raises(typer.Exit):
         result = processor.process(
             version=version,
@@ -615,15 +624,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_create_processor()
     processor.process(
         version=version,
         patch=12,
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/test_version_drop_processor.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-import unittest
+import os
+from unittest import mock
 
+import pytest
 import typer
 from click import ClickException
+from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationPackageDoesNotExistError,
 )
 from snowflake.cli.plugins.nativeapp.policy import (
     AllowAlwaysPolicy,
     AskAlwaysPolicy,
     DenyAlwaysPolicy,
 )
 from snowflake.cli.plugins.nativeapp.version.version_processor import (
     NativeAppVersionDropProcessor,
 )
-from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.connector.cursor import DictCursor
 
 from tests.nativeapp.patch_utils import mock_get_app_pkg_distribution_in_sf
-from tests.nativeapp.utils import *
-from tests.testing_utils.fixtures import *
+from tests.nativeapp.utils import (
+    FIND_VERSION_FROM_MANIFEST,
+    NATIVEAPP_MANAGER_EXECUTE,
+    TYPER_CONFIRM,
+    VERSION_MODULE,
+    mock_execute_helper,
+    mock_snowflake_yml_file,
+)
+from tests.testing_utils.files_and_dirs import create_named_file
 
 DROP_PROCESSOR = "NativeAppVersionDropProcessor"
 
 allow_always_policy = AllowAlwaysPolicy()
 ask_always_policy = AskAlwaysPolicy()
 deny_always_policy = DenyAlwaysPolicy()
 
 
 def _get_version_drop_processor():
     dm = DefinitionManager()
 
     return NativeAppVersionDropProcessor(
-        project_definition=dm.project_definition["native_app"],
+        project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 # Test version drop process when there is no existing application package
 @mock.patch(
     f"{VERSION_MODULE}.{DROP_PROCESSOR}.get_existing_app_pkg_info", return_value=None
@@ -44,15 +53,15 @@
     "policy_param", [allow_always_policy, ask_always_policy, deny_always_policy]
 )
 def test_process_has_no_existing_app_pkg(mock_get_existing, policy_param, temp_dir):
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_drop_processor()
     with pytest.raises(ApplicationPackageDoesNotExistError):
         processor.process(
             version="some_version", policy=policy_param, is_interactive=True
@@ -79,15 +88,15 @@
     temp_dir,
 ):
 
     mock_mismatch.return_Value = "internal"
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_drop_processor()
     with pytest.raises(ClickException):
         processor.process(
             version=None, policy=policy_param, is_interactive=True
@@ -129,15 +138,15 @@
     temp_dir,
 ):
 
     mock_mismatch.return_value = "internal"
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_drop_processor()
     with pytest.raises(typer.Exit):
         result = processor.process(
             version=None, policy=policy_param, is_interactive=is_interactive_param
@@ -198,15 +207,15 @@
         ]
     )
     mock_execute.side_effect = side_effects
 
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
-        dir=current_working_directory,
+        dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     processor = _get_version_drop_processor()
     processor.process(
         version=None, policy=policy_param, is_interactive=is_interactive_param
     )
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/utils.py` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 NATIVEAPP_MANAGER_EXECUTE_QUERIES = f"{NATIVEAPP_MANAGER}._execute_queries"
 NATIVEAPP_MANAGER_APP_PKG_DISTRIBUTION_IN_SF = (
     f"{NATIVEAPP_MANAGER}.get_app_pkg_distribution_in_snowflake"
 )
 NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME = (
     f"{NATIVEAPP_MANAGER}.verify_project_distribution"
 )
+NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO = (
+    f"{NATIVEAPP_MANAGER}.get_existing_app_pkg_info"
+)
 
 TEARDOWN_PROCESSOR_GET_EXISTING_APP_INFO = f"{TEARDOWN_PROCESSOR}.get_existing_app_info"
 TEARDOWN_PROCESSOR_GET_EXISTING_APP_PKG_INFO = (
     f"{TEARDOWN_PROCESSOR}.get_existing_app_pkg_info"
 )
 TEARDOWN_PROCESSOR_IS_CORRECT_OWNER = f"{TEARDOWN_MODULE}.ensure_correct_owner"
 TEARDOWN_PROCESSOR_DROP_GENERIC_OBJECT = f"{TEARDOWN_PROCESSOR}.drop_generic_object"
 
 RUN_PROCESSOR_GET_EXISTING_APP_INFO = f"{RUN_PROCESSOR}.get_existing_app_info"
-RUN_PROCESSOR_GET_EXISTING_APP_PKG_INFO = f"{RUN_PROCESSOR}.get_existing_app_pkg_info"
 
 FIND_VERSION_FROM_MANIFEST = f"{VERSION_MODULE}.find_version_info_in_manifest_file"
 
 mock_snowflake_yml_file = dedent(
     """\
         definition_version: 1
         native_app:
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/__snapshots__/test_commands.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr`

 * *Files 6% similar despite different names*

```diff
@@ -354,7 +354,32 @@
 # ---
 # name: test_init_no_template_success[with_spaces-init_args4]
   '''
   Snowflake Native App project demo_na_project has been created at: demo na project
   
   '''
 # ---
+# name: test_list_templates_no_options_success
+  '''
+  +------------------------------------------------------------------------------+
+  | template         | description                                               |
+  |------------------+-----------------------------------------------------------|
+  | basic            | This is the basic project template for a Snowflake Native |
+  |                  | App project. It contains minimal code meant to help you   |
+  |                  | set up your first application object in your account      |
+  |                  | quickly.                                                  |
+  | streamlit-java   | This is an example template for a Snowflake Native App    |
+  |                  | project which demonstrates the use of Java extension code |
+  |                  | and adding Streamlit code. This template is meant to      |
+  |                  | guide developers towards a possible project structure on  |
+  |                  | the basis of functionality, as well as to indicate the    |
+  |                  | contents of some common and useful files.                 |
+  | streamlit-python | This is an example template for a Snowflake Native App    |
+  |                  | project which demonstrates the use of Python extension    |
+  |                  | code and adding Streamlit code. This template is meant to |
+  |                  | guide developers towards a possible project structure on  |
+  |                  | the basis of functionality, as well as to indicate the    |
+  |                  | contents of some common and useful files.                 |
+  +------------------------------------------------------------------------------+
+  
+  '''
+# ---
```

### Comparing `snowflake_cli_labs-2.1.2/tests/nativeapp/__snapshots__/test_init.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/object/test_common.py` & `snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import Tuple
+
+import pytest
 from snowflake.cli.plugins.object.common import (
-    _parse_tag,
     Tag,
     TagError,
+    _parse_tag,
 )
-from typing import Tuple
-import pytest
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
         ("tag=value", ("tag", "value")),
         ("_underscore_start=value", ("_underscore_start", "value")),
```

### Comparing `snowflake_cli_labs-2.1.2/tests/object/test_object.py` & `snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 import pytest
-from snowflake.cli.api.constants import SUPPORTED_OBJECTS, OBJECT_TO_NAMES
-from snowflake.cli.plugins.object.commands import _scope_validate
 from click import ClickException
+from snowflake.cli.api.constants import OBJECT_TO_NAMES, SUPPORTED_OBJECTS
+from snowflake.cli.plugins.object.commands import _scope_validate
 
 
 @mock.patch("snowflake.connector.connect")
 @pytest.mark.parametrize(
     "object_type, expected",
     [
         ("compute-pool", "compute pools"),
@@ -25,14 +25,15 @@
         ("streamlit", "streamlits"),
         ("table", "tables"),
         ("task", "tasks"),
         ("user", "users"),
         ("warehouse", "warehouses"),
         ("view", "views"),
         ("image-repository", "image repositories"),
+        ("git-repository", "git repositories"),
     ],
 )
 def test_show(
     mock_connector, object_type, expected, mock_cursor, runner, snapshot, mock_ctx
 ):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
@@ -58,14 +59,15 @@
     ("stream", "stream_example"),
     ("streamlit", "streamlit_example"),
     ("table", "table_example"),
     ("task", "task_example"),
     ("user", "user_example"),
     ("warehouse", "warehouse_example"),
     ("view", "view_example"),
+    ("git-repository", "git_repository_example"),
 ]
 
 
 @mock.patch("snowflake.connector.connect")
 @pytest.mark.parametrize(
     "object_type, input_scope, input_name",
     [
```

### Comparing `snowflake_cli_labs-2.1.2/tests/object/__snapshots__/test_object.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,26 @@
   |------+-------------+--------|
   | ID   | NUMBER(38,0 | COLUMN |
   | NAME | VARCHAR(100 | COLUMN |
   +-----------------------------+
   
   '''
 # ---
+# name: test_describe[git-repository-git_repository_example]
+  '''
+  SELECT A MOCK QUERY
+  +-----------------------------+
+  | name | type        | kind   |
+  |------+-------------+--------|
+  | ID   | NUMBER(38,0 | COLUMN |
+  | NAME | VARCHAR(100 | COLUMN |
+  +-----------------------------+
+  
+  '''
+# ---
 # name: test_describe[integration-integration_example]
   '''
   SELECT A MOCK QUERY
   +-----------------------------+
   | name | type        | kind   |
   |------+-------------+--------|
   | ID   | NUMBER(38,0 | COLUMN |
@@ -252,14 +264,25 @@
   | status |
   |--------|
   | f      |
   +--------+
   
   '''
 # ---
+# name: test_drop[git-repository-git_repository_example]
+  '''
+  SELECT A MOCK QUERY
+  +--------+
+  | status |
+  |--------|
+  | g      |
+  +--------+
+  
+  '''
+# ---
 # name: test_drop[image-repository-image_repository_example]
   '''
   SELECT A MOCK QUERY
   +--------+
   | status |
   |--------|
   | i      |
```

### Comparing `snowflake_cli_labs-2.1.2/tests/object/stage/test_diff.py` & `snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import hashlib
-from typing import Dict, Tuple
+from pathlib import Path
+from typing import Dict, List, Tuple, Union
+from unittest import mock
 
+import pytest
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
-from snowflake.cli.plugins.object.stage.diff import (
+from snowflake.cli.plugins.stage.diff import (
     DiffResult,
     delete_only_on_stage_files,
     enumerate_files,
     get_stage_path_from_file,
     put_files_on_stage,
     stage_diff,
     sync_local_diff_with_stage,
 )
-from snowflake.cli.plugins.object.stage.manager import StageManager
+from snowflake.cli.plugins.stage.manager import StageManager
 
 from tests.testing_utils.files_and_dirs import temp_local_dir
-from tests.testing_utils.fixtures import *
 
-STAGE_MANAGER = "snowflake.cli.plugins.object.stage.manager.StageManager"
+STAGE_MANAGER = "snowflake.cli.plugins.stage.manager.StageManager"
 
 FILE_CONTENTS = {
     "README.md": "This is a README\n",
     "ui/streamlit.py": "# this is a streamlit\n",
     "my.jar": b"083hgia2r92tha",
 }
 DEFAULT_LAST_MODIFIED = "Tue, 5 Sep 2023 17:59:21 GMT"
 STAGE_LS_COLUMNS = ["name", "size", "md5", "last_modified"]
 
 
 def md5_of(contents: Union[str, bytes]) -> str:
-    hash = hashlib.md5()
+    hash_value = hashlib.md5()
     if isinstance(contents, bytes):
-        hash.update(contents)
+        hash_value.update(contents)
     else:
-        hash.update(contents.encode("UTF-8"))
-    return hash.hexdigest()
+        hash_value.update(contents.encode("UTF-8"))
+    return hash_value.hexdigest()
 
 
 def stage_contents(
     files: Dict[str, Union[str, bytes]], last_modified: str = DEFAULT_LAST_MODIFIED
 ) -> List[Tuple[str, int, str, str]]:
     """
     Return file contents as they would be listed by a SNOWFLAKE_SSE stage
@@ -179,15 +181,15 @@
             files=["ui/nested/environment.yml", "README.md"],
             role="some_role",
             overwrite=overwrite_param,
         )
         expected = [
             mock.call(
                 local_path=local_path / "ui/nested/environment.yml",
-                stage_path=f"{stage_name}/ui/nested",  # TODO: verify if trailing slash is needed, doesnt seem so from regression tests
+                stage_path=f"{stage_name}/ui/nested",  # TODO: verify if trailing slash is needed, doesn't seem so from regression tests
                 role="some_role",
                 overwrite=overwrite_param,
             ),
             mock.call(
                 local_path=local_path / "README.md",
                 stage_path=f"{stage_name}",
                 role="some_role",
```

### Comparing `snowflake_cli_labs-2.1.2/tests/object/stage/test_stage.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,435 +1,480 @@
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from unittest import mock
+import json
+from unittest.mock import Mock, patch
 
 import pytest
-from snowflake.cli.plugins.object.stage.manager import StageManager
-from snowflake.connector.cursor import DictCursor
-
-STAGE_MANAGER = "snowflake.cli.plugins.object.stage.manager.StageManager"
-
-
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_list(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "stage", "list", "-c", "empty", "stageName"])
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("ls @stageName")
+from click import ClickException
+from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.api.project.util import to_string_literal
+from snowflake.cli.plugins.spcs.common import (
+    NoPropertiesProvidedError,
+)
+from snowflake.cli.plugins.spcs.compute_pool.commands import _compute_pool_name_callback
+from snowflake.cli.plugins.spcs.compute_pool.manager import ComputePoolManager
+from snowflake.connector.cursor import SnowflakeCursor
+
+from tests.spcs.test_common import SPCS_OBJECT_EXISTS_ERROR
+from tests_integration.testing_utils.assertions.test_result_assertions import (
+    assert_that_result_is_successful_and_executed_successfully,
+)
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_list_quoted(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "stage", "list", "-c", "empty", '"stage name"'])
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("ls '@\"stage name\"'")
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_create(mock_execute_query):
+    pool_name = "test_pool"
+    min_nodes = 2
+    max_nodes = 3
+    instance_family = "test_family"
+    auto_resume = True
+    initially_suspended = False
+    auto_suspend_secs = 7200
+    comment = "'test comment'"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().create(
+        pool_name=pool_name,
+        min_nodes=min_nodes,
+        max_nodes=max_nodes,
+        instance_family=instance_family,
+        auto_resume=auto_resume,
+        initially_suspended=initially_suspended,
+        auto_suspend_secs=auto_suspend_secs,
+        comment=comment,
+        if_not_exists=False,
+    )
+    expected_query = " ".join(
+        [
+            "CREATE COMPUTE POOL test_pool",
+            "MIN_NODES = 2",
+            "MAX_NODES = 3",
+            "INSTANCE_FAMILY = test_family",
+            "AUTO_RESUME = True",
+            "INITIALLY_SUSPENDED = False",
+            "AUTO_SUSPEND_SECS = 7200",
+            "COMMENT = 'test comment'",
+        ]
+    )
+    actual_query = " ".join(mock_execute_query.mock_calls[0].args[0].split())
+    assert expected_query == actual_query
+    assert result == cursor
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_remote_to_local(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(
-            ["object", "stage", "copy", "-c", "empty", "@stageName", str(tmp_dir)]
-        )
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.create")
+def test_create_pool_cli_defaults(mock_create, runner):
+    result = runner.invoke(
+        [
+            "spcs",
+            "compute-pool",
+            "create",
+            "test_pool",
+            "--family",
+            "test_family",
+        ]
+    )
     assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"get @stageName file://{Path(tmp_dir).resolve()}/ parallel=4"
+    mock_create.assert_called_once_with(
+        pool_name="test_pool",
+        min_nodes=1,
+        max_nodes=1,
+        instance_family="test_family",
+        auto_resume=True,
+        initially_suspended=False,
+        auto_suspend_secs=3600,
+        comment=None,
+        if_not_exists=False,
     )
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_remote_to_local_quoted_stage(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(
-            ["object", "stage", "copy", "-c", "empty", '@"stage name"', str(tmp_dir)]
-        )
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.create")
+def test_create_pool_cli(mock_create, runner):
+    result = runner.invoke(
+        [
+            "spcs",
+            "compute-pool",
+            "create",
+            "test_pool",
+            "--min-nodes",
+            "2",
+            "--max-nodes",
+            "3",
+            "--family",
+            "test_family",
+            "--no-auto-resume",
+            "--init-suspend",
+            "--auto-suspend-secs",
+            "7200",
+            "--comment",
+            "this is a test",
+            "--if-not-exists",
+        ]
+    )
     assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"get '@\"stage name\"' file://{Path(tmp_dir).resolve()}/ parallel=4"
+    mock_create.assert_called_once_with(
+        pool_name="test_pool",
+        min_nodes=2,
+        max_nodes=3,
+        instance_family="test_family",
+        auto_resume=False,
+        initially_suspended=True,
+        auto_suspend_secs=7200,
+        comment=to_string_literal("this is a test"),
+        if_not_exists=True,
     )
 
 
-@pytest.mark.parametrize(
-    "raw_path,expected_uri",
-    [
-        ("{}/dest", "file://{}/dest/"),
-        ("{}/dest.dir", "file://{}/dest.dir/"),
-        ("{}/dest0", "file://{}/dest0/"),
-        ("{}/dest dir", "'file://{}/dest dir/'"),
-        ("{}/dest#dir", "file://{}/dest#dir/"),
-        ("{}/dest*dir", "file://{}/dest*dir/"),
-        ("{}/dest_?dir", "file://{}/dest_?dir/"),
-        ("{}/dest%dir", "file://{}/dest%dir/"),
-        ('{}/dest"dir', 'file://{}/dest"dir/'),
-        ("{}/dest'dir", r"'file://{}/dest\'dir/'"),
-        ("{}/dest\tdir", r"'file://{}/dest\tdir/'"),
-    ],
-)
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_remote_to_local_quoted_uri(
-    mock_execute, runner, mock_cursor, raw_path, expected_uri
-):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        tmp_dir = Path(tmp_dir).resolve()
-        local_path = raw_path.replace("{}", str(tmp_dir))
-        file_uri = expected_uri.replace("{}", str(tmp_dir))
-        result = runner.invoke(
-            ["object", "stage", "copy", "-c", "empty", "@stageName", local_path]
-        )
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(f"get @stageName {file_uri} parallel=4")
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.handle_object_already_exists")
+def test_create_compute_pool_already_exists(mock_handle, mock_execute):
+    pool_name = "test_pool"
+    mock_execute.side_effect = SPCS_OBJECT_EXISTS_ERROR
+    ComputePoolManager().create(
+        pool_name=pool_name,
+        min_nodes=1,
+        max_nodes=1,
+        instance_family="test_family",
+        auto_resume=False,
+        initially_suspended=True,
+        auto_suspend_secs=7200,
+        comment=to_string_literal("this is a test"),
+        if_not_exists=False,
+    )
+    mock_handle.assert_called_once_with(
+        SPCS_OBJECT_EXISTS_ERROR, ObjectType.COMPUTE_POOL, pool_name
+    )
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_local_to_remote(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(
-            [
-                "object",
-                "stage",
-                "copy",
-                "-c",
-                "empty",
-                "--overwrite",
-                "--parallel",
-                42,
-                str(tmp_dir),
-                "@stageName",
-            ]
-        )
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"put file://{Path(tmp_dir).resolve()}/* @stageName auto_compress=false parallel=42 overwrite=True"
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_create_compute_pool_if_not_exists(mock_execute_query):
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().create(
+        pool_name="test_pool",
+        min_nodes=1,
+        max_nodes=1,
+        instance_family="test_family",
+        auto_resume=True,
+        initially_suspended=False,
+        auto_suspend_secs=3600,
+        comment=None,
+        if_not_exists=True,
     )
+    expected_query = " ".join(
+        [
+            "CREATE COMPUTE POOL IF NOT EXISTS test_pool",
+            "MIN_NODES = 1",
+            "MAX_NODES = 1",
+            "INSTANCE_FAMILY = test_family",
+            "AUTO_RESUME = True",
+            "INITIALLY_SUSPENDED = False",
+            "AUTO_SUSPEND_SECS = 3600",
+        ]
+    )
+    actual_query = " ".join(mock_execute_query.mock_calls[0].args[0].split())
+    assert expected_query == actual_query
+    assert result == cursor
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_local_to_remote_quoted_stage(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(
-            [
-                "object",
-                "stage",
-                "copy",
-                "-c",
-                "empty",
-                "--overwrite",
-                "--parallel",
-                42,
-                str(tmp_dir),
-                '@"stage name"',
-            ]
-        )
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"put file://{Path(tmp_dir).resolve()}/* '@\"stage name\"' auto_compress=false parallel=42 overwrite=True"
-    )
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_stop(mock_execute_query):
+    pool_name = "test_pool"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().stop(pool_name)
+    expected_query = "alter compute pool test_pool stop all"
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
 
 
-@pytest.mark.parametrize(
-    "raw_path,expected_uri",
-    [
-        ("{}/readme.md", "file://{}/readme.md"),
-        ("{}/readme0.md", "file://{}/readme0.md"),
-        ("{}/read me.md", "'file://{}/read me.md'"),
-        ("{}/read#me.md", "file://{}/read#me.md"),
-        ("{}/read*.md", "file://{}/read*.md"),
-        ("{}/read_?me.md", "file://{}/read_?me.md"),
-        ("{}/read%me.md", "file://{}/read%me.md"),
-        ('{}/read"me.md', 'file://{}/read"me.md'),
-        ("{}/read'me.md", r"'file://{}/read\'me.md'"),
-        ("{}/read\tme.md", r"'file://{}/read\tme.md'"),
-    ],
-)
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_local_to_remote_quoted_path(
-    mock_execute, runner, mock_cursor, raw_path, expected_uri
-):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        tmp_dir = Path(tmp_dir).resolve()
-        local_path = raw_path.replace("{}", str(tmp_dir))
-        file_uri = expected_uri.replace("{}", str(tmp_dir))
-
-        result = runner.invoke(
-            [
-                "object",
-                "stage",
-                "copy",
-                "-c",
-                "empty",
-                "--overwrite",
-                "--parallel",
-                42,
-                local_path,
-                "@stageName",
-            ]
-        )
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"put {file_uri} @stageName auto_compress=false parallel=42 overwrite=True"
-    )
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_suspend(mock_execute_query):
+    pool_name = "test_pool"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().suspend(pool_name)
+    expected_query = "alter compute pool test_pool suspend"
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_copy_local_to_remote_star(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(
-            [
-                "object",
-                "stage",
-                "copy",
-                "-c",
-                "empty",
-                "--overwrite",
-                "--parallel",
-                42,
-                str(tmp_dir) + "/*.py",
-                "@stageName",
-            ]
-        )
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.suspend")
+def test_suspend_cli(mock_suspend, mock_cursor, runner):
+    pool_name = "test_pool"
+    cursor = mock_cursor(
+        rows=[["Statement executed successfully."]], columns=["status"]
+    )
+    mock_suspend.return_value = cursor
+    result = runner.invoke(["spcs", "compute-pool", "suspend", pool_name])
+    mock_suspend.assert_called_once_with(pool_name)
     assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with(
-        f"put file://{Path(tmp_dir).resolve()}/*.py @stageName auto_compress=false parallel=42 overwrite=True"
+    assert "Statement executed successfully" in result.output
+
+    cursor_copy = mock_cursor(
+        rows=[["Statement executed successfully."]], columns=["status"]
+    )
+    mock_suspend.return_value = cursor_copy
+    result_json = runner.invoke(
+        ["spcs", "compute-pool", "suspend", pool_name, "--format", "json"]
     )
+    result_json_parsed = json.loads(result_json.output)
+    assert isinstance(result_json_parsed, dict)
+    assert result_json_parsed == {"status": "Statement executed successfully."}
 
 
-@pytest.mark.parametrize(
-    "source, dest",
-    [
-        ("@snow/stage", "@stage/snow"),
-        ("snow://stage", "snow://stage/snow"),
-        ("local/path", "other/local/path"),
-    ],
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
 )
-def test_copy_throws_error_for_same_platform_operation(runner, source, dest, snapshot):
-    result = runner.invoke(["object", "stage", "copy", source, dest])
-    assert result.exit_code == 1
-    assert result.output == snapshot
+def test_resume(mock_execute_query):
+    pool_name = "test_pool"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().resume(pool_name)
+    expected_query = "alter compute pool test_pool resume"
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_create(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "stage", "create", "-c", "empty", "stageName"])
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.resume")
+def test_resume_cli(mock_resume, mock_cursor, runner):
+    pool_name = "test_pool"
+    cursor = mock_cursor(
+        rows=[["Statement executed successfully."]], columns=["status"]
+    )
+    mock_resume.return_value = cursor
+    result = runner.invoke(["spcs", "compute-pool", "resume", pool_name])
+    mock_resume.assert_called_once_with(pool_name)
     assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("create stage if not exists stageName")
+    assert "Statement executed successfully" in result.output
 
+    cursor_copy = mock_cursor(
+        rows=[["Statement executed successfully."]], columns=["status"]
+    )
+    mock_resume.return_value = cursor_copy
+    result_json = runner.invoke(
+        ["spcs", "compute-pool", "resume", pool_name, "--format", "json"]
+    )
+    result_json_parsed = json.loads(result_json.output)
+    assert isinstance(result_json_parsed, dict)
+    assert result_json_parsed == {"status": "Statement executed successfully."}
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_create_quoted(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "stage", "create", "-c", "empty", '"stage name"'])
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with('create stage if not exists "stage name"')
 
+@patch("snowflake.cli.plugins.spcs.compute_pool.commands.is_valid_object_name")
+def test_compute_pool_name_callback(mock_is_valid):
+    name = "test_pool"
+    mock_is_valid.return_value = True
+    assert _compute_pool_name_callback(name) == name
 
-@mock.patch("snowflake.cli.plugins.object.commands.ObjectManager._execute_query")
-def test_stage_drop(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "drop", "stage", "stageName", "-c", "empty"])
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("drop stage stageName")
 
+@patch("snowflake.cli.plugins.spcs.compute_pool.commands.is_valid_object_name")
+def test_compute_pool_name_callback_invalid(mock_is_valid):
+    name = "test_pool"
+    mock_is_valid.return_value = False
+    with pytest.raises(ClickException) as e:
+        _compute_pool_name_callback(name)
+    assert "is not a valid compute pool name." in e.value.message
 
-@mock.patch("snowflake.cli.plugins.object.commands.ObjectManager._execute_query")
-def test_stage_drop_quoted(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(["object", "drop", "stage", '"stage name"', "-c", "empty"])
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with('drop stage "stage name"')
 
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_set_property(mock_execute_query):
+    pool_name = "test_pool"
+    min_nodes = 2
+    max_nodes = 3
+    auto_resume = False
+    auto_suspend_secs = 7200
+    comment = to_string_literal("this is a test")
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().set_property(
+        pool_name, min_nodes, max_nodes, auto_resume, auto_suspend_secs, comment
+    )
+    expected_query = "\n".join(
+        [
+            f"alter compute pool {pool_name} set",
+            f"min_nodes = {min_nodes}",
+            f"max_nodes = {max_nodes}",
+            f"auto_resume = {auto_resume}",
+            f"auto_suspend_secs = {auto_suspend_secs}",
+            f"comment = {comment}",
+        ]
+    )
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_remove(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
-    result = runner.invoke(
-        ["object", "stage", "remove", "-c", "empty", "stageName", "my/file/foo.csv"]
+
+def test_set_property_no_properties():
+    pool_name = "test_pool"
+    with pytest.raises(NoPropertiesProvidedError) as e:
+        ComputePoolManager().set_property(pool_name, None, None, None, None, None)
+    assert (
+        e.value.message
+        == f"No properties specified for compute pool '{pool_name}'. Please provide at least one property to set."
     )
-    assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("remove @stageName/my/file/foo.csv")
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_remove_quoted(mock_execute, runner, mock_cursor):
-    mock_execute.return_value = mock_cursor(["row"], [])
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.set_property"
+)
+def test_set_property_cli(mock_set, mock_statement_success, runner):
+    cursor = mock_statement_success()
+    mock_set.return_value = cursor
+    pool_name = "test_pool"
+    min_nodes = 2
+    max_nodes = 3
+    auto_resume = False
+    auto_suspend_secs = 7200
+    comment = "this is a test"
     result = runner.invoke(
-        ["object", "stage", "remove", "-c", "empty", '"stage name"', "my/file/foo.csv"]
+        [
+            "spcs",
+            "compute-pool",
+            "set",
+            pool_name,
+            "--min-nodes",
+            str(min_nodes),
+            "--max-nodes",
+            str(max_nodes),
+            "--no-auto-resume",
+            "--auto-suspend-secs",
+            auto_suspend_secs,
+            "--comment",
+            comment,
+        ]
+    )
+    mock_set.assert_called_once_with(
+        pool_name=pool_name,
+        min_nodes=min_nodes,
+        max_nodes=max_nodes,
+        auto_resume=auto_resume,
+        auto_suspend_secs=auto_suspend_secs,
+        comment=to_string_literal(comment),
     )
     assert result.exit_code == 0, result.output
-    mock_execute.assert_called_once_with("remove '@\"stage name\"/my/file/foo.csv'")
+    assert "Statement executed successfully" in result.output
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_print_result_for_put_directory(
-    mock_execute, mock_cursor, runner, snapshot
-):
-    mock_execute.return_value = mock_cursor(
-        rows=[
-            ["file1.txt", "file1.txt", 10, 8, "NONE", "NONE", "UPLOADED", ""],
-            ["file2.txt", "file2.txt", 10, 8, "NONE", "NONE", "UPLOADED", ""],
-            ["file3.txt", "file3.txt", 10, 8, "NONE", "NONE", "UPLOADED", ""],
-        ],
-        columns=[
-            "source",
-            "target",
-            "source_size",
-            "target_size",
-            "source_compression",
-            "target_compression",
-            "status",
-            "message",
-        ],
-    )
-
-    with TemporaryDirectory() as tmp_dir:
-        tmp_dir_path = Path(tmp_dir)
-        (tmp_dir_path / "file1.txt").touch()
-        (tmp_dir_path / "file2.txt").touch()
-        (tmp_dir_path / "file3.txt").touch()
-        result = runner.invoke(["object", "stage", "copy", tmp_dir, "@stageName"])
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.set_property"
+)
+def test_set_property_no_properties_cli(mock_set, runner):
+    pool_name = "test_pool"
+    mock_set.side_effect = NoPropertiesProvidedError(
+        f"No properties specified for compute pool '{pool_name}'. Please provide at least one property to set."
+    )
+    result = runner.invoke(["spcs", "compute-pool", "set", pool_name])
+    assert result.exit_code == 1, result.output
+    assert "No properties specified" in result.output
+    mock_set.assert_called_once_with(
+        pool_name=pool_name,
+        min_nodes=None,
+        max_nodes=None,
+        auto_resume=None,
+        auto_suspend_secs=None,
+        comment=None,
+    )
 
-    assert result.exit_code == 0, result.output
-    assert result.output == snapshot
+
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_unset_property(mock_execute_query):
+    pool_name = "test_pool"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().unset_property(pool_name, True, True, True)
+    expected_query = (
+        "alter compute pool test_pool unset auto_resume,auto_suspend_secs,comment"
+    )
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_print_result_for_get_all_files_from_stage(
-    mock_execute, mock_cursor, runner, snapshot
-):
-    mock_execute.return_value = mock_cursor(
-        rows=[
-            ["file1.txt", 10, "DOWNLOADED", ""],
-            ["file2.txt", 10, "DOWNLOADED", ""],
-            ["file3.txt", 10, "DOWNLOADED", ""],
-        ],
-        columns=[
-            "file",
-            "size",
-            "status",
-            "message",
-        ],
+def test_unset_property_no_properties():
+    pool_name = "test_pool"
+    with pytest.raises(NoPropertiesProvidedError) as e:
+        ComputePoolManager().unset_property(pool_name, False, False, False)
+    assert (
+        e.value.message
+        == f"No properties specified for compute pool '{pool_name}'. Please provide at least one property to reset to its default value."
     )
 
-    with TemporaryDirectory() as tmp_dir:
-        result = runner.invoke(["object", "stage", "copy", "@stageName", tmp_dir])
 
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.unset_property"
+)
+def test_unset_property_cli(mock_unset, mock_statement_success, runner):
+    cursor = mock_statement_success()
+    mock_unset.return_value = cursor
+    pool_name = "test_pool"
+    result = runner.invoke(
+        [
+            "spcs",
+            "compute-pool",
+            "unset",
+            pool_name,
+            "--auto-resume",
+            "--auto-suspend-secs",
+            "--comment",
+        ]
+    )
+    mock_unset.assert_called_once_with(
+        pool_name=pool_name, auto_resume=True, auto_suspend_secs=True, comment=True
+    )
     assert result.exit_code == 0, result.output
-    assert result.output == snapshot
+    assert "Statement executed successfully" in result.output
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_remove(mock_execute, mock_cursor):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    sm = StageManager()
-    sm.remove("stageName", "my/file/foo.csv", "new_role")
-    expected = [
-        mock.call("select current_role()", cursor_class=DictCursor),
-        mock.call("use role new_role"),
-        mock.call("remove @stageName/my/file/foo.csv"),
-        mock.call("use role old_role"),
-    ]
-    assert mock_execute.mock_calls == expected
-
-
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_remove_quoted(mock_execute, mock_cursor):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    sm = StageManager()
-    sm.remove('"stage name"', "my/file/foo.csv", "new_role")
-    expected = [
-        mock.call("select current_role()", cursor_class=DictCursor),
-        mock.call("use role new_role"),
-        mock.call("remove '@\"stage name\"/my/file/foo.csv'"),
-        mock.call("use role old_role"),
-    ]
-    assert mock_execute.mock_calls == expected
-
-
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_remove_no_role_change(mock_execute, mock_cursor):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    sm = StageManager()
-    sm.remove("stageName", "my/file/foo.csv", "old_role")
-    expected = [
-        mock.call("select current_role()", cursor_class=DictCursor),
-        mock.call("remove @stageName/my/file/foo.csv"),
-    ]
-    assert mock_execute.mock_calls == expected
-
-
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_put(mock_execute, mock_cursor):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    with TemporaryDirectory() as tmp_dir:
-        sm = StageManager()
-        sm.put(Path(tmp_dir).resolve(), "stageName", role="new_role")
-        expected = [
-            mock.call("select current_role()", cursor_class=DictCursor),
-            mock.call("use role new_role"),
-            mock.call(
-                f"put file://{Path(tmp_dir).resolve()} @stageName auto_compress=false parallel=4 overwrite=False"
-            ),
-            mock.call("use role old_role"),
-        ]
-        assert mock_execute.mock_calls == expected
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.unset_property"
+)
+def test_unset_property_no_properties_cli(mock_unset, runner):
+    pool_name = "test_pool"
+    mock_unset.side_effect = NoPropertiesProvidedError(
+        f"No properties specified for compute pool '{pool_name}'. Please provide at least one property to reset to its default value."
+    )
+    result = runner.invoke(["spcs", "compute-pool", "unset", pool_name])
+    assert result.exit_code == 1, result.output
+    assert "No properties specified" in result.output
+    mock_unset.assert_called_once_with(
+        pool_name=pool_name, auto_resume=False, auto_suspend_secs=False, comment=False
+    )
 
 
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_put_quoted_stage(mock_execute, mock_cursor):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    with TemporaryDirectory() as tmp_dir:
-        sm = StageManager()
-        sm.put(Path(tmp_dir).resolve(), '"stage name"', role="new_role")
-        expected = [
-            mock.call("select current_role()", cursor_class=DictCursor),
-            mock.call("use role new_role"),
-            mock.call(
-                f"put file://{Path(tmp_dir).resolve()} '@\"stage name\"' auto_compress=false parallel=4 overwrite=False"
-            ),
-            mock.call("use role old_role"),
-        ]
-        assert mock_execute.mock_calls == expected
+def test_unset_property_with_args(runner):
+    pool_name = "test_pool"
+    result = runner.invoke(
+        ["spcs", "compute-pool", "unset", pool_name, "--auto-suspend-secs", "1"]
+    )
+    assert result.exit_code == 2, result.output
+    assert "Got unexpected extra argument" in result.output
 
 
-@pytest.mark.parametrize(
-    "raw_path,expected_uri",
-    [
-        ("{}/readme.md", "file://{}/readme.md"),
-        ("{}/readme0.md", "file://{}/readme0.md"),
-        ("{}/read me.md", "'file://{}/read me.md'"),
-        ("{}/read#me.md", "file://{}/read#me.md"),
-        ("{}/read*.md", "file://{}/read*.md"),
-        ("{}/read_?me.md", "file://{}/read_?me.md"),
-        ("{}/read%me.md", "file://{}/read%me.md"),
-        ('{}/read"me.md', 'file://{}/read"me.md'),
-        ("{}/read'me.md", r"'file://{}/read\'me.md'"),
-        ("{}/read\tme.md", r"'file://{}/read\tme.md'"),
-    ],
-)
-@mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_stage_internal_put_quoted_path(
-    mock_execute, mock_cursor, raw_path, expected_uri
-):
-    mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    with TemporaryDirectory() as tmp_dir:
-        sm = StageManager()
-        tmp_dir = Path(tmp_dir).resolve()
-        src_path = raw_path.replace("{}", str(tmp_dir))
-        src_uri = expected_uri.replace("{}", str(tmp_dir))
-        sm.put(src_path, "stageName", role="new_role")
-        expected = [
-            mock.call("select current_role()", cursor_class=DictCursor),
-            mock.call("use role new_role"),
-            mock.call(
-                f"put {src_uri} @stageName auto_compress=false parallel=4 overwrite=False"
-            ),
-            mock.call("use role old_role"),
-        ]
-        assert mock_execute.mock_calls == expected
+@patch(
+    "snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager._execute_query"
+)
+def test_status(mock_execute_query):
+    pool_name = "test_pool"
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    result = ComputePoolManager().status(pool_name=pool_name)
+    expected_query = f"call system$get_compute_pool_status('{pool_name}')"
+    mock_execute_query.assert_called_once_with(expected_query)
+    assert result == cursor
+
+
+@patch("snowflake.cli.plugins.spcs.compute_pool.manager.ComputePoolManager.status")
+def test_status_cli(mock_status, mock_statement_success, runner):
+    pool_name = "test_pool"
+    mock_status.return_value = mock_statement_success()
+    result = runner.invoke(["spcs", "compute-pool", "status", pool_name])
+    mock_status.assert_called_once_with(pool_name=pool_name)
+    assert_that_result_is_successful_and_executed_successfully(result)
```

### Comparing `snowflake_cli_labs-2.1.2/tests/output/test_format_silent_enforcement.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/output/test_printing.py` & `snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from datetime import datetime
 from textwrap import dedent
+from typing import NamedTuple
 
+import pytest
 from snowflake.cli.api.output.formats import OutputFormat
 from snowflake.cli.api.output.types import (
     CollectionResult,
     MessageResult,
     MultipleResults,
     ObjectResult,
     QueryResult,
     SingleQueryResult,
 )
 from snowflake.cli.app.printing import print_result
 
 from tests.testing_utils.conversion import get_output, get_output_as_json
-from tests.testing_utils.fixtures import *
 
 
 class MockResultMetadata(NamedTuple):
     name: str
 
 
 def test_single_value_from_query(capsys, mock_cursor):
```

### Comparing `snowflake_cli_labs-2.1.2/tests/plugin/test_broken_plugin.py` & `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     result = runner.invoke(["--config-file", config_path, "connection", "list"])
 
     assert (
         caplog.messages[0]
         == "Cannot register plugin [broken_plugin]: Invalid command path [snow broken run]. Command group [broken] does not exist."
     )
     assert result.output == dedent(
-        """+---------------------------------------+
-| connection_name | parameters          |
-|-----------------+---------------------|
-| test            | {'account': 'test'} |
-+---------------------------------------+
+        """\
+     +----------------------------------------------------+
+     | connection_name | parameters          | is_default |
+     |-----------------+---------------------+------------|
+     | test            | {'account': 'test'} | False      |
+     +----------------------------------------------------+
     """
     )
 
 
 @pytest.fixture(scope="module")
 def _install_plugin(test_root_path):
     import subprocess
```

### Comparing `snowflake_cli_labs-2.1.2/tests/plugin/test_failing_plugin.py` & `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,58 @@
 from textwrap import dedent
 
 import pytest
 
 
-def test_failing_plugin(runner, test_root_path, _install_plugin, caplog):
+def test_override_build_in_commands(runner, test_root_path, _install_plugin, caplog):
     config_path = (
-        test_root_path / "test_data" / "configs" / "failing_plugin_config.toml"
+        test_root_path / "test_data" / "configs" / "override_plugin_config.toml"
     )
 
     result = runner.invoke(["--config-file", config_path, "connection", "list"])
 
     assert (
         caplog.messages[0]
-        == "Cannot register plugin [failing_plugin]: Some error in plugin"
+        == "Cannot register plugin [override]: Cannot add command [snow connection list] because it already exists."
     )
     assert result.output == dedent(
-        """+---------------------------------------+
-| connection_name | parameters          |
-|-----------------+---------------------|
-| test            | {'account': 'test'} |
-+---------------------------------------+
+        """\
+     Outside command code
+     +----------------------------------------------------+
+     | connection_name | parameters          | is_default |
+     |-----------------+---------------------+------------|
+     | test            | {'account': 'test'} | False      |
+     +----------------------------------------------------+
+    """
+    )
+
+
+def test_disabled_plugin_is_not_executed(
+    runner, test_root_path, _install_plugin, caplog
+):
+    config_path = (
+        test_root_path
+        / "test_data"
+        / "configs"
+        / "disabled_override_plugin_config.toml"
+    )
+
+    result = runner.invoke(["--config-file", config_path, "connection", "list"])
+
+    assert len(caplog.messages) == 0
+    assert result.output == dedent(
+        """\
+     +----------------------------------------------------+
+     | connection_name | parameters          | is_default |
+     |-----------------+---------------------+------------|
+     | test            | {'account': 'test'} | False      |
+     +----------------------------------------------------+
     """
     )
 
 
 @pytest.fixture(scope="module")
 def _install_plugin(test_root_path):
     import subprocess
 
-    path = test_root_path / ".." / "test_external_plugins" / "failing_plugin"
+    path = test_root_path / ".." / "test_external_plugins" / "override_build_in_command"
     subprocess.check_call(["pip", "install", path])
```

### Comparing `snowflake_cli_labs-2.1.2/tests/project/fixtures.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     """
     Returns paths to [snowflake_yml, (snowflake_local_yml)].
     These files are temporary copies of the project definition found in
     dir_name and will be deleted when this context manager goes out-of-scope.
     These files reside alongside any other files in the project directory.
     If there is no local overrides file, returns a list of length 1.
     """
-    with temp_cloned_dir(PROJECT_DIR / dir_name) as dir:
-        project_yml = dir / "snowflake.yml"
-        local_yml = dir / "snowflake.local.yml"
+    with temp_cloned_dir(PROJECT_DIR / dir_name) as dir_:
+        project_yml = dir_ / "snowflake.yml"
+        local_yml = dir_ / "snowflake.local.yml"
         if local_yml.exists():
             yield [project_yml, local_yml]
         else:
             yield [project_yml]
 
 
 @pytest.fixture
```

### Comparing `snowflake_cli_labs-2.1.2/tests/project/test_definition_manager.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from pathlib import Path
 from unittest import TestCase, mock
-from unittest.mock import patch
 
+import pytest
 from snowflake.cli.api.exceptions import MissingConfiguration
 from snowflake.cli.api.project.definition_manager import DefinitionManager
 
-from tests.project.fixtures import *
-from tests.testing_utils.fixtures import *
-
 
 def mock_is_file_for(*known_files):
     def fake_is_file(self):
         return str(self) in known_files
 
     return mock.patch.object(Path, "is_file", autospec=True, side_effect=fake_is_file)
 
@@ -19,25 +16,25 @@
 class DefinitionManagerTest(TestCase):
     exception_message = "Cannot find project definition (snowflake.yml). Please provide a path to the project or run this command in a valid project directory."
 
     @mock.patch("os.getcwd", return_value="/hello/world")
     def test_no_project_parameter_provided(self, mock_getcwd):
         with mock_is_file_for("/hello/world/snowflake.yml") as mock_is_file:
             definition_manager = DefinitionManager()
-            assert definition_manager._project_config_paths == [
+            assert definition_manager._project_config_paths == [  # noqa: SLF001
                 Path("/hello/world/snowflake.yml")
             ]
 
     @mock.patch("os.getcwd", return_value="/hello/world")
     def test_finds_local_project_definition(self, mock_getcwd):
         with mock_is_file_for(
             "/hello/world/snowflake.yml", "/hello/world/snowflake.local.yml"
         ) as mock_is_file:
             definition_manager = DefinitionManager()
-            assert definition_manager._project_config_paths == [
+            assert definition_manager._project_config_paths == [  # noqa: SLF001
                 Path("/hello/world/snowflake.yml"),
                 Path("/hello/world/snowflake.local.yml"),
             ]
 
     @mock.patch("os.path.abspath", return_value="/hello/world/test")
     def test_double_dash_project_parameter_provided(self, mock_abs):
         with mock_is_file_for("/hello/world/snowflake.yml") as mock_is_file:
```

### Comparing `snowflake_cli_labs-2.1.2/tests/project/test_util.py` & `snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+from itertools import permutations
+
 import pytest
 from snowflake.cli.api.project.util import (
     append_to_identifier,
+    escape_like_pattern,
     is_valid_identifier,
+    is_valid_object_name,
     is_valid_quoted_identifier,
     is_valid_string_literal,
     is_valid_unquoted_identifier,
     to_identifier,
     to_string_literal,
-    is_valid_object_name,
-    escape_like_pattern,
 )
 
-from itertools import permutations
-
 VALID_UNQUOTED_IDENTIFIERS = (
     "_",
     "____",
     "A",
     "a",
     "_aA1",
     "a$1",
@@ -49,53 +49,53 @@
     '"abc',  # unterminated quote
     'abc"',  # missing leading quote
     '"abc"def"',  # improperly escaped inner quote
 )
 
 
 def test_is_valid_unquoted_identifier():
-    for id in VALID_UNQUOTED_IDENTIFIERS:
-        assert is_valid_unquoted_identifier(id)
+    for id_ in VALID_UNQUOTED_IDENTIFIERS:
+        assert is_valid_unquoted_identifier(id_)
 
-    for id in VALID_QUOTED_IDENTIFIERS:
-        assert not is_valid_unquoted_identifier(id)
+    for id_ in VALID_QUOTED_IDENTIFIERS:
+        assert not is_valid_unquoted_identifier(id_)
 
-    for id in INVALID_UNQUOTED_IDENTIFIERS:
-        assert not is_valid_unquoted_identifier(id)
+    for id_ in INVALID_UNQUOTED_IDENTIFIERS:
+        assert not is_valid_unquoted_identifier(id_)
 
-    for id in INVALID_QUOTED_IDENTIFIERS:
-        assert not is_valid_unquoted_identifier(id)
+    for id_ in INVALID_QUOTED_IDENTIFIERS:
+        assert not is_valid_unquoted_identifier(id_)
 
 
 def test_is_valid_quoted_identifier():
-    for id in VALID_UNQUOTED_IDENTIFIERS:
-        assert not is_valid_quoted_identifier(id)
+    for id_ in VALID_UNQUOTED_IDENTIFIERS:
+        assert not is_valid_quoted_identifier(id_)
 
-    for id in VALID_QUOTED_IDENTIFIERS:
-        assert is_valid_quoted_identifier(id)
+    for id_ in VALID_QUOTED_IDENTIFIERS:
+        assert is_valid_quoted_identifier(id_)
 
-    for id in INVALID_UNQUOTED_IDENTIFIERS:
-        assert not is_valid_quoted_identifier(id)
+    for id_ in INVALID_UNQUOTED_IDENTIFIERS:
+        assert not is_valid_quoted_identifier(id_)
 
-    for id in INVALID_QUOTED_IDENTIFIERS:
-        assert not is_valid_quoted_identifier(id)
+    for id_ in INVALID_QUOTED_IDENTIFIERS:
+        assert not is_valid_quoted_identifier(id_)
 
 
 def test_is_valid_identifier():
-    for id in VALID_UNQUOTED_IDENTIFIERS:
-        assert is_valid_identifier(id)
+    for id_ in VALID_UNQUOTED_IDENTIFIERS:
+        assert is_valid_identifier(id_)
 
-    for id in VALID_QUOTED_IDENTIFIERS:
-        assert is_valid_identifier(id)
+    for id_ in VALID_QUOTED_IDENTIFIERS:
+        assert is_valid_identifier(id_)
 
-    for id in INVALID_UNQUOTED_IDENTIFIERS:
-        assert not is_valid_identifier(id)
+    for id_ in INVALID_UNQUOTED_IDENTIFIERS:
+        assert not is_valid_identifier(id_)
 
-    for id in INVALID_QUOTED_IDENTIFIERS:
-        assert not is_valid_identifier(id)
+    for id_ in INVALID_QUOTED_IDENTIFIERS:
+        assert not is_valid_identifier(id_)
 
 
 def test_is_valid_object_name():
     valid_identifiers = VALID_QUOTED_IDENTIFIERS + VALID_UNQUOTED_IDENTIFIERS
     invalid_identifiers = INVALID_QUOTED_IDENTIFIERS + INVALID_UNQUOTED_IDENTIFIERS
 
     # any combination of 1, 2, or 3 valid identifiers separated by a '.' is valid
@@ -128,18 +128,18 @@
             if has_quotes:
                 assert not is_valid_object_name(name, max_depth=2, allow_quoted=False)
             else:
                 assert is_valid_object_name(name, max_depth=2, allow_quoted=False)
 
 
 def test_to_identifier():
-    for id in VALID_UNQUOTED_IDENTIFIERS:
-        assert to_identifier(id) == id
-    for id in VALID_QUOTED_IDENTIFIERS:
-        assert to_identifier(id) == id
+    for id_ in VALID_UNQUOTED_IDENTIFIERS:
+        assert to_identifier(id_) == id_
+    for id_ in VALID_QUOTED_IDENTIFIERS:
+        assert to_identifier(id_) == id_
 
     assert to_identifier("abc def") == '"abc def"'
     assert to_identifier('abc"def') == '"abc""def"'
     assert to_identifier("abc'def") == '"abc\'def"'
     assert to_identifier("(A)") == '"(A)"'
```

### Comparing `snowflake_cli_labs-2.1.2/tests/snowpark/test_function.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,18 @@
     mock_connector,
     runner,
     mock_ctx,
     mock_cursor,
     project_directory,
 ):
     rows = [
-        ("packages", '["foo=1.2.3", "bar>=3.0.0"]'),
+        ("packages", '["foo==1.2.3", "bar>=3.0.0"]'),
         ("handler", "app.func1_handler"),
         ("returns", "string"),
+        ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
     ]
 
     queries, result, project_dir = _deploy_function(
         rows,
         mock_connector,
         runner,
         mock_ctx,
@@ -169,15 +170,15 @@
     mock_connector,
     runner,
     mock_ctx,
     mock_cursor,
     project_directory,
 ):
     rows = [
-        ("packages", '["foo=1.2.3"]'),
+        ("packages", '["foo==1.2.3"]'),
         ("handler", "main.py:app"),
         ("returns", "table(variant)"),
     ]
 
     queries, result, project_dir = _deploy_function(
         rows,
         mock_connector,
@@ -203,30 +204,30 @@
             """\
             create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)
             returns string
             language python
             runtime_version=3.10
             imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
             handler='app.func1_handler'
-            packages=('foo=1.2.3','bar>=3.0.0')
+            packages=('foo==1.2.3','bar>=3.0.0')
             """
         ).strip(),
     ]
 
 
 @mock.patch("snowflake.connector.connect")
 def test_deploy_function_needs_update_because_handler_changes(
     mock_connector,
     runner,
     mock_ctx,
     mock_cursor,
     project_directory,
 ):
     rows = [
-        ("packages", '["foo=1.2.3", "bar>=3.0.0"]'),
+        ("packages", '["foo==1.2.3", "bar>=3.0.0"]'),
         ("handler", "main.py:oldApp"),
         ("returns", "table(variant)"),
     ]
 
     queries, result, project_dir = _deploy_function(
         rows,
         mock_connector,
@@ -253,15 +254,15 @@
             """\
             create or replace function MOCKDATABASE.MOCKSCHEMA.FUNC1(a string default 'default value', b variant)
             returns string
             language python
             runtime_version=3.10
             imports=('@MOCKDATABASE.MOCKSCHEMA.DEV_DEPLOYMENT/my_snowpark_project/app.zip')
             handler='app.func1_handler'
-            packages=('foo=1.2.3','bar>=3.0.0')
+            packages=('foo==1.2.3','bar>=3.0.0')
             """
         ).strip(),
     ]
 
 
 @mock.patch("snowflake.connector.connect")
 @mock.patch("snowflake.cli.plugins.snowpark.commands.ObjectManager.describe")
@@ -314,15 +315,15 @@
             "snowpark",
             "execute",
             "function",
             "functionName(42, 'string')",
         ]
     )
 
-    assert result.exit_code == 0, result._output
+    assert result.exit_code == 0, result.output
     assert ctx.get_query() == "select functionName(42, 'string')"
 
 
 def _deploy_function(
     rows,
     mock_connector,
     runner,
@@ -338,15 +339,15 @@
     ) as om_describe, mock.patch(
         "snowflake.cli.plugins.snowpark.commands.ObjectManager.show"
     ) as om_show:
         om_describe.return_value = rows
 
         with project_directory("snowpark_functions") as temp_dir:
             (Path(temp_dir) / "requirements.snowflake.txt").write_text(
-                "foo=1.2.3\nbar>=3.0.0"
+                "foo==1.2.3\nbar>=3.0.0"
             )
             result = runner.invoke(
                 [
                     "snowpark",
                     "deploy",
                     "--format",
                     "json",
```

### Comparing `snowflake_cli_labs-2.1.2/tests/snowpark/test_package.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,151 @@
 import logging
 import os
+from pathlib import Path
 from unittest import mock
-from unittest.mock import MagicMock, patch
-from zipfile import ZipFile
+from unittest.mock import patch
 
 import pytest
-from requirements.requirement import Requirement
-
-import snowflake.cli.plugins.snowpark.package.manager
-import src.snowflake.cli.plugins.snowpark.package.manager
-from snowflake.cli.plugins.snowpark.models import SplitRequirements
-from snowflake.cli.plugins.snowpark.package.utils import NotInAnaconda, NothingFound
+import snowflake.cli.plugins.snowpark.models
+import snowflake.cli.plugins.snowpark.package.utils
+from snowflake.cli.api.secure_path import SecurePath
+from snowflake.cli.api.utils import path_utils
+from snowflake.cli.plugins.snowpark import package_utils
+from snowflake.cli.plugins.snowpark.package.anaconda_packages import (
+    AnacondaPackages,
+)
 
 from tests.test_data import test_data
 
 
-class TestPackage:
-    @pytest.mark.parametrize(
-        "argument",
-        ["snowflake-connector-python", "some-weird-package-we-dont-know"],
+def test_prepare_app_zip(
+    temp_dir,
+    app_zip: str,
+    temp_directory_for_app_zip: str,
+):
+    result = snowflake.cli.plugins.snowpark.package.utils.prepare_app_zip(
+        SecurePath(app_zip), SecurePath(temp_directory_for_app_zip)
+    )
+    assert str(result.path) == os.path.join(
+        temp_directory_for_app_zip, Path(app_zip).name
     )
-    @patch("snowflake.cli.plugins.snowpark.package_utils.requests")
-    def test_package_lookup(
-        self, mock_requests, argument, monkeypatch, runner, snapshot
-    ) -> None:
-        mock_requests.get.return_value = self.mocked_anaconda_response(
-            test_data.anaconda_response
-        )
-
-        result = runner.invoke(["snowpark", "package", "lookup", argument, "--yes"])
-
-        assert result.exit_code == 0
-        assert result.output == snapshot
 
-    @patch("snowflake.cli.plugins.snowpark.package_utils.install_packages")
-    @patch("snowflake.cli.plugins.snowpark.package_utils.parse_anaconda_packages")
-    def test_package_lookup_with_install_packages(
-        self, mock_package, mock_install, runner, capfd, snapshot
-    ) -> None:
 
-        mock_package.return_value = SplitRequirements(
-            [], [Requirement("some-other-package")]
-        )
-        mock_install.return_value = (
-            True,
-            SplitRequirements(
-                [Requirement("snowflake-snowpark-python")],
-                [Requirement("some-other-package")],
-            ),
+def test_prepare_app_zip_if_exception_is_raised_if_no_source(
+    temp_directory_for_app_zip,
+):
+    with pytest.raises(FileNotFoundError) as expected_error:
+        snowflake.cli.plugins.snowpark.package.utils.prepare_app_zip(
+            SecurePath("/non/existent/path"), SecurePath(temp_directory_for_app_zip)
         )
 
-        result = runner.invoke(
-            ["snowpark", "package", "lookup", "some-other-package", "--yes"]
-        )
-        assert result.exit_code == 0
-        assert result.output == snapshot
+    assert expected_error.value.errno == 2
+    assert expected_error.type == FileNotFoundError
 
-    @patch("snowflake.cli.plugins.snowpark.package.commands.lookup")
-    def test_package_create(
-        self, mock_lookup, caplog, temp_dir, dot_packages_directory, runner
-    ) -> None:
 
-        mock_lookup.return_value = NotInAnaconda(
-            SplitRequirements([], ["some-other-package"]), "totally-awesome-package"
+def test_prepare_app_zip_if_exception_is_raised_if_no_dst(app_zip):
+    with pytest.raises(FileNotFoundError) as expected_error:
+        snowflake.cli.plugins.snowpark.package.utils.prepare_app_zip(
+            SecurePath(app_zip), SecurePath("/non/existent/path")
         )
 
-        with caplog.at_level(
-            logging.DEBUG, logger="snowflake.cli.plugins.snowpark.package"
-        ):
-            result = runner.invoke(
-                ["snowpark", "package", "create", "totally-awesome-package", "--yes"]
-            )
-
-        assert result.exit_code == 0
-        assert os.path.isfile("totally-awesome-package.zip")
+    assert expected_error.value.errno == 2
+    assert expected_error.type == FileNotFoundError
 
-        zip_file = ZipFile("totally-awesome-package.zip", "r")
 
-        assert (
-            "totally-awesome-package/totally-awesome-module.py" in zip_file.namelist()
-        )
-        os.remove("totally-awesome-package.zip")
-
-    @mock.patch("snowflake.cli.plugins.snowpark.package.manager.StageManager")
-    @mock.patch("snowflake.connector.connect")
-    def test_package_upload(
-        self,
-        mock_connector,
-        mock_stage_manager,
-        package_file: str,
-        runner,
-        mock_ctx,
-        mock_cursor,
-    ) -> None:
-        ctx = mock_ctx()
-        mock_connector.return_value = ctx
-        mock_stage_manager().put.return_value = mock_cursor(
-            rows=[("", "", "", "", "", "", "UPLOADED")], columns=[]
-        )
+def test_parse_requirements_with_correct_file(
+    correct_requirements_snowflake_txt: str, temp_dir
+):
+    result = package_utils.parse_requirements(
+        SecurePath(correct_requirements_snowflake_txt)
+    )
 
-        result = runner.invoke(
-            ["snowpark", "package", "upload", "-f", package_file, "-s", "stageName"]
-        )
+    assert len(result) == len(test_data.requirements)
 
-        assert result.exit_code == 0
-        assert ctx.get_query() == ""
 
-    @mock.patch(
-        "snowflake.cli.plugins.snowpark.package.manager.StageManager._execute_query"
-    )
-    def test_package_upload_to_path(
-        self,
-        mock_execute_queries,
-        package_file: str,
-        runner,
-        mock_ctx,
-        mock_cursor,
-    ) -> None:
-        mock_execute_queries.return_value = MagicMock()
-
-        result = runner.invoke(
-            [
-                "snowpark",
-                "package",
-                "upload",
-                "-f",
-                package_file,
-                "-s",
-                "db.schema.stage/path/to/file",
-            ]
+def test_parse_requirements_with_nonexistent_file(temp_dir):
+    path = os.path.join(temp_dir, "non_existent.file")
+    result = package_utils.parse_requirements(SecurePath(path))
+
+    assert result == []
+
+
+@pytest.mark.parametrize(
+    "contents, expected",
+    [
+        (
+            """pytest==1.0.0\nDjango==3.2.1\nawesome_lib==3.3.3""",
+            ["pytest==1.0.0", "django==3.2.1", "awesome_lib==3.3.3"],
+        ),
+        ("""toml # some-comment""", ["toml"]),
+        ("", []),
+        ("""some-package==1.2.3#incorrect_comment""", ["some_package==1.2.3"]),
+        ("""#only comment here""", []),
+        (
+            """pytest==1.0\n# comment\nawesome_lib==3.3.3""",
+            ["pytest==1.0", "awesome_lib==3.3.3"],
+        ),
+    ],
+)
+@mock.patch("snowflake.cli.plugins.snowpark.package_utils.SecurePath.read_text")
+def test_parse_requirements_corner_cases(
+    mock_file, contents, expected, correct_requirements_snowflake_txt
+):
+    mock_file.return_value = contents
+    result = [
+        p.name_and_version
+        for p in package_utils.parse_requirements(
+            SecurePath(correct_requirements_snowflake_txt)
+        )
+    ]
+    mock_file.assert_called_with(file_size_limit_mb=128)
+    assert result == expected
+
+
+def test_parse_requirements(correct_requirements_txt: str):
+    result = package_utils.parse_requirements(SecurePath(correct_requirements_txt))
+    result.sort(key=lambda r: r.name)
+
+    assert len(result) == 3
+    assert result[0].name == "awesome_lib"
+    assert result[0].specifier is True
+    assert result[0].specs == [("==", "3.3.3")]
+    assert result[1].name == "django"
+    assert result[1].specifier is True
+    assert result[1].specs == [("==", "3.2.1")]
+    assert result[2].name == "pytest"
+    assert result[2].specifier is True
+    assert result[2].specs == [("==", "1.0.0")]
+
+
+@patch("platform.system")
+@pytest.mark.parametrize(
+    "argument, expected",
+    [
+        ("C:\\Something\\Something Else", "C:\\Something\\Something Else"),
+        (
+            "/var/folders/k8/3sdqh3nn4gg7lpr5fz0fjlqw0000gn/T/tmpja15jymq",
+            "/var/folders/k8/3sdqh3nn4gg7lpr5fz0fjlqw0000gn/T/tmpja15jymq",
+        ),
+    ],
+)
+def test_path_resolver(mock_system, argument, expected):
+    mock_system.response_value = "Windows"
+
+    assert path_utils.path_resolver(argument) == expected
+
+
+@patch("snowflake.cli.plugins.snowpark.package_utils.Venv.pip_wheel")
+def test_pip_fail_message(mock_installer, correct_requirements_txt, caplog):
+    mock_installer.return_value = 42
+
+    with caplog.at_level(logging.INFO, "snowflake.cli.plugins.snowpark.package_utils"):
+        requirements = package_utils.parse_requirements(
+            SecurePath(correct_requirements_txt)
+        )
+        package_utils.download_unavailable_packages(
+            requirements=requirements,
+            target_dir=SecurePath(".packages"),
+            anaconda_packages=AnacondaPackages.empty(),
         )
 
-        assert result.exit_code == 0
-        assert mock_execute_queries.call_count == 2
-        create, put = mock_execute_queries.call_args_list
-        assert create.args[0] == "create stage if not exists db.schema.stage"
-        assert "db.schema.stage/path/to/file" in put.args[0]
-
-    @pytest.mark.parametrize("command", ["lookup", "create"])
-    @pytest.mark.parametrize(
-        "flags,expected_value",
-        [
-            (["--pypi-download"], True),
-            (["-y"], True),
-            (["--yes"], True),
-            (["--pypi-download", "-y"], True),
-            ([], False),
-        ],
-    )
-    @mock.patch("snowflake.cli.plugins.snowpark.package.commands.lookup")
-    def test_install_flag(self, mock_lookup, command, flags, expected_value, runner):
-        mock_lookup.return_value = NothingFound
-        result = runner.invoke(["snowpark", "package", "lookup", "foo", *flags])
-
-        mock_lookup.assert_called_with(name="foo", install_packages=expected_value)
-
-    @staticmethod
-    def mocked_anaconda_response(response: dict):
-        mock_response = MagicMock()
-        mock_response.status_code = 200
-        mock_response.json.return_value = response
-
-        return mock_response
+    assert "pip failed with return code 42" in caplog.text
```

### Comparing `snowflake_cli_labs-2.1.2/tests/snowpark/test_procedure.py` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import json
 from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 from unittest.mock import call
 
-import pytest
-
 from snowflake.cli.api.constants import ObjectType
 from snowflake.connector import ProgrammingError
 
-from click import ClickException
-
 
 def test_deploy_function_no_procedure(runner, project_directory):
     with project_directory("empty_project"):
         result = runner.invoke(
             [
                 "snowpark",
                 "deploy",
@@ -254,22 +250,24 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
+                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "test"),
                 ("returns", "string"),
+                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
 
@@ -305,22 +303,24 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
+                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "foo"),
                 ("returns", "string"),
+                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
 
@@ -356,14 +356,15 @@
 ):
     mock_om_describe.side_effect = [
         mock_cursor(
             [
                 ("packages", "[]"),
                 ("handler", "hello"),
                 ("returns", "string"),
+                ("imports", "DEV_DEPLOYMENT/my_snowpark_project/app.zip"),
             ],
             columns=["key", "value"],
         ),
         ProgrammingError("does not exist or not authorized"),
     ]
     ctx = mock_ctx()
     mock_conn.return_value = ctx
```

### Comparing `snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/snowpark/__snapshots__/test_procedure.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/test_common.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from snowflake.cli.plugins.spcs.common import validate_and_set_instances
-from tests.testing_utils.fixtures import *
+from unittest.mock import Mock
+
+import pytest
 from click import ClickException
-from snowflake.connector.errors import ProgrammingError
-from snowflake.cli.plugins.spcs.common import handle_object_already_exists
 from snowflake.cli.api.exceptions import ObjectAlreadyExistsError, ObjectType
-from unittest.mock import Mock
+from snowflake.cli.plugins.spcs.common import (
+    handle_object_already_exists,
+    validate_and_set_instances,
+)
+from snowflake.connector.errors import ProgrammingError
 
 
 @pytest.mark.parametrize(
     "min_instances, max_instances, expected_max",
     [
         (2, None, 2),  # max_instances is None, set max_instances to min_instances
         (
```

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/test_image_repository.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from tests.testing_utils.fixtures import *
 import json
-from snowflake.cli.plugins.spcs.image_repository.manager import ImageRepositoryManager
 from typing import Dict
-from click import ClickException
+from unittest import mock
 from unittest.mock import Mock
-from snowflake.connector.cursor import SnowflakeCursor
-from snowflake.connector.errors import ProgrammingError
+
+import pytest
+from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.exceptions import (
     DatabaseNotProvidedError,
     SchemaNotProvidedError,
 )
-from snowflake.cli.api.constants import ObjectType
+from snowflake.cli.plugins.spcs.image_repository.manager import ImageRepositoryManager
+from snowflake.connector.cursor import SnowflakeCursor
+from snowflake.connector.errors import ProgrammingError
+
 from tests.spcs.test_common import SPCS_OBJECT_EXISTS_ERROR
 
 MOCK_ROWS = [
     [
         "2023-01-01 00:00:00",
         "IMAGES",
         "DB",
@@ -38,59 +40,93 @@
 ]
 MOCK_ROWS_DICT = [
     {col_name: col_val for col_name, col_val in zip(MOCK_COLUMNS, row)}
     for row in MOCK_ROWS
 ]
 
 
+@pytest.mark.parametrize(
+    "replace, if_not_exists, expected_query",
+    [
+        (False, False, "create image repository test_repo"),
+        (False, True, "create image repository if not exists test_repo"),
+        (True, False, "create or replace image repository test_repo"),
+        # (True, True) is an invalid case as OR REPLACE and IF NOT EXISTS are mutually exclusive.
+    ],
+)
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._execute_schema_query"
 )
-def test_create(
-    mock_execute,
-):
+def test_create(mock_execute, replace, if_not_exists, expected_query):
     repo_name = "test_repo"
     cursor = Mock(spec=SnowflakeCursor)
     mock_execute.return_value = cursor
-    result = ImageRepositoryManager().create(name=repo_name)
-    expected_query = "create image repository test_repo"
-    mock_execute.assert_called_once_with(expected_query)
+    result = ImageRepositoryManager().create(
+        name=repo_name, replace=replace, if_not_exists=if_not_exists
+    )
+    mock_execute.assert_called_once_with(expected_query, name=repo_name)
     assert result == cursor
 
 
+def test_create_replace_and_if_not_exist():
+    with pytest.raises(ValueError) as e:
+        ImageRepositoryManager().create(
+            name="test_repo", replace=True, if_not_exists=True
+        )
+    assert "mutually exclusive" in str(e.value)
+
+
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.create"
 )
-def test_create_cli(mock_create, mock_cursor, runner):
+def test_create_cli(mock_create, mock_cursor, runner, snapshot):
     repo_name = "test_repo"
     cursor = mock_cursor(
         rows=[[f"Image Repository {repo_name.upper()} successfully created."]],
         columns=["status"],
     )
     mock_create.return_value = cursor
-    result = runner.invoke(["spcs", "image-repository", "create", repo_name])
-    mock_create.assert_called_once_with(name=repo_name)
-    assert result.exit_code == 0, result.output
-    assert (
-        f"Image Repository {repo_name.upper()} successfully created." in result.output
+    command = ["spcs", "image-repository", "create", repo_name]
+    result = runner.invoke(command)
+    mock_create.assert_called_once_with(
+        name=repo_name, replace=False, if_not_exists=False
     )
+    assert result.exit_code == 0, result.output
+    assert result.output == snapshot
+
+
+def test_create_cli_replace_and_if_not_exists_fails(runner, snapshot):
+    command = [
+        "spcs",
+        "image-repository",
+        "create",
+        "test_repo",
+        "--replace",
+        "--if-not-exists",
+    ]
+    result = runner.invoke(command)
+    assert result.exit_code == 1
+    assert result.output == snapshot
 
 
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._execute_schema_query"
 )
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.handle_object_already_exists"
 )
 def test_create_repository_already_exists(mock_handle, mock_execute):
     repo_name = "test_object"
     mock_execute.side_effect = SPCS_OBJECT_EXISTS_ERROR
-    ImageRepositoryManager().create(repo_name)
+    ImageRepositoryManager().create(repo_name, replace=False, if_not_exists=False)
     mock_handle.assert_called_once_with(
-        SPCS_OBJECT_EXISTS_ERROR, ObjectType.IMAGE_REPOSITORY, repo_name
+        SPCS_OBJECT_EXISTS_ERROR,
+        ObjectType.IMAGE_REPOSITORY,
+        repo_name,
+        replace_available=True,
     )
 
 
 @mock.patch("snowflake.cli.plugins.spcs.image_repository.commands.requests.get")
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.commands.ImageRepositoryManager._execute_query"
 )
@@ -161,15 +197,15 @@
 
     result = runner.invoke(
         [
             "spcs",
             "image-repository",
             "list-tags",
             "IMAGES",
-            "--image_name",
+            "--image-name",
             "/DB/SCHEMA/IMAGES/super-cool-repo",
             "--format",
             "JSON",
         ]
     )
 
     assert result.exit_code == 0, result.output
@@ -186,87 +222,76 @@
     mock_url.return_value = repo_url
     result = runner.invoke(["spcs", "image-repository", "url", "IMAGES"])
     assert result.exit_code == 0, result.output
     assert result.output.strip() == repo_url
 
 
 @mock.patch(
-    "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.check_database_and_schema"
-)
-@mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.show_specific_object"
 )
-def test_get_repository_url(mock_get_row, mock_check_database_and_schema):
+def test_get_repository_url(mock_get_row):
     expected_row = MOCK_ROWS_DICT[0]
     mock_get_row.return_value = expected_row
     result = ImageRepositoryManager().get_repository_url(repo_name="IMAGES")
     mock_get_row.assert_called_once_with(
         "image repositories", "IMAGES", check_schema=True
     )
     assert isinstance(expected_row, Dict)
     assert "repository_url" in expected_row
     assert result == f"https://{expected_row['repository_url']}"
 
 
 @mock.patch(
-    "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.check_database_and_schema"
-)
-@mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.show_specific_object"
 )
-def test_get_repository_url_no_scheme(mock_get_row, mock_check_database_and_schema):
+def test_get_repository_url_no_scheme(mock_get_row):
     expected_row = MOCK_ROWS_DICT[0]
     mock_get_row.return_value = expected_row
     result = ImageRepositoryManager().get_repository_url(
         repo_name="IMAGES", with_scheme=False
     )
     mock_get_row.assert_called_once_with(
         "image repositories", "IMAGES", check_schema=True
     )
     assert isinstance(expected_row, Dict)
     assert "repository_url" in expected_row
     assert result == expected_row["repository_url"]
 
 
 @mock.patch(
-    "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.check_database_and_schema"
-)
-@mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._conn"
 )
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager.show_specific_object"
 )
-def test_get_repository_url_no_repo_found(
-    mock_get_row, mock_conn, mock_check_database_and_schema
-):
+def test_get_repository_url_no_repo_found(mock_get_row, mock_conn):
     mock_get_row.return_value = None
     mock_conn.database = "DB"
     mock_conn.schema = "SCHEMA"
-    with pytest.raises(ClickException) as e:
+    with pytest.raises(ProgrammingError) as e:
         ImageRepositoryManager().get_repository_url(repo_name="IMAGES")
     assert (
-        e.value.message
-        == "Image repository 'IMAGES' does not exist in database 'DB' and schema 'SCHEMA' or not authorized."
+        e.value.msg
+        == "Image repository 'DB.SCHEMA.IMAGES' does not exist or not authorized."
     )
     mock_get_row.assert_called_once_with(
         "image repositories", "IMAGES", check_schema=True
     )
 
 
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._conn"
 )
-def test_get_repository_url_no_database(mock_conn):
+def test_get_repository_url_no_database_provided(mock_conn):
     mock_conn.database = None
     with pytest.raises(DatabaseNotProvidedError):
-        ImageRepositoryManager().get_repository_url("test_repo")
+        ImageRepositoryManager().get_repository_url("IMAGES")
 
 
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_repository.manager.ImageRepositoryManager._conn"
 )
-@mock.patch("snowflake.cli.api.sql_execution.SqlExecutionMixin.check_database_exists")
-def test_get_repository_url_no_schema(mock_check_database_exists, mock_conn):
+def test_get_repository_url_no_schema_provided(mock_conn):
+    mock_conn.database = "DB"
     mock_conn.schema = None
     with pytest.raises(SchemaNotProvidedError):
-        ImageRepositoryManager().get_repository_url("test_repo")
+        ImageRepositoryManager().get_repository_url("IMAGES")
```

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/test_jobs.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import os
 from tempfile import TemporaryDirectory
+from unittest import mock
 
-from tests.testing_utils.fixtures import *
+import pytest
 
 
+@pytest.mark.skip("Snowpark Container Services Job not supported.")
 @mock.patch("snowflake.connector.connect")
 def test_create_job(mock_connector, runner, mock_ctx):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
 
     test_spec = """
 spec:
@@ -36,25 +39,27 @@
         "IN COMPUTE POOL testPool\n"
         "FROM SPECIFICATION $$\n"
         '{"spec": {"containers": [{"name": "main", "image": "public.ecr.aws/myrepo:latest"}]}}\n'
         "$$\n"
     )
 
 
+@pytest.mark.skip("Snowpark Container Services Job not supported.")
 @mock.patch("snowflake.connector.connect")
 def test_job_status(mock_connector, runner, mock_ctx):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
 
     result = runner.invoke(["spcs", "job", "status", "jobName"])
 
     assert result.exit_code == 0, result.output
     assert ctx.get_query() == "CALL SYSTEM$GET_JOB_STATUS('jobName')"
 
 
+@pytest.mark.skip("Snowpark Container Services Job not supported.")
 @mock.patch("snowflake.connector.connect")
 def test_job_logs(mock_connector, runner, mock_ctx):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
 
     result = runner.invoke(
         ["spcs", "job", "logs", "--container-name", "containerName", "jobName"]
```

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/test_registry.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
-from subprocess import CalledProcessError
+from subprocess import PIPE, CalledProcessError
+from unittest import mock
 
-from tests.testing_utils.fixtures import *
+import pytest
+from click import ClickException
 from snowflake.cli.plugins.spcs.image_registry.manager import (
-    RegistryManager,
     NoImageRepositoriesFoundError,
+    RegistryManager,
 )
 from snowflake.connector.cursor import DictCursor
-from click import ClickException
 
 
 @mock.patch("snowflake.cli.plugins.spcs.image_registry.manager.RegistryManager._conn")
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_registry.manager.RegistryManager._execute_query"
 )
 def test_registry_get_token(mock_execute, mock_conn, mock_cursor, runner):
     mock_execute.return_value = mock_cursor(
         ["row"], ["Statement executed successfully"]
     )
-    mock_conn._rest._token_request.return_value = {
+    mock_conn._rest._token_request.return_value = {  # noqa: SLF001
         "data": {
             "sessionToken": "token1234",
             "validityInSecondsST": 42,
         }
     }
     result = runner.invoke(["spcs", "image-registry", "token", "--format", "JSON"])
     assert result.exit_code == 0, result.output
@@ -103,15 +104,15 @@
         (
             "http://snowservices.registry.snowflakecomputing.com/db/schema/tutorial_repo",
             True,
         ),
     ],
 )
 def test_has_url_scheme(url: str, expected: bool):
-    assert RegistryManager()._has_url_scheme(url) == expected
+    assert RegistryManager()._has_url_scheme(url) == expected  # noqa: SLF001
 
 
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_registry.manager.RegistryManager.get_token"
 )
 @mock.patch(
     "snowflake.cli.plugins.spcs.image_registry.manager.RegistryManager.get_registry_url"
@@ -134,15 +135,15 @@
         "0sessiontoken",
         "--password-stdin",
         test_url,
     ]
 
     result = RegistryManager().docker_registry_login()
     mock_check_output.assert_called_once_with(
-        expected_command, input=json.dumps(test_token), text=True
+        expected_command, input=json.dumps(test_token), text=True, stderr=PIPE
     )
     mock_get_url.assert_called_once_with()
     mock_get_token.assert_called_once_with()
     assert result == test_output
 
 
 @mock.patch(
```

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/test_services.py` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import json
+from pathlib import Path
 from textwrap import dedent
 from unittest.mock import Mock, patch
-import json
 
-from tests.spcs.test_common import SPCS_OBJECT_EXISTS_ERROR
-from snowflake.cli.plugins.spcs.common import NoPropertiesProvidedError
+import pytest
+from click import ClickException
 from snowflake.cli.api.constants import ObjectType
-from snowflake.cli.plugins.spcs.services.manager import ServiceManager
-from tests.testing_utils.fixtures import *
 from snowflake.cli.api.project.util import to_string_literal
 from snowflake.cli.plugins.object.common import Tag
+from snowflake.cli.plugins.spcs.common import NoPropertiesProvidedError
 from snowflake.cli.plugins.spcs.services.commands import _service_name_callback
-from click import ClickException
+from snowflake.cli.plugins.spcs.services.manager import ServiceManager
+from snowflake.connector.cursor import SnowflakeCursor
+from yaml import YAMLError
+
+from tests.spcs.test_common import SPCS_OBJECT_EXISTS_ERROR
 
 SPEC_CONTENT = dedent(
     """
     spec:
         containers:
         - name: cloudbeaver
           image: /spcs_demos_db/cloudbeaver:23.2.1
@@ -64,14 +68,15 @@
         min_instances=min_instances,
         max_instances=max_instances,
         auto_resume=auto_resume,
         external_access_integrations=external_access_integrations,
         query_warehouse=query_warehouse,
         tags=tags,
         comment=comment,
+        if_not_exists=False,
     )
     expected_query = " ".join(
         [
             "CREATE SERVICE test_service",
             "IN COMPUTE POOL test_pool",
             f"FROM SPECIFICATION $$ {json.dumps(SPEC_DICT)} $$",
             "MIN_INSTANCES = 42 MAX_INSTANCES = 43",
@@ -108,18 +113,19 @@
     mock_create.assert_called_once_with(
         service_name="test_service",
         compute_pool="test_pool",
         spec_path=spec_path,
         min_instances=1,
         max_instances=1,
         auto_resume=True,
-        external_access_integrations=[],
+        external_access_integrations=None,
         query_warehouse=None,
-        tags=[],
+        tags=None,
         comment=None,
+        if_not_exists=False,
     )
 
 
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager.create")
 def test_create_service_cli(mock_create, other_directory, runner):
     tmp_dir = Path(other_directory)
     spec_path = tmp_dir / "spec.yml"
@@ -147,62 +153,65 @@
             "test_warehouse",
             "--tag",
             "name=value",
             "--tag",
             '"$trange name"=normal value',
             "--comment",
             "this is a test",
+            "--if-not-exists",
         ]
     )
     assert result.exit_code == 0, result.output
     mock_create.assert_called_once_with(
         service_name="test_service",
         compute_pool="test_pool",
         spec_path=spec_path,
         min_instances=42,
         max_instances=43,
         auto_resume=False,
         external_access_integrations=["google_api", "salesforce_api"],
         query_warehouse="test_warehouse",
         tags=[Tag("name", "value"), Tag('"$trange name"', "normal value")],
         comment=to_string_literal("this is a test"),
+        if_not_exists=True,
     )
 
 
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._read_yaml")
 def test_create_service_with_invalid_spec(mock_read_yaml):
     service_name = "test_service"
     compute_pool = "test_pool"
     spec_path = "/path/to/spec.yaml"
     min_instances = 42
     max_instances = 42
     external_access_integrations = query_warehouse = tags = comment = None
     auto_resume = False
-    mock_read_yaml.side_effect = strictyaml.YAMLError("Invalid YAML")
+    mock_read_yaml.side_effect = YAMLError("Invalid YAML")
 
-    with pytest.raises(strictyaml.YAMLError):
+    with pytest.raises(YAMLError):
         ServiceManager().create(
             service_name=service_name,
             compute_pool=compute_pool,
             spec_path=Path(spec_path),
             min_instances=min_instances,
             max_instances=max_instances,
             auto_resume=auto_resume,
             external_access_integrations=external_access_integrations,
             query_warehouse=query_warehouse,
             tags=tags,
             comment=comment,
+            if_not_exists=False,
         )
 
 
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._read_yaml")
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._execute_query")
 @patch("snowflake.cli.plugins.spcs.services.manager.handle_object_already_exists")
-def test_create_repository_already_exists(mock_handle, mock_execute, mock_read_yaml):
-    service_name = "test_object"
+def test_create_service_already_exists(mock_handle, mock_execute, mock_read_yaml):
+    service_name = "test_service"
     compute_pool = "test_pool"
     spec_path = "/path/to/spec.yaml"
     min_instances = 42
     max_instances = 42
     external_access_integrations = query_warehouse = tags = comment = None
     auto_resume = False
     mock_execute.side_effect = SPCS_OBJECT_EXISTS_ERROR
@@ -213,21 +222,56 @@
         min_instances=min_instances,
         max_instances=max_instances,
         auto_resume=auto_resume,
         external_access_integrations=external_access_integrations,
         query_warehouse=query_warehouse,
         tags=tags,
         comment=comment,
+        if_not_exists=False,
     )
     mock_handle.assert_called_once_with(
         SPCS_OBJECT_EXISTS_ERROR, ObjectType.SERVICE, service_name
     )
 
 
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._execute_query")
+def test_create_service_if_not_exists(mock_execute_query, other_directory):
+    cursor = Mock(spec=SnowflakeCursor)
+    mock_execute_query.return_value = cursor
+    tmp_dir = Path(other_directory)
+    spec_path = tmp_dir / "spec.yml"
+    spec_path.write_text(SPEC_CONTENT)
+    result = ServiceManager().create(
+        service_name="test_service",
+        compute_pool="test_pool",
+        spec_path=spec_path,
+        min_instances=1,
+        max_instances=1,
+        auto_resume=True,
+        external_access_integrations=None,
+        query_warehouse=None,
+        tags=None,
+        comment=None,
+        if_not_exists=True,
+    )
+    expected_query = " ".join(
+        [
+            "CREATE SERVICE IF NOT EXISTS test_service",
+            "IN COMPUTE POOL test_pool",
+            f"FROM SPECIFICATION $$ {json.dumps(SPEC_DICT)} $$",
+            "MIN_INSTANCES = 1 MAX_INSTANCES = 1",
+            "AUTO_RESUME = True",
+        ]
+    )
+    actual_query = " ".join(mock_execute_query.mock_calls[0].args[0].split())
+    assert expected_query == actual_query
+    assert result == cursor
+
+
+@patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._execute_query")
 def test_status(mock_execute_query):
     service_name = "test_service"
     cursor = Mock(spec=SnowflakeCursor)
     mock_execute_query.return_value = cursor
     result = ServiceManager().status(service_name)
     expected_query = "CALL SYSTEM$GET_SERVICE_STATUS('test_service')"
     mock_execute_query.assert_called_once_with(expected_query)
@@ -259,15 +303,15 @@
     assert result == cursor
 
 
 def test_read_yaml(other_directory):
     tmp_dir = Path(other_directory)
     spec_path = tmp_dir / "spec.yml"
     spec_path.write_text(SPEC_CONTENT)
-    result = ServiceManager()._read_yaml(spec_path)
+    result = ServiceManager()._read_yaml(spec_path)  # noqa: SLF001
     assert result == json.dumps(SPEC_DICT)
 
 
 @patch("snowflake.cli.plugins.spcs.services.manager.ServiceManager._execute_query")
 def test_upgrade_spec(mock_execute_query, other_directory):
     service_name = "test_service"
     cursor = Mock(spec=SnowflakeCursor)
```

### Comparing `snowflake_cli_labs-2.1.2/tests/spcs/__snapshots__/test_registry.ambr` & `snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/streamlit/test_commands.py` & `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import shutil
 from textwrap import dedent
+from unittest import mock
 
+import pytest
 from snowflake.cli.plugins.connection.util import REGIONLESS_QUERY
 
-from tests.testing_utils.fixtures import *
-
 STREAMLIT_NAME = "test_streamlit"
 TEST_WAREHOUSE = "test_warehouse"
 
 
 @mock.patch("snowflake.connector.connect")
 def test_list_streamlit(mock_connector, runner, mock_ctx):
     ctx = mock_ctx()
@@ -72,15 +73,15 @@
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT",
         _put_query(
             "streamlit_app.py", "@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/test_streamlit"
         ),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         "select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -122,15 +123,15 @@
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT",
         _put_query(
             "streamlit_app.py", "@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/test_streamlit"
         ),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         "select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -172,15 +173,15 @@
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT",
         _put_query(
             "streamlit_app.py", "@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/test_streamlit"
         ),
         dedent(
             f"""
-            CREATE OR REPLACE STREAMLIT {STREAMLIT_NAME}
+            CREATE OR REPLACE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         "select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -239,15 +240,15 @@
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT",
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", root_path),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -279,15 +280,15 @@
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT",
         _put_query("streamlit_app.py", root_path),
         _put_query("pages/*.py", f"{root_path}/pages"),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -321,15 +322,15 @@
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", root_path),
         _put_query("pages/*.py", f"{root_path}/pages"),
         _put_query("utils/utils.py", f"{root_path}/utils"),
         _put_query("extra_file.py", root_path),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -364,15 +365,15 @@
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT_STAGE",
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", root_path),
         _put_query("pages/*.py", f"{root_path}/pages"),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT_STAGE/{STREAMLIT_NAME}'
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -404,15 +405,15 @@
     assert ctx.get_queries() == [
         "create stage if not exists MOCKDATABASE.MOCKSCHEMA.STREAMLIT_STAGE",
         _put_query("main.py", root_path),
         _put_query("streamlit_environment.yml", root_path),
         _put_query("streamlit_pages/*.py", f"{root_path}/pages"),
         dedent(
             f"""
-            CREATE STREAMLIT {STREAMLIT_NAME}
+            CREATE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             ROOT_LOCATION = '@MOCKDATABASE.MOCKSCHEMA.STREAMLIT_STAGE/{STREAMLIT_NAME}'
             MAIN_FILE = 'main.py'
             QUERY_WAREHOUSE = streamlit_warehouse
             """
         ).strip(),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
@@ -436,27 +437,27 @@
     )
     mock_connector.return_value = ctx
 
     with project_directory("example_streamlit"):
         result = runner.invoke(["streamlit", "deploy", "--experimental"])
 
     root_path = (
-        f"snow://streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
+        f"@streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
         "default_checkout"
     )
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
         dedent(
             f"""
-            CREATE STREAMLIT IF NOT EXISTS {STREAMLIT_NAME}
+            CREATE STREAMLIT IF NOT EXISTS MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
-        "ALTER streamlit test_streamlit CHECKOUT",
+        f"ALTER streamlit MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()} CHECKOUT",
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", f"{root_path}"),
         _put_query("pages/*.py", f"{root_path}/pages"),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
         f"select current_account_name()",
     ]
@@ -501,23 +502,23 @@
 
     with project_directory("example_streamlit"):
         result2 = runner.invoke(["streamlit", "deploy", "--experimental"])
 
     assert result2.exit_code == 0, result2.output
 
     root_path = (
-        f"snow://streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
+        f"@streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
         "default_checkout"
     )
 
     # Same as normal, except no CHECKOUT query
     assert ctx.get_queries() == [
         dedent(
             f"""
-            CREATE STREAMLIT IF NOT EXISTS {STREAMLIT_NAME}
+            CREATE STREAMLIT IF NOT EXISTS MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", f"{root_path}"),
         _put_query("pages/*.py", f"{root_path}/pages"),
@@ -543,27 +544,27 @@
     )
     mock_connector.return_value = ctx
 
     with project_directory("example_streamlit_no_stage"):
         result = runner.invoke(["streamlit", "deploy", "--experimental"])
 
     root_path = (
-        f"snow://streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
+        f"@streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
         "default_checkout"
     )
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
         dedent(
             f"""
-            CREATE STREAMLIT IF NOT EXISTS {STREAMLIT_NAME}
+            CREATE STREAMLIT IF NOT EXISTS MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
-        "ALTER streamlit test_streamlit CHECKOUT",
+        f"ALTER streamlit MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()} CHECKOUT",
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", f"{root_path}"),
         _put_query("pages/*.py", f"{root_path}/pages"),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
         f"select current_account_name()",
     ]
@@ -585,27 +586,27 @@
     )
     mock_connector.return_value = ctx
 
     with project_directory("example_streamlit"):
         result = runner.invoke(["streamlit", "deploy", "--experimental", "--replace"])
 
     root_path = (
-        f"snow://streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
+        f"@streamlit/MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}/"
         "default_checkout"
     )
     assert result.exit_code == 0, result.output
     assert ctx.get_queries() == [
         dedent(
             f"""
-            CREATE OR REPLACE STREAMLIT {STREAMLIT_NAME}
+            CREATE OR REPLACE STREAMLIT MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()}
             MAIN_FILE = 'streamlit_app.py'
             QUERY_WAREHOUSE = test_warehouse
             """
         ).strip(),
-        "ALTER streamlit test_streamlit CHECKOUT",
+        f"ALTER streamlit MOCKDATABASE.MOCKSCHEMA.{STREAMLIT_NAME.upper()} CHECKOUT",
         _put_query("streamlit_app.py", root_path),
         _put_query("environment.yml", f"{root_path}"),
         _put_query("pages/*.py", f"{root_path}/pages"),
         f"select system$get_snowsight_host()",
         REGIONLESS_QUERY,
         f"select current_account_name()",
     ]
```

### Comparing `snowflake_cli_labs-2.1.2/tests/streamlit/test_config.py` & `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from collections import OrderedDict
 from pathlib import Path
 
 import pytest
-from strictyaml import YAML, as_document
 
-from src.snowflake.cli.api.project.definition import load_project_definition, merge_left
+from src.snowflake.cli.api.project.definition import load_project_definition
 
 TEST_DATA = Path(__file__).parent.parent / "test_data" / "streamlit"
 FILE_WITH_LONG_LIST = TEST_DATA / "with_list_in_source_file.yml"
 ANOTHER_FILE_WITH_LONG_LIST = TEST_DATA / "another_file_with_list.yml"
 FILE_WITH_SINGLE_ITEM_LIST = TEST_DATA / "with_single_item.yml"
 ANOTHER_FILE_WITH_SINGLE_ITEM = TEST_DATA / "another_file_with_single_item.yml"
 
@@ -28,8 +26,8 @@
         ([FILE_WITH_LONG_LIST, ANOTHER_FILE_WITH_LONG_LIST], "boing.py"),
     ],
 )
 def test_load_project_definition(test_files, expected):
 
     result = load_project_definition(test_files)
 
-    assert expected in result["streamlit"]["additional_source_files"]
+    assert expected in result.streamlit.additional_source_files
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/test_data.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from requirements.requirement import Requirement
+from snowflake.cli.plugins.snowpark.models import Requirement
 
 requirements = ["pytest==1.0.0", "Django==3.2.1", "awesome_lib==3.3.3"]
 
 packages = [
     Requirement.parse_line("snowflake-connector-python"),
     Requirement.parse_line("snowflake-snowpark-python"),
     Requirement.parse_line("my-totally-awesome-package"),
@@ -70,14 +70,20 @@
             "name": "streamlit",
             "subdirs": ["osx-64", "linux-64", "osx-arm64", "linux-aarch64", "win-64"],
             "version": "1.22.0",
             "license": "Apache-2.0",
             "md5": "a6e6f90bb4d3fef3a2f5778ec7b5196c",
             "timestamp": 1701377760,
         },
+        "package-with-non-pep-version": {
+            "version": "4d",
+            "license": "Apache-2.0",
+            "md5": "0bb4d3fef3a4d3fef3a2f5778e345d77",
+            "timestamp": 1701393763,
+        },
     },
 }
 
 describe_function_response = """[
   {
     "property": "signature",
     "value": "()"
```

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/integration/app/manifest.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/integration_external/app/manifest.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_functions/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/app.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures/app.zip` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/test_data/projects/snowpark_procedures_coverage/app.py` & `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests/testing_utils/files_and_dirs.py` & `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Generator, List, Union
 
-import stat
-
 from snowflake.cli.api.secure_utils import file_permissions_are_strict
 
 
-def create_temp_file(suffix: str, dir: str, contents: List[str]) -> str:
-    with tempfile.NamedTemporaryFile(suffix=suffix, dir=dir, delete=False) as tmp:
+def create_temp_file(suffix: str, dir_name: str, contents: List[str]) -> str:
+    with tempfile.NamedTemporaryFile(suffix=suffix, dir=dir_name, delete=False) as tmp:
         _write_to_file(tmp.name, contents)
     return tmp.name
 
 
-def create_named_file(file_name: str, dir: str, contents: List[str]):
-    file_path = os.path.join(dir, file_name)
+def create_named_file(file_name: str, dir_name: str, contents: List[str]):
+    file_path = os.path.join(dir_name, file_name)
     _write_to_file(file_path, contents)
     return file_path
 
 
 def _write_to_file(path: str, contents: List[str]) -> None:
     with open(path, "w") as new_file:
         for line in contents:
```

### Comparing `snowflake_cli_labs-2.1.2/tests/testing_utils/fixtures.py` & `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import functools
+import importlib
 import os
 import shutil
-import tempfile
 import sys
-import importlib
+import tempfile
 from contextlib import contextmanager
 from io import StringIO
 from pathlib import Path
 from typing import Generator, List, NamedTuple, Optional, Union
 from unittest import mock
 
 import pytest
-import strictyaml
+import yaml
 from snowflake.cli.api.project.definition import merge_left
+from snowflake.cli.app.cli_app import app_factory
 from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
-from strictyaml import as_document
 from typer import Typer
 from typer.testing import CliRunner
 
 from tests.test_data import test_data
 from tests.testing_utils.files_and_dirs import create_named_file, create_temp_file
 
 REQUIREMENTS_SNOWFLAKE = "requirements.snowflake.txt"
@@ -67,24 +67,17 @@
     req_txt = create_named_file(
         REQUIREMENTS_SNOWFLAKE, temp_dir, test_data.requirements
     )
     yield req_txt
     os.remove(req_txt)
 
 
-@pytest.fixture
-def dot_packages_directory(temp_dir):
-    dir_path = ".packages/totally-awesome-package"
-    os.makedirs(dir_path)
-    create_named_file("totally-awesome-module.py", dir_path, [])
-
-
 @pytest.fixture()
 def mock_ctx(mock_cursor):
-    return lambda cursor=mock_cursor(["row"], []): MockConnectionCtx(cursor)
+    yield lambda cursor=mock_cursor(["row"], []): MockConnectionCtx(cursor)
 
 
 class MockConnectionCtx(mock.MagicMock):
     def __init__(self, cursor=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.queries: List[str] = []
         self.cs = cursor
@@ -196,17 +189,16 @@
 def package_file():
     with tempfile.TemporaryDirectory() as tmp:
         yield create_named_file("app.zip", tmp, [])
 
 
 @pytest.fixture(scope="function")
 def runner(test_snowcli_config):
-    from snowflake.cli.app.cli_app import app
-
-    return SnowCLIRunner(app, test_snowcli_config)
+    app = app_factory()
+    yield SnowCLIRunner(app, test_snowcli_config)
 
 
 @pytest.fixture
 def temp_dir():
     initial_dir = os.getcwd()
     tmp = tempfile.TemporaryDirectory()
     os.chdir(tmp.name)
@@ -246,18 +238,20 @@
     @contextmanager
     def _temporary_project_directory(
         project_name, merge_project_definition: Optional[dict] = None
     ):
         test_data_file = test_root_path / "test_data" / "projects" / project_name
         shutil.copytree(test_data_file, temp_dir, dirs_exist_ok=True)
         if merge_project_definition:
-            project_definition = strictyaml.load(Path("snowflake.yml").read_text()).data
+            project_definition = yaml.load(
+                Path("snowflake.yml").read_text(), Loader=yaml.BaseLoader
+            )
             merge_left(project_definition, merge_project_definition)
             with open(Path(temp_dir) / "snowflake.yml", "w") as file:
-                file.write(as_document(project_definition).as_yaml())
+                file.write(yaml.dump(project_definition))
 
         yield Path(temp_dir)
 
     return _temporary_project_directory
 
 
 @pytest.fixture
@@ -291,15 +285,18 @@
         parts = parameter_path.split(".")
         current_object = yml
         while parts:
             part = parts.pop(0)
             evaluated_part = int(part) if part.isdigit() else part
 
             if parts:
-                current_object = current_object[evaluated_part]
+                if isinstance(current_object, dict):
+                    current_object = current_object.setdefault(evaluated_part, {})
+                else:
+                    current_object = current_object[evaluated_part]
             else:
                 current_object[evaluated_part] = value
 
         with open(snowflake_yml_path, "w+") as fh:
             yaml.safe_dump(yml, fh)
 
     return _update
```

### Comparing `snowflake_cli_labs-2.1.2/tests_e2e/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_e2e/test_error_handling.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_e2e/test_installation.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_e2e/test_snowpark_examples.py` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_e2e/__snapshots__/test_installation.ambr` & `snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,24 @@
   │ --info                       Shows information about the Snowflake CLI       │
   │ --config-file          FILE  Specifies Snowflake CLI configuration file that │
   │                              should be used                                  │
   │                              [default: None]                                 │
   │ --help         -h            Show this message and exit.                     │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
-  │ app         Manages a Snowflake Native App                                   │
-  │ connection  Manages connections to Snowflake.                                │
-  │ object      Manages Snowflake objects like warehouses and stages             │
-  │ snowpark    Manages procedures and functions.                                │
-  │ spcs        Manages Snowpark Container Services compute pools, services,     │
-  │             image registries, and image repositories.                        │
-  │ sql         Executes Snowflake query.                                        │
-  │ streamlit   Manages Streamlit in Snowflake.                                  │
+  │ app          Manages a Snowflake Native App                                  │
+  │ connection   Manages connections to Snowflake.                               │
+  │ git          Manages git repositories in Snowflake.                          │
+  │ object       Manages Snowflake objects like warehouses and stages            │
+  │ snowpark     Manages procedures and functions.                               │
+  │ spcs         Manages Snowpark Container Services compute pools, services,    │
+  │              image registries, and image repositories.                       │
+  │ sql          Executes Snowflake query.                                       │
+  │ stage        Manages stages.                                                 │
+  │ streamlit    Manages a Streamlit app in Snowflake.                           │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
 # name: test_snow_sql
   '''
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/conftest.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from json import JSONDecodeError
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pytest
-import strictyaml
+import yaml
+
 from snowflake.cli.api.cli_global_context import cli_context_manager
 from snowflake.cli.api.project.definition import merge_left
-from snowflake.cli.app.cli_app import app
-from strictyaml import as_document
+from snowflake.cli.app.cli_app import app_factory
 from typer import Typer
 from typer.testing import CliRunner
 
-from tests.conftest import clean_logging_handlers_fixture
-from tests.testing_utils.fixtures import alter_snowflake_yml, snowflake_home
+from tests.conftest import clean_logging_handlers_fixture  # noqa: F401
+from tests.testing_utils.fixtures import (
+    alter_snowflake_yml,  # noqa: F401
+    snowflake_home,
+)
 
 pytest_plugins = [
     "tests_integration.testing_utils",
     "tests_integration.snowflake_connector",
 ]
 
 TEST_DIR = Path(__file__).parent
@@ -109,37 +112,45 @@
         self, args, connection: str = "integration", **kwargs
     ) -> CommandResult:
         return self.invoke_with_config([*args, "-c", connection], **kwargs)
 
 
 @pytest.fixture
 def runner(test_snowcli_config_provider):
-    return SnowCLIRunner(app, test_snowcli_config_provider)
+    app = app_factory()
+    yield SnowCLIRunner(app, test_snowcli_config_provider)
 
 
 class QueryResultJsonEncoderError(RuntimeError):
     def __init__(self, output: str):
         super().__init__(f"Can not parse query result:\n{output}")
 
 
 @pytest.fixture
 def project_directory(temporary_working_directory, test_root_path):
     @contextmanager
     def _temporary_project_directory(
-        project_name, merge_project_definition: Optional[dict] = None
+        project_name,
+        merge_project_definition: Optional[dict] = None,
+        subpath: Optional[Path] = None,
     ):
         test_data_file = test_root_path / "test_data" / "projects" / project_name
-        shutil.copytree(test_data_file, temporary_working_directory, dirs_exist_ok=True)
+        project_dir = temporary_working_directory
+        if subpath:
+            project_dir = temporary_working_directory / subpath
+            project_dir.mkdir(parents=True)
+        shutil.copytree(test_data_file, project_dir, dirs_exist_ok=True)
         if merge_project_definition:
-            project_definition = strictyaml.load(Path("snowflake.yml").read_text()).data
+            with Path("snowflake.yml").open("r") as fh:
+                project_definition = yaml.safe_load(fh)
             merge_left(project_definition, merge_project_definition)
-            with open(Path(temporary_working_directory) / "snowflake.yml", "w") as file:
-                file.write(as_document(project_definition).as_yaml())
+            with open(Path(project_dir) / "snowflake.yml", "w") as file:
+                yaml.dump(project_definition, file)
 
-        yield temporary_working_directory
+        yield project_dir
 
     return _temporary_project_directory
 
 
 @pytest.fixture(autouse=True)
 def reset_global_context_after_each_test(request):
     cli_context_manager.reset()
@@ -147,10 +158,7 @@
 
 
 # This automatically used fixture isolates default location
 # of config files from user's system.
 @pytest.fixture(autouse=True)
 def isolate_snowflake_home(snowflake_home):
     yield snowflake_home
-
-
-__all__ = ["alter_snowflake_yml", "snowflake_home", "clean_logging_handlers_fixture"]
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/snowflake_connector.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,67 @@
 
 import os
 import uuid
 
 import pytest
 from snowflake import connector
 from snowflake.cli.api.exceptions import EnvironmentVariableNotFoundError
+from contextlib import contextmanager
+from unittest import mock
 
 _ENV_PARAMETER_PREFIX = "SNOWFLAKE_CONNECTIONS_INTEGRATION"
+SCHEMA_ENV_PARAMETER = f"{_ENV_PARAMETER_PREFIX}_SCHEMA"
+DATABASE_ENV_PARAMETER = f"{_ENV_PARAMETER_PREFIX}_DATABASE"
 
 
-@pytest.fixture(scope="function")
-def test_database(snowflake_session):
-    database_name = f"db_{uuid.uuid4().hex}"
+def add_uuid_to_name(name: str) -> str:
+    return f"{name}_{uuid.uuid4().hex}"
+
+
+@contextmanager
+def mock_single_env_var(name: str, value: str):
+    env = dict(os.environ)
+    env[name] = value
+    with mock.patch.dict(os.environ, env):
+        yield
+
+
+def _escape_name(name: str) -> str:
+    if "-" in name:
+        name = f'"{name}"'
+    return name
+
+
+@contextmanager
+def setup_test_database(snowflake_session, database_name: str):
+    database_name = _escape_name(database_name)
     snowflake_session.execute_string(
         f"create database {database_name}; use database {database_name}; use schema public;"
     )
-    os.environ[f"{_ENV_PARAMETER_PREFIX}_DATABASE"] = database_name
+    with mock_single_env_var(DATABASE_ENV_PARAMETER, value=database_name):
+        yield
+    snowflake_session.execute_string(f"drop database {database_name}")
 
-    yield database_name
 
-    snowflake_session.execute_string(f"drop database {database_name}")
-    del os.environ[f"{_ENV_PARAMETER_PREFIX}_DATABASE"]
+@contextmanager
+def setup_test_schema(snowflake_session, schema_name: str):
+    schema_name = _escape_name(schema_name)
+    snowflake_session.execute_string(
+        f"create schema {schema_name}; use schema {schema_name};"
+    )
+    with mock_single_env_var(SCHEMA_ENV_PARAMETER, value=schema_name):
+        yield
+    snowflake_session.execute_string(f"drop schema {schema_name}")
+
+
+@pytest.fixture(scope="function")
+def test_database(snowflake_session):
+    database_name = add_uuid_to_name("db")
+    with setup_test_database(snowflake_session, database_name):
+        yield database_name
 
 
 @pytest.fixture(scope="function")
 def test_role(snowflake_session):
     role_name = f"role_{uuid.uuid4().hex}"
     snowflake_session.execute_string(
         f"create role {role_name}; grant role {role_name} to user {snowflake_session.user};"
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_external_plugins.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,18 @@
     assert_that_result_is_successful_and_output_json_contains(
         result_of_multilingual_hello_fr, {"GREETING": "Salut John!"}
     )
 
 
 @pytest.mark.integration
 def test_loading_of_installed_plugins_if_only_one_plugin_is_enabled(
-    runner, install_plugins, caplog, reset_command_registration_state
+    runner,
+    install_plugins,
+    caplog,
+    reset_command_registration_state,
 ):
     runner.use_config("config_with_enabled_only_one_external_plugin.toml")
 
     result_of_top_level_help = runner.invoke_with_config(["--help"])
     assert_that_result_is_successful(result_of_top_level_help)
     _assert_that_no_error_logs(caplog)
     assert "multilingual-hello" not in result_of_top_level_help.output
@@ -107,39 +110,48 @@
     )
     assert_that_result_is_successful_and_output_json_contains(
         result_of_snowpark_hello, {"GREETING": "Hello John! You are in Snowpark!"}
     )
 
 
 @pytest.mark.integration
+@pytest.mark.parametrize(
+    "config_value",
+    (
+        pytest.param("1", id="integer as value"),
+        pytest.param('"True"', id="string as value"),
+    ),
+)
 def test_enabled_value_must_be_boolean(
-    runner, snowflake_home, reset_command_registration_state
+    config_value,
+    runner,
+    snowflake_home,
+    reset_command_registration_state,
 ):
     def _use_config_with_value(value):
         config = Path(snowflake_home) / "config.toml"
         config.write_text(
             f"""
 [cli.plugins.multilingual-hello]
 enabled = {value}"""
         )
         runner.use_config(config)
 
-    for value in ["1", '"True"']:
-        _use_config_with_value(value)
-        result = runner.invoke_with_config(["--help"])
-        output = result.output.splitlines()
-        assert all(
-            [
-                "Error" in output[0],
-                'Invalid plugin configuration. [multilingual-hello]: "enabled" must be a'
-                in output[1],
-                "boolean" in output[2],
-            ]
-        )
-        reset_command_registration_state()
+    _use_config_with_value(config_value)
+    result = runner.invoke_with_config(("--help,"))
+
+    first, second, third, *_ = result.output.splitlines()
+    assert "Error" in first, first
+    assert (
+        'Invalid plugin configuration. [multilingual-hello]: "enabled" must be a'
+        in second
+    ), second
+    assert "boolean" in third, third
+
+    reset_command_registration_state()
 
 
 def _assert_that_no_error_logs(caplog):
     error_logs = [
         record.message for record in caplog.records if record.levelname == "ERROR"
     ]
     assert error_logs == []
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_nativeapp.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py`

 * *Files 13% similar despite different names*

```diff
@@ -492,7 +492,75 @@
                     project_name,
                 ],
                 env=TEST_ENV,
             )
             assert result.exit_code == 0
         finally:
             single_template_repo.close()
+
+
+# Tests a simple flow of executing "snow app deploy", verifying that an application package was created, and an application was not
+@pytest.mark.integration
+def test_nativeapp_init_deploy(
+    runner,
+    snowflake_session,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    result = runner.invoke_json(
+        ["app", "init", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_name)):
+        result = runner.invoke_with_connection_json(
+            ["app", "deploy"],
+            env=TEST_ENV,
+        )
+        assert result.exit_code == 0
+
+        try:
+            # package exist
+            package_name = f"{project_name}_pkg_{USER_NAME}".upper()
+            app_name = f"{project_name}_{USER_NAME}".upper()
+            assert contains_row_with(
+                row_from_snowflake_session(
+                    snowflake_session.execute_string(
+                        f"show application packages like '{package_name}'",
+                    )
+                ),
+                dict(name=package_name),
+            )
+
+            # manifest file exists
+            stage_name = "app_src.stage"  # as defined in native-apps-templates/basic
+            stage_files = runner.invoke_with_connection_json(
+                ["stage", "list-files", f"{package_name}.{stage_name}"],
+                env=TEST_ENV,
+            )
+            assert contains_row_with(stage_files.json, {"name": "stage/manifest.yml"})
+
+            # app does not exist
+            assert not_contains_row_with(
+                row_from_snowflake_session(
+                    snowflake_session.execute_string(
+                        f"show applications like '{app_name}'",
+                    )
+                ),
+                dict(name=app_name),
+            )
+
+            # make sure we always delete the app
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_object.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_snowpark_external_access.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_sql.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_stage.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,57 @@
-import os
-import tempfile
-from pathlib import Path
-
 import pytest
 
-from tests_integration.test_utils import (
-    contains_row_with,
-    not_contains_row_with,
-    row_from_snowflake_session,
+from tests_integration.test_utils import row_from_snowflake_session
+from tests_integration.testing_utils.assertions.test_result_assertions import (
+    assert_that_result_is_successful_and_output_json_equals,
 )
+from tests_integration.testing_utils.naming_utils import ObjectNameProvider
 
 
 @pytest.mark.integration
-def test_stage(runner, snowflake_session, test_database, tmp_path):
-    stage_name = "test_stage"
+def test_token(runner):
+    result = runner.invoke_with_connection_json(["spcs", "image-registry", "token"])
 
-    result = runner.invoke_with_connection_json(
-        ["object", "stage", "create", stage_name]
-    )
-    assert contains_row_with(
-        result.json,
-        {"status": f"Stage area {stage_name.upper()} successfully created."},
-    )
+    assert result.exit_code == 0
+    assert result.json
+    assert "token" in result.json
+    assert result.json["token"]
+    assert "expires_in" in result.json
+    assert result.json["expires_in"]
 
-    result = runner.invoke_with_connection_json(["object", "list", "stage"])
-    expect = snowflake_session.execute_string(f"show stages like '{stage_name}'")
-    assert contains_row_with(result.json, row_from_snowflake_session(expect)[0])
-
-    filename = "test.txt"
-    with tempfile.TemporaryDirectory() as td:
-        file_path = os.path.join(td, filename)
-        Path(file_path).touch()
-
-        result = runner.invoke_with_connection_json(
-            ["object", "stage", "copy", file_path, f"@{stage_name}"]
-        )
-        assert result.exit_code == 0, result.output
-        assert contains_row_with(
-            result.json,
-            {"source": filename, "target": filename, "status": "UPLOADED"},
-        )
-
-    result = runner.invoke_with_connection_json(["object", "stage", "list", stage_name])
-    expect = snowflake_session.execute_string(f"list @{stage_name}")
-    assert result.json == row_from_snowflake_session(expect)
-
-    # Operation fails because directory exists
-    result = runner.invoke_with_connection_json(
-        ["object", "stage", "copy", f"@{stage_name}", tmp_path.parent.__str__()]
-    )
-    assert result.exit_code == 0, result.output
-    assert contains_row_with(result.json, {"file": filename, "status": "DOWNLOADED"})
-    assert os.path.isfile(tmp_path.parent / filename)
 
-    result = runner.invoke_with_connection_json(
-        ["object", "stage", "remove", stage_name, f"/{filename}"]
-    )
-    assert contains_row_with(
-        result.json,
-        {"name": f"{stage_name}/{filename}", "result": "removed"},
+@pytest.mark.integration
+def test_get_registry_url(test_database, test_role, runner, snowflake_session):
+    # newly created test_role should have no access to image repositories and should not be able to get registry URL
+    test_repo = ObjectNameProvider("test_repo").create_and_get_next_object_name()
+    snowflake_session.execute_string(f"create image repository {test_repo}")
+
+    fail_result = runner.invoke_with_connection(
+        ["spcs", "image-registry", "url", "--role", test_role]
+    )
+    assert fail_result.exit_code == 1, fail_result.output
+    assert "No image repository found." in fail_result.output
+
+    # role should be able to get registry URL once granted read access to an image repository
+    repo_list_cursor = snowflake_session.execute_string("show image repositories")
+    expected_repo_url = row_from_snowflake_session(repo_list_cursor)[0][
+        "repository_url"
+    ]
+    expected_registry_url = "/".join(expected_repo_url.split("/")[:-3])
+    snowflake_session.execute_string(
+        f"grant usage on database {snowflake_session.database} to role {test_role};"
+        f"grant usage on schema {snowflake_session.schema} to role {test_role};"
+        f"grant read on image repository {test_repo} to role {test_role};"
     )
-    expect = snowflake_session.execute_string(f"list @{stage_name}")
-    assert not_contains_row_with(
-        row_from_snowflake_session(expect), {"name": f"{stage_name}/{filename}"}
+    success_result = runner.invoke_with_connection(
+        ["spcs", "image-registry", "url", "--role", test_role]
     )
+    assert success_result.exit_code == 0, success_result.output
+    assert success_result.output.strip() == expected_registry_url
 
-    result = runner.invoke_with_connection_json(["object", "drop", "stage", stage_name])
-    assert contains_row_with(
-        result.json,
-        {"status": f"{stage_name.upper()} successfully dropped."},
+
+@pytest.mark.integration
+def test_registry_login(runner):
+    result = runner.invoke_with_connection_json(["spcs", "image-registry", "login"])
+    assert_that_result_is_successful_and_output_json_equals(
+        result, {"message": "Login Succeeded"}
     )
-    expect = snowflake_session.execute_string(f"show stages like '%{stage_name}%'")
-    assert row_from_snowflake_session(expect) == []
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_streamlit.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py`

 * *Files 20% similar despite different names*

```diff
@@ -145,23 +145,76 @@
     expect = snowflake_session.execute_string(
         f"show streamlits like '{streamlit_name}'"
     )
     assert row_from_snowflake_session(expect) == []
 
 
 @pytest.mark.integration
-def test_streamlit_is_visible_in_anaconda_channel():
-    from requirements.requirement import Requirement
-    from snowflake.cli.plugins.snowpark.package_utils import parse_anaconda_packages
-
-    streamlit = Requirement.parse_line("streamlit")
-
-    result = parse_anaconda_packages([streamlit])
+def test_fully_qualified_name(
+    alter_snowflake_yml, test_database, project_directory, runner, snapshot
+):
+    default_schema = "PUBLIC"
+    different_schema = "TOTALLY_DIFFERENT_SCHEMA"
+    database = test_database.upper()
+    assert (
+        runner.invoke_with_connection(
+            ["sql", "-q", f"create schema {database}.{different_schema}"]
+        ).exit_code
+        == 0
+    )
 
-    assert streamlit in result.snowflake
+    # test fully qualified name as name
+    with project_directory("streamlit") as tmp_dir:
+        streamlit_name = "streamlit_fqn"
+        snowflake_yml = tmp_dir / "snowflake.yml"
+
+        # FQN with "default" values
+        alter_snowflake_yml(
+            snowflake_yml,
+            parameter_path="streamlit.name",
+            value=f"{database}.{default_schema}.{streamlit_name}",
+        )
+        result = runner.invoke_with_connection_json(["streamlit", "deploy"])
+        assert result.exit_code == 0
+        assert result.json == {
+            "message": "Streamlit successfully deployed and available under "
+            f"https://app.snowflake.com/SFENGINEERING/snowcli_it/#/streamlit-apps/{database}.{default_schema}.{streamlit_name.upper()}",
+        }
+
+        # FQN with different schema - should not conflict
+        alter_snowflake_yml(
+            snowflake_yml,
+            parameter_path="streamlit.name",
+            value=f"{database}.{different_schema}.{streamlit_name}",
+        )
+        result = runner.invoke_with_connection_json(["streamlit", "deploy"])
+        assert result.exit_code == 0
+        assert result.json == {
+            "message": "Streamlit successfully deployed and available under "
+            f"https://app.snowflake.com/SFENGINEERING/snowcli_it/#/streamlit-apps/{database}.{different_schema}.{streamlit_name.upper()}",
+        }
+
+        # FQN with just schema provided - should update
+        alter_snowflake_yml(
+            snowflake_yml,
+            parameter_path="streamlit.name",
+            value=f"{different_schema}.{streamlit_name}",
+        )
+        result = runner.invoke_with_connection(
+            ["streamlit", "deploy"], catch_exceptions=True
+        )
+        assert result.exit_code == 1
+        result = runner.invoke_with_connection_json(
+            ["streamlit", "deploy", "--replace"]
+        )
+        assert result.exit_code == 0
+        assert result.json == {
+            "message": "Streamlit successfully deployed and available under "
+            f"https://app.snowflake.com/SFENGINEERING/snowcli_it/#/streamlit-apps/{database}.{different_schema}.{streamlit_name.upper()}",
+        }
 
 
 @pytest.fixture
 def _new_streamlit_role(snowflake_session, test_database):
     role_name = f"snowcli_streamlit_role_{uuid.uuid4().hex}"
     result = snowflake_session.execute_string(
         f"set user = (select current_user()); "
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_temporary_connection.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/test_image_repository.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def _list_tags(runner):
     result = runner.invoke_with_connection_json(
         [
             "spcs",
             "image-repository",
             "list-tags",
             "snowcli_repository",
-            "--image_name",
+            "--image-name",
             f"/{INTEGRATION_DATABASE}/{INTEGRATION_SCHEMA}/{INTEGRATION_REPOSITORY}/snowpark_test_echo",
             "--database",
             INTEGRATION_DATABASE,
             "--schema",
             INTEGRATION_SCHEMA,
         ]
     )
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/test_jobs.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/test_registry.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,81 @@
-import pytest
+import json
 
-from tests_integration.test_utils import row_from_snowflake_session
-from tests_integration.testing_utils.assertions.test_result_assertions import (
-    assert_that_result_is_successful_and_output_json_equals,
-)
-from tests_integration.testing_utils.naming_utils import ObjectNameProvider
-
-
-@pytest.mark.integration
-def test_token(runner):
-    result = runner.invoke_with_connection_json(["spcs", "image-registry", "token"])
-
-    assert result.exit_code == 0
-    assert result.json
-    assert "token" in result.json
-    assert result.json["token"]
-    assert "expires_in" in result.json
-    assert result.json["expires_in"]
-
-
-@pytest.mark.integration
-def test_get_registry_url(test_database, test_role, runner, snowflake_session):
-    # newly created test_role should have no access to image repositories and should not be able to get registry URL
-    test_repo = ObjectNameProvider("test_repo").create_and_get_next_object_name()
-    snowflake_session.execute_string(f"create image repository {test_repo}")
-
-    fail_result = runner.invoke_with_connection(
-        ["spcs", "image-registry", "url", "--role", test_role]
-    )
-    assert fail_result.exit_code == 1, fail_result.output
-    assert "No image repository found." in fail_result.output
-
-    # role should be able to get registry URL once granted read access to an image repository
-    repo_list_cursor = snowflake_session.execute_string("show image repositories")
-    expected_repo_url = row_from_snowflake_session(repo_list_cursor)[0][
-        "repository_url"
-    ]
-    expected_registry_url = "/".join(expected_repo_url.split("/")[:-3])
-    snowflake_session.execute_string(
-        f"grant usage on database {snowflake_session.database} to role {test_role};"
-        f"grant usage on schema {snowflake_session.schema} to role {test_role};"
-        f"grant read on image repository {test_repo} to role {test_role};"
-    )
-    success_result = runner.invoke_with_connection(
-        ["spcs", "image-registry", "url", "--role", test_role]
-    )
-    assert success_result.exit_code == 0, success_result.output
-    assert success_result.output.strip() == expected_registry_url
-
-
-@pytest.mark.integration
-def test_registry_login(runner):
-    result = runner.invoke_with_connection_json(["spcs", "image-registry", "login"])
-    assert_that_result_is_successful_and_output_json_equals(
-        result, {"message": "Login Succeeded"}
-    )
+from snowflake.connector import SnowflakeConnection
+
+from tests_integration.conftest import SnowCLIRunner
+from tests_integration.test_utils import contains_row_with
+
+
+class SnowparkJobsTestSetup:
+    def __init__(
+        self,
+        runner: SnowCLIRunner,
+        snowflake_session: SnowflakeConnection,
+        test_root_path,
+    ):
+        self.runner = runner
+        self.snowflake_session = snowflake_session
+        self.test_root_path = test_root_path
+
+
+class SnowparkJobsTestSteps:
+    compute_pool = "snowcli_compute_pool"
+    database = "snowcli_db"
+    schema = "public"
+
+    def __init__(self, setup: SnowparkJobsTestSetup):
+        self._setup = setup
+
+    def create_job(self) -> str:
+        result = self._setup.runner.invoke_with_connection_json(
+            [
+                "spcs",
+                "job",
+                "create",
+                "--compute-pool",
+                self.compute_pool,
+                "--spec-path",
+                f"{self._setup.test_root_path}/spcs/spec/spec.yml",
+                "--database",
+                self.database,
+                "--schema",
+                self.schema,
+            ],
+        )
+        assert isinstance(result.json, dict), result.output
+        status = result.json["status"]
+        assert status.__contains__("completed successfully")
+        return status.replace("Job ", "").replace(
+            " completed successfully with status: DONE.", ""
+        )
+
+    def status_should_return_job(self, job_id: str) -> None:
+        result = self._setup.runner.invoke_with_connection_json(
+            ["spcs", "job", "status", job_id], connection="spcs"
+        )
+        assert isinstance(result.json, dict)
+        status_json = result.json["SYSTEM$GET_JOB_STATUS"]
+        status = json.loads(status_json)
+        assert contains_row_with(
+            status,
+            {
+                "serviceName": job_id,
+                "status": "DONE",
+                "message": "Completed successfully",
+            },
+        )
+
+    def logs_should_return_job_logs(self, job_id: str) -> None:
+        result = self._setup.runner.invoke_with_connection(
+            ["spcs", "job", "logs", job_id, "--container-name", "hello-world"],
+        )
+        assert result.output
+        assert result.output.strip() == f"{job_id}/0 Hello World!"
+
+    def drop_job(self, job_id: str) -> None:
+        result = self._setup.runner.invoke_with_connection_json(
+            ["spcs", "job", "drop", job_id],
+        )
+        assert result.json == {
+            "SYSTEM$CANCEL_JOB": f"Job {job_id} successfully terminated"
+        }
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/test_services.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/docker/echo_service.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/testing_utils/compute_pool_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/spcs/testing_utils/spcs_services_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark/app/app.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml` & `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/testing_utils/naming_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/testing_utils/snowpark_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 import os
 import re
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Tuple, Optional
 from zipfile import ZipFile
 
 from syrupy import SnapshotAssertion
 
 from tests_integration.conftest import SnowCLIRunner
 from tests_integration.testing_utils import assert_that_result_is_error
 from tests_integration.testing_utils.assertions.test_file_assertions import (
@@ -111,17 +111,19 @@
 
         entity_name = identifier.rsplit("(")[0]
 
         assert_that_result_is_successful(result)
         assert_that_result_contains_row_with(
             result,
             {
-                identifier.upper()
-                if object_type == TestType.FUNCTION.value
-                else entity_name.upper(): expected_value
+                (
+                    identifier.upper()
+                    if object_type == TestType.FUNCTION.value
+                    else entity_name.upper()
+                ): expected_value
             },
         )
 
     def object_describe_should_return_entity_description(
         self,
         object_type: str,
         identifier: str,
@@ -143,30 +145,33 @@
                 result, {"property": "returns", "value": returns}
             )
         assert_that_result_contains_row_with(
             result, {"property": "signature", "value": signature}
         )
         assert result.json is not None
 
-    def snowpark_build_should_zip_files(self, *args) -> None:
+    def snowpark_build_should_zip_files(self, *args, additional_files=None) -> None:
+        if not additional_files:
+            additional_files = []
+
         current_files = set(Path(".").glob("**/*"))
         result = self._setup.runner.invoke_json(
-            ["snowpark", "build", "--pypi-download", "yes", "--format", "JSON", *args]
+            ["snowpark", "build", "--format", "JSON", *args]
         )
 
         assert result.exit_code == 0, result.output
         assert result.json, result.output
         assert "message" in result.json
         assert "Build done. Artifact path:" in result.json["message"]  # type: ignore
 
         assert_that_current_working_directory_contains_only_following_files(
             *current_files,
             Path("app.zip"),
+            *additional_files,
             Path("requirements.snowflake.txt"),
-            Path("requirements.other.txt"),
             excluded_paths=[".packages"],
         )
 
     def snowpark_deploy_with_coverage_wrapper_should_finish_successfully_and_return(
         self, expected_result: List[Dict[str, str]]
     ):
         return self._run_deploy(expected_result, ["--install-coverage-wrapper"])
@@ -177,23 +182,23 @@
         additional_arguments: List[str] = [],
     ):
         self._run_deploy(expected_result, additional_arguments)
 
     def _run_deploy(
         self,
         expected_result: List[Dict[str, str]],
-        additional_arguments: List[str] = [],
+        additional_arguments: Optional[List[str]] = None,
     ):
         arguments = [
             "snowpark",
             "deploy",
         ]
 
         if additional_arguments:
-            arguments.append(*additional_arguments)
+            arguments.extend(additional_arguments)
 
         result = self._setup.runner.invoke_with_connection_json(arguments)
         assert_that_result_is_successful(result)
         assert result.json == expected_result
 
     def snowpark_deploy_should_return_error_with_message_contains(
         self, message_contains: str
@@ -218,15 +223,15 @@
                 identifier,
             ]
         )
         assert_that_result_is_successful(result)
 
     def package_should_build_proper_artifact(self, package_name: str, file_name: str):
         result = self._setup.runner.invoke_with_connection_json(
-            ["snowpark", "package", "create", package_name, "-y"]
+            ["snowpark", "package", "create", package_name, "--pypi-download"]
         )
 
         assert result.exit_code == 0
         assert os.path.isfile(f"{package_name}.zip")
         assert file_name in ZipFile(f"{package_name}.zip").namelist()
 
     def package_should_upload_artifact_to_stage(self, file_name, stage_name):
```

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/testing_utils/sql_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/testing_utils/working_directory_utils.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/tests_integration/testing_utils/assertions/test_result_assertions.py` & `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/LICENSE` & `snowflake_cli_labs-2.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.1.2/pyproject.toml` & `snowflake_cli_labs-2.2.0rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 authors = [{ name = "Snowflake Inc." }]
 license = { file = "LICENSE" }
 dynamic = ["version"]
 requires-python = ">=3.8"
 description = "Snowflake CLI"
 readme = "README.md"
 dependencies = [
-  "coverage==7.4.1",
   "jinja2==3.1.3",
   "pluggy==1.4.0",
   "PyYAML==6.0.1",
-  "rich==13.7.0",
+  "rich==13.7.1",
   "requests==2.31.0",
-  "requirements-parser==0.5.0",
-  "setuptools==69.1.0",
-  "snowflake-connector-python[secure-local-storage]==3.7.0",
-  "strictyaml==1.7.3",
+  "requirements-parser==0.9.0",
+  "setuptools==69.5.1",
+  "snowflake-connector-python[secure-local-storage]==3.8.1",
   "tomlkit==0.12.3",
-  "typer==0.9.0",
+  "typer==0.12.3",
   "urllib3>=1.21.1,<2.3",
-  "GitPython==3.1.42",
+  "GitPython==3.1.43",
   "pip",
+  "pydantic==2.7.0"
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
@@ -37,24 +36,24 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: SQL",
   "Topic :: Database",
 ]
 
 [project.optional-dependencies]
 development = [
-  "coverage==7.4.1",
+  "coverage==7.4.4",
   "pre-commit>=3.5.0",
-  "pytest==8.0.1",
+  "pytest==8.1.1",
   "pytest-randomly==3.15.0",
   "syrupy==4.6.1",
 ]
 
 [project.urls]
-"Source code" = "https://github.com/Snowflake-Labs/snowcli"
-"Bug Tracker" = "https://github.com/Snowflake-Labs/snowcli/issues"
+"Source code" = "https://github.com/snowflakedb/snowflake-cli"
+"Bug Tracker" = "https://github.com/snowflakedb/snowflake-cli/issues"
 
 [project.scripts]
 snow = "snowflake.cli.app.__main__:main"
 
 [tool.coverage.report]
 exclude_also = ["@(abc\\.)?abstractmethod", "@(abc\\.)?abstractproperty"]
 
@@ -118,17 +117,22 @@
   "I",      # isort
   "G",      # flake8-logging-format
   "N",      # pep8 naming
   "A",      # flake 8 builtins
   "TID252", # relative imports
   "SLF",    # Accessing private methods
   "F401",   # unused imports
+  "F403",   # star imports
 ]
 
 [tool.pytest.ini_options]
 addopts = "-m 'not integration and not performance and not e2e and not spcs and not loaded_modules'"
 markers = [
   "integration: mark test as integration test",
   "performance: mark test as performance test",
-  "e2e: mark test to execute on SnowCLI installed in fresh virtual environment",
+  "e2e: mark test to execute on Snowflake CLI installed in fresh virtual environment",
   "loaded_modules: checks loaded modules",
 ]
+
+
+[tool.codespell]
+skip = 'tests/*'
```

### Comparing `snowflake_cli_labs-2.1.2/PKG-INFO` & `snowflake_cli_labs-2.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: snowflake-cli-labs
-Version: 2.1.2
+Version: 2.2.0rc0
 Summary: Snowflake CLI
-Project-URL: Source code, https://github.com/Snowflake-Labs/snowcli
-Project-URL: Bug Tracker, https://github.com/Snowflake-Labs/snowcli/issues
+Project-URL: Source code, https://github.com/snowflakedb/snowflake-cli
+Project-URL: Bug Tracker, https://github.com/snowflakedb/snowflake-cli/issues
 Author: Snowflake Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -213,42 +213,45 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Requires-Python: >=3.8
-Requires-Dist: coverage==7.4.1
-Requires-Dist: gitpython==3.1.42
+Requires-Dist: gitpython==3.1.43
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: pip
 Requires-Dist: pluggy==1.4.0
+Requires-Dist: pydantic==2.7.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requirements-parser==0.5.0
-Requires-Dist: rich==13.7.0
-Requires-Dist: setuptools==69.1.0
-Requires-Dist: snowflake-connector-python[secure-local-storage]==3.7.0
-Requires-Dist: strictyaml==1.7.3
+Requires-Dist: requirements-parser==0.9.0
+Requires-Dist: rich==13.7.1
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: snowflake-connector-python[secure-local-storage]==3.8.1
 Requires-Dist: tomlkit==0.12.3
-Requires-Dist: typer==0.9.0
+Requires-Dist: typer==0.12.3
 Requires-Dist: urllib3<2.3,>=1.21.1
 Provides-Extra: development
-Requires-Dist: coverage==7.4.1; extra == 'development'
+Requires-Dist: coverage==7.4.4; extra == 'development'
 Requires-Dist: pre-commit>=3.5.0; extra == 'development'
 Requires-Dist: pytest-randomly==3.15.0; extra == 'development'
-Requires-Dist: pytest==8.0.1; extra == 'development'
+Requires-Dist: pytest==8.1.1; extra == 'development'
 Requires-Dist: syrupy==4.6.1; extra == 'development'
 Description-Content-Type: text/markdown
 
-# Snowflake Developer CLI
+# Snowflake CLI
+
+Snowflake CLI is an open-source command-line tool explicitly designed for developer-centric workloads in addition to SQL operations. It is a flexible and extensible tool that can accommodate modern development practices and technologies.
+
+With Snowflake CLI, developers can create, manage, update, and view apps running on Snowflake across workloads such as Streamlit in Snowflake, the Snowflake Native App Framework, Snowpark Container Services, and Snowpark. It supports a range of Snowflake features, including user-defined functions, stored procedures, Streamlit in Snowflake, and SQL execution.
+
+
+**Note**: Snowflake CLI is in Public Preview (PuPr). Docs at https://docs.snowflake.com/en/developer-guide/snowflake-cli-v2/index
 
-**Note**: Snowflake CLI is in Private Preview (PrPr). You must register for the PrPr to use Snowflake CLI by filling out the
-[Snowflake CLI  - PrPr Intake Form](https://forms.gle/HZNhPNbzn7oExjFu8). For more information, you can contact a
-Snowflake sales representative.
 
 ## Install Snowflake CLI
 
 ### Install with pip (PyPi)
 
 Requires Python >= 3.8
 
@@ -259,25 +262,25 @@
 
 ### Install with Homebrew (Mac only)
 
 Requires [Homebrew](https://brew.sh/).
 
 ```bash
 brew tap Snowflake-Labs/snowflake-cli
-brew install snowcli
+brew install snowflake-cli
 snow --help
 ```
 
 ### Install from source
 
 Requires Python >= 3.8 and git
 
 ```bash
-git clone https://github.com/snowflake-labs/snowcli
-cd snowcli
+git clone https://github.com/snowflakedb/snowflake-cli
+cd snowflake-cli
 # you can also do the below in an active virtual environment:
 # python -m venv .venv
 # source .venv/bin/activate
 hatch build && pip install .
 snow --version
 ```
```

