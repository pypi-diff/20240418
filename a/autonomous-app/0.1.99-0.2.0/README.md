# Comparing `tmp/autonomous-app-0.1.99.tar.gz` & `tmp/autonomous_app-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.99.tar", last modified: Mon Dec 18 19:30:00 2023, max compression
+gzip compressed data, was "autonomous_app-0.2.0.tar", last modified: Wed Apr 17 21:27:46 2024, max compression
```

## Comparing `autonomous-app-0.1.99.tar` & `autonomous_app-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,55 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.153805 autonomous-app-0.1.99/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.99/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 19:30:00.152805 autonomous-app-0.1.99/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2012 2023-08-02 17:40:38.000000 autonomous-app-0.1.99/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.99/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      536 2023-12-18 15:47:18.000000 autonomous-app-0.1.99/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-12-18 19:30:00.153805 autonomous-app-0.1.99/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.99/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.130805 autonomous-app-0.1.99/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.134805 autonomous-app-0.1.99/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       87 2023-12-18 19:26:51.000000 autonomous-app-0.1.99/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.135805 autonomous-app-0.1.99/src/autonomous/ai/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       31 2023-11-11 17:40:30.000000 autonomous-app-0.1.99/src/autonomous/ai/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.137805 autonomous-app-0.1.99/src/autonomous/ai/agents/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3767 2023-11-25 02:11:35.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/autogen.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      442 2023-11-21 17:15:45.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/baseagent.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1681 2023-11-25 02:14:34.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/local.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1535 2023-11-21 18:06:03.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/mockai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4041 2023-11-21 17:36:18.000000 autonomous-app-0.1.99/src/autonomous/ai/agents/openai.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1255 2023-12-02 03:55:36.000000 autonomous-app-0.1.99/src/autonomous/ai/autoteam.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.137805 autonomous-app-0.1.99/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-10-27 15:43:10.000000 autonomous-app-0.1.99/src/autonomous/apis/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.139805 autonomous-app-0.1.99/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.99/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.140805 autonomous-app-0.1.99/src/autonomous/apis/wikijs/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       24 2023-09-17 14:05:05.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     7803 2023-12-05 17:36:34.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/api.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      699 2023-11-12 04:29:55.000000 autonomous-app-0.1.99/src/autonomous/apis/wikijs/page.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.129805 autonomous-app-0.1.99/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.141805 autonomous-app-0.1.99/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       54 2023-07-28 15:13:30.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      941 2023-10-31 13:06:19.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/api.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1634 2023-10-31 13:53:35.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      795 2023-10-31 13:04:04.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.142805 autonomous-app-0.1.99/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      239 2023-11-02 16:15:57.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/models/model.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      548 2023-10-31 13:57:31.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.143805 autonomous-app-0.1.99/src/autonomous/app_template/app/views/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/__init__.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      384 2023-10-31 13:03:32.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/admin.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.143805 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      464 2023-10-31 13:02:03.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/api/task.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)     2248 2023-11-03 17:59:06.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/auth.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      657 2023-11-25 02:27:16.000000 autonomous-app-0.1.99/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.144805 autonomous-app-0.1.99/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      545 2023-07-28 15:11:47.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/conftest.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      225 2023-11-08 20:35:25.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      964 2023-11-08 21:07:18.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_auth.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2467 2023-10-31 13:57:41.000000 autonomous-app-0.1.99/src/autonomous/app_template/tests/test_tasks.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.145805 autonomous-app-0.1.99/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1132 2023-10-06 16:58:12.000000 autonomous-app-0.1.99/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2080 2023-12-02 03:44:55.000000 autonomous-app-0.1.99/src/autonomous/assets.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.146805 autonomous-app-0.1.99/src/autonomous/auth/
--rw-r--r--   0 samoore   (1000) samoore   (1000)      161 2023-10-30 19:07:42.000000 autonomous-app-0.1.99/src/autonomous/auth/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3299 2023-12-16 21:28:15.000000 autonomous-app-0.1.99/src/autonomous/auth/autoauth.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      886 2023-10-08 14:52:15.000000 autonomous-app-0.1.99/src/autonomous/auth/github.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1049 2023-10-06 19:49:20.000000 autonomous-app-0.1.99/src/autonomous/auth/google.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2153 2023-12-16 21:30:14.000000 autonomous-app-0.1.99/src/autonomous/auth/user.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.99/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.146805 autonomous-app-0.1.99/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1485 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     7609 2023-11-30 18:58:13.000000 autonomous-app-0.1.99/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1460 2023-11-13 19:36:43.000000 autonomous-app-0.1.99/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.147805 autonomous-app-0.1.99/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-11-02 16:21:48.000000 autonomous-app-0.1.99/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      586 2023-11-07 17:04:09.000000 autonomous-app-0.1.99/src/autonomous/model/autoattribute.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)    12318 2023-12-08 19:50:29.000000 autonomous-app-0.1.99/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      733 2023-11-22 00:01:47.000000 autonomous-app-0.1.99/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.149805 autonomous-app-0.1.99/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       49 2023-09-09 15:30:58.000000 autonomous-app-0.1.99/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2350 2023-12-12 17:00:48.000000 autonomous-app-0.1.99/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2815 2023-12-18 19:24:04.000000 autonomous-app-0.1.99/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2286 2023-12-18 15:10:22.000000 autonomous-app-0.1.99/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3885 2023-11-29 14:43:31.000000 autonomous-app-0.1.99/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.149805 autonomous-app-0.1.99/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       32 2023-08-25 19:55:23.000000 autonomous-app-0.1.99/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4379 2023-11-17 16:47:39.000000 autonomous-app-0.1.99/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-12-18 19:30:00.151805 autonomous-app-0.1.99/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4293 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2555 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      182 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-12-18 19:30:00.000000 autonomous-app-0.1.99/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.584751 autonomous_app-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-17 21:27:46.584751 autonomous_app-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:27:46.584751 autonomous_app-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.576750 autonomous_app-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.576750 autonomous_app-0.2.0/src/autonomous/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-17 21:27:21.000000 autonomous_app-0.2.0/src/autonomous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.576750 autonomous_app-0.2.0/src/autonomous/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.0/src/autonomous/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7829 2024-04-17 21:26:48.000000 autonomous_app-0.2.0/src/autonomous/ai/oaiagent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/auth/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.0/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/auth/github.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/auth/google.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.0/src/autonomous/auth/user.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/db/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.0/src/autonomous/db/autodb.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.0/src/autonomous/db/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/errors/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/errors/danglingreferenceerror.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/model/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.0/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.0/src/autonomous/model/automodel.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.0/src/autonomous/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.0/src/autonomous/model/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.0/src/autonomous/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.0/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.0/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/storage/version_control/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/version_control/GHCallbacks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/version_control/GHOrganization.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/version_control/GHRepo.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/version_control/GHVersionControl.py
+-rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/storage/version_control/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.580751 autonomous_app-0.2.0/src/autonomous/tasks/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.0/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:27:46.584751 autonomous_app-0.2.0/src/autonomous_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-17 21:27:46.000000 autonomous_app-0.2.0/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-17 21:27:46.000000 autonomous_app-0.2.0/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:27:46.000000 autonomous_app-0.2.0/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-17 21:27:46.000000 autonomous_app-0.2.0/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-17 21:27:46.000000 autonomous_app-0.2.0/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.99/LICENSE` & `autonomous_app-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/PKG-INFO` & `autonomous_app-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.99
+Version: 0.2.0
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,95 +21,91 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: homepage, https://github.com/Sallenmoore/autonomous
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: icecream
 Requires-Dist: setuptools
 Requires-Dist: python-dotenv
 Requires-Dist: PyGithub
 Requires-Dist: pygit2
 Requires-Dist: cloudinary
 Requires-Dist: pillow
-Requires-Dist: redis
+Requires-Dist: pymongo
 Requires-Dist: jsmin
 Requires-Dist: requests
 Requires-Dist: gunicorn
 Requires-Dist: Authlib
-Requires-Dist: rq
-Requires-Dist: rq-dashboard
-Requires-Dist: pyautogen
-Requires-Dist: openai
+Requires-Dist: openai>=1.21.1
 Requires-Dist: validators
 Requires-Dist: dateparser
 Requires-Dist: python-slugify
 
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask.
-The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
+A self-contained containerized Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
-- Built-in Local NoSQL database and Model API
-- Cloud file storage with Cloudinary or S3
-- Auto-Generated Documentation Pages (Coming Soon!!!)
+- Container based MongoDB database
+- Model ORM API
+- File storage locally or with services such as Cloudinary or S3 
+- Separate service for long running tasks
+- Built-in Authentication with Google or Github
+- Auto-Generated Documentation Pages
 
 ## Dependencies
 
 - **Languages**
-  - [Python 3.10](/Dev/language/python)
+  - [Python 3.11](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
   - [Docker](https://docs.docker.com/)
   - [Docker Compose](https://github.com/compose-spec/compose-spec/blob/master/spec.md)
 - **Server**
   - [nginx](https://docs.nginx.com/nginx/)
   - [gunicorn](https://docs.gunicorn.org/en/stable/configure.html)
 - **Networking and Serialization**
   - [requests](https://requests.readthedocs.io/en/latest/)
 - **Database**
-  - [Local](https://tinydb.readthedocs.io/en/latest/)
+  - [pymongo](https://pymongo.readthedocs.io/en/stable/api/pymongo/index.html)
 - **Testing**
   - [pytest](/Dev/tools/pytest)
   - [coverage](https://coverage.readthedocs.io/en/6.4.1/cmd.html)
 - **Documentation** - Coming Soon
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
-  - [highlight.js](https://highlightjs.org/)
-
 ---
 
 ## Developer Notes
 
 ### TODO
 
-- Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
-- Add more database options
 - 100% testing coverage
 
 ### Issue Tracking
 
 - None
 
 ## Processes
```

### Comparing `autonomous-app-0.1.99/README.md` & `autonomous_app-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask.
-The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
+A self-contained containerized Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
-- Built-in Local NoSQL database and Model API
-- Cloud file storage with Cloudinary or S3
-- Auto-Generated Documentation Pages (Coming Soon!!!)
+- Container based MongoDB database
+- Model ORM API
+- File storage locally or with services such as Cloudinary or S3 
+- Separate service for long running tasks
+- Built-in Authentication with Google or Github
+- Auto-Generated Documentation Pages
 
 ## Dependencies
 
 - **Languages**
-  - [Python 3.10](/Dev/language/python)
+  - [Python 3.11](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
   - [Docker](https://docs.docker.com/)
   - [Docker Compose](https://github.com/compose-spec/compose-spec/blob/master/spec.md)
 - **Server**
   - [nginx](https://docs.nginx.com/nginx/)
   - [gunicorn](https://docs.gunicorn.org/en/stable/configure.html)
 - **Networking and Serialization**
   - [requests](https://requests.readthedocs.io/en/latest/)
 - **Database**
-  - [Local](https://tinydb.readthedocs.io/en/latest/)
+  - [pymongo](https://pymongo.readthedocs.io/en/stable/api/pymongo/index.html)
 - **Testing**
   - [pytest](/Dev/tools/pytest)
   - [coverage](https://coverage.readthedocs.io/en/6.4.1/cmd.html)
 - **Documentation** - Coming Soon
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
-  - [highlight.js](https://highlightjs.org/)
-
 ---
 
 ## Developer Notes
 
 ### TODO
 
-- Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
-- Add more database options
 - 100% testing coverage
 
 ### Issue Tracking
 
 - None
 
 ## Processes
```

### Comparing `autonomous-app-0.1.99/pyproject.toml` & `autonomous_app-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,47 +6,41 @@
 name = "autonomous-app"
 authors = [
     {name = "Steven A Moore", email = "samoore@binghamton.edu"},
 ]
 description = "Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications."
 dynamic = ["version", "dependencies"]
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 license={file = "LICENSE"}
 classifiers=[
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 homepage="https://github.com/Sallenmoore/autonomous"
 
-[project.scripts]
-#https://setuptools.pypa.io/en/latest/userguide/entry_point.html
-autoapp = "autonomous.cli:createapp"
-
 [tool.setuptools.dynamic]
 #https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
 version = {attr = "autonomous.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.dynamic.optional-dependencies]
 dev = {file = ["requirements_dev.txt"]}
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["src"]
 include = ["autonomous*"]
 
 [tool.pytest.ini_options]
-addopts = "--cov=autonomous -rx -l -x -s --log-level=INFO --ignore=src --no-cov-on-fail -v" # --cov-reset
+addopts = "--cov=autonomous -rx -l -x -s --log-level=INFO --ignore=src --no-cov-on-fail -v --pdb --cov-reset"
+
 testpaths = [
      "tests",
 ]
 pythonpath = [
     "src/autonomous",
 ]
-log_auto_indent = true
-
-[tool.isort]
-profile = "black"
+log_auto_indent = true
```

### Comparing `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous_app-0.2.0/src/autonomous/storage/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous_app-0.2.0/src/autonomous/storage/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/apis/version_control/GHRepo.py` & `autonomous_app-0.2.0/src/autonomous/storage/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/auth/autoauth.py` & `autonomous_app-0.2.0/src/autonomous/auth/autoauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,22 @@
         )
 
     @classmethod
     def current_user(cls):
         """
         Returns the current user.
         """
+        user = cls.user_class.get_guest()
         if session.get("user") and session["user"]["state"] == "authenticated":
-            return cls.user_class.get(session["user"].get("pk"))
-        return cls.user_class.get_guest()
+            try:
+                user = cls.user_class.get(session["user"].get("pk"))
+                user.pk
+            except Exception as e:
+                log(e, session["user"])
+        return user
 
     def authenticate(self):
         """
         Initiates the authentication process.
         Returns a redirect URL which should be used to redirect the user to the OpenID provider for authentication.
         """
         uri, state = self.session.create_authorization_url(self.issuer)
@@ -70,15 +75,15 @@
         )
         # log(token)
 
         userinfo = requests.get(self.req_uri, auth=OAuth2Auth(token))
         return userinfo.json(), token
 
     @classmethod
-    def auth_required(cls, guest=False):
+    def auth_required(cls, guest=False, admin=False):
         """
         If you decorate a view with this, it will ensure that the current user is
         logged in and authenticated before calling the actual view. For
         example:
 
             @app.route('/post')
             @auth_required
@@ -91,16 +96,19 @@
         """
 
         def wrap(func):
             @wraps(func)
             def decorated_view(*args, **kwargs):
                 # log(session.get("user"))
                 user = cls.current_user()
-                if user.state == "authenticated":
+                if not user:
+                    return redirect(url_for("auth.login"))
+                elif user.state == "authenticated":
                     user.last_login = datetime.now()
+                    # log(user)
                     user.save()
                 session["user"] = user.serialize()
 
                 if not guest and user.is_guest:
                     return redirect(url_for("auth.login"))
                 return func(*args, **kwargs)
```

### Comparing `autonomous-app-0.1.99/src/autonomous/auth/github.py` & `autonomous_app-0.2.0/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/auth/google.py` & `autonomous_app-0.2.0/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/auth/user.py` & `autonomous_app-0.2.0/src/autonomous/auth/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 """
-    This module provides a User class that uses the OpenIDAuth class for authentication.
+This module provides a User class that uses the OpenIDAuth class for authentication.
 """
+
 from datetime import datetime
 
 from autonomous import log
 from autonomous.model.autoattribute import AutoAttribute
 from autonomous.model.automodel import AutoModel
 
 
 class AutoUser(AutoModel):
     """
     This class represents a user who can authenticate using OpenID.
     """
 
     attributes = {
-        "name": AutoAttribute("TEXT", required=True),
-        "email": AutoAttribute("TAG", required=True),
+        "name": AutoAttribute("TEXT"),
+        "email": AutoAttribute("TEXT", required=True),
         "last_login": datetime.now(),
         "state": "unauthenticated",
         "provider": None,
         "role": "user",
         "token": None,
     }
 
+    def __eq__(self, other):
+        return self.pk == other.pk
+
     @classmethod
     def authenticate(cls, user_info, token=None):
         """
         Initiates the authentication process.
         Returns a redirect URL which should be used to redirect the user to the OpenID provider for authentication.
         """
         email = user_info["email"].strip()
         name = user_info["name"].strip()
-        # log(cls, user_info)
         user = cls.find(email=email)
-        # log(user)
-        if not user:
-            # FIXME: attempting a lookup hack because something is fucked up
-            for u in cls.all():
-                if u.email == email:
-                    user = u
         if not user:
-            # log("Creating new user...")
+            log(f"Creating new user for {email}")
             user = cls(name=name, email=email)
 
         # parse user_info into a user object
         user.name = name
         user.email = email
         user.last_login = datetime.now()
         user.state = "authenticated"
         user.save()
-        # log(user.pk)
         return user
 
     @property
     def is_authenticated(self):
         """
         Returns True if the user is authenticated, False otherwise.
         """
         return self.state == "authenticated"
 
     @classmethod
     def get_guest(cls):
         """
         Returns a guest user.
         """
-        return cls(name="Guest", email="guest@mail.com", state="guest", role="guest")
+        guest = cls.find(name="_GuestOfAutonomous_", state="guest")
+        if not guest:
+            guest = cls(
+                name="_GuestOfAutonomous_",
+                email="guest@mail.com",
+                state="guest",
+                role="guest",
+            )
+            guest.save()
+        return guest
 
     @property
     def is_guest(self):
         """
         Returns True if the user is a guest, False otherwise.
         """
         return self.state == "guest"
```

### Comparing `autonomous-app-0.1.99/src/autonomous/logger.py` & `autonomous_app-0.2.0/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/model/autoattribute.py` & `autonomous_app-0.2.0/src/autonomous/model/autoattribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class AutoAttribute:
     def __init__(
         self, type, default=None, required=False, unique=False, primary_key=False
     ):
         if type in [
-            "TAG",
             "TEXT",
             "NUMERIC",
+            "MODEL",
         ]:
             self.type = type
         else:
             raise ValueError(f"Invalid type {type}")
 
         self.default = default
         self.required = required
```

### Comparing `autonomous-app-0.1.99/src/autonomous/model/automodel.py` & `autonomous_app-0.2.0/src/autonomous/model/automodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # opt : Optional[str]  # for optional attributes
 # default : Optional[str] = "value"  # for default values
 import copy
 import importlib
 import json
-import uuid
 from abc import ABC
 from datetime import datetime
 
 from autonomous import log
+from autonomous.errors import DanglingReferenceError
 
 from .autoattribute import AutoAttribute
 from .orm import ORM
+from .serializer import AutoDecoder, AutoEncoder
 
 
 class DelayedModel:
     def __init__(self, model, pk):
         # log(model, pk)
         assert model
         assert pk
@@ -22,27 +23,21 @@
         module = importlib.import_module(module_name)
         model = getattr(module, class_name)
         object.__setattr__(self, "_delayed_model", model)
         object.__setattr__(self, "_delayed_pk", pk)
         object.__setattr__(self, "_delayed_obj", None)
 
     def _instance(self):
+        #### DO NOT TO ANY LOGGING IN THIS METHOD; IT CAUSES INFINITE RECURSION ####
         if not object.__getattribute__(self, "_delayed_obj"):
             _pk = object.__getattribute__(self, "_delayed_pk")
             _model = object.__getattribute__(self, "_delayed_model")
-            # log(_pk, _model)
-            # breakpoint()
             _obj = _model.get(_pk)
-            # log(_obj)
-            try:
-                assert _obj
-            except AssertionError as e:
-                msg = f"{e}\n\nModel relationship error. Most likely failed to clean up dangling reference.\nModel: {_model}\npk: {_pk}\nResult: {_obj}"
-                # log(msg)
-                raise Exception(msg)
+            if not _pk or not _model or _obj is None:
+                raise DanglingReferenceError(_model, _pk, _obj)
             else:
                 object.__setattr__(self, "_delayed_obj", _obj)
 
         return object.__getattribute__(self, "_delayed_obj")
 
     # def __getattr__(self, name):
     #     return getattr(self._instance(), name)
@@ -52,48 +47,49 @@
         if name in [
             "_delayed_model",
             "_delayed_pk",
             "_delayed_obj",
             "_instance",
         ]:
             return object.__getattribute__(self, name)
-        return object.__getattribute__(self._instance(), name)
+        try:
+            return object.__getattribute__(self._instance(), name)
+        except DanglingReferenceError as e:
+            log(e)
+            return None
 
     def __setattr__(self, name, value):
         if name.startswith("_delayed"):
             object.__setattr__(self, name, value)
         else:
             setattr(self._instance(), name, value)
 
     def __delattr__(self, name):
         delattr(self._instance(), name)
 
     def __nonzero__(self):
         return bool(self._instance())
 
     def __str__(self):
-        return str(self._instance())
+        return str(self._instance().__dict__)
 
     def __repr__(self):
-        result = repr(self._delayed_obj)
-        msg = f"\n<<DelayedModel {self._delayed_model.__name__}:{self._delayed_pk}>>:\t{result}"
+        msg = f"\n<<DelayedModel {self._delayed_model.__name__}:{self._delayed_pk}>>"
         return msg
 
     def __hash__(self):
         return hash(self._instance())
 
 
 class AutoModel(ABC):
     attributes = {}
     _table_name = ""
     _table = None
     _orm = ORM
 
-    _save_memo = {}
-
     def __new__(cls, *args, **kwargs):
         """
         Create a new instance of the AutoModel.
 
         This method is responsible for creating a new instance of the AutoModel class.
         It sets default attributes, populates the object from the database if a primary key is provided,
         and handles additional keyword arguments.
@@ -103,170 +99,209 @@
             *args: Positional arguments.
             **kwargs: Keyword arguments, including 'pk' for primary key.
 
         Returns:
             obj: The created AutoModel instance.
         """
         obj = super().__new__(cls)
-        pk = kwargs.get("pk", args[0] if args else None)
+        pk = kwargs.pop("pk", None)
         # set default attributes
         # Get model data from database
         result = cls.table().get(pk) or {}
+
         # set object attributes
         for k, v in cls.attributes.items():
             if isinstance(v, AutoAttribute):
                 v = v.default
-            v = copy.deepcopy(v)
-            setattr(obj, k, result.get(k, v))
-
-        # update model with keyword arguments
+            setattr(obj, k, result.get(k, copy.deepcopy(v)))
+        obj.pk = pk
         obj.__dict__ |= kwargs
-
-        # log(obj, kwargs)
-        _automodel = obj.__dict__.pop("_automodel", None)
-        obj.__dict__ |= cls._deserialize(obj.__dict__)
-        obj.__dict__["_automodel"] = _automodel
-
+        # breakpoint()
+        obj.__dict__ = AutoDecoder.decode(obj.__dict__)
+        obj._automodel = obj.model_name(qualified=True)
         obj.last_updated = datetime.now()
 
         return obj
 
     def __getattribute__(self, name):
         obj = super().__getattribute__(name)
-        if isinstance(obj, DelayedModel):
-            return obj._instance()
+        if not name.startswith("__"):
+            if isinstance(obj, DelayedModel):
+                try:
+                    result = obj._instance()
+                except DanglingReferenceError as e:
+                    log(e)
+                    super().__setattr__(name, None)
+                    self.save()
+                    return None
+                else:
+                    super().__setattr__(name, result)
+
+            elif isinstance(obj, list):
+                for i, item in enumerate(obj):
+                    if isinstance(item, DelayedModel):
+                        try:
+                            result = item._instance()
+                        except DanglingReferenceError as e:
+                            log(e)
+                            obj[i] = None
+                            self.save()
+                        else:
+                            obj[i] = result
+
+            elif isinstance(obj, dict):
+                for key, item in obj.items():
+                    if isinstance(item, DelayedModel):
+                        try:
+                            result = item._instance()
+                        except DanglingReferenceError as e:
+                            log(e)
+                            obj[key] = None
+                            self.save()
+                        else:
+                            obj[key] = result
         return obj
 
+    def __str__(self) -> str:
+        return self.__repr__()
+
     def __repr__(self) -> str:
         """
         Return a string representation of the AutoModel instance.
 
         Returns:
             str: A string representation of the AutoModel instance.
         """
-        return f"{self.__dict__}"
+        return str(self.__dict__)
 
     def __eq__(self, other):
-        return self.pk == other.pk
+        return self.pk == other.pk if other else False
 
-    def get_save_key(self):
-        return f"{self.__class__.__name__}-{self.pk}"
+    @classmethod
+    def load_model(cls, model, module=None):
+        if not module:
+            module = f"models.{model.lower()}"
+        module = importlib.import_module(module)
+        return getattr(module, model)
 
     @classmethod
     def table(cls):
         # breakpoint()
         if not cls._table or cls._table.name != cls.__name__:
-            cls.attributes["pk"] = AutoAttribute("TAG", primary_key=True)
+            cls.attributes["pk"] = None
             cls.attributes["last_updated"] = datetime.now()
             cls.attributes["_automodel"] = AutoAttribute(
-                "TAG", default=cls.model_name()
+                "TEXT", default=cls.model_name(qualified=True)
             )
             cls._table = cls._orm(cls._table_name or cls.__name__, cls.attributes)
         return cls._table
 
     @classmethod
-    def model_name(cls):
+    def model_name(cls, qualified=False):
         """
         Get the fully qualified name of this model.
 
         Returns:
             str: The fully qualified name of this model.
         """
-        return f"{cls.__module__}.{cls.__name__}"
+        return f"{cls.__module__}.{cls.__name__}" if qualified else cls.__name__
+
+    @property
+    def _id(self):
+        """
+        Get the primary key of this model.
 
-    ## TODO: Save all sub objects
-    ## FIXME: This is causing issues
-    # def _subobj_save(self, obj, key):
-    #     if isinstance(obj, list):
-    #         for v in obj:
-    #             if self._subobj_save(v, key) is None:
-    #                 obj.remove(v)
-    #     elif isinstance(obj, dict):
-    #         for k, v in obj.items():
-    #             if self._subobj_save(v, key) is None:
-    #                 obj[k] = None
-    #     elif issubclass(obj.__class__, (AutoModel, DelayedModel)):
-    #         if not obj.pk:
-    #             obj.pk = str(uuid.uuid4())
-    #         if obj.pk not in self._save_memo[key]:
-    #             obj._save(key)
+        Returns:
+            int: The primary key of this model.
+        """
+        return self.pk
 
-    def _save(self, key):
+    @_id.setter
+    def _id(self, _id):
         """
-        Save this model to the database.
+        Get the primary key of this model.
 
         Returns:
-            int: The primary key (pk) of the saved model.
+            int: The primary key of this model.
+        """
+        self.pk = str(_id)
+
+    def validate(self):
+        """
+        Validate this model.
+        """
+        for key, vattr in self.attributes.items():
+            if isinstance(vattr, AutoAttribute):
+                val = getattr(self, key)
+                if vattr.type == "TEXT":
+                    if not isinstance(val, str):
+                        raise TypeError(f"Value must be a string, not {type(val)}")
+                elif vattr.type == "NUMERIC":
+                    if not isinstance(val, (int, float)):
+                        raise TypeError(f"Value must be a number, not {type(val)}")
+                elif vattr.type == "MODEL":
+                    # log(isinstance(val, (AutoModel, DelayedModel)), type(val))
+                    if val is not None and not isinstance(
+                        val, (AutoModel, DelayedModel)
+                    ):
+                        raise TypeError(
+                            f"Value must be an AutoModel or None, not {type(val)}"
+                        )
+                else:
+                    raise ValueError(f"Invalid type {self.type}")
 
-        ALGO:
-        - add self.pk to save_memo is self.pk
-        - save object not in save memo or without pk into database
-        """
-
-        assert self.pk  # sanity check
-        assert key and key in AutoModel._save_memo  # sanity check
-
-        local_key = self.get_save_key()
-
-        # if key == local_key:
-        #     log(f"Saving root object {key}")
-        # else:
-        #     log(f"Saving child object {local_key} for root {key}")
-
-        if local_key not in AutoModel._save_memo[key]:
-            AutoModel._save_memo[key].append(local_key)
-            self.pk = self.table().save(self.serialize())
-        # FIXME: STILL NOT WORKING
-        # for attr in self.attributes:
-        #     self._subobj_save(getattr(self, attr), key)
-        return self.pk
+                if vattr.required and val is None:
+                    raise ValueError(f"{key} is required")
+                if vattr.unique and len(self.search(**{key: val})) > 1:
+                    raise ValueError(f"{key} must be unique")
+                if vattr.primary_key:
+                    self.pk = val
 
     def save(self):
         """
         Save this model to the database.
 
         Returns:
             int: The primary key (pk) of the saved model.
         """
-        if not self.pk:
-            self.pk = str(uuid.uuid4())
-        key = self.get_save_key()
-        AutoModel._save_memo[key] = []
-        result = self._save(key)
-        assert result == self.pk
-        AutoModel._save_memo.pop(key)
-        return result
+        self.validate()
+        serialized_obj = self.serialize()
+        serialized_obj["pk"] = self.pk
+        self.pk = self.table().save(serialized_obj)
+
+        return self.pk
 
     @classmethod
     def get(cls, pk):
         """
         Get a model by primary key.
 
         Args:
             pk (int): The primary key of the model to retrieve.
 
         Returns:
             AutoModel or None: The retrieved AutoModel instance, or None if not found.
         """
-        # breakpoint()
-        result = cls.table().get(pk)
+        table = cls.table()
+        result = table.get(pk)
         return cls(**result) if result else None
 
     @classmethod
     def random(cls):
         """
         Get a model by primary key.
 
         Args:
             pk (int): The primary key of the model to retrieve.
 
         Returns:
             AutoModel or None: The retrieved AutoModel instance, or None if not found.
         """
         result = cls.table().random()
+        # breakpoint()
         return cls(**result) if result else None
 
     @classmethod
     def all(cls):
         """
         Get all models of this type.
 
@@ -282,14 +317,16 @@
 
         Args:
             **kwargs: Keyword arguments to search for (dict).
 
         Returns:
             list: A list of AutoModel instances that match the search criteria.
         """
+        for k, v in kwargs.items():
+            kwargs[k] = AutoEncoder.encode(v)
         return [cls(**attribs) for attribs in cls.table().search(**kwargs)]
 
     @classmethod
     def find(cls, **kwargs):
         """
         Find the first model containing the keyword values and return it.
 
@@ -298,107 +335,23 @@
 
         Returns:
             AutoModel or None: The first matching AutoModel instance, or None if not found.
         """
         attribs = cls.table().find(**kwargs)
         return cls(**attribs) if attribs else None
 
-    def _subobj_delete(self, obj):
-        if isinstance(obj, list):
-            for v in obj:
-                self._subobj_delete(v)
-        elif isinstance(obj, dict):
-            for v in obj.values():
-                self._subobj_delete(v)
-        elif issubclass(obj.__class__, (AutoModel, DelayedModel)):
-            obj.delete()
-
-    def delete(self, sub_objects=False):
+    def delete(self):
         """
         Delete this model from the database.
         """
-        if sub_objects:
-            for k in self.attributes:
-                if attr := getattr(self, k):
-                    self._subobj_delete(attr)
-        return self.table().delete(pk=self.pk)
-
-    serialized_tracker = []
-
-    @classmethod
-    def _serialize(cls, val):
-        if isinstance(val, list):
-            new_list = []
-            for v in val:
-                obj = cls._serialize(v)
-                new_list.append(obj)
-            val = new_list
-        elif isinstance(val, dict):
-            new_dict = {}
-            for k, v in val.items():
-                new_dict[k] = cls._serialize(v)
-            val = new_dict
-        elif isinstance(val, datetime):
-            val = {"_datetime": val.isoformat()}
-        elif issubclass(val.__class__, (AutoModel, DelayedModel)):
-            if val.pk:
-                val = {
-                    "pk": val.pk,
-                    "_automodel": val.model_name(),
-                }
-            else:
-                log(
-                    val.__class__.__name__,
-                    "The above object was not been saved. You must save subobjects if you want them to persist.",
-                )
-                val = None
-
-        return val
+        return self.table().delete(self.pk)
 
     def serialize(self):
         """
         Serialize this model to a dictionary.
 
         Returns:
             dict: A dictionary representation of the serialized model.
         """
-        record = {k: v for k, v in self.__dict__.items() if k in self.attributes}
-        result = self._serialize(record)
-        return result | {
-            "_automodel": self.model_name(),
-        }
-
-    @classmethod
-    def _deserialize(cls, val):
-        if isinstance(val, dict):
-            if val.get("_automodel"):
-                if val.get("pk"):
-                    # log(val.get('pk'))
-                    assert len(val.get("pk"))
-                    val = DelayedModel(val["_automodel"], val["pk"])
-                else:
-                    val = None
-            elif "_datetime" in val:
-                val = datetime.fromisoformat(val["_datetime"])
-            else:
-                for k, v in val.items():
-                    val[k] = cls._deserialize(v)
-        elif isinstance(val, list):
-            for i, v in enumerate(val):
-                val[i] = cls._deserialize(v)
-        return val
-
-    @classmethod
-    def deserialize(cls, vars):
-        """
-        Deserialize a dictionary to a model.
-
-        Args:
-            vars (dict): The dictionary to deserialize.
-
-        Returns:
-            AutoModel: A deserialized AutoModel instance.
-        """
-        if "_automodel" not in vars:
-            raise ValueError("Cannot only deserialize automodel objects")
-
-        return cls(**vars)
+        vars = {k: v for k, v in self.__dict__.items() if k in self.attributes}
+        json_vars = AutoEncoder.encode(vars)
+        return json_vars
```

### Comparing `autonomous-app-0.1.99/src/autonomous/storage/imagestorage.py` & `autonomous_app-0.2.0/src/autonomous/storage/imagestorage.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,71 +11,105 @@
 class ImageStorage:
     _sizes = {"thumbnail": 100, "small": 300, "medium": 600, "large": 1000}
 
     def __init__(self, path="static/images"):
         self.base_path = path
 
     @classmethod
-    def _create_key(cls, folder="", image_type="webp"):
-        if folder:
-            return f"{folder.replace('/', '.')}.{uuid.uuid4()}.{image_type}"
-        else:
-            return f"{uuid.uuid4()}.{image_type}"
-
-    def _resize_image(self, asset_id, max_size):
-        img_type = self.get_img_type(asset_id)
-        file_path = f"{self.get_path(asset_id)}/orig.{img_type}"
+    def _get_key(cls, folder="", pkey=None):
+        if folder and not folder.endswith("/"):
+            folder = f"{folder}/"
+        folder = f"{folder.replace('/', '.')}{pkey or uuid.uuid4()}"
+        return f"{folder}"
+
+    def _resize_image(self, asset_id, max_size=1024):
+        # log("Resizing image", asset_id, max_size)
+        file_path = f"{self.get_path(asset_id)}/orig.webp"
         with Image.open(file_path) as img:
-            max_size = self._sizes.get(max_size) or int(max_size)
             resized_img = img.copy()
+            max_size = self._sizes.get(max_size) or int(max_size)
             resized_img.thumbnail((max_size, max_size))
             img_byte_arr = io.BytesIO()
             resized_img.save(img_byte_arr, format="WEBP")
             return img_byte_arr.getvalue()
 
-    def save(self, file, image_type="webp", folder=""):
-        asset_id = self._create_key(folder, image_type)
+    def _convert_image(self, raw, crop=False):
+        with Image.open(io.BytesIO(raw)) as img:
+            width, height = img.size
+            if crop and width != height:
+                max_size = min(width, height)
+                img.crop(
+                    (
+                        (width - max_size) / 2,
+                        (height - max_size) / 2,
+                        (width + max_size) / 2,
+                        (height + max_size) / 2,
+                    )
+                )
+            img = img.copy()
+            img_byte_arr = io.BytesIO()
+            img.save(img_byte_arr, format="WEBP")
+            return img_byte_arr.getvalue()
+
+    def save(self, file, folder="", crop=False):
+        asset_id = self._get_key(folder)
         os.makedirs(self.get_path(asset_id), exist_ok=True)
-        file_path = f"{self.get_path(asset_id)}/orig.{image_type}"
+        file_path = f"{self.get_path(asset_id)}/orig.webp"
         with open(file_path, "wb") as asset:
+            file = self._convert_image(file, crop=crop)
             asset.write(file)
         return asset_id
 
     def get_url(self, asset_id, size="orig", full_url=False):
-        original_path = f"{self.get_path(asset_id)}/orig.{self.get_img_type(asset_id)}"
+        # log(f"Getting image: {asset_id}.{size}")
+        if not asset_id:
+            return ""
+        original_path = f"{self.get_path(asset_id)}"
+        # log(f"Getting image: {asset_id}.{size}", original_path)
         if not os.path.exists(original_path):
-            log(f"Original image not found: {original_path}")
+            # log(f"Original image not found: {original_path}")
             return ""
-
-        file_path = f"{self.get_path(asset_id)}/{size}.{self.get_img_type(asset_id)}"
-        if not os.path.exists(file_path):
+        file_path = f"{original_path}/{size}.webp"
+        # log(file_path)
+        if (
+            size != "orig"
+            and os.path.exists(original_path)
+            and not os.path.exists(file_path)
+        ):
             # If the file doesn't exist, create it
             result = self._resize_image(asset_id, size)
             with open(file_path, "wb") as asset:
                 asset.write(result)
-
-        return (
+        result_url = (
             f"/{file_path}"
             if not full_url
             else f"{os.environ.get('APP_BASE_URL', '')}/{file_path}"
         )
+        # log(f"Returning image url: {result_url}")
+        return result_url
 
     def get_path(self, asset_id):
-        img_path, _ = asset_id.rsplit(".", maxsplit=1)
-        asset_path = img_path.replace(".", "/")
-        return os.path.join(self.base_path, asset_path)
-
-    def get_img_type(self, asset_id):
-        return asset_id.rsplit(".", maxsplit=1)[-1]
+        if asset_id:
+            asset_path = asset_id.replace(".", "/")
+            if asset_path.endswith("/"):
+                asset_path = asset_path[:-1]
+            return os.path.join(self.base_path, f"{asset_path}")
+        else:
+            return self.base_path
 
-    def search(self, folder=None, **kwargs):
+    def search(self, folder="", **kwargs):
         imgs = []
-        if folder:
-            for f in os.listdir(f"{self.base_path}/{folder}"):
-                imgs.append(self._create_key(f"{folder}/{f}"))
+        for f in os.listdir(f"{self.base_path}/{folder}"):
+            log(f"{self.base_path}/{folder}", f)
+            img_key = self._get_key(
+                f"{folder}",
+                pkey=f,
+            )
+            log(img_key)
+            imgs.append(img_key)
         return imgs
 
     def remove(self, asset_id):
         file_path = self.get_path(asset_id)
         if os.path.isdir(file_path):
             shutil.rmtree(file_path)
             return True
```

### Comparing `autonomous-app-0.1.99/src/autonomous/storage/localstorage.py` & `autonomous_app-0.2.0/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.99/src/autonomous/tasks/autotask.py` & `autonomous_app-0.2.0/src/autonomous/tasks/autotask.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import importlib
 import os
 import subprocess
+import time
 
 from redis import Redis
 from rq import Queue, Worker
 from rq.job import Job
 
 from autonomous import log
 
+# class AutoJob(Job):
+#     def perform(self):
+#         start = time.time()
+#         result = super().perform()
+#         end = time.time()
+#         log.info(
+#             "Job Finished",
+#             key=self.key,
+#             seconds=(end - start),
+#             method=self.func_name,
+#             data_size=len(self._data),
+#             queue=self.origin,
+#             enqueued_at=self.enqueued_at.timestamp() if self.enqueued_at else None,
+#             started_at=self.started_at.timestamp() if self.started_at else None,
+#         )
+#         return result
+
 
 class AutoTask:
     def __init__(self, job):
         self.job = job
 
     @property
     def id(self):
@@ -26,21 +44,19 @@
 
     @property
     def running(self):
         return self.status == "running"
 
     @property
     def finished(self):
-        result = self.status == "finished"
-        return result
+        return self.status == "finished"
 
     @property
     def failed(self):
-        result = self.status == "failed"
-        return result
+        return self.status == "failed"
 
     @property
     def result(self):
         result = self.job.latest_result()
         result_dict = {
             "id": self.id,
             "return_value": result.return_value if result else None,
@@ -59,16 +75,16 @@
 
 class AutoTasks:
     _connection = None
     queue = None
     workers = []
     all_tasks = []
     config = {
-        "host": os.environ.get("REDIS_HOST", ""),
-        "port": os.environ.get("REDIS_PORT", ""),
+        "host": os.environ.get("REDIS_HOST"),
+        "port": os.environ.get("REDIS_PORT"),
         "password": os.environ.get("REDIS_PASSWORD"),
         "username": os.environ.get("REDIS_USERNAME"),
         "db": os.environ.get("REDIS_DB", 0),
     }
 
     def __init__(self, queue="default", num_workers=3):
         if not AutoTasks._connection:
@@ -93,14 +109,15 @@
         :param job: job function
         :param args: job function args
         :param kwargs: job function kwargs
         args and kwargs: use these to explicitly pass arguments and keyword to the underlying job function.
         _task_<option>:pass options to the task object
         :return: job
         """
+
         job = AutoTasks.queue.enqueue(
             func,
             job_timeout=kwargs.get("_task_job_timeout", 3600),
             args=args,
             kwargs=kwargs,
         )
         self.create_worker(func)
```

### Comparing `autonomous-app-0.1.99/src/autonomous_app.egg-info/PKG-INFO` & `autonomous_app-0.2.0/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.99
+Version: 0.2.0
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,95 +21,91 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: homepage, https://github.com/Sallenmoore/autonomous
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 Requires-Dist: icecream
 Requires-Dist: setuptools
 Requires-Dist: python-dotenv
 Requires-Dist: PyGithub
 Requires-Dist: pygit2
 Requires-Dist: cloudinary
 Requires-Dist: pillow
-Requires-Dist: redis
+Requires-Dist: pymongo
 Requires-Dist: jsmin
 Requires-Dist: requests
 Requires-Dist: gunicorn
 Requires-Dist: Authlib
-Requires-Dist: rq
-Requires-Dist: rq-dashboard
-Requires-Dist: pyautogen
-Requires-Dist: openai
+Requires-Dist: openai>=1.21.1
 Requires-Dist: validators
 Requires-Dist: dateparser
 Requires-Dist: python-slugify
 
 # Autonomous
 
 :warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask.
-The goal is to make it easy to create self-contained Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
+A self-contained containerized Python applications with minimal dependencies using built in libraries for many different kinds of tasks.
 
 - **[pypi](https://test.pypi.org/project/autonomous)**
 - **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
-- Built-in Local NoSQL database and Model API
-- Cloud file storage with Cloudinary or S3
-- Auto-Generated Documentation Pages (Coming Soon!!!)
+- Container based MongoDB database
+- Model ORM API
+- File storage locally or with services such as Cloudinary or S3 
+- Separate service for long running tasks
+- Built-in Authentication with Google or Github
+- Auto-Generated Documentation Pages
 
 ## Dependencies
 
 - **Languages**
-  - [Python 3.10](/Dev/language/python)
+  - [Python 3.11](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
   - [Docker](https://docs.docker.com/)
   - [Docker Compose](https://github.com/compose-spec/compose-spec/blob/master/spec.md)
 - **Server**
   - [nginx](https://docs.nginx.com/nginx/)
   - [gunicorn](https://docs.gunicorn.org/en/stable/configure.html)
 - **Networking and Serialization**
   - [requests](https://requests.readthedocs.io/en/latest/)
 - **Database**
-  - [Local](https://tinydb.readthedocs.io/en/latest/)
+  - [pymongo](https://pymongo.readthedocs.io/en/stable/api/pymongo/index.html)
 - **Testing**
   - [pytest](/Dev/tools/pytest)
   - [coverage](https://coverage.readthedocs.io/en/6.4.1/cmd.html)
 - **Documentation** - Coming Soon
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
-  - [highlight.js](https://highlightjs.org/)
-
 ---
 
 ## Developer Notes
 
 ### TODO
 
-- Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
-- Add more database options
 - 100% testing coverage
 
 ### Issue Tracking
 
 - None
 
 ## Processes
```

