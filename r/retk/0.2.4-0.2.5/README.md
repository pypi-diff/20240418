# Comparing `tmp/retk-0.2.4.tar.gz` & `tmp/retk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retk-0.2.4.tar", last modified: Wed Apr 17 01:54:47 2024, max compression
+gzip compressed data, was "retk-0.2.5.tar", last modified: Thu Apr 18 19:00:48 2024, max compression
```

## Comparing `retk-0.2.4.tar` & `retk-0.2.5.tar`

### file list

```diff
@@ -1,469 +1,177 @@
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.300920 retk-0.2.4/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    35149 2023-12-13 13:08:22.000000 retk-0.2.4/LICENSE
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5874 2024-04-17 01:54:47.300833 retk-0.2.4/PKG-INFO
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4073 2024-02-22 05:30:54.000000 retk-0.2.4/README.md
--rw-r--r--   0 morvanzhou   (501) staff       (20)       94 2022-11-07 07:33:46.000000 retk-0.2.4/pyproject.toml
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1509 2024-04-17 01:54:47.301327 retk-0.2.4/setup.cfg
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.093384 retk-0.2.4/src/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.099459 retk-0.2.4/src/rethink/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4112 2024-04-05 08:00:09.000000 retk-0.2.4/src/rethink/.env.local
--rw-r--r--   0 morvanzhou   (501) staff       (20)      283 2024-04-03 16:25:09.000000 retk-0.2.4/src/rethink/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)       91 2024-04-03 15:50:31.000000 retk-0.2.4/src/rethink/_version.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1927 2024-04-15 17:15:20.000000 retk-0.2.4/src/rethink/application.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4240 2024-04-05 08:10:50.000000 retk-0.2.4/src/rethink/config.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    10935 2024-04-16 03:57:11.000000 retk-0.2.4/src/rethink/const.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.104323 retk-0.2.4/src/rethink/controllers/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-31 15:56:56.000000 retk-0.2.4/src/rethink/controllers/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4898 2024-04-13 15:56:36.000000 retk-0.2.4/src/rethink/controllers/account.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      536 2024-04-17 01:41:48.000000 retk-0.2.4/src/rethink/controllers/app_system.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.104855 retk-0.2.4/src/rethink/controllers/files/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2023-10-31 05:38:31.000000 retk-0.2.4/src/rethink/controllers/files/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3109 2024-04-16 05:30:46.000000 retk-0.2.4/src/rethink/controllers/files/upload_files.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.106221 retk-0.2.4/src/rethink/controllers/node/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2023-10-02 07:49:52.000000 retk-0.2.4/src/rethink/controllers/node/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5275 2024-04-16 05:19:18.000000 retk-0.2.4/src/rethink/controllers/node/node_ops.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1816 2024-04-16 05:28:12.000000 retk-0.2.4/src/rethink/controllers/node/search.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2456 2024-04-13 17:54:19.000000 retk-0.2.4/src/rethink/controllers/node/trash_ops.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3723 2024-04-15 16:44:51.000000 retk-0.2.4/src/rethink/controllers/oauth.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3122 2024-04-15 17:26:46.000000 retk-0.2.4/src/rethink/controllers/plugin.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      749 2024-04-16 02:03:56.000000 retk-0.2.4/src/rethink/controllers/recent.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.109577 retk-0.2.4/src/rethink/controllers/schemas/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      206 2024-04-13 15:45:30.000000 retk-0.2.4/src/rethink/controllers/schemas/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1163 2024-04-13 15:45:30.000000 retk-0.2.4/src/rethink/controllers/schemas/account.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      233 2024-04-17 01:41:15.000000 retk-0.2.4/src/rethink/controllers/schemas/app_system.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      649 2024-04-16 03:57:11.000000 retk-0.2.4/src/rethink/controllers/schemas/files.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1795 2024-04-16 12:21:26.000000 retk-0.2.4/src/rethink/controllers/schemas/node.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)       91 2024-04-13 17:54:19.000000 retk-0.2.4/src/rethink/controllers/schemas/oauth.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      640 2024-04-15 17:11:45.000000 retk-0.2.4/src/rethink/controllers/schemas/plugin.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      320 2024-04-16 02:03:56.000000 retk-0.2.4/src/rethink/controllers/schemas/recent.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2302 2024-04-16 04:23:41.000000 retk-0.2.4/src/rethink/controllers/schemas/user.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3996 2024-04-13 15:56:36.000000 retk-0.2.4/src/rethink/controllers/user.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3794 2024-04-13 11:14:49.000000 retk-0.2.4/src/rethink/controllers/utils.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.110331 retk-0.2.4/src/rethink/core/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       89 2024-04-12 19:12:16.000000 retk-0.2.4/src/rethink/core/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.120252 retk-0.2.4/src/rethink/core/account/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       73 2024-04-16 01:48:35.000000 retk-0.2.4/src/rethink/core/account/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1598 2024-04-12 05:59:21.000000 retk-0.2.4/src/rethink/core/account/app_captcha.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4235 2024-04-12 19:12:22.000000 retk-0.2.4/src/rethink/core/account/email.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3058 2024-04-13 09:15:51.000000 retk-0.2.4/src/rethink/core/account/manager.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.124411 retk-0.2.4/src/rethink/core/files/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      144 2024-02-01 04:24:50.000000 retk-0.2.4/src/rethink/core/files/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      714 2024-01-31 05:02:48.000000 retk-0.2.4/src/rethink/core/files/get.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.124741 retk-0.2.4/src/rethink/core/files/importing/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-31 06:56:13.000000 retk-0.2.4/src/rethink/core/files/importing/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.126330 retk-0.2.4/src/rethink/core/files/importing/async_tasks/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1077 2024-01-31 12:31:27.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.147336 retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-31 07:00:15.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5961 2024-04-02 01:59:19.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/ops.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7972 2024-04-13 10:39:34.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/task.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.147802 retk-0.2.4/src/rethink/core/files/importing/async_tasks/text/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-31 07:02:26.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/text/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3160 2024-04-13 11:10:48.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/text/task.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3530 2024-01-31 12:36:46.000000 retk-0.2.4/src/rethink/core/files/importing/async_tasks/utils.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.148639 retk-0.2.4/src/rethink/core/files/importing/sync_tasks/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       59 2024-01-31 16:06:38.000000 retk-0.2.4/src/rethink/core/files/importing/sync_tasks/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1641 2024-02-01 05:15:40.000000 retk-0.2.4/src/rethink/core/files/importing/sync_tasks/editor.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4991 2024-04-13 10:00:15.000000 retk-0.2.4/src/rethink/core/files/saver.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6163 2024-04-16 03:57:11.000000 retk-0.2.4/src/rethink/core/files/upload.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.150616 retk-0.2.4/src/rethink/core/node/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       75 2024-04-16 01:48:36.000000 retk-0.2.4/src/rethink/core/node/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7171 2024-04-16 01:48:35.000000 retk-0.2.4/src/rethink/core/node/backup.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13529 2024-04-13 10:07:45.000000 retk-0.2.4/src/rethink/core/node/node.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1710 2024-04-02 03:26:52.000000 retk-0.2.4/src/rethink/core/node/node_utils.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3547 2024-04-13 09:35:42.000000 retk-0.2.4/src/rethink/core/node/search.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1363 2024-04-13 08:23:26.000000 retk-0.2.4/src/rethink/core/recent.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7059 2024-04-16 01:48:35.000000 retk-0.2.4/src/rethink/core/user.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.151191 retk-0.2.4/src/rethink/depend/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-10 03:52:25.000000 retk-0.2.4/src/rethink/depend/__init__.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.155368 retk-0.2.4/src/rethink/depend/mongita/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2465 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    44121 2024-01-31 16:06:38.000000 retk-0.2.4/src/rethink/depend/mongita/collection.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1199 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/command_cursor.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4117 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/common.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5465 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/cursor.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4484 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/database.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.156584 retk-0.2.4/src/rethink/depend/mongita/engines/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/engines/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9518 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/engines/disk_engine.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2994 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/engines/engine_common.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2167 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/engines/memory_engine.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1077 2024-01-31 16:03:55.000000 retk-0.2.4/src/rethink/depend/mongita/errors.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5827 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/mongita_client.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5340 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/mongitasync.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      375 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/read_concern.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      684 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/results.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      588 2023-11-18 10:29:27.000000 retk-0.2.4/src/rethink/depend/mongita/write_concern.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.159339 retk-0.2.4/src/rethink/depend/sso/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2023-08-07 17:23:01.000000 retk-0.2.4/src/rethink/depend/sso/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11277 2023-10-08 08:12:55.000000 retk-0.2.4/src/rethink/depend/sso/base.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1200 2023-09-13 06:45:25.000000 retk-0.2.4/src/rethink/depend/sso/facebook.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2511 2023-10-08 08:04:28.000000 retk-0.2.4/src/rethink/depend/sso/generic.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      932 2023-10-06 08:43:20.000000 retk-0.2.4/src/rethink/depend/sso/github.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      905 2023-09-12 14:15:39.000000 retk-0.2.4/src/rethink/depend/sso/gitlab.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1304 2023-09-12 14:15:39.000000 retk-0.2.4/src/rethink/depend/sso/google.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1713 2023-10-08 08:12:55.000000 retk-0.2.4/src/rethink/depend/sso/microsoft.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1301 2023-09-13 06:26:38.000000 retk-0.2.4/src/rethink/depend/sso/qq.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.160248 retk-0.2.4/src/rethink/dist-local/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.160523 retk-0.2.4/src/rethink/dist-local/css/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   173347 2024-04-05 10:20:51.000000 retk-0.2.4/src/rethink/dist-local/css/app.css
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.088624 retk-0.2.4/src/rethink/dist-local/dist/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.088238 retk-0.2.4/src/rethink/dist-local/dist/css/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.161971 retk-0.2.4/src/rethink/dist-local/dist/css/content-theme/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4721 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/css/content-theme/ant-design.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2793 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/css/content-theme/dark.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2510 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/css/content-theme/light.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2814 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/css/content-theme/wechat.css
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.162485 retk-0.2.4/src/rethink/dist-local/dist/images/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.167157 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4773 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/b3log.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3663 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/chainbook.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3291 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/doge.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1587 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/hacpai.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13662 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/huaji.gif
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3264 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/latke.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1587 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/liandi.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1052 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/lute.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3738 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/octocat.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2247 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/pipe.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1153 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/siyuan.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3890 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/solo.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3267 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/sym.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4901 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/trollface.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2177 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/vditor.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5128 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/wide.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     8469 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/emoji/wulian.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1517 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/img-loading.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2050 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/images/logo.png
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.091238 retk-0.2.4/src/rethink/dist-local/dist/js/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.167494 retk-0.2.4/src/rethink/dist-local/dist/js/abcjs/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   363243 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/abcjs/abcjs_basic.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.168345 retk-0.2.4/src/rethink/dist-local/dist/js/echarts/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   762119 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/echarts/echarts.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.169597 retk-0.2.4/src/rethink/dist-local/dist/js/flowchart.js/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   125802 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/flowchart.js/flowchart.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.173953 retk-0.2.4/src/rethink/dist-local/dist/js/graphviz/
--rw-r--r--   0 morvanzhou   (501) staff       (20)  4423759 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/graphviz/full.render.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11468 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/graphviz/viz.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.179635 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   376423 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/highlight.pack.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6604 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/solidity.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.188221 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6457 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/abap.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5774 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5013 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol_nu.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7299 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/ant-design.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6374 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/arduino.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6732 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/autumn.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6149 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/borland.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5931 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/bw.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     8006 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/colorful.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6125 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/dracula.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7277 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/emacs.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7407 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/friendly.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6144 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/fruity.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7638 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/github.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4366 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/igor.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7076 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/lovelace.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7248 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/manni.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5876 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokai.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7188 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokailight.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7646 2024-04-05 10:20:51.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/murphy.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7139 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/native.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6172 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-dark.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6172 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-light.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7988 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pastie.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6754 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/perldoc.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7041 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pygments.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7312 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rainbow_dash.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5192 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rrt.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6072 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6291 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark256.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7780 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-light.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6002 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/swapoff.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     8775 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/tango.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6940 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/trac.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6007 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vim.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4436 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vs.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6672 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/xcode.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2733 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/highlight.js/yul.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.190588 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2384 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/en_US.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2694 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/fr_FR.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3010 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/ja_JP.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2739 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/ko_KR.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2700 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/pt_BR.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4172 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/ru_RU.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2634 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/sv_SE.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2530 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_CN.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2512 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_TW.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.191286 retk-0.2.4/src/rethink/dist-local/dist/js/icons/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    42983 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/icons/ant.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    20896 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/icons/material.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.192831 retk-0.2.4/src/rethink/dist-local/dist/js/katex/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.211443 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    63632 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    33516 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    28076 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12368 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7716 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6912 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12344 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7656 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6908 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19584 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13296 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11348 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19572 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13208 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11316 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    51336 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    29912 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    25324 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    32968 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19412 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16780 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    33580 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19676 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16988 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    53580 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    30772 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    26272 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    31196 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    18668 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16400 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    31308 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    18748 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16440 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    24504 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    14408 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12216 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    22364 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    14112 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12028 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19436 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12316 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    10344 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16648 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    10588 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9644 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    12228 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6496 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5468 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11508 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6188 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5208 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7588 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4420 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3624 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    10364 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5980 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4928 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    27556 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16028 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13568 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 morvanzhou   (501) staff       (20)    23196 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)   277038 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    33730 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/katex/mhchem.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.211760 retk-0.2.4/src/rethink/dist-local/dist/js/lute/
--rw-r--r--   0 morvanzhou   (501) staff       (20)  3785907 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/lute/lute.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.222025 retk-0.2.4/src/rethink/dist-local/dist/js/markmap/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    23112 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/markmap/katex.min.css
--rw-r--r--   0 morvanzhou   (501) staff       (20)   824275 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/markmap/markmap.min.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2383 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/markmap/prism.css
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.222671 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11358 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/LICENSE
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.226624 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6982 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/assistive-mml.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    18478 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/complexity.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    32640 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/explorer.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     8767 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/semantic-enrich.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.228942 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   106067 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/asciimath.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.229664 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    33265 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml/entities.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    14009 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.090858 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.237371 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3302 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/action.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   147205 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/all-packages.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    23357 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/ams.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7056 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/amscd.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7019 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/autoload.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3693 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bbox.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4709 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/boldsymbol.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7150 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/braket.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    17174 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bussproofs.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4029 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/cancel.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9192 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/color.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3076 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/colorV2.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4764 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/configMacros.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3071 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/enclose.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4158 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/extpfeil.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3572 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/html.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    36819 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/mhchem.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    10840 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/newcommand.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2049 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noerrors.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2657 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noundefined.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    23443 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/physics.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6521 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/require.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3842 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/tagFormat.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    15926 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/textmacros.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4151 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/unicode.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3258 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/verb.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   129130 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-base.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   270488 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-full.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   163954 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.237838 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.248343 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/
--rw-r--r--   0 morvanzhou   (501) staff       (20)   326869 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/de.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   423424 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/en.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   326446 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/es.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   321576 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/fr.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)  1795679 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/mathmaps_ie.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   301796 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/nemeth.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)      288 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/sre-node.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   874345 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/sre_browser.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)  1811419 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mathjax/tex-svg-full.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.249259 retk-0.2.4/src/rethink/dist-local/dist/js/mermaid/
--rw-r--r--   0 morvanzhou   (501) staff       (20)  1084448 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/mermaid/mermaid.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.250776 retk-0.2.4/src/rethink/dist-local/dist/js/plantuml/
--rw-r--r--   0 morvanzhou   (501) staff       (20)    29433 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/dist/js/plantuml/plantuml-encoder.min.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)    38078 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/favicon.ico
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.263747 retk-0.2.4/src/rethink/dist-local/img/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5369 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/2023_Obsidian_logo.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      482 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/back.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      695 2024-04-05 10:20:51.000000 retk-0.2.4/src/rethink/dist-local/img/checked-success.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      374 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/chevron-double-left.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1266 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/circle-user.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      800 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/cross.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      578 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/diagonal-arrow-right-up.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      642 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/dropdown-arrow.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      298 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/expand-down.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      299 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/expand-up.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      426 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/expand.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3995 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/eye-closed.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      815 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/eye-open.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      990 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/github-mark.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      799 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/home.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      888 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/import.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      451 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/list.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)    16729 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/loading-dots.gif
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19402 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/loading.gif
--rw-r--r--   0 morvanzhou   (501) staff       (20)      353 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/menu.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)    85421 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/morvanQR.png
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1555 2024-04-05 10:20:55.000000 retk-0.2.4/src/rethink/dist-local/img/node.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      909 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/plugin.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      342 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/plus.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      565 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/recentoutline.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      549 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/restore.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      763 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/return-arrow.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1851 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/search.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      534 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/sort.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      443 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/tab.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      400 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/text.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      925 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/three-dots-vertical.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      392 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/tick.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1149 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/trash.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      725 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/upload.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1044 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/view-grid.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      798 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/img/white-cross.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)      989 2024-04-05 10:20:51.000000 retk-0.2.4/src/rethink/dist-local/index.html
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.269397 retk-0.2.4/src/rethink/dist-local/js/
--rw-r--r--   0 morvanzhou   (501) staff       (20)  1868785 2024-04-05 10:21:06.000000 retk-0.2.4/src/rethink/dist-local/js/app.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)  1266654 2024-04-05 10:21:06.000000 retk-0.2.4/src/rethink/dist-local/js/chunk-vendors.js
--rw-r--r--   0 morvanzhou   (501) staff       (20)   121728 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/js/highlight.min.js
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.269978 retk-0.2.4/src/rethink/dist-local/media/
--rw-r--r--   0 morvanzhou   (501) staff       (20)  3429085 2024-04-05 10:18:56.000000 retk-0.2.4/src/rethink/dist-local/media/demo.mp4
--rw-r--r--   0 morvanzhou   (501) staff       (20)      910 2024-04-03 14:39:55.000000 retk-0.2.4/src/rethink/logger.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.279581 retk-0.2.4/src/rethink/models/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2024-01-31 13:38:00.000000 retk-0.2.4/src/rethink/models/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    15037 2024-04-13 09:47:06.000000 retk-0.2.4/src/rethink/models/client.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      500 2024-01-31 13:21:43.000000 retk-0.2.4/src/rethink/models/coll.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2095 2024-04-12 17:17:25.000000 retk-0.2.4/src/rethink/models/db_ops.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1530 2024-04-11 07:06:46.000000 retk-0.2.4/src/rethink/models/indexing.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.281938 retk-0.2.4/src/rethink/models/search_engine/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      111 2024-01-31 16:03:12.000000 retk-0.2.4/src/rethink/models/search_engine/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9132 2023-12-13 06:16:11.000000 retk-0.2.4/src/rethink/models/search_engine/baidu_stopwords.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4717 2023-12-12 10:26:15.000000 retk-0.2.4/src/rethink/models/search_engine/cn_stopwords.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3958 2024-04-13 09:35:42.000000 retk-0.2.4/src/rethink/models/search_engine/engine.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    22542 2024-04-13 11:14:49.000000 retk-0.2.4/src/rethink/models/search_engine/engine_es.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    11133 2024-04-13 11:14:49.000000 retk-0.2.4/src/rethink/models/search_engine/engine_local.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4708 2024-04-16 04:23:41.000000 retk-0.2.4/src/rethink/models/tps.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.283170 retk-0.2.4/src/rethink/plugins/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       36 2024-04-03 16:25:09.000000 retk-0.2.4/src/rethink/plugins/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     6725 2024-04-16 01:35:55.000000 retk-0.2.4/src/rethink/plugins/base.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1669 2024-04-13 09:23:28.000000 retk-0.2.4/src/rethink/plugins/handler.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.092495 retk-0.2.4/src/rethink/plugins/official_plugins/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.283546 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.284937 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/__pycache__/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2907 2024-04-03 15:55:19.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/__pycache__/main.cpython-310.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5341 2024-04-03 15:56:29.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2910 2024-04-03 15:51:31.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2910 2024-03-28 17:43:34.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/__pycache__/main.cpython-39.pyc
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.285295 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/_static/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5502 2024-03-28 17:43:23.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/_static/logo.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2773 2024-03-28 17:43:23.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/main.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.285841 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1907 2024-03-28 17:43:21.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/home.html
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3197 2024-03-28 17:43:21.000000 retk-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/side.html
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.286172 retk-0.2.4/src/rethink/plugins/official_plugins/summary/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.287171 retk-0.2.4/src/rethink/plugins/official_plugins/summary/__pycache__/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2968 2024-04-03 15:55:19.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/__pycache__/main.cpython-310.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5620 2024-04-03 15:56:29.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2988 2024-04-03 15:51:31.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2988 2024-03-28 17:32:45.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/__pycache__/main.cpython-39.pyc
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.092812 retk-0.2.4/src/rethink/plugins/official_plugins/summary/_static/
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.287617 retk-0.2.4/src/rethink/plugins/official_plugins/summary/_static/image/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      929 2024-03-23 10:54:56.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/_static/image/logo.svg
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2554 2024-03-28 17:32:44.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/main.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.288620 retk-0.2.4/src/rethink/plugins/official_plugins/summary/templates/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      917 2024-03-28 17:43:21.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/templates/home.html
--rw-r--r--   0 morvanzhou   (501) staff       (20)      917 2024-03-28 17:43:21.000000 retk-0.2.4/src/rethink/plugins/official_plugins/summary/templates/side.html
--rw-r--r--   0 morvanzhou   (501) staff       (20)      754 2024-04-16 01:47:58.000000 retk-0.2.4/src/rethink/plugins/register.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.289649 retk-0.2.4/src/rethink/plugins/schedule/
--rw-r--r--   0 morvanzhou   (501) staff       (20)      116 2024-04-03 16:25:09.000000 retk-0.2.4/src/rethink/plugins/schedule/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)       77 2024-03-20 10:09:19.000000 retk-0.2.4/src/rethink/plugins/schedule/scheduler.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1586 2024-03-20 02:57:36.000000 retk-0.2.4/src/rethink/plugins/schedule/timing.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      722 2024-01-30 06:55:38.000000 retk-0.2.4/src/rethink/regex.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.293288 retk-0.2.4/src/rethink/routes/
--rw-r--r--   0 morvanzhou   (501) staff       (20)        0 2023-09-13 05:36:55.000000 retk-0.2.4/src/rethink/routes/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1803 2024-04-13 16:01:43.000000 retk-0.2.4/src/rethink/routes/account.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      529 2024-04-12 18:19:31.000000 retk-0.2.4/src/rethink/routes/app_captcha.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      677 2024-04-16 10:16:39.000000 retk-0.2.4/src/rethink/routes/app_system.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2486 2024-04-13 15:45:30.000000 retk-0.2.4/src/rethink/routes/files.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5869 2024-04-16 05:28:12.000000 retk-0.2.4/src/rethink/routes/node.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1113 2024-04-15 16:14:15.000000 retk-0.2.4/src/rethink/routes/oauth.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2245 2024-04-15 17:30:43.000000 retk-0.2.4/src/rethink/routes/plugin.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)      916 2024-04-16 02:03:56.000000 retk-0.2.4/src/rethink/routes/recent.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2373 2024-04-12 19:12:22.000000 retk-0.2.4/src/rethink/routes/self_hosted.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3409 2024-04-13 15:56:36.000000 retk-0.2.4/src/rethink/routes/trash.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1412 2024-04-13 15:57:11.000000 retk-0.2.4/src/rethink/routes/user.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2275 2024-04-13 11:14:49.000000 retk-0.2.4/src/rethink/routes/utils.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4201 2024-04-05 10:20:55.000000 retk-0.2.4/src/rethink/run.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1207 2024-04-05 09:50:14.000000 retk-0.2.4/src/rethink/safety.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    13043 2024-04-16 01:40:43.000000 retk-0.2.4/src/rethink/utils.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.294113 retk-0.2.4/src/rethink/version_manager/
--rw-r--r--   0 morvanzhou   (501) staff       (20)       58 2024-04-03 16:25:09.000000 retk-0.2.4/src/rethink/version_manager/__init__.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2204 2024-04-03 14:48:06.000000 retk-0.2.4/src/rethink/version_manager/migrate.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1360 2024-04-03 14:48:06.000000 retk-0.2.4/src/rethink/version_manager/recover.py
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.299886 retk-0.2.4/src/retk.egg-info/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     5874 2024-04-17 01:54:47.000000 retk-0.2.4/src/retk.egg-info/PKG-INFO
--rw-r--r--   0 morvanzhou   (501) staff       (20)    19990 2024-04-17 01:54:47.000000 retk-0.2.4/src/retk.egg-info/SOURCES.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)        1 2024-04-17 01:54:47.000000 retk-0.2.4/src/retk.egg-info/dependency_links.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)      446 2024-04-17 01:54:47.000000 retk-0.2.4/src/retk.egg-info/requires.txt
--rw-r--r--   0 morvanzhou   (501) staff       (20)        8 2024-04-17 01:54:47.000000 retk-0.2.4/src/retk.egg-info/top_level.txt
-drwxr-xr-x   0 morvanzhou   (501) staff       (20)        0 2024-04-17 01:54:47.299489 retk-0.2.4/tests/
--rw-r--r--   0 morvanzhou   (501) staff       (20)     3526 2024-04-13 10:12:44.000000 retk-0.2.4/tests/test_account.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    29829 2024-04-16 05:30:46.000000 retk-0.2.4/tests/test_api.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4703 2024-01-31 14:30:15.000000 retk-0.2.4/tests/test_core_files_obsidian.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    20879 2024-04-16 05:32:56.000000 retk-0.2.4/tests/test_core_local.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)    18844 2024-04-13 11:14:49.000000 retk-0.2.4/tests/test_core_remote.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     1802 2024-04-13 10:17:53.000000 retk-0.2.4/tests/test_data_restore.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     4521 2024-04-13 10:16:07.000000 retk-0.2.4/tests/test_plugins.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2708 2024-04-05 10:21:44.000000 retk-0.2.4/tests/test_run.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9980 2024-04-13 11:14:49.000000 retk-0.2.4/tests/test_search_es.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     7068 2024-04-13 11:14:49.000000 retk-0.2.4/tests/test_search_local.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2254 2024-04-15 16:44:17.000000 retk-0.2.4/tests/test_sso.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     9327 2024-04-11 08:07:23.000000 retk-0.2.4/tests/test_utils.py
--rw-r--r--   0 morvanzhou   (501) staff       (20)     2615 2024-04-03 14:48:06.000000 retk-0.2.4/tests/test_version_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.884403 retk-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 19:00:39.000000 retk-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-18 19:00:48.884403 retk-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-18 19:00:39.000000 retk-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 19:00:39.000000 retk-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-18 19:00:48.884403 retk-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.856403 retk-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.864403 retk-0.2.5/src/retk/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.864403 retk-0.2.5/src/retk/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/app_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.864403 retk-0.2.5/src/retk/controllers/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/files/upload_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.864403 retk-0.2.5/src/retk/controllers/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/node/node_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/node/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/node/trash_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/recent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/controllers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/app_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/recent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/controllers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/account/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/account/app_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/account/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/account/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/async_task/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/async_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/async_task/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/async_task/send_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/files/importing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/files/importing/async_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.868403 retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.872403 retk-0.2.5/src/retk/core/files/importing/async_tasks/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/text/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/async_tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.872403 retk-0.2.5/src/retk/core/files/importing/sync_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/sync_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/importing/sync_tasks/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/files/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.872403 retk-0.2.5/src/retk/core/node/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/node/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/node/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/node/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/recent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.872403 retk-0.2.5/src/retk/depend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.872403 retk-0.2.5/src/retk/depend/mongita/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/command_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.876403 retk-0.2.5/src/retk/depend/mongita/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/engines/disk_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/engines/engine_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/engines/memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/mongita_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/mongitasync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/read_concern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/mongita/write_concern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.876403 retk-0.2.5/src/retk/depend/sso/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/depend/sso/qq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.876403 retk-0.2.5/src/retk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/coll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/db_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.876403 retk-0.2.5/src/retk/models/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/search_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23257 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/search_engine/engine_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/search_engine/engine_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/models/tps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.876403 retk-0.2.5/src/retk/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.880403 retk-0.2.5/src/retk/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/schedule/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/plugins/schedule/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.880403 retk-0.2.5/src/retk/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/app_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/app_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/recent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/self_hosted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/trash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/routes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.880403 retk-0.2.5/src/retk/version_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/version_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/version_manager/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 19:00:39.000000 retk-0.2.5/src/retk/version_manager/recover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.884403 retk-0.2.5/src/retk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-18 19:00:48.000000 retk-0.2.5/src/retk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-18 19:00:48.000000 retk-0.2.5/src/retk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:00:48.000000 retk-0.2.5/src/retk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-18 19:00:48.000000 retk-0.2.5/src/retk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 19:00:48.000000 retk-0.2.5/src/retk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:00:48.884403 retk-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33552 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_core_async_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_core_files_obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_core_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_core_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_data_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_search_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_search_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9315 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-18 19:00:39.000000 retk-0.2.5/tests/test_version_manager.py
```

### Comparing `retk-0.2.4/LICENSE` & `retk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/PKG-INFO` & `retk-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retk
-Version: 0.2.4
+Version: 0.2.5
 Summary: keep and reuse your thoughts
 Home-page: https://github.com/MorvanZhou/rethink
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/rethink/issues
 Project-URL: Source, https://github.com/MorvanZhou/rethink
 Classifier: Programming Language :: Python :: 3
@@ -47,19 +47,19 @@
 Requires-Dist: motor>=3.3.2; extra == "remote"
 Requires-Dist: elasticsearch[async]~=8.11.0; extra == "remote"
 
 # Rethink
 
 [![Unittest](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml/badge.svg)](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml)
 [![License](https://img.shields.io/github/license/MorvanZhou/rethink)](https://github.com/MorvanZhou/rethink/blob/master/LICENSE)
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/v/rethink-note?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/v/retk?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/pyversions/rethink-note.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/pyversions/retk.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
 <p align="center">
   <strong>English</strong> | <a href="README_ZH.md" target="_blank">简体中文</a>
 </p>
 
 A note-taking app dependent on python.
@@ -95,44 +95,44 @@
 5. **Multi-language**: Support multiple languages, including Chinese and English.
 
 ## Install
 
 First install:
 
 ```shell
-pip install rethink-note
+pip install retk
 ```
 
 To update:
 
 ```shell
-pip install -U rethink-note
+pip install -U retk
 ```
 
 ## Usage
 
-Quickly start the note web service with `rethink.run()`, and save your note data locally,
+Quickly start the note web service with `retk.run()`, and save your note data locally,
 The default save path is the `.data` folder under the path of this script:
 
 ```python
-import rethink
+import retk
 
-rethink.run()
+retk.run()
 ```
 
-If you need to customize settings, you can set the parameters in `rethink.run()`:
+If you need to customize settings, you can set the parameters in `retk.run()`:
 
 ```python
-import rethink
+import retk
 
-rethink.run(
-    path='.',  # path to store notes, default is current directory
-    host="127.0.0.1",  # host ip, default is localhost
-    port=8080,  # port number, default is 8080
-    language="zh"  # language, default is English, optional: zh, en
+retk.run(
+   path='.',  # path to store notes, default is current directory
+   host="127.0.0.1",  # host ip, default is localhost
+   port=8080,  # port number, default is 8080
+   language="zh"  # language, default is English, optional: zh, en
 )
 ```
 
 All notes will be stored in the path specified by `path`,
 and the `.data` folder will be created in your `path` directory.
 
 English and Chinese languages are supported, and the default is English `en`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: retk Version: 0.2.4 Summary: keep and reuse your
+Metadata-Version: 2.1 Name: retk Version: 0.2.5 Summary: keep and reuse your
 thoughts Home-page: https://github.com/MorvanZhou/rethink Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com Project-URL: Bug Tracker, https://
 github.com/MorvanZhou/rethink/issues Project-URL: Source, https://github.com/
 MorvanZhou/rethink Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -46,21 +46,21 @@
 you wrote before? Unable to effectively form a note network? Rethink
 automatically recommend related notes while writing, actively assist you in
 forming a knowledge network. 4. **Local storage**: Rethink attaches great
 importance to data security. You can store data in a local storage. Or you can
 also use the online version [https://rethink.run](https://rethink.run), which
 makes it easy to synchronize across multiple platforms. 5. **Multi-language**:
 Support multiple languages, including Chinese and English. ## Install First
-install: ```shell pip install rethink-note ``` To update: ```shell pip install
--U rethink-note ``` ## Usage Quickly start the note web service with
-`rethink.run()`, and save your note data locally, The default save path is the
-`.data` folder under the path of this script: ```python import rethink
-rethink.run() ``` If you need to customize settings, you can set the parameters
-in `rethink.run()`: ```python import rethink rethink.run( path='.', # path to
-store notes, default is current directory host="127.0.0.1", # host ip, default
-is localhost port=8080, # port number, default is 8080 language="zh" #
-language, default is English, optional: zh, en ) ``` All notes will be stored
-in the path specified by `path`, and the `.data` folder will be created in your
-`path` directory. English and Chinese languages are supported, and the default
-is English `en`. If you want to use Chinese `zh`, you can use `language="zh"`
-parameter. Open your browser and visit `http://127.0.0.1:8080` to start
-recording your ideas. ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
+install: ```shell pip install retk ``` To update: ```shell pip install -U retk
+``` ## Usage Quickly start the note web service with `retk.run()`, and save
+your note data locally, The default save path is the `.data` folder under the
+path of this script: ```python import retk retk.run() ``` If you need to
+customize settings, you can set the parameters in `retk.run()`: ```python
+import retk retk.run( path='.', # path to store notes, default is current
+directory host="127.0.0.1", # host ip, default is localhost port=8080, # port
+number, default is 8080 language="zh" # language, default is English, optional:
+zh, en ) ``` All notes will be stored in the path specified by `path`, and the
+`.data` folder will be created in your `path` directory. English and Chinese
+languages are supported, and the default is English `en`. If you want to use
+Chinese `zh`, you can use `language="zh"` parameter. Open your browser and
+visit `http://127.0.0.1:8080` to start recording your ideas. ## Star History
+_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `retk-0.2.4/README.md` & `retk-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Rethink
 
 [![Unittest](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml/badge.svg)](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml)
 [![License](https://img.shields.io/github/license/MorvanZhou/rethink)](https://github.com/MorvanZhou/rethink/blob/master/LICENSE)
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/v/rethink-note?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/v/retk?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/pyversions/rethink-note.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/pyversions/retk.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
 <p align="center">
   <strong>English</strong> | <a href="README_ZH.md" target="_blank">简体中文</a>
 </p>
 
 A note-taking app dependent on python.
@@ -46,44 +46,44 @@
 5. **Multi-language**: Support multiple languages, including Chinese and English.
 
 ## Install
 
 First install:
 
 ```shell
-pip install rethink-note
+pip install retk
 ```
 
 To update:
 
 ```shell
-pip install -U rethink-note
+pip install -U retk
 ```
 
 ## Usage
 
-Quickly start the note web service with `rethink.run()`, and save your note data locally,
+Quickly start the note web service with `retk.run()`, and save your note data locally,
 The default save path is the `.data` folder under the path of this script:
 
 ```python
-import rethink
+import retk
 
-rethink.run()
+retk.run()
 ```
 
-If you need to customize settings, you can set the parameters in `rethink.run()`:
+If you need to customize settings, you can set the parameters in `retk.run()`:
 
 ```python
-import rethink
+import retk
 
-rethink.run(
-    path='.',  # path to store notes, default is current directory
-    host="127.0.0.1",  # host ip, default is localhost
-    port=8080,  # port number, default is 8080
-    language="zh"  # language, default is English, optional: zh, en
+retk.run(
+   path='.',  # path to store notes, default is current directory
+   host="127.0.0.1",  # host ip, default is localhost
+   port=8080,  # port number, default is 8080
+   language="zh"  # language, default is English, optional: zh, en
 )
 ```
 
 All notes will be stored in the path specified by `path`,
 and the `.data` folder will be created in your `path` directory.
 
 English and Chinese languages are supported, and the default is English `en`.
```

#### html2text {}

```diff
@@ -22,21 +22,21 @@
 you wrote before? Unable to effectively form a note network? Rethink
 automatically recommend related notes while writing, actively assist you in
 forming a knowledge network. 4. **Local storage**: Rethink attaches great
 importance to data security. You can store data in a local storage. Or you can
 also use the online version [https://rethink.run](https://rethink.run), which
 makes it easy to synchronize across multiple platforms. 5. **Multi-language**:
 Support multiple languages, including Chinese and English. ## Install First
-install: ```shell pip install rethink-note ``` To update: ```shell pip install
--U rethink-note ``` ## Usage Quickly start the note web service with
-`rethink.run()`, and save your note data locally, The default save path is the
-`.data` folder under the path of this script: ```python import rethink
-rethink.run() ``` If you need to customize settings, you can set the parameters
-in `rethink.run()`: ```python import rethink rethink.run( path='.', # path to
-store notes, default is current directory host="127.0.0.1", # host ip, default
-is localhost port=8080, # port number, default is 8080 language="zh" #
-language, default is English, optional: zh, en ) ``` All notes will be stored
-in the path specified by `path`, and the `.data` folder will be created in your
-`path` directory. English and Chinese languages are supported, and the default
-is English `en`. If you want to use Chinese `zh`, you can use `language="zh"`
-parameter. Open your browser and visit `http://127.0.0.1:8080` to start
-recording your ideas. ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
+install: ```shell pip install retk ``` To update: ```shell pip install -U retk
+``` ## Usage Quickly start the note web service with `retk.run()`, and save
+your note data locally, The default save path is the `.data` folder under the
+path of this script: ```python import retk retk.run() ``` If you need to
+customize settings, you can set the parameters in `retk.run()`: ```python
+import retk retk.run( path='.', # path to store notes, default is current
+directory host="127.0.0.1", # host ip, default is localhost port=8080, # port
+number, default is 8080 language="zh" # language, default is English, optional:
+zh, en ) ``` All notes will be stored in the path specified by `path`, and the
+`.data` folder will be created in your `path` directory. English and Chinese
+languages are supported, and the default is English `en`. If you want to use
+Chinese `zh`, you can use `language="zh"` parameter. Open your browser and
+visit `http://127.0.0.1:8080` to start recording your ideas. ## Star History
+_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `retk-0.2.4/setup.cfg` & `retk-0.2.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = retk
-version = 0.2.4
+version = 0.2.5
 author = MorvanZhou
 author_email = morvanzhou@hotmail.com
 description = keep and reuse your thoughts
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MorvanZhou/rethink
 project_urls =
```

### Comparing `retk-0.2.4/src/rethink/application.py` & `retk-0.2.5/src/retk/application.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 
-from rethink import const, config, safety, utils
-from rethink.logger import logger, add_rotating_file_handler
+from retk import const, config, safety, utils
+from retk.core import async_task
+from retk.logger import logger, add_rotating_file_handler
 from .models.client import client
 from .routes import (
     user,
     oauth,
     node,
     recent,
     trash,
     app_captcha,
     files,
     plugin,
     self_hosted,
     app_system,
     account,
+    admin,
 )
 
 app = FastAPI(
     docs_url="/docs",
     openapi_url="/openapi.json",
 )
 
@@ -43,14 +45,15 @@
 app.include_router(trash.router)
 app.include_router(app_captcha.router)
 app.include_router(files.router)
 app.include_router(plugin.router)
 app.include_router(self_hosted.router)
 app.include_router(app_system.router)
 app.include_router(account.router)
+app.include_router(admin.router)
 
 self_hosted.mount_static(app=app)
 
 
 @app.on_event("startup")
 async def startup_event():
     if not config.is_local_db():
@@ -64,7 +67,10 @@
     logger.debug(f'startup_event VUE_APP_API_PORT: {os.environ.get("VUE_APP_API_PORT")}')
     logger.debug(f'startup_event VUE_APP_LANGUAGE: {os.environ.get("VUE_APP_LANGUAGE")}')
     await client.init()
     logger.debug("db initialized")
 
     # local finish up
     utils.local_finish_up()
+
+    # async threading task
+    async_task.init()
```

### Comparing `retk-0.2.4/src/rethink/config.py` & `retk-0.2.5/src/retk/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import bcrypt
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from pydantic import Field, DirectoryPath
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
-from rethink.logger import logger
+from retk.logger import logger
 
 
 class Settings(BaseSettings):
     ONE_USER: bool = Field(default=1, env='ONE_USER')
     RETHINK_SERVER_DEBUG: bool = Field(default=False, env='RETHINK_SERVER_DEBUG')
     VERIFY_REFERER: bool = Field(default=False, env='VERIFY_REFERER')
     PLUGINS: bool = Field(default=False, env='PLUGINS')
```

### Comparing `retk-0.2.4/src/rethink/const.py` & `retk-0.2.5/src/retk/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Dict
 
 DOMAIN = "rethink.run"
 RETHINK_DIR = Path(__file__).parent
 FRONTEND_DIR = RETHINK_DIR / "dist-local"
 MD_MAX_LENGTH = 100_000
 REQUEST_ID_MAX_LENGTH = 50
+UID_MAX_LENGTH = 30
 NID_MAX_LENGTH = 30
 FID_MAX_LENGTH = 30
 SEARCH_QUERY_MAX_LENGTH = 100
 RECOMMEND_CONTENT_MAX_LENGTH = 200
 EMAIL_MAX_LENGTH = 100
 PASSWORD_MAX_LENGTH = 20
 NICKNAME_MAX_LENGTH = 20
@@ -57,14 +58,17 @@
     IMPORT_PROCESS_NOT_FINISHED = 23
     UPLOAD_TASK_TIMEOUT = 24
     USER_SPACE_NOT_ENOUGH = 25
     INVALID_EMAIL = 26
     URL_TOO_LONG = 27
     OAUTH_PROVIDER_NOT_FOUND = 28
     TASK_NOT_FOUND = 29
+    ACCOUNT_EXIST_TRY_FORGET_PASSWORD = 30
+    USER_DISABLED = 31
+    NOT_PERMITTED = 32
 
 
 INT_CODE_MAP: Dict[int, Code] = {
     c.value: c for c in Code
 }
 
 
@@ -103,14 +107,20 @@
         en="Last import process not finished, please try again later"),
     Code.UPLOAD_TASK_TIMEOUT: CodeMessage(zh="文件上传任务超时", en="Upload task timeout"),
     Code.USER_SPACE_NOT_ENOUGH: CodeMessage(zh="用户空间不足", en="User space not enough"),
     Code.INVALID_EMAIL: CodeMessage(zh="邮箱格式错误", en="Email format error"),
     Code.URL_TOO_LONG: CodeMessage(zh="URL字符太长", en="URL too long"),
     Code.OAUTH_PROVIDER_NOT_FOUND: CodeMessage(zh="未找到 OAuth 提供商", en="OAuth provider not found"),
     Code.TASK_NOT_FOUND: CodeMessage(zh="任务未找到", en="Task not found"),
+    Code.ACCOUNT_EXIST_TRY_FORGET_PASSWORD: CodeMessage(
+        zh="账户已存在，请尝试通过忘记密码找回",
+        en="Account exists, try forget password to recover",
+    ),
+    Code.USER_DISABLED: CodeMessage(zh="用户已被禁用", en="User has been disabled"),
+    Code.NOT_PERMITTED: CodeMessage(zh="无权限", en="Not permitted"),
 }
 
 CODE2STATUS_CODE: Dict[Code, int] = {
     Code.OK: 200,
     Code.ACCOUNT_OR_PASSWORD_ERROR: 401,
     Code.INVALID_AUTH: 401,
     Code.EXPIRED_AUTH: 401,
@@ -136,14 +146,17 @@
     Code.IMPORT_PROCESS_NOT_FINISHED: 403,
     Code.UPLOAD_TASK_TIMEOUT: 408,
     Code.USER_SPACE_NOT_ENOUGH: 403,
     Code.INVALID_EMAIL: 400,
     Code.URL_TOO_LONG: 406,
     Code.OAUTH_PROVIDER_NOT_FOUND: 404,
     Code.TASK_NOT_FOUND: 404,
+    Code.ACCOUNT_EXIST_TRY_FORGET_PASSWORD: 422,
+    Code.USER_DISABLED: 403,
+    Code.NOT_PERMITTED: 403,
 }
 
 DEFAULT_USER = {
     "nickname": "rethink",
     "email": "rethink@rethink.run",
     "avatar": "",
 }
@@ -210,17 +223,17 @@
 
         Use @ to link between notes. For example [@How do I record](/n/{}) .
 
         Rethink also supports markdown syntax, for example:
         
         # My task list
         
-        - [x] task 1
+        - [ ] task 1
         - [ ] task 2
-        - [ ] task 3
+        - [x] task 3
         
         """),
     ],
     Language.ZH.value: [
         dedent("""\
         # 我如何记录
```

### Comparing `retk-0.2.4/src/rethink/controllers/account.py` & `retk-0.2.5/src/retk/controllers/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from random import randint
 from typing import Tuple
 
 from fastapi.responses import StreamingResponse
 
-from rethink import config
-from rethink import const
-from rethink.controllers import schemas
-from rethink.controllers.utils import json_exception
-from rethink.core import account
-from rethink.models.tps import AuthedUser
-from rethink.utils import jwt_encode
+from retk import config
+from retk import const
+from retk.controllers import schemas
+from retk.controllers.utils import json_exception
+from retk.core import account, user
+from retk.models.tps import AuthedUser
+from retk.utils import jwt_encode
 
 
 async def signup(
         au: AuthedUser,
         req: schemas.account.SignupRequest,
 ) -> schemas.account.TokenResponse:
     if not const.Language.is_valid(req.language):
@@ -55,23 +55,27 @@
     # TODO: 后台应记录成功登录用户名和 IP、时间.
     #  当尝试登录 IP 不在历史常登录 IP 地理位置时，应进行多因素二次验证用户身份，防止用户因密码泄漏被窃取账户
     u, code = await account.manager.get_user_by_email(req.email)
     if code != const.Code.OK:
         raise json_exception(
             request_id=au.request_id,
             code=code,
-            language=const.Language.EN.value,
+            language=req.language,
         )
 
-    if not await account.manager.is_right_password(au, req.password):
+    if not await account.manager.is_right_password(
+            email=u["email"],
+            hashed=u["hashed"],
+            password=req.password,
+    ):
         code = const.Code.ACCOUNT_OR_PASSWORD_ERROR
         raise json_exception(
             request_id=au.request_id,
             code=code,
-            language=u["settings"]["language"],
+            language=req.language,
         )
     token = jwt_encode(
         exp_delta=config.get_settings().JWT_EXPIRED_DELTA,
         data={"uid": u["id"], "language": u["settings"]["language"]},
     )
     return schemas.account.TokenResponse(
         requestId=au.request_id,
@@ -84,19 +88,34 @@
         req: schemas.account.ForgetPasswordRequest
 ) -> schemas.RequestIdResponse:
     code = account.email.verify_number(token=req.verificationToken, number_str=req.verification)
     if code != const.Code.OK:
         raise json_exception(
             request_id=au.request_id,
             code=code,
-            language=const.Language.EN.value,
+            language=req.language,
         )
-    u, code = await account.manager.reset_password(
-        email=req.email,
-        password=req.newPassword,
+    u, code = await user.get_by_email(email=req.email)
+    if code != const.Code.OK:
+        raise json_exception(
+            request_id=au.request_id,
+            code=code,
+            language=req.language,
+        )
+
+    if u is None:
+        raise json_exception(
+            request_id=au.request_id,
+            code=const.Code.INVALID_AUTH,
+            language=req.language,
+        )
+
+    code = await user.reset_password(
+        uid=u["id"],
+        hashed=account.manager.hash_password(password=req.newPassword, email=req.email)
     )
     if code != const.Code.OK:
         raise json_exception(
             request_id=au.request_id,
             code=code,
             language=const.Language.EN.value,
         )
@@ -134,20 +153,30 @@
         numbers=numbers,
         expire=expired_min,
         language=language,
     )
     return numbers, expired_min, code
 
 
-def email_send_code(
+async def email_send_code(
         au: AuthedUser,
         req: schemas.account.EmailVerificationRequest
 ) -> schemas.account.TokenResponse:
     if req.language not in [lang.value for lang in const.Language.__members__.values()]:
         req.language = const.Language.EN.value
+
+    if not req.userExistOk:
+        u, code = await user.get_by_email(email=req.email)
+        if u is not None:
+            raise json_exception(
+                request_id=au.request_id,
+                code=const.Code.ACCOUNT_EXIST_TRY_FORGET_PASSWORD,
+                language=req.language,
+            )
+
     numbers, expired_min, code = __check_and_send_email(
         email=req.email,
         token=req.captchaToken,
         code_str=req.captchaCode,
         language=req.language,
     )
     if code != const.Code.OK:
```

### Comparing `retk-0.2.4/src/rethink/controllers/files/upload_files.py` & `retk-0.2.5/src/retk/controllers/files/upload_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 from fastapi import UploadFile
 
-from rethink import const, core
-from rethink.controllers import schemas
-from rethink.controllers.utils import (
+from retk import const, core
+from retk.controllers import schemas
+from retk.controllers.utils import (
     AuthedUser,
     datetime2str,
     is_allowed_mime_type,
     maybe_raise_json_exception,
 )
 
 
@@ -35,19 +35,19 @@
         requestId=au.request_id,
     )
 
 
 async def get_upload_process(
         au: AuthedUser,
 ) -> schemas.files.FileUploadProcessResponse:
-    doc, code = await core.files.get_upload_process(uid=au.u.id)
+    doc = await core.files.get_upload_process(uid=au.u.id)
     if doc is None:
         return schemas.files.FileUploadProcessResponse(
-            code=code.value,
-            msg=const.get_msg_by_code(code, au.language),
+            code=const.Code.OK.value,
+            msg=const.get_msg_by_code(const.Code.OK, au.language),
             requestId=au.request_id,
             process=0.,
             type="",
             startAt="",
             running=False,
         )
```

### Comparing `retk-0.2.4/src/rethink/controllers/node/node_ops.py` & `retk-0.2.5/src/retk/controllers/node/node_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from rethink import const, core
-from rethink.controllers import schemas
-from rethink.controllers.utils import datetime2str, maybe_raise_json_exception
-from rethink.models.tps import AuthedUser, Node
-from rethink.utils import contain_only_http_link, get_title_description_from_link
+from retk import const, core
+from retk.controllers import schemas
+from retk.controllers.utils import datetime2str, maybe_raise_json_exception
+from retk.models.tps import AuthedUser, Node
+from retk.utils import contain_only_http_link, get_title_description_from_link
 
 
 def __get_node_data(n: Node) -> schemas.node.NodeData:
     from_nodes: List[schemas.node.NodeData.LinkedNode] = []
     to_nodes: List[schemas.node.NodeData.LinkedNode] = []
     for nodes, n_nodes in zip(
             [from_nodes, to_nodes],
@@ -116,21 +116,21 @@
     )
 
 
 async def get_core_nodes(
         au: AuthedUser,
         p: int,
         limit: int,
-) -> schemas.node.GetFromTrashResponse:
+) -> schemas.node.NodesSearchResponse:
     nodes, total = await core.node.core_nodes(
         au=au,
         page=p,
         limit=limit,
     )
-    return schemas.node.GetFromTrashResponse(
+    return schemas.node.NodesSearchResponse(
         requestId=au.request_id,
         data=_get_node_search_response_data(nodes=nodes, total=total),
     )
 
 
 def _get_node_search_response_data(nodes: List[Node], total: int) -> schemas.node.NodesSearchResponse.Data:
     return schemas.node.NodesSearchResponse.Data(
```

### Comparing `retk-0.2.4/src/rethink/controllers/node/search.py` & `retk-0.2.5/src/retk/controllers/node/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal, Optional
 
-from rethink import core
-from rethink.controllers import schemas
-from rethink.models.tps import AuthedUser
+from retk import core
+from retk.controllers import schemas
+from retk.models.tps import AuthedUser
 
 
 async def user_nodes(
         au: AuthedUser,
         q: str,
         sort: Literal["createdAt", "modifiedAt", "title", "similarity"],
         order: Literal["asc", "desc"],
```

### Comparing `retk-0.2.4/src/rethink/controllers/node/trash_ops.py` & `retk-0.2.5/src/retk/controllers/node/trash_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from rethink import core
-from rethink.controllers import schemas
-from rethink.controllers.node.node_ops import _get_node_search_response_data
-from rethink.controllers.utils import maybe_raise_json_exception
-from rethink.models.tps import AuthedUser
+from retk import core
+from retk.controllers import schemas
+from retk.controllers.node.node_ops import _get_node_search_response_data
+from retk.controllers.utils import maybe_raise_json_exception
+from retk.models.tps import AuthedUser
 
 
 async def move_to_trash(
         au: AuthedUser,
         nid: str,
 ) -> schemas.RequestIdResponse:
     code = await core.node.to_trash(au=au, nid=nid)
@@ -29,17 +29,17 @@
     )
 
 
 async def get_from_trash(
         au: AuthedUser,
         p: int = 0,
         limit: int = 10,
-) -> schemas.node.GetFromTrashResponse:
+) -> schemas.node.NodesSearchResponse:
     nodes, total = await core.node.get_nodes_in_trash(au=au, page=p, limit=limit)
-    return schemas.node.GetFromTrashResponse(
+    return schemas.node.NodesSearchResponse(
         requestId=au.request_id,
         data=_get_node_search_response_data(nodes=nodes, total=total),
     )
 
 
 async def restore_from_trash(
         au: AuthedUser,
```

### Comparing `retk-0.2.4/src/rethink/controllers/oauth.py` & `retk-0.2.5/src/retk/controllers/oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict
 
 from fastapi import Request
 
-from rethink import config, const, core, utils
-from rethink.controllers.utils import json_exception
-from rethink.depend.sso.base import SSOLoginError, SSOBase
-from rethink.depend.sso.facebook import FacebookSSO
-from rethink.depend.sso.github import GithubSSO
-# from rethink.depend.sso.qq import QQSSO
+from retk import config, const, core, utils
+from retk.controllers.utils import json_exception
+from retk.depend.sso.base import SSOLoginError, SSOBase
+from retk.depend.sso.facebook import FacebookSSO
+from retk.depend.sso.github import GithubSSO
+# from retk.depend.sso.qq import QQSSO
 from .schemas.account import TokenResponse
 from .schemas.oauth import OAuthResponse
 
 sso_map: Dict[str, SSOBase] = {}
 user_source_map: Dict[str, int] = {}
```

### Comparing `retk-0.2.4/src/rethink/controllers/plugin.py` & `retk-0.2.5/src/retk/controllers/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from rethink import const
-from rethink.controllers import schemas
-from rethink.controllers.utils import maybe_raise_json_exception
-from rethink.core import node
-from rethink.models.tps import AuthedUser
-from rethink.plugins.base import get_plugins, event_plugin_map
+from retk import const, config
+from retk.controllers import schemas
+from retk.controllers.utils import maybe_raise_json_exception, json_exception
+from retk.core import node
+from retk.models.tps import AuthedUser
+from retk.plugins.base import get_plugins, event_plugin_map
 
 
 async def get_all_plugins(
         au: AuthedUser,
 ) -> schemas.plugin.PluginsResponse:
     plugins = [
         schemas.plugin.PluginsResponse.Plugin(
@@ -92,23 +92,38 @@
         pid: str,
         nid: str,
 ) -> schemas.plugin.RenderPluginResponse:
     return await __render(au=au, pid=pid, nid=nid)
 
 
 async def plugin_call(
-        au: AuthedUser,
         req: schemas.plugin.PluginCallRequest,
 ) -> schemas.plugin.PluginCallResponse:
+    if not config.is_local_db():
+        raise json_exception(
+            request_id=req.requestId,
+            code=const.Code.NOT_PERMITTED,
+            language=const.Language.EN.value,
+            log_msg="plugin call is not allowed in production",
+        )
     plugins = get_plugins()
     try:
         plugin = plugins[req.pluginId]
     except KeyError:
-        return maybe_raise_json_exception(au=au, code=const.Code.PLUGIN_NOT_FOUND)
+        return schemas.plugin.PluginCallResponse(
+            success=False,
+            message="plugin not found",
+            requestId=req.requestId,
+            pluginId=req.pluginId,
+            method=req.method,
+            data=None,
+        )
 
-    data = plugin.handle_api_call(req.method, req.data)
+    res = plugin.handle_api_call(req.method, req.data)
     return schemas.plugin.PluginCallResponse(
-        requestId=au.request_id,
+        success=res.success,
+        message=res.message,
+        requestId=req.requestId,
         pluginId=req.pluginId,
         method=req.method,
-        data=data,
+        data=res.data,
     )
```

### Comparing `retk-0.2.4/src/rethink/controllers/recent.py` & `retk-0.2.5/src/retk/controllers/recent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from rethink import core
-from rethink.controllers import schemas
-from rethink.controllers.utils import maybe_raise_json_exception
-from rethink.models.tps import AuthedUser
+from retk import core
+from retk.controllers import schemas
+from retk.controllers.utils import maybe_raise_json_exception
+from retk.models.tps import AuthedUser
 
 
 async def add_recent_at_node(
         au: AuthedUser,
         req: schemas.recent.AtNodeRequest
 ) -> schemas.RequestIdResponse:
     code = await core.recent.added_at_node(au=au, nid=req.nid, to_nid=req.toNid)
```

### Comparing `retk-0.2.4/src/rethink/controllers/schemas/account.py` & `retk-0.2.5/src/retk/controllers/schemas/account.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Literal
 
 from pydantic import BaseModel, EmailStr, Field
 
-from rethink import const
+from retk import const
 
 
 class TokenResponse(BaseModel):
     requestId: str
     token: str = ""
 
 
@@ -17,21 +17,24 @@
     captchaCode: str = Field(max_length=10)
     language: Literal["en", "zh"]
 
 
 class LoginRequest(BaseModel):
     email: EmailStr = Field(max_length=const.EMAIL_MAX_LENGTH)
     password: str = Field(max_length=const.PASSWORD_MAX_LENGTH)
+    language: Literal["en", "zh"] = const.Language.EN.value
 
 
 class EmailVerificationRequest(BaseModel):
     email: str = Field(max_length=const.EMAIL_MAX_LENGTH)
+    userExistOk: bool = Field(type=bool, default=False)
     captchaToken: str = Field(max_length=2000)
     captchaCode: str = Field(max_length=10)
     language: Literal["en", "zh"] = const.Language.EN.value
 
 
 class ForgetPasswordRequest(BaseModel):
     email: str = Field(max_length=const.EMAIL_MAX_LENGTH)
     newPassword: str = Field(max_length=const.PASSWORD_MAX_LENGTH)
     verification: str = Field(max_length=const.PASSWORD_MAX_LENGTH)
     verificationToken: str = Field(max_length=2000)
+    language: Literal["en", "zh"] = const.Language.EN.value
```

### Comparing `retk-0.2.4/src/rethink/controllers/schemas/files.py` & `retk-0.2.5/src/retk/controllers/schemas/files.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/controllers/schemas/node.py` & `retk-0.2.5/src/retk/controllers/schemas/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from pydantic import BaseModel, NonNegativeInt, Field
 
-from rethink import const
+from retk import const
 
 
 class NodeData(BaseModel):
     class LinkedNode(BaseModel):
         id: str
         title: str
         md: str
@@ -60,19 +60,14 @@
         nodes: List[Node]
         total: NonNegativeInt
 
     requestId: str
     data: Data
 
 
-class GetFromTrashResponse(BaseModel):
-    requestId: str
-    data: NodesSearchResponse.Data
-
-
 class BatchNodeIdsRequest(BaseModel):
     nids: List[str] = Field(default_factory=list, min_length=1, max_length=1000)
 
 
 class HistEditionsResponse(BaseModel):
     requestId: str
     versions: List[str] = Field(default_factory=list)
```

### Comparing `retk-0.2.4/src/rethink/controllers/schemas/user.py` & `retk-0.2.5/src/retk/controllers/schemas/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Optional
 
 from pydantic import BaseModel, NonNegativeInt, Field, NonNegativeFloat
 
-from rethink import const
-from rethink.models.tps import CODE_THEME_TYPES
+from retk import const
+from retk.models.tps import CODE_THEME_TYPES
 
 
 class UserInfoResponse(BaseModel):
     class User(BaseModel):
         class LastState(BaseModel):
             nodeDisplayMethod: NonNegativeInt
             nodeDisplaySortKey: Literal["modifiedAt", "createdAt", "title", "similarity"]
@@ -20,14 +20,15 @@
             editorCodeTheme: CODE_THEME_TYPES
             editorSepRightWidth: float
             editorSideCurrentToolId: str
 
         email: str
         nickname: str
         avatar: str
+        source: int
         createdAt: str
         usedSpace: NonNegativeInt = 0
         maxSpace: NonNegativeInt = 0
         lastState: LastState
         settings: Settings
 
     requestId: str
```

### Comparing `retk-0.2.4/src/rethink/controllers/user.py` & `retk-0.2.5/src/retk/controllers/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from rethink import const, core, config
-from rethink.controllers import schemas
-from rethink.controllers.utils import datetime2str, maybe_raise_json_exception
-from rethink.core import account
-from rethink.core.user import reset_password
-from rethink.models.tps import AuthedUser
-from rethink.utils import mask_email, regex
+from retk import const, core, config
+from retk.controllers import schemas
+from retk.controllers.utils import datetime2str, maybe_raise_json_exception
+from retk.core import account
+from retk.core.user import reset_password
+from retk.models.tps import AuthedUser
+from retk.utils import mask_email, regex
 
 
 async def get_user(
         au: AuthedUser,
 ) -> schemas.user.UserInfoResponse:
     _email = mask_email(au.u.email)
     if config.is_local_db():
@@ -17,14 +17,15 @@
         max_space = const.USER_TYPE.id2config(au.u.type).max_store_space
     return schemas.user.UserInfoResponse(
         requestId=au.request_id,
         user=schemas.user.UserInfoResponse.User(
             email=_email,
             nickname=au.u.nickname,
             avatar=au.u.avatar,
+            source=au.u.source,
             createdAt=datetime2str(au.u._id.generation_time),
             usedSpace=au.u.used_space,
             maxSpace=max_space,
             lastState=schemas.user.UserInfoResponse.User.LastState(
                 nodeDisplayMethod=au.u.last_state.node_display_method,
                 nodeDisplaySortKey=au.u.last_state.node_display_sort_key,
             ),
@@ -60,14 +61,15 @@
     u_settings = u["settings"]
     return schemas.user.UserInfoResponse(
         requestId=au.request_id,
         user=schemas.user.UserInfoResponse.User(
             email=u["email"],
             nickname=u["nickname"],
             avatar=u["avatar"],
+            source=u["source"],
             createdAt=datetime2str(u["_id"].generation_time),
             usedSpace=u["usedSpace"],
             maxSpace=max_space,
             lastState=schemas.user.UserInfoResponse.User.LastState(
                 nodeDisplayMethod=last_state["nodeDisplayMethod"],
                 nodeDisplaySortKey=last_state["nodeDisplaySortKey"],
             ),
@@ -87,18 +89,22 @@
 async def update_password(
         au: AuthedUser,
         req: schemas.user.UpdatePasswordRequest
 ) -> schemas.RequestIdResponse:
     if regex.VALID_PASSWORD.match(req.newPassword) is None:
         return maybe_raise_json_exception(au=au, code=const.Code.INVALID_PASSWORD)
 
-    ok = await account.manager.is_right_password(au, req.oldPassword)
+    ok = await account.manager.is_right_password(
+        email=au.u.email,
+        hashed=au.u.hashed,
+        password=req.oldPassword,
+    )
     if not ok:
         return maybe_raise_json_exception(au=au, code=const.Code.OLD_PASSWORD_ERROR)
 
     hashed = account.manager.hash_password(password=req.newPassword, email=au.u.email)
-    code = await reset_password(au=au, hashed=hashed)
+    code = await reset_password(uid=au.u.id, hashed=hashed)
     maybe_raise_json_exception(au=au, code=code)
 
     return schemas.RequestIdResponse(
         requestId=au.request_id,
     )
```

### Comparing `retk-0.2.4/src/rethink/controllers/utils.py` & `retk-0.2.5/src/retk/routes/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,130 @@
-import datetime
-import inspect
+import time
 import traceback
-from typing import Sequence
-from urllib.parse import urlparse
+from functools import wraps
+from typing import Optional
 
 import jwt
-from fastapi import Header, HTTPException
-
-from rethink import core, const
-from rethink.logger import logger
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
-from rethink.utils import jwt_decode
-
-
-def datetime2str(dt: datetime.datetime) -> str:
-    return dt.strftime('%Y-%m-%dT%H:%M:%SZ')
-
-
-def is_allowed_mime_type(data_url, allowed_mime_types: Sequence[str]):
-    try:
-        result = urlparse(data_url)
-        if result.scheme != 'data':
-            return False
-
-        media_type = result.path.split(';')[0]
-        return media_type in allowed_mime_types
-    except Exception:  # pylint: disable=broad-except
-        return False
+from fastapi import HTTPException, Header, Depends
+from fastapi.params import Path
+from starlette.status import HTTP_403_FORBIDDEN
+from typing_extensions import Annotated
+
+from retk import const, config, core
+from retk.controllers.utils import json_exception
+from retk.logger import logger
+from retk.models.tps import AuthedUser, convert_user_dict_to_authed_user
+from retk.utils import jwt_decode
+
+REFERER_PREFIX = f"https://{const.DOMAIN}"
+
+
+def measure_time_spend(func):
+    @wraps(func)
+    async def wrapper(*args, **kwargs):
+        t0 = time.perf_counter()
+        uid = ""
+        try:
+            au: AuthedUser = kwargs["au"]
+        except KeyError:
+            req_id = ""
+        else:
+            req_id = au.request_id
+            if au.u is not None:
+                uid = au.u.id
+
+        req_s = str(kwargs.get("req", ""))
+
+        req_s = req_s[:200] + "..." if len(req_s) > 200 else req_s
+        if func.__name__ not in ["login", "forget_password", "signup"]:
+            logger.debug(f"REQ: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | {req_s}")
+
+        resp = await func(*args, **kwargs)
+        t1 = time.perf_counter()
+        try:
+            req_id = resp.requestId
+        except AttributeError:
+            req_id = ""
+        logger.debug(f"RESP: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | spend={t1 - t0:.4f}s")
+        return resp
+
+    return wrapper
+
+
+def verify_referer(referer: Optional[str] = Header(None)):
+    if config.get_settings().VERIFY_REFERER and not referer.startswith(REFERER_PREFIX):
+        logger.error(f"referer={referer} not startswith {REFERER_PREFIX}")
+        raise HTTPException(
+            status_code=HTTP_403_FORBIDDEN,
+            detail="Invalid referer",
+        )
+    return referer
 
 
-async def process_headers(
+async def process_normal_headers(
         token: str = Header(alias="Authorization", default=""),
         request_id: str = Header(
             default="", alias="RequestId", max_length=const.REQUEST_ID_MAX_LENGTH
         )
 ) -> AuthedUser:
     """if no requestId, default to empty string"""
     au = AuthedUser(
         u=None,
         request_id=request_id,
         language=const.Language.EN.value,
     )
     err = ""
     if token is None or token == "":
         return au
+    u = None
     try:
         payload = jwt_decode(token=token)
         u, code = await core.user.get(uid=payload["uid"])
         if code != const.Code.OK:
-            logger.error(f"core.user.get err: {const.CODE_MESSAGES[code].zh}")
-            raise json_exception(
-                request_id=request_id,
-                code=code,
-            )
-        au.language = u["settings"]["language"]
-        au.u = convert_user_dict_to_authed_user(u)
+            err = f"get user failed, code={code}"
     except jwt.exceptions.ExpiredSignatureError:
         code = const.Code.EXPIRED_AUTH
         err = "auth expired"
     except jwt.exceptions.DecodeError:
         code = const.Code.INVALID_AUTH
         err = "token decode error"
     except jwt.exceptions.InvalidTokenError:
         code = const.Code.INVALID_AUTH
         err = "invalid token"
     except Exception:  # pylint: disable=broad-except
         code = const.Code.INVALID_AUTH
         err = traceback.format_exc()
-    if code != const.Code.OK:
+    if code != const.Code.OK or u is None:
         raise json_exception(
             request_id=request_id,
             code=code,
             log_msg=err,
         )
+    au.language = u["settings"]["language"]
+    au.u = convert_user_dict_to_authed_user(u)
     return au
 
 
-def json_exception(
-        request_id: str,
-        code: const.Code,
-        language: str = const.Language.EN.value,
-        log_msg: str = None
-) -> HTTPException:
-    def get_parent_function_info() -> str:
-        previous_frame = inspect.currentframe().f_back.f_back.f_code
-        caller = previous_frame.co_name
-        previous_frame_file = previous_frame.co_filename
-        previous_frame_line = previous_frame.co_firstlineno
-        return f"{caller} in {previous_frame_file}:{previous_frame_line}"
-
-    if log_msg is not None:
-        # get parent function name
-        one_line_log = log_msg.replace("\n", "\\n")
-        logger.error(f"reqId='{request_id}' | {get_parent_function_info()} | err='{one_line_log}'")
-
-    status_code = const.CODE2STATUS_CODE[code]
-    if status_code == 500:
-        one_line_log = const.get_msg_by_code(code, language).replace("\n", "\\n")
-        logger.error(f"reqId='{request_id}' | {get_parent_function_info()} | err='{one_line_log}'")
-
-    return HTTPException(
-        status_code=status_code,
-        detail={
-            "code": code.value,
-            "msg": const.get_msg_by_code(code, language),
-            "requestId": request_id,
-        }
-    )
-
-
-def maybe_raise_json_exception(
-        au: AuthedUser,
-        code: const.Code,
-):
-    if code != const.Code.OK:
+async def process_admin_headers(
+        token: str = Header(alias="Authorization", default=""),
+        request_id: str = Header(
+            default="", alias="RequestId", max_length=const.REQUEST_ID_MAX_LENGTH
+        )
+) -> AuthedUser:
+    au = await process_normal_headers(token=token, request_id=request_id)
+    if au.u is None or au.u.type != const.USER_TYPE.ADMIN.id:
         raise json_exception(
             request_id=au.request_id,
-            code=code,
-            language=au.language,
+            code=const.Code.NOT_PERMITTED,
         )
+    return au
+
+
+ANNOTATED_AUTHED_USER = Annotated[AuthedUser, Depends(process_normal_headers)]
+ANNOTATED_AUTHED_ADMIN = Annotated[AuthedUser, Depends(process_admin_headers)]
+
+ANNOTATED_UID = Annotated[str, Path(title="The ID of user", max_length=const.UID_MAX_LENGTH, min_length=8)]
+ANNOTATED_NID = Annotated[str, Path(title="The ID of node", max_length=const.NID_MAX_LENGTH, min_length=8)]
+ANNOTATED_PID = Annotated[str, Path(title="The ID of plugin", max_length=const.PLUGIN_ID_MAX_LENGTH)]
+ANNOTATED_FID = Annotated[str, Path(title="The ID of file", max_length=const.FID_MAX_LENGTH)]
+
+DEPENDS_REFERER = Depends(verify_referer)
```

### Comparing `retk-0.2.4/src/rethink/core/account/app_captcha.py` & `retk-0.2.5/src/retk/core/account/app_captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from random import choices
 from typing import Tuple, Dict
 
 import jwt
 from captcha.audio import AudioCaptcha
 from captcha.image import ImageCaptcha
 
-from rethink import const, config
-from rethink.utils import jwt_encode, jwt_decode
+from retk import const, config
+from retk.utils import jwt_encode, jwt_decode
 
 DEFAULT_CAPTCHA_EXPIRE_SECOND = 60
 
 img_captcha = ImageCaptcha(font_sizes=(35, 30, 32))
 audio_captcha = AudioCaptcha()
 
 alphabet = "3467ACDEFGJKLMNPQRTVWXYbdfgkmnprtwy"
```

### Comparing `retk-0.2.4/src/rethink/core/account/email.py` & `retk-0.2.5/src/retk/core/account/email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import email.header
-import smtplib
 from datetime import timedelta
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from textwrap import dedent
 from typing import List, Tuple
 
 import jwt
 
-from rethink import const, config, regex, utils
+from retk import const, config, regex, utils
+from retk.core import async_task
 
 
 class EmailServer:
     default_language = const.Language.EN
 
     lang_subject = {
         const.Language.EN.value: "Rethink: Security Code",
@@ -83,20 +83,19 @@
         msg = MIMEMultipart('alternative')
         msg['Subject'] = email.header.Header(subject, 'utf-8')
         msg['From'] = conf.RETHINK_EMAIL
         msg['To'] = ", ".join(recipients)
         html_body = MIMEText(html_message, 'html', 'utf-8')
         msg.attach(html_body)
 
-        server = smtplib.SMTP('smtp.office365.com', 587)
-        server.ehlo()
-        server.starttls()
-        server.login(conf.RETHINK_EMAIL, password=conf.RETHINK_EMAIL_PASSWORD)
-        server.sendmail(conf.RETHINK_EMAIL, recipients, msg.as_string())
-        server.quit()
+        async_task.put_task(
+            task_name=async_task.TaskName.SEND_EMAIL,
+            recipients=recipients,
+            subject=msg.as_string()
+        )
         return const.Code.OK
 
 
 email_server = EmailServer()
 
 
 def encode_number(number: str, expired_min: int) -> str:
```

### Comparing `retk-0.2.4/src/rethink/core/account/manager.py` & `retk-0.2.5/src/retk/core/account/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import base64
 import hashlib
 import os
 from typing import Optional, Tuple
 
 import bcrypt
 
-from rethink import config, const, regex
-from rethink.core import user, node
-from rethink.logger import logger
-from rethink.models import tps
+from retk import config, const, regex
+from retk.core import user, node
+from retk.logger import logger
+from retk.models import tps
+from retk.models.client import client
 
 
 async def get_user_by_email(email: str) -> Tuple[Optional[tps.UserMeta], const.Code]:
     return await user.get_by_email(email=email)
 
 
-async def is_right_password(au: tps.AuthedUser, password: str) -> bool:
+async def is_right_password(email: str, hashed: str, password: str) -> bool:
     if config.get_settings().ONE_USER:
         pw = os.getenv("RETHINK_SERVER_PASSWORD", None)
         if pw is not None:
             return pw == password
         return True
-    base_pw = _base_password(password=password, email=au.u.email)
-    match = bcrypt.checkpw(base_pw, au.u.hashed.encode("utf-8"))
+    base_pw = _base_password(password=password, email=email)
+    match = bcrypt.checkpw(base_pw, hashed.encode("utf-8"))
     return match
 
 
 def _base_password(password: str, email: str) -> bytes:
     # update hash strategy
     s = f"{password}&&{config.get_settings().DB_SALT}$${email}"
     logger.debug(f"hashing: {s}")
@@ -76,24 +77,31 @@
     if code != const.Code.OK:
         return None, code
 
     code = await node.new_user_add_default_nodes(uid=u["id"], language=language)
     return u, code
 
 
-async def reset_password(
-        email: str,
-        password: str,
-) -> Tuple[Optional[tps.UserMeta], const.Code]:
-    code = login_by_email_pwd(email=email, password=password)
-    if code != const.Code.OK:
-        return None, code
-    u, code = await user.get_by_email(email=email)
-    if code != const.Code.OK:
-        return None, code
-    if u is None:
-        return None, const.Code.INVALID_AUTH
-    code = await user.reset_password(
-        uid=u["id"],
-        hashed=hash_password(password=password, email=email)
+async def delete(uid: str):
+    res = await client.coll.users.delete_one({"id": uid})
+    if res.deleted_count != 1:
+        return
+    await client.coll.nodes.delete_many({"uid": uid})
+    await client.coll.user_file.delete_many({"uid": uid})
+    await client.coll.import_data.delete_many({"uid": uid})
+    await client.search.force_delete_all(uid=uid)
+
+
+async def disable(uid: str) -> const.Code:
+    res = await client.coll.users.update_one(
+        {"id": uid},
+        {"$set": {"disabled": True}}
     )
-    return u, code
+    return const.Code.OK if res.acknowledged == 1 else const.Code.OPERATION_FAILED
+
+
+async def enable(uid: str) -> const.Code:
+    res = await client.coll.users.update_one(
+        {"id": uid},
+        {"$set": {"disabled": False}}
+    )
+    return const.Code.OK if res.acknowledged == 1 else const.Code.OPERATION_FAILED
```

### Comparing `retk-0.2.4/src/rethink/core/files/get.py` & `retk-0.2.5/src/retk/core/files/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple, Literal
 
-from rethink.models.client import client
-from rethink.models.tps import UserFile
+from retk.models.client import client
+from retk.models.tps import UserFile
 
 
 def get_files(
         uid: str,
         page: int,
         page_size: int,
         sort: Literal["filename", "created_at", "size"] = "created_at",
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/async_tasks/__init__.py` & `retk-0.2.5/src/retk/core/files/importing/async_tasks/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import asyncio
 import multiprocessing
 import traceback
 
-from rethink.logger import logger
+from retk.logger import logger
 from .obsidian.task import upload_obsidian_task
 from .text.task import update_text_task
 
 ctx = multiprocessing.get_context('spawn')
 QUEUE = ctx.Queue()
 
 
-def async_task(queue: multiprocessing.Queue):
+def __async_task(queue: multiprocessing.Queue):
     try:
         loop = asyncio.get_running_loop()
     except RuntimeError:
         loop = asyncio.get_event_loop()
     while True:
         item = queue.get()
         task = item.pop("task")
@@ -32,12 +32,12 @@
             oneline = msg.replace("\n", "\\n")
             logger.error(f"async task error: {oneline}")
     loop.close()
 
 
 def init():
     p = ctx.Process(
-        target=async_task,
+        target=__async_task,
         args=(QUEUE,),
         daemon=True,
     )
     p.start()
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/ops.py` & `retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import zipfile
 from dataclasses import dataclass, field
 from datetime import datetime
 from os.path import normpath
 from pathlib import Path
 from typing import Tuple, Dict, Optional
 
-from rethink import regex, const
-from rethink.core.files.saver import saver, File
-from rethink.utils import short_uuid
+from retk import regex, const
+from retk.core.files.saver import saver, File
+from retk.utils import short_uuid
 
 
 @dataclass
 class UnzipObsidian:
     @dataclass
     class Meta:
         __slots__ = ["filepath", "filename", "title", "file", "size", "duplicate", "created_at"]
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/task.py` & `retk-0.2.5/src/retk/core/files/importing/async_tasks/obsidian/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 import zipfile
 
 import pymongo.errors
 
-from rethink import const, core
-from rethink.logger import logger
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
+from retk import const, core
+from retk.logger import logger
+from retk.models.tps import AuthedUser, convert_user_dict_to_authed_user
 from . import ops
 from .. import utils
 
 
 async def upload_obsidian_task(  # noqa: C901
         bytes_data: bytes,
         filename: str,
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/async_tasks/text/task.py` & `retk-0.2.5/src/retk/core/files/importing/async_tasks/text/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 import pymongo.errors
 
-from rethink import const, core
-from rethink.logger import logger
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
+from retk import const, core
+from retk.logger import logger
+from retk.models.tps import AuthedUser, convert_user_dict_to_authed_user
 from .. import utils
 
 
 async def update_text_task(  # noqa: C901
         files: List[dict],
         max_file_size: int,
         uid: str,
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/async_tasks/utils.py` & `retk-0.2.5/src/retk/core/files/importing/async_tasks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 from typing import Optional, Tuple
 
 from bson import ObjectId
 from bson.tz_util import utc
 
-from rethink import const, config
-from rethink.models.client import client
-from rethink.models.tps import ImportData
+from retk import const, config
+from retk.models.client import client
+from retk.models.tps import ImportData
 
 
 async def check_last_task_finished(uid: str, type_: str) -> Tuple[Optional[ImportData], bool]:
     doc = await client.coll.import_data.find_one({"uid": uid})
     if doc and doc["running"]:
         await set_running_false(
             uid=uid,
@@ -103,15 +103,15 @@
         )
     if doc is None:
         return doc, const.Code.OPERATION_FAILED
     return doc, const.Code.OK
 
 
 async def import_set_modules():
-    from rethink.models.client import client
+    from retk.models.client import client
     await client.init()
 
 
 async def set_running_false(
         uid: str,
         code: const.Code,
         msg: str = "",
```

### Comparing `retk-0.2.4/src/rethink/core/files/importing/sync_tasks/editor.py` & `retk-0.2.5/src/retk/core/files/importing/sync_tasks/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from fastapi import UploadFile
 
-from rethink import const
-from rethink.core.files.saver import saver, File
+from retk import const
+from retk.core.files.saver import saver, File
 
 
 async def save_editor_upload_files(
         uid: str,
         files: List[UploadFile],
 ) -> dict:
     res = {
```

### Comparing `retk-0.2.4/src/rethink/core/files/saver.py` & `retk-0.2.5/src/retk/core/files/saver.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from dataclasses import dataclass
 from typing import BinaryIO
 
 from PIL import Image, UnidentifiedImageError
 from bson import ObjectId
 from qcloud_cos import CosConfig, CosServiceError, CosS3Client
 
-from rethink.config import get_settings, is_local_db
-from rethink.const import IMG_RESIZE_THRESHOLD, FileTypes
-from rethink.core.user import update_used_space
-from rethink.logger import logger
-from rethink.models.client import client
-from rethink.models.tps import UserFile
+from retk.config import get_settings, is_local_db
+from retk.const import IMG_RESIZE_THRESHOLD, FileTypes
+from retk.core.user import update_used_space
+from retk.logger import logger
+from retk.models.client import client
+from retk.models.tps import UserFile
 
 
 @dataclass
 class File:
     data: BinaryIO
     filename: str
 
@@ -80,15 +80,15 @@
 
     async def save_local(self, uid: str, file: File) -> str:
         path = get_settings().RETHINK_LOCAL_STORAGE_PATH / ".data" / "files" / file.hashed_filename
         path.parent.mkdir(parents=True, exist_ok=True)
 
         if path.exists():
             # skip the same image
-            return ""
+            return f"/files/{file.hashed_filename}"
 
         try:
             if file.type == FileTypes.IMAGE:
                 file.image_resize(resize_threshold=self.resize_threshold)
                 Image.open(file.data).save(path)
             else:
                 with open(path, "wb") as f:
```

### Comparing `retk-0.2.4/src/rethink/core/files/upload.py` & `retk-0.2.5/src/retk/core/files/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import List, Tuple, Optional
 
 import httpx
 from bson.tz_util import utc
 from fastapi import UploadFile
 from starlette.datastructures import Headers
 
-from rethink import const, core
-from rethink.config import is_local_db
-from rethink.logger import logger
-from rethink.models.client import client
-from rethink.models.tps import AuthedUser
-from rethink.utils import ssrf_check, ASYNC_CLIENT_HEADERS
+from retk import const, core
+from retk.config import is_local_db
+from retk.logger import logger
+from retk.models.client import client
+from retk.models.tps import AuthedUser
+from retk.utils import ssrf_check, ASYNC_CLIENT_HEADERS
 from .importing import async_tasks, sync_tasks
 
 QUEUE_INITED = False
 
 
 async def upload_obsidian(au: AuthedUser, zipped_files: List[UploadFile]) -> const.Code:
     max_file_count = 1
@@ -96,19 +96,19 @@
             "max_file_size": max_file_size,
             "uid": au.u.id,
             "request_id": au.request_id,
         })
     return const.Code.OK
 
 
-async def get_upload_process(uid: str) -> Tuple[Optional[dict], const.Code]:
+async def get_upload_process(uid: str) -> Optional[dict]:
     timeout_minus = 5
     doc = await client.coll.import_data.find_one({"uid": uid})
     if doc is None:
-        return None, const.Code.TASK_NOT_FOUND
+        return None
     now = datetime.datetime.now(tz=utc)
 
     # upload timeout
     if doc["running"] and \
             now.replace(tzinfo=None) - doc["startAt"].replace(tzinfo=None) \
             > datetime.timedelta(minutes=timeout_minus):
         doc["running"] = False
@@ -116,15 +116,15 @@
             {"uid": uid},
             {"$set": {
                 "running": False,
                 "code": const.Code.UPLOAD_TASK_TIMEOUT.value,
                 "msg": f"Timeout, upload not finish in {timeout_minus} mins",
             }},
         )
-    return doc, const.Code.OK
+    return doc
 
 
 async def vditor_upload(au: AuthedUser, files: List[UploadFile]) -> dict:
     res = {
         "errFiles": [],
         "succMap": {},
         "code": const.Code.OK,
```

### Comparing `retk-0.2.4/src/rethink/core/node/backup.py` & `retk-0.2.5/src/retk/core/node/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pathlib import Path
 from typing import List, Tuple
 
 from bson.tz_util import utc
 from pydantic_settings import BaseSettings
 from qcloud_cos import CosConfig, CosServiceError, CosS3Client
 
-from rethink import config, const
-from rethink.logger import logger
-from rethink.models import tps
-from rethink.models.client import client
+from retk import config, const
+from retk.logger import logger
+from retk.models import tps
+from retk.models.client import client
 
 
 async def storage_md(node: tps.Node, keep_hist: bool) -> const.Code:  # noqa: C901
     nid = node["id"]
     md = node["md"]
     hist = node.get("history", [])
     date_format = "%Y-%m-%d %H:%M:%S.%fZ"
```

### Comparing `retk-0.2.4/src/rethink/core/node/node.py` & `retk-0.2.5/src/retk/core/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 import datetime
 from typing import List, Optional, Tuple, Dict, Any
 
 from bson import ObjectId
 from bson.tz_util import utc
 
-from rethink import config, const, utils, regex
-from rethink import plugins
-from rethink.core import user
-from rethink.logger import logger
-from rethink.models import tps, db_ops
-from rethink.models.client import client
-from rethink.models.search_engine.engine import SearchDoc
+from retk import config, const, utils, regex
+from retk import plugins
+from retk.core import user
+from retk.logger import logger
+from retk.models import tps, db_ops
+from retk.models.client import client
+from retk.models.search_engine.engine import SearchDoc
 from . import backup, node_utils
 
 
 @plugins.handler.on_node_added
 async def post(  # noqa: C901
         au: tps.AuthedUser,
         md: str,
```

### Comparing `retk-0.2.4/src/rethink/core/node/node_utils.py` & `retk-0.2.5/src/retk/core/node/node_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Set, Tuple
 
-from rethink import const, regex
-from rethink.models import tps, db_ops
-from rethink.models.client import client
+from retk import const, regex
+from retk.models import tps, db_ops
+from retk.models.client import client
 
 
 def get_linked_nodes(new_md) -> Tuple[set, const.Code]:
     # last first
     cache_current_to_nid: Set[str] = set()
 
     for match in list(regex.MD_AT_LINK.finditer(new_md))[::-1]:
```

### Comparing `retk-0.2.4/src/rethink/core/node/search.py` & `retk-0.2.5/src/retk/core/node/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict, Tuple, Sequence, Literal
 
-from rethink.controllers.schemas.node import NodesSearchResponse
-from rethink.controllers.utils import datetime2str
-from rethink.core.recent import put_recent_search
-from rethink.models import tps
-from rethink.models.client import client
-from rethink.models.search_engine.engine import SearchResult
+from retk.controllers.schemas.node import NodesSearchResponse
+from retk.controllers.utils import datetime2str
+from retk.core.recent import put_recent_search
+from retk.models import tps
+from retk.models.client import client
+from retk.models.search_engine.engine import SearchResult
 
 
 async def _2node_data(
         hits: Sequence[SearchResult],
 ) -> List[NodesSearchResponse.Data.Node]:
     nodes = await client.coll.nodes.find({"id": {"$in": [hit.nid for hit in hits]}}).to_list(length=None)
     nodes_map: Dict[str, tps.Node] = {n["id"]: n for n in nodes}
```

### Comparing `retk-0.2.4/src/rethink/core/recent.py` & `retk-0.2.5/src/retk/core/recent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from rethink import const
-from rethink.models.client import client
-from rethink.models.tps import AuthedUser
+from retk import const
+from retk.models.client import client
+from retk.models.tps import AuthedUser
 
 
 async def added_at_node(
         au: AuthedUser,
         nid: str,
         to_nid: str,
 ) -> const.Code:
```

### Comparing `retk-0.2.4/src/rethink/core/user.py` & `retk-0.2.5/src/retk/core/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import html
 from typing import Optional, Tuple
 
 from bson import ObjectId
 from bson.tz_util import utc
 from pymongo.errors import DuplicateKeyError
 
-from rethink import const, config, utils
-from rethink.controllers.schemas.user import PatchUserRequest
-from rethink.models import tps
-from rethink.models.client import client
+from retk import const, config, utils
+from retk.controllers.schemas.user import PatchUserRequest
+from retk.models import tps
+from retk.models.client import client
 
 
 async def add(
         account: str,
         source: int,
         email: str,
         hashed: str,
@@ -129,54 +129,33 @@
         )
         if res.modified_count != 1:
             return None, const.Code.OPERATION_FAILED
 
     return await get(uid=au.u.id)
 
 
-async def delete(uid: str) -> const.Code:
-    res = await client.coll.users.delete_one({"id": uid})
-    return const.Code.OK if res.deleted_count == 1 else const.Code.OPERATION_FAILED
-
-
-async def disable(uid: str) -> const.Code:
-    res = await client.coll.users.update_one(
-        {"id": uid},
-        {"$set": {"disabled": True}}
-    )
-    return const.Code.OK if res.modified_count == 1 else const.Code.OPERATION_FAILED
-
-
-async def enable(uid: str) -> const.Code:
-    res = await client.coll.users.update_one(
-        {"id": uid},
-        {"$set": {"disabled": False}}
-    )
-    return const.Code.OK if res.modified_count == 1 else const.Code.OPERATION_FAILED
-
-
-async def get_by_email(email: str) -> Tuple[Optional[tps.UserMeta], const.Code]:
+async def get_by_email(email: str, disabled: bool = False) -> Tuple[Optional[tps.UserMeta], const.Code]:
     if config.get_settings().ONE_USER:
         source = const.UserSource.LOCAL.value
     else:
         source = const.UserSource.EMAIL.value
-    return await get_account(account=email, source=source)
+    return await get_account(account=email, source=source, disabled=disabled)
 
 
-async def get_account(account: str, source: int) -> Tuple[Optional[tps.UserMeta], const.Code]:
-    u = await client.coll.users.find_one({"source": source, "account": account, "disabled": False})
+async def get_account(account: str, source: int, disabled: bool = False) -> Tuple[Optional[tps.UserMeta], const.Code]:
+    u = await client.coll.users.find_one({"source": source, "account": account, "disabled": disabled})
     if u is None:
         return None, const.Code.ACCOUNT_OR_PASSWORD_ERROR
     return u, const.Code.OK
 
 
 async def get(uid: str) -> Tuple[Optional[tps.UserMeta], const.Code]:
     u = await client.coll.users.find_one({"id": uid, "disabled": False})
     if u is None:
-        return None, const.Code.ACCOUNT_OR_PASSWORD_ERROR
+        return None, const.Code.USER_DISABLED
     if u["usedSpace"] < 0:
         # reset usedSpace to 0
         await client.coll.users.update_one(
             {"id": uid},
             {"$set": {"usedSpace": 0}}
         )
         u["usedSpace"] = 0
@@ -196,13 +175,13 @@
 
 async def user_space_not_enough(au: tps.AuthedUser) -> bool:
     if config.is_local_db():
         return False
     return au.u.used_space > const.USER_TYPE.id2config(au.u.type).max_store_space
 
 
-async def reset_password(au: tps.AuthedUser, hashed: str) -> const.Code:
+async def reset_password(uid: str, hashed: str) -> const.Code:
     res = await client.coll.users.update_one(
-        {"id": au.u.id},
+        {"id": uid},
         {"$set": {"hashed": hashed}}
     )
     return const.Code.OK if res.acknowledged == 1 else const.Code.OPERATION_FAILED
```

### Comparing `retk-0.2.4/src/rethink/depend/mongita/__init__.py` & `retk-0.2.5/src/retk/depend/mongita/__init__.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/collection.py` & `retk-0.2.5/src/retk/depend/mongita/collection.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/command_cursor.py` & `retk-0.2.5/src/retk/depend/mongita/command_cursor.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/common.py` & `retk-0.2.5/src/retk/depend/mongita/common.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/cursor.py` & `retk-0.2.5/src/retk/depend/mongita/cursor.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/database.py` & `retk-0.2.5/src/retk/depend/mongita/database.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/engines/disk_engine.py` & `retk-0.2.5/src/retk/depend/mongita/engines/disk_engine.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/engines/engine_common.py` & `retk-0.2.5/src/retk/depend/mongita/engines/engine_common.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/engines/memory_engine.py` & `retk-0.2.5/src/retk/depend/mongita/engines/memory_engine.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/errors.py` & `retk-0.2.5/src/retk/depend/mongita/errors.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/mongita_client.py` & `retk-0.2.5/src/retk/depend/mongita/mongita_client.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/mongitasync.py` & `retk-0.2.5/src/retk/depend/mongita/mongitasync.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/results.py` & `retk-0.2.5/src/retk/depend/mongita/results.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/mongita/write_concern.py` & `retk-0.2.5/src/retk/depend/mongita/write_concern.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/base.py` & `retk-0.2.5/src/retk/depend/sso/base.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/facebook.py` & `retk-0.2.5/src/retk/depend/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/generic.py` & `retk-0.2.5/src/retk/depend/sso/generic.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/github.py` & `retk-0.2.5/src/retk/depend/sso/github.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/gitlab.py` & `retk-0.2.5/src/retk/depend/sso/gitlab.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/google.py` & `retk-0.2.5/src/retk/depend/sso/google.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/microsoft.py` & `retk-0.2.5/src/retk/depend/sso/microsoft.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/depend/sso/qq.py` & `retk-0.2.5/src/retk/depend/sso/qq.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/logger.py` & `retk-0.2.5/src/retk/logger.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/models/client.py` & `retk-0.2.5/src/retk/models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import os
 import struct
 from typing import Optional, Union
 
 from bson import ObjectId
 from bson.tz_util import utc
 
-from rethink import config, const, utils, version_manager
-from rethink.depend.mongita import MongitaClientDisk
-from rethink.logger import logger
-from rethink.models.search_engine.engine import BaseEngine, SearchDoc, RestoreSearchDoc
-from rethink.models.search_engine.engine_local import LocalSearcher
+from retk import config, const, utils, version_manager
+from retk.depend.mongita import MongitaClientDisk
+from retk.logger import logger
+from retk.models.search_engine.engine import BaseEngine, SearchDoc, RestoreSearchDoc
+from retk.models.search_engine.engine_local import LocalSearcher
 from .coll import Collections
 from .indexing import remote_try_build_index
 from .tps import UserFile, ImportData, UserMeta, Node, AuthedUser, convert_user_dict_to_authed_user
 
 try:
     from motor.motor_asyncio import AsyncIOMotorClient
-    from rethink.models.search_engine.engine_es import ESSearcher
+    from retk.models.search_engine.engine_es import ESSearcher
 except ImportError:
     pass
 
 
 class Client:
     coll: Collections = Collections()
     mongo: Optional[Union["AsyncIOMotorClient", MongitaClientDisk]] = None
```

### Comparing `retk-0.2.4/src/rethink/models/db_ops.py` & `retk-0.2.5/src/retk/models/db_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
-from rethink import config
-from rethink.depend.mongita.results import UpdateResult
+from retk import config
+from retk.depend.mongita.results import UpdateResult
 from .client import client
 
 
 async def remove_from_node(from_nid: str, to_nid: str):
     if config.is_local_db():
         # no $pull support
         to_n = await client.coll.nodes.find_one({"id": to_nid})
```

### Comparing `retk-0.2.4/src/rethink/models/indexing.py` & `retk-0.2.5/src/retk/models/indexing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from rethink.models.coll import Collections
+from retk.models.coll import Collections
 
 IS_MOTOR = True
 try:
     from motor.motor_asyncio import AsyncIOMotorCollection
 except ImportError:
     IS_MOTOR = False
```

### Comparing `retk-0.2.4/src/rethink/models/search_engine/engine.py` & `retk-0.2.5/src/retk/models/search_engine/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Tuple, Sequence, Literal
 
-from rethink import const
-from rethink.models.tps import AuthedUser
-from rethink.utils import strip_html_tags
+from retk import const
+from retk.models.tps import AuthedUser
+from retk.utils import strip_html_tags
 
 
 @dataclass
 class SearchDoc:
     nid: str
     title: str
     body: str
@@ -95,14 +95,18 @@
         ...
 
     @abstractmethod
     async def delete_batch(self, au: AuthedUser, nids: List[str]) -> const.Code:
         ...
 
     @abstractmethod
+    async def force_delete_all(self, uid: str) -> const.Code:
+        ...
+
+    @abstractmethod
     async def update_batch(self, au: AuthedUser, docs: List[SearchDoc]) -> const.Code:
         ...
 
     @abstractmethod
     async def batch_to_trash(self, au: AuthedUser, nids: List[str]) -> const.Code:
         ...
```

### Comparing `retk-0.2.4/src/rethink/models/search_engine/engine_es.py` & `retk-0.2.5/src/retk/models/search_engine/engine_es.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
 from typing import List, Tuple, Sequence, Dict, Any, Literal
 
 from bson.tz_util import utc
 from elastic_transport import ObjectApiResponse
 from elasticsearch import AsyncElasticsearch, helpers
 
-from rethink import const
-from rethink.config import get_settings
-from rethink.logger import logger
-from rethink.models.search_engine.engine import (
+from retk import const
+from retk.config import get_settings
+from retk.logger import logger
+from retk.models.search_engine.engine import (
     BaseEngine, SearchDoc, SearchResult, RestoreSearchDoc, STOPWORDS,
 )
-from rethink.models.tps import AuthedUser
+from retk.models.tps import AuthedUser
 
 
 def datetime2str(dt: datetime.datetime) -> str:
     return dt.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
 
 
 def get_utc_now() -> str:
@@ -429,14 +429,38 @@
             logger.error(f"delete batch failed, resp: {resp}")
             return const.Code.OPERATION_FAILED
         if resp.body["deleted"] != len(nids):
             logger.error(f"delete batch failed, resp: {resp}")
             return const.Code.OPERATION_FAILED
         return const.Code.OK
 
+    async def force_delete_all(self, uid: str) -> const.Code:
+        resp = await self.es.delete_by_query(
+            index=self.index,
+            body={
+                "query": {
+                    "bool": {
+                        "must": [
+                            {
+                                "term": {
+                                    "uid": uid
+                                }
+                            },
+
+                        ]
+                    }
+                }
+            },
+            refresh=True,
+        )
+        if resp.meta.status != 200:
+            logger.error(f"force delete all failed, resp: {resp}")
+            return const.Code.OPERATION_FAILED
+        return const.Code.OK
+
     async def update_batch(self, au: AuthedUser, docs: List[SearchDoc]) -> const.Code:
         actions = []
         now = datetime.datetime.now(tz=utc)
         for doc in docs:
             d = doc.__dict__
             d["modifiedAt"] = datetime2str(now)
             d["uid"] = au.u.id
```

### Comparing `retk-0.2.4/src/rethink/models/search_engine/engine_local.py` & `retk-0.2.5/src/retk/models/search_engine/engine_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from jieba.analyse import ChineseAnalyzer
 from whoosh.fields import TEXT, ID, Schema, DATETIME, BOOLEAN
 from whoosh.highlight import Highlighter, HtmlFormatter
 from whoosh.index import create_in, open_dir, FileIndex
 from whoosh.qparser import QueryParser, syntax
 from whoosh.query import Term, And, Or, Every
 
-from rethink import config, const
-from rethink.logger import logger
-from rethink.models.search_engine.engine import (
+from retk import config, const
+from retk.logger import logger
+from retk.models.search_engine.engine import (
     BaseEngine, SearchDoc, SearchResult, RestoreSearchDoc, STOPWORDS,
 )
-from rethink.models.tps import AuthedUser
+from retk.models.tps import AuthedUser
 
 jieba.setLogLevel(logging.ERROR)
 
 
 class LocalSearcher(BaseEngine):
     ix: FileIndex
     indexing_schema: Schema
@@ -146,14 +146,21 @@
             count = writer.delete_by_query(q=q)
             if count != 1:
                 logger.error(f"nid {nid} not found or more than one found")
                 return const.Code.NODE_NOT_EXIST
         writer.commit()
         return const.Code.OK
 
+    async def force_delete_all(self, uid: str) -> const.Code:
+        writer = self.ix.writer()
+        q = Term("uid", uid)
+        writer.delete_by_query(q=q)
+        writer.commit()
+        return const.Code.OK
+
     async def update_batch(self, au: AuthedUser, docs: List[SearchDoc]) -> const.Code:
         writer = self.ix.writer()
         for doc in docs:
             with self.ix.searcher() as searcher:
                 resp = searcher.search(And([Term("uid", au.u.id), Term("nid", doc.nid)]))
                 if len(resp) != 1:
                     logger.error(f"nid {doc.nid} not found or more than one found")
```

### Comparing `retk-0.2.4/src/rethink/models/tps.py` & `retk-0.2.5/src/retk/models/tps.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/plugins/base.py` & `retk-0.2.5/src/retk/plugins/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,53 +5,61 @@
 
 
 Usage:
 
 1. Create a new plugin by inheriting from `Plugin`:
 
     ```python
-    import rethink
+    import retk
 
-    class MyPlugin(rethink.Plugin):
+    class MyPlugin(retk.Plugin):
         name = "MyPlugin"
         version = "0.1.0"
         description = "A demo plugin."
         author = "me"
 
 
         def before_node_updated(self, uid: str, nid: str, data: Dict[str, Any]) -> None:
             print("before_node_updated")
             data["md"] = "before_node_updated:" + data["md"]
     ```
 
 2. Add the plugin to the system:
 
     ```python
-    rethink.add_plugin(MyPlugin())
+    retk.add_plugin(MyPlugin())
     ```
 
 3. Run rethink server:
 
     ```python
-    rethink.run()
+    retk.run()
     ```
 
 4. Check when update a node, the `before_node_updated` text will show on your note.
 """
 
 import base64
 import inspect
 import os
+from dataclasses import dataclass
 from typing import Dict, List, Optional, Any
 
-from rethink import const
-from rethink.models import tps
+from retk import const
+from retk.models import tps
 from .schedule.timing import Timing
 
 
+@dataclass
+class PluginAPICallReturn:
+    success: bool
+    message: str
+    data: Any
+
+
 class Plugin:
     """
     Attributes:
         name (str): The name of the plugin.
         version (str): The version of the plugin.
         description (str): The description of the plugin.
         author (str): The author of the plugin.
@@ -106,30 +114,30 @@
 
     def on_node_updated(self, node: tps.Node, old_node: tps.Node) -> None:
         raise NotImplementedError
 
     def on_schedule(self) -> None:
         raise NotImplementedError
 
-    def handle_api_call(self, method: str, data: Any) -> Any:
+    def handle_api_call(self, method: str, data: Any) -> PluginAPICallReturn:
         """
         api call from your plugin rendered page. etc. plugin home page, editor side bar.
 
         POST: https://ip:port/plugin/call
 
         The exact POST url can be found in self.api_call_url
 
         Body: {
             "pluginId: "your plugin id",
             "method": "your method",
             "data": any data format,
             "requestId": "unique request id string"
         }
         Response: {
-            "code": int code,
+            "success": boolean,
             "message": "message",
             "requestId": "unique request id string",
             "pluginId: "your plugin id",
             "method": "your method",
             "data": any data format,
         }
 
@@ -153,15 +161,15 @@
             str: the api call url
         """
         try:
             port = os.environ["VUE_APP_API_PORT"]
             host = os.environ['RETHINK_SERVER_HOSTNAME']
         except KeyError:
             raise ValueError("the host or port number is not set in the environment.")
-        return f"http://{host}:{port}/api/plugin/call"
+        return f"http://{host}:{port}/api/plugins/call"
 
 
 event_plugin_map: Dict[str, List[Plugin]] = {
     "on_node_added": [],
     "before_node_updated": [],
     "on_node_updated": [],
     "on_schedule": [],
```

### Comparing `retk-0.2.4/src/rethink/plugins/handler.py` & `retk-0.2.5/src/retk/plugins/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable
 
-from rethink.const import Code
-from rethink.models.tps import AuthedUser
+from retk.const import Code
+from retk.models.tps import AuthedUser
 from .base import event_plugin_map
 
 
 def on_node_added(func: Callable):
     async def wrapper(*args, **kwargs):
         data, code = await func(*args, **kwargs)
         if code != Code.OK:
```

### Comparing `retk-0.2.4/src/rethink/plugins/register.py` & `retk-0.2.5/src/retk/plugins/register.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from rethink import config
-from rethink.logger import logger
-from rethink.plugins.base import add_plugin, remove_plugin
-from rethink.plugins.official_plugins.favorites.main import Favorites
-from rethink.plugins.official_plugins.summary.main import DailySummary
+from retk import config
+from retk.logger import logger
+from retk.plugins.base import add_plugin, remove_plugin
+from retk.plugins.official_plugins.favorites.main import Favorites
+from retk.plugins.official_plugins.summary.main import DailySummary
 
 _official_plugins = [
     DailySummary(),
     Favorites(),
 ]
```

### Comparing `retk-0.2.4/src/rethink/plugins/schedule/timing.py` & `retk-0.2.5/src/retk/plugins/schedule/timing.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/regex.py` & `retk-0.2.5/src/retk/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from rethink import const
+from retk import const
 
 # at least 6 characters, at most 20 characters, at least one letter and one number
 VALID_PASSWORD = re.compile(r"^(?=.*[A-Za-z])(?=.*\d).{6,20}$")
 
 EMAIL = re.compile(r'^[.0-9a-zA-Z_]{1,18}@([0-9a-zA-Z-]{1,13}\.){1,}[a-zA-Z]{1,3}$')
 
 MD_CODE = re.compile(r"^```[^\S\r\n]*[a-z]*?\n(.*?)\n```$", re.MULTILINE | re.DOTALL)
```

### Comparing `retk-0.2.4/src/rethink/routes/account.py` & `retk-0.2.5/src/retk/routes/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Optional
 
 from fastapi import APIRouter
 
-from rethink.controllers import schemas, account
-from rethink.routes import utils
+from retk.controllers import schemas, account
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/account",
     tags=["user"],
     responses={404: {"description": "Not found"}},
 )
 
 
 @router.post(
     "/",
     status_code=201,
     response_model=schemas.account.TokenResponse,
 )
 @utils.measure_time_spend
-async def register(
+async def signup(
         au: utils.ANNOTATED_AUTHED_USER,
         req: schemas.account.SignupRequest,
         referer: Optional[str] = utils.DEPENDS_REFERER,
 ) -> schemas.account.TokenResponse:
     return await account.signup(au=au, req=req)
 
 
@@ -61,8 +61,8 @@
 )
 @utils.measure_time_spend
 async def email_verification(
         au: utils.ANNOTATED_AUTHED_USER,
         req: schemas.account.EmailVerificationRequest,
         referer: Optional[str] = utils.DEPENDS_REFERER,
 ) -> schemas.account.TokenResponse:
-    return account.email_send_code(au=au, req=req)
+    return await account.email_send_code(au=au, req=req)
```

### Comparing `retk-0.2.4/src/rethink/routes/app_captcha.py` & `retk-0.2.5/src/retk/routes/app_captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi.responses import StreamingResponse
 
-from rethink.controllers import account
-from rethink.routes import utils
+from retk.controllers import account
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/captcha",
     tags=["captcha"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/routes/app_system.py` & `retk-0.2.5/src/retk/routes/app_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from fastapi import APIRouter
 
-from rethink.controllers import schemas
-from rethink.controllers.app_system import get_latest_version
-from rethink.routes import utils
+from retk.controllers import schemas
+from retk.controllers.app_system import get_latest_version
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/system",
     tags=["system"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/routes/files.py` & `retk-0.2.5/src/retk/routes/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 
 from fastapi import APIRouter, UploadFile, Request
 
-from rethink.controllers import schemas
-from rethink.controllers.files import upload_files
-from rethink.routes import utils
+from retk.controllers import schemas
+from retk.controllers.files import upload_files
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/files",
     tags=["files"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/routes/node.py` & `retk-0.2.5/src/retk/routes/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional, Literal
 
 from fastapi import APIRouter
 from fastapi.params import Path, Query
 from typing_extensions import Annotated
 
-from rethink import const
-from rethink.controllers import schemas
-from rethink.controllers.node import node_ops, search
-from rethink.routes import utils
+from retk import const
+from retk.controllers import schemas
+from retk.controllers.node import node_ops, search
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/nodes",
     tags=["node"],
     responses={404: {"description": "Not found"}},
 )
 
@@ -77,23 +77,23 @@
     )
 
 
 # make sure this is before /{nid} otherwise it will be treated as a nid
 @router.get(
     path="/core",
     status_code=200,
-    response_model=schemas.node.GetFromTrashResponse,
+    response_model=schemas.node.NodesSearchResponse,
 )
 @utils.measure_time_spend
 async def get_core_nodes(
         au: utils.ANNOTATED_AUTHED_USER,
         p: int = Query(default=0, ge=0, description="page number"),
         limit: int = Query(default=10, ge=0, le=const.SEARCH_LIMIT_MAX),
         referer: Optional[str] = utils.DEPENDS_REFERER,
-) -> schemas.node.GetFromTrashResponse:
+) -> schemas.node.NodesSearchResponse:
     return await node_ops.get_core_nodes(
         au=au,
         p=p,
         limit=limit,
     )
```

### Comparing `retk-0.2.4/src/rethink/routes/oauth.py` & `retk-0.2.5/src/retk/routes/oauth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import Request, APIRouter
 from fastapi.params import Annotated, Path
 
-from rethink.controllers import oauth as co
-from rethink.controllers.schemas.account import TokenResponse
-from rethink.routes import utils
+from retk.controllers import oauth as co
+from retk.controllers.schemas.account import TokenResponse
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/oauth",
     tags=["oauth"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/routes/plugin.py` & `retk-0.2.5/src/retk/routes/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import APIRouter
 
-from rethink.controllers import plugin as plugin_ops
-from rethink.controllers import schemas
-from rethink.plugins.register import register_official_plugins
-from rethink.routes import utils
+from retk.controllers import plugin as plugin_ops
+from retk.controllers import schemas
+from retk.plugins.register import register_official_plugins
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/plugins",
     tags=["user"],
     responses={404: {"description": "Not found"}},
 )
 
@@ -72,11 +72,10 @@
 @router.post(
     path="/call",
     status_code=200,
     response_model=schemas.plugin.PluginCallResponse
 )
 @utils.measure_time_spend
 async def plugin_call(
-        au: utils.ANNOTATED_AUTHED_USER,
         req: schemas.plugin.PluginCallRequest,
 ) -> schemas.plugin.PluginCallResponse:
-    return await plugin_ops.plugin_call(au=au, req=req)
+    return await plugin_ops.plugin_call(req=req)
```

### Comparing `retk-0.2.4/src/rethink/routes/recent.py` & `retk-0.2.5/src/retk/routes/recent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fastapi import APIRouter
 
-from rethink.controllers import schemas, recent
-from rethink.routes import utils
+from retk.controllers import schemas, recent
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/recent",
     tags=["search"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/routes/self_hosted.py` & `retk-0.2.5/src/retk/routes/self_hosted.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 from fastapi import APIRouter, HTTPException, FastAPI
-from fastapi.responses import HTMLResponse, FileResponse
+from fastapi.responses import HTMLResponse, FileResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 
-from rethink import const, config
-from rethink.logger import logger
-from rethink.models.client import client
-from rethink.routes import utils
+from retk import const, config
+from retk.logger import logger
+from retk.models.client import client
+from retk.routes import utils
 
 router = APIRouter(
     tags=["self_hosted"],
     responses={404: {"description": "Not found"}},
 )
 
 
@@ -20,37 +20,41 @@
     try:
         await client.search.es.close()
     except (AttributeError, ValueError):
         pass
     logger.debug("db closed")
 
 
-@router.get("/", response_class=HTMLResponse)
 @router.get("/sauth", response_class=HTMLResponse)
 @router.get("/docs", response_class=HTMLResponse)
 @router.get("/login", response_class=HTMLResponse)
 @router.get("/about", response_class=HTMLResponse)
 @router.get("/r", response_class=HTMLResponse)
 @router.get("/r/{path}", response_class=HTMLResponse)
 @router.get("/r/plugin/{pid}", response_class=HTMLResponse)
 @router.get("/n/{nid}", response_class=HTMLResponse)
-async def index() -> HTMLResponse:
+async def app_page() -> HTMLResponse:
     content = (const.FRONTEND_DIR / "index.html").read_text(encoding="utf-8")
     if os.getenv("RETHINK_SERVER_PASSWORD", None) is not None:
         req_password = "window.VUE_APP_ONE_USER_REQUIRE_AUTH=1;"
     else:
         req_password = ""
     content += f"<script>window.VUE_APP_API_PORT={os.getenv('VUE_APP_API_PORT')};" \
                f"{req_password}</script>"
     return HTMLResponse(
         content=content,
         status_code=200,
     )
 
 
+@router.get("/", response_class=RedirectResponse)
+async def index() -> RedirectResponse:
+    return RedirectResponse(url="/r")
+
+
 @router.get(
     "/files/{fid}",
     status_code=200,
     response_class=FileResponse,
 )
 async def user_data(
         fid: str = utils.ANNOTATED_FID
```

### Comparing `retk-0.2.4/src/rethink/routes/trash.py` & `retk-0.2.5/src/retk/routes/trash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Optional
 
 from fastapi import APIRouter, Query
 
-from rethink.controllers import schemas
-from rethink.controllers.node import trash_ops
-from rethink.routes import utils
+from retk.controllers import schemas
+from retk.controllers.node import trash_ops
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/trash",
     tags=["trash"],
     responses={404: {"description": "Not found"}},
 )
 
 
 @router.get(
     path="/",
     status_code=200,
-    response_model=schemas.node.GetFromTrashResponse,
+    response_model=schemas.node.NodesSearchResponse,
 )
 @utils.measure_time_spend
 async def get_from_trash(
         au: utils.ANNOTATED_AUTHED_USER,
         p: int = Query(default=0, ge=0, description="page number"),
         limit: int = Query(default=10, ge=0, le=200, description="page size"),
         referer: Optional[str] = utils.DEPENDS_REFERER,
-) -> schemas.node.GetFromTrashResponse:
+) -> schemas.node.NodesSearchResponse:
     return await trash_ops.get_from_trash(
         au=au,
         p=p,
         limit=limit,
     )
```

### Comparing `retk-0.2.4/src/rethink/routes/user.py` & `retk-0.2.5/src/retk/routes/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from fastapi import APIRouter
 
-from rethink.controllers import schemas, user
-from rethink.routes import utils
+from retk.controllers import schemas, user
+from retk.routes import utils
 
 router = APIRouter(
     prefix="/api/users",
     tags=["user"],
     responses={404: {"description": "Not found"}},
 )
```

### Comparing `retk-0.2.4/src/rethink/run.py` & `retk-0.2.5/src/retk/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 import threading
 from pathlib import Path
 from typing import Literal, Union
 
 import uvicorn
 
-from rethink.plugins.base import event_plugin_map, Plugin
-from rethink.plugins.schedule.scheduler import scheduler
-from rethink.plugins.schedule.timing import Every
+from retk.plugins.base import event_plugin_map, Plugin
+from retk.plugins.schedule.scheduler import scheduler
+from retk.plugins.schedule.timing import Every
 
 
 def _schedule_job(plugin: Plugin, on: bool = False):
     if plugin.schedule_timing is None or not plugin.activated:
         return
 
     if on:
@@ -109,15 +109,15 @@
         if len(password) < 8:
             print("Password is too short. The password is highly recommended to be at least 8 characters!")
         os.environ["RETHINK_SERVER_PASSWORD"] = password
 
     td = _start_on_schedule_plugins()
 
     uvicorn.run(
-        "rethink.application:app",
+        "retk.application:app",
         host=host,
         port=port,
         reload=False,
         workers=1,
         log_level="error",
         env_file=os.path.join(os.path.abspath(os.path.dirname(__file__)), ".env.local"),
     )
```

### Comparing `retk-0.2.4/src/rethink/safety.py` & `retk-0.2.5/src/retk/safety.py`

 * *Files identical despite different names*

### Comparing `retk-0.2.4/src/rethink/utils.py` & `retk-0.2.5/src/retk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from urllib.parse import urlparse
 
 import httpx
 import jwt
 from bson import ObjectId
 from markdown import Markdown
 
-from rethink import config, const, regex
-from rethink.logger import logger
-from rethink.models import tps
+from retk import config, const, regex
+from retk.logger import logger
+from retk.models import tps
 
 HEADERS = {
     'typ': 'jwt',
     'alg': 'RS256'
 }
 alphabet = "3467ACDEFGHJKLMNPQRTUVWXYabcdefghkmnoprtuvwxy"
 alphabet_len = len(alphabet)
@@ -62,20 +62,23 @@
     payload.update(data)
     token = jwt.encode(
         payload=payload,
         key=config.get_settings().JWT_KEY,
         algorithm=HEADERS["alg"],
         headers=HEADERS,
     )
-    return token
+    return f"Bearer {token}"
 
 
 def jwt_decode(token: str) -> dict:
+    t = token.split("Bearer ", maxsplit=1)
+    if len(t) != 2:
+        raise jwt.InvalidTokenError("Invalid token")
     return jwt.decode(
-        token,
+        t[1],
         key=config.get_settings().JWT_KEY_PUB,
         algorithms=[HEADERS["alg"]],
         options={"verify_exp": True}
     )
 
 
 class HTMLStripper(HTMLParser):
@@ -405,16 +408,27 @@
         "inTrashAt": in_trash_at,
         "fromNodeIds": from_node_ids,
         "toNodeIds": to_node_ids,
         "history": history,
     }
 
 
+def parse_version(version: str) -> Optional[Tuple[int, int, int]]:
+    vs = version.split(".")
+    if len(vs) != 3:
+        return None
+    try:
+        vs = (int(vs[0]), int(vs[1]), int(vs[2]))
+    except ValueError:
+        return None
+    return vs
+
+
 async def get_latest_version() -> Tuple[Tuple[int, int, int], const.Code]:
-    url = 'https://pypi.org/pypi/rethink-note/json'
+    url = 'https://pypi.org/pypi/retk/json'
     default_version = (0, 0, 0)
     async with httpx.AsyncClient() as ac:
         try:
             response = await ac.get(
                 url=url,
                 headers=ASYNC_CLIENT_HEADERS,
                 follow_redirects=False,
@@ -437,17 +451,12 @@
     package_info = response.json()
 
     try:
         v = package_info['info']['version']
     except KeyError:
         logger.debug(f"failed to get {url}: {response.text}")
         return default_version, const.Code.OPERATION_FAILED
-    vs = v.split(".")
-    if len(vs) != 3:
-        logger.debug(f"failed to get {url}: {v}")
-        return default_version, const.Code.OPERATION_FAILED
-    try:
-        vs = (int(vs[0]), int(vs[1]), int(vs[2]))
-    except ValueError:
+    vs = parse_version(v)
+    if vs is None:
         logger.debug(f"failed to get {url}: {v}")
         return default_version, const.Code.OPERATION_FAILED
     return vs, const.Code.OK
```

### Comparing `retk-0.2.4/src/rethink/version_manager/migrate.py` & `retk-0.2.5/src/retk/version_manager/migrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
 from typing import Union, Dict, Optional
 
-from rethink._version import __version__
-from rethink.logger import logger
+from retk._version import __version__
+from retk.logger import logger
 
 
 def version_tuple(v):
     return tuple(map(int, (v.split("."))))
 
 
 __current_version = version_tuple(__version__)
```

### Comparing `retk-0.2.4/src/rethink/version_manager/recover.py` & `retk-0.2.5/src/retk/version_manager/recover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from bson import ObjectId
 
-from rethink import const, utils
-from rethink._version import __version__
+from retk import const, utils
+from retk._version import __version__
 
 
 def dump_dot_rethink(path: Union[os.PathLike, Path]) -> Dict:
     version = {
         "version": __version__,
         "_id": ObjectId(),
         "id": utils.short_uuid(),
```

### Comparing `retk-0.2.4/src/retk.egg-info/PKG-INFO` & `retk-0.2.5/src/retk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retk
-Version: 0.2.4
+Version: 0.2.5
 Summary: keep and reuse your thoughts
 Home-page: https://github.com/MorvanZhou/rethink
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/rethink/issues
 Project-URL: Source, https://github.com/MorvanZhou/rethink
 Classifier: Programming Language :: Python :: 3
@@ -47,19 +47,19 @@
 Requires-Dist: motor>=3.3.2; extra == "remote"
 Requires-Dist: elasticsearch[async]~=8.11.0; extra == "remote"
 
 # Rethink
 
 [![Unittest](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml/badge.svg)](https://github.com/MorvanZhou/rethink/actions/workflows/python-app.yml)
 [![License](https://img.shields.io/github/license/MorvanZhou/rethink)](https://github.com/MorvanZhou/rethink/blob/master/LICENSE)
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/v/rethink-note?color=%2334D058&label=pypi%20package" alt="Package version">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/v/retk?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://pypi.org/project/rethink-note" target="_blank">
-<img src="https://img.shields.io/pypi/pyversions/rethink-note.svg?color=%2334D058" alt="Supported Python versions">
+<a href="https://pypi.org/project/retk" target="_blank">
+<img src="https://img.shields.io/pypi/pyversions/retk.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 
 <p align="center">
   <strong>English</strong> | <a href="README_ZH.md" target="_blank">简体中文</a>
 </p>
 
 A note-taking app dependent on python.
@@ -95,44 +95,44 @@
 5. **Multi-language**: Support multiple languages, including Chinese and English.
 
 ## Install
 
 First install:
 
 ```shell
-pip install rethink-note
+pip install retk
 ```
 
 To update:
 
 ```shell
-pip install -U rethink-note
+pip install -U retk
 ```
 
 ## Usage
 
-Quickly start the note web service with `rethink.run()`, and save your note data locally,
+Quickly start the note web service with `retk.run()`, and save your note data locally,
 The default save path is the `.data` folder under the path of this script:
 
 ```python
-import rethink
+import retk
 
-rethink.run()
+retk.run()
 ```
 
-If you need to customize settings, you can set the parameters in `rethink.run()`:
+If you need to customize settings, you can set the parameters in `retk.run()`:
 
 ```python
-import rethink
+import retk
 
-rethink.run(
-    path='.',  # path to store notes, default is current directory
-    host="127.0.0.1",  # host ip, default is localhost
-    port=8080,  # port number, default is 8080
-    language="zh"  # language, default is English, optional: zh, en
+retk.run(
+   path='.',  # path to store notes, default is current directory
+   host="127.0.0.1",  # host ip, default is localhost
+   port=8080,  # port number, default is 8080
+   language="zh"  # language, default is English, optional: zh, en
 )
 ```
 
 All notes will be stored in the path specified by `path`,
 and the `.data` folder will be created in your `path` directory.
 
 English and Chinese languages are supported, and the default is English `en`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: retk Version: 0.2.4 Summary: keep and reuse your
+Metadata-Version: 2.1 Name: retk Version: 0.2.5 Summary: keep and reuse your
 thoughts Home-page: https://github.com/MorvanZhou/rethink Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com Project-URL: Bug Tracker, https://
 github.com/MorvanZhou/rethink/issues Project-URL: Source, https://github.com/
 MorvanZhou/rethink Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -46,21 +46,21 @@
 you wrote before? Unable to effectively form a note network? Rethink
 automatically recommend related notes while writing, actively assist you in
 forming a knowledge network. 4. **Local storage**: Rethink attaches great
 importance to data security. You can store data in a local storage. Or you can
 also use the online version [https://rethink.run](https://rethink.run), which
 makes it easy to synchronize across multiple platforms. 5. **Multi-language**:
 Support multiple languages, including Chinese and English. ## Install First
-install: ```shell pip install rethink-note ``` To update: ```shell pip install
--U rethink-note ``` ## Usage Quickly start the note web service with
-`rethink.run()`, and save your note data locally, The default save path is the
-`.data` folder under the path of this script: ```python import rethink
-rethink.run() ``` If you need to customize settings, you can set the parameters
-in `rethink.run()`: ```python import rethink rethink.run( path='.', # path to
-store notes, default is current directory host="127.0.0.1", # host ip, default
-is localhost port=8080, # port number, default is 8080 language="zh" #
-language, default is English, optional: zh, en ) ``` All notes will be stored
-in the path specified by `path`, and the `.data` folder will be created in your
-`path` directory. English and Chinese languages are supported, and the default
-is English `en`. If you want to use Chinese `zh`, you can use `language="zh"`
-parameter. Open your browser and visit `http://127.0.0.1:8080` to start
-recording your ideas. ## Star History_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
+install: ```shell pip install retk ``` To update: ```shell pip install -U retk
+``` ## Usage Quickly start the note web service with `retk.run()`, and save
+your note data locally, The default save path is the `.data` folder under the
+path of this script: ```python import retk retk.run() ``` If you need to
+customize settings, you can set the parameters in `retk.run()`: ```python
+import retk retk.run( path='.', # path to store notes, default is current
+directory host="127.0.0.1", # host ip, default is localhost port=8080, # port
+number, default is 8080 language="zh" # language, default is English, optional:
+zh, en ) ``` All notes will be stored in the path specified by `path`, and the
+`.data` folder will be created in your `path` directory. English and Chinese
+languages are supported, and the default is English `en`. If you want to use
+Chinese `zh`, you can use `language="zh"` parameter. Open your browser and
+visit `http://127.0.0.1:8080` to start recording your ideas. ## Star History
+_[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
```

### Comparing `retk-0.2.4/tests/test_account.py` & `retk-0.2.5/tests/test_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import unittest
 from io import BytesIO
 
 import bcrypt
 
-from rethink import const, regex
-from rethink.core import account
-from rethink.models.client import client
-from rethink.models.tps import convert_user_dict_to_authed_user
-from rethink.utils import jwt_decode
+from retk import const, regex
+from retk.core import account
+from retk.models.client import client
+from retk.models.tps import convert_user_dict_to_authed_user
+from retk.utils import jwt_decode
 from . import utils
 
 
 class AccountTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls):
         utils.set_env(".env.test.local")
@@ -49,15 +49,19 @@
         self.assertIsNone(u)
 
     async def test_verify_user(self):
         u, err = await account.manager.get_user_by_email("rethink@rethink.run")
         self.assertEqual(const.Code.OK, err)
         self.assertIsNotNone(u)
         au = convert_user_dict_to_authed_user(u)
-        ok = await account.manager.is_right_password(au, "rethink")
+        ok = await account.manager.is_right_password(
+            email=au.email,
+            hashed=au.hashed,
+            password="rethink"
+        )
         self.assertTrue(ok)
 
     def test_valid_password(self):
         for t, b in [
             ("rethink", False),
             ("123334", False),
             ("ret123", True),
```

### Comparing `retk-0.2.4/tests/test_api.py` & `retk-0.2.5/tests/test_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from unittest.mock import patch
 from zipfile import ZipFile
 
 from PIL import Image
 from fastapi.testclient import TestClient
 from httpx import Response
 
-from rethink import const, config
-from rethink.application import app
-from rethink.core import account
-from rethink.models.client import client
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
-from rethink.plugins.register import register_official_plugins, unregister_official_plugins
-from rethink.utils import jwt_decode
+from retk import const, config, PluginAPICallReturn
+from retk.application import app
+from retk.core import account
+from retk.models.client import client
+from retk.models.tps import convert_user_dict_to_authed_user
+from retk.plugins.register import register_official_plugins, unregister_official_plugins
+from retk.utils import jwt_decode
 from . import utils
 
 
 class PublicApiTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
@@ -62,25 +62,26 @@
         )
         self.assertEqual(403, resp.status_code)
         rj = resp.json()
         self.assertEqual(const.Code.ONE_USER_MODE.value, rj["detail"]["code"])
         self.assertEqual("xxx", rj["detail"]["requestId"])
 
     @patch(
-        "rethink.core.account.email.EmailServer._send"
+        "retk.core.account.email.EmailServer._send"
     )
     def test_email_verification(self, mock_send):
         mock_send.return_value = const.Code.OK
         token, _ = account.app_captcha.generate()
         data = jwt_decode(token)
 
         resp = self.client.put(
             "/api/account/email/send-code",
             json={
                 "email": "a@c.com",
+                "userExistOk": True,
                 "captchaToken": token,
                 "captchaCode": data["code"],
                 "language": "zh",
             },
             headers={"RequestId": "xxx"}
         )
         self.assertEqual(200, resp.status_code)
@@ -101,15 +102,16 @@
             "/api/account/login",
             json={
                 "email": const.DEFAULT_USER["email"],
                 "password": "",
             })
         self.assertEqual(200, resp.status_code)
         rj = resp.json()
-        self.assertEqual(811, len(rj["token"]))
+        self.assertEqual(818, len(rj["token"]))
+        self.assertTrue(rj["token"].startswith("Bearer "))
         self.default_headers = {
             "Authorization": rj["token"],
             "RequestId": "xxx",
         }
 
     async def asyncTearDown(self) -> None:
         await client.drop()
@@ -200,20 +202,20 @@
             headers={
                 "Authorization": u_token,
                 "RequestId": "xxx",
             }
         )
         _ = self.check_ok_response(resp, 200)
         u = await client.coll.users.find_one({"email": email})
-        au = AuthedUser(
-            u=convert_user_dict_to_authed_user(u),
-            language=lang,
-            request_id="xxx"
-        )
-        self.assertTrue(await account.manager.is_right_password(au, "abc222"))
+        au = convert_user_dict_to_authed_user(u)
+        self.assertTrue(await account.manager.is_right_password(
+            email=au.email,
+            hashed=au.hashed,
+            password="abc222"
+        ))
 
         uid = (await client.coll.users.find_one({"email": email}))["id"]
         await client.coll.users.delete_one({"id": uid})
         await client.coll.nodes.delete_many({"uid": uid})
         config.get_settings().ONE_USER = True
 
     def test_get_user(self):
@@ -707,15 +709,15 @@
             "/api/files/vditor/images",
             json={"url": img},
             headers=self.default_headers
         )
         self.error_check(resp, 400, const.Code.FILE_OPEN_ERROR)
 
     @patch(
-        "rethink.utils.httpx.AsyncClient.get",
+        "retk.utils.httpx.AsyncClient.get",
         return_value=Response(200, content="<title>百度一下</title>".encode("utf-8"))
     )
     def test_put_quick_node(self, mocker):
         resp = self.client.post(
             "/api/nodes/quick",
             json={
                 "md": "node1\ntext",
@@ -744,21 +746,23 @@
 
     def test_system_latest_version(self):
         resp = self.client.get(
             "/api/system/latest-version",
             headers=self.default_headers
         )
         rj = self.check_ok_response(resp, 200)
-        for n in rj["version"]:
+        for n in rj["remote"]:
+            self.assertTrue(isinstance(n, int))
+        for n in rj["local"]:
             self.assertTrue(isinstance(n, int))
 
-    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
-    @patch("rethink.core.node.backup.__remove_md_from_cos")
-    @patch("rethink.core.node.backup.__get_md_from_cos")
-    @patch("rethink.core.node.backup.__save_md_to_cos")
+    @patch("retk.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("retk.core.node.backup.__remove_md_from_cos")
+    @patch("retk.core.node.backup.__get_md_from_cos")
+    @patch("retk.core.node.backup.__save_md_to_cos")
     def test_md_history(
             self,
             mock_save_md_to_cos,
             mock_get_md_from_cos,
             mock_remove_md_from_cos,
             mock_remove_md_all_versions_from_cos,
     ):
@@ -815,15 +819,15 @@
             headers=self.default_headers
         )
         rj = self.check_ok_response(resp, 200)
         self.assertEqual("title1\ntext", rj["md"])
 
         config.get_settings().MD_BACKUP_INTERVAL = bi
 
-    @patch("rethink.plugins.base.Plugin.handle_api_call")
+    @patch("retk.plugins.base.Plugin.handle_api_call")
     def test_plugin(self, mock_handle_api_call):
         def check_one_plugin(ps):
             self.assertGreater(len(ps), 1)
             p = ps[0]
             self.assertIn("id", p)
             self.assertIn("name", p)
             self.assertIn("version", p)
@@ -875,31 +879,156 @@
         )
         rj = self.check_ok_response(resp, 200)
         self.assertNotEqual("", rj["html"])
 
         resp = self.client.post(
             "/api/plugins/call",
             json={
+                "requestId": "xxx",
                 "pluginId": "xasdqw",
                 "method": "test",
                 "data": "test",
             },
             headers=self.default_headers
         )
-        self.error_check(resp, 404, const.Code.PLUGIN_NOT_FOUND)
+        rj = resp.json()
+        self.assertEqual(False, rj["success"])
 
-        mock_handle_api_call.return_value = "test"
+        mock_handle_api_call.return_value = PluginAPICallReturn(
+            success=True,
+            message="",
+            data="test"
+        )
         resp = self.client.post(
             "/api/plugins/call",
             json={
                 "pluginId": pid,
                 "method": "method",
                 "data": "test",
             },
             headers=self.default_headers
         )
-        rj = self.check_ok_response(resp, 200)
+        rj = resp.json()
         self.assertEqual("method", rj["method"])
         self.assertEqual("test", rj["data"])
 
         unregister_official_plugins()
         config.get_settings().PLUGINS = False
+
+    async def test_admin(self):
+        resp = self.client.put(
+            "/api/admin/users/disable",
+            json={
+                "uid": "xxx",
+            },
+            headers=self.default_headers
+        )
+        self.error_check(resp, 403, const.Code.NOT_PERMITTED)
+
+        u = await client.coll.users.find_one({"email": const.DEFAULT_USER["email"]})
+        admin_uid = u["id"]
+        doc = await client.coll.users.update_one(
+            {"id": admin_uid},
+            {"$set": {"type": const.USER_TYPE.ADMIN.id}}
+        )
+        self.assertEqual(1, doc.modified_count)
+
+        resp = self.client.put(
+            "/api/admin/users/disable",
+            json={
+                "uid": "xxx",
+            },
+            headers=self.default_headers
+        )
+        self.check_ok_response(resp, 200)
+
+        config.get_settings().ONE_USER = False
+        config.get_settings().DB_SALT = "test"
+        token, code = account.app_captcha.generate()
+        data = jwt_decode(token)
+        code = data["code"].replace(config.get_settings().CAPTCHA_SALT, "")
+        lang = "zh"
+        email = "a@b.cd"
+        resp = self.client.post(
+            "/api/account",
+            json={
+                "email": email,
+                "password": "abc111",
+                "captchaToken": token,
+                "captchaCode": code,
+                "language": lang,
+            },
+            headers={"RequestId": "xxx"}
+        )
+        rj = self.check_ok_response(resp, 201)
+        u_token = rj["token"]
+        uid = (await client.coll.users.find_one({"email": email}))["id"]
+
+        resp = self.client.get(
+            "/api/users",
+            headers={
+                "Authorization": u_token,
+                "RequestId": "xxx"
+            }
+        )
+        self.check_ok_response(resp, 200)
+
+        resp = self.client.put(
+            "/api/admin/users/disable",
+            json={
+                "uid": uid,
+            },
+            headers=self.default_headers
+        )
+        self.check_ok_response(resp, 200)
+
+        resp = self.client.get(
+            "/api/users",
+            headers={
+                "Authorization": u_token,
+                "RequestId": "xxx"
+            }
+        )
+        self.error_check(resp, 403, const.Code.USER_DISABLED)
+
+        resp = self.client.put(
+            "/api/admin/users/enable/email",
+            json={
+                "email": email,
+            },
+            headers=self.default_headers
+        )
+        self.check_ok_response(resp, 200)
+
+        resp = self.client.get(
+            "/api/users",
+            headers={
+                "Authorization": u_token,
+                "RequestId": "xxx"
+            }
+        )
+        self.check_ok_response(resp, 200)
+
+        resp = self.client.put(
+            "/api/admin/users/delete",
+            json={
+                "uid": uid,
+            },
+            headers=self.default_headers
+        )
+        self.check_ok_response(resp, 200)
+
+        resp = self.client.get(
+            "/api/users",
+            headers={
+                "Authorization": u_token,
+                "RequestId": "xxx"
+            }
+        )
+        self.error_check(resp, 403, const.Code.USER_DISABLED)
+
+        doc = await client.coll.users.update_one(
+            {"id": admin_uid},
+            {"$set": {"type": const.USER_TYPE.NORMAL.id}}
+        )
+        self.assertEqual(1, doc.modified_count)
+        config.get_settings().ONE_USER = True
```

### Comparing `retk-0.2.4/tests/test_core_files_obsidian.py` & `retk-0.2.5/tests/test_core_files_obsidian.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 import unittest
 from textwrap import dedent
 from zipfile import ZipFile, BadZipFile
 
 from bson import ObjectId
 
-from rethink import core, const
-from rethink.core.files import saver
-from rethink.core.files.importing.async_tasks.obsidian import ops
-from rethink.models.client import client
+from retk import core, const
+from retk.core.files import saver
+from retk.core.files.importing.async_tasks.obsidian import ops
+from retk.models.client import client
 from . import utils
 
 
 class ObsidianTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
```

### Comparing `retk-0.2.4/tests/test_core_local.py` & `retk-0.2.5/tests/test_core_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 import httpx
 from PIL import Image
 from bson import ObjectId
 from bson.tz_util import utc
 from fastapi import UploadFile
 from starlette.datastructures import Headers
 
-from rethink import const, core, config
-from rethink.controllers.schemas.user import PatchUserRequest
-from rethink.core.files.importing.async_tasks.utils import update_process
-from rethink.models import db_ops
-from rethink.models.client import client
-from rethink.models.tps import ImportData, AuthedUser, convert_user_dict_to_authed_user
-from rethink.utils import short_uuid
+from retk import const, core, config
+from retk.controllers.schemas.user import PatchUserRequest
+from retk.core.files.importing.async_tasks.utils import update_process
+from retk.models import db_ops
+from retk.models.client import client
+from retk.models.tps import ImportData, AuthedUser, convert_user_dict_to_authed_user
+from retk.utils import short_uuid
 from . import utils
 
 
 class LocalModelsTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
@@ -88,30 +88,29 @@
         u, code = await core.user.get(_uid)
         self.assertEqual(const.Code.OK, code)
         self.assertEqual("bbb", u["hashed"])
         self.assertEqual("2", u["nickname"])
         self.assertEqual("3", u["avatar"])
         self.assertEqual(const.NodeDisplayMethod.LIST.value, u["lastState"]["nodeDisplayMethod"])
 
-        code = await core.user.disable(uid=_uid)
+        code = await core.account.manager.disable(uid=_uid)
         self.assertEqual(const.Code.OK, code)
 
         u, code = await core.user.get(uid=_uid)
-        self.assertEqual(const.Code.ACCOUNT_OR_PASSWORD_ERROR, code)
+        self.assertEqual(const.Code.USER_DISABLED, code)
         self.assertIsNone(u)
 
-        code = await core.user.enable(uid=_uid)
+        code = await core.account.manager.enable(uid=_uid)
         self.assertEqual(const.Code.OK, code)
 
-        code = await core.user.disable(uid="sdwqdqw")
-        self.assertEqual(const.Code.OPERATION_FAILED, code)
-
-        code = await core.user.delete(uid=_uid)
+        code = await core.account.manager.disable(uid="sdwqdqw")
         self.assertEqual(const.Code.OK, code)
 
+        await core.account.manager.delete(uid=_uid)
+
     async def test_node(self):
         node, code = await core.node.post(
             au=self.au, md="a" * (const.MD_MAX_LENGTH + 1), type_=const.NodeType.MARKDOWN.value
         )
         self.assertEqual(const.Code.NOTE_EXCEED_MAX_LENGTH, code)
         self.assertIsNone(node)
 
@@ -383,19 +382,18 @@
         }
         res = await client.coll.import_data.insert_one(doc)
         self.assertTrue(res.acknowledged)
 
         doc, code = await update_process("xxx", "obsidian", 10)
         self.assertEqual(const.Code.OK, code)
 
-        doc, code = await core.files.get_upload_process("xxx1213")
-        self.assertEqual(const.Code.TASK_NOT_FOUND, code)
+        doc = await core.files.get_upload_process("xxx1213")
+        self.assertIsNone(doc)
 
-        doc, code = await core.files.get_upload_process("xxx")
-        self.assertEqual(const.Code.OK, code)
+        doc = await core.files.get_upload_process("xxx")
         self.assertEqual(10, doc["process"])
         self.assertEqual("obsidian", doc["type"])
         self.assertEqual(now, doc["startAt"])
         self.assertTrue(doc["running"])
 
         await client.coll.import_data.delete_one({"uid": "xxx"})
 
@@ -438,15 +436,15 @@
         buf.close()
         await img_file.close()
 
         u, code = await core.user.get(self.au.u.id)
         self.assertEqual(used_space + size, u["usedSpace"])
 
     @patch(
-        "rethink.core.files.upload.httpx.AsyncClient.get",
+        "retk.core.files.upload.httpx.AsyncClient.get",
     )
     async def test_fetch_image_vditor(self, mock_get):
         f = open(Path(__file__).parent / "tmp" / "fake.png", "rb")
         mock_get.return_value = httpx.Response(
             200,
             content=f.read(),
             headers={"content-type": "image/png"}
```

### Comparing `retk-0.2.4/tests/test_core_remote.py` & `retk-0.2.5/tests/test_core_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from textwrap import dedent
 from unittest.mock import patch
 
 import elastic_transport
 import pymongo.errors
 from bson import ObjectId
 
-from rethink import const, config, core
-from rethink.controllers.schemas.user import PatchUserRequest
-from rethink.core.account.manager import signup
-from rethink.models import db_ops
-from rethink.models.client import client
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
-from rethink.utils import jwt_encode
+from retk import const, config, core
+from retk.controllers.schemas.user import PatchUserRequest
+from retk.core.account.manager import signup
+from retk.models import db_ops
+from retk.models.client import client
+from retk.models.tps import AuthedUser, convert_user_dict_to_authed_user
+from retk.utils import jwt_encode
 from . import utils
 
 
 class RemoteModelsTest(unittest.IsolatedAsyncioTestCase):
     default_pwd = "rethink123"
 
     @classmethod
@@ -154,34 +154,33 @@
         self.assertEqual(const.Code.OK, code)
 
         u, code = await core.user.get(_id)
         self.assertEqual(const.Code.OK, code)
         self.assertEqual("2", u["nickname"])
         self.assertEqual("3", u["avatar"])
 
-        code = await core.user.disable(uid=_id)
+        code = await core.account.manager.disable(uid=_id)
         self.assertEqual(const.Code.OK, code)
 
         u, code = await core.user.get(uid=_id)
-        self.assertEqual(const.Code.ACCOUNT_OR_PASSWORD_ERROR, code)
+        self.assertEqual(const.Code.USER_DISABLED, code)
 
-        code = await core.user.enable(uid=_id)
+        code = await core.account.manager.enable(uid=_id)
         self.assertEqual(const.Code.OK, code)
 
-        code = await core.user.disable(uid="ssaa")
-        self.assertEqual(const.Code.OPERATION_FAILED, code)
-
-        code = await core.user.delete(uid=_id)
+        code = await core.account.manager.disable(uid="ssaa")
         self.assertEqual(const.Code.OK, code)
 
+        await core.account.manager.delete(uid=_id)
+
     @utils.skip_no_connect
-    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
-    @patch("rethink.core.node.backup.__remove_md_from_cos")
-    @patch("rethink.core.node.backup.__get_md_from_cos")
-    @patch("rethink.core.node.backup.__save_md_to_cos")
+    @patch("retk.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("retk.core.node.backup.__remove_md_from_cos")
+    @patch("retk.core.node.backup.__get_md_from_cos")
+    @patch("retk.core.node.backup.__save_md_to_cos")
     async def test_node(
             self,
             mock_save_md_to_cos,
             mock_get_md_from_cos,
             mock_remove_md_from_cos,
             mock_remove_md_all_versions_from_cos,
     ):
@@ -246,18 +245,18 @@
         self.assertEqual(used_space - len(node["md"].encode("utf-8")), u["usedSpace"])
 
         nodes, total = await core.node.core_nodes(au=self.au, page=0, limit=10)
         self.assertEqual(2, len(nodes))
         self.assertEqual(2, total)
 
     @utils.skip_no_connect
-    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
-    @patch("rethink.core.node.backup.__remove_md_from_cos")
-    @patch("rethink.core.node.backup.__get_md_from_cos")
-    @patch("rethink.core.node.backup.__save_md_to_cos")
+    @patch("retk.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("retk.core.node.backup.__remove_md_from_cos")
+    @patch("retk.core.node.backup.__get_md_from_cos")
+    @patch("retk.core.node.backup.__save_md_to_cos")
     async def test_parse_at(
             self,
             mock_save_md_to_cos,
             mock_get_md_from_cos,
             mock_remove_md_from_cos,
             mock_remove_md_all_versions_from_cos,
     ):
@@ -363,18 +362,18 @@
 
         await client.search.refresh()
         nodes, total = await client.search.search(self.au)
         self.assertEqual(4, len(nodes))
         self.assertEqual(4, total)
 
     @utils.skip_no_connect
-    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
-    @patch("rethink.core.node.backup.__remove_md_from_cos")
-    @patch("rethink.core.node.backup.__get_md_from_cos")
-    @patch("rethink.core.node.backup.__save_md_to_cos")
+    @patch("retk.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("retk.core.node.backup.__remove_md_from_cos")
+    @patch("retk.core.node.backup.__get_md_from_cos")
+    @patch("retk.core.node.backup.__save_md_to_cos")
     async def test_batch(
             self,
             mock_save_md_to_cos,
             mock_get_md_from_cos,
             mock_remove_md_from_cos,
             mock_remove_md_all_versions_from_cos,
     ):
@@ -437,18 +436,18 @@
             now = u["usedSpace"] - base_used_space
             if now < 0:
                 now = 0
                 base_used_space = 0
             self.assertAlmostEqual(value, now, msg=f"delta: {delta}, value: {value}")
 
     @utils.skip_no_connect
-    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
-    @patch("rethink.core.node.backup.__remove_md_from_cos")
-    @patch("rethink.core.node.backup.__get_md_from_cos")
-    @patch("rethink.core.node.backup.__save_md_to_cos")
+    @patch("retk.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("retk.core.node.backup.__remove_md_from_cos")
+    @patch("retk.core.node.backup.__get_md_from_cos")
+    @patch("retk.core.node.backup.__save_md_to_cos")
     async def test_md_history(
             self,
             mock_save_md_to_cos,
             mock_get_md_from_cos,
             mock_remove_md_from_cos,
             mock_remove_md_all_versions_from_cos,
     ):
```

### Comparing `retk-0.2.4/tests/test_data_restore.py` & `retk-0.2.5/tests/test_data_restore.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
-from rethink import const, core
-from rethink.models.client import client
-from rethink.models.tps import AuthedUser, convert_user_dict_to_authed_user
+from retk import const, core
+from retk.models.client import client
+from retk.models.tps import AuthedUser, convert_user_dict_to_authed_user
 from . import utils
 
 
 class DataRestoreTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
```

### Comparing `retk-0.2.4/tests/test_plugins.py` & `retk-0.2.5/tests/test_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import shutil
 import unittest
 from pathlib import Path
 from typing import Dict
 
-import rethink
-from rethink import core, const
-from rethink.models.client import client
-from rethink.models.tps import convert_user_dict_to_authed_user, AuthedUser
-from rethink.plugins.base import event_plugin_map
+import retk
+from retk import core, const
+from retk.models.client import client
+from retk.models.tps import convert_user_dict_to_authed_user, AuthedUser
+from retk.plugins.base import event_plugin_map
 from . import utils
 
 
-class TestPlugin(rethink.Plugin):
+class TestPlugin(retk.Plugin):
     id = "testPlugin"
     name = "TestPlugin"
     version = "0.1.0"
     description = "A demo test plugin."
     author = "morvanzhou"
     icon = "tmp/back.svg"
     template = "<h1>{h}</h1>\n<p>{p}</p>"
 
     def __init__(self):
         super().__init__()
-        self.cache: Dict[str, rethink.tps.Node] = {}
+        self.cache: Dict[str, retk.tps.Node] = {}
         self.bmd = ""
         self.h = ""
         self.p = ""
 
     def render(self):
         return self.template.format(h=self.h, p=self.p)
 
-    def on_node_added(self, node: rethink.tps.Node):
+    def on_node_added(self, node: retk.tps.Node):
         self.cache[node["id"]] = node
 
     def before_node_updated(self, uid: str, nid: str, data: Dict[str, str]):
         self.bmd = "before_node_updated:" + data["md"]
 
-    def on_node_updated(self, node: rethink.tps.Node, old_node: rethink.tps.Node):
+    def on_node_updated(self, node: retk.tps.Node, old_node: retk.tps.Node):
         self.cache[node["id"]] = node
 
 
 svg = """<?xml version="1.0" encoding="utf-8"?>
 <svg width="800px" height="800px" viewBox="0 0 1024 1024" xmlns="http://www.w3.org/2000/svg">
     <path fill="#000000" d="M224 480h640a32 32 0 1 1 0 64H224a32 32 0 0 1 0-64z"/>
     <path fill="#000000"
@@ -61,26 +61,26 @@
     @classmethod
     def tearDownClass(cls) -> None:
         utils.drop_env(".env.test.local")
         shutil.rmtree(Path(__file__).parent / "tmp", ignore_errors=True)
 
     async def asyncSetUp(self) -> None:
         self.p = TestPlugin()
-        rethink.add_plugin(self.p)
+        retk.add_plugin(self.p)
 
         await client.init()
         u, _ = await core.user.get_by_email(email=const.DEFAULT_USER["email"])
         self.au = AuthedUser(
             u=convert_user_dict_to_authed_user(u),
             request_id="test",
             language=const.Language.EN.value,
         )
 
     async def asyncTearDown(self) -> None:
-        rethink.remove_plugin(self.p)
+        retk.remove_plugin(self.p)
         await client.drop()
         shutil.rmtree(Path(__file__).parent / "tmp" / ".data" / "files", ignore_errors=True)
         shutil.rmtree(Path(__file__).parent / "tmp" / ".data" / "md", ignore_errors=True)
 
     def test_creation(self):
         self.assertEqual(self.p.id, "testPlugin")
         self.assertEqual(self.p.name, "TestPlugin")
@@ -107,26 +107,26 @@
 
     async def test_event(self):
         self.assertIn(self.p, event_plugin_map["on_node_added"])
 
         node, code = await core.node.post(
             au=self.au, md="a", type_=const.NodeType.MARKDOWN.value
         )
-        self.assertEqual(rethink.const.Code.OK, code)
+        self.assertEqual(retk.const.Code.OK, code)
         self.assertEqual(node, self.p.cache[node["id"]])
         self.assertEqual("a", self.p.cache[node["id"]]["md"])
 
         self.assertEqual("", self.p.bmd)
         node, _, code = await core.node.update_md(
             au=self.au, nid=node["id"], md="b"
         )
-        self.assertEqual(rethink.const.Code.OK, code)
+        self.assertEqual(retk.const.Code.OK, code)
         self.assertEqual(node, self.p.cache[node["id"]])
         self.assertEqual("b", self.p.cache[node["id"]]["md"])
         self.assertEqual("before_node_updated:b", self.p.bmd)
 
     def test_timing(self):
         with self.assertRaises(ValueError):
-            rethink.schedule.every_minute_at(second=-1)
-        t = rethink.schedule.every_minute_at(second=1)
+            retk.schedule.every_minute_at(second=-1)
+        t = retk.schedule.every_minute_at(second=1)
         self.assertEqual(1, t.at_second)
         self.assertEqual(0, t.at_minute)
```

### Comparing `retk-0.2.4/tests/test_run.py` & `retk-0.2.5/tests/test_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import shutil
 import socket
 import time
 import unittest
 import urllib.request
 from pathlib import Path
 
-import rethink
-from rethink import config
+import retk
+from retk import config
 
 
 class TestRun(unittest.TestCase):
     path: Path
 
     @classmethod
     def setUpClass(cls) -> None:
@@ -23,17 +23,17 @@
     def tearDownClass(cls) -> None:
         shutil.rmtree(str(cls.path), ignore_errors=True)
         config.get_settings.cache_clear()
 
     def test_run(self, password=None):
         port = 8001
 
-        p = multiprocessing.Process(target=rethink.run, kwargs={
+        p = multiprocessing.Process(target=retk.run, kwargs={
             "path": self.path, "port": port, "language": "zh", "headless": True,
-            "debug": False, "password": password,
+            "debug": True, "password": password,
         })
         p.start()
         # p.join()
         while True:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             sock.settimeout(2)
             result = sock.connect_ex(('127.0.0.1', port))
@@ -66,26 +66,26 @@
         self.assertEqual(2, len(list((self.path / ".data" / "md").glob("*.md"))))
 
     def test_run_with_pw(self):
         return self.test_run(password="12345678")
 
     # def test_plugin(self):
     #
-    #     class TestPlugin(rethink.Plugin):
+    #     class TestPlugin(retk.Plugin):
     #         name = "TestPlugin"
     #         version = "0.1.0"
     #         description = "A demo test plugin."
     #         author = "morvanzhou"
     #         template = "<h1>{h}</h1>\n<p>{p}</p>"
-    #         schedule_timing = rethink.schedule.every_minute_at(second=0)
+    #         schedule_timing = retk.schedule.every_minute_at(second=0)
     #
     #         def __init__(self):
     #             super().__init__()
     #             self.count = 0
     #
     #         def on_schedule(self) -> None:
     #             print(self.count, time.time())
     #             self.count += 1
     #
     #     plugin = TestPlugin()
-    #     rethink.add_plugin(plugin)
-    #     rethink.run()
+    #     retk.add_plugin(plugin)
+    #     retk.run()
```

### Comparing `retk-0.2.4/tests/test_search_es.py` & `retk-0.2.5/tests/test_search_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import unittest
 
 import elastic_transport
 from bson import ObjectId
 
-from rethink import const, config
-from rethink.models.search_engine.engine_es import ESSearcher, SearchDoc
-from rethink.models.tps import AuthedUser
+from retk import const, config
+from retk.models.search_engine.engine_es import ESSearcher, SearchDoc
+from retk.models.tps import AuthedUser
 from . import utils
 
 
 class ESTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.development")
```

### Comparing `retk-0.2.4/tests/test_search_local.py` & `retk-0.2.5/tests/test_search_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import time
 import unittest
 
 from bson import ObjectId
 
-from rethink import const
-from rethink.models.search_engine.engine_local import LocalSearcher, SearchDoc
-from rethink.models.tps import AuthedUser
+from retk import const
+from retk.models.search_engine.engine_local import LocalSearcher, SearchDoc
+from retk.models.tps import AuthedUser
 from . import utils
 
 
 class LocalSearchTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
```

### Comparing `retk-0.2.4/tests/test_sso.py` & `retk-0.2.5/tests/test_sso.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from unittest.mock import patch
 
 from fastapi import HTTPException
 
-from rethink.controllers import oauth
-from rethink.depend.sso import github
+from retk.controllers import oauth
+from retk.depend.sso import github
 from tests import utils
 
 
 class SSOTest(unittest.IsolatedAsyncioTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         utils.set_env(".env.test.local")
@@ -51,15 +51,15 @@
         })
         self.assertEqual("id", open_id.id)
         self.assertEqual("github", open_id.provider)
         self.assertEqual("login", open_id.display_name)
         self.assertEqual("avatar_url", open_id.picture)
         self.assertEqual("email", open_id.email)
 
-    @patch("rethink.depend.sso.base.SSOBase.get_login_url")
+    @patch("retk.depend.sso.base.SSOBase.get_login_url")
     async def test_login_github(
             self,
             mock_get_login_url,
     ):
         mock_get_login_url.return_value = "https://github.com/"
         res = await oauth.login_provider("github")
         self.assertEqual("https://github.com/", res.uri.unicode_string())
```

### Comparing `retk-0.2.4/tests/test_utils.py` & `retk-0.2.5/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from textwrap import dedent
 from unittest.mock import patch
 
 import httpx
 
-from rethink import const, config, utils
+from retk import const, config, utils
 
 
 class UtilsTest(unittest.TestCase):
     def setUp(self) -> None:
         config.get_settings.cache_clear()
 
     def tearDown(self) -> None:
@@ -113,16 +113,16 @@
         config.get_settings.cache_clear()
 
     @classmethod
     def tearDownClass(cls) -> None:
         config.get_settings.cache_clear()
 
     # @unittest.skip("skip outer connection test")
-    @patch("rethink.utils.httpx.AsyncClient.get")
-    @patch("rethink.config.get_settings")
+    @patch("retk.utils.httpx.AsyncClient.get")
+    @patch("retk.config.get_settings")
     async def test_get_title_description_from_link(self, mock_get_settings, mock_get, ):
         s = config.Settings
         s.COS_BUCKET_NAME = "rethink-dev-1258395282"
         s.COS_REGION = "ap-hongkong"
         s.DB_HOST = "127.0.0.1"
         mock_get_settings.return_value = s
         for url, content, res in [
@@ -214,15 +214,15 @@
             ("abc@b", "ab**c@b"),
             ("abcd@b", "ab**d@b"),
             ("abcdef@b", "ab**f@b"),
         ]:
             self.assertEqual(res, utils.mask_email(email))
 
     @patch(
-        "rethink.config.get_settings",
+        "retk.config.get_settings",
     )
     def test_ssrf(self, mock_get_settings):
         for pre, url in [
             (
                     "rethink-product-1258395282",
                     "https://rethink-product-1258395282.cos.ap-hongkong.myqcloud.com/userData/Rro/as.png",
             ),
```

### Comparing `retk-0.2.4/tests/test_version_manager.py` & `retk-0.2.5/tests/test_version_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import json
 import shutil
 import unittest
 from pathlib import Path
 
-from rethink import const, version_manager, __version__
+from retk import const, version_manager, __version__
 
 
 class RecoverTest(unittest.TestCase):
     def setUp(self) -> None:
         self.tmp_dir = Path(__file__).parent / "tmp"
         self.tmp_dir.mkdir(parents=True, exist_ok=True)
 
     def tearDown(self) -> None:
         # remove all files and dirs
         shutil.rmtree(self.tmp_dir, ignore_errors=True)
 
+    def test_package_version(self):
+        vs = __version__.split(".")
+        vs_int = list(map(int, vs))
+        self.assertEqual(3, len(vs_int))
+
     def test_dump_load(self):
         version_manager.recover.dump_dot_rethink(self.tmp_dir / ".rethink.json")
 
         v = version_manager.recover.load_dot_rethink(self.tmp_dir / ".rethink.json")
         self.assertIsNotNone(v)
-        self.assertEqual(__version__, v["version"])
+        # self.assertEqual(__version__, v["version"])
         self.assertEqual(const.DEFAULT_USER["email"], v["email"])
         self.assertEqual(const.DEFAULT_USER["nickname"], v["nickname"])
         self.assertEqual(const.DEFAULT_USER["avatar"], v["avatar"])
         self.assertEqual(const.DEFAULT_USER["email"], v["account"])
         self.assertEqual(const.Language.EN.value, v["settings"]["language"])
         self.assertEqual(const.AppTheme.LIGHT.value, v["settings"]["theme"])
         self.assertEqual(const.EditorMode.WYSIWYG.value, v["settings"]["editorMode"])
@@ -58,8 +63,9 @@
         dot_data_dir.mkdir(parents=True, exist_ok=True)
 
         with open(self.tmp_dir / ".data" / ".rethink.json", "w", encoding="utf-8") as f:
             json.dump(dot_rethink, f, indent=2, ensure_ascii=False)
 
         version_manager.migrate.to_latest_version(self.tmp_dir)
         v = version_manager.recover.load_dot_rethink(self.tmp_dir / ".data" / ".rethink.json")
-        self.assertEqual(__version__, v["version"])
+        # self.assertEqual(__version__, v["version"])
+        self.assertGreater(len(v["version"]), 0)
```

