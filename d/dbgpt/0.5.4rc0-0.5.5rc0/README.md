# Comparing `tmp/dbgpt-0.5.4rc0.tar.gz` & `tmp/dbgpt-0.5.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.4rc0.tar", last modified: Thu Apr 11 05:05:19 2024, max compression
+gzip compressed data, was "dbgpt-0.5.5rc0.tar", last modified: Thu Apr 18 03:05:22 2024, max compression
```

## Comparing `dbgpt-0.5.4rc0.tar` & `dbgpt-0.5.5rc0.tar`

### file list

```diff
@@ -1,461 +1,462 @@
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.368039 dbgpt-0.5.4rc0/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.4rc0/LICENSE
--rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.4rc0/MANIFEST.in
--rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:19.367289 dbgpt-0.5.4rc0/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/README.md
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.973762 dbgpt-0.5.4rc0/dbgpt/
--rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.981845 dbgpt-0.5.4rc0/dbgpt/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13796 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/_private/config.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1625 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      983 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/_private/pydantic.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.4rc0/dbgpt/_version.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.982750 dbgpt-0.5.4rc0/dbgpt/agent/
--rw-r--r--   0 staneyffer   (501) staff       (20)      944 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.989166 dbgpt-0.5.4rc0/dbgpt/agent/actions/
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5106 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/blank_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/chart_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/code_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/dashboard_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/indicator_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/plugin_action.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.996611 dbgpt-0.5.4rc0/dbgpt/agent/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3463 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    35778 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5616 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_team.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.998902 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3496 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.000032 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/priority.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3632 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/role.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      455 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/user_proxy_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.005797 dbgpt-0.5.4rc0/dbgpt/agent/expand/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-11 02:57:34.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/code_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5410 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/data_scientist_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2710 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/plugin_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22133 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1680 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/summary_assistant_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.008669 dbgpt-0.5.4rc0/dbgpt/agent/memory/
--rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/default_gpts_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/gpts_memory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.012326 dbgpt-0.5.4rc0/dbgpt/agent/plan/
--rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.016378 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10858 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6004 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/team_awel_layout.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/plan_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7577 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/planner_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/team_auto_plan.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.019545 dbgpt-0.5.4rc0/dbgpt/agent/plugin/
--rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.022966 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/
--rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.023575 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/
--rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.026320 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/
--rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22478 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/generator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/plugins_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.030330 dbgpt-0.5.4rc0/dbgpt/agent/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3698 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 01:48:23.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_db_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_knowledge_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_plugin_api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.032017 dbgpt-0.5.4rc0/dbgpt/agent/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 04:29:39.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/cmp.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.033422 dbgpt-0.5.4rc0/dbgpt/cli/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/cli/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.041821 dbgpt-0.5.4rc0/dbgpt/client/
--rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/app.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14121 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3718 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/client/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3562 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/flow.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6906 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9418 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/client/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10595 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/component.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.043705 dbgpt-0.5.4rc0/dbgpt/configs/
--rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/configs/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/configs/model_config.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.044635 dbgpt-0.5.4rc0/dbgpt/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.047812 dbgpt-0.5.4rc0/dbgpt/core/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.048644 dbgpt-0.5.4rc0/dbgpt/core/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)     6044 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.053927 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3515 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.059666 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    33486 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/compat.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    28676 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.064144 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.065894 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.068366 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/
--rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.071359 dbgpt-0.5.4rc0/dbgpt/core/awel/task/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.077642 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/
--rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37793 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.081292 dbgpt-0.5.4rc0/dbgpt/core/awel/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/_typing_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/http_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.093577 dbgpt-0.5.4rc0/dbgpt/core/interface/
--rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3793 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31087 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    42772 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/message.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.101651 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    16374 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    26524 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1725 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15124 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.102606 dbgpt-0.5.4rc0/dbgpt/core/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.105315 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.107003 dbgpt-0.5.4rc0/dbgpt/core/schema/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3868 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.111492 dbgpt-0.5.4rc0/dbgpt/datasource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114151 dbgpt-0.5.4rc0/dbgpt/datasource/manages/
--rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connect_config_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114912 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.116360 dbgpt-0.5.4rc0/dbgpt/datasource/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.126686 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mysql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.127572 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.128426 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.130689 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/redis.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.135298 dbgpt-0.5.4rc0/dbgpt/model/
--rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.150106 dbgpt-0.5.4rc0/dbgpt/model/adapter/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/cli.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.152289 dbgpt-0.5.4rc0/dbgpt/model/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/parameter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.154070 dbgpt-0.5.4rc0/dbgpt/model/proxy/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.165126 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/
--rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/claude.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/moonshot.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.167691 dbgpt-0.5.4rc0/dbgpt/model/utils/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.169670 dbgpt-0.5.4rc0/dbgpt/rag/
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.174299 dbgpt-0.5.4rc0/dbgpt/rag/assembler/
--rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.178536 dbgpt-0.5.4rc0/dbgpt/rag/embedding/
--rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    24178 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.180597 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/
--rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.184058 dbgpt-0.5.4rc0/dbgpt/rag/extractor/
--rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.187268 dbgpt-0.5.4rc0/dbgpt/rag/graph/
--rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/graph/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.203704 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/json.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/markdown.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.217047 dbgpt-0.5.4rc0/dbgpt/rag/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.222651 dbgpt-0.5.4rc0/dbgpt/rag/retriever/
--rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.224784 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.227962 dbgpt-0.5.4rc0/dbgpt/rag/summary/
--rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3964 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.231422 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/
--rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.233812 dbgpt-0.5.4rc0/dbgpt/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.238853 dbgpt-0.5.4rc0/dbgpt/storage/cache/
--rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/embedding_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.240028 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.241804 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.243560 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/
--rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.245833 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/
--rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.250741 dbgpt-0.5.4rc0/dbgpt/storage/metadata/
--rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9255 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/schema.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.257290 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/
--rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7796 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8232 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/chroma_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/filters.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    21307 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3462 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6749 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298070 dbgpt-0.5.4rc0/dbgpt/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/annotations.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/api_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298880 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.300181 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9300 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/chat_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/code_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/command_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/config_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.301400 dbgpt-0.5.4rc0/dbgpt/util/console/
--rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/console.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.4rc0/dbgpt/util/date_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.304988 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9344 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11619 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5905 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/error_types.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1313 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/fastapi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/formatting.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/function_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/global_helper.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/json_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/memory_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/model_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/module_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/net_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.305930 dbgpt-0.5.4rc0/dbgpt/util/network/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9777 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      545 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/path_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8661 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.306804 dbgpt-0.5.4rc0/dbgpt/util/serialization/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/singleton.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.310685 dbgpt-0.5.4rc0/dbgpt/util/speech/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/gtts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/say.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/string_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/system_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.315968 dbgpt-0.5.4rc0/dbgpt/util/tracer/
--rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.317582 dbgpt-0.5.4rc0/dbgpt/vis/
--rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 04:24:29.000000 dbgpt-0.5.4rc0/dbgpt/vis/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.323394 dbgpt-0.5.4rc0/dbgpt/vis/tags/
--rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_message.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_plans.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_chart.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_code.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_dashboard.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_execution.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_result.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_plugin.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.977858 dbgpt-0.5.4rc0/dbgpt.egg-info/
--rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    12638 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/SOURCES.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/dependency_links.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/entry_points.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)     4943 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/top_level.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-11 05:05:19.368143 dbgpt-0.5.4rc0/setup.cfg
--rw-r--r--   0 staneyffer   (501) staff       (20)    23342 2024-04-11 01:47:19.000000 dbgpt-0.5.4rc0/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.085496 dbgpt-0.5.5rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.5rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.5rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:22.084796 dbgpt-0.5.5rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.797715 dbgpt-0.5.5rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801427 dbgpt-0.5.5rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14183 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.5rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801728 dbgpt-0.5.5rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1125 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.806821 dbgpt-0.5.5rc0/dbgpt/agent/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5354 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3746 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4461 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.810930 dbgpt-0.5.5rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5364 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    35815 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5544 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.812142 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.813235 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      466 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.817278 dbgpt-0.5.5rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-16 17:14:04.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2207 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5415 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22055 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1685 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/summary_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.819411 dbgpt-0.5.5rc0/dbgpt/agent/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.821740 dbgpt-0.5.5rc0/dbgpt/agent/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.823998 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10852 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6014 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8258 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7582 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.825803 dbgpt-0.5.5rc0/dbgpt/agent/plugin/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.827682 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.828088 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.830121 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22485 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.832787 dbgpt-0.5.5rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3721 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_plugin_api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.834142 dbgpt-0.5.5rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.835035 dbgpt-0.5.5rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.838920 dbgpt-0.5.5rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.5rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9487 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10759 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.839908 dbgpt-0.5.5rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.840591 dbgpt-0.5.5rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842026 dbgpt-0.5.5rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842690 dbgpt-0.5.5rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6061 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.845836 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.849896 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29039 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.852865 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.854341 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.856561 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.859147 dbgpt-0.5.5rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.863491 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.866415 dbgpt-0.5.5rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.873538 dbgpt-0.5.5rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    42803 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878118 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26575 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878848 dbgpt-0.5.5rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.881201 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.882453 dbgpt-0.5.5rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8246 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.885625 dbgpt-0.5.5rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.887735 dbgpt-0.5.5rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.888451 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.889918 dbgpt-0.5.5rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.897610 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898231 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898831 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.900469 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.903268 dbgpt-0.5.5rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.912503 dbgpt-0.5.5rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.914015 dbgpt-0.5.5rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.915211 dbgpt-0.5.5rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.923920 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.926322 dbgpt-0.5.5rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.927912 dbgpt-0.5.5rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.931570 dbgpt-0.5.5rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.934462 dbgpt-0.5.5rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24261 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.935766 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938265 dbgpt-0.5.5rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938914 dbgpt-0.5.5rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.947645 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.953454 dbgpt-0.5.5rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.957440 dbgpt-0.5.5rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.959293 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.961655 dbgpt-0.5.5rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.964496 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.965560 dbgpt-0.5.5rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973084 dbgpt-0.5.5rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973881 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.975078 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.976473 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.978356 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.982178 dbgpt-0.5.5rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.986115 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7923 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8233 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    21288 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3440 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6727 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.010463 dbgpt-0.5.5rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.011350 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.013055 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.5rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.014455 dbgpt-0.5.5rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.5rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.019006 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11198 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10560 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.020208 dbgpt-0.5.5rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/retry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.021012 dbgpt-0.5.5rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.025755 dbgpt-0.5.5rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/system_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.030555 dbgpt-0.5.5rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.032504 dbgpt-0.5.5rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.038159 dbgpt-0.5.5rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.799891 dbgpt-0.5.5rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12658 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4987 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-18 03:05:22.085629 dbgpt-0.5.5rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24009 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/setup.py
```

### Comparing `dbgpt-0.5.4rc0/LICENSE` & `dbgpt-0.5.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/PKG-INFO` & `dbgpt-0.5.5rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,408 +1,405 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.4rc0
+Version: 0.5.5rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
-Requires-Dist: pydantic<2,>=1
+Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Provides-Extra: core
-Requires-Dist: aiohttp==3.8.4; extra == "core"
 Requires-Dist: chardet==5.1.0; extra == "core"
 Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: python-dotenv==1.0.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
-Requires-Dist: pydantic<2,>=1; extra == "core"
 Requires-Dist: typeguard; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: pydantic>=2.6.0; extra == "core"
 Provides-Extra: client
-Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: httpx; extra == "client"
 Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: cachetools; extra == "client"
-Requires-Dist: pydantic<2,>=1; extra == "client"
 Requires-Dist: typeguard; extra == "client"
-Requires-Dist: httpx; extra == "client"
-Requires-Dist: fastapi==0.98.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: pydantic>=2.6.0; extra == "client"
 Provides-Extra: cli
-Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: click; extra == "cli"
 Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
+Requires-Dist: tomlkit; extra == "cli"
 Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
 Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: pydantic<2,>=1; extra == "cli"
 Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: fastapi==0.98.0; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: click; extra == "cli"
+Requires-Dist: rich; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
+Requires-Dist: aiohttp==3.8.4; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: tomlkit; extra == "cli"
-Requires-Dist: rich; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: click; extra == "agent"
 Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: termcolor; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
 Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: pydantic<2,>=1; extra == "agent"
 Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
-Requires-Dist: fastapi==0.98.0; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: click; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: rich; extra == "agent"
 Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
 Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: tomlkit; extra == "agent"
-Requires-Dist: rich; extra == "agent"
-Requires-Dist: termcolor; extra == "agent"
-Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: pydantic>=2.6.0; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: click; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: pydantic<2,>=1; extra == "simple-framework"
 Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: fastapi==0.98.0; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: psutil==5.9.4; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
 Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Requires-Dist: tomlkit; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
+Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
+Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
-Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: click; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
+Requires-Dist: msgpack; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: pydantic<2,>=1; extra == "framework"
 Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: fastapi==0.98.0; extra == "framework"
-Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: click; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
 Requires-Dist: rich; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
-Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
 Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: jinja2; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: pydantic>=2.6.0; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: prettytable; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
-Requires-Dist: pymilvus; extra == "vstore"
-Requires-Dist: weaviate-client; extra == "vstore"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore"
+Provides-Extra: vstore-weaviate
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
+Requires-Dist: weaviate-client; extra == "vstore-weaviate"
+Provides-Extra: vstore-milvus
+Requires-Dist: pymilvus; extra == "vstore-milvus"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
+Provides-Extra: vstore-all
+Requires-Dist: pymilvus; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
+Requires-Dist: weaviate-client; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
-Requires-Dist: pymysql; extra == "datasource-all"
-Requires-Dist: pyspark; extra == "datasource-all"
 Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
+Requires-Dist: thrift_sasl; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
+Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: thrift_sasl; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: pymilvus; extra == "rag"
-Requires-Dist: weaviate-client; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: spacy==3.5.3; extra == "rag"
-Requires-Dist: chromadb==0.4.10; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: bs4; extra == "rag"
+Requires-Dist: pypdf; extra == "rag"
 Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
-Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Requires-Dist: python-multipart; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
+Requires-Dist: langchain>=0.0.286; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
+Requires-Dist: chromadb>=0.4.22; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: openai; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
 Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: pydantic<2,>=1; extra == "openai"
 Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: fastapi==0.98.0; extra == "openai"
-Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
 Requires-Dist: rich; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
-Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
 Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: markdown; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: aiofiles; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: pymilvus; extra == "openai"
-Requires-Dist: weaviate-client; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: spacy==3.5.3; extra == "openai"
-Requires-Dist: chromadb==0.4.10; extra == "openai"
-Requires-Dist: markdown; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: jinja2; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: python-multipart; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
 Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: openai; extra == "openai"
+Requires-Dist: prettytable; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: graphviz; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: protobuf==3.20.3; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: click; extra == "default"
+Requires-Dist: fschat; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: cachetools; extra == "default"
-Requires-Dist: pydantic<2,>=1; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
 Requires-Dist: typeguard; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: fastapi==0.98.0; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: click; extra == "default"
-Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: rich; extra == "default"
-Requires-Dist: termcolor; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: jinja2; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: pympler; extra == "default"
-Requires-Dist: duckdb; extra == "default"
 Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: fschat; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
 Requires-Dist: pymysql; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: markdown; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: pympler; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: pymilvus; extra == "default"
-Requires-Dist: weaviate-client; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: spacy==3.5.3; extra == "default"
-Requires-Dist: chromadb==0.4.10; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: python-docx; extra == "default"
 Requires-Dist: pypdf; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: jinja2; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
+Requires-Dist: schedule; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: chromadb>=0.4.22; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: psutil==5.9.4; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: prettytable; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: graphviz; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Provides-Extra: all
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: chromadb==0.4.10; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: schedule; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: thrift; extra == "all"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: protobuf==3.20.3; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: chromadb>=0.4.22; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: httpx; extra == "all"
 Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
 Requires-Dist: pympler; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: click; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: fastapi>=0.100.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
 Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: pyspark; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
 Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: spacy==3.5.3; extra == "all"
-Requires-Dist: python-docx; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
 Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: pyhive; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
 Requires-Dist: seaborn; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
 Requires-Dist: vllm; extra == "all"
-Requires-Dist: msgpack; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
```

### Comparing `dbgpt-0.5.4rc0/README.md` & `dbgpt-0.5.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/_private/config.py` & `dbgpt-0.5.5rc0/dbgpt/_private/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """Initialize the Config class"""
 
         self.NEW_SERVER_MODE = False
         self.SERVER_LIGHT_MODE = False
 
         # Gradio language version: en, zh
         self.LANGUAGE = os.getenv("LANGUAGE", "en")
-        self.WEB_SERVER_PORT = int(os.getenv("WEB_SERVER_PORT", 5000))
+        self.DBGPT_WEBSERVER_PORT = int(os.getenv("DBGPT_WEBSERVER_PORT", 5670))
 
         self.debug_mode = False
         self.skip_reprompt = False
         self.temperature = float(os.getenv("TEMPERATURE", 0.7))
 
         # self.NUM_GPUS = int(os.getenv("NUM_GPUS", 1))
 
@@ -296,14 +296,23 @@
         )
         self.MODEL_CACHE_STORAGE_DISK_DIR: Optional[str] = os.getenv(
             "MODEL_CACHE_STORAGE_DISK_DIR"
         )
         # global dbgpt api key
         self.API_KEYS = os.getenv("API_KEYS", None)
 
+        # Non-streaming scene retries
+        self.DBGPT_APP_SCENE_NON_STREAMING_RETRIES_BASE = int(
+            os.getenv("DBGPT_APP_SCENE_NON_STREAMING_RETRIES_BASE", 1)
+        )
+        # Non-streaming scene parallelism
+        self.DBGPT_APP_SCENE_NON_STREAMING_PARALLELISM_BASE = int(
+            os.getenv("DBGPT_APP_SCENE_NON_STREAMING_PARALLELISM_BASE", 1)
+        )
+
     @property
     def local_db_manager(self) -> "ConnectorManager":
         from dbgpt.datasource.manages import ConnectorManager
 
         if not self.SYSTEM_APP:
             raise ValueError("SYSTEM_APP is not set")
         return ConnectorManager.get_instance(self.SYSTEM_APP)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 
 DEFAULT_CONTEXT_WINDOW = 3900
 DEFAULT_NUM_OUTPUTS = 256
 
 
 class LLMMetadata(BaseModel):
+    model_config = ConfigDict(protected_namespaces=())
+
     context_window: int = Field(
         default=DEFAULT_CONTEXT_WINDOW,
         description=(
             "Total number of tokens the model can be input and output for one response."
         ),
     )
     num_output: int = Field(
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,27 +3,35 @@
 from .actions.action import Action, ActionOutput  # noqa: F401
 from .core.agent import (  # noqa: F401
     Agent,
     AgentContext,
     AgentGenerateContext,
     AgentMessage,
 )
+from .core.agent_manage import (  # noqa: F401
+    AgentManager,
+    get_agent_manager,
+    initialize_agent,
+)
 from .core.base_agent import ConversableAgent  # noqa: F401
 from .core.llm.llm import LLMConfig  # noqa: F401
 from .core.schema import PluginStorageType  # noqa: F401
 from .core.user_proxy_agent import UserProxyAgent  # noqa: F401
 from .memory.gpts_memory import GptsMemory  # noqa: F401
 from .resource.resource_api import AgentResource, ResourceType  # noqa: F401
 from .resource.resource_loader import ResourceLoader  # noqa: F401
 
 __ALL__ = [
     "Agent",
     "AgentContext",
     "AgentGenerateContext",
     "AgentMessage",
+    "AgentManager",
+    "initialize_agent",
+    "get_agent_manager",
     "ConversableAgent",
     "Action",
     "ActionOutput",
     "LLMConfig",
     "GptsMemory",
     "AgentResource",
     "ResourceType",
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,21 @@
     TypeVar,
     Union,
     cast,
     get_args,
     get_origin,
 )
 
-from dbgpt._private.pydantic import BaseModel
+from dbgpt._private.pydantic import (
+    BaseModel,
+    field_default,
+    field_description,
+    model_fields,
+    model_to_dict,
+)
 from dbgpt.util.json_utils import find_json_objects
 
 from ...vis.base import Vis
 from ..resource.resource_api import AgentResource, ResourceType
 from ..resource.resource_loader import ResourceLoader
 
 T = TypeVar("T", bound=Union[BaseModel, List[BaseModel], None])
@@ -41,14 +47,18 @@
         cls: Type["ActionOutput"], param: Optional[Dict]
     ) -> Optional["ActionOutput"]:
         """Convert dict to ActionOutput object."""
         if not param:
             return None
         return cls.parse_obj(param)
 
+    def to_dict(self) -> Dict[str, Any]:
+        """Convert the object to a dictionary."""
+        return model_to_dict(self)
+
 
 class Action(ABC, Generic[T]):
     """Base Action class for defining agent actions."""
 
     def __init__(self):
         """Create an action."""
         self.resource_loader: Optional[ResourceLoader] = None
@@ -81,20 +91,21 @@
         if model_type is None:
             return None
         origin = get_origin(model_type)
         args = get_args(model_type)
         if origin is None:
             example = {}
             single_model_type = cast(Type[BaseModel], model_type)
-            for field_name, field in single_model_type.__fields__.items():
-                field_info = field.field_info
-                if field_info.description:
-                    example[field_name] = field_info.description
-                elif field_info.default:
-                    example[field_name] = field_info.default
+            for field_name, field in model_fields(single_model_type).items():
+                description = field_description(field)
+                default_value = field_default(field)
+                if description:
+                    example[field_name] = description
+                elif default_value:
+                    example[field_name] = default_value
                 else:
                     example[field_name] = ""
             return example
         elif origin is list or origin is List:
             element_type = cast(Type[BaseModel], args[0])
             if issubclass(element_type, BaseModel):
                 list_example = self._create_example(element_type)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/blank_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/chart_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Chart Action for SQL execution and rendering."""
 import json
 import logging
 from typing import Optional
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, Field, model_to_json
 from dbgpt.vis.tags.vis_chart import Vis, VisChart
 
 from ..resource.resource_api import AgentResource, ResourceType
 from ..resource.resource_db_api import ResourceDbClient
 from .action import Action, ActionOutput
 
 logger = logging.getLogger(__name__)
@@ -82,21 +82,21 @@
                 )
             if not resource:
                 raise ValueError("The data resource is not found！")
             data_df = await resource_db_client.query_to_df(resource.value, param.sql)
             if not self.render_protocol:
                 raise ValueError("The rendering protocol is not initialized！")
             view = await self.render_protocol.display(
-                chart=json.loads(param.json()), data_df=data_df
+                chart=json.loads(model_to_json(param)), data_df=data_df
             )
             if not self.resource_need:
                 raise ValueError("The resource type is not found！")
             return ActionOutput(
                 is_exe_success=True,
-                content=param.json(),
+                content=model_to_json(param),
                 view=view,
                 resource_type=self.resource_need.value,
                 resource_value=resource.value,
             )
         except Exception as e:
             logger.exception("Check your answers, the sql run failed！")
             return ActionOutput(
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/code_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/dashboard_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Dashboard Action Module."""
 import json
 import logging
 from typing import List, Optional
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, Field, model_to_dict
 from dbgpt.vis.tags.vis_dashboard import Vis, VisDashboard
 
 from ..resource.resource_api import AgentResource, ResourceType
 from ..resource.resource_db_api import ResourceDbClient
 from .action import Action, ActionOutput
 
 logger = logging.getLogger(__name__)
@@ -26,14 +26,18 @@
         "what to output, just output 'response_table' uniformly.",
     )
     sql: str = Field(
         ..., description="Executable sql generated for the current target/problem"
     )
     thought: str = Field(..., description="Summary of thoughts to the user")
 
+    def to_dict(self):
+        """Convert to dict."""
+        return model_to_dict(self)
+
 
 class DashboardAction(Action[List[ChartItem]]):
     """Dashboard action class."""
 
     def __init__(self):
         """Create a dashboard action."""
         super().__init__()
@@ -97,27 +101,29 @@
             chart_params = []
             for chart_item in chart_items:
                 chart_dict = {}
                 try:
                     sql_df = await resource_db_client.query_to_df(
                         resource.value, chart_item.sql
                     )
-                    chart_dict = chart_item.dict()
+                    chart_dict = chart_item.to_dict()
 
                     chart_dict["data"] = sql_df
                 except Exception as e:
                     logger.warning(f"Sql execute failed！{str(e)}")
                     chart_dict["err_msg"] = str(e)
                 chart_params.append(chart_dict)
             if not self.render_protocol:
                 raise ValueError("The render protocol is not initialized!")
             view = await self.render_protocol.display(charts=chart_params)
             return ActionOutput(
                 is_exe_success=True,
-                content=json.dumps([chart_item.dict() for chart_item in chart_items]),
+                content=json.dumps(
+                    [chart_item.to_dict() for chart_item in chart_items]
+                ),
                 view=view,
             )
         except Exception as e:
             logger.exception("Dashboard generate Failed！")
             return ActionOutput(
                 is_exe_success=False, content=f"Dashboard action run failed!{str(e)}"
             )
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/indicator_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/actions/plugin_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/agent_manage.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,81 @@
-"""Manages the registration and retrieval of agents."""
+"""DuckDB connector."""
+from typing import Any, Iterable, Optional
 
-import logging
-import re
-from collections import defaultdict
-from typing import Dict, List, Type
-
-from ..expand.code_assistant_agent import CodeAssistantAgent
-from ..expand.dashboard_assistant_agent import DashboardAssistantAgent
-from ..expand.data_scientist_agent import DataScientistAgent
-from ..expand.plugin_assistant_agent import PluginAssistantAgent
-from ..expand.summary_assistant_agent import SummaryAssistantAgent
-from .agent import Agent
-
-logger = logging.getLogger(__name__)
-
-
-def participant_roles(agents: List[Agent]) -> str:
-    """Return a string listing the roles of the agents."""
-    # Default to all agents registered
-    roles = []
-    for agent in agents:
-        roles.append(f"{agent.get_name()}: {agent.get_describe()}")
-    return "\n".join(roles)
-
-
-def mentioned_agents(message_content: str, agents: List[Agent]) -> Dict:
-    """Return a dictionary mapping agent names to mention counts.
-
-    Finds and counts agent mentions in the string message_content, taking word
-    boundaries into account.
-
-    Returns: A dictionary mapping agent names to mention counts (to be included,
-    at least one mention must occur)
-    """
-    mentions = dict()
-    for agent in agents:
-        regex = (
-            r"(?<=\W)" + re.escape(agent.get_name()) + r"(?=\W)"
-        )  # Finds agent mentions, taking word boundaries into account
-        count = len(
-            re.findall(regex, " " + message_content + " ")
-        )  # Pad the message to help with matching
-        if count > 0:
-            mentions[agent.get_name()] = count
-    return mentions
-
-
-class AgentManager:
-    """Manages the registration and retrieval of agents."""
-
-    def __init__(self):
-        """Create a new AgentManager."""
-        self._agents = defaultdict()
-
-    def register_agent(self, cls):
-        """Register an agent."""
-        self._agents[cls().profile] = cls
-
-    def get_by_name(self, name: str) -> Type[Agent]:
-        """Return an agent by name.
-
-        Args:
-            name (str): The name of the agent to retrieve.
-
-        Returns:
-            Type[Agent]: The agent with the given name.
-
-        Raises:
-            ValueError: If the agent with the given name is not registered.
-        """
-        if name not in self._agents:
-            raise ValueError(f"Agent:{name} not register!")
-        return self._agents[name]
-
-    def get_describe_by_name(self, name: str) -> str:
-        """Return the description of an agent by name."""
-        return self._agents[name].desc
-
-    def all_agents(self):
-        """Return a dictionary of all registered agents and their descriptions."""
-        result = {}
-        for name, cls in self._agents.items():
-            result[name] = cls.desc
-        return result
-
-    def list_agents(self):
-        """Return a list of all registered agents and their descriptions."""
-        result = []
-        for name, cls in self._agents.items():
-            instance = cls()
-            result.append(
-                {
-                    "name": instance.profile,
-                    "desc": instance.goal,
-                }
-            )
-        return result
+from sqlalchemy import create_engine, text
+
+from .base import RDBMSConnector
 
 
-agent_manager = AgentManager()
+class DuckDbConnector(RDBMSConnector):
+    """DuckDB connector."""
+
+    db_type: str = "duckdb"
+    db_dialect: str = "duckdb"
+
+    @classmethod
+    def from_file_path(
+        cls, file_path: str, engine_args: Optional[dict] = None, **kwargs: Any
+    ) -> RDBMSConnector:
+        """Construct a SQLAlchemy engine from URI."""
+        _engine_args = engine_args or {}
+        return cls(create_engine("duckdb:///" + file_path, **_engine_args), **kwargs)
+
+    def get_users(self):
+        """Get users."""
+        cursor = self.session.execute(
+            text(
+                "SELECT * FROM sqlite_master WHERE type = 'table' AND "
+                "name = 'duckdb_sys_users';"
+            )
+        )
+        users = cursor.fetchall()
+        return [(user[0], user[1]) for user in users]
+
+    def get_grants(self):
+        """Get grants."""
+        return []
+
+    def get_collation(self):
+        """Get collation."""
+        return "UTF-8"
+
+    def get_charset(self):
+        """Get character_set of current database."""
+        return "UTF-8"
+
+    def get_table_comments(self, db_name: str):
+        """Get table comments."""
+        cursor = self.session.execute(
+            text(
+                """
+                SELECT name, sql FROM sqlite_master WHERE type='table'
+                """
+            )
+        )
+        table_comments = cursor.fetchall()
+        return [
+            (table_comment[0], table_comment[1]) for table_comment in table_comments
+        ]
+
+    def table_simple_info(self) -> Iterable[str]:
+        """Get table simple info."""
+        _tables_sql = """
+                SELECT name FROM sqlite_master WHERE type='table'
+            """
+        cursor = self.session.execute(text(_tables_sql))
+        tables_results = cursor.fetchall()
+        results = []
+        for row in tables_results:
+            table_name = row[0]
+            _sql = f"""
+                PRAGMA  table_info({table_name})
+            """
+            cursor_colums = self.session.execute(text(_sql))
+            colum_results = cursor_colums.fetchall()
+            table_colums = []
+            for row_col in colum_results:
+                field_info = list(row_col)
+                table_colums.append(field_info[1])
 
-agent_manager.register_agent(CodeAssistantAgent)
-agent_manager.register_agent(DashboardAssistantAgent)
-agent_manager.register_agent(DataScientistAgent)
-agent_manager.register_agent(SummaryAssistantAgent)
-agent_manager.register_agent(PluginAssistantAgent)
+            results.append(f"{table_name}({','.join(table_colums)});")
+        return results
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/base_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base agent class for conversable agents."""
 
 import asyncio
 import json
 import logging
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
-from dbgpt._private.pydantic import Field
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import LLMClient, ModelMessageRoleType
 from dbgpt.util.error_types import LLMChatError
 from dbgpt.util.tracer import SpanType, root_tracer
 from dbgpt.util.utils import colored
 
 from ..actions.action import Action, ActionOutput
 from ..memory.base import GptsMessage
@@ -21,32 +21,29 @@
 from .llm.llm_client import AIWrapper
 from .role import Role
 
 logger = logging.getLogger(__name__)
 
 
 class ConversableAgent(Role, Agent):
-    """ConversableAgent is a agent that can communicate with other agents."""
+    """ConversableAgent is an agent that can communicate with other agents."""
+
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     agent_context: Optional[AgentContext] = Field(None, description="Agent context")
     actions: List[Action] = Field(default_factory=list)
     resources: List[AgentResource] = Field(default_factory=list)
     llm_config: Optional[LLMConfig] = None
     memory: GptsMemory = Field(default_factory=GptsMemory)
     resource_loader: Optional[ResourceLoader] = None
     max_retry_count: int = 3
     consecutive_auto_reply_counter: int = 0
     llm_client: Optional[AIWrapper] = None
     oai_system_message: List[Dict] = Field(default_factory=list)
 
-    class Config:
-        """Pydantic configuration."""
-
-        arbitrary_types_allowed = True
-
     def __init__(self, **kwargs):
         """Create a new agent."""
         Role.__init__(self, **kwargs)
         Agent.__init__(self)
 
     def init_system_message(self) -> None:
         """Initialize the system message."""
@@ -373,16 +370,18 @@
                     act_out: Optional[ActionOutput] = await self.act(
                         message=llm_reply,
                         sender=sender,
                         reviewer=reviewer,
                         **act_extent_param,
                     )
                     if act_out:
-                        reply_message.action_report = act_out.dict()
-                    span.metadata["action_report"] = act_out.dict() if act_out else None
+                        reply_message.action_report = act_out.to_dict()
+                    span.metadata["action_report"] = (
+                        act_out.to_dict() if act_out else None
+                    )
 
                 with root_tracer.start_span(
                     "agent.generate_reply.verify",
                     metadata={
                         "llm_reply": llm_reply,
                         "sender": sender.get_name(),
                         "reviewer": reviewer.get_name() if reviewer else None,
@@ -492,27 +491,27 @@
                 "agent.act.run",
                 metadata={
                     "message": message,
                     "sender": sender.get_name() if sender else None,
                     "recipient": self.get_name(),
                     "reviewer": reviewer.get_name() if reviewer else None,
                     "need_resource": need_resource.to_dict() if need_resource else None,
-                    "rely_action_out": last_out.dict() if last_out else None,
+                    "rely_action_out": last_out.to_dict() if last_out else None,
                     "conv_uid": self.not_null_agent_context.conv_id,
                     "action_index": i,
                     "total_action": len(self.actions),
                 },
             ) as span:
                 last_out = await action.run(
                     ai_message=message,
                     resource=need_resource,
                     rely_action_out=last_out,
                     **kwargs,
                 )
-                span.metadata["action_out"] = last_out.dict() if last_out else None
+                span.metadata["action_out"] = last_out.to_dict() if last_out else None
         return last_out
 
     async def correctness_check(
         self, message: AgentMessage
     ) -> Tuple[bool, Optional[str]]:
         """Verify the correctness of the results."""
         return True, None
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/base_team.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base classes for managing a group of agents in a team chat."""
 
 import logging
 from typing import Dict, List, Optional, Tuple, Union
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 
 from ..actions.action import ActionOutput
 from .agent import Agent, AgentMessage
 from .base_agent import ConversableAgent
 
 logger = logging.getLogger(__name__)
 
@@ -64,24 +64,21 @@
             )
     return rst
 
 
 class Team(BaseModel):
     """Team class for managing a group of agents in a team chat."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     agents: List[Agent] = Field(default_factory=list)
     messages: List[Dict] = Field(default_factory=list)
     max_round: int = 100
     is_team: bool = True
 
-    class Config:
-        """Pydantic model configuration."""
-
-        arbitrary_types_allowed = True
-
     def __init__(self, **kwargs):
         """Create a new Team instance."""
         super().__init__(**kwargs)
 
     def hire(self, agents: List[Agent]):
         """Hire roles to cooperate."""
         self.agents.extend(agents)
@@ -118,29 +115,26 @@
         message["content"] = _content_str(message["content"])
         self.messages.append(message)
 
 
 class ManagerAgent(ConversableAgent, Team):
     """Manager Agent class."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     profile: str = "TeamManager"
     goal: str = "manage all hired intelligent agents to complete mission objectives"
     constraints: List[str] = []
     desc: str = goal
     is_team: bool = True
 
     # The management agent does not need to retry the exception. The actual execution
     # of the agent has already been retried.
     max_retry_count: int = 1
 
-    class Config:
-        """Pydantic model configuration."""
-
-        arbitrary_types_allowed = True
-
     def __init__(self, **kwargs):
         """Create a new ManagerAgent instance."""
         ConversableAgent.__init__(self, **kwargs)
         Team.__init__(self, **kwargs)
 
     async def thinking(
         self, messages: List[AgentMessage], prompt: Optional[str] = None
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """LLM module."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional, Type
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 from dbgpt.core import LLMClient, ModelMetadata, ModelRequest
 
 logger = logging.getLogger(__name__)
 
 
 def _build_model_request(input_value: Dict) -> ModelRequest:
     """Build model request from input value.
@@ -102,15 +102,12 @@
     """Register llm strategy."""
     llm_strategies[llm_strategy_type].append(strategy)
 
 
 class LLMConfig(BaseModel):
     """LLM configuration."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     llm_client: Optional[LLMClient] = Field(default_factory=LLMClient)
     llm_strategy: LLMStrategyType = Field(default=LLMStrategyType.Default)
     strategy_context: Optional[Any] = None
-
-    class Config:
-        """Pydantic model config."""
-
-        arbitrary_types_allowed = True
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/priority.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/core/role.py` & `dbgpt-0.5.5rc0/dbgpt/agent/core/role.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """Role class for role-based conversation."""
 from abc import ABC
 from typing import List, Optional
 
-from dbgpt._private.pydantic import BaseModel
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 
 
 class Role(ABC, BaseModel):
     """Role class for role-based conversation."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     profile: str = ""
     name: str = ""
-    resource_introduction = ""
+    resource_introduction: str = ""
     goal: str = ""
 
     expand_prompt: str = ""
 
-    fixed_subgoal: Optional[str] = None
+    fixed_subgoal: Optional[str] = Field(None, description="Fixed subgoal")
 
-    constraints: List[str] = []
+    constraints: List[str] = Field(default_factory=list, description="Constraints")
     examples: str = ""
     desc: str = ""
     language: str = "en"
     is_human: bool = False
     is_team: bool = False
 
-    class Config:
-        """Pydantic config."""
-
-        arbitrary_types_allowed = True
-
     def prompt_template(
         self,
         specified_prompt: Optional[str] = None,
     ) -> str:
         """Return the prompt template for the role.
 
         Args:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/Indicator_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/Indicator_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/code_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/dashboard_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/dashboard_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
         "conversation, and do not omit or modify the content of the analysis sql.",
     ]
     desc: str = (
         "Observe and organize various analysis results and construct "
         "professional reports"
     )
 
-    max_retry_count: int = 3
-
     def __init__(self, **kwargs):
         """Create a new instance of DashboardAssistantAgent."""
         super().__init__(**kwargs)
         self._init_actions([DashboardAction])
 
     def _init_reply_message(self, received_message: AgentMessage) -> AgentMessage:
         reply_message = super()._init_reply_message(received_message)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/data_scientist_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class DataScientistAgent(ConversableAgent):
     """Data Scientist Agent."""
 
-    name = "Edgar"
+    name: str = "Edgar"
     profile: str = "DataScientist"
     goal: str = (
         "Use correct {dialect} SQL to analyze and solve tasks based on the data"
         " structure information of the database given in the resource."
     )
     constraints: List[str] = [
         "Please check the generated SQL carefully. Please strictly abide by the data "
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/plugin_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class PluginAssistantAgent(ConversableAgent):
     """Plugin Assistant Agent."""
 
     plugin_generator: Optional[PluginPromptGenerator] = None
 
-    name = "LuBan"
+    name: str = "LuBan"
     profile: str = "ToolExpert"
     goal: str = (
         "Read and understand the tool information given in the resources below to "
         "understand their capabilities and how to use them,and choosing the right tools"
         " to achieve the user's goals."
     )
     constraints: List[str] = [
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,32 +240,28 @@
             act_out: Optional[ActionOutput] = await self.act(
                 message=final_summary_ai_reply,
                 sender=sender,
                 reviewer=reviewer,
                 **act_extent_param,
             )
             if act_out:
-                reply_message.action_report = act_out.dict()
+                reply_message.action_report = act_out.to_dict()
             # 4.Reply information verification
             check_pass, reason = await self.verify(reply_message, sender, reviewer)
             is_success = check_pass
             # 5.Optimize wrong answers myself
             if not check_pass:
                 reply_message.content = reason
             reply_message.success = is_success
         return reply_message
 
-    async def verify(
-        self,
-        message: AgentMessage,
-        sender: Agent,
-        reviewer: Optional[Agent] = None,
-        **kwargs,
+    async def correctness_check(
+        self, message: AgentMessage
     ) -> Tuple[bool, Optional[str]]:
-        """Verify the correctness of the message."""
+        """Verify the correctness of the results."""
         action_report = message.action_report
         task_result = ""
         if action_report:
             task_result = action_report.get("content", "")
 
         check_result, model = await self.thinking(
             messages=[
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/expand/summary_assistant_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/expand/summary_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SummaryAssistantAgent(ConversableAgent):
     """Summary Assistant Agent."""
 
-    name = "Aristotle"
+    name: str = "Aristotle"
     profile: str = "Summarizer"
     goal: str = (
         "Summarize answer summaries based on user questions from provided "
         "resource information or from historical conversation memories."
     )
 
     constraints: List[str] = [
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/memory/base.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/memory/default_gpts_memory.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/memory/gpts_memory.py` & `dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dbgpt.core.awel.trigger.base import Trigger
 from dbgpt.core.interface.message import ModelMessageRoleType
 
 # TODO: Don't dependent on MixinLLMOperator
 from dbgpt.model.operators.llm_operator import MixinLLMOperator
 
 from ...core.agent import Agent, AgentGenerateContext, AgentMessage
-from ...core.agent_manage import agent_manager
+from ...core.agent_manage import get_agent_manager
 from ...core.base_agent import ConversableAgent
 from ...core.llm.llm import LLMConfig
 from .agent_operator_resource import AWELAgent
 
 
 class BaseAgentOperator:
     """The abstract operator for an Agent."""
@@ -240,15 +240,15 @@
 
     async def get_agent(
         self,
         input_value: AgentGenerateContext,
     ) -> ConversableAgent:
         """Build the agent."""
         # agent build
-        agent_cls: Type[ConversableAgent] = agent_manager.get_by_name(  # type: ignore
+        agent_cls: Type[ConversableAgent] = get_agent_manager().get_by_name(
             self.awel_agent.agent_profile
         )
         llm_config = self.awel_agent.llm_config
 
         if not llm_config:
             if input_value.llm_client:
                 llm_config = LLMConfig(llm_client=input_value.llm_client)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator_resource.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """The AWEL Agent Operator Resource."""
 from typing import Any, Dict, List, Optional
 
-from dbgpt._private.pydantic import BaseModel, Field, root_validator
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_validator
 from dbgpt.core import LLMClient
 from dbgpt.core.awel.flow import (
     FunctionDynamicOptions,
     OptionValue,
     Parameter,
     ResourceCategory,
     register_resource,
 )
 
-from ...core.agent_manage import agent_manager
+from ...core.agent_manage import get_agent_manager
 from ...core.llm.llm import LLMConfig, LLMStrategyType
 from ...resource.resource_api import AgentResource, ResourceType
 
 
 @register_resource(
     label="AWEL Agent Resource",
     name="agent_operator_resource",
@@ -51,17 +51,20 @@
         ),
     ],
     alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentResource"],
 )
 class AWELAgentResource(AgentResource):
     """AWEL Agent Resource."""
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the agent ResourceType."""
+        if not isinstance(values, dict):
+            return values
         name = values.pop("agent_resource_name")
         type = values.pop("agent_resource_type")
         value = values.pop("agent_resource_value")
 
         values["name"] = name
         values["type"] = ResourceType(type)
         values["value"] = value
@@ -105,24 +108,21 @@
         ),
     ],
     alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentConfig"],
 )
 class AWELAgentConfig(LLMConfig):
     """AWEL Agent Config."""
 
-    @root_validator(pre=True)
-    def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """Pre fill the agent ResourceType."""
-        return values
+    pass
 
 
 def _agent_resource_option_values() -> List[OptionValue]:
     return [
         OptionValue(label=item["name"], name=item["name"], value=item["name"])
-        for item in agent_manager.list_agents()
+        for item in get_agent_manager().list_agents()
     ]
 
 
 @register_resource(
     label="AWEL Layout Agent",
     name="agent_operator_agent",
     description="The Agent to build the Agent Operator.",
@@ -169,28 +169,28 @@
         ),
     ],
     alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgent"],
 )
 class AWELAgent(BaseModel):
     """AWEL Agent."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     agent_profile: str
     role_name: Optional[str] = None
     llm_config: Optional[LLMConfig] = None
     resources: List[AgentResource] = Field(default_factory=list)
     fixed_subgoal: Optional[str] = None
 
-    class Config:
-        """Config for the BaseModel."""
-
-        arbitrary_types_allowed = True
-
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the agent ResourceType."""
+        if not isinstance(values, dict):
+            return values
         resource = values.pop("agent_resource")
         llm_config = values.pop("agent_llm_Config")
 
         if resource is not None:
             values["resources"] = [resource]
 
         if llm_config is not None:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/team_awel_layout.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """The manager of the team for the AWEL layout."""
 
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional, cast
 
 from dbgpt._private.config import Config
-from dbgpt._private.pydantic import BaseModel, Field, validator
+from dbgpt._private.pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    model_to_dict,
+    validator,
+)
 from dbgpt.core.awel import DAG
 from dbgpt.core.awel.dag.dag_manager import DAGManager
 
 from ...actions.action import ActionOutput
 from ...core.agent import Agent, AgentGenerateContext, AgentMessage
 from ...core.base_team import ManagerAgent
 from .agent_operator import AWELAgentOperator, WrappedAgentOperator
@@ -66,31 +72,28 @@
     flow_category: Optional[str] = Field(
         default="common",
         description="The flow category of current dag",
     )
 
     def to_dict(self):
         """Convert the object to a dictionary."""
-        return self.dict()
+        return model_to_dict(self)
 
 
 class AWELBaseManager(ManagerAgent, ABC):
     """AWEL base manager."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     goal: str = (
         "Promote and solve user problems according to the process arranged by AWEL."
     )
     constraints: List[str] = []
     desc: str = goal
 
-    class Config:
-        """Config for the BaseModel."""
-
-        arbitrary_types_allowed = True
-
     async def _a_process_received_message(self, message: AgentMessage, sender: Agent):
         """Process the received message."""
         pass
 
     @abstractmethod
     def get_dag(self) -> DAG:
         """Get the DAG of the manager."""
@@ -153,23 +156,20 @@
 
 class WrappedAWELLayoutManager(AWELBaseManager):
     """The manager of the team for the AWEL layout.
 
     Receives a DAG or builds a DAG from the agents.
     """
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     profile: str = "WrappedAWELLayoutManager"
 
     dag: Optional[DAG] = Field(None, description="The DAG of the manager")
 
-    class Config:
-        """Config for the BaseModel."""
-
-        arbitrary_types_allowed = True
-
     def get_dag(self) -> DAG:
         """Get the DAG of the manager."""
         if self.dag:
             return self.dag
         conv_id = self.not_null_agent_context.conv_id
         last_node: Optional[WrappedAgentOperator] = None
         with DAG(
@@ -232,23 +232,20 @@
                 content=f"Failed to complete goal! {str(e)}",
             )
 
 
 class DefaultAWELLayoutManager(AWELBaseManager):
     """The manager of the team for the AWEL layout."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     profile: str = "DefaultAWELLayoutManager"
 
     dag: AWELTeamContext = Field(...)
 
-    class Config:
-        """Config for the BaseModel."""
-
-        arbitrary_types_allowed = True
-
     @validator("dag")
     def check_dag(cls, value):
         """Check the DAG of the manager."""
         assert value is not None and value != "", "dag must not be empty"
         return value
 
     def get_dag(self) -> DAG:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/plan_action.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/planner_agent.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     ]
     desc_zh: str = "你是一个任务规划专家！可以协调智能体，分配资源完成复杂的任务目标。"
     desc: str = (
         "You are a task planning expert! You can coordinate intelligent agents"
         " and allocate resources to achieve complex task goals."
     )
 
-    examples = """
+    examples: str = """
     user:help me build a sales report summarizing our key metrics and trends
     assistants:[
         {{
             "serial_number": "1",
             "agent": "DataScientist",
             "content": "Retrieve total sales, average sales, and number of transactions grouped by "product_category"'.",
             "rely": ""
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plan/team_auto_plan.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command_manage.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     name: str
     location: List[int]
     args: dict
     status: Union[Status, str] = Status.TODO.value
     logo_url: Optional[str] = None
     api_result: Optional[str] = None
     err_msg: Optional[str] = None
-    start_time = datetime.now().timestamp() * 1000
+    start_time: float = datetime.now().timestamp() * 1000
     end_time: Optional[str] = None
 
     df: Any = None
 
 
 class ApiCall:
     """A class representing an API call."""
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/exceptions.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/generator.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/loader.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/plugin/plugins_util.py` & `dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Resource API for the agent."""
 import json
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from dbgpt._private.pydantic import BaseModel
+from dbgpt._private.pydantic import BaseModel, model_to_dict
 
 
 class ResourceType(Enum):
     """Resource type enumeration."""
 
     DB = "database"
     Knowledge = "knowledge"
@@ -63,15 +63,15 @@
             r = AgentResource.from_dict(item)
             if r:
                 json_list.append(r)
         return json_list
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert the AgentResource object to a dictionary."""
-        temp = self.dict()
+        temp = model_to_dict(self)
         for field, value in temp.items():
             if isinstance(value, Enum):
                 temp[field] = value.value
         return temp
 
 
 class ResourceClient(ABC):
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_db_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Database resource client API."""
 import logging
 from contextlib import contextmanager
-from typing import Iterator, List, Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterator, List, Optional, Union
 
 from .resource_api import AgentResource, ResourceClient, ResourceType
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceDbClient(ResourceClient):
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_knowledge_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_loader.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_plugin_api.py` & `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_plugin_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/agent/util/cmp.py` & `dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/_cli.py` & `dbgpt-0.5.5rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/app.py` & `dbgpt-0.5.5rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/client.py` & `dbgpt-0.5.5rc0/dbgpt/client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 from typing import Any, AsyncGenerator, Dict, List, Optional, Union
 from urllib.parse import urlparse
 
 import httpx
 
+from dbgpt._private.pydantic import model_to_dict
 from dbgpt.core.schema.api import ChatCompletionResponse, ChatCompletionStreamResponse
 
 from .schema import ChatCompletionRequestBody
 
 CLIENT_API_PATH = "api"
 CLIENT_SERVE_PATH = "serve"
 
@@ -57,15 +58,15 @@
         version: str = "v2",
         timeout: Optional[httpx._types.TimeoutTypes] = 120,
     ):
         """Create the client.
 
         Args:
             api_base: Optional[str], a full URL for the DB-GPT API.
-                Defaults to the `http://localhost:5000/api/v2`.
+                Defaults to the `http://localhost:5670/api/v2`.
             api_key: Optional[str], The dbgpt api key to use for authentication.
                 Defaults to None.
             timeout: Optional[httpx._types.TimeoutTypes]: The timeout to use.
                 Defaults to None.
             In most cases, pass in a float number to specify the timeout in seconds.
         Returns:
             None
@@ -73,22 +74,22 @@
 
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5000/api/v2"
+            DBGPT_API_BASE = "http://localhost:5670/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             client.chat(model="chatgpt_proxyllm", messages="Hello?")
         """
         if not api_base:
             api_base = os.getenv(
-                "DBGPT_API_BASE", f"http://localhost:5000/{CLIENT_API_PATH}/{version}"
+                "DBGPT_API_BASE", f"http://localhost:5670/{CLIENT_API_PATH}/{version}"
             )
         if not api_key:
             api_key = os.getenv("DBGPT_API_KEY")
         if api_base and is_valid_url(api_base):
             self._api_url = api_base
         else:
             raise ValueError(f"api url {api_base} does not exist or is not accessible.")
@@ -142,15 +143,15 @@
             ChatCompletionResponse: The chat completion response.
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5000/api/v2"
+            DBGPT_API_BASE = "http://localhost:5670/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             res = await client.chat(model="chatgpt_proxyllm", messages="Hello?")
         """
         request = ChatCompletionRequestBody(
             model=model,
             messages=messages,
@@ -163,15 +164,15 @@
             user_name=user_name,
             sys_code=sys_code,
             span_id=span_id,
             incremental=incremental,
             enable_vis=enable_vis,
         )
         response = await self._http_client.post(
-            self._api_url + "/chat/completions", json=request.dict()
+            self._api_url + "/chat/completions", json=model_to_dict(request)
         )
         if response.status_code == 200:
             json_data = json.loads(response.text)
             chat_completion_response = ChatCompletionResponse(**json_data)
             return chat_completion_response
         else:
             return json.loads(response.content)
@@ -218,15 +219,15 @@
 
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5000/api/v2"
+            DBGPT_API_BASE = "http://localhost:5670/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             res = await client.chat_stream(model="chatgpt_proxyllm", messages="Hello?")
         """
         request = ChatCompletionRequestBody(
             model=model,
             messages=messages,
@@ -238,15 +239,15 @@
             conv_uid=conv_uid,
             user_name=user_name,
             sys_code=sys_code,
             span_id=span_id,
             incremental=incremental,
             enable_vis=enable_vis,
         )
-        async for chat_completion_response in self._chat_stream(request.dict()):
+        async for chat_completion_response in self._chat_stream(model_to_dict(request)):
             yield chat_completion_response
 
     async def _chat_stream(
         self, data: Dict[str, Any]
     ) -> AsyncGenerator[ChatCompletionStreamResponse, None]:
         """Chat Stream Completion.
 
@@ -258,14 +259,15 @@
         async with self._http_client.stream(
             method="POST",
             url=self._api_url + "/chat/completions",
             json=data,
             headers={},
         ) as response:
             if response.status_code == 200:
+                sse_data = ""
                 async for line in response.aiter_lines():
                     try:
                         if line.strip() == "data: [DONE]":
                             break
                         if line.startswith("data:"):
                             if line.startswith("data: "):
                                 sse_data = line[len("data: ") :]
@@ -273,15 +275,17 @@
                                 sse_data = line[len("data:") :]
                             json_data = json.loads(sse_data)
                             chat_completion_response = ChatCompletionStreamResponse(
                                 **json_data
                             )
                             yield chat_completion_response
                     except Exception as e:
-                        raise e
+                        raise Exception(
+                            f"Failed to parse SSE data: {e}, sse_data: {sse_data}"
+                        )
 
             else:
                 try:
                     error = await response.aread()
                     yield json.loads(error)
                 except Exception as e:
                     raise e
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/client/datasource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """this module contains the datasource client functions."""
 from typing import List
 
+from dbgpt._private.pydantic import model_to_dict
 from dbgpt.core.schema.api import Result
 
 from .client import Client, ClientException
 from .schema import DatasourceModel
 
 
 async def create_datasource(
@@ -13,15 +14,15 @@
     """Create a new datasource.
 
     Args:
         client (Client): The dbgpt client.
         datasource (DatasourceModel): The datasource model.
     """
     try:
-        res = await client.get("/datasources", datasource.dict())
+        res = await client.get("/datasources", model_to_dict(datasource))
         result: Result = res.json()
         if result["success"]:
             return DatasourceModel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to create datasource: {e}")
@@ -37,15 +38,15 @@
         datasource (DatasourceModel): The datasource model.
     Returns:
         DatasourceModel: The datasource model.
     Raises:
         ClientException: If the request failed.
     """
     try:
-        res = await client.put("/datasources", datasource.dict())
+        res = await client.put("/datasources", model_to_dict(datasource))
         result: Result = res.json()
         if result["success"]:
             return DatasourceModel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to update datasource: {e}")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/flow.py` & `dbgpt-0.5.5rc0/dbgpt/client/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Create a new flow.
 
     Args:
         client (Client): The dbgpt client.
         flow (FlowPanel): The flow panel.
     """
     try:
-        res = await client.get("/awel/flows", flow.dict())
+        res = await client.get("/awel/flows", flow.to_dict())
         result: Result = res.json()
         if result["success"]:
             return FlowPanel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to create flow: {e}")
@@ -33,15 +33,15 @@
         flow (FlowPanel): The flow panel.
     Returns:
         FlowPanel: The flow panel.
     Raises:
         ClientException: If the request failed.
     """
     try:
-        res = await client.put("/awel/flows", flow.dict())
+        res = await client.put("/awel/flows", flow.to_dict())
         result: Result = res.json()
         if result["success"]:
             return FlowPanel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to update flow: {e}")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/client/knowledge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Knowledge API client."""
 import json
 from typing import List
 
+from dbgpt._private.pydantic import model_to_dict, model_to_json
 from dbgpt.core.schema.api import Result
 
 from .client import Client, ClientException
 from .schema import DocumentModel, SpaceModel, SyncModel
 
 
 async def create_space(client: Client, space_model: SpaceModel) -> SpaceModel:
@@ -16,15 +17,15 @@
         space_model (SpaceModel): The space model.
     Returns:
         SpaceModel: The space model.
     Raises:
         ClientException: If the request failed.
     """
     try:
-        res = await client.post("/knowledge/spaces", space_model.dict())
+        res = await client.post("/knowledge/spaces", model_to_dict(space_model))
         result: Result = res.json()
         if result["success"]:
             return SpaceModel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to create space: {e}")
@@ -38,15 +39,15 @@
         space_model (SpaceModel): The space model.
     Returns:
         SpaceModel: The space model.
     Raises:
         ClientException: If the request failed.
     """
     try:
-        res = await client.put("/knowledge/spaces", space_model.dict())
+        res = await client.put("/knowledge/spaces", model_to_dict(space_model))
         result: Result = res.json()
         if result["success"]:
             return SpaceModel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to update space: {e}")
@@ -122,15 +123,15 @@
 
     Args:
         client (Client): The dbgpt client.
         doc_model (SpaceModel): The document model.
 
     """
     try:
-        res = await client.post_param("/knowledge/documents", doc_model.dict())
+        res = await client.post_param("/knowledge/documents", model_to_dict(doc_model))
         result: Result = res.json()
         if result["success"]:
             return DocumentModel(**result["data"])
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
         raise ClientException(f"Failed to create document: {e}")
@@ -206,15 +207,15 @@
     Returns:
         List: The list of document ids.
     Raises:
         ClientException: If the request failed.
     """
     try:
         res = await client.post(
-            "/knowledge/documents/sync", [json.loads(sync_model.json())]
+            "/knowledge/documents/sync", [json.loads(model_to_json(sync_model))]
         )
         result: Result = res.json()
         if result["success"]:
             return result["data"]
         else:
             raise ClientException(status=result["err_code"], reason=result)
     except Exception as e:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/client/schema.py` & `dbgpt-0.5.5rc0/dbgpt/client/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from fastapi import File, UploadFile
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 from dbgpt.rag.chunk_manager import ChunkParameters
 
 
 class ChatCompletionRequestBody(BaseModel):
     """ChatCompletion LLM http request body."""
 
     model: str = Field(
@@ -56,15 +56,15 @@
     )
     incremental: bool = Field(
         default=True,
         description="Used to control whether the content is returned incrementally "
         "or in full each time. "
         "If this parameter is not provided, the default is full return.",
     )
-    enable_vis: str = Field(
+    enable_vis: bool = Field(
         default=True, description="response content whether to output vis label"
     )
 
 
 class ChatMode(Enum):
     """Chat mode."""
 
@@ -263,14 +263,16 @@
     """doc_source: doc source"""
     space_id: str = Field(None, description="space_id")
 
 
 class SyncModel(BaseModel):
     """Sync model."""
 
+    model_config = ConfigDict(protected_namespaces=())
+
     """doc_id: doc id"""
     doc_id: str = Field(None, description="The doc id")
 
     """space id"""
     space_id: str = Field(None, description="The space id")
 
     """model_name: model name"""
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/component.py` & `dbgpt-0.5.5rc0/dbgpt/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     TRACER = "dbgpt_tracer"
     TRACER_SPAN_STORAGE = "dbgpt_tracer_span_storage"
     RAG_GRAPH_DEFAULT = "dbgpt_rag_engine_default"
     AWEL_TRIGGER_MANAGER = "dbgpt_awel_trigger_manager"
     AWEL_DAG_MANAGER = "dbgpt_awel_dag_manager"
     UNIFIED_METADATA_DB_MANAGER_FACTORY = "dbgpt_unified_metadata_db_manager_factory"
     CONNECTOR_MANAGER = "dbgpt_connector_manager"
+    AGENT_MANAGER = "dbgpt_agent_manager"
 
 
 _EMPTY_DEFAULT_COMPONENT = "_EMPTY_DEFAULT_COMPONENT"
 
 
 @PublicAPI(stability="beta")
 class BaseComponent(LifeCycle, ABC):
@@ -292,31 +293,33 @@
         await asyncio.gather(*tasks)
 
     def _build(self):
         """Integrate lifecycle events with the internal ASGI app if available."""
         if not self.app:
             self._register_exit_handler()
             return
+        from dbgpt.util.fastapi import register_event_handler
 
-        @self.app.on_event("startup")
         async def startup_event():
             """ASGI app startup event handler."""
 
             async def _startup_func():
                 try:
                     await self.async_after_start()
                 except Exception as e:
                     logger.error(f"Error starting system app: {e}")
                     sys.exit(1)
 
             asyncio.create_task(_startup_func())
             self.after_start()
 
-        @self.app.on_event("shutdown")
         async def shutdown_event():
             """ASGI app shutdown event handler."""
             await self.async_before_stop()
             self.before_stop()
 
+        register_event_handler(self.app, "startup", startup_event)
+        register_event_handler(self.app, "shutdown", shutdown_event)
+
     def _register_exit_handler(self):
         """Register an exit handler to stop the system app."""
         atexit.register(self.before_stop)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/configs/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/configs/model_config.py` & `dbgpt-0.5.5rc0/dbgpt/configs/model_config.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,17 @@
 
     if not logger_filename:
         logger_filename = "dbgpt_awel_dev.log"
     setup_logging("dbgpt", logging_level=logging_level, logger_filename=logger_filename)
 
     start_http = _check_has_http_trigger(dags)
     if start_http:
-        from fastapi import FastAPI
+        from dbgpt.util.fastapi import create_app
 
-        app = FastAPI()
+        app = create_app()
     else:
         app = None
     system_app = SystemApp(app)
     DAGVar.set_current_system_app(system_app)
     trigger_manager = DefaultTriggerManager()
     system_app.register_instance(trigger_manager)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """DAGManager is a component of AWEL, it is used to manage DAGs.
 
 DAGManager will load DAGs from dag_dirs, and register the trigger nodes
 to TriggerManager.
 """
 import logging
+import threading
 from typing import Dict, List, Optional
 
 from dbgpt.component import BaseComponent, ComponentType, SystemApp
 
 from .base import DAG
 from .loader import LocalFileDAGLoader
 
@@ -25,14 +26,15 @@
         Args:
             system_app (SystemApp): The system app.
             dag_dirs (List[str]): The directories to load DAGs.
         """
         from ..trigger.trigger_manager import DefaultTriggerManager
 
         super().__init__(system_app)
+        self.lock = threading.Lock()
         self.dag_loader = LocalFileDAGLoader(dag_dirs)
         self.system_app = system_app
         self.dag_map: Dict[str, DAG] = {}
         self.dag_alias_map: Dict[str, str] = {}
         self._trigger_manager: Optional["DefaultTriggerManager"] = None
 
     def init_app(self, system_app: SystemApp):
@@ -57,45 +59,60 @@
 
     def after_start(self):
         """Execute after the application starts."""
         self.load_dags()
 
     def register_dag(self, dag: DAG, alias_name: Optional[str] = None):
         """Register a DAG."""
-        dag_id = dag.dag_id
-        if dag_id in self.dag_map:
-            raise ValueError(f"Register DAG error, DAG ID {dag_id} has already exist")
-        self.dag_map[dag_id] = dag
-        if alias_name:
-            self.dag_alias_map[alias_name] = dag_id
-
-        if self._trigger_manager:
-            for trigger in dag.trigger_nodes:
-                self._trigger_manager.register_trigger(trigger, self.system_app)
-            self._trigger_manager.after_register()
-        else:
-            logger.warning("No trigger manager, not register dag trigger")
+        with self.lock:
+            dag_id = dag.dag_id
+            if dag_id in self.dag_map:
+                raise ValueError(
+                    f"Register DAG error, DAG ID {dag_id} has already exist"
+                )
+            self.dag_map[dag_id] = dag
+            if alias_name:
+                self.dag_alias_map[alias_name] = dag_id
+
+            if self._trigger_manager:
+                for trigger in dag.trigger_nodes:
+                    self._trigger_manager.register_trigger(trigger, self.system_app)
+                self._trigger_manager.after_register()
+            else:
+                logger.warning("No trigger manager, not register dag trigger")
 
     def unregister_dag(self, dag_id: str):
         """Unregister a DAG."""
-        if dag_id not in self.dag_map:
-            raise ValueError(f"Unregister DAG error, DAG ID {dag_id} does not exist")
-        dag = self.dag_map[dag_id]
-        # Clear the alias map
-        for alias_name, _dag_id in self.dag_alias_map.items():
-            if _dag_id == dag_id:
+        with self.lock:
+            if dag_id not in self.dag_map:
+                raise ValueError(
+                    f"Unregister DAG error, DAG ID {dag_id} does not exist"
+                )
+            dag = self.dag_map[dag_id]
+
+            # Collect aliases to remove
+            # TODO(fangyinc): It can be faster if we maintain a reverse map
+            aliases_to_remove = [
+                alias_name
+                for alias_name, _dag_id in self.dag_alias_map.items()
+                if _dag_id == dag_id
+            ]
+            # Remove collected aliases
+            for alias_name in aliases_to_remove:
                 del self.dag_alias_map[alias_name]
 
-        if self._trigger_manager:
-            for trigger in dag.trigger_nodes:
-                self._trigger_manager.unregister_trigger(trigger, self.system_app)
-        del self.dag_map[dag_id]
+            if self._trigger_manager:
+                for trigger in dag.trigger_nodes:
+                    self._trigger_manager.unregister_trigger(trigger, self.system_app)
+            # Finally remove the DAG from the map
+            del self.dag_map[dag_id]
 
     def get_dag(
         self, dag_id: Optional[str] = None, alias_name: Optional[str] = None
     ) -> Optional[DAG]:
         """Get a DAG by dag_id or alias_name."""
+        # Not lock, because it is read only and need to be fast
         if dag_id and dag_id in self.dag_map:
             return self.dag_map[dag_id]
         if alias_name in self.dag_alias_map:
             return self.dag_map.get(self.dag_alias_map[alias_name])
         return None
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 import dataclasses
 import inspect
 from abc import ABC
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union, cast
 
-from dbgpt._private.pydantic import BaseModel, Field, ValidationError, root_validator
+from dbgpt._private.pydantic import (
+    BaseModel,
+    Field,
+    ValidationError,
+    model_to_dict,
+    model_validator,
+)
 from dbgpt.core.awel.util.parameter_util import BaseDynamicOptions, OptionValue
 from dbgpt.core.interface.serialization import Serializable
 
 from .exceptions import FlowMetadataException, FlowParameterMetadataException
 
 _TYPE_REGISTRY: Dict[str, Type] = {}
 
@@ -277,15 +283,15 @@
         ...,
         description="The type class of the parameter",
         examples=["builtins.str", "builtins.int"],
     )
 
     def new(self: TM) -> TM:
         """Copy the metadata."""
-        return self.__class__(**self.dict())
+        return self.__class__(**self.model_dump(exclude_defaults=True))
 
 
 class Parameter(TypeMetadata, Serializable):
     """Parameter for build operator."""
 
     label: str = Field(
         ..., description="The label to display in UI", examples=["OpenAI API Key"]
@@ -328,20 +334,23 @@
     options: Optional[Union[BaseDynamicOptions, List[OptionValue]]] = Field(
         None, description="The options of the parameter"
     )
     value: Optional[Any] = Field(
         None, description="The value of the parameter(Saved in the dag file)"
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata.
 
         Transform the value to the real type.
         """
+        if not isinstance(values, dict):
+            return values
         type_cls = values.get("type_cls")
         to_handle_values = {
             "value": values.get("value"),
             "default": values.get("default"),
         }
         if type_cls:
             for k, v in to_handle_values.items():
@@ -439,15 +448,15 @@
             description=data["description"],
             options=data["options"],
             value=data["value"],
         )
 
     def to_dict(self) -> Dict:
         """Convert current metadata to json dict."""
-        dict_value = self.dict(exclude={"options"})
+        dict_value = model_to_dict(self, exclude={"options"})
         if not self.options:
             dict_value["options"] = None
         elif isinstance(self.options, BaseDynamicOptions):
             values = self.options.option_values()
             dict_value["options"] = [value.to_dict() for value in values]
         else:
             dict_value["options"] = [value.to_dict() for value in self.options]
@@ -531,15 +540,15 @@
         ...,
         description="The description of the field",
         examples=["The LLM operator.", "OpenAI LLM Client"],
     )
 
     def to_dict(self) -> Dict:
         """Convert current metadata to json dict."""
-        return self.dict()
+        return model_to_dict(self)
 
 
 class Resource(BaseResource, TypeMetadata):
     """The resource of the operator."""
 
     pass
 
@@ -689,17 +698,20 @@
             runnable_parameters.update(
                 current_parameters[view_param_key].to_runnable_parameter(
                     view_param.get_typed_value(), resources, key_to_resource_instance
                 )
             )
         return runnable_parameters
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def base_pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata."""
+        if not isinstance(values, dict):
+            return values
         if "category_label" not in values:
             category = values["category"]
             if isinstance(category, str):
                 if issubclass(cls, ResourceMetadata):
                     category = ResourceCategory.value_of(category)
                 else:
                     category = OperatorCategory.value_of(category)
@@ -709,15 +721,15 @@
     def get_origin_id(self) -> str:
         """Get the origin id."""
         split_ids = self.id.split("_")
         return "_".join(split_ids[:-1])
 
     def to_dict(self) -> Dict:
         """Convert current metadata to json dict."""
-        dict_value = self.dict(exclude={"parameters"})
+        dict_value = model_to_dict(self, exclude={"parameters"})
         dict_value["parameters"] = [
             parameter.to_dict() for parameter in self.parameters
         ]
         return dict_value
 
 
 class ResourceMetadata(BaseMetadata, TypeMetadata):
@@ -734,17 +746,20 @@
         description="The parent class of the resource",
         examples=[
             "dbgpt.core.interface.llm.LLMClient",
             "resource_dbgpt.model.proxy.llms.chatgpt.OpenAILLMClient",
         ],
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata."""
+        if not isinstance(values, dict):
+            return values
         if "flow_type" not in values:
             values["flow_type"] = "resource"
         if "id" not in values:
             values["id"] = values["flow_type"] + "_" + values["type_cls"]
         return values
 
     def new_alias(self, alias: Optional[List[str]] = None) -> List[str]:
@@ -842,17 +857,20 @@
 
     type_cls: Optional[str] = Field(
         default=None,
         description="The type class of the operator",
         examples=["dbgpt.model.operators.LLMOperator"],
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata."""
+        if not isinstance(values, dict):
+            return values
         if "flow_type" not in values:
             values["flow_type"] = "operator"
         if "id" not in values:
             key = cls.get_key(
                 values["name"], values["category"], values.get("version", "v1")
             )
             values["id"] = values["flow_type"] + "_" + key
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/compat.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/compat.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 import logging
 import uuid
 from contextlib import suppress
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
-from dbgpt._private.pydantic import BaseModel, Field, root_validator, validator
+from dbgpt._private.pydantic import (
+    BaseModel,
+    Field,
+    field_validator,
+    model_to_dict,
+    model_validator,
+)
 from dbgpt.core.awel.dag.base import DAG, DAGNode
 
 from .base import (
     OperatorType,
     ResourceMetadata,
     ResourceType,
     ViewMetadata,
@@ -69,15 +75,16 @@
     data: Union[ViewMetadata, ResourceMetadata] = Field(
         ..., description="Data of the node"
     )
     position_absolute: FlowPositionData = Field(
         ..., description="Absolute position of the node"
     )
 
-    @validator("data", pre=True)
+    @field_validator("data", mode="before")
+    @classmethod
     def parse_data(cls, value: Any):
         """Parse the data."""
         if isinstance(value, dict):
             flow_type = value.get("flow_type")
             if flow_type == "operator":
                 return ViewMetadata(**value)
             elif flow_type == "resource":
@@ -119,17 +126,20 @@
     )
     type: Optional[str] = Field(
         default=None,
         description="Type of current UI node(Just for UI)",
         examples=["buttonedge"],
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata."""
+        if not isinstance(values, dict):
+            return values
         if (
             "source_order" not in values
             and "source_handle" in values
             and values["source_handle"] is not None
         ):
             with suppress(Exception):
                 values["source_order"] = int(values["source_handle"].split("|")[-1])
@@ -311,28 +321,35 @@
     )
     gmt_modified: Optional[str] = Field(
         None,
         description="The flow panel modified time.",
         examples=["2021-08-01 12:00:00", "2021-08-01 12:00:01", "2021-08-01 12:00:02"],
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the metadata."""
+        if not isinstance(values, dict):
+            return values
         label = values.get("label")
         name = values.get("name")
         flow_category = str(values.get("flow_category", ""))
         if not label and name:
             values["label"] = name
             name = name.replace(" ", "_")
             if flow_category:
                 name = str(flow_category) + "_" + name
             values["name"] = name
         return values
 
+    def to_dict(self) -> Dict[str, Any]:
+        """Convert to dict."""
+        return model_to_dict(self)
+
 
 class FlowFactory:
     """Flow factory."""
 
     def __init__(self, dag_prefix: str = "flow_dag"):
         """Init the flow factory."""
         self._dag_prefix = dag_prefix
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/ext_http_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,22 @@
     Optional,
     Type,
     Union,
     cast,
     get_origin,
 )
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import (
+    BaseModel,
+    Field,
+    field_is_required,
+    field_outer_type,
+    model_fields,
+    model_to_dict,
+)
 from dbgpt.util.i18n_utils import _
 
 from ..dag.base import DAG
 from ..flow import (
     IOField,
     OperatorCategory,
     OperatorType,
@@ -57,15 +64,15 @@
         super().__init__(msg)
         self.msg = msg
         self.code = code
 
 
 def _default_streaming_predict_func(body: "CommonRequestType") -> bool:
     if isinstance(body, BaseModel):
-        body = body.dict()
+        body = model_to_dict(body)
     elif isinstance(body, str):
         try:
             body = json.loads(body)
         except Exception:
             return False
     elif not isinstance(body, dict):
         return False
@@ -250,15 +257,15 @@
     )
     incremental: bool = Field(
         default=True,
         description="Used to control whether the content is returned incrementally "
         "or in full each time. "
         "If this parameter is not provided, the default is full return.",
     )
-    enable_vis: str = Field(
+    enable_vis: bool = Field(
         default=True, description="response content whether to output vis label"
     )
     extra: Optional[Dict[str, Any]] = Field(
         default=None, description="The extra info of the model inference"
     )
 
     @property
@@ -570,26 +577,28 @@
                     else:
                         body = req_body_cls(**kwargs)
                     return await _trigger_dag_func(body)
 
                 if isinstance(req_body_cls, type) and issubclass(
                     req_body_cls, BaseModel
                 ):
-                    fields = req_body_cls.__fields__  # type: ignore
+                    fields = model_fields(req_body_cls)  # type: ignore
                     parameters = []
                     for field_name, field in fields.items():
                         default_value = (
-                            Parameter.empty if field.required else field.default
+                            Parameter.empty
+                            if field_is_required(field)
+                            else field.default
                         )
                         parameters.append(
                             Parameter(
                                 name=field_name,
                                 kind=Parameter.KEYWORD_ONLY,
                                 default=default_value,
-                                annotation=field.outer_type_,
+                                annotation=field_outer_type(field),
                             )
                         )
                 elif req_body_cls == Dict[str, Any] or req_body_cls == dict:
                     raise AWELHttpError(
                         f"Query methods {self._methods} not support dict type"
                     )
                 else:
@@ -1025,15 +1034,15 @@
     def __init__(self, prefix_key: Optional[str] = None, **kwargs):
         """Initialize a RequestBodyToDictOperator."""
         super().__init__(**kwargs)
         self._key = prefix_key
 
     async def map(self, request_body: CommonLLMHttpRequestBody) -> Dict[str, Any]:
         """Map the request body to response body."""
-        dict_value = request_body.dict()
+        dict_value = model_to_dict(request_body)
         if not self._key:
             return dict_value
         else:
             keys = self._key.split(".")
             for k in keys:
                 dict_value = dict_value[k]
             if not isinstance(dict_value, dict):
@@ -1134,13 +1143,13 @@
     def __init__(self, key: str = "user_input", **kwargs):
         """Initialize a UserInputParsedOperator."""
         self._key = key
         super().__init__(**kwargs)
 
     async def map(self, request_body: CommonLLMHttpRequestBody) -> str:
         """Map the request body to response body."""
-        dict_value = request_body.dict()
+        dict_value = model_to_dict(request_body)
         if not self._key or self._key not in dict_value:
             raise ValueError(
                 f"Prefix key {self._key} is not a valid key of the request body"
             )
         return dict_value[self._key]
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The parameter utility."""
 
 import inspect
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List
 
-from dbgpt._private.pydantic import BaseModel, Field, root_validator
+from dbgpt._private.pydantic import BaseModel, Field, model_validator
 from dbgpt.core.interface.serialization import Serializable
 
 _DEFAULT_DYNAMIC_REGISTRY = {}
 
 
 class OptionValue(Serializable, BaseModel):
     """The option value of the parameter."""
@@ -40,17 +40,20 @@
         ..., description="The unique id of the function to generate the dynamic options"
     )
 
     def option_values(self) -> List[OptionValue]:
         """Return the option values of the parameter."""
         return self.func()
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the function id."""
+        if not isinstance(values, dict):
+            return values
         func = values.get("func")
         if func is None:
             raise ValueError(
                 "The function to generate the dynamic options is required."
             )
         func_id = _generate_unique_id(func)
         values["func_id"] = func_id
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Chunk document schema."""
 
 import json
 import uuid
 from typing import Any, Dict
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, Field, model_to_dict
 
 
 class Document(BaseModel):
     """Document including document content, document metadata."""
 
     content: str = Field(default="", description="document text content")
 
@@ -60,15 +60,15 @@
     separator: str = Field(
         default="\n",
         description="Separator between metadata fields when converting to string.",
     )
 
     def to_dict(self, **kwargs: Any) -> Dict[str, Any]:
         """Convert Chunk to dict."""
-        data = self.dict(**kwargs)
+        data = model_to_dict(self, **kwargs)
         data["class_name"] = self.class_name()
         return data
 
     def to_json(self, **kwargs: Any) -> str:
         """Convert Chunk to json."""
         data = self.to_dict(**kwargs)
         return json.dumps(data)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
 from typing import Any, AsyncIterator, Dict, List, Optional, Union
 
 from cachetools import TTLCache
 
-from dbgpt._private.pydantic import BaseModel
+from dbgpt._private.pydantic import BaseModel, model_to_dict
 from dbgpt.core.interface.message import ModelMessage, ModelMessageRoleType
 from dbgpt.util import BaseParameters
 from dbgpt.util.annotations import PublicAPI
 from dbgpt.util.model_utils import GPUInfo
 
 logger = logging.getLogger(__name__)
 
@@ -308,15 +308,15 @@
         if not context:
             context = ModelRequestContext(stream=stream)
         elif not isinstance(context, ModelRequestContext):
             context_dict = None
             if isinstance(context, dict):
                 context_dict = context
             elif isinstance(context, BaseModel):
-                context_dict = context.dict()
+                context_dict = model_to_dict(context)
             if context_dict and "stream" not in context_dict:
                 context_dict["stream"] = stream
             if context_dict:
                 context = ModelRequestContext(**context_dict)
             else:
                 context = ModelRequestContext(stream=stream)
         return ModelRequest(
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/message.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, Field, model_to_dict
 from dbgpt.core.interface.storage import (
     InMemoryStorage,
     ResourceIdentifier,
     StorageInterface,
     StorageItem,
 )
 
@@ -38,15 +38,15 @@
         """Convert to dict.
 
         Returns:
             Dict: The dict object
         """
         return {
             "type": self.type,
-            "data": self.dict(),
+            "data": model_to_dict(self),
             "index": self.index,
             "round_index": self.round_index,
         }
 
     @staticmethod
     def messages_to_string(messages: List["BaseMessage"]) -> str:
         """Convert messages to str.
@@ -260,15 +260,15 @@
 
         Args:
             messages (List["ModelMessage"]): The model messages
 
         Returns:
             List[Dict[str, str]]: The dict list
         """
-        return list(map(lambda m: m.dict(), messages))
+        return list(map(lambda m: model_to_dict(m), messages))
 
     @staticmethod
     def build_human_message(content: str) -> "ModelMessage":
         """Build human message.
 
         Args:
             content (str): The content
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The prompt operator."""
 from abc import ABC
 from typing import Any, Dict, List, Optional, Union
 
-from dbgpt._private.pydantic import root_validator
+from dbgpt._private.pydantic import model_validator
 from dbgpt.core import (
     ModelMessage,
     ModelMessageRoleType,
     ModelOutput,
     StorageConversation,
 )
 from dbgpt.core.awel import JoinOperator, MapOperator
@@ -67,17 +67,20 @@
             description=_("The human message."),
         ),
     ],
 )
 class CommonChatPromptTemplate(ChatPromptTemplate):
     """The common chat prompt template."""
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre fill the messages."""
+        if not isinstance(values, dict):
+            return values
         if "system_message" not in values:
             values["system_message"] = "You are a helpful AI Assistant."
         if "human_message" not in values:
             values["human_message"] = "{user_input}"
         if "message_placeholder" not in values:
             values["message_placeholder"] = "chat_history"
         system_message = values.pop("system_message")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import dataclasses
 import json
 from abc import ABC, abstractmethod
 from string import Formatter
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 
-from dbgpt._private.pydantic import BaseModel, root_validator
+from dbgpt._private.pydantic import BaseModel, ConfigDict, model_validator
 from dbgpt.core.interface.message import BaseMessage, HumanMessage, SystemMessage
 from dbgpt.core.interface.storage import (
     InMemoryStorage,
     QuerySpec,
     ResourceIdentifier,
     StorageInterface,
     StorageItem,
@@ -47,14 +47,16 @@
     input_variables: List[str]
     """A list of the names of the variables the prompt template expects."""
 
 
 class PromptTemplate(BasePromptTemplate):
     """Prompt template."""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     template: str
     """The prompt template."""
 
     template_format: str = "f-string"
     """The format of the prompt template. Options are: 'f-string', 'jinja2'."""
 
     response_key: str = "response"
@@ -65,19 +67,14 @@
     response_format: Optional[str] = None
 
     template_scene: Optional[str] = None
 
     template_define: Optional[str] = None
     """this template define"""
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        arbitrary_types_allowed = True
-
     @property
     def _prompt_type(self) -> str:
         """Return the prompt type key."""
         return "prompt"
 
     def format(self, **kwargs: Any) -> str:
         """Format the prompt with the inputs."""
@@ -235,17 +232,20 @@
                     k: v for k, v in kwargs.items() if k in message.input_variables
                 }
                 result_messages.extend(message.format_messages(**pass_kwargs))
             else:
                 raise ValueError(f"Unsupported message type: {type(message)}")
         return result_messages
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def base_pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre-fill the messages."""
+        if not isinstance(values, dict):
+            return values
         input_variables = values.get("input_variables", {})
         messages = values.get("messages", [])
         if not input_variables:
             input_variables = set()
             for message in messages:
                 if isinstance(message, (BaseChatPromptTemplate, MessagesPlaceholder)):
                     input_variables.update(message.input_variables)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, Type
 
 
 class Serializable(ABC):
     """The serializable abstract class."""
 
-    serializer: Optional["Serializer"] = None
+    _serializer: Optional["Serializer"] = None
 
     @abstractmethod
     def to_dict(self) -> Dict:
         """Convert the object's state to a dictionary."""
 
     def serialize(self) -> bytes:
         """Convert the object into bytes for storage or transmission.
 
         Returns:
             bytes: The byte array after serialization
         """
-        if self.serializer is None:
+        if self._serializer is None:
             raise ValueError(
-                "Serializer is not set. Please set the serializer before serialization."
+                "Serializer is not set. Please set the serializer before "
+                "serialization."
             )
-        return self.serializer.serialize(self)
+        return self._serializer.serialize(self)
 
     def set_serializer(self, serializer: "Serializer") -> None:
         """Set the serializer for current serializable object.
 
         Args:
             serializer (Serializer): The serializer to set
         """
-        self.serializer = serializer
+        self._serializer = serializer
 
 
 class Serializer(ABC):
     """The serializer abstract class for serializing cache keys and values."""
 
     @abstractmethod
     def serialize(self, obj: Serializable) -> bytes:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py` & `dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,28 +422,28 @@
         """Save the data to the storage.
 
         Args:
             data (T): The data to save
         """
         if not data:
             raise StorageError("Data cannot be None")
-        if not data.serializer:
+        if not data._serializer:
             data.set_serializer(self.serializer)
 
         if data.identifier.str_identifier in self._data:
             raise StorageError(
                 f"Data with identifier {data.identifier.str_identifier} already exists"
             )
         self._data[data.identifier.str_identifier] = data.serialize()
 
     def update(self, data: T) -> None:
         """Update the data to the storage."""
         if not data:
             raise StorageError("Data cannot be None")
-        if not data.serializer:
+        if not data._serializer:
             data.set_serializer(self.serializer)
         self._data[data.identifier.str_identifier] = data.serialize()
 
     def save_or_update(self, data: T) -> None:
         """Save or update the data to the storage."""
         self.update(data)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/base.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/manages/connect_config_db.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/cli.py` & `dbgpt-0.5.5rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/parameter.py` & `dbgpt-0.5.5rc0/dbgpt/model/parameter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/moonshot.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 from typing import Any, Dict, List, Optional
 
 import aiohttp
 import requests
 
-from dbgpt._private.pydantic import BaseModel, Extra, Field
+from dbgpt._private.pydantic import EXTRA_FORBID, BaseModel, ConfigDict, Field
 from dbgpt.core import Embeddings
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.util.i18n_utils import _
 
 DEFAULT_MODEL_NAME = "sentence-transformers/all-mpnet-base-v2"
 DEFAULT_INSTRUCT_MODEL = "hkunlp/instructor-large"
 DEFAULT_BGE_MODEL = "BAAI/bge-large-en"
@@ -60,14 +60,16 @@
             hf = HuggingFaceEmbeddings(
                 model_name=model_name,
                 model_kwargs=model_kwargs,
                 encode_kwargs=encode_kwargs,
             )
     """
 
+    model_config = ConfigDict(extra=EXTRA_FORBID, protected_namespaces=())
+
     client: Any  #: :meta private:
     model_name: str = DEFAULT_MODEL_NAME
     """Model name to use."""
     cache_folder: Optional[str] = None
     """Path to store models. Can be also set by SENTENCE_TRANSFORMERS_HOME
     environment variable."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
@@ -89,19 +91,14 @@
                 "Please install it with `pip install sentence-transformers`."
             ) from exc
 
         self.client = sentence_transformers.SentenceTransformer(
             self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
         )
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
@@ -180,14 +177,16 @@
             hf = HuggingFaceInstructEmbeddings(
                 model_name=model_name,
                 model_kwargs=model_kwargs,
                 encode_kwargs=encode_kwargs,
             )
     """
 
+    model_config = ConfigDict(extra=EXTRA_FORBID, protected_namespaces=())
+
     client: Any  #: :meta private:
     model_name: str = DEFAULT_INSTRUCT_MODEL
     """Model name to use."""
     cache_folder: Optional[str] = None
     """Path to store models. Can be also set by SENTENCE_TRANSFORMERS_HOME
     environment variable."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
@@ -207,19 +206,14 @@
 
             self.client = INSTRUCTOR(
                 self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
             )
         except ImportError as e:
             raise ImportError("Dependencies for InstructorEmbedding not found.") from e
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace instruct model.
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
@@ -263,14 +257,16 @@
             hf = HuggingFaceBgeEmbeddings(
                 model_name=model_name,
                 model_kwargs=model_kwargs,
                 encode_kwargs=encode_kwargs,
             )
     """
 
+    model_config = ConfigDict(extra=EXTRA_FORBID, protected_namespaces=())
+
     client: Any  #: :meta private:
     model_name: str = DEFAULT_BGE_MODEL
     """Model name to use."""
     cache_folder: Optional[str] = None
     """Path to store models.
     Can be also set by SENTENCE_TRANSFORMERS_HOME environment variable."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
@@ -294,19 +290,14 @@
 
         self.client = sentence_transformers.SentenceTransformer(
             self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
         )
         if "-zh" in self.model_name:
             self.query_instruction = DEFAULT_QUERY_BGE_INSTRUCTION_ZH
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
@@ -356,14 +347,16 @@
 )
 class HuggingFaceInferenceAPIEmbeddings(BaseModel, Embeddings):
     """Embed texts using the HuggingFace API.
 
     Requires a HuggingFace Inference API key and a model name.
     """
 
+    model_config = ConfigDict(arbitrary_types_allowed=True, protected_namespaces=())
+
     api_key: str
     """Your API key for the HuggingFace Inference API."""
     model_name: str = "sentence-transformers/all-MiniLM-L6-v2"
     """The name of the model to use for text embeddings."""
 
     @property
     def _api_url(self) -> str:
@@ -471,14 +464,16 @@
     """Jina AI embeddings.
 
     This class is used to get embeddings for a list of texts using the Jina AI API.
     It requires an API key and a model name. The default model name is
     "jina-embeddings-v2-base-en".
     """
 
+    model_config = ConfigDict(arbitrary_types_allowed=True, protected_namespaces=())
+
     api_url: Any  #: :meta private:
     session: Any  #: :meta private:
     api_key: str
     """API key for the Jina AI API.."""
     model_name: str = "jina-embeddings-v2-base-en"
     """The name of the model to use for text embeddings. Defaults to
     "jina-embeddings-v2-base-en"."""
@@ -623,14 +618,16 @@
                 api_key="my_api_token",
                 model_name="text2vec",
             )
             texts = ["Hello, world!", "How are you?"]
             openai_embeddings.embed_documents(texts)
     """
 
+    model_config = ConfigDict(arbitrary_types_allowed=True, protected_namespaces=())
+
     api_url: str = Field(
         default="http://localhost:8100/api/v1/embeddings",
         description="The URL of the embeddings API.",
     )
     api_key: Optional[str] = Field(
         default=None, description="The API key for the embeddings API."
     )
@@ -639,19 +636,14 @@
     )
     timeout: int = Field(
         default=60, description="The timeout for the request in seconds."
     )
 
     session: Optional[requests.Session] = None
 
-    class Config:
-        """Configuration for this pydantic object."""
-
-        arbitrary_types_allowed = True
-
     def __init__(self, **kwargs):
         """Initialize the OpenAPIEmbeddings."""
         super().__init__(**kwargs)
         try:
             import requests
         except ImportError:
             raise ValueError(
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py` & `dbgpt-0.5.5rc0/dbgpt/rag/evaluation/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py` & `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/url.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/retriever/base.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py` & `dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Summary for rdbms database."""
-
+import re
 from typing import TYPE_CHECKING, List, Optional
 
 from dbgpt._private.config import Config
 from dbgpt.datasource import BaseConnector
 from dbgpt.rag.summary.db_summary import DBSummary
 
 if TYPE_CHECKING:
@@ -98,18 +98,28 @@
     for column in conn.get_columns(table_name):
         if column.get("comment"):
             columns.append(f"{column['name']} ({column.get('comment')})")
         else:
             columns.append(f"{column['name']}")
 
     column_str = ", ".join(columns)
+    # Obtain index information
     index_keys = []
-    for index_key in conn.get_indexes(table_name):
-        key_str = ", ".join(index_key["column_names"])
-        index_keys.append(f"{index_key['name']}(`{key_str}`) ")  # noqa
+    raw_indexes = conn.get_indexes(table_name)
+    for index in raw_indexes:
+        if isinstance(index, tuple):  # Process tuple type index information
+            index_name, index_creation_command = index
+            # Extract column names using re
+            matched_columns = re.findall(r"\(([^)]+)\)", index_creation_command)
+            if matched_columns:
+                key_str = ", ".join(matched_columns)
+                index_keys.append(f"{index_name}(`{key_str}`) ")
+        else:
+            key_str = ", ".join(index["column_names"])
+            index_keys.append(f"{index['name']}(`{key_str}`) ")
     table_str = summary_template.format(table_name=table_name, columns=column_str)
     if len(index_keys) > 0:
         index_key_str = ", ".join(index_keys)
         table_str += f", and index keys: {index_key_str}"
     try:
         comment = conn.get_table_comment(table_name)
     except Exception:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,24 +54,24 @@
                 f"Got a larger chunk overlap ({chunk_overlap}) than chunk size "
                 f"({chunk_size}), should be smaller."
             )
         # callback_manager = callback_manager or CallbackManager([])
         tokenizer = tokenizer or globals_helper.tokenizer
 
         all_seps = [separator] + (backup_separators or [])
-        self._split_fns = [split_by_sep(sep) for sep in all_seps] + [split_by_char()]
 
         super().__init__(
             chunk_size=chunk_size,
             chunk_overlap=chunk_overlap,
             separator=separator,
             backup_separators=backup_separators,
             # callback_manager=callback_manager,
             tokenizer=tokenizer,
         )
+        self._split_fns = [split_by_sep(sep) for sep in all_seps] + [split_by_char()]
 
     @classmethod
     def class_name(cls) -> str:
         """Return the class name."""
         return "TokenTextSplitter"
 
     def split_text_metadata_aware(self, text: str, metadata_str: str) -> List[str]:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from contextlib import contextmanager
 from typing import Any, Dict, Generic, Iterator, List, Optional, TypeVar, Union
 
 from sqlalchemy.orm.session import Session
 
+from dbgpt._private.pydantic import model_to_dict
 from dbgpt.util.pagination_utils import PaginationResult
 
 from .db_manager import BaseQuery, DatabaseManager, db
 
 # The entity type
 T = TypeVar("T")
 # The request schema type
@@ -161,15 +162,15 @@
             RES: The response schema object.
         """
         with self.session() as session:
             query = self._create_query_object(session, query_request)
             entry = query.first()
             if entry is None:
                 raise Exception("Invalid request")
-            for key, value in update_request.dict().items():  # type: ignore
+            for key, value in model_to_dict(update_request).items():  # type: ignore
                 if value is not None:
                     setattr(entry, key, value)
             session.merge(entry)
             res = self.get_one(self.to_request(entry))
             if not res:
                 raise Exception("Update failed")
             return res
@@ -268,15 +269,17 @@
             query_request (QUERY_SPEC): The request schema object or dict for query.
         Returns:
             BaseQuery: The query object.
         """
         model_cls = type(self.from_request(query_request))
         query = session.query(model_cls)
         query_dict = (
-            query_request if isinstance(query_request, dict) else query_request.dict()
+            query_request
+            if isinstance(query_request, dict)
+            else model_to_dict(query_request)
         )
         for key, value in query_dict.items():
             if value is not None:
                 if isinstance(value, (list, tuple, dict, set)):
                     continue
                 query = query.filter(getattr(model_cls, key) == value)
         return query  # type: ignore
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/schema.py` & `dbgpt-0.5.5rc0/dbgpt/storage/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Vector store base class."""
 import logging
 import math
 import time
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_to_dict
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import Parameter
 from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.i18n_utils import _
 
 logger = logging.getLogger(__name__)
 
@@ -83,18 +83,15 @@
     ),
 ]
 
 
 class VectorStoreConfig(BaseModel):
     """Vector store config."""
 
-    class Config:
-        """Config for BaseModel."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     name: str = Field(
         default="dbgpt_collection",
         description="The name of vector store, if not set, will use the default name.",
     )
     user: Optional[str] = Field(
         default=None,
@@ -118,14 +115,18 @@
     )
     max_threads: int = Field(
         default=1,
         description="The max number of threads to use. Default is 1. If you set this "
         "bigger than 1, please make sure your vector store is thread-safe.",
     )
 
+    def to_dict(self, **kwargs) -> Dict[str, Any]:
+        """Convert to dict."""
+        return model_to_dict(self, **kwargs)
+
 
 class VectorStoreBase(ABC):
     """Vector store base class."""
 
     @abstractmethod
     def load_document(self, chunks: List[Chunk]) -> List[str]:
         """Load document in vector database.
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 from typing import List, Optional
 
 from chromadb import PersistentClient
 from chromadb.config import Settings
 
-from dbgpt._private.pydantic import Field
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.configs.model_config import PILOT_PATH
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.util.i18n_utils import _
 
 from .base import _COMMON_PARAMETERS, VectorStoreBase, VectorStoreConfig
 from .filters import FilterOperator, MetadataFilters
@@ -34,38 +34,35 @@
             default=None,
         ),
     ],
 )
 class ChromaVectorConfig(VectorStoreConfig):
     """Chroma vector store config."""
 
-    class Config:
-        """Config for BaseModel."""
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
-        arbitrary_types_allowed = True
-
-    persist_path: str = Field(
+    persist_path: Optional[str] = Field(
         default=os.getenv("CHROMA_PERSIST_PATH", None),
         description="the persist path of vector store.",
     )
-    collection_metadata: dict = Field(
+    collection_metadata: Optional[dict] = Field(
         default=None,
         description="the index metadata of vector store, if not set, will use the "
         "default metadata.",
     )
 
 
 class ChromaStore(VectorStoreBase):
     """Chroma vector store."""
 
     def __init__(self, vector_store_config: ChromaVectorConfig) -> None:
         """Create a ChromaStore instance."""
         from langchain.vectorstores import Chroma
 
-        chroma_vector_config = vector_store_config.dict(exclude_none=True)
+        chroma_vector_config = vector_store_config.to_dict(exclude_none=True)
         chroma_path = chroma_vector_config.get(
             "persist_path", os.path.join(PILOT_PATH, "data")
         )
         self.persist_dir = os.path.join(
             chroma_path, vector_store_config.name + ".vectordb"
         )
         self.embeddings = vector_store_config.embedding_fn
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/filters.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Vector Store Meta data filters."""
 from enum import Enum
 from typing import List, Union
 
-from pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, Field
 
 
 class FilterOperator(str, Enum):
     """Meta data filter operator."""
 
     EQ = "=="
     GT = ">"
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 from typing import Any, Iterable, List, Optional
 
-from dbgpt._private.pydantic import Field
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.storage.vector_store.base import (
     _COMMON_PARAMETERS,
     VectorStoreBase,
     VectorStoreConfig,
 )
@@ -92,18 +92,15 @@
         ),
     ],
     description=_("Milvus vector store."),
 )
 class MilvusVectorConfig(VectorStoreConfig):
     """Milvus vector store config."""
 
-    class Config:
-        """Config for BaseModel."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     uri: str = Field(
         default="localhost",
         description="The uri of milvus store, if not set, will use the default uri.",
     )
     port: str = Field(
         default="19530",
@@ -151,15 +148,15 @@
         Args:
             vector_store_config (MilvusVectorConfig): MilvusStore config.
             refer to https://milvus.io/docs/v2.0.x/manage_connection.md
         """
         from pymilvus import connections
 
         connect_kwargs = {}
-        milvus_vector_config = vector_store_config.dict()
+        milvus_vector_config = vector_store_config.to_dict()
         self.uri = milvus_vector_config.get("uri") or os.getenv(
             "MILVUS_URL", "localhost"
         )
         self.port = milvus_vector_config.get("post") or os.getenv(
             "MILVUS_PORT", "19530"
         )
         self.username = milvus_vector_config.get("user") or os.getenv("MILVUS_USERNAME")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Postgres vector store."""
 import logging
 from typing import List, Optional
 
-from dbgpt._private.pydantic import Field
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.storage.vector_store.base import (
     _COMMON_PARAMETERS,
     VectorStoreBase,
     VectorStoreConfig,
 )
@@ -35,18 +35,15 @@
         ),
     ],
     description="PG vector store.",
 )
 class PGVectorConfig(VectorStoreConfig):
     """PG vector store config."""
 
-    class Config:
-        """Config for BaseModel."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     connection_string: str = Field(
         default=None,
         description="the connection string of vector store, if not set, will use the "
         "default connection string.",
     )
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Weaviate vector store."""
 import logging
 import os
 from typing import List, Optional
 
-from dbgpt._private.pydantic import Field
+from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import Chunk
 from dbgpt.core.awel.flow import Parameter, ResourceCategory, register_resource
 from dbgpt.util.i18n_utils import _
 
 from .base import _COMMON_PARAMETERS, VectorStoreBase, VectorStoreConfig
 from .filters import MetadataFilters
 
@@ -40,18 +40,15 @@
             default=None,
         ),
     ],
 )
 class WeaviateVectorConfig(VectorStoreConfig):
     """Weaviate vector store config."""
 
-    class Config:
-        """Config for BaseModel."""
-
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     weaviate_url: str = Field(
         default=os.getenv("WEAVIATE_URL", None),
         description="weaviate url address, if not set, will use the default url.",
     )
     persist_path: str = Field(
         default=os.getenv("WEAVIATE_PERSIST_PATH", None),
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/annotations.py` & `dbgpt-0.5.5rc0/dbgpt/util/annotations.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/api_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 model_name = "vicuna-7b-v1.5"
 model_path = LLM_MODEL_CONFIG[model_name]
 # or vllm
 model_type = "huggingface"
 
-controller_addr = "http://127.0.0.1:5000"
+controller_addr = "http://127.0.0.1:5670"
 
 result_csv_file = None
 
 parallel_nums = [1, 2, 4, 16, 32]
 # parallel_nums = [1, 2, 4]
 
 
@@ -214,17 +214,17 @@
                 if "torch.cuda.OutOfMemoryError" in msg:
                     return
 
     sys.exit(0)
 
 
 def startup_llm_env():
-    from fastapi import FastAPI
+    from dbgpt.util.fastapi import create_app
 
-    app = FastAPI()
+    app = create_app()
     initialize_worker_manager_in_client(
         app=app,
         model_name=model_name,
         model_path=model_path,
         run_locally=False,
         controller_addr=controller_addr,
         local_port=6000,
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/chat_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/code_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/code_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/command_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/command_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     from dbgpt.util.parameter_utils import EnvArgumentParser
 
     env_to_app = {}
     env_to_app.update(os.environ)
     app_env = EnvArgumentParser._kwargs_to_env_key_value(kwargs)
     env_to_app.update(app_env)
-    cmd = f"uvicorn {app} --host 0.0.0.0 --port 5000"
+    cmd = f"uvicorn {app} --host 0.0.0.0 --port 5670"
     if "windows" in platform.system().lower():
         raise Exception("Not support on windows")
     else:  # macOS, Linux, and other Unix-like systems
         process = subprocess.Popen(cmd, shell=True, env=env_to_app)
     print(f"Started {app} with gunicorn in background with pid: {process.pid}")
 
 
@@ -133,16 +133,16 @@
                 if connections is not None and len(ports) == 0:
                     for connection in connections:
                         if connection.status == psutil.CONN_LISTEN:
                             ports.append(connection.laddr.port)
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
 
-    # Sort ports with preference for 8000 and 5000
-    ports.sort(key=lambda x: (x != 8000, x != 5000, x))
+    # Sort ports with preference for 8000 and 5670
+    ports.sort(key=lambda x: (x != 8000, x != 5670, x))
     return ports
 
 
 @lru_cache()
 def _detect_controller_address() -> str:
     controller_addr = os.getenv("CONTROLLER_ADDRESS")
     if controller_addr:
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/config_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/console/console.py` & `dbgpt-0.5.5rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import inspect
 import logging
 import os
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, Type, TypeVar, cast
 
 import schedule
 import tomlkit
 
-from dbgpt._private.pydantic import BaseModel, Field, root_validator
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_validator
 from dbgpt.component import BaseComponent, SystemApp
 from dbgpt.core.awel.flow.flow_factory import FlowPanel
 from dbgpt.util.dbgpts.base import (
     DBGPTS_METADATA_FILE,
     INSTALL_DIR,
     INSTALL_METADATA_FILE,
 )
 
 logger = logging.getLogger(__name__)
+T = TypeVar("T")
 
 
 class BasePackage(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     name: str = Field(..., description="The name of the package")
     label: str = Field(..., description="The label of the package")
     package_type: str = Field(..., description="The type of the package")
     version: str = Field(..., description="The version of the package")
     description: str = Field(..., description="The description of the package")
     path: str = Field(..., description="The path of the package")
@@ -43,17 +43,20 @@
     repo: str = Field(..., description="The repository of the package")
     package: str = Field(..., description="The package name(like name in pypi)")
 
     @classmethod
     def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
         return cls(**values)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Pre-fill the definition_file"""
+        if not isinstance(values, dict):
+            return values
         import importlib.resources as pkg_resources
 
         name = values.get("name")
         root = values.get("root")
         if not name:
             raise ValueError("The name is required")
         if not root:
@@ -64,17 +67,43 @@
             # Read the file
             values["path"] = os.path.dirname(os.path.abspath(path))
         return values
 
     def abs_definition_file(self) -> str:
         return str(Path(self.path) / self.definition_file)
 
+    @classmethod
+    def load_module_class(
+        cls, values: Dict[str, Any], expected_cls: Type[T]
+    ) -> List[Type[T]]:
+        import importlib.resources as pkg_resources
+
+        from dbgpt.core.awel.dag.loader import _load_modules_from_file
+
+        name = values.get("name")
+        root = values.get("root")
+        if not name:
+            raise ValueError("The name is required")
+        if not root:
+            raise ValueError("The root is required")
+        if root not in sys.path:
+            sys.path.append(root)
+        with pkg_resources.path(name, "__init__.py") as path:
+            mods = _load_modules_from_file(str(path), name, show_log=False)
+            all_cls = [_get_classes_from_module(m) for m in mods]
+            module_cls = []
+            for list_cls in all_cls:
+                for c in list_cls:
+                    if issubclass(c, expected_cls):
+                        module_cls.append(c)
+            return module_cls
+
 
 class FlowPackage(BasePackage):
-    package_type = "flow"
+    package_type: str = "flow"
 
     @classmethod
     def build_from(
         cls, values: Dict[str, Any], ext_dict: Dict[str, Any]
     ) -> "FlowPackage":
         if values["definition_type"] == "json":
             return FlowJsonPackage.build_from(values, ext_dict)
@@ -95,40 +124,40 @@
         import json
 
         with open(self.abs_definition_file(), "r", encoding="utf-8") as f:
             return json.loads(f.read())
 
 
 class OperatorPackage(BasePackage):
-    package_type = "operator"
+    package_type: str = "operator"
 
     operators: List[type] = Field(
         default_factory=list, description="The operators of the package"
     )
 
     @classmethod
     def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
-        import importlib.resources as pkg_resources
-
         from dbgpt.core.awel import BaseOperator
-        from dbgpt.core.awel.dag.loader import _load_modules_from_file
 
-        name = values.get("name")
-        root = values.get("root")
-        if root not in sys.path:
-            sys.path.append(root)
-        with pkg_resources.path(name, "__init__.py") as path:
-            mods = _load_modules_from_file(str(path), name, show_log=False)
-            all_cls = [_get_classes_from_module(m) for m in mods]
-            operators = []
-            for list_cls in all_cls:
-                for c in list_cls:
-                    if issubclass(c, BaseOperator):
-                        operators.append(c)
-            values["operators"] = operators
+        values["operators"] = cls.load_module_class(values, BaseOperator)
+        return cls(**values)
+
+
+class AgentPackage(BasePackage):
+    package_type: str = "agent"
+
+    agents: List[type] = Field(
+        default_factory=list, description="The agents of the package"
+    )
+
+    @classmethod
+    def build_from(cls, values: Dict[str, Any], ext_dict: Dict[str, Any]):
+        from dbgpt.agent import ConversableAgent
+
+        values["agents"] = cls.load_module_class(values, ConversableAgent)
         return cls(**values)
 
 
 class InstalledPackage(BaseModel):
     name: str = Field(..., description="The name of the package")
     repo: str = Field(..., description="The repository of the package")
     root: str = Field(..., description="The root of the package")
@@ -149,28 +178,33 @@
         Path(package.root) / DBGPTS_METADATA_FILE, mode="r+", encoding="utf-8"
     ) as f:
         metadata = tomlkit.loads(f.read())
     ext_metadata = {}
     pkg_dict = {}
     for key, value in metadata.items():
         if key == "flow":
-            pkg_dict = value
+            pkg_dict = {k: v for k, v in value.items()}
             pkg_dict["package_type"] = "flow"
         elif key == "operator":
             pkg_dict = {k: v for k, v in value.items()}
             pkg_dict["package_type"] = "operator"
+        elif key == "agent":
+            pkg_dict = {k: v for k, v in value.items()}
+            pkg_dict["package_type"] = "agent"
         else:
             ext_metadata[key] = value
     pkg_dict["root"] = package.root
     pkg_dict["repo"] = package.repo
     pkg_dict["package"] = package.package
     if pkg_dict["package_type"] == "flow":
         return FlowPackage.build_from(pkg_dict, ext_metadata)
     elif pkg_dict["package_type"] == "operator":
         return OperatorPackage.build_from(pkg_dict, ext_metadata)
+    elif pkg_dict["package_type"] == "agent":
+        return AgentPackage.build_from(pkg_dict, ext_metadata)
     else:
         raise ValueError(
             f"Unsupported package package_type: {pkg_dict['package_type']}"
         )
 
 
 def _load_installed_package(path: str) -> List[InstalledPackage]:
@@ -204,15 +238,15 @@
         parsed_packages.append(_parse_package_metadata(package))
     return parsed_packages
 
 
 class DBGPTsLoader(BaseComponent):
     """The loader of the dbgpts packages"""
 
-    name = "dbgpt_dbgpts_loader"
+    name: str = "dbgpt_dbgpts_loader"
 
     def __init__(
         self,
         system_app: Optional[SystemApp] = None,
         install_dir: Optional[str] = None,
         load_dbgpts_interval: int = 10,
     ):
@@ -239,14 +273,15 @@
             packages = _load_package_from_path(self._install_dir)
             if is_first:
                 logger.info(
                     f"Found {len(packages)} dbgpts packages from {self._install_dir}"
                 )
             for package in packages:
                 self._packages[package.name] = package
+                self._register_packages(package)
         except Exception as e:
             logger.warning(f"Load dbgpts package error: {e}")
 
     def get_flows(self) -> List[FlowPanel]:
         """Get the flows.
 
         Returns:
@@ -264,7 +299,20 @@
                 "editable": False,
                 "description": package.description,
                 "source": package.repo,
                 "flow_data": package.read_definition_json(),
             }
             panels.append(FlowPanel(**dict_value))
         return panels
+
+    def _register_packages(self, package: BasePackage):
+        if package.package_type == "agent":
+            from dbgpt.agent import ConversableAgent, get_agent_manager
+
+            agent_manager = get_agent_manager(self._system_app)
+            pkg = cast(AgentPackage, package)
+            for agent_cls in pkg.agents:
+                if issubclass(agent_cls, ConversableAgent):
+                    try:
+                        agent_manager.register_agent(agent_cls, ignore_duplicate=True)
+                    except ValueError as e:
+                        logger.warning(f"Register agent {agent_cls} error: {e}")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,15 @@
     """Print all repos"""
     repos = _list_repos_details()
     repos.sort(key=lambda x: (x[0], x[1]))
     table = Table(title=_("Repos"))
     table.add_column(_("Repository"), justify="right", style="cyan", no_wrap=True)
     table.add_column(_("Path"), justify="right", style="green")
     for repo, full_path in repos:
-        if full_path.startswith(str(Path.home())):
-            full_path = full_path.replace(str(Path.home()), "~")
+        full_path = _print_path(full_path)
         table.add_row(repo, full_path)
     cl.print(table)
 
 
 def _install_default_repos_if_no_repos():
     """Install the default repos if no repos exist."""
     has_repos = False
@@ -241,15 +240,22 @@
             f"({_print_path(install_path)}).",
             exit_code=1,
         )
     try:
         shutil.copytree(package_path, install_path)
         cl.info(f"Installing dbgpts '{name}' from {repo}...")
         os.chdir(install_path)
-        subprocess.run(["poetry", "install"], check=True)
+        subprocess.run(["poetry", "build"], check=True)
+        wheel_files = list(install_path.glob("dist/*.whl"))
+        if not wheel_files:
+            cl.error("No wheel file found after building the package.", exit_code=1)
+        # Install the wheel file using pip
+        wheel_file = wheel_files[0]
+        cl.info(f"Installing dbgpts '{name}' wheel file {_print_path(wheel_file)}...")
+        subprocess.run(["pip", "install", str(wheel_file)], check=True)
         _write_install_metadata(name, repo, install_path)
         cl.success(f"Installed dbgpts at {_print_path(install_path)}.")
         cl.success(f"dbgpts '{name}' installed successfully.")
     except Exception as e:
         if install_path.exists():
             shutil.rmtree(install_path)
         raise e
@@ -353,11 +359,10 @@
     table.add_column(_("Type"), style="blue")
     table.add_column(_("Repository"), style="magenta")
     table.add_column(_("Path"), justify="right", style="green")
 
     packages.sort(key=lambda x: (x.package, x.package_type, x.repo))
     for package in packages:
         str_path = package.root
-        if str_path.startswith(str(Path.home())):
-            str_path = str_path.replace(str(Path.home()), "~")
+        str_path = _print_path(str_path)
         table.add_row(package.package, package.package_type, package.repo, str_path)
     cl.print(table)
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/error_types.py` & `dbgpt-0.5.5rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/formatting.py` & `dbgpt-0.5.5rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/function_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/function_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/global_helper.py` & `dbgpt-0.5.5rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/json_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/model_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/module_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/net_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/network/_cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,18 +193,20 @@
 
 
 def _start_http_forward(
     local_port, remote_host, remote_port, ssl: bool, timeout, proxies: str | None = None
 ):
     import httpx
     import uvicorn
-    from fastapi import BackgroundTasks, FastAPI, Request, Response
+    from fastapi import BackgroundTasks, Request, Response
     from fastapi.responses import StreamingResponse
 
-    app = FastAPI()
+    from dbgpt.util.fastapi import create_app
+
+    app = create_app()
 
     @app.middleware("http")
     async def forward_http_request(request: Request, call_next):
         """Forward HTTP request to remote host."""
         nonlocal proxies
         req_body = await request.body()
         scheme = request.scope.get("scheme")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Generic, List, TypeVar
 
-from dbgpt._private.pydantic import BaseModel, Field
+from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 
 T = TypeVar("T")
 
 
 class PaginationResult(BaseModel, Generic[T]):
     """Pagination result"""
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     items: List[T] = Field(..., description="The items in the current page")
     total_count: int = Field(..., description="Total number of items")
     total_pages: int = Field(..., description="total number of pages")
     page: int = Field(..., description="Current page number")
     page_size: int = Field(..., description="Number of items per page")
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 import logging
 from string import Formatter
 from typing import Callable, List, Optional, Sequence, Set
 
 from dbgpt._private.llm_metadata import LLMMetadata
-from dbgpt._private.pydantic import BaseModel, Field, PrivateAttr
+from dbgpt._private.pydantic import BaseModel, Field, PrivateAttr, model_validator
 from dbgpt.core.interface.prompt import get_template_vars
 from dbgpt.rag.text_splitter.token_splitter import TokenTextSplitter
 from dbgpt.util.global_helper import globals_helper
 
 DEFAULT_PADDING = 5
 DEFAULT_CHUNK_OVERLAP_RATIO = 0.1
 
@@ -58,44 +58,47 @@
         default=DEFAULT_NUM_OUTPUTS,
         description="The amount of token-space to leave in input for generation.",
     )
     chunk_overlap_ratio: float = Field(
         default=DEFAULT_CHUNK_OVERLAP_RATIO,
         description="The percentage token amount that each chunk should overlap.",
     )
-    chunk_size_limit: Optional[int] = Field(description="The maximum size of a chunk.")
+    chunk_size_limit: Optional[int] = Field(
+        None, description="The maximum size of a chunk."
+    )
     separator: str = Field(
         default=" ", description="The separator when chunking tokens."
     )
 
-    _tokenizer: Callable[[str], List] = PrivateAttr()
+    _tokenizer: Optional[Callable[[str], List]] = PrivateAttr()
 
     def __init__(
         self,
         context_window: int = DEFAULT_CONTEXT_WINDOW,
         num_output: int = DEFAULT_NUM_OUTPUTS,
         chunk_overlap_ratio: float = DEFAULT_CHUNK_OVERLAP_RATIO,
         chunk_size_limit: Optional[int] = None,
         tokenizer: Optional[Callable[[str], List]] = None,
         separator: str = " ",
+        **kwargs,
     ) -> None:
         """Init params."""
         if chunk_overlap_ratio > 1.0 or chunk_overlap_ratio < 0.0:
             raise ValueError("chunk_overlap_ratio must be a float between 0. and 1.")
 
-        # TODO: make configurable
-        self._tokenizer = tokenizer or globals_helper.tokenizer
-
         super().__init__(
             context_window=context_window,
             num_output=num_output,
             chunk_overlap_ratio=chunk_overlap_ratio,
             chunk_size_limit=chunk_size_limit,
             separator=separator,
+            **kwargs,
         )
+        # TODO: make configurable
+        self._tokenizer = tokenizer or globals_helper.tokenizer
 
     def token_count(self, prompt_template: str) -> int:
         """Get token count of prompt template."""
         empty_prompt_txt = get_empty_prompt_txt(prompt_template)
         return len(self._tokenizer(empty_prompt_txt))
 
     @classmethod
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py` & `dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/singleton.py` & `dbgpt-0.5.5rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/speech/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/speech/say.py` & `dbgpt-0.5.5rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/string_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/system_utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/util/utils.py` & `dbgpt-0.5.5rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/vis/__init__.py` & `dbgpt-0.5.5rc0/dbgpt/vis/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """GPT-Vis Module."""
 
-from .client import vis_client  # noqa: F401
 from .base import Vis  # noqa: F401
+from .client import vis_client  # noqa: F401
 from .tags.vis_agent_message import VisAgentMessages  # noqa: F401
 from .tags.vis_agent_plans import VisAgentPlans  # noqa: F401
 from .tags.vis_chart import VisChart  # noqa: F401
 from .tags.vis_code import VisCode  # noqa: F401
 from .tags.vis_dashboard import VisDashboard  # noqa: F401
 from .tags.vis_plugin import VisPlugin  # noqa: F401
```

### Comparing `dbgpt-0.5.4rc0/dbgpt/vis/base.py` & `dbgpt-0.5.5rc0/dbgpt/vis/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/vis/client.py` & `dbgpt-0.5.5rc0/dbgpt/vis/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_chart.py` & `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_dashboard.py` & `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,408 +1,405 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.4rc0
+Version: 0.5.5rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
-Requires-Dist: pydantic<2,>=1
+Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
 Provides-Extra: core
-Requires-Dist: aiohttp==3.8.4; extra == "core"
 Requires-Dist: chardet==5.1.0; extra == "core"
 Requires-Dist: importlib-resources==5.12.0; extra == "core"
-Requires-Dist: python-dotenv==1.0.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
-Requires-Dist: pydantic<2,>=1; extra == "core"
 Requires-Dist: typeguard; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: pydantic>=2.6.0; extra == "core"
 Provides-Extra: client
-Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: httpx; extra == "client"
 Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: cachetools; extra == "client"
-Requires-Dist: pydantic<2,>=1; extra == "client"
 Requires-Dist: typeguard; extra == "client"
-Requires-Dist: httpx; extra == "client"
-Requires-Dist: fastapi==0.98.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: pydantic>=2.6.0; extra == "client"
 Provides-Extra: cli
-Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: click; extra == "cli"
 Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
+Requires-Dist: tomlkit; extra == "cli"
 Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: prettytable; extra == "cli"
 Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: pydantic<2,>=1; extra == "cli"
 Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
-Requires-Dist: fastapi==0.98.0; extra == "cli"
-Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: click; extra == "cli"
+Requires-Dist: rich; extra == "cli"
 Requires-Dist: psutil==5.9.4; extra == "cli"
+Requires-Dist: aiohttp==3.8.4; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: tomlkit; extra == "cli"
-Requires-Dist: rich; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: click; extra == "agent"
 Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
+Requires-Dist: tomlkit; extra == "agent"
+Requires-Dist: termcolor; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: prettytable; extra == "agent"
 Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: pydantic<2,>=1; extra == "agent"
 Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
-Requires-Dist: fastapi==0.98.0; extra == "agent"
-Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: click; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: rich; extra == "agent"
 Requires-Dist: psutil==5.9.4; extra == "agent"
+Requires-Dist: aiohttp==3.8.4; extra == "agent"
 Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: tomlkit; extra == "agent"
-Requires-Dist: rich; extra == "agent"
-Requires-Dist: termcolor; extra == "agent"
-Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: pydantic>=2.6.0; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: click; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: msgpack; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
-Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: pydantic<2,>=1; extra == "simple-framework"
 Requires-Dist: typeguard; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: fastapi==0.98.0; extra == "simple-framework"
-Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: psutil==5.9.4; extra == "simple-framework"
+Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
 Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: jinja2; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Requires-Dist: tomlkit; extra == "simple-framework"
-Requires-Dist: rich; extra == "simple-framework"
+Requires-Dist: cachetools; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
+Requires-Dist: psutil==5.9.4; extra == "simple-framework"
 Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: prettytable; extra == "simple-framework"
+Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
-Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: click; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
+Requires-Dist: msgpack; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
 Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: pydantic<2,>=1; extra == "framework"
 Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: fastapi==0.98.0; extra == "framework"
-Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: click; extra == "framework"
-Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
 Requires-Dist: rich; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
-Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
-Requires-Dist: duckdb; extra == "framework"
 Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: jsonschema; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: jinja2; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: cachetools; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: pydantic>=2.6.0; extra == "framework"
+Requires-Dist: psutil==5.9.4; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: prettytable; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: python-dotenv==1.0.0; extra == "framework"
+Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: duckdb; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
 Provides-Extra: torch
-Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchvision==0.17.1; extra == "torch"
+Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
-Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
+Requires-Dist: torch==2.2.1; extra == "torch-cpu"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cpu"
 Provides-Extra: torch-cuda
-Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchvision==0.17.1; extra == "torch-cuda"
+Requires-Dist: torch==2.2.1; extra == "torch-cuda"
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
 Provides-Extra: vstore
-Requires-Dist: pymilvus; extra == "vstore"
-Requires-Dist: weaviate-client; extra == "vstore"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore"
+Provides-Extra: vstore-weaviate
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
+Requires-Dist: weaviate-client; extra == "vstore-weaviate"
+Provides-Extra: vstore-milvus
+Requires-Dist: pymilvus; extra == "vstore-milvus"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
+Provides-Extra: vstore-all
+Requires-Dist: pymilvus; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
+Requires-Dist: weaviate-client; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
-Requires-Dist: pymysql; extra == "datasource-all"
-Requires-Dist: pyspark; extra == "datasource-all"
 Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: pyspark; extra == "datasource-all"
+Requires-Dist: clickhouse-connect; extra == "datasource-all"
+Requires-Dist: thrift_sasl; extra == "datasource-all"
 Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
-Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
+Requires-Dist: pymysql; extra == "datasource-all"
 Requires-Dist: thrift; extra == "datasource-all"
-Requires-Dist: thrift_sasl; extra == "datasource-all"
+Requires-Dist: psycopg2; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: pymilvus; extra == "rag"
-Requires-Dist: weaviate-client; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: spacy==3.5.3; extra == "rag"
-Requires-Dist: chromadb==0.4.10; extra == "rag"
-Requires-Dist: markdown; extra == "rag"
-Requires-Dist: bs4; extra == "rag"
+Requires-Dist: pypdf; extra == "rag"
 Requires-Dist: python-pptx; extra == "rag"
 Requires-Dist: python-docx; extra == "rag"
-Requires-Dist: pypdf; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: markdown; extra == "rag"
 Requires-Dist: python-multipart; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
+Requires-Dist: langchain>=0.0.286; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
+Requires-Dist: chromadb>=0.4.22; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: openai; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
 Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: pydantic<2,>=1; extra == "openai"
 Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: fastapi==0.98.0; extra == "openai"
-Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: click; extra == "openai"
-Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
 Requires-Dist: rich; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
-Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
-Requires-Dist: duckdb; extra == "openai"
 Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
 Requires-Dist: pymysql; extra == "openai"
-Requires-Dist: jsonschema; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: markdown; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: aiofiles; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: pymilvus; extra == "openai"
-Requires-Dist: weaviate-client; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: spacy==3.5.3; extra == "openai"
-Requires-Dist: chromadb==0.4.10; extra == "openai"
-Requires-Dist: markdown; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: jinja2; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: python-multipart; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: cachetools; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: pydantic>=2.6.0; extra == "openai"
+Requires-Dist: psutil==5.9.4; extra == "openai"
 Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: openai; extra == "openai"
+Requires-Dist: prettytable; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: graphviz; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: python-dotenv==1.0.0; extra == "openai"
+Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: duckdb; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: protobuf==3.20.3; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: click; extra == "default"
+Requires-Dist: fschat; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
 Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: cachetools; extra == "default"
-Requires-Dist: pydantic<2,>=1; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
 Requires-Dist: typeguard; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: fastapi==0.98.0; extra == "default"
-Requires-Dist: prettytable; extra == "default"
-Requires-Dist: click; extra == "default"
-Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
 Requires-Dist: rich; extra == "default"
-Requires-Dist: termcolor; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
-Requires-Dist: jinja2; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: pympler; extra == "default"
-Requires-Dist: duckdb; extra == "default"
 Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
-Requires-Dist: fschat; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
 Requires-Dist: pymysql; extra == "default"
-Requires-Dist: jsonschema; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: markdown; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: pympler; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
 Requires-Dist: aiofiles; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: graphviz; extra == "default"
-Requires-Dist: pymilvus; extra == "default"
-Requires-Dist: weaviate-client; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: spacy==3.5.3; extra == "default"
-Requires-Dist: chromadb==0.4.10; extra == "default"
-Requires-Dist: markdown; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: python-docx; extra == "default"
 Requires-Dist: pypdf; extra == "default"
+Requires-Dist: seaborn; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: jinja2; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
+Requires-Dist: bs4; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
+Requires-Dist: schedule; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: chromadb>=0.4.22; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: cachetools; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
+Requires-Dist: psutil==5.9.4; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
 Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: pymysql; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: prettytable; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: accelerate>=0.20.3; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: graphviz; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: python-dotenv==1.0.0; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: duckdb; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Provides-Extra: all
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: chromadb==0.4.10; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: schedule; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: fschat; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: thrift; extra == "all"
 Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: protobuf==3.20.3; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: chromadb>=0.4.22; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: httpx; extra == "all"
 Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
 Requires-Dist: pympler; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: click; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: fastapi>=0.100.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
 Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: pyspark; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
 Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: spacy==3.5.3; extra == "all"
-Requires-Dist: python-docx; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
 Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: pyhive; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
 Requires-Dist: seaborn; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
 Requires-Dist: vllm; extra == "all"
-Requires-Dist: msgpack; extra == "all"
 Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
 Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
```

### Comparing `dbgpt-0.5.4rc0/dbgpt.egg-info/SOURCES.txt` & `dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -323,14 +323,15 @@
 dbgpt/util/net_utils.py
 dbgpt/util/openai_utils.py
 dbgpt/util/pagination_utils.py
 dbgpt/util/parameter_utils.py
 dbgpt/util/path_utils.py
 dbgpt/util/pd_utils.py
 dbgpt/util/prompt_util.py
+dbgpt/util/retry.py
 dbgpt/util/similarity_util.py
 dbgpt/util/singleton.py
 dbgpt/util/splitter_utils.py
 dbgpt/util/string_utils.py
 dbgpt/util/system_utils.py
 dbgpt/util/utils.py
 dbgpt/util/benchmarks/__init__.py
```

### Comparing `dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,408 +1,412 @@
 aiohttp==3.8.4
 chardet==5.1.0
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
-pydantic<2,>=1
+pydantic>=2.6.0
 typeguard
 
 [agent]
-aiohttp==3.8.4
+click
 chardet==5.1.0
+httpx
+tomlkit
+termcolor
 importlib-resources==5.12.0
-python-dotenv==1.0.0
+fastapi>=0.100.0
+prettytable
 cachetools
-pydantic<2,>=1
 typeguard
-httpx
-fastapi==0.98.0
-prettytable
-click
+pandas==2.0.3
+rich
 psutil==5.9.4
+aiohttp==3.8.4
 colorama==0.4.6
-tomlkit
-rich
-termcolor
-pandas==2.0.3
+python-dotenv==1.0.0
+pydantic>=2.6.0
 
 [all]
-python-multipart
-clickhouse-connect
-pymysql
-GitPython
-markdown
-psycopg2
-pymssql
-chromadb==0.4.10
-torchaudio==2.2.1
-alembic==1.12.0
-schedule
+click
+fschat
 importlib-resources==5.12.0
-duckdb-engine
-prettytable
-dashscope
-jinja2
-uvicorn
-duckdb
+typeguard
+thrift
 SQLAlchemy<2.0.29,>=2.0.25
-python-dotenv==1.0.0
 gpt4all
-chardet
-python-pptx
-llama-cpp-python
-sentencepiece
-protobuf==3.20.3
-colorama==0.4.6
-mysqlclient==2.1.0
-coloredlogs
-fschat
-pypdf
-torchvision==0.17.1
-rocksdict
+pymilvus
+GitPython
+gTTS==2.3.1
+clickhouse-connect
+dashscope
+sentence-transformers
+cpm_kernels
+openai
 sqlparse==0.4.4
-xlrd==2.0.1
+graphviz
+python-dotenv==1.0.0
+duckdb
+shortuuid
+torchaudio==2.2.1
+duckdb-engine
+markdown
+pymysql
+rocksdict
+bitsandbytes
+pypdf
+openpyxl==3.1.2
+bs4
+chromadb>=0.4.22
+pyspark
+chardet==5.1.0
+httpx
 tomlkit
+cachetools
+transformers>=4.34.0
+pymssql
+termcolor
+accelerate>=0.20.3
+aiohttp==3.8.4
+uvicorn
+sentencepiece
+spacy>=3.7
 pympler
-sentence-transformers
-click
+alembic==1.12.0
+chardet
+psycopg2
+fastapi>=0.100.0
+schedule
+python-docx
+pyhive
+pydantic>=2.6.0
+python-pptx
+zhipuai
 pandas==2.0.3
-pyspark
+torchvision==0.17.1
 tiktoken
-aiohttp==3.8.4
-zhipuai
-torch==2.2.1
-transformers>=4.34.0
-pymilvus
+xlrd==2.0.1
+msgpack
+mysqlclient==2.1.0
+rich
+pydoris<2.0.0,>=1.0.2
+colorama==0.4.6
 langchain>=0.0.286
-thrift
-bs4
-openai
-thrift_sasl
-spacy==3.5.3
-python-docx
+torch==2.2.1
+coloredlogs
 aiofiles
-tokenizers>=0.14
-graphviz
-weaviate-client
-accelerate>=0.20.3
-psutil==5.9.4
-httpx
-fastapi==0.98.0
-chardet==5.1.0
-pyhive
+llama-cpp-python
 seaborn
-bitsandbytes
+jinja2
+python-multipart
+tokenizers>=0.14
 vllm
-msgpack
 auto-gpt-plugin-template
-pydantic<2,>=1
-pydoris<2.0.0,>=1.0.2
-rich
-openpyxl==3.1.2
+psutil==5.9.4
+thrift_sasl
+prettytable
+weaviate-client
 jsonschema
-cachetools
-termcolor
-shortuuid
-typeguard
-gTTS==2.3.1
-cpm_kernels
 
 [bitsandbytes]
 bitsandbytes
 
 [cache]
 rocksdict
 
 [cli]
-aiohttp==3.8.4
+click
 chardet==5.1.0
+httpx
+tomlkit
 importlib-resources==5.12.0
-python-dotenv==1.0.0
+fastapi>=0.100.0
+prettytable
 cachetools
-pydantic<2,>=1
 typeguard
-httpx
-fastapi==0.98.0
-prettytable
-click
+rich
 psutil==5.9.4
+aiohttp==3.8.4
 colorama==0.4.6
-tomlkit
-rich
+python-dotenv==1.0.0
+pydantic>=2.6.0
 
 [client]
-aiohttp==3.8.4
 chardet==5.1.0
+httpx
 importlib-resources==5.12.0
-python-dotenv==1.0.0
+fastapi>=0.100.0
 cachetools
-pydantic<2,>=1
 typeguard
-httpx
-fastapi==0.98.0
+aiohttp==3.8.4
+python-dotenv==1.0.0
+pydantic>=2.6.0
 
 [core]
-aiohttp==3.8.4
 chardet==5.1.0
 importlib-resources==5.12.0
-python-dotenv==1.0.0
 cachetools
-pydantic<2,>=1
 typeguard
+aiohttp==3.8.4
+python-dotenv==1.0.0
+pydantic>=2.6.0
 
 [datasource]
 pymysql
 
 [datasource_all]
-pymysql
-pyspark
 pymssql
-psycopg2
+pyspark
+clickhouse-connect
+thrift_sasl
 mysqlclient==2.1.0
 pydoris<2.0.0,>=1.0.2
-clickhouse-connect
 pyhive
+pymysql
 thrift
-thrift_sasl
+psycopg2
 
 [default]
-tokenizers>=0.14
-accelerate>=0.20.3
-protobuf==3.20.3
-zhipuai
-dashscope
-chardet
-sentencepiece
-aiohttp==3.8.4
-chardet==5.1.0
+click
+fschat
+torchaudio==2.2.1
+msgpack
+uvicorn
 importlib-resources==5.12.0
-python-dotenv==1.0.0
-cachetools
-pydantic<2,>=1
+sentencepiece
 typeguard
-httpx
-fastapi==0.98.0
-prettytable
-click
-psutil==5.9.4
-colorama==0.4.6
-tomlkit
 rich
-termcolor
-pandas==2.0.3
-jinja2
-uvicorn
-shortuuid
-SQLAlchemy<2.0.29,>=2.0.25
-msgpack
-pympler
-duckdb
 duckdb-engine
-schedule
-sqlparse==0.4.4
-fschat
-coloredlogs
-seaborn
-auto-gpt-plugin-template
-gTTS==2.3.1
+spacy>=3.7
 pymysql
-jsonschema
-transformers>=4.34.0
+markdown
+colorama==0.4.6
+rocksdict
+langchain>=0.0.286
+pympler
 alembic==1.12.0
-openpyxl==3.1.2
-xlrd==2.0.1
+torch==2.2.1
+chardet
+SQLAlchemy<2.0.29,>=2.0.25
+coloredlogs
 aiofiles
-GitPython
-graphviz
-pymilvus
-weaviate-client
-langchain>=0.0.286
-spacy==3.5.3
-chromadb==0.4.10
-markdown
-bs4
-python-pptx
-python-docx
 pypdf
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
 python-multipart
-sentence-transformers
-torch==2.2.1
-torchvision==0.17.1
-torchaudio==2.2.1
-cpm_kernels
-rocksdict
-
-[framework]
-aiohttp==3.8.4
+bs4
+tokenizers>=0.14
+schedule
+GitPython
+chromadb>=0.4.22
 chardet==5.1.0
-importlib-resources==5.12.0
-python-dotenv==1.0.0
-cachetools
-pydantic<2,>=1
-typeguard
 httpx
-fastapi==0.98.0
-prettytable
-click
-psutil==5.9.4
-colorama==0.4.6
 tomlkit
-rich
+gTTS==2.3.1
+python-docx
+cachetools
+auto-gpt-plugin-template
+dashscope
+pydantic>=2.6.0
+psutil==5.9.4
+transformers>=4.34.0
+sentence-transformers
+zhipuai
+python-pptx
+cpm_kernels
 termcolor
+prettytable
+sqlparse==0.4.4
+accelerate>=0.20.3
 pandas==2.0.3
-jinja2
-uvicorn
+graphviz
+torchvision==0.17.1
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
+xlrd==2.0.1
+duckdb
 shortuuid
-SQLAlchemy<2.0.29,>=2.0.25
+
+[framework]
+click
+fschat
 msgpack
-pympler
-duckdb
+uvicorn
+importlib-resources==5.12.0
+typeguard
+rich
 duckdb-engine
-schedule
-sqlparse==0.4.4
-fschat
-coloredlogs
-seaborn
-auto-gpt-plugin-template
-gTTS==2.3.1
 pymysql
-jsonschema
-transformers>=4.34.0
+colorama==0.4.6
+pympler
 alembic==1.12.0
-openpyxl==3.1.2
-xlrd==2.0.1
+SQLAlchemy<2.0.29,>=2.0.25
+coloredlogs
 aiofiles
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
 GitPython
+schedule
+chardet==5.1.0
+httpx
+tomlkit
+gTTS==2.3.1
+cachetools
+auto-gpt-plugin-template
+transformers>=4.34.0
+pydantic>=2.6.0
+psutil==5.9.4
+termcolor
+prettytable
+sqlparse==0.4.4
+pandas==2.0.3
 graphviz
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
+xlrd==2.0.1
+duckdb
+shortuuid
 
 [gpt4all]
 gpt4all
 
 [llama_cpp]
 llama-cpp-python
 
 [openai]
-tiktoken
-openai
-aiohttp==3.8.4
-chardet==5.1.0
+click
+fschat
+msgpack
+uvicorn
 importlib-resources==5.12.0
-python-dotenv==1.0.0
-cachetools
-pydantic<2,>=1
 typeguard
-httpx
-fastapi==0.98.0
-prettytable
-click
-psutil==5.9.4
-colorama==0.4.6
-tomlkit
 rich
-termcolor
-pandas==2.0.3
-jinja2
-uvicorn
-shortuuid
-SQLAlchemy<2.0.29,>=2.0.25
-msgpack
-pympler
-duckdb
 duckdb-engine
-schedule
-sqlparse==0.4.4
-fschat
-coloredlogs
-seaborn
-auto-gpt-plugin-template
-gTTS==2.3.1
+spacy>=3.7
 pymysql
-jsonschema
-transformers>=4.34.0
+markdown
+colorama==0.4.6
+langchain>=0.0.286
+pympler
 alembic==1.12.0
-openpyxl==3.1.2
-xlrd==2.0.1
+SQLAlchemy<2.0.29,>=2.0.25
+coloredlogs
 aiofiles
-GitPython
-graphviz
-pymilvus
-weaviate-client
-langchain>=0.0.286
-spacy==3.5.3
-chromadb==0.4.10
-markdown
-bs4
-python-pptx
-python-docx
 pypdf
+seaborn
+openpyxl==3.1.2
+jinja2
+fastapi>=0.100.0
 python-multipart
+bs4
+GitPython
+schedule
+chromadb>=0.4.22
+chardet==5.1.0
+httpx
+tomlkit
+gTTS==2.3.1
+python-docx
+cachetools
+auto-gpt-plugin-template
+transformers>=4.34.0
+pydantic>=2.6.0
+psutil==5.9.4
 sentence-transformers
+python-pptx
+termcolor
+openai
+prettytable
+sqlparse==0.4.4
+pandas==2.0.3
+graphviz
+tiktoken
+aiohttp==3.8.4
+jsonschema
+python-dotenv==1.0.0
+xlrd==2.0.1
+duckdb
+shortuuid
 
 [quantization]
 cpm_kernels
 
 [rag]
-pymilvus
-weaviate-client
-langchain>=0.0.286
-spacy==3.5.3
-chromadb==0.4.10
-markdown
-bs4
+pypdf
 python-pptx
 python-docx
-pypdf
+spacy>=3.7
+markdown
 python-multipart
 sentence-transformers
+langchain>=0.0.286
+bs4
+chromadb>=0.4.22
 
 [simple_framework]
-aiohttp==3.8.4
-chardet==5.1.0
+click
+fschat
+msgpack
+uvicorn
 importlib-resources==5.12.0
-python-dotenv==1.0.0
-cachetools
-pydantic<2,>=1
 typeguard
-httpx
-fastapi==0.98.0
-prettytable
-click
-psutil==5.9.4
+rich
+duckdb-engine
 colorama==0.4.6
+pympler
+SQLAlchemy<2.0.29,>=2.0.25
+jinja2
+fastapi>=0.100.0
+schedule
+chardet==5.1.0
+httpx
 tomlkit
-rich
+cachetools
+pydantic>=2.6.0
+psutil==5.9.4
 termcolor
+prettytable
+sqlparse==0.4.4
 pandas==2.0.3
-jinja2
-uvicorn
-shortuuid
-SQLAlchemy<2.0.29,>=2.0.25
-msgpack
-pympler
+aiohttp==3.8.4
+python-dotenv==1.0.0
 duckdb
-duckdb-engine
-schedule
-sqlparse==0.4.4
-fschat
+shortuuid
 
 [torch]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [torch_cpu]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [torch_cuda]
-torch==2.2.1
 torchvision==0.17.1
+torch==2.2.1
 torchaudio==2.2.1
 
 [vllm]
 vllm
 
 [vstore]
+chromadb>=0.4.22
+
+[vstore_all]
 pymilvus
+chromadb>=0.4.22
+weaviate-client
+
+[vstore_milvus]
+pymilvus
+chromadb>=0.4.22
+
+[vstore_weaviate]
+chromadb>=0.4.22
 weaviate-client
```

### Comparing `dbgpt-0.5.4rc0/setup.py` & `dbgpt-0.5.5rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,21 @@
 
 
 class SetupSpec:
     def __init__(self) -> None:
         self.extras: dict = {}
         self.install_requires: List[str] = []
 
+    @property
+    def unique_extras(self) -> dict[str, list[str]]:
+        unique_extras = {}
+        for k, v in self.extras.items():
+            unique_extras[k] = list(set(v))
+        return unique_extras
+
 
 setup_spec = SetupSpec()
 
 
 class AVXType(Enum):
     BASIC = "basic"
     AVX = "AVX"
@@ -401,22 +408,22 @@
     """
     setup_spec.extras["core"] = [
         "aiohttp==3.8.4",
         "chardet==5.1.0",
         "importlib-resources==5.12.0",
         "python-dotenv==1.0.0",
         "cachetools",
-        "pydantic<2,>=1",
+        "pydantic>=2.6.0",
         # For AWEL type checking
         "typeguard",
     ]
     # For DB-GPT python client SDK
     setup_spec.extras["client"] = setup_spec.extras["core"] + [
         "httpx",
-        "fastapi==0.98.0",
+        "fastapi>=0.100.0",
     ]
     # Simple command line dependencies
     setup_spec.extras["cli"] = setup_spec.extras["client"] + [
         "prettytable",
         "click",
         "psutil==5.9.4",
         "colorama==0.4.6",
@@ -486,16 +493,15 @@
 
 def knowledge_requires():
     """
     pip install "dbgpt[rag]"
     """
     setup_spec.extras["rag"] = setup_spec.extras["vstore"] + [
         "langchain>=0.0.286",
-        "spacy==3.5.3",
-        "chromadb==0.4.10",
+        "spacy>=3.7",
         "markdown",
         "bs4",
         "python-pptx",
         "python-docx",
         "pypdf",
         "python-multipart",
         "sentence-transformers",
@@ -550,17 +556,31 @@
 
 
 def all_vector_store_requires():
     """
     pip install "dbgpt[vstore]"
     """
     setup_spec.extras["vstore"] = [
-        "pymilvus",
+        "chromadb>=0.4.22",
+    ]
+    setup_spec.extras["vstore_weaviate"] = setup_spec.extras["vstore"] + [
+        # "protobuf",
+        # "grpcio",
+        # weaviate depends on grpc which version is very low, we should install it
+        # manually.
         "weaviate-client",
     ]
+    setup_spec.extras["vstore_milvus"] = setup_spec.extras["vstore"] + [
+        "pymilvus",
+    ]
+    setup_spec.extras["vstore_all"] = (
+        setup_spec.extras["vstore"]
+        + setup_spec.extras["vstore_weaviate"]
+        + setup_spec.extras["vstore_milvus"]
+    )
 
 
 def all_datasource_requires():
     """
     pip install "dbgpt[datasource]"
     """
     setup_spec.extras["datasource"] = [
@@ -626,15 +646,14 @@
     """
     pip install "dbgpt[default]"
     """
     setup_spec.extras["default"] = [
         # "tokenizers==0.13.3",
         "tokenizers>=0.14",
         "accelerate>=0.20.3",
-        "protobuf==3.20.3",
         "zhipuai",
         "dashscope",
         "chardet",
         "sentencepiece",
     ]
     setup_spec.extras["default"] += setup_spec.extras["framework"]
     setup_spec.extras["default"] += setup_spec.extras["rag"]
@@ -730,14 +749,14 @@
     "and your data is 100% private and secure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=setup_spec.install_requires,
     url="https://github.com/eosphoros-ai/DB-GPT",
     license="https://opensource.org/license/mit/",
     python_requires=">=3.10",
-    extras_require=setup_spec.extras,
+    extras_require=setup_spec.unique_extras,
     entry_points={
         "console_scripts": [
             "dbgpt=dbgpt.cli.cli_scripts:main",
         ],
     },
 )
```

