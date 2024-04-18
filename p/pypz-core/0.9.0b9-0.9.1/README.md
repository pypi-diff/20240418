# Comparing `tmp/pypz-core-0.9.0b9.tar.gz` & `tmp/pypz_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypz-core-0.9.0b9.tar", last modified: Tue Feb 13 09:32:31 2024, max compression
+gzip compressed data, was "pypz_core-0.9.1.tar", last modified: Thu Apr 18 05:48:27 2024, max compression
```

## Comparing `pypz-core-0.9.0b9.tar` & `pypz_core-0.9.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.478429 pypz-core-0.9.0b9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-13 09:32:31.478429 pypz-core-0.9.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:32:31.478429 pypz-core-0.9.0b9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.458429 pypz-core-0.9.0b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.458429 pypz-core-0.9.0b9/src/pypz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.462429 pypz-core-0.9.0b9/src/pypz/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21924 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/abstracts/channel_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/abstracts/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.462429 pypz-core-0.9.0b9/src/pypz/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.466429 pypz-core-0.9.0b9/src/pypz/core/channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30689 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18476 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/channels/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/channels/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/channels/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.466429 pypz-core-0.9.0b9/src/pypz/core/commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/commons/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/commons/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.470430 pypz-core-0.9.0b9/src/pypz/core/specs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18189 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)    32973 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/core/specs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.470430 pypz-core-0.9.0b9/src/pypz/deployers/
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/deployers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz/executors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz/executors/operator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/operator/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/operator/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/operator/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    26759 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/operator/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz/executors/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/executors/pipeline/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.458429 pypz-core-0.9.0b9/src/pypz/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz/plugins/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/plugins/loggers/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz/runnables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/runnables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/runnables/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-13 09:32:14.000000 pypz-core-0.9.0b9/src/pypz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:31.474429 pypz-core-0.9.0b9/src/pypz_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-13 09:32:31.000000 pypz-core-0.9.0b9/src/pypz_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-13 09:32:31.000000 pypz-core-0.9.0b9/src/pypz_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:32:31.000000 pypz-core-0.9.0b9/src/pypz_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-13 09:32:31.000000 pypz-core-0.9.0b9/src/pypz_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 09:32:31.000000 pypz-core-0.9.0b9/src/pypz_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.835513 pypz_core-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:48:23.000000 pypz_core-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 05:48:27.835513 pypz_core-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 05:48:23.000000 pypz_core-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-18 05:48:23.000000 pypz_core-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:48:27.835513 pypz_core-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/pypz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/pypz/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21924 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/abstracts/channel_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/abstracts/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/pypz/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/pypz/core/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/channels/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/channels/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/channels/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.827513 pypz_core-0.9.1/src/pypz/core/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/commons/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/commons/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/core/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18196 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/core/specs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/deployers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/deployers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/executors/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/operator/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/operator/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/operator/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26792 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/operator/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/executors/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/executors/pipeline/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.823513 pypz_core-0.9.1/src/pypz/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/plugins/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/plugins/loggers/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz/runnables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/runnables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/runnables/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 05:48:23.000000 pypz_core-0.9.1/src/pypz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:27.831513 pypz_core-0.9.1/src/pypz_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 05:48:27.000000 pypz_core-0.9.1/src/pypz_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 05:48:27.000000 pypz_core-0.9.1/src/pypz_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:48:27.000000 pypz_core-0.9.1/src/pypz_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 05:48:27.000000 pypz_core-0.9.1/src/pypz_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 05:48:27.000000 pypz_core-0.9.1/src/pypz_core.egg-info/top_level.txt
```

### Comparing `pypz-core-0.9.0b9/LICENSE` & `pypz_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/PKG-INFO` & `pypz_core-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pypz-core
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: Core components of pypz (pipes), which is a lightweight Pipeline as Code (PaC) framework.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,pypz-core
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: static
-Requires-Dist: flake8; extra == "static"
+Requires-Dist: flake8~=7.0.0; extra == "static"
 Requires-Dist: flake8-html~=0.4.3; extra == "static"
-Requires-Dist: mypy; extra == "static"
-Requires-Dist: coverage; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains all the necessary core components to realize the
 functionalities of *pypz*.
 
 Check the [documentation](https://lazlowa.github.io/pypz-python/index.html) for
```

### Comparing `pypz-core-0.9.0b9/README.md` & `pypz_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/pyproject.toml` & `pypz_core-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 keywords = [
     "pypz",
     "pypz-core"
 ]
 
 [project.optional-dependencies]
 static = [
-    "flake8",
+    "flake8 ~= 7.0.0",
     "flake8-html ~= 0.4.3",
-    "mypy",
-    "coverage"
+    "mypy ~= 1.8.0",
+    "coverage ~= 7.4.1"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "pypz.version.PROJECT_VERSION"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `pypz-core-0.9.0b9/src/pypz/abstracts/channel_ports.py` & `pypz_core-0.9.1/src/pypz/abstracts/channel_ports.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/abstracts/misc.py` & `pypz_core-0.9.1/src/pypz/abstracts/misc.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/channels/base.py` & `pypz_core-0.9.1/src/pypz/core/channels/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import logging
 import threading
 import time
 import traceback
-from typing import Callable, Any, TYPE_CHECKING
+from typing import Callable, Any, TYPE_CHECKING, Optional
 from abc import ABC, abstractmethod
 import concurrent.futures
 import json
 
 from pypz.core.channels.status import ChannelStatusMonitor, ChannelFilter, ChannelStatusMessage, ChannelStatus, \
     NameSeparator
 from pypz.core.commons.loggers import ContextLogger
@@ -65,15 +65,15 @@
     ParamKeyLogLevel = "logLevel"
     ParamKeyMetricsEnabled = "metricsEnabled"
 
     # ======================= Ctor =======================
 
     def __init__(self, channel_name: str,
                  context: 'PortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
 
         if channel_name is None:
             raise ValueError("Channel name must be provided")
 
         if context is None:
             raise ValueError("Context instance must be provided")
@@ -157,15 +157,15 @@
         """
 
         self._status_map: dict[str, ChannelStatusMonitor] = dict()
         """
         This map stores the health statuses of all connected channels
         """
 
-        self._executor: concurrent.futures.ThreadPoolExecutor = executor
+        self._executor: Optional[concurrent.futures.ThreadPoolExecutor] = executor
         """
         This executor is used to execute the background thread, which will invoke the sendHealthStatus method
         """
 
         self._control_loop_exception_timer: int = 0
         """
         Control loop is, where the control information are sent to the counter channel. Should
@@ -331,26 +331,29 @@
         the output.
 
         :return: number of tracked input channels
         """
 
         return len(self._status_map)
 
-    def retrieve_connected_channel_unique_names(self, filter_function: Callable[[ChannelFilter], bool] = None) -> set:
+    def retrieve_connected_channel_unique_names(
+            self,
+            filter_function: Optional[Callable[[ChannelFilter], bool]] = None
+    ) -> set:
         """
         This method returns a set of connected channel names given the evaluation
         criteria passed as argument.
 
         :param filter_function: check_function check the ChannelFilter for more details (nullable)
         :return: Set of channel names that passes the given evaluation
         """
 
         connected_channel_names = set()
 
-        for key, val in self._status_map.items():
+        for key, val in self._status_map.copy().items():
             if filter_function is not None:
                 if filter_function(val):
                     connected_channel_names.add(key)
             else:
                 connected_channel_names.add(key)
 
         return connected_channel_names
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/channels/io.py` & `pypz_core-0.9.1/src/pypz/core/channels/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import concurrent.futures
-from typing import Any, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING, Optional
 from abc import abstractmethod
 import threading
 
 from pypz.core.channels.base import ChannelBase, ChannelMetric
 from pypz.core.channels.status import ChannelStatus
 from pypz.core.commons.utils import current_time_millis
 
@@ -50,15 +50,15 @@
     This variable specifies the length of the metric buffer and so the averaging window
     """
 
     # ======================= Ctor =======================
 
     def __init__(self, channel_name: str,
                  context: 'InputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
         self._read_record_count: int = 0
         """
         Counter for how many records have been read by this channel. Note that this value can differ from the
         offset value in case of crash-restart. Still the framework maintains the difference between this value
@@ -298,15 +298,15 @@
     This variable specifies the length of the metric buffer and so the averaging window
     """
 
     # ======================= Ctor =======================
 
     def __init__(self, channel_name: str,
                  context: 'OutputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
         self._written_record_count: int = 0
         """
         Number of outputted records.
         """
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/channels/misc.py` & `pypz_core-0.9.1/src/pypz/core/channels/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import concurrent.futures
-from typing import Any, TYPE_CHECKING
+from typing import Any, TYPE_CHECKING, Optional
 
 from pypz.core.channels.io import ChannelReader, ChannelWriter
 
 if TYPE_CHECKING:
     from pypz.core.specs.plugin import InputPortPlugin, OutputPortPlugin
 
 
 class BlankChannelReader(ChannelReader):
     def __init__(self, channel_name: str,
                  context: 'InputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
     def _load_input_record_offset(self) -> int:
         return 0
 
     def has_records(self) -> bool:
@@ -63,15 +63,15 @@
         return []
 
 
 class BlankChannelWriter(ChannelWriter):
 
     def __init__(self, channel_name: str,
                  context: 'OutputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
     def _write_records(self, records: list[Any]) -> None:
         pass
 
     def _create_resources(self) -> bool:
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/channels/status.py` & `pypz_core-0.9.1/src/pypz/core/channels/status.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/commons/loggers.py` & `pypz_core-0.9.1/src/pypz/core/commons/loggers.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/commons/parameters.py` & `pypz_core-0.9.1/src/pypz/core/commons/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,27 @@
     """
 
     def __init__(self,
                  required: bool,
                  parameter_type: Type[ParameterType],
                  alt_name: Optional[str] = None,
                  description: Optional[str] = None,
-                 on_update: Callable[[Any], None] = None):
+                 on_update: Callable[[Any, Any], None] = None):
 
         if parameter_type is None:
             raise TypeError("Parameter type must be specified")
 
         if "typing" == parameter_type.__module__:
             raise TypeError(f"Type description not allowed: {parameter_type}")
 
         self.parameter_type: Type[ParameterType] = parameter_type \
-            if not isinstance(parameter_type, GenericAlias) else parameter_type.__origin__
+            if not isinstance(parameter_type, GenericAlias) else parameter_type.__origin__  # type: ignore
 
         self.generic_types: list[type] = None \
-            if not isinstance(parameter_type, GenericAlias) else parameter_type.__args__
+            if not isinstance(parameter_type, GenericAlias) else parameter_type.__args__  # type: ignore
 
         if not issubclass(self.parameter_type, allowed_param_types):
             raise TypeError(f"Invalid parameter type: {self.parameter_type}. Allowed types are: {allowed_param_types}")
 
         self.required: bool = required
 
         self.name: Optional[str] = alt_name
@@ -184,15 +184,15 @@
             (self.description == other.description) and \
             (self.generic_types == other.generic_types)
 
     def to_dict(self, instance=None) -> dict:
         return {
             self.name: {
                 'type': None if self.parameter_type is None else
-                self.parameter_type.__origin__ if isinstance(self.parameter_type, GenericAlias)
+                self.parameter_type.__origin__ if isinstance(self.parameter_type, GenericAlias)  # type: ignore
                 else self.parameter_type.__name__,
                 'required': self.required,
                 'description': self.description,
                 'currentValue': None if instance is None else self.__get__(instance, None)
             }
         }
 
@@ -216,15 +216,15 @@
     :param on_update: callback to react on value update
     """
 
     def __init__(self,
                  parameter_type: Type[ParameterType] = None,
                  alt_name: str = None,
                  description: Optional[str] = None,
-                 on_update: Callable[[Any], None] = None):
+                 on_update: Callable[[Any, Any], None] = None):
         super().__init__(True, parameter_type, alt_name, description, on_update)
 
 
 class OptionalParameter(ExpectedParameter[ParameterType]):
     """
     Convenience class to represent an optional parameter
     Usage:
@@ -243,15 +243,15 @@
     :param on_update: callback to react on value update
     """
 
     def __init__(self,
                  parameter_type: Type[ParameterType] = None,
                  alt_name: str = None,
                  description: Optional[str] = None,
-                 on_update: Callable[[Any], None] = None):
+                 on_update: Callable[[Any, Any], None] = None):
         super().__init__(False, parameter_type, alt_name, description, on_update)
 
 
 def retrieve_parameters(input_val, parameter_type: Type[ExpectedParameter]) -> dict[str, ExpectedParameter]:
     """
     This method attempts to retrieve all described parameters with
     either public or protected scope. Private scoped parameters are
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/commons/utils.py` & `pypz_core-0.9.1/src/pypz/core/commons/utils.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/dtos.py` & `pypz_core-0.9.1/src/pypz/core/specs/dtos.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
-from typing import Optional, Type, TypeVar
+from typing import Optional, Type, TypeVar, Union
 
 NestedInstanceDTOType = TypeVar("NestedInstanceDTOType", bound='InstanceDTO')
 
 
 class SpecDTO:
     """
     This class represents the base Data Transfer Object for an instance spec.
@@ -42,27 +42,27 @@
     def __init__(self,
                  name: str = None,
                  location: str = None,
                  expectedParameters: dict = None,
                  types: list = None,
                  nestedInstanceType: str = None,
                  nestedInstances: list[NestedInstanceDTOType] = None,
-                 nested_instance_dto_type: Optional[Type[NestedInstanceDTOType]] = 'default'):
+                 nested_instance_dto_type: Optional[Union[Type[NestedInstanceDTOType], str]] = 'default'):
         self.name: str = name
         self.location: str = location
         self.expectedParameters: dict = expectedParameters
         self.types: list = types
         self.nestedInstanceType: str = nestedInstanceType
-        self.nestedInstances: Optional[set[NestedInstanceDTOType]] = None
+        self.nestedInstances: Optional[list[NestedInstanceDTOType]] = None
 
         if nested_instance_dto_type == 'default':
-            nested_instance_dto_type = InstanceDTO
+            nested_instance_dto_type = InstanceDTO  # type: ignore
 
         if (nestedInstances is not None) and (nested_instance_dto_type is not None):
-            self.nestedInstances: list[NestedInstanceDTOType] = list()
+            self.nestedInstances = list()
             if isinstance(nestedInstances, (set, list)):
                 for nestedInstance in nestedInstances:
                     if isinstance(nestedInstance, InstanceDTO):
                         self.nestedInstances.append(nestedInstance)
                     elif isinstance(nestedInstance, dict):
                         self.nestedInstances.append(nested_instance_dto_type(**nestedInstance))
                     else:
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/instance.py` & `pypz_core-0.9.1/src/pypz/core/specs/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import inspect
 import re
 import sys
 import types
+import typing
 from abc import ABCMeta, ABC, abstractmethod
 from typing import Type, Any, TypeVar, Generic, Optional
 
 import yaml
 
 from pypz.core.commons.utils import TemplateResolver, is_type_allowed, convert_to_dict
 from pypz.core.commons.parameters import retrieve_parameters, ExpectedParameter, allowed_param_types
@@ -71,14 +72,15 @@
 class InstanceInitInterceptor(ABCMeta):
     """
     This metaclass has the responsibility to intercept the instance initialization and so
     ensure that instance name and context objects are resolved automatically, before
     executing the __init__ of the instance. For more information refer to InterceptedInstance.
     """
 
+    @typing.no_type_check
     def __call__(cls: Type[InterceptedInstanceType], name: str = None, *args, **kwargs) -> InterceptedInstanceType:
         """
         This method is called, if a class object is being created, hence we can intercept
         the __init__ call. The following rules are considered for interception:
         - caller frame shall be an object and shall be an instance of Instance
         - name or context object is not provided
         In these cases is the Instance init intercepted, in any other cases a normal
@@ -133,15 +135,15 @@
         if nested_instance_type is not None and not issubclass(nested_instance_type, Instance):
             raise TypeError(f"Invalid nested instance type: {nested_instance_type}. "
                             f"Must be an extension of {Instance}")
 
         # Member declarations
         # ===================
 
-        self.__nested_instance_type: Type[NestedInstanceType] | None = nested_instance_type
+        self.__nested_instance_type: Optional[Type[NestedInstanceType]] = nested_instance_type
         """
         Stores the specified type of the nested instances. This is required to
         be able to discover those instances
         """
 
         self.__reference = kwargs["reference"] if "reference" in kwargs else None
         """
@@ -605,17 +607,18 @@
         if instance_dto.spec.location is not None:
             # TODO - remote retrieval shall be implemented here
             raise NotImplementedError("Location based retrieval not yet implemented")
 
         mock_nonexistent = ("mock_nonexistent" in kwargs) and (kwargs["mock_nonexistent"])
 
         try:
-            instance = load_class_by_name(instance_dto.spec.name.replace(":", "."))(instance_dto.name,
-                                                                                    from_dto=instance_dto,
-                                                                                    *args, **kwargs)
+            instance: Instance = \
+                load_class_by_name(instance_dto.spec.name.replace(":", "."))(instance_dto.name,
+                                                                             from_dto=instance_dto,
+                                                                             *args, **kwargs)
         except (ModuleNotFoundError, AttributeError) as e:
             if mock_nonexistent:
                 if (instance_dto.spec.types is None) or (0 == len(instance_dto.spec.types)):
                     raise AttributeError("Missing type specification: instance.spec.types: List[Str]")
 
                 base_classes = set()
                 abstract_methods = set()
@@ -628,32 +631,31 @@
                     base_classes.add(loaded_class)
                     abstract_methods.update(loaded_class.__abstractmethods__)
 
                 nested_instance_type = None if instance_dto.spec.nestedInstanceType is None \
                     else load_class_by_name(instance_dto.spec.nestedInstanceType)
 
                 # Creating dummy implementation of abstract methods
-                class_body = {abstract_method: lambda: None for abstract_method in abstract_methods}
+                class_body: dict[str, Any] = {abstract_method: lambda: None for abstract_method in abstract_methods}
 
                 module_and_name = instance_dto.spec.name.split(":")
                 class_body["__module__"] = module_and_name[0]
                 class_body["mocked"] = True
 
                 # Create new type with name and bases
                 instance_type = types.new_class(module_and_name[1],
                                                 tuple(remove_super_classes(base_classes)),
                                                 {}, lambda ns: ns.update(class_body))
 
-                if "nested_instance_type" in inspect.signature(instance_type.__init__).parameters:
-                    instance: Instance = instance_type(instance_dto.name,
-                                                       nested_instance_type=nested_instance_type,
-                                                       from_dto=instance_dto, *args, **kwargs)
+                if "nested_instance_type" in inspect.signature(instance_type.__init__).parameters:  # type: ignore
+                    instance = instance_type(instance_dto.name,
+                                             nested_instance_type=nested_instance_type,
+                                             from_dto=instance_dto, *args, **kwargs)
                 else:
-                    instance: Instance = instance_type(instance_dto.name,
-                                                       from_dto=instance_dto, *args, **kwargs)
+                    instance = instance_type(instance_dto.name, from_dto=instance_dto, *args, **kwargs)
 
                 print(f"[WARNING] Mock instance created of spec '{instance_dto.spec.name}' for "
                       f"[{instance.get_full_name()}]. Reason: {e}", file=sys.stderr)
             else:
                 raise
 
         if ("disable_auto_update" not in kwargs) or (not kwargs["disable_auto_update"]):
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/misc.py` & `pypz_core-0.9.1/src/pypz/core/specs/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
-from typing import Optional, Any
+from typing import Optional, Any, TypeVar
 
-from pypz.core.specs.instance import Instance, NestedInstanceType
+from pypz.core.specs.instance import Instance
 from pypz.core.specs.operator import Operator
 from pypz.core.specs.plugin import Plugin, PortPlugin, InputPortPlugin, OutputPortPlugin, ResourceHandlerPlugin, \
     ServicePlugin
 
 
-class BlankInstance(Instance[NestedInstanceType]):
+BlankNestedInstanceType = TypeVar('BlankNestedInstanceType', bound='BlankInstance')
+
+
+class BlankInstance(Instance[BlankNestedInstanceType]):
 
     def _on_interrupt(self, system_signal: int = None) -> None:
         pass
 
     def _on_error(self) -> None:
         pass
```

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/operator.py` & `pypz_core-0.9.1/src/pypz/core/specs/operator.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/pipeline.py` & `pypz_core-0.9.1/src/pypz/core/specs/pipeline.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/plugin.py` & `pypz_core-0.9.1/src/pypz/core/specs/plugin.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/core/specs/utils.py` & `pypz_core-0.9.1/src/pypz/core/specs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 import types
 import re
+import typing
 from importlib import import_module
 from typing import Callable, Any, Iterable
 
 IncludedCascadingParameterPrefix = "#"
 """
 This strings denotes a cascading parameter. Included cascading parameter means
 that the model defines this parameter will get it provided as well the sub instances.
@@ -48,14 +49,15 @@
     def __setitem__(self, name, value):
         if ((name not in self) or (value != self[name])):
             super().__setitem__(name, value)
             if name in self.__update_callbacks:
                 for callback in self.__update_callbacks[name]:
                     callback(value)
 
+    @typing.no_type_check
     def update(self, __m, **kwargs) -> None:
         super().update(__m, **kwargs)
 
         for name, value in __m.items():
             if ((name not in self) or (value != self[name])) and (name in self.__update_callbacks):
                 for callback in self.__update_callbacks[name]:
                     callback(value)
@@ -75,18 +77,19 @@
     if there are instances w/o any dependencies, then those will be placed to level 0, which
     is the list[0]. On level 1 all the instances are placed that has dependencies to level 0
     instances and so on.
 
     :param instances: set of instances to resolve the dependencies across
     :return: list of sets, where the list represents dependency levels and set the instances on it
     """
-    if 0 < len(instances):
-        resolved_instances = set()
-        dependency_level_list = list()
-        instance_set = instances if isinstance(instances, set) else set(instances)
+    instance_set = instances if isinstance(instances, set) else set(instances)
+
+    if 0 < len(instance_set):
+        resolved_instances: set = set()
+        dependency_level_list: list[set] = list()
 
         for level in range(len(instance_set)):
             # We cannot have more dependency levels than instances we have, hence
             # the outer loop can always create a dependency level, where the instances
             # on the actual level will be stored
             dependency_level_list.append(set())
 
@@ -98,15 +101,15 @@
 
                 if (instance not in resolved_instances) and \
                         ((0 == len(available_dependencies)) or
                          available_dependencies.issubset(resolved_instances)):
                     dependency_level_list[level].add(instance)
 
             resolved_instances.update(dependency_level_list[level])
-            if len(resolved_instances) == len(instances):
+            if len(resolved_instances) == len(instance_set):
                 # Early termination, since all instance dependencies have been resolved
                 return dependency_level_list
 
         # If resolution could not be concluded in N*N steps, then it is very possible
         # that there is a circular dependency. Notice that the method depends_on()
         # checks for circular dependencies, still there is an edge case, where that
         # list is altered outside of that method.
```

### Comparing `pypz-core-0.9.0b9/src/pypz/deployers/base.py` & `pypz_core-0.9.1/src/pypz/deployers/base.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/commons.py` & `pypz_core-0.9.1/src/pypz/executors/commons.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/operator/context.py` & `pypz_core-0.9.1/src/pypz/executors/operator/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,27 +44,27 @@
         """
 
         self.__exit_code: ExitCodes = ExitCodes.NoError
         """
         Exit code of the state machine, which can be modified among the states
         """
 
-        self.__plugin_type_registry: dict[Type[PluginType], set[PluginType]] = dict()
+        self.__plugin_type_registry: dict[Type[Plugin], set[Plugin]] = dict()
         """
         This member holds all the context entities along their implemented interfaces. It allows
         simple type based iteration/execution.
         """
 
         for nested_instance in self.__operator.get_protected().get_nested_instances().values():
             for spec_class in nested_instance.get_protected().get_spec_classes():
                 if spec_class not in self.__plugin_type_registry:
                     self.__plugin_type_registry[spec_class] = set()
                 self.__plugin_type_registry[spec_class].add(nested_instance)
 
-        self.__typed_dependency_graphs: dict[Type[PluginType], list[set[PluginType]]] = dict()
+        self.__typed_dependency_graphs: dict[Type[Plugin], list[set[Plugin]]] = dict()
         """
         This member holds the nested instances ordered by their resolved dependency list along
         their types. The key holds the instance type, the value is a list of set, where each list
         element represents a dependency level i.e., the 0th element holds the instances w/o
         dependencies, the 1st element holds the instances that are dependent on instances on
         the 0th level and so on.
         """
```

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/operator/executor.py` & `pypz_core-0.9.1/src/pypz/executors/operator/executor.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/operator/signals.py` & `pypz_core-0.9.1/src/pypz/executors/operator/signals.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/operator/states.py` & `pypz_core-0.9.1/src/pypz/executors/operator/states.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,21 @@
         """
 
         self._transition_map: dict[Type[BaseSignal], State] = dict()
         """
         Contains the possible transitions from this state
         """
 
-        self._reason: BaseSignal | None = None
+        self._reason: Optional[BaseSignal] = None
         """
         Contains the information about the signal that drove the
         state machine into this state i.e., the reason of this state
         """
 
-        self._prev_state: State | None = None
+        self._prev_state: Optional[State] = None
         """
         Contains the information about the previous state the
         state machine was in
         """
 
         self._context: ExecutionContext = context
         """
@@ -154,15 +154,15 @@
 
     @abstractmethod
     def on_execute(self) -> BaseSignal:
         pass
 
     # ======== public methods =========
 
-    def get_prev_state(self) -> State:
+    def get_prev_state(self) -> Optional[State]:
         return self._prev_state
 
     def get_transitions(self):
         return self._transition_map
 
     def set_transition(self, signal: Type[BaseSignal], new_state: State) -> None:
         self._logger.debug("Setting up transition: (%s)--[%s]-->(%s)", self.__class__.__name__,
@@ -211,16 +211,17 @@
         """
 
         all_instances_finished: bool = True
         error_in_instances: list[str] = list()
 
         for execution_element in execution_chain:
 
-            method_name = \
-                execution_element[0] if isinstance(execution_element[0], str) else execution_element[0].__name__
+            method_name = execution_element[0] \
+                if isinstance(execution_element[0], str) else execution_element[0].__name__  # type: ignore
+
             instances = execution_element[1]
 
             futures: dict[concurrent.futures.Future, Callable[[], Any]] = dict()
             method_to_instance: dict[Callable[[], Any], Instance] = dict()
 
             for instance in instances:
                 # Early termination in case an actual instance object does not implement the
```

### Comparing `pypz-core-0.9.0b9/src/pypz/executors/pipeline/executor.py` & `pypz_core-0.9.1/src/pypz/executors/pipeline/executor.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/plugins/loggers/default.py` & `pypz_core-0.9.1/src/pypz/plugins/loggers/default.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/runnables/operator.py` & `pypz_core-0.9.1/src/pypz/runnables/operator.py`

 * *Files identical despite different names*

### Comparing `pypz-core-0.9.0b9/src/pypz/version.py` & `pypz_core-0.9.1/src/pypz/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =============================================================================
 
-PROJECT_VERSION = "0.9.0b9"
+PROJECT_VERSION = "0.9.1"
```

### Comparing `pypz-core-0.9.0b9/src/pypz_core.egg-info/PKG-INFO` & `pypz_core-0.9.1/src/pypz_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pypz-core
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: Core components of pypz (pipes), which is a lightweight Pipeline as Code (PaC) framework.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,pypz-core
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: static
-Requires-Dist: flake8; extra == "static"
+Requires-Dist: flake8~=7.0.0; extra == "static"
 Requires-Dist: flake8-html~=0.4.3; extra == "static"
-Requires-Dist: mypy; extra == "static"
-Requires-Dist: coverage; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains all the necessary core components to realize the
 functionalities of *pypz*.
 
 Check the [documentation](https://lazlowa.github.io/pypz-python/index.html) for
```

### Comparing `pypz-core-0.9.0b9/src/pypz_core.egg-info/SOURCES.txt` & `pypz_core-0.9.1/src/pypz_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

