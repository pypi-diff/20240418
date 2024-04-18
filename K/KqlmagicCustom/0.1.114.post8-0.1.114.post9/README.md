# Comparing `tmp/KqlmagicCustom-0.1.114.post8.tar.gz` & `tmp/KqlmagicCustom-0.1.114.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KqlmagicCustom-0.1.114.post8.tar", last modified: Sun Jan  9 02:44:40 2022, max compression
+gzip compressed data, was "KqlmagicCustom-0.1.114.post9.tar", last modified: Mon Jan 31 21:26:13 2022, max compression
```

## Comparing `KqlmagicCustom-0.1.114.post8.tar` & `KqlmagicCustom-0.1.114.post9.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxrwx   0        0        0        0 2022-01-09 02:44:40.092881 KqlmagicCustom-0.1.114.post8/
--rw-rw-rw-   0        0        0     7943 2019-08-27 16:01:02.000000 KqlmagicCustom-0.1.114.post8/HISTORY.rst
--rw-rw-rw-   0        0        0     1129 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post8/LICENSE.TXT
--rw-rw-rw-   0        0        0       60 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post8/MANIFEST.in
--rw-rw-rw-   0        0        0        0 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post8/NEWS.txt
--rw-rw-rw-   0        0        0      156 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post8/NOTICE.TXT
--rw-rw-rw-   0        0        0     6010 2022-01-09 02:44:40.093747 KqlmagicCustom-0.1.114.post8/PKG-INFO
--rw-rw-rw-   0        0        0     3255 2021-04-14 13:37:56.000000 KqlmagicCustom-0.1.114.post8/README.rst
--rw-rw-rw-   0        0        0      990 2019-07-21 15:56:58.000000 KqlmagicCustom-0.1.114.post8/TODO.txt
-drwxrwxrwx   0        0        0        0 2022-01-09 02:44:39.910021 KqlmagicCustom-0.1.114.post8/azure/
-drwxrwxrwx   0        0        0        0 2022-01-09 02:44:40.061204 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/
--rw-rw-rw-   0        0        0      881 2022-01-08 01:24:58.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/__init__.py
--rw-rw-rw-   0        0        0      980 2021-01-30 00:34:21.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_debug_utils.py
--rw-rw-rw-   0        0        0     2494 2022-01-08 17:47:05.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_meta.py
--rw-rw-rw-   0        0        0     7431 2021-04-17 12:40:06.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_require.py
--rw-rw-rw-   0        0        0     1607 2021-01-05 16:27:01.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_test.py
--rw-rw-rw-   0        0        0     1661 2022-01-09 02:43:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_version.py
--rw-rw-rw-   0        0        0      787 2021-01-16 19:57:34.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aad_helper.py
--rw-rw-rw-   0        0        0    11140 2021-12-09 23:42:37.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/activate_kernel_command.py
--rw-rw-rw-   0        0        0     6652 2020-12-14 21:59:22.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/adal_token_cache.py
--rw-rw-rw-   0        0        0     4055 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/ai_engine.py
--rw-rw-rw-   0        0        0     1235 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aimon_engine.py
--rw-rw-rw-   0        0        0     3721 2021-05-16 00:25:32.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/allow_py_comments_before_cell.py
--rw-rw-rw-   0        0        0     3349 2022-01-08 01:09:59.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/allow_single_line_cell.py
--rw-rw-rw-   0        0        0     3383 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aria_engine.py
--rw-rw-rw-   0        0        0     3413 2020-12-28 17:09:46.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/bug_report.py
--rw-rw-rw-   0        0        0     8654 2021-01-16 19:43:40.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/cache_client.py
--rw-rw-rw-   0        0        0     6003 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/cache_engine.py
--rw-rw-rw-   0        0        0    11142 2020-12-14 21:52:04.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/column_guesser.py
--rw-rw-rw-   0        0        0     9103 2020-12-14 21:21:59.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/connection.py
--rw-rw-rw-   0        0        0    17167 2021-05-16 00:25:12.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/constants.py
--rw-rw-rw-   0        0        0    10754 2021-01-29 23:49:58.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/database_html.py
--rw-rw-rw-   0        0        0    17673 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dependencies.py
--rw-rw-rw-   0        0        0     5252 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dict_db_storage.py
--rw-rw-rw-   0        0        0    40211 2021-12-09 23:42:37.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/display.py
--rw-rw-rw-   0        0        0     3558 2020-12-13 16:12:43.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dpapi_crypto.py
--rw-rw-rw-   0        0        0     2080 2020-12-13 16:12:43.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dpapi_crypto_msal.py
--rw-rw-rw-   0        0        0    12384 2020-12-28 17:09:46.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/draft_client.py
--rw-rw-rw-   0        0        0     2677 2020-12-14 21:27:53.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/email_notification.py
--rw-rw-rw-   0        0        0     4581 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/engine.py
--rw-rw-rw-   0        0        0      393 2020-12-14 22:03:01.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/exceptions.py
--rw-rw-rw-   0        0        0     6744 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/fernet_crypto.py
--rw-rw-rw-   0        0        0    46668 2021-06-09 00:55:59.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/help.py
--rw-rw-rw-   0        0        0     3662 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/help_html.py
--rw-rw-rw-   0        0        0    10090 2021-05-16 00:25:12.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/ipython_api.py
--rw-rw-rw-   0        0        0      943 2020-11-11 17:54:29.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_client.py
--rw-rw-rw-   0        0        0    23464 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_engine.py
--rw-rw-rw-   0        0        0    35606 2021-07-21 13:40:55.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_magic.py
--rw-rw-rw-   0        0        0   107020 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_magic_core.py
--rw-rw-rw-   0        0        0     9498 2022-01-08 17:39:28.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_proxy.py
--rw-rw-rw-   0        0        0    16435 2022-01-09 02:43:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_response.py
--rw-rw-rw-   0        0        0    14278 2020-12-29 15:45:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kusto_client.py
--rw-rw-rw-   0        0        0     7879 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kusto_engine.py
--rw-rw-rw-   0        0        0     3942 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/la_engine.py
--rw-rw-rw-   0        0        0     7419 2021-07-21 14:43:15.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/log.py
--rw-rw-rw-   0        0        0     2575 2021-01-16 20:34:59.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/magic_extension.py
--rw-rw-rw-   0        0        0     4468 2020-12-27 12:51:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/msal_token_cache.py
--rw-rw-rw-   0        0        0    47280 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_aad_helper.py
--rw-rw-rw-   0        0        0    65747 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_aad_helper_msal.py
--rw-rw-rw-   0        0        0    23093 2021-11-02 20:56:13.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_files_server.py
--rw-rw-rw-   0        0        0     9179 2021-12-09 23:42:36.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_files_server_management.py
--rw-rw-rw-   0        0        0    11472 2021-06-09 00:26:50.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_utils.py
--rw-rw-rw-   0        0        0    19088 2021-01-16 20:49:36.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/palette.py
--rw-rw-rw-   0        0        0    14110 2021-01-16 16:41:24.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/parameterizer.py
--rw-rw-rw-   0        0        0    74745 2021-07-21 13:57:01.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/parser.py
--rw-rw-rw-   0        0        0     2149 2021-05-16 00:25:12.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/python_command.py
--rw-rw-rw-   0        0        0    86223 2021-12-10 00:03:24.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/results.py
--rw-rw-rw-   0        0        0    12045 2020-12-22 18:15:35.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/sso_storage.py
--rw-rw-rw-   0        0        0    16719 2021-01-16 19:43:40.000000 KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/version.py
-drwxrwxrwx   0        0        0        0 2022-01-09 02:44:40.090562 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/
--rw-rw-rw-   0        0        0     6010 2022-01-09 02:44:39.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2180 2022-01-09 02:44:39.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-09 02:44:39.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-01-17 00:00:43.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4676 2022-01-09 02:44:39.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-01-09 02:44:39.000000 KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2274 2020-09-14 22:22:20.000000 KqlmagicCustom-0.1.114.post8/azure_bdist_wheel.py
--rw-rw-rw-   0        0        0      105 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post8/dev_requirements.txt
--rw-rw-rw-   0        0        0      152 2022-01-09 02:44:40.096140 KqlmagicCustom-0.1.114.post8/setup.cfg
--rw-rw-rw-   0        0        0     8260 2022-01-09 02:44:38.000000 KqlmagicCustom-0.1.114.post8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-31 21:26:13.922107 KqlmagicCustom-0.1.114.post9/
+-rw-rw-rw-   0        0        0     7943 2019-08-27 16:01:02.000000 KqlmagicCustom-0.1.114.post9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1129 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post9/LICENSE.TXT
+-rw-rw-rw-   0        0        0       60 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post9/MANIFEST.in
+-rw-rw-rw-   0        0        0        0 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post9/NEWS.txt
+-rw-rw-rw-   0        0        0      156 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post9/NOTICE.TXT
+-rw-rw-rw-   0        0        0     6031 2022-01-31 21:26:13.922107 KqlmagicCustom-0.1.114.post9/PKG-INFO
+-rw-rw-rw-   0        0        0     3255 2021-04-14 13:37:56.000000 KqlmagicCustom-0.1.114.post9/README.rst
+-rw-rw-rw-   0        0        0      990 2019-07-21 15:56:58.000000 KqlmagicCustom-0.1.114.post9/TODO.txt
+drwxrwxrwx   0        0        0        0 2022-01-31 21:26:13.727802 KqlmagicCustom-0.1.114.post9/azure/
+drwxrwxrwx   0        0        0        0 2022-01-31 21:26:13.870818 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/
+-rw-rw-rw-   0        0        0      881 2022-01-08 01:24:58.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/__init__.py
+-rw-rw-rw-   0        0        0      980 2021-01-30 00:34:21.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_debug_utils.py
+-rw-rw-rw-   0        0        0     2494 2022-01-08 17:47:05.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_meta.py
+-rw-rw-rw-   0        0        0     7616 2022-01-31 20:22:58.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_require.py
+-rw-rw-rw-   0        0        0     1607 2021-01-05 16:27:01.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_test.py
+-rw-rw-rw-   0        0        0     1661 2022-01-27 15:28:47.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_version.py
+-rw-rw-rw-   0        0        0      787 2021-01-16 19:57:34.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aad_helper.py
+-rw-rw-rw-   0        0        0    11140 2021-12-09 23:42:37.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/activate_kernel_command.py
+-rw-rw-rw-   0        0        0     6652 2020-12-14 21:59:22.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/adal_token_cache.py
+-rw-rw-rw-   0        0        0     4055 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/ai_engine.py
+-rw-rw-rw-   0        0        0     1235 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aimon_engine.py
+-rw-rw-rw-   0        0        0     3721 2021-05-16 00:25:32.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/allow_py_comments_before_cell.py
+-rw-rw-rw-   0        0        0     3349 2022-01-08 01:09:59.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/allow_single_line_cell.py
+-rw-rw-rw-   0        0        0     3383 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aria_engine.py
+-rw-rw-rw-   0        0        0     3589 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/bug_report.py
+-rw-rw-rw-   0        0        0     8654 2021-01-16 19:43:40.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/cache_client.py
+-rw-rw-rw-   0        0        0     6003 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/cache_engine.py
+-rw-rw-rw-   0        0        0    11142 2020-12-14 21:52:04.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/column_guesser.py
+-rw-rw-rw-   0        0        0     9103 2020-12-14 21:21:59.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/connection.py
+-rw-rw-rw-   0        0        0    17570 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/constants.py
+-rw-rw-rw-   0        0        0    10754 2021-01-29 23:49:58.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/database_html.py
+-rw-rw-rw-   0        0        0    17682 2022-01-31 21:08:08.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dependencies.py
+-rw-rw-rw-   0        0        0     5252 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dict_db_storage.py
+-rw-rw-rw-   0        0        0    40255 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/display.py
+-rw-rw-rw-   0        0        0     3558 2020-12-13 16:12:43.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dpapi_crypto.py
+-rw-rw-rw-   0        0        0     2080 2020-12-13 16:12:43.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dpapi_crypto_msal.py
+-rw-rw-rw-   0        0        0    12323 2022-01-30 22:03:29.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/draft_client.py
+-rw-rw-rw-   0        0        0     2677 2020-12-14 21:27:53.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/email_notification.py
+-rw-rw-rw-   0        0        0     4581 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/engine.py
+-rw-rw-rw-   0        0        0      393 2020-12-14 22:03:01.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/exceptions.py
+-rw-rw-rw-   0        0        0     6744 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/fernet_crypto.py
+-rw-rw-rw-   0        0        0    46690 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/help.py
+-rw-rw-rw-   0        0        0     3662 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/help_html.py
+-rw-rw-rw-   0        0        0    12491 2022-01-31 21:13:19.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/http_client.py
+-rw-rw-rw-   0        0        0    10112 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/ipython_api.py
+-rw-rw-rw-   0        0        0     1051 2022-01-30 22:03:29.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_client.py
+-rw-rw-rw-   0        0        0    23464 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_engine.py
+-rw-rw-rw-   0        0        0    35650 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_magic.py
+-rw-rw-rw-   0        0        0   107906 2022-01-31 19:39:32.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_magic_core.py
+-rw-rw-rw-   0        0        0     9498 2022-01-08 17:39:28.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_proxy.py
+-rw-rw-rw-   0        0        0    16435 2022-01-09 02:43:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_response.py
+-rw-rw-rw-   0        0        0    14153 2022-01-30 22:03:29.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kusto_client.py
+-rw-rw-rw-   0        0        0     7879 2021-12-09 23:57:20.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kusto_engine.py
+-rw-rw-rw-   0        0        0     3942 2020-12-30 17:28:00.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/la_engine.py
+-rw-rw-rw-   0        0        0     7419 2021-07-21 14:43:15.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/log.py
+-rw-rw-rw-   0        0        0     2575 2021-01-16 20:34:59.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/magic_extension.py
+-rw-rw-rw-   0        0        0     4468 2020-12-27 12:51:20.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/msal_token_cache.py
+-rw-rw-rw-   0        0        0    47445 2022-01-31 21:08:08.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_aad_helper.py
+-rw-rw-rw-   0        0        0    66064 2022-01-31 21:08:08.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_aad_helper_msal.py
+-rw-rw-rw-   0        0        0    23093 2021-11-02 20:56:13.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_files_server.py
+-rw-rw-rw-   0        0        0     9179 2021-12-09 23:42:36.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_files_server_management.py
+-rw-rw-rw-   0        0        0    11472 2021-06-09 00:26:50.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_utils.py
+-rw-rw-rw-   0        0        0    19088 2021-01-16 20:49:36.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/palette.py
+-rw-rw-rw-   0        0        0    14110 2021-01-16 16:41:24.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/parameterizer.py
+-rw-rw-rw-   0        0        0    74745 2021-07-21 13:57:01.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/parser.py
+-rw-rw-rw-   0        0        0     2149 2021-05-16 00:25:12.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/python_command.py
+-rw-rw-rw-   0        0        0    86611 2022-01-31 19:17:41.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/results.py
+-rw-rw-rw-   0        0        0    12045 2020-12-22 18:15:35.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/sso_storage.py
+-rw-rw-rw-   0        0        0    16770 2022-01-30 22:03:29.000000 KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/version.py
+drwxrwxrwx   0        0        0        0 2022-01-31 21:26:13.921224 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/
+-rw-rw-rw-   0        0        0     6031 2022-01-31 21:26:13.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2210 2022-01-31 21:26:13.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-31 21:26:13.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-01-17 00:00:43.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4770 2022-01-31 21:26:13.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-01-31 21:26:13.000000 KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2274 2020-09-14 22:22:20.000000 KqlmagicCustom-0.1.114.post9/azure_bdist_wheel.py
+-rw-rw-rw-   0        0        0      105 2018-12-20 19:59:08.000000 KqlmagicCustom-0.1.114.post9/dev_requirements.txt
+-rw-rw-rw-   0        0        0      152 2022-01-31 21:26:13.924259 KqlmagicCustom-0.1.114.post9/setup.cfg
+-rw-rw-rw-   0        0        0     8260 2022-01-31 21:26:12.000000 KqlmagicCustom-0.1.114.post9/setup.py
```

### Comparing `KqlmagicCustom-0.1.114.post8/HISTORY.rst` & `KqlmagicCustom-0.1.114.post9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/LICENSE.TXT` & `KqlmagicCustom-0.1.114.post9/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/PKG-INFO` & `KqlmagicCustom-0.1.114.post9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KqlmagicCustom
-Version: 0.1.114.post8
+Version: 0.1.114.post9
 Summary: Kqlmagic: Microsoft Azure Monitor magic extension to Jupyter notebook (Custom Dependencies)
 Home-page: https://github.com/Microsoft/jupyter-Kqlmagic
 Author: Michael Binshtock
 Author-email: michabin@microsoft.com
 Maintainer: Michael Binshtock
 Maintainer-email: michabin@microsoft.com
 License: MIT License
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: default
 Provides-Extra: naked
+Provides-Extra: saw
 Provides-Extra: jupyter-basic
 Provides-Extra: ipython-basic
 Provides-Extra: python-basic
 Provides-Extra: basic
 Provides-Extra: jupyter-extended
 Provides-Extra: ipython-extended
 Provides-Extra: python-extended
```

### Comparing `KqlmagicCustom-0.1.114.post8/README.rst` & `KqlmagicCustom-0.1.114.post9/README.rst`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/TODO.txt` & `KqlmagicCustom-0.1.114.post9/TODO.txt`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/__init__.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_debug_utils.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_debug_utils.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_meta.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_meta.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_require.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_require.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,16 @@
 
 _SSO_REQUIRES = list_union(_KQLMAGIC_SSO_REQUIRES, _AZCLI_SSO_REQUIRES, _VSCODE_SSO_REQUIRES, _MSAL_SSO_REQUIRES,
                           _MSI_SSO_REQUIRES)
 
 _EXTRA_REQUIRES = list_union(_PLOT_REQUIRES, _DATAFRAME_REQUIRES, _SSO_REQUIRES, _IPYWIDGETS_REQUIRES)
 # ---------------------------------------------------
 
+_SAW_REQUIRES = list_union(_AUTH_REQUIRES, _JUPYTER_REQUIRES, _IPYTHON_REQUIRES, _IPYWIDGETS_REQUIRES, _DATAFRAME_PANDAS_REQUIRES, _JSON_COLOR_REQUIRES)
+
 
 # the most slim configuration
 _NAKED_REQUIRES = []
 
 # includes all configuration
 
 _PYTHON_BASIC_REQUIRES  = list_union(_BASIC_REQUIRES)
@@ -169,14 +171,16 @@
 ]
 
 EXTRAS_REQUIRE      = {
     'default': _DEFAULT_REQUIRES,
 
     'naked': _NAKED_REQUIRES,
 
+    'saw': _SAW_REQUIRES,
+
     'jupyter-basic': _JUPYTER_BASIC_REQUIRES,
     'ipython-basic': _IPYTHON_BASIC_REQUIRES,
     'python-basic': _PYTHON_BASIC_REQUIRES,
     'basic': _BASIC_REQUIRES,
 
     'jupyter-extended': _JUPYTER_EXTENDED_REQUIRES,
     'ipython-extended': _IPYTHON_EXTENDED_REQUIRES,
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_test.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_test.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/_version.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # (1, 2, 0, 'dev', 21) => "1.2.dev21"
 # (1, 2, 0, 'alpha', 7) => "1.2a7"
 # (1, 2, 0, 'beta', 2) => "1.2b2"
 # (1, 2, 0, 'rc', 4) => "1.2rc4"
 # (1, 2, 0, 'final', 0) => "1.2"
 
 
-__version_info__ = (0, 1, 114, "post", 8)
+__version_info__ = (0, 1, 114, "post", 9)
 
 assert len(__version_info__) == 5
 assert __version_info__[3] in ('dev', 'alpha', 'beta', 'rc', 'final', 'post')
 
 __version__ = '.'.join(map(str, __version_info__[:2 if __version_info__[2] == 0 else 3]))
 
 if __version_info__[3] in ('dev', 'post'):
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aad_helper.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aad_helper.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/activate_kernel_command.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/activate_kernel_command.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/adal_token_cache.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/adal_token_cache.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/ai_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/ai_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aimon_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aimon_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/allow_py_comments_before_cell.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/allow_py_comments_before_cell.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/allow_single_line_cell.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/allow_single_line_cell.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/aria_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/aria_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/bug_report.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/bug_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,28 +45,34 @@
 
         else:
             implementation_version = 'Unknown'
 
     except:
         pass
 
-    return {'name': implementation, 'version': implementation_version}
+    try:
+        implementation_branch = platform.python_branch()
+    except:
+        implementation_branch = 'Unknown'
+
+    return {'name': implementation, 'version': implementation_version, 'branch': implementation_branch}
 
 
 def _platform_info() -> dict:
     """Return a dict with the system version and release."""
 
-    platform_system = 'Unknown'
-    platform_release = 'Unknown'
     try:
         platform_system = platform.system()
-        platform_release = platform.release()
+    except:
+        platform_system = 'Unknown'
 
+    try:
+        platform_release = platform.release()
     except:
-        pass
+        platform_release = 'Unknown'
 
     return {'system': platform_system, 'release': platform_release}
 
 
 def _packages_info() -> dict:
     """Return a dict with installed packages version"""
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/cache_client.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/cache_client.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/cache_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/cache_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/column_guesser.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/column_guesser.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/connection.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/connection.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/constants.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,24 @@
             "support_auth_script":      True,
                     "support_reconnect_script": False,
             "support_file_url":         True,
                     "support__help_menu":       False,
                     "support_json_object":      False,
         },
 
+        "azuredatastudiosaw": {
+            "support_javascript":       True,
+            "support_deep_link_script": True,
+            "support_auth_script":      True,
+                    "support_reconnect_script": False,
+            "support_file_url":         True,
+                    "support__help_menu":       False,
+                    "support_json_object":      False,
+        },
+
         "visualstudiocode": {
             "support_javascript":       True,
             "support_deep_link_script": True,
             "support_auth_script":      True,
                     "support_reconnect_script": False,
             "support_file_url":         True,
                     "support__help_menu":       False,
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/database_html.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/database_html.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dependencies.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     dependencies: list = [
         ('dateutil.parser', 'python-dateutil', MANDATORY_TAG, "won't be able handle datetime properly", 'dateutil'),
         ('traitlets', 'traitlets', MANDATORY_TAG, "won't be able to use execute Kqlmagic", VERSION_IN_MODULE),
 
         ('prettytable', 'prettytable', OPTIONAL_TAG, "won't be able to display tables", VERSION_IN_MODULE),
         # ('tabulate', 'tabulate', OPTIONAL_TAG, "won't be able to display tables", VERSION_IN_MODULE),
-        ('requests', 'requests', OPTIONAL_TAG, "won't be able to query data sources, except local cache", VERSION_IN_MODULE),
+        ('requests', 'requests', OPTIONAL_TAG, "will use urllib, that might have ssl and or proxies restrictions", VERSION_IN_MODULE),
         ('msal', 'msal', OPTIONAL_TAG, "won't be able to authenticate using msal authentication modes, and Kqlmagic sso will be disabled", VERSION_IN_MODULE),
         ('azure.identity', 'azure-identity', OPTIONAL_TAG, "Some authentication options won't be available", VERSION_IN_MODULE),
         ('pandas', 'pandas', OPTIONAL_TAG, "won't be able to use dataframes", VERSION_IN_MODULE),
         ('IPython', 'ipython', OPTIONAL_TAG, "won't be to execute as an jupyter magic", VERSION_IN_MODULE),
         ('ipykernel', 'ipykernel', OPTIONAL_TAG, "won't be to execute as an jupyter magic on some jupyter variants", VERSION_IN_MODULE),
         ('pygments', 'pygments', OPTIONAL_TAG, "json objects won't be decorated with colors", VERSION_IN_MODULE),
         ('pygments.lexers.data', 'pygments', OPTIONAL_TAG, "json objects won't be decorated with colors", 'pygments'),
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dict_db_storage.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dict_db_storage.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/display.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def get_show_window_html_obj(window_name, file_path, button_text=None, onclick_visibility=None, isText:bool=None, palette:dict=None, before_text=None, after_text=None, close_window_timeout_in_secs=None, content=None, options=None):
         options = options or {}
         html_str = None
         mode = options.get("popup_interaction", "auto")
         if mode == "auto":
             if options.get("notebook_app") in ["ipython"] and options.get("test_notebook_app") in ["none", "ipython"]: 
                 mode = "webbrowser_open_at_kernel"
-            elif options.get("notebook_app") in ["visualstudiocode", "azuredatastudio"] and options.get("test_notebook_app") in ["none", "visualstudiocode", "azuredatastudio"]: 
+            elif options.get("notebook_app") in ["visualstudiocode", "azuredatastudiosaw", "azuredatastudio"] and options.get("test_notebook_app") in ["none", "visualstudiocode", "azuredatastudio", "azuredatastudiosaw"]: 
                 mode = "reference"
             elif options.get("notebook_app") in ["nteract"] and options.get("temp_files_server_address") is None:
                 mode = "reference"
             else:
                 mode = "button"
         if mode == "webbrowser_open_at_kernel":
             url = Display._get_file_path_url(file_path, options=options)
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dpapi_crypto.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dpapi_crypto.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/dpapi_crypto_msal.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/dpapi_crypto_msal.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/draft_client.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/draft_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 # --------------------------------------------------------------------------
 
 from typing import Union, Dict
 import uuid
 import json
 
 
-from .dependencies import Dependencies
 from .my_utils import json_dumps 
 from .constants import Constants, ConnStrKeys, Cloud, Schema
 from .kql_response import KqlQueryResponse, KqlSchemaResponse, KqlError
 # from .my_aad_helper import _MyAadHelper, ConnKeysKCSB
 from .my_aad_helper_msal import _MyAadHelper, ConnKeysKCSB
 from ._version import __version__
 from .log import logger
 from .kql_client import KqlClient
 from .exceptions import KqlEngineError
 
-
 class DraftClient(KqlClient):
     """Draft Client
 
         Parameters
         ----------
         conn_kv : dict
             Connection string key/value that contains the credentials to access the resource via Draft.
@@ -219,18 +217,18 @@
         KqlClient.last_query_info = {
             "request": {
                 "endpoint": api_url,
                 "headers": log_request_headers,
                 "timeout": options.get("timeout"),
             }
         }
-        requests = Dependencies.get_module("requests")
+
         if is_metadata:
             logger().debug(f"DraftClient::execute - GET request - url: {api_url}, headers: {log_request_headers}, timeout: {options.get('timeout')}")
-            response = requests.get(api_url, headers=request_headers, timeout=options.get("timeout"))
+            response = self._http_client.get(api_url, headers=request_headers, timeout=options.get("timeout"))
         else:
             request_payload = {
                 "query": query
             }
 
             # Implicit Cross Workspace Queries: https://dev.loganalytics.io/oms/documentation/3-Using-the-API/CrossResourceQuery
             # workspaces - string[] - A list of workspaces that are included in the query.
@@ -244,26 +242,26 @@
                     request_payload["timespan"] = timespan
 
             logger().debug(f"DraftClient::execute - POST request - url: {api_url}, headers: {log_request_headers}, payload: {request_payload}, timeout: {options.get('timeout')}")
 
             # collect this inormation, in case bug report will be generated
             self.last_query_info["request"]["payload"] = request_payload  # pylint: disable=unsupported-assignment-operation, unsubscriptable-object
 
-            response = requests.post(api_url, headers=request_headers, json=request_payload, timeout=options.get("timeout"))
+            response = self._http_client.post(api_url, headers=request_headers, json=request_payload, timeout=options.get("timeout"))
 
         logger().debug(f"DraftClient::execute - response - status: {response.status_code}, headers: {response.headers}, payload: {response.text}")
         #
         # handle response
         #
         # collect this inormation, in case bug report will be generated
         self.last_query_info["response"] = {  # pylint: disable=unsupported-assignment-operation
             "status_code": response.status_code
         }
 
-        if response.status_code != requests.codes.ok:  # pylint: disable=E1101
+        if response.status_code < 200  or response.status_code >= 300:  # pylint: disable=E1101
             try:
                 parsed_error = json.loads(response.text)
             except:
                 parsed_error = response.text
             # collect this inormation, in case bug report will be generated
             self.last_query_info["response"]["error"] = parsed_error  # pylint: disable=unsupported-assignment-operation, unsubscriptable-object
             raise KqlError(response.text, response)
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/email_notification.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/email_notification.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/fernet_crypto.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/fernet_crypto.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/help.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
 
 ## {Constants.MAGIC_CLASS_NAME_UPPER}_AZUREML_COMPUTE
 Specified azureml backend compute host address. If not specified popup windows might not work properly.<br>
 Default: value taken from {Constants.MAGIC_CLASS_NAME_UPPER}_NOTEBOOK_SERVICE_ADDRESS<br>
 <br>
 
 ## {Constants.MAGIC_CLASS_NAME_UPPER}_NOTEBOOK_APP
-Force the specified jupyter implementation. valid values are: "auto", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "nteract"<br>
+Force the specified jupyter implementation. valid values are: "auto", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "nteract", "azuredatastudiosaw"<br>
 Default: "auto" (auto detect implementation)<br>
 <br>
 
 ## {Constants.MAGIC_CLASS_NAME_UPPER}_LOAD_MODE
 If set to 'silent', banner won't be displayed on {Constants.MAGIC_PACKAGE_NAME} load. valid values: 'silent'<br>
 Default: None<br>
 <br>
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/help_html.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/help_html.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/ipython_api.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/ipython_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             return True
         else:
             return False
 
 
     @classmethod
     def try_kernel_reconnect(cls, **options)->bool:
-        if options is None or options.get("notebook_app") not in ["jupyterlab", "visualstudiocode", "azuredatastudio", "nteract"]:
+        if options is None or options.get("notebook_app") not in ["jupyterlab", "visualstudiocode", "azuredatastudio", "azuredatastudiosaw", "nteract"]:
             result = cls.try_kernel_execute("""try {IPython.notebook.kernel.reconnect();} catch(err) {;}""")
             time.sleep(1)
             return result
         else:
             return False
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_client.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 # --------------------------------------------------------------------------
 
 from typing import Union
 import uuid
 
 from .kql_response import KqlQueryResponse, KqlSchemaResponse
 from .aad_helper import AadHelper
+from .http_client import HttpClient
 
 
 class KqlClient(object):
 
     # collect this information, in case bug report will be generated
     last_query_info:dict = None
 
     _aad_helper:AadHelper
+    _http_client:HttpClient
 
     _session_guid:str = str(uuid.uuid4())
 
 
     def __init__(self)->None:
         self._aad_helper = None
+        self._http_client = HttpClient()
 
 
     def execute(self, id:str, query:str, accept_partial_results:bool=False, **options)->Union[KqlQueryResponse, KqlSchemaResponse]:
         raise NotImplementedError(self.__class__.__name__ + ".execute")
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_magic.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,23 +452,23 @@
         read_only=True,
         config=True, 
         allow_none=True, 
         help="""Notebook service address."""        
     )
 
     notebook_app = Enum(
-        ["auto", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "nteract"], 
+        ["auto", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "azuredatastudiosaw", "nteract"], 
         default_value="auto",
         read_only=True,
         config=True, 
         help="""Set notebook application used."""
     )  # TODO: add "papermill"
 
     test_notebook_app = Enum(
-        ["none", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "nteract"], 
+        ["none", "jupyterlab", "azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "ipython", "visualstudiocode", "azuredatastudio", "azuredatastudiosaw", "nteract"], 
         default_value="none",
         read_only=True,
         config=True, 
         help="""Set testing application mode, results should return for the specified notebook application."""
     )  # TODO: add "papermill"
 
     kernel_id = Unicode(
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_magic_core.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_magic_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import os
 import sys
+import platform
 import time
 import json
 import hashlib
 import urllib.parse
 import urllib.request
 import traceback
 import uuid
@@ -313,15 +314,19 @@
 
         #
         # first we do auto detection
         #
         app = "auto"
         if app == "auto":  # ELECTRON_RUN_AS_NODE
             notebook_service_address = self.default_options.notebook_service_address or ""
-            if notebook_service_address == "https://notebooks.azure.com" or notebook_service_address.endswith(".notebooks.azure.com"):
+            python_branch = platform.python_branch()
+            if python_branch.endswith("/msft-spython"):
+                app = "azuredatastudiosaw"
+                _kernel_location = "local"
+            elif notebook_service_address == "https://notebooks.azure.com" or notebook_service_address.endswith(".notebooks.azure.com"):
                 app = "azurenotebook"
                 _kernel_location = "remote"
             elif notebook_service_address.endswith((".azureml.net", ".azureml.ms")):
                 app = "azuremljupyternotebook" if is_env_var("AZUREML_NB_PATH") else "azuremljupyterlab"
                 _kernel_location = "remote"
             elif is_env_var("AZUREML_NB_PATH"):
                 app = "azuremljupyternotebook"
@@ -379,15 +384,17 @@
 
             self.default_options.set_trait("notebook_app", app, force=True, lock=True)
             logger().debug(f"Kqlmagic_core::_init_options - set default option 'notebook_app' to: {app}")
 
         kernel_location = self.default_options.kernel_location or "auto"
         if kernel_location == "auto":
             kernel_location = _kernel_location or "auto"
-            if kernel_location == "auto":
+            if app in ["azuredatastudiosaw"]:
+                kernel_location = "local"
+            elif kernel_location == "auto":
                 app_info = self.get_app_from_parent()
                 kernel_location = app_info.get("kernel_location", kernel_location)
             if kernel_location == "auto":           
                 if app in ["azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab"]:
                     kernel_location = "remote"
                 elif app in ["ipython"]:
                     kernel_location = "local"
@@ -409,15 +416,15 @@
             self.default_options.set_trait("table_package", table_package)
             logger().debug(f"Kqlmagic_core::_init_options - set default option 'table_package' to: {table_package}")
 
         temp_folder_location = self.default_options.temp_folder_location or "auto"
         if temp_folder_location == "auto":
             if kernel_location in ["auto", "remote"]:
                 temp_folder_location = "starting_dir"
-            elif app in ["azuredatastudio", "nteract", "visualstudiocode"]:
+            elif app in ["azuredatastudio", "azuredatastudiosaw", "nteract", "visualstudiocode"]:
                 temp_folder_location = "user_dir"
             elif app in ["azurenotebook", "azureml", "azuremljupyternotebook", "azuremljupyterlab", "jupyternotebook", "jupyterlab"]:
                 temp_folder_location = "starting_dir"
             else:
                 temp_folder_location = "starting_dir"
             self.default_options.set_trait("temp_folder_location", temp_folder_location, force=True, lock=True)
             logger().debug(f"Kqlmagic_core::_init_options - set default option 'temp_folder_location' to: {temp_folder_location}")
@@ -454,25 +461,29 @@
                         parent_proc = proc
                         break
 
                 if parent_proc is not None:
                     name = parent_proc.name().lower()
                     if name.startswith("nteract"):
                         return {"app": "nteract", "kernel_location": "local"}
+                    elif name.startswith("azuredatastudio-saw"):
+                        return {"app": "azuredatastudiosaw", "kernel_location": "local"}
                     elif name.startswith("azuredatastudio"):
                         return {"app": "azuredatastudio", "kernel_location": "local"}
                     cmdline = parent_proc.cmdline()
                     if cmdline is not None and len(cmdline) > 0:
                         for item in cmdline:
                             item = item.lower()
                             if item.endswith(".exe"):
                                 if item.endswith("jupyter-notebook.exe"):
                                     return {"app": "jupyternotebook"}
                                 elif item.endswith("jupyter-lab.exe"):
                                     return {"app": "jupyterlab"}
+                                elif item.endswith("azuredatastudio-saw.exe"):
+                                    return {"app": "azuredatastudiosaw", "kernel_location": "local"}
                                 elif item.endswith("azuredatastudio.exe"):
                                     return {"app": "azuredatastudio", "kernel_location": "local"}
                                 elif item.endswith("nteract.exe"):
                                     return {"app": "nteract", "kernel_location": "local"}
                                 elif item.endswith("vscode_datascience_helpers.kernel_launcher_daemon"):
                                     return {"app": "visualstudiocode", "kernel_location": "local"}
                                 elif item.endswith("vscode_datascience_helpers.jupyter_daemon"):
@@ -641,15 +652,15 @@
                 logger().debug("Kqlmagic_core::_show_what_new - failed to fetch HISTORY.md")
                 pass
 
 
     def _set_temp_files_server(self, options:Dict[str,Any]=None)->None:
         options = options or {}
         if (options.get("temp_files_server") == "kqlmagic"
-            or (options.get('notebook_app') in ["visualstudiocode", "azuredatastudio", "nteract"]
+            or (options.get('notebook_app') in ["visualstudiocode", "azuredatastudio", "azuredatastudiosaw", "nteract"]
                 and options.get("kernel_location") == "local"
                 and options.get("temp_files_server") == "auto")):
             if self.is_temp_files_server_on is None:
                 self._start_temp_files_server(options=options)
         elif self.is_temp_files_server_on is True:
             self._abort_temp_files_server(options)
 
@@ -1231,15 +1242,15 @@
         msg = self._get_connection_info(**options)
         if len(msg) > 0:
             Display.showInfoMessage(msg)
 
 
     def _add_help_to_jupyter_help_menu(self, user_ns:Dict[str,Any], start_time:float=None, options:dict=None)->None:
         options = options or {}
-        if Help_html.showfiles_base_url is None and self.default_options.notebook_app not in ["azuredatastudio", "ipython", "visualstudiocode", "nteract"]:
+        if Help_html.showfiles_base_url is None and self.default_options.notebook_app not in ["azuredatastudio", "azuredatastudiosaw", "ipython", "visualstudiocode", "nteract"]:
             if start_time is not None:
                 self._discover_notebook_url_start_time = start_time
             else:
                 now_time = time.time()   
                 seconds = now_time - self._discover_notebook_url_start_time
                 if (seconds < 5):
                     time.sleep(5 - seconds)
@@ -1668,20 +1679,23 @@
                 "azureml": "azureml",
                 "azuremljupyternotebook": "azuremljupyternotebook", 
                 "azuremljupyterlab": "azuremljupyterlab",
                 "jupyternotebook": "jupyternotebook", 
                 "ipython": "ipython", 
                 "visualstudiocode": "visualstudiocode",
                 "azuredatastudio": "azuredatastudio",
+                "azuredatastudiosaw": "azuredatastudiosaw",
                 "nteract": "nteract",
                 "lab": "jupyterlab", 
                 "notebook": "jupyternotebook", 
                 "ipy": "ipython", 
                 "vsc": "visualstudiocode",
                 "ads": "azuredatastudio",
+                "saw": "azuredatastudiosaw",
+                "secureadminworkstation": "azuredatastudiosaw",
                 "azurenotebooks": "azurenotebook",
                 # "papermill":"papermill" #TODO: add "papermill"
             }.get(lookup_key)
             if app is not None:
                 app = app.strip()
                 self.default_options.set_trait("notebook_app", app, force=True)
                 logger().debug(f"_override_default_configuration - set default option 'notebook_app' to: {app}")
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_proxy.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_proxy.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kql_response.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kql_response.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kusto_client.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kusto_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 from typing import Dict
 import re
 import uuid
 import json
 
 
-from .dependencies import Dependencies
-# from .my_aad_helper import _MyAadHelper, ConnKeysKCSB
 from .my_aad_helper_msal import _MyAadHelper, ConnKeysKCSB
 from .kql_response import KqlQueryResponse, KqlError
 from .constants import Constants, ConnStrKeys, Cloud
 from ._version import __version__
 from .log import logger
 from .exceptions import KqlEngineError
 from .my_utils import json_dumps 
@@ -276,29 +274,29 @@
             "request": {
                 "endpoint": endpoint,
                 "headers": log_request_headers,
                 "payload": request_payload,
                 "timeout": options.get("timeout"),
             }
         }
-        requests = Dependencies.get_module("requests")
-        response = requests.post(endpoint, headers=request_headers, json=request_payload, timeout=options.get("timeout"))
+
+        response = self._http_client.post(endpoint, headers=request_headers, json=request_payload, timeout=options.get("timeout"))
 
         logger().debug(f"KustoClient::execute - response - status: {response.status_code}, headers: {response.headers}, payload: {response.text}")
 
         # print("response status code: ", response.status_code)
         # print("response", response)
         # print("response text", response.text)
 
         # collect this information, in case bug report will be generated
         self.last_query_info["response"] = {  # pylint: disable=unsupported-assignment-operation
             "status_code": response.status_code
         }
 
-        if response.status_code != requests.codes.ok:  # pylint: disable=E1101
+        if response.status_code < 200  or response.status_code >= 300:  # pylint: disable=E1101
             try:
                 parsed_error = json.loads(response.text)
             except:
                 parsed_error = response.text
             # collect this information, in case bug report will be generated
             self.last_query_info["response"]["error"] = parsed_error  # pylint: disable=unsupported-assignment-operation, unsubscriptable-object
             raise KqlError(response.text, response)
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/kusto_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/kusto_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/la_engine.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/la_engine.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/log.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/log.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/magic_extension.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/magic_extension.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/msal_token_cache.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/msal_token_cache.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_aad_helper.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_aad_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,17 @@
                     logger().debug(f"_MyAadHelper::acquire_token - aad/code - resource: '{self._resource}', client: '{self._client_id}'")
                     code: dict = self._current_adal_context.acquire_user_code(self._resource, self._client_id)
                     url = code[OAuth2DeviceCodeResponseParameters.VERIFICATION_URL]
                     device_code = code[OAuth2DeviceCodeResponseParameters.USER_CODE].strip()
 
                     device_code_login_notification = self._options.get("device_code_login_notification")
                     if device_code_login_notification == "auto":
-                        if self._options.get("notebook_app") in ["ipython"]:
+                        if self._options.get("notebook_app") in ["visualstudiocodesaw"]:
+                            device_code_login_notification = "terminal"
+                        elif self._options.get("notebook_app") in ["ipython"]:
                             device_code_login_notification = "popup_interaction"
                         elif self._options.get("notebook_app") in ["visualstudiocode", "azuredatastudio"]:
                             device_code_login_notification = "popup_interaction"
                         elif self._options.get("notebook_app") in ["nteract"]:
 
                             if self._options.get("kernel_location") == "local":
                                 # ntreact cannot execute authentication script, workaround using temp_file_server webbrowser
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_aad_helper_msal.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_aad_helper_msal.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,19 +243,20 @@
 
 # shared cached context per authority
 global_msal_client_app_sso = {}
 
 
 class _MyAadHelper(AadHelper):
 
-    def __init__(self, kcsb, default_clientid, msal_client_app=None, msal_client_app_sso=None, **options):
+    def __init__(self, kcsb, default_clientid, msal_client_app=None, msal_client_app_sso=None, http_client=None, **options):
         global global_msal_client_app
         global global_msal_client_app_sso
 
         super(_MyAadHelper, self).__init__(kcsb, default_clientid, msal_client_app, msal_client_app_sso, **options)
+        self._http_client = http_client
         self._username = None
         if all([kcsb.aad_user_id, kcsb.password]):
             self._authentication_method = AuthenticationMethod.aad_username_password
             self._username = kcsb.aad_user_id
             self._password = kcsb.password
         elif all([kcsb.application_client_id, kcsb.application_key]):
             self._authentication_method = AuthenticationMethod.aad_application_key
@@ -445,15 +446,17 @@
                 elif self._authentication_method is AuthenticationMethod.aad_code_login:
                     flow = self._current_msal_client_app.initiate_device_flow(scopes=self._scopes)
                     url = flow[OAuth2DeviceCodeResponseParameters.VERIFICATION_URL]
                     device_code = flow[OAuth2DeviceCodeResponseParameters.USER_CODE].strip()
 
                     device_code_login_notification = self._options.get("device_code_login_notification")
                     if device_code_login_notification == "auto":
-                        if self._options.get("notebook_app") in ["ipython"]:
+                        if self._options.get("notebook_app") in ["visualstudiocodesaw"]:
+                            device_code_login_notification = "terminal"
+                        elif self._options.get("notebook_app") in ["ipython"]:
                             device_code_login_notification = "popup_interaction"
                         elif self._options.get("notebook_app") in ["visualstudiocode", "azuredatastudio"]:
                             device_code_login_notification = "popup_interaction"
                         elif self._options.get("notebook_app") in ["nteract"]:
 
                             if self._options.get("kernel_location") == "local":
                                 # ntreact cannot execute authentication script, workaround using temp_file_server webbrowser
@@ -998,15 +1001,15 @@
                 # print(f">>> _get_token_authority: {self._get_token_authority(token)}")
                 # print(f">>> _get_authority_from_token: {self._get_authority_from_token(token)}")
                 # print(f">>> _get_token_client_id: {self._get_token_client_id(token)}")
                 # print(f">>> _get_client_id_from_token: {self._get_client_id_from_token(token)}")
                 # print(f">>> _get_token_user_id: {self._get_token_user_id(token)}")
                 # print(f">>> _get_username_from_token: {self._get_username_from_token(token)}")
 
-                app = msal.PublicClientApplication(client_id, authority=authority_uri)
+                app = msal.PublicClientApplication(client_id, authority=authority_uri, http_client=self._http_client)
                 result = app.acquire_token_by_refresh_token(refresh_token, scopes)  # pylint: disable=no-member
                 if "error" in result:
                     self._warn_on_token_validation_failure(f"failed to migrate token to msal app: {result}")
                 else:
                     valid_token = self._acquire_msal_token_silent(client_app_type=ClientAppType.public, msal_client_app=app, scopes=scopes, username=username)
                     _vtk = {x:"XXXXX" if x.lower().endswith("token") else valid_token[x] for x in valid_token}
                     vclaims = self._get_token_claims(self._get_token_access_token(valid_token))
@@ -1071,17 +1074,17 @@
         # return json.dumps(client_app_key)
 
     def _create_client_app(self, cache=None):
         client_app = None
         msal = Dependencies.get_module("msal", dont_throw=True)
         if msal:
             if self._client_app_type == ClientAppType.public:
-                client_app = msal.PublicClientApplication(self._client_id, authority=self._authority_uri, token_cache=cache)
+                client_app = msal.PublicClientApplication(self._client_id, authority=self._authority_uri, token_cache=cache, http_client=self._http_client)
             elif self._client_app_type == ClientAppType.confidential:
-                client_app = msal.ConfidentialClientApplication(self._client_id, authority=self._authority_uri, client_credential=self._client_credential, token_cache=cache)
+                client_app = msal.ConfidentialClientApplication(self._client_id, authority=self._authority_uri, client_credential=self._client_credential, token_cache=cache, http_client=self._http_client)
         return client_app
 
 
 
     def _set_msal_client_app(self, msal_client_app=None, msal_client_app_sso=None):
         "set the msal application"
         global global_msal_client_app
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_files_server.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_files_server.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_files_server_management.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_files_server_management.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/my_utils.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/my_utils.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/palette.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/palette.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/parameterizer.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/parameterizer.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/parser.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/parser.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/python_command.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/python_command.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/results.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,16 @@
     spaces = "&nbsp;" * len(match_obj.group(2))
     return f"{match_obj.group(1)}{spaces}"
 
 
 class DisplayRows(list):
 
     def __init__(self, rows:list, limit:int):
-        self.limit = min(limit or len(rows), len(rows))
-        self.rows = rows
+        self.rows = [] if rows is None else rows
+        self.limit = len(self.rows) if limit is None else min(max(0, limit), len(self.rows))
         self.row_index = 0
 
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             if key.start and key.start >= self.limit:
                 return
@@ -545,37 +545,46 @@
             )
         return None
 
 
     def _getPrettyTableHtml(self)->Dict[str,str]:
         "get query result in a table format as an HTML string"
 
-        display_limit = 0 if not self.options.get("display_limit") else self.options.get("display_limit")
-        table = DisplayRows(self, display_limit)
-        prettytable = Dependencies.get_module('prettytable', dont_throw=True)
-        if prettytable:
-            if self.pretty is None:
-                # table printing style to any of prettytable's defined styles (currently DEFAULT, MSWORD_FRIENDLY, PLAIN_COLUMNS, RANDOM)
-                prettytable_style = prettytable.__dict__[self.options.get("prettytable_style", "DEFAULT").upper()]
-                self.pretty = PrettyTable(self.field_names, style=prettytable_style) if len(self.field_names) > 0 else None
-            self.pretty.add_rows(table)
-            result = self.pretty.get_html_string()
-            _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
-            result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
-        else:
-            tabulate = Dependencies.get_module('tabulate', dont_throw=True)
-            if tabulate:
-                result = tabulate.tabulate(table, self.field_names, tablefmt="html")
+        display_limit = self.options.get("display_limit")
+        if display_limit is None:
+            display_limit = len(self)
+
+        if display_limit >= 0:
+            table = DisplayRows(self, display_limit)
+            prettytable = Dependencies.get_module('prettytable', dont_throw=True)
+            if prettytable:
+                if self.pretty is None:
+                    # table printing style to any of prettytable's defined styles (currently DEFAULT, MSWORD_FRIENDLY, PLAIN_COLUMNS, RANDOM)
+                    prettytable_style = prettytable.__dict__[self.options.get("prettytable_style", "DEFAULT").upper()]
+                    self.pretty = PrettyTable(self.field_names, style=prettytable_style) if len(self.field_names) > 0 else None
+
+                self.pretty.add_rows(table)
+                result = self.pretty.get_html_string()
+                _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
+                result = _cell_with_spaces_pattern.sub(_nonbreaking_spaces, result)
             else:
-                prettytable = Dependencies.get_module('prettytable')
-                return {}
+                tabulate = Dependencies.get_module('tabulate', dont_throw=True)
+                if tabulate:
+                    result = tabulate.tabulate(table, self.field_names, tablefmt="html")
+                else:
+                    prettytable = Dependencies.get_module('prettytable')
+                    return {}
+
+            if len(self) > display_limit:
+                result = f'{result}\n<span style="font-style:italic;text-align:center;">{len(self)} rows, truncated to display_limit of {display_limit}</span>'
+            
+            return {"body": result}
+        else:
+            return {}
 
-        if display_limit > 0 and len(self) > display_limit:
-            result = f'{result}\n<span style="font-style:italic;text-align:center;">{len(self)} rows, truncated to display_limit of {display_limit}</span>'
-        return {"body": result}
 
 
     def need_suppress_next_workaround(self)->bool:
         if self.options.get("table_package") != "pandas_html_table_schema" \
                 or self.options.get("popup_window") \
                 or (len(self) == 1 and len(self[0]) == 1 and (isinstance(self[0][0], dict) or isinstance(self[0][0], list))):
             return False
@@ -591,45 +600,47 @@
         pd = None
         pandas__repr_data_resource_ = None
         pandas_display_html_table_schema = None
         pandas__repr_data_resource_patched = False
         if not options.get("popup_window") and len(self) == 1 and len(self[0]) == 1 and (isinstance(self[0][0], dict) or isinstance(self[0][0], list)):
             content = Display.to_json_styled_class(self[0][0], options=options)
         else:
-            if options.get("table_package", "").lower() in ["pandas", "pandas_html_table_schema"]:
+            display_limit = options.get("display_limit")
+            if type(display_limit) == int and display_limit < 0:
+                content = Display.toHtml(**{}, title='table')
+
+            elif options.get("table_package", "").lower() in ["pandas", "pandas_html_table_schema"]:
                 pd = Dependencies.get_module("pandas")
 
                 df = self.to_dataframe()
-                display_limit = options.get("display_limit")
                 if display_limit is not None:
                     df = df.head(display_limit)
 
                 pd.set_option('display.max_rows', display_limit)
                 pd.set_option('display.max_columns', None)
                 try:
                     pd.set_option('display.min_rows', display_limit)
                 except:
                     pass
                 pd.set_option('display.large_repr', "truncate")
 
-
                 if options.get("table_package", "") == "pandas_html_table_schema" and not options.get("popup_window"):
                     df_copied = False
                     for idx, column_type in enumerate(self.columns_type):
                         if column_type == "dynamic":
                             if not df_copied:
                                 df_copied =  True
                                 df = df.copy()
                             col_name = self.columns_name[idx]
                             for item_idx, item in enumerate(df[col_name]):
                                 df.loc[item_idx, col_name] = f"{item}"
 
                     pandas_display_html_table_schema = pd.options.display.html.table_schema
                     pd.options.display.html.table_schema = True
-                    if options.get("notebook_app") in ["azuredatastudio"]:
+                    if options.get("notebook_app") in ["azuredatastudio", "azuredatastudiosaw"]:
                         pandas__repr_data_resource_ = self._patch_pandas__repr_data_resource_()
                         pandas__repr_data_resource_patched = True
                     content = df
 
                 else:
                     pandas_display_html_table_schema = pd.options.display.html.table_schema
                     pd.options.display.html.table_schema = False
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/sso_storage.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/sso_storage.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/azure/Kqlmagic/version.py` & `KqlmagicCustom-0.1.114.post9/azure/Kqlmagic/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,18 @@
 
 import sys
 import re
 from functools import cmp_to_key
 from typing import Any, Dict, Tuple, Iterable
 
 
-import requests
-
-
 from .constants import Constants
 from .help import MarkdownString
 from ._version import __version__
+from .http_client import HttpClient
 
 
 _IGNORE_POST_VERSION_PATTERN = r'[.]?(post|rev|r)[0-9]*$'
 _IS_STABLE_VESRION_PATTERN = r'[v]?([0-9]+[!])?[0-9]+(\.[0-9]*)*([.]?(post|rev|r)[0-9]*)?$'
 
 try:
     import pkg_resources
@@ -382,15 +380,16 @@
     Raises
     ------
     RequestsException
         If request to PyPI fails.
     """
 
     api_url = f"https://pypi.org/pypi/{package_name}/json"
-    response = requests.get(api_url)
+    http_client = HttpClient()
+    response = http_client.get(api_url)
 
     #
     # handle response
     #
 
     response.raise_for_status()
     json_response = response.json()
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/PKG-INFO` & `KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KqlmagicCustom
-Version: 0.1.114.post8
+Version: 0.1.114.post9
 Summary: Kqlmagic: Microsoft Azure Monitor magic extension to Jupyter notebook (Custom Dependencies)
 Home-page: https://github.com/Microsoft/jupyter-Kqlmagic
 Author: Michael Binshtock
 Author-email: michabin@microsoft.com
 Maintainer: Michael Binshtock
 Maintainer-email: michabin@microsoft.com
 License: MIT License
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: default
 Provides-Extra: naked
+Provides-Extra: saw
 Provides-Extra: jupyter-basic
 Provides-Extra: ipython-basic
 Provides-Extra: python-basic
 Provides-Extra: basic
 Provides-Extra: jupyter-extended
 Provides-Extra: ipython-extended
 Provides-Extra: python-extended
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/SOURCES.txt` & `KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 azure/Kqlmagic/draft_client.py
 azure/Kqlmagic/email_notification.py
 azure/Kqlmagic/engine.py
 azure/Kqlmagic/exceptions.py
 azure/Kqlmagic/fernet_crypto.py
 azure/Kqlmagic/help.py
 azure/Kqlmagic/help_html.py
+azure/Kqlmagic/http_client.py
 azure/Kqlmagic/ipython_api.py
 azure/Kqlmagic/kql_client.py
 azure/Kqlmagic/kql_engine.py
 azure/Kqlmagic/kql_magic.py
 azure/Kqlmagic/kql_magic_core.py
 azure/Kqlmagic/kql_proxy.py
 azure/Kqlmagic/kql_response.py
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure/KqlmagicCustom.egg-info/requires.txt` & `KqlmagicCustom-0.1.114.post9/azure/KqlmagicCustom.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,200 +11,200 @@
 [base_utils]
 psutil>=5.4.7
 setuptools>=41.0.1
 flask>=1.0.3
 isodate>=0.6.0
 
 [basic]
-requests>=2.21.0
-ipykernel>=5.1.1
-msal>=1.11.0
 ipython>=7.1.1
+ipykernel>=5.1.1
 prettytable>=0.7.2
+msal>=1.11.0
+requests>=2.21.0
 
 [default]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
+ipython>=7.1.1
 matplotlib>=3.0.0
-plotly>=3.10.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-pandas>=0.23.4
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
+Markdown>=3.0.1
 ipywidgets
-Pygments>=2.2.0
+psutil>=5.4.7
+azure-identity>=1.5.0
+setuptools>=41.0.1
+msal-extensions>=0.3.0
 requests>=2.21.0
-Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
 flask>=1.0.3
-azure-identity>=1.5.0
+plotly>=3.10.0
+msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
 ipykernel>=5.1.1
+password-strength>=0.0.3
+isodate>=0.6.0
+pandas>=0.23.4
+lxml>=4.2.5
 msal>=1.11.0
-ipython>=7.1.1
-msal-extensions>=0.3.0
-pyperclip>=1.7.0
-msrestazure>=0.6.3
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [dev]
 twine
 pip
 wheel
 black
 flake8
 pipreqs
 mccabe
 pep8autopep8
 pydocstyle
 
 [extended]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
+ipython>=7.1.1
 matplotlib>=3.0.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-beautifulsoup4>=4.6.3
+Markdown>=3.0.1
 psutil>=5.4.7
-Pygments>=2.2.0
+azure-identity>=1.5.0
+setuptools>=41.0.1
+msal-extensions>=0.3.0
 requests>=2.21.0
-Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
 flask>=1.0.3
-azure-identity>=1.5.0
+msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
 ipykernel>=5.1.1
+password-strength>=0.0.3
+isodate>=0.6.0
+lxml>=4.2.5
 msal>=1.11.0
-ipython>=7.1.1
-msal-extensions>=0.3.0
-pyperclip>=1.7.0
-msrestazure>=0.6.3
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [ipython-all]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
+ipython>=7.1.1
 matplotlib>=3.0.0
-plotly>=3.10.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-pandas>=0.23.4
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
-ipywidgets
-Pygments>=2.2.0
-requests>=2.21.0
 Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
-flask>=1.0.3
+ipywidgets
+psutil>=5.4.7
 azure-identity>=1.5.0
-msal>=1.11.0
-ipython>=7.1.1
+setuptools>=41.0.1
 msal-extensions>=0.3.0
-pyperclip>=1.7.0
+requests>=2.21.0
+flask>=1.0.3
+plotly>=3.10.0
 msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
+password-strength>=0.0.3
+isodate>=0.6.0
+pandas>=0.23.4
+lxml>=4.2.5
+msal>=1.11.0
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [ipython-basic]
 prettytable>=0.7.2
 ipython>=7.1.1
 msal>=1.11.0
 requests>=2.21.0
 
 [ipython-extended]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
+ipython>=7.1.1
 matplotlib>=3.0.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
-Pygments>=2.2.0
-requests>=2.21.0
 Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
-flask>=1.0.3
+psutil>=5.4.7
 azure-identity>=1.5.0
-msal>=1.11.0
-ipython>=7.1.1
+setuptools>=41.0.1
 msal-extensions>=0.3.0
-pyperclip>=1.7.0
+requests>=2.21.0
+flask>=1.0.3
 msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
+password-strength>=0.0.3
+isodate>=0.6.0
+lxml>=4.2.5
+msal>=1.11.0
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [json_color]
 Pygments>=2.2.0
 
 [jupyter-all]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
 matplotlib>=3.0.0
-plotly>=3.10.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-pandas>=0.23.4
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
+Markdown>=3.0.1
 ipywidgets
-Pygments>=2.2.0
+psutil>=5.4.7
+azure-identity>=1.5.0
+setuptools>=41.0.1
+msal-extensions>=0.3.0
 requests>=2.21.0
-Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
 flask>=1.0.3
-azure-identity>=1.5.0
+plotly>=3.10.0
+msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
 ipykernel>=5.1.1
+password-strength>=0.0.3
+isodate>=0.6.0
+pandas>=0.23.4
+lxml>=4.2.5
 msal>=1.11.0
-msal-extensions>=0.3.0
-pyperclip>=1.7.0
-msrestazure>=0.6.3
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [jupyter-basic]
 prettytable>=0.7.2
 ipykernel>=5.1.1
 msal>=1.11.0
 requests>=2.21.0
 
 [jupyter-extended]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
 matplotlib>=3.0.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-beautifulsoup4>=4.6.3
+Markdown>=3.0.1
 psutil>=5.4.7
-Pygments>=2.2.0
+azure-identity>=1.5.0
+setuptools>=41.0.1
+msal-extensions>=0.3.0
 requests>=2.21.0
-Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
 flask>=1.0.3
-azure-identity>=1.5.0
+msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
 ipykernel>=5.1.1
+password-strength>=0.0.3
+isodate>=0.6.0
+lxml>=4.2.5
 msal>=1.11.0
-msal-extensions>=0.3.0
-pyperclip>=1.7.0
-msrestazure>=0.6.3
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [kqlmagic_fernet_sso]
 cryptography>=2.7
 password-strength>=0.0.3
 
 [kqlmagic_msal_sso]
 cryptography>=2.7
 password-strength>=0.0.3
 
 [kqlmagic_sso]
-cryptography>=2.7
 password-strength>=0.0.3
+cryptography>=2.7
 msal>=1.11.0
 msal-extensions>=0.3.0
 
 [matplotlib_palettes]
 matplotlib>=3.0.0
 
 [msal_sso]
@@ -218,71 +218,79 @@
 [pandas]
 pandas>=0.23.4
 
 [plotly]
 plotly>=3.10.0
 
 [python-all]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
 matplotlib>=3.0.0
-plotly>=3.10.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-pandas>=0.23.4
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
-ipywidgets
-Pygments>=2.2.0
-requests>=2.21.0
 Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
-flask>=1.0.3
+ipywidgets
+psutil>=5.4.7
 azure-identity>=1.5.0
-msal>=1.11.0
+setuptools>=41.0.1
 msal-extensions>=0.3.0
-pyperclip>=1.7.0
+requests>=2.21.0
+flask>=1.0.3
+plotly>=3.10.0
 msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
+password-strength>=0.0.3
+isodate>=0.6.0
+pandas>=0.23.4
+lxml>=4.2.5
+msal>=1.11.0
+cryptography>=2.7
+beautifulsoup4>=4.6.3
 
 [python-basic]
 prettytable>=0.7.2
 msal>=1.11.0
 requests>=2.21.0
 
 [python-extended]
-setuptools>=41.0.1
-cryptography>=2.7
+pyperclip>=1.7.0
 matplotlib>=3.0.0
-password-strength>=0.0.3
-prettytable>=0.7.2
 azure-common>=1.1.25
-beautifulsoup4>=4.6.3
-psutil>=5.4.7
-Pygments>=2.2.0
-requests>=2.21.0
 Markdown>=3.0.1
-lxml>=4.2.5
-isodate>=0.6.0
-flask>=1.0.3
+psutil>=5.4.7
 azure-identity>=1.5.0
-msal>=1.11.0
+setuptools>=41.0.1
 msal-extensions>=0.3.0
-pyperclip>=1.7.0
+requests>=2.21.0
+flask>=1.0.3
 msrestazure>=0.6.3
+prettytable>=0.7.2
+Pygments>=2.2.0
+password-strength>=0.0.3
+isodate>=0.6.0
+lxml>=4.2.5
+msal>=1.11.0
+cryptography>=2.7
+beautifulsoup4>=4.6.3
+
+[saw]
+ipython>=7.1.1
+ipykernel>=5.1.1
+pandas>=0.23.4
+msal>=1.11.0
+Pygments>=2.2.0
+ipywidgets
 
 [sso]
-cryptography>=2.7
-azure-identity>=1.5.0
 password-strength>=0.0.3
-msal>=1.11.0
-msal-extensions>=0.3.0
+azure-identity>=1.5.0
 msrestazure>=0.6.3
+msal-extensions>=0.3.0
 azure-common>=1.1.25
+msal>=1.11.0
+cryptography>=2.7
 
 [tests]
 pytest
 pytest-pep8
 pytest-docstyle
 pytest-flakes
 pytest-cov
@@ -291,23 +299,23 @@
 
 [text_utils]
 Markdown>=3.0.1
 beautifulsoup4>=4.6.3
 lxml>=4.2.5
 
 [utils]
-isodate>=0.6.0
+pyperclip>=1.7.0
+psutil>=5.4.7
 flask>=1.0.3
-setuptools>=41.0.1
+isodate>=0.6.0
 matplotlib>=3.0.0
-beautifulsoup4>=4.6.3
-Markdown>=3.0.1
+setuptools>=41.0.1
 lxml>=4.2.5
-pyperclip>=1.7.0
-psutil>=5.4.7
+Markdown>=3.0.1
 Pygments>=2.2.0
+beautifulsoup4>=4.6.3
 
 [vscode_sso]
 azure-identity>=1.5.0
 
 [widgets]
 ipywidgets
```

### Comparing `KqlmagicCustom-0.1.114.post8/azure_bdist_wheel.py` & `KqlmagicCustom-0.1.114.post9/azure_bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `KqlmagicCustom-0.1.114.post8/setup.py` & `KqlmagicCustom-0.1.114.post9/setup.py`

 * *Files identical despite different names*

