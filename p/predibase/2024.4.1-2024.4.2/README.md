# Comparing `tmp/predibase-2024.4.1.tar.gz` & `tmp/predibase-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-2024.4.1.tar", last modified: Thu Apr 18 20:03:44 2024, max compression
+gzip compressed data, was "predibase-2024.4.2.tar", last modified: Thu Apr 18 20:31:15 2024, max compression
```

## Comparing `predibase-2024.4.1.tar` & `predibase-2024.4.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.949184 predibase-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 20:01:45.000000 predibase-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 20:03:44.949184 predibase-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 20:01:45.000000 predibase-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.917184 predibase-2024.4.1/predibase/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.925184 predibase-2024.4.1/predibase/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/list_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/connection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/deployment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/engine_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/llm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/permission_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.929184 predibase-2024.4.1/predibase/pql/
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/pql/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    34402 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/pql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/pql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/query_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.933184 predibase-2024.4.1/predibase/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/connection_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.937184 predibase-2024.4.1/predibase/resource/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.937184 predibase-2024.4.1/predibase/resource/llm/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/templates/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/templates/lora_bf16.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/templates/qlora_4bit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/llm/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    50487 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resource_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.941184 predibase-2024.4.1/predibase/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/resources/repos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/triton_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.945184 predibase-2024.4.1/predibase/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.921184 predibase-2024.4.1/predibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 20:03:44.000000 predibase-2024.4.1/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.945184 predibase-2024.4.1/predibase_notebook/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:03:44.949184 predibase-2024.4.1/predibase_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:01:45.000000 predibase-2024.4.1/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 20:03:44.000000 predibase-2024.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:03:44.949184 predibase-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-18 20:01:45.000000 predibase-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.750134 predibase-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 20:29:15.000000 predibase-2024.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 20:31:15.750134 predibase-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 20:29:15.000000 predibase-2024.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.726134 predibase-2024.4.2/predibase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.730134 predibase-2024.4.2/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/list_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.734134 predibase-2024.4.2/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34402 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.738134 predibase-2024.4.2/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.742133 predibase-2024.4.2/predibase/resource/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.742133 predibase-2024.4.2/predibase/resource/llm/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/templates/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/templates/lora_bf16.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/templates/qlora_4bit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/llm/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50487 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resource_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.746133 predibase-2024.4.2/predibase/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/completions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/resources/repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/triton_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.746133 predibase-2024.4.2/predibase/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.730134 predibase-2024.4.2/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 20:31:15.000000 predibase-2024.4.2/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.750134 predibase-2024.4.2/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:15.750134 predibase-2024.4.2/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:29:15.000000 predibase-2024.4.2/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-18 20:31:15.000000 predibase-2024.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:31:15.750134 predibase-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-18 20:29:15.000000 predibase-2024.4.2/setup.py
```

### Comparing `predibase-2024.4.1/predibase/__init__.py` & `predibase-2024.4.2/predibase/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/_client.py` & `predibase-2024.4.2/predibase/_client.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/_errors.py` & `predibase-2024.4.2/predibase/_errors.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli.py` & `predibase-2024.4.2/predibase/cli.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/create.py` & `predibase-2024.4.2/predibase/cli_commands/create.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/delete.py` & `predibase-2024.4.2/predibase/cli_commands/delete.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/deploy.py` & `predibase-2024.4.2/predibase/cli_commands/deploy.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/download.py` & `predibase-2024.4.2/predibase/cli_commands/download.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/finetune.py` & `predibase-2024.4.2/predibase/cli_commands/finetune.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/list_resources.py` & `predibase-2024.4.2/predibase/cli_commands/list_resources.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/prompt.py` & `predibase-2024.4.2/predibase/cli_commands/prompt.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/settings.py` & `predibase-2024.4.2/predibase/cli_commands/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/upload.py` & `predibase-2024.4.2/predibase/cli_commands/upload.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/cli_commands/utils.py` & `predibase-2024.4.2/predibase/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/client.py` & `predibase-2024.4.2/predibase/client.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/connection.py` & `predibase-2024.4.2/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/connection_mixin.py` & `predibase-2024.4.2/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/dataset_mixin.py` & `predibase-2024.4.2/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/deployment_mixin.py` & `predibase-2024.4.2/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/engine_mixin.py` & `predibase-2024.4.2/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/llm_mixin.py` & `predibase-2024.4.2/predibase/llm_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/model_mixin.py` & `predibase-2024.4.2/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/permission_mixin.py` & `predibase-2024.4.2/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/pql/__init__.py` & `predibase-2024.4.2/predibase/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/pql/adapter.py` & `predibase-2024.4.2/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/pql/api.py` & `predibase-2024.4.2/predibase/pql/api.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/pql/utils.py` & `predibase-2024.4.2/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/predictor.py` & `predibase-2024.4.2/predibase/predictor.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/query_mixin.py` & `predibase-2024.4.2/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/config.py` & `predibase-2024.4.2/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/connection.py` & `predibase-2024.4.2/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/connection_object.py` & `predibase-2024.4.2/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/connection_properties.py` & `predibase-2024.4.2/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/dataset.py` & `predibase-2024.4.2/predibase/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/dataset_info.py` & `predibase-2024.4.2/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/deployment.py` & `predibase-2024.4.2/predibase/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/engine.py` & `predibase-2024.4.2/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/interface.py` & `predibase-2024.4.2/predibase/resource/llm/interface.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/response.py` & `predibase-2024.4.2/predibase/resource/llm/response.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/template.py` & `predibase-2024.4.2/predibase/resource/llm/template.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/templates/lora_bf16.yaml` & `predibase-2024.4.2/predibase/resource/llm/templates/lora_bf16.yaml`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/templates/qlora_4bit.yaml` & `predibase-2024.4.2/predibase/resource/llm/templates/qlora_4bit.yaml`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/llm/util.py` & `predibase-2024.4.2/predibase/resource/llm/util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/model.py` & `predibase-2024.4.2/predibase/resource/model.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/query.py` & `predibase-2024.4.2/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource/user.py` & `predibase-2024.4.2/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resource_util.py` & `predibase-2024.4.2/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/adapters.py` & `predibase-2024.4.2/predibase/resources/adapters.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/completions.py` & `predibase-2024.4.2/predibase/resources/completions.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/datasets.py` & `predibase-2024.4.2/predibase/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/deployment.py` & `predibase-2024.4.2/predibase/resources/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/deployments.py` & `predibase-2024.4.2/predibase/resources/deployments.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/model.py` & `predibase-2024.4.2/predibase/resources/model.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/resources/repos.py` & `predibase-2024.4.2/predibase/resources/repos.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/triton_util.py` & `predibase-2024.4.2/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/util/__init__.py` & `predibase-2024.4.2/predibase/util/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/util/json.py` & `predibase-2024.4.2/predibase/util/json.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/util/metrics.py` & `predibase-2024.4.2/predibase/util/metrics.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/util/settings.py` & `predibase-2024.4.2/predibase/util/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase/util/tensorboard.py` & `predibase-2024.4.2/predibase/util/tensorboard.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase.egg-info/SOURCES.txt` & `predibase-2024.4.2/predibase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase_notebook/__init__.py` & `predibase-2024.4.2/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/predibase_notebook/env.py` & `predibase-2024.4.2/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.1/setup.py` & `predibase-2024.4.2/setup.py`

 * *Files identical despite different names*

