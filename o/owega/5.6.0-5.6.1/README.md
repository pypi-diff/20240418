# Comparing `tmp/owega-5.6.0.tar.gz` & `tmp/owega-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.6.0.tar", last modified: Mon Apr 15 15:38:06 2024, max compression
+gzip compressed data, was "owega-5.6.1.tar", last modified: Thu Apr 18 20:51:53 2024, max compression
```

## Comparing `owega-5.6.0.tar` & `owega-5.6.1.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.365899 owega-5.6.0/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-10 21:13:16.000000 owega-5.6.0/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15683 2024-04-15 15:38:06.365899 owega-5.6.0/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-10 21:13:16.000000 owega-5.6.0/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.363899 owega-5.6.0/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.364899 owega-5.6.0/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1492 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.364899 owega-5.6.0/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4378 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5850 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.364899 owega-5.6.0/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-10 21:13:16.000000 owega-5.6.0/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-10 21:13:16.000000 owega-5.6.0/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-10 21:13:16.000000 owega-5.6.0/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9257 2024-04-15 15:37:02.000000 owega-5.6.0/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.364899 owega-5.6.0/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-10 21:13:16.000000 owega-5.6.0/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23392 2024-04-15 15:35:20.000000 owega-5.6.0/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-10 21:13:16.000000 owega-5.6.0/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-10 21:13:16.000000 owega-5.6.0/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.365899 owega-5.6.0/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-10 21:13:16.000000 owega-5.6.0/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1808 2024-04-15 15:36:15.000000 owega-5.6.0/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.365899 owega-5.6.0/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-10 21:13:16.000000 owega-5.6.0/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10076 2024-04-10 21:13:16.000000 owega-5.6.0/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-10 21:13:16.000000 owega-5.6.0/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-10 21:13:16.000000 owega-5.6.0/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11666 2024-04-10 21:13:16.000000 owega-5.6.0/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6042 2024-04-10 21:13:16.000000 owega-5.6.0/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-15 15:38:06.365899 owega-5.6.0/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15683 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1637 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-15 15:38:06.000000 owega-5.6.0/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-10 21:13:16.000000 owega-5.6.0/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-15 15:38:06.365899 owega-5.6.0/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-10 21:13:16.000000 owega-5.6.0/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.018164 owega-5.6.1/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.1/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15726 2024-04-18 20:51:53.018164 owega-5.6.1/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.1/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.012164 owega-5.6.1/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.015164 owega-5.6.1/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      874 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1430 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1076 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1515 2024-04-18 20:42:21.000000 owega-5.6.1/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1695 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3372 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1175 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4778 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1692 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      418 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      422 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3056 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      993 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1568 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1670 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      552 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      967 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      846 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1617 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1277 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1446 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1105 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.015164 owega-5.6.1/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4341 2024-04-18 20:40:40.000000 owega-5.6.1/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5813 2024-04-18 20:41:08.000000 owega-5.6.1/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.016164 owega-5.6.1/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2762 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5590 2024-04-17 02:21:38.000000 owega-5.6.1/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       62 2024-04-17 02:21:38.000000 owega-5.6.1/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.1/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9249 2024-04-18 20:30:35.000000 owega-5.6.1/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23524 2024-04-18 20:51:22.000000 owega-5.6.1/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1533 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.1/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.1/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1808 2024-04-17 02:21:38.000000 owega-5.6.1/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.1/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10102 2024-04-18 20:35:07.000000 owega-5.6.1/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:49:15.000000 owega-5.6.1/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.1/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.1/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11666 2024-04-17 02:21:38.000000 owega-5.6.1/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6026 2024-04-18 20:46:49.000000 owega-5.6.1/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-04-18 20:51:53.017164 owega-5.6.1/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15726 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-04-18 20:51:52.000000 owega-5.6.1/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.1/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-04-18 20:51:53.018164 owega-5.6.1/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-17 02:21:38.000000 owega-5.6.1/setup.py
```

### Comparing `owega-5.6.0/PKG-INFO` & `owega-5.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.0
+Version: 5.6.1
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.0 CHANGELOG:
+OWEGA v5.6.1 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -355,8 +355,9 @@
 5.5.4: Fixed a debug_print never showing.
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
 5.6.0: Added basic support for Chub's API 
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
+5.6.1: Added extensive logging for errors.
 ```
```

### Comparing `owega-5.6.0/README.md` & `owega-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.6.1/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_commands.py` & `owega-5.6.1/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_context.py` & `owega-5.6.1/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.6.1/owega/OweHandlers/handle_del_sysmem.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     temp_is_temp=False,
     silent=False
 ):
     """Handle /del_sysmem."""
     given = given.strip()
     for index, sysmem in enumerate(messages.systemsouv):
         if not silent:
-            print(f"[\033[0;95mSystem souvenir\033[0m] [\033[0;92m{index}\033[0m]:")
+            print("[\033[0;95mSystem souvenir\033[0m] "
+                  + f"[\033[0;92m{index}\033[0m]:")
             print('\033[0;37m', end='')
             print(sysmem)
             print('\033[0m', end='')
             print()
     try:
         if not given:
             msg_id = ps['integer'].prompt(pt.ANSI(
```

### Comparing `owega-5.6.0/owega/OweHandlers/handle_dinput.py` & `owega-5.6.1/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_edit.py` & `owega-5.6.1/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_estimation.py` & `owega-5.6.1/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_finput.py` & `owega-5.6.1/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_frequency.py` & `owega-5.6.1/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_image.py` & `owega-5.6.1/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_load.py` & `owega-5.6.1/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_model.py` & `owega-5.6.1/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_presence.py` & `owega-5.6.1/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_quit.py` & `owega-5.6.1/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_save.py` & `owega-5.6.1/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_system.py` & `owega-5.6.1/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_temperature.py` & `owega-5.6.1/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_tokens.py` & `owega-5.6.1/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_top_p.py` & `owega-5.6.1/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handle_tts.py` & `owega-5.6.1/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OweHandlers/handlers.py` & `owega-5.6.1/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OwegaFun/__init__.py` & `owega-5.6.1/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OwegaFun/functions.py` & `owega-5.6.1/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.6.1/owega/OwegaFun/longTermSouvenirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Long Term Souvenirs related functions."""
 from .functions import Functions, disabledFunction
-from owega.config import debug_print
 import json
 
 LTS = Functions()
 
 
 fcts = {}
 fcts["addfun"] = disabledFunction
```

### Comparing `owega-5.6.0/owega/OwegaFun/utility.py` & `owega-5.6.1/owega/OwegaFun/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Utility functions."""
 from owega.utils import command_text
-from owega.config import debug_print
 from .functions import Functions
 import subprocess
 import prompt_toolkit as pt
 import json
 import requests
 import bs4
 from markdownify import MarkdownConverter as MC
```

### Comparing `owega-5.6.0/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.6.1/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/OwegaSession/promptsession.py` & `owega-5.6.1/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/ask.py` & `owega-5.6.1/owega/ask.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import openai
 import json5 as json
 import json as jsonbase
 import re
 import requests
 from .utils import debug_print
+from . import getLogger
 
 
 def convert_invalid_json(invalid_json):
     """
     Try converting invalid json to valid json.
 
     Sometimes, GPT will give back invalid json.
@@ -42,20 +43,22 @@
     temp_api_key="",
     temp_organization="",
     top_p=baseConf.get("top_p", 1.0),
     frequency_penalty=baseConf.get("frequency_penalty", 0.0),
     presence_penalty=baseConf.get("presence_penalty", 0.0),
 ):
     """Ask a question via OpenAI or Mistral based on the model."""
-    if baseConf.get("debug", False):
-        bc = baseConf.copy()
-        bc["api_key"] = "REDACTED"
-        bc["mistral_api"] = "REDACTED"
-        bc["chub_api"] = "REDACTED"
-        debug_print(f"{bc}", True)
+    logger = getLogger.getLogger(__name__, debug=baseConf.get("debug", False))
+
+    bc = baseConf.copy()
+    bc["api_key"] = "REDACTED"
+    bc["mistral_api"] = "REDACTED"
+    bc["chub_api"] = "REDACTED"
+    logger.debug(f"{bc}")
+
     connectLTS(
         messages.add_memory, messages.remove_memory, messages.edit_memory)
     old_api_key = openai.api_key
     old_organization = openai.organization
     if (prompt):
         messages.add_question(prompt)
     else:
@@ -72,29 +75,27 @@
 
     headers = {}
     data_payload = {}
 
     client = openai.OpenAI()
 
     if is_chub:
-        debug_print(f"Using Chub's API for model: {model}",
-            baseConf.get("debug", False))
+        logger.info(f"Using Chub's API for model: {model}")
         if model in ["mars", "asha"]:
             model = "asha"
             client.base_url = 'https://mars.chub.ai/chub/asha/v1'
         elif model in ["mercury", "mythomax"]:
             model = "mythomax"
             client.base_url = 'https://mercury.chub.ai/mythomax/v1'
         elif model in ["mistral", "mixtral"]:
             model = "mixtral"
             client.base_url = 'https://mars.chub.ai/mixtral/v1'
         client.api_key = baseConf.get('chub_api', '')
     elif is_mistral:
-        debug_print(f"Using Mistral API for model: {model}",
-            baseConf.get("debug", False))
+        logger.info(f"Using Mistral API for model: {model}")
         client.base_url = 'https://api.mistral.ai/v1'
         client.api_key = baseConf.get('mistral_api', '')
 
     if isinstance(function_call, bool):
         if function_call:
             function_call = "auto"
         else:
@@ -148,15 +149,15 @@
                             max_tokens=max_tokens,
                             top_p=top_p,
                             frequency_penalty=frequency_penalty,
                             presence_penalty=presence_penalty,
                             messages=messages.get_messages(),
                         )
                     except Exception as e:
-                        print(e)
+                        logger.exception(e)
                 else:
                     response = client.chat.completions.create(
                         model=model,
                         temperature=temperature,
                         max_tokens=max_tokens,
                         top_p=top_p,
                         frequency_penalty=frequency_penalty,
@@ -165,25 +166,25 @@
                         tools=functionlist_to_toollist(
                             existingFunctions.getEnabled()),
                         tool_choice=function_call,
                     )
         except openai.BadRequestError as e:
             try:
                 messages.shorten()
-            except Exception:
-                print("[Owega] Critical error... Aborting request...")
-                print("[Owega] " +
-                      "Please, send the following to @darkgeem on discord")
-                print("[Owega] Along with a saved .json of your request.")
-                print(e)
+            except Exception as e:
+                lf = getLogger.getLoggerFile()
+                logger.critical("Critical error... Aborting request...")
+                logger.critical(f"Please, send {lf} to @darkgeem on discord")
+                logger.critical("Along with a saved .json of your request.")
+                logger.exception(e)
                 return messages
         except openai.InternalServerError:
-            print("[Owega] Service unavailable...", end="")
+            logger.error("Service unavailable...")
             time.sleep(1)
-            print(" Retrying now...")
+            logger.error("Retrying now...")
     # do something with the response
     message = response.choices[0].message
     while message.tool_calls is not None:
         try:
             for tool_call in message.tool_calls:
                 tool_function = tool_call.function
                 function_name = tool_function.name
@@ -214,21 +215,21 @@
                         tools=functionlist_to_toollist(
                             existingFunctions.getEnabled()),
                         tool_choice=function_call,
                     )
                 except openai.error.InvalidRequestError:
                     messages.shorten()
                 except openai.error.ServiceUnavailableError:
-                    print("[Owega] Service unavailable...", end="")
+                    logger.error("Service unavailable...")
                     time.sleep(1)
-                    print(" Retrying now...")
+                    logger.error("Retrying now...")
                 message = response2.choices[0].message
         except Exception as e:
-            print("Exception: " + str(e))
-            print(message.tool_calls[0].function.name)
-            print(message.tool_calls[0].function.arguments)
+            logger.exception(e)
+            logger.error(message.tool_calls[0].function.name)
+            logger.error(message.tool_calls[0].function.arguments)
             break
     try:
         messages.add_answer(message.content.strip())
     except Exception as e:
-        print("Exception: " + str(e))
+        logger.exception(e)
     return messages
```

### Comparing `owega-5.6.0/owega/changelog/changelog.py` & `owega-5.6.1/owega/changelog/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 6, 1)
+            .addLine("Added extensive logging for errors.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 6, 0)
             .addLine("Added basic support for Chub's API ")
             .addLine("(chub mars, mercury, mixtral)")
             .addLine("Also, Mi(s/x)tral support is no more in beta :D")
         )
 
         self.logs.append(
```

### Comparing `owega-5.6.0/owega/changelog/changelogEntry.py` & `owega-5.6.1/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/changelog/version.py` & `owega-5.6.1/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/config/baseConf.py` & `owega-5.6.1/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/conversation/conversation.py` & `owega-5.6.1/owega/conversation/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Handles a GPT conversation history."""
 import json5 as json
 import sys
 from owega.changelog import OwegaChangelog, Version
+from .. import getLogger
 
 
 # messages class, contains helper functions to manage context and messages
 class Conversation:
     """Contains an history and everything that should be stored."""
 
     def __init__(
@@ -14,14 +15,15 @@
             "forced to answer any question asked"
     ):
         """Initialize the Conversation."""
         self.context = system_context
         self.souvenirs = []
         self.messages = []
         self.systemsouv = []
+        self.logger = getLogger.getLogger(__name__)
 
     def get_context(self):
         """Get AI context."""
         return self.context
 
     def set_context(
         self,
@@ -276,19 +278,16 @@
                 compat_mode = True
         if compat_mode:
             return self.old_load(path)
         return self.new_load(path)
 
     def shorten(self):
         """Shorten the message array."""
-        print(
-            "[Owega] Too many tokens required, shortening the messages "
-            + "array...",
-            file=sys.stderr
-        )
+        self.logger.error(
+            "Too many tokens required, shortening the messages array...")
         if (len(self.messages) <= 1):
             raise ValueError("Can't shorten messages, already at minimum")
         self.messages.pop(1)
 
     # prints an Conversation history
     def print_history(self):
         """Print the message history."""
```

### Comparing `owega-5.6.0/owega/license.py` & `owega-5.6.1/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/owega.py` & `owega-5.6.1/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.0/owega/utils.py` & `owega-5.6.1/owega/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import openai
 import warnings
 from .conversation import Conversation
 from .config import baseConf
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 warnings.filterwarnings("ignore", category=RuntimeWarning, message=".*pygame.*")
 import pygame  # noqa
+from . import getLogger
 
 
 def genconfig(conf_path=""):
     """Generate the config file if it doesn't exist already."""
     if not conf_path:
         conf_path = get_home_dir() + "/.owega.json"
     is_blank = True
@@ -83,20 +84,17 @@
         req = ""
         req += ppt
         req += json.dumps(messages.get_messages())
         req += json.dumps(functions)
         tokens = encoder.encode(req)
         return len(tokens)
     except Exception as e:
-        if baseConf.baseConf.get("debug"):
-            print(
-                "An error has occured while estimating tokens:",
-                file=sys.stderr
-            )
-            print(e, file=sys.stderr)
+        logger = getLogger.getLogger(__name__, baseConf.baseConf.get("debug"))
+        logger.info("An error has occured while estimating tokens:")
+        logger.info(e)
         return 0
 
 
 def get_temp_file() -> str:
     """Get a temp file location."""
     tmp = tempfile.NamedTemporaryFile(
         prefix="owega_temp.",
```

### Comparing `owega-5.6.0/owega.egg-info/PKG-INFO` & `owega-5.6.1/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.0
+Version: 5.6.1
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.0 CHANGELOG:
+OWEGA v5.6.1 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -355,8 +355,9 @@
 5.5.4: Fixed a debug_print never showing.
 5.5.5: Now using openai module to ask mistral API.
        (the code is waaaay cleaner)
 
 5.6.0: Added basic support for Chub's API 
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
+5.6.1: Added extensive logging for errors.
 ```
```

### Comparing `owega-5.6.0/owega.egg-info/SOURCES.txt` & `owega-5.6.1/owega.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 owega/__init__.py
 owega/__main__.py
 owega/ask.py
+owega/getLogger.py
 owega/handlerBase.py
 owega/license.py
 owega/owega.py
 owega/utils.py
 owega.egg-info/PKG-INFO
 owega.egg-info/SOURCES.txt
 owega.egg-info/dependency_links.txt
```

### Comparing `owega-5.6.0/setup.py` & `owega-5.6.1/setup.py`

 * *Files identical despite different names*

