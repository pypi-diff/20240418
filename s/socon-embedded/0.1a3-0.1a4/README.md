# Comparing `tmp/socon-embedded-0.1a3.tar.gz` & `tmp/socon_embedded-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socon-embedded-0.1a3.tar", last modified: Fri Apr 12 09:06:54 2024, max compression
+gzip compressed data, was "socon_embedded-0.1a4.tar", last modified: Thu Apr 18 13:03:21 2024, max compression
```

## Comparing `socon-embedded-0.1a3.tar` & `socon_embedded-0.1a4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.563077 socon-embedded-0.1a3/
--rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/.gitignore
--rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/AUTHORS
--rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/LICENSE
--rw-rw-rw-   0        0        0     1767 2024-04-12 09:06:54.560061 socon-embedded-0.1a3/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/README.rst
--rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon-embedded-0.1a3/__init__.py
--rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/plugins.py
--rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/pyproject.toml
--rw-rw-rw-   0        0        0       98 2024-01-25 15:49:53.000000 socon-embedded-0.1a3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 09:06:54.564079 socon-embedded-0.1a3/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.060394 socon-embedded-0.1a3/socon_embedded/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/__init__.py
--rw-rw-rw-   0        0        0      424 2024-04-12 09:06:52.000000 socon-embedded-0.1a3/socon_embedded/_version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.177153 socon-embedded-0.1a3/socon_embedded/action/
--rw-rw-rw-   0        0        0      771 2024-04-11 12:13:38.000000 socon-embedded-0.1a3/socon_embedded/action/__init__.py
--rw-rw-rw-   0        0        0      664 2024-04-11 09:42:54.000000 socon-embedded-0.1a3/socon_embedded/action/call.py
--rw-rw-rw-   0        0        0     2917 2024-04-11 09:41:05.000000 socon-embedded-0.1a3/socon_embedded/action/copy.py
--rw-rw-rw-   0        0        0      256 2024-04-11 09:44:01.000000 socon-embedded-0.1a3/socon_embedded/action/move.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.192909 socon-embedded-0.1a3/socon_embedded/builder/
--rw-rw-rw-   0        0        0    10354 2024-04-11 13:05:46.000000 socon-embedded-0.1a3/socon_embedded/builder/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon-embedded-0.1a3/socon_embedded/builder/parser.py
--rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon-embedded-0.1a3/socon_embedded/builder/result.py
--rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.214996 socon-embedded-0.1a3/socon_embedded/executor/
--rw-rw-rw-   0        0        0        0 2024-04-11 11:55:38.000000 socon-embedded-0.1a3/socon_embedded/executor/__init__.py
--rw-rw-rw-   0        0        0    10090 2024-04-11 13:37:06.000000 socon-embedded-0.1a3/socon_embedded/executor/app_executor.py
--rw-rw-rw-   0        0        0     4370 2024-04-11 13:38:20.000000 socon-embedded-0.1a3/socon_embedded/executor/task_executor.py
--rw-rw-rw-   0        0        0      818 2024-04-11 12:15:08.000000 socon-embedded-0.1a3/socon_embedded/executor/task_result.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.219715 socon-embedded-0.1a3/socon_embedded/management/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.230012 socon-embedded-0.1a3/socon_embedded/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/management/commands/__init__.py
--rw-rw-rw-   0        0        0     7842 2024-04-11 13:07:03.000000 socon-embedded-0.1a3/socon_embedded/management/commands/build.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.241254 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/
--rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1956 2024-04-11 12:47:56.000000 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/from_file.py
--rw-rw-rw-   0        0        0     2950 2024-04-12 07:54:43.000000 socon-embedded-0.1a3/socon_embedded/managers.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.260404 socon-embedded-0.1a3/socon_embedded/schema/
--rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon-embedded-0.1a3/socon_embedded/schema/__init__.py
--rw-rw-rw-   0        0        0     8498 2024-04-11 12:13:57.000000 socon-embedded-0.1a3/socon_embedded/schema/apps.py
--rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/schema/base.py
--rw-rw-rw-   0        0        0     3734 2024-04-12 09:00:31.000000 socon-embedded-0.1a3/socon_embedded/schema/task.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.287245 socon-embedded-0.1a3/socon_embedded/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/utils/__init__.py
--rw-rw-rw-   0        0        0     2523 2024-04-04 12:31:10.000000 socon-embedded-0.1a3/socon_embedded/utils/converter.py
--rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/utils/jinja.py
--rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/utils/loader.py
--rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/utils/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.553450 socon-embedded-0.1a3/socon_embedded.egg-info/
--rw-rw-rw-   0        0        0     1767 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2529 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.307933 socon-embedded-0.1a3/tests/
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.345221 socon-embedded-0.1a3/tests/action/
--rw-rw-rw-   0        0        0      267 2024-04-11 12:46:08.000000 socon-embedded-0.1a3/tests/action/__init__.py
--rw-rw-rw-   0        0        0      720 2024-04-11 12:45:24.000000 socon-embedded-0.1a3/tests/action/test_call_command.py
--rw-rw-rw-   0        0        0     1755 2024-04-11 12:44:43.000000 socon-embedded-0.1a3/tests/action/test_copy.py
--rw-rw-rw-   0        0        0      626 2024-04-12 08:59:07.000000 socon-embedded-0.1a3/tests/action/test_discover.py
--rw-rw-rw-   0        0        0        0 2024-04-11 12:45:29.000000 socon-embedded-0.1a3/tests/action/test_move.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.365882 socon-embedded-0.1a3/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:32:35.000000 socon-embedded-0.1a3/tests/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.380365 socon-embedded-0.1a3/tests/commands/datafixtures/
--rw-rw-rw-   0        0        0      397 2024-04-11 13:02:05.000000 socon-embedded-0.1a3/tests/commands/datafixtures/simple_app_config.yml
--rw-rw-rw-   0        0        0      493 2024-04-11 13:02:22.000000 socon-embedded-0.1a3/tests/commands/datafixtures/simple_app_with_task.yml
--rw-rw-rw-   0        0        0      370 2024-04-11 12:36:04.000000 socon-embedded-0.1a3/tests/commands/test_build_command.py
--rw-rw-rw-   0        0        0      439 2024-04-12 08:53:56.000000 socon-embedded-0.1a3/tests/commands/test_from_file.py
--rw-rw-rw-   0        0        0      330 2024-04-12 08:52:00.000000 socon-embedded-0.1a3/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.404499 socon-embedded-0.1a3/tests/executor/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:18:37.000000 socon-embedded-0.1a3/tests/executor/__init__.py
--rw-rw-rw-   0        0        0       72 2024-04-11 12:28:37.000000 socon-embedded-0.1a3/tests/executor/test_task_executor.py
--rw-rw-rw-   0        0        0      580 2024-04-11 12:23:44.000000 socon-embedded-0.1a3/tests/executor/test_task_result.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.416931 socon-embedded-0.1a3/tests/management/
--rw-rw-rw-   0        0        0        0 2024-04-11 12:58:57.000000 socon-embedded-0.1a3/tests/management/__init__.py
--rw-rw-rw-   0        0        0       33 2024-04-11 12:59:16.000000 socon-embedded-0.1a3/tests/management/config.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.426288 socon-embedded-0.1a3/tests/projects/
--rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon-embedded-0.1a3/tests/projects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.457763 socon-embedded-0.1a3/tests/projects/test_project/
--rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon-embedded-0.1a3/tests/projects/test_project/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-12 08:56:26.000000 socon-embedded-0.1a3/tests/projects/test_project/action.py
--rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/projects/test_project/builder.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.464141 socon-embedded-0.1a3/tests/projects/test_project/management/
--rw-rw-rw-   0        0        0       33 2024-04-12 08:51:00.000000 socon-embedded-0.1a3/tests/projects/test_project/management/config.py
--rw-rw-rw-   0        0        0      171 2024-04-12 08:51:38.000000 socon-embedded-0.1a3/tests/projects/test_project/projects.py
--rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/pytest.ini
--rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/tests/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.486348 socon-embedded-0.1a3/tests/schema/
--rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/schema/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.533233 socon-embedded-0.1a3/tests/schema/datafixtures/
--rw-rw-rw-   0        0        0       80 2024-04-04 13:07:32.000000 socon-embedded-0.1a3/tests/schema/datafixtures/action_extra_args.yml
--rw-rw-rw-   0        0        0       47 2024-04-02 13:14:24.000000 socon-embedded-0.1a3/tests/schema/datafixtures/bad_action.yml
--rw-rw-rw-   0        0        0       59 2024-04-02 13:13:17.000000 socon-embedded-0.1a3/tests/schema/datafixtures/copy_schema.yml
--rw-rw-rw-   0        0        0       91 2024-04-02 15:27:00.000000 socon-embedded-0.1a3/tests/schema/datafixtures/multiple_valid_action.yml
--rw-rw-rw-   0        0        0       19 2024-04-02 15:22:54.000000 socon-embedded-0.1a3/tests/schema/datafixtures/no_action.yml
--rw-rw-rw-   0        0        0       77 2024-04-02 13:15:18.000000 socon-embedded-0.1a3/tests/schema/datafixtures/set_action.yml
--rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/schema/test_app_registry.py
--rw-rw-rw-   0        0        0     2652 2024-04-11 12:14:54.000000 socon-embedded-0.1a3/tests/schema/test_tasks.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.545081 socon-embedded-0.1a3/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tests/utils/test_splitter.py
--rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.261208 socon_embedded-0.1a4/
+-rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/.gitignore
+-rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/AUTHORS
+-rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/LICENSE
+-rw-rw-rw-   0        0        0     1767 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/README.rst
+-rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon_embedded-0.1a4/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/plugins.py
+-rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/pyproject.toml
+-rw-rw-rw-   0        0        0       98 2024-01-25 15:49:53.000000 socon_embedded-0.1a4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:03:21.261208 socon_embedded-0.1a4/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.736597 socon_embedded-0.1a4/socon_embedded/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.817664 socon_embedded-0.1a4/socon_embedded/action/
+-rw-rw-rw-   0        0        0      771 2024-04-11 12:13:38.000000 socon_embedded-0.1a4/socon_embedded/action/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-04-11 09:42:54.000000 socon_embedded-0.1a4/socon_embedded/action/call.py
+-rw-rw-rw-   0        0        0     2917 2024-04-11 09:41:05.000000 socon_embedded-0.1a4/socon_embedded/action/copy.py
+-rw-rw-rw-   0        0        0      256 2024-04-11 09:44:01.000000 socon_embedded-0.1a4/socon_embedded/action/move.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.847310 socon_embedded-0.1a4/socon_embedded/builder/
+-rw-rw-rw-   0        0        0    10354 2024-04-11 13:05:46.000000 socon_embedded-0.1a4/socon_embedded/builder/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon_embedded-0.1a4/socon_embedded/builder/parser.py
+-rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon_embedded-0.1a4/socon_embedded/builder/result.py
+-rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.878832 socon_embedded-0.1a4/socon_embedded/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:55:38.000000 socon_embedded-0.1a4/socon_embedded/executor/__init__.py
+-rw-rw-rw-   0        0        0    10090 2024-04-11 13:37:06.000000 socon_embedded-0.1a4/socon_embedded/executor/app_executor.py
+-rw-rw-rw-   0        0        0     4352 2024-04-12 12:59:49.000000 socon_embedded-0.1a4/socon_embedded/executor/task_executor.py
+-rw-rw-rw-   0        0        0      818 2024-04-11 12:15:08.000000 socon_embedded-0.1a4/socon_embedded/executor/task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.888949 socon_embedded-0.1a4/socon_embedded/management/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.903704 socon_embedded-0.1a4/socon_embedded/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     7842 2024-04-11 13:07:03.000000 socon_embedded-0.1a4/socon_embedded/management/commands/build.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.909263 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/
+-rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     1956 2024-04-11 12:47:56.000000 socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/from_file.py
+-rw-rw-rw-   0        0        0     2950 2024-04-12 07:54:43.000000 socon_embedded-0.1a4/socon_embedded/managers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.940645 socon_embedded-0.1a4/socon_embedded/schema/
+-rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon_embedded-0.1a4/socon_embedded/schema/__init__.py
+-rw-rw-rw-   0        0        0     8498 2024-04-11 12:13:57.000000 socon_embedded-0.1a4/socon_embedded/schema/apps.py
+-rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/schema/base.py
+-rw-rw-rw-   0        0        0     4133 2024-04-18 13:01:30.000000 socon_embedded-0.1a4/socon_embedded/schema/task.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:20.981744 socon_embedded-0.1a4/socon_embedded/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon_embedded-0.1a4/socon_embedded/utils/__init__.py
+-rw-rw-rw-   0        0        0     2523 2024-04-04 12:31:10.000000 socon_embedded-0.1a4/socon_embedded/utils/converter.py
+-rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/utils/jinja.py
+-rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon_embedded-0.1a4/socon_embedded/utils/loader.py
+-rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon_embedded-0.1a4/socon_embedded/utils/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/socon_embedded.egg-info/
+-rw-rw-rw-   0        0        0     1767 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2529 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-18 13:03:20.000000 socon_embedded-0.1a4/socon_embedded.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.004200 socon_embedded-0.1a4/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.054293 socon_embedded-0.1a4/tests/action/
+-rw-rw-rw-   0        0        0      267 2024-04-11 12:46:08.000000 socon_embedded-0.1a4/tests/action/__init__.py
+-rw-rw-rw-   0        0        0      720 2024-04-11 12:45:24.000000 socon_embedded-0.1a4/tests/action/test_call_command.py
+-rw-rw-rw-   0        0        0     1755 2024-04-11 12:44:43.000000 socon_embedded-0.1a4/tests/action/test_copy.py
+-rw-rw-rw-   0        0        0      626 2024-04-12 08:59:07.000000 socon_embedded-0.1a4/tests/action/test_discover.py
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:45:29.000000 socon_embedded-0.1a4/tests/action/test_move.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.075089 socon_embedded-0.1a4/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:32:35.000000 socon_embedded-0.1a4/tests/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.085297 socon_embedded-0.1a4/tests/commands/datafixtures/
+-rw-rw-rw-   0        0        0      397 2024-04-11 13:02:05.000000 socon_embedded-0.1a4/tests/commands/datafixtures/simple_app_config.yml
+-rw-rw-rw-   0        0        0      493 2024-04-11 13:02:22.000000 socon_embedded-0.1a4/tests/commands/datafixtures/simple_app_with_task.yml
+-rw-rw-rw-   0        0        0      370 2024-04-11 12:36:04.000000 socon_embedded-0.1a4/tests/commands/test_build_command.py
+-rw-rw-rw-   0        0        0      439 2024-04-12 08:53:56.000000 socon_embedded-0.1a4/tests/commands/test_from_file.py
+-rw-rw-rw-   0        0        0      330 2024-04-12 08:52:00.000000 socon_embedded-0.1a4/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.105917 socon_embedded-0.1a4/tests/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:18:37.000000 socon_embedded-0.1a4/tests/executor/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-04-11 12:28:37.000000 socon_embedded-0.1a4/tests/executor/test_task_executor.py
+-rw-rw-rw-   0        0        0      580 2024-04-11 12:23:44.000000 socon_embedded-0.1a4/tests/executor/test_task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.117991 socon_embedded-0.1a4/tests/management/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:58:57.000000 socon_embedded-0.1a4/tests/management/__init__.py
+-rw-rw-rw-   0        0        0       33 2024-04-11 12:59:16.000000 socon_embedded-0.1a4/tests/management/config.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.117991 socon_embedded-0.1a4/tests/projects/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a4/tests/projects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.157568 socon_embedded-0.1a4/tests/projects/test_project/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon_embedded-0.1a4/tests/projects/test_project/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-04-12 08:56:26.000000 socon_embedded-0.1a4/tests/projects/test_project/action.py
+-rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/projects/test_project/builder.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.166789 socon_embedded-0.1a4/tests/projects/test_project/management/
+-rw-rw-rw-   0        0        0       33 2024-04-12 08:51:00.000000 socon_embedded-0.1a4/tests/projects/test_project/management/config.py
+-rw-rw-rw-   0        0        0      171 2024-04-12 08:51:38.000000 socon_embedded-0.1a4/tests/projects/test_project/projects.py
+-rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/pytest.ini
+-rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon_embedded-0.1a4/tests/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.178391 socon_embedded-0.1a4/tests/schema/
+-rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/schema/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.239667 socon_embedded-0.1a4/tests/schema/datafixtures/
+-rw-rw-rw-   0        0        0       80 2024-04-04 13:07:32.000000 socon_embedded-0.1a4/tests/schema/datafixtures/action_extra_args.yml
+-rw-rw-rw-   0        0        0       47 2024-04-02 13:14:24.000000 socon_embedded-0.1a4/tests/schema/datafixtures/bad_action.yml
+-rw-rw-rw-   0        0        0       59 2024-04-02 13:13:17.000000 socon_embedded-0.1a4/tests/schema/datafixtures/copy_schema.yml
+-rw-rw-rw-   0        0        0       91 2024-04-02 15:27:00.000000 socon_embedded-0.1a4/tests/schema/datafixtures/multiple_valid_action.yml
+-rw-rw-rw-   0        0        0       19 2024-04-02 15:22:54.000000 socon_embedded-0.1a4/tests/schema/datafixtures/no_action.yml
+-rw-rw-rw-   0        0        0       77 2024-04-02 13:15:18.000000 socon_embedded-0.1a4/tests/schema/datafixtures/set_action.yml
+-rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon_embedded-0.1a4/tests/schema/test_app_registry.py
+-rw-rw-rw-   0        0        0     2652 2024-04-11 12:14:54.000000 socon_embedded-0.1a4/tests/schema/test_tasks.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:03:21.251022 socon_embedded-0.1a4/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tests/utils/test_splitter.py
+-rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon_embedded-0.1a4/tox.ini
```

### Comparing `socon-embedded-0.1a3/.gitignore` & `socon_embedded-0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/CODE_OF_CONDUCT.md` & `socon_embedded-0.1a4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/LICENSE` & `socon_embedded-0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/PKG-INFO` & `socon_embedded-0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a3
+Version: 0.1a4
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socon-embedded-0.1a3/README.rst` & `socon_embedded-0.1a4/README.rst`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/pyproject.toml` & `socon_embedded-0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/action/__init__.py` & `socon_embedded-0.1a4/socon_embedded/action/__init__.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/action/call.py` & `socon_embedded-0.1a4/socon_embedded/action/call.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/action/copy.py` & `socon_embedded-0.1a4/socon_embedded/action/copy.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/builder/__init__.py` & `socon_embedded-0.1a4/socon_embedded/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/builder/parser.py` & `socon_embedded-0.1a4/socon_embedded/builder/parser.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/builder/result.py` & `socon_embedded-0.1a4/socon_embedded/builder/result.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/exceptions.py` & `socon_embedded-0.1a4/socon_embedded/exceptions.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/executor/app_executor.py` & `socon_embedded-0.1a4/socon_embedded/executor/app_executor.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/executor/task_executor.py` & `socon_embedded-0.1a4/socon_embedded/executor/task_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             self._terminal.line()
 
     def cleanup(self) -> None:
         for executor in self._played_tasks:
             executor.cleanup()
 
     def _task_on_start(self, task: Task):
-        if self._terminal._current_line not in ["", "\n", "\r"]:
+        if self._terminal._current_line != "":
             self._terminal.line()
         self._terminal.line(f"TASK [{task.name}]")
         self._terminal.sep("*")
 
     def _task_on_failed(self, result: TaskResult):
         msg = "failed: => {}".format(self._dump_results(result._result))
         self._terminal.line(msg, fg="red")
```

### Comparing `socon-embedded-0.1a3/socon_embedded/executor/task_result.py` & `socon_embedded-0.1a4/socon_embedded/executor/task_result.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/management/commands/build.py` & `socon_embedded-0.1a4/socon_embedded/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/from_file.py` & `socon_embedded-0.1a4/socon_embedded/management/commands/subcommands/from_file.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/managers.py` & `socon_embedded-0.1a4/socon_embedded/managers.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/schema/apps.py` & `socon_embedded-0.1a4/socon_embedded/schema/apps.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/schema/base.py` & `socon_embedded-0.1a4/socon_embedded/schema/base.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/schema/task.py` & `socon_embedded-0.1a4/socon_embedded/schema/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-from typing import List, Literal, Optional, Type
+from typing import List, Literal, Optional, Type, Any
 
 from socon.core.registry import projects
 
 from socon_embedded.exceptions import ParserError
 from socon_embedded.managers import get_action_manager
 from socon_embedded.schema.base import Base, Nameable, get_field_names
 
 from pydantic import BaseModel, Field, model_validator
 
 
 class Task(Base, Nameable):
     """Call a module (action) with specific arguments and other parameters"""
 
-    action: Type
+    action: Any
     args: dict = {}
 
     retries: Optional[int] = 0
     timeout: Optional[int] = None
 
     @model_validator(mode="before")
     @classmethod
@@ -27,28 +27,33 @@
         args = {}
 
         if "action" in values:
             action = values["action"]
         if "args" in values:
             args = values["args"]
 
+        # If the application registry filters some of the apps,
+        # the validation will need to be retriggered and the action
+        # will already be an instance. To avoid that, we check if we already have an action instance and return it as his.
+        if isinstance(action, object) and action is not None:
+            return values
+
         # filter out task attributes so we're only querying unrecognized keys as actions/modules
         non_task_values = dict(
             (k, v) for k, v in values.items() if (k not in get_field_names(Task))
         )
 
         # walk the filtered input dictionary to see if we recognize a module name
         action_manager = get_action_manager()
         for item, value in non_task_values.items():
             is_action_candidate = False
             if item in action_manager.get_hooks_name():
                 is_action_candidate = True
 
             if is_action_candidate:
-
                 # finding more than one module name is a problem
                 if action is not None:
                     raise ParserError(
                         "conflicting action statements: {}, {}".format(action, item)
                     )
 
                 action = item
@@ -78,15 +83,16 @@
         values["action"] = action
         values["args"] = args
         return values
 
     @model_validator(mode="after")
     def post_process_action(self):
         """Validate the action schema"""
-        self.action = self.action(self)
+        if isinstance(self.action, type):
+            self.action = self.action(self)
         return self
 
 
 class Taskable(BaseModel):
     """
     Make a schema taskable.
     Give the ability to have pre_tasks, post_tasks and tasks
```

### Comparing `socon-embedded-0.1a3/socon_embedded/utils/converter.py` & `socon_embedded-0.1a4/socon_embedded/utils/converter.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/utils/loader.py` & `socon_embedded-0.1a4/socon_embedded/utils/loader.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded/utils/parser.py` & `socon_embedded-0.1a4/socon_embedded/utils/parser.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/socon_embedded.egg-info/PKG-INFO` & `socon_embedded-0.1a4/socon_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a3
+Version: 0.1a4
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socon-embedded-0.1a3/socon_embedded.egg-info/SOURCES.txt` & `socon_embedded-0.1a4/socon_embedded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/action/test_call_command.py` & `socon_embedded-0.1a4/tests/action/test_call_command.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/action/test_copy.py` & `socon_embedded-0.1a4/tests/action/test_copy.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/action/test_discover.py` & `socon_embedded-0.1a4/tests/action/test_discover.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/executor/test_task_result.py` & `socon_embedded-0.1a4/tests/executor/test_task_result.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/schema/test_app_registry.py` & `socon_embedded-0.1a4/tests/schema/test_app_registry.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/schema/test_tasks.py` & `socon_embedded-0.1a4/tests/schema/test_tasks.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tests/utils/test_splitter.py` & `socon_embedded-0.1a4/tests/utils/test_splitter.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a3/tox.ini` & `socon_embedded-0.1a4/tox.ini`

 * *Files identical despite different names*

