# Comparing `tmp/aegis-tools-2.5.5.tar.gz` & `tmp/aegis-tools-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.5.5.tar", last modified: Tue Apr  2 02:20:33 2024, max compression
+gzip compressed data, was "aegis-tools-2.5.6.tar", last modified: Thu Apr 18 02:55:17 2024, max compression
```

## Comparing `aegis-tools-2.5.5.tar` & `aegis-tools-2.5.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.379211 aegis-tools-2.5.5/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.359211 aegis-tools-2.5.5/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20800 2024-03-21 19:10:22.000000 aegis-tools-2.5.5/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19045 2024-01-31 22:09:14.000000 aegis-tools-2.5.5/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.5/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24750 2024-03-21 19:10:22.000000 aegis-tools-2.5.5/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27285 2024-03-25 22:46:01.000000 aegis-tools-2.5.5/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.5/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46086 2024-04-02 02:17:33.000000 aegis-tools-2.5.5/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.367211 aegis-tools-2.5.5/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.5/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.5/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.5/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.5/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.5/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    33163 2024-02-23 20:02:21.000000 aegis-tools-2.5.5/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.5/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.5/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.5/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.5/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.5/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.5/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.5/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.5/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.5/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.5/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.5/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.5/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.5/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.5/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78603 2024-04-02 02:17:33.000000 aegis-tools-2.5.5/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-02 02:20:33.375211 aegis-tools-2.5.5/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-02 02:20:33.000000 aegis-tools-2.5.5/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-02 02:20:33.379211 aegis-tools-2.5.5/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.5/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-18 02:55:17.782236 aegis-tools-2.5.6/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-18 02:55:17.782236 aegis-tools-2.5.6/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-18 02:55:17.766236 aegis-tools-2.5.6/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    20800 2024-03-21 19:10:22.000000 aegis-tools-2.5.6/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    19045 2024-01-31 22:09:14.000000 aegis-tools-2.5.6/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2831 2024-02-09 21:33:25.000000 aegis-tools-2.5.6/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    24750 2024-03-21 19:10:22.000000 aegis-tools-2.5.6/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    27285 2024-03-25 22:46:01.000000 aegis-tools-2.5.6/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.5.6/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    46086 2024-04-02 02:17:33.000000 aegis-tools-2.5.6/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-18 02:55:17.770236 aegis-tools-2.5.6/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.5.6/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4611 2024-01-31 22:04:42.000000 aegis-tools-2.5.6/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.5.6/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.5.6/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.5.6/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    37012 2024-04-18 02:54:56.000000 aegis-tools-2.5.6/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-18 02:55:17.778236 aegis-tools-2.5.6/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3071 2023-09-30 03:49:20.000000 aegis-tools-2.5.6/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.5.6/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.5.6/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.5.6/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3377 2023-08-14 03:31:20.000000 aegis-tools-2.5.6/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2238 2023-09-30 03:49:39.000000 aegis-tools-2.5.6/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.5.6/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1857 2023-09-30 03:52:25.000000 aegis-tools-2.5.6/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.5.6/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.5.6/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.5.6/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.5.6/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.5.6/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.5.6/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    78603 2024-04-02 02:17:33.000000 aegis-tools-2.5.6/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2024-04-18 02:55:17.782236 aegis-tools-2.5.6/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2024-04-18 02:55:17.000000 aegis-tools-2.5.6/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2024-04-18 02:55:17.782236 aegis-tools-2.5.6/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1716 2023-09-26 15:24:50.000000 aegis-tools-2.5.6/setup.py
```

### Comparing `aegis-tools-2.5.5/LICENSE` & `aegis-tools-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/PKG-INFO` & `aegis-tools-2.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.5
+Version: 2.5.6
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.5/README.md` & `aegis-tools-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/aegis_.py` & `aegis-tools-2.5.6/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/build.py` & `aegis-tools-2.5.6/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/config.py` & `aegis-tools-2.5.6/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/database.py` & `aegis-tools-2.5.6/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/hydra.py` & `aegis-tools-2.5.6/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/mailer.py` & `aegis-tools-2.5.6/aegis/mailer.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/model.py` & `aegis-tools-2.5.6/aegis/model.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.5.6/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.5.6/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/build-mysql.sql` & `aegis-tools-2.5.6/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/build-pgsql.sql` & `aegis-tools-2.5.6/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.5.6/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/google_signin.sql` & `aegis-tools-2.5.6/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.5.6/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.5.6/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/member_auth.sql` & `aegis-tools-2.5.6/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.5.6/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/sql/reports.sql` & `aegis-tools-2.5.6/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/stdlib.py` & `aegis-tools-2.5.6/aegis/stdlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 import json
 import logging
 import os
 import pprint
 import random
 import re
 import shlex
+import signal
 import socket
 import string
 import subprocess
 import sys
+import threading
 import time
 import urllib.parse
 import xml
 
 # Extern Imports
 import bcrypt
 import dateutil.parser
@@ -279,20 +281,22 @@
         if not count:
             break
     if rjust:
         return amt.rjust(rjust)
     return amt
 
 
-# >>> "%4.2f Trillion Should Be Enough" % (float(26*pow(36, 7)) / float(pow(1024, 4)))
-# '1.85 Trillion Should Be Enough'
-# >>> "If Not, %4.2f Trillion Should Definitely Be Enough" % (float(26*pow(36, 9)) / float(pow(1024, 4)))
-# 'If Not, 2401.57 Trillion Should Definitely Be Enough'
-
-# Combine with a second factor like a row_id to eliminate unbelievably lucky brute force possibilities. Enforce at least one letter so it can't be cast to an int
+# Token format that is unique and hard to guess. Enforce at least one letter so it can't accidentally be cast to an int.
+# Combine with a second factor like a row_id to eliminate unbelievably lucky brute force possibilities.
+#>>> chars=8; "%4.2f Trillion Should Be Enough For Just %s Chars" % (float(26*pow(36, chars-1)) / float(pow(1024, 4)), chars)
+#'1.85 Trillion Should Be Enough For Just 8 Chars'
+#>>> chars=10; "If not, %4.2f Trillion in %s Chars Should Definitely Be Enough" % (float(26*pow(36, chars-1)) / float(pow(1024, 4)), chars)
+#'If not, 2401.57 Trillion in 10 Chars Should Definitely Be Enough'
+#>>> chars=12; "Ludicrous Odds: %s Chars Makes For %4.2f Trillion Possibilities (3 Quintillion)" % (chars, float(26*pow(36, chars-1)) / float(pow(1024, 4)))
+#'Ludicrous Odds: 12 Chars Makes For 3112440.30 Trillion Possibilities (3 Quintillion)'
 token_length = 10
 token_chars = string.ascii_letters + string.digits
 def magic_token(length=token_length):
     return random.choice(string.ascii_lowercase) + functools.reduce(lambda x, y: x + random.choice(token_chars), range(length-1), '').lower()
 
 def validate_token(row_id, token):
     return validate_int(row_id) and token and len([ch for ch in token if ch in token_chars]) == token_length
@@ -1013,7 +1017,82 @@
 def write_version(version_str):
     # write config files into the build directory and not version control
     aegis_dir = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
     version_file = os.path.join(aegis_dir, 'version.json')
     version_json = open(version_file, 'w')
     version_json.write('{"version": "%s"}\n' % version_str)
     version_json.close()
+
+
+class DaemonThread(threading.Thread):
+    # quitting uses threading.Event() at the class level to synchronize flags between threads
+    quitting = threading.Event()
+    filename = __file__
+
+    def __init__(self, *args, **kwargs):
+        threading.Thread.__init__(self, *args, **kwargs)
+        self.start_t = time.time()
+        self.record_cnt = 0
+        self.last_id = 0
+
+    # Alert and debug hooks likely need to be defined in applications
+    def exception_alert(self, ex):
+        logw(ex, "EXCEPTION ALERT - OVERRIDE ME IN CHILD CLASS")
+        # XXX TODO It could default to channels
+
+    def run(self):
+        try:
+            self.process()
+        except Exception as ex:
+            logging.exception(ex)
+            self.exception_alert(ex)
+
+    def finish(self):
+        end_t = time.time()
+        exec_t = end_t - self.start_t
+        recs_s = max(float(self.record_cnt), 1.0) / exec_t
+        recs_h = max(float(self.record_cnt), 1.0) / exec_t * 3600
+        logging.info("%s ending.  Records: %d   Seconds: %4.3f   Records/sec: %4.3f   Records/hr: %4.3f   Last Id: %s", self.name, self.record_cnt, exec_t, recs_s, recs_h, self.last_id)
+
+    def main_thread(self, sleep_sec=3):
+        # Handling signals only works in the main thread
+        signal.signal(signal.SIGINT, self.signal_stop)
+        signal.signal(signal.SIGTERM, self.signal_stop)
+        signal.signal(signal.SIGHUP, self.signal_stop)
+        signal.signal(signal.SIGUSR1, self.signal_debug)
+        # Main thread is used only as a control thread... monitors quitting variable, and sleep gets interrupted by signal. And that's it!
+        while threading.active_count() > 1:
+            if DaemonThread.quitting.is_set():
+                logging.warning("DaemonThread waiting %ss for threads to finish... %s active" % (sleep_sec, threading.active_count()))
+                threads = threading.enumerate()
+                if len(threads) > 1:
+                    thr = random.choice(threads[1:])
+                    if thr != threading.current_thread():
+                        thr.join(1.0)
+            else:
+                time.sleep(sleep_sec)
+
+    @staticmethod
+    def signal_stop(signal, frm):
+        logging.warning('SIGINT or SIGTERM received (%s). Quitting now...', signal)
+        DaemonThread.quitting.set()
+
+    # Debug dump in response to kill -SIGUSR1
+    @staticmethod
+    def signal_debug(sig, frame):
+        """Interrupt running process, and provide a stack trace for each thread. Trigger using kill -SIGUSR1 <pid>"""
+        # Show memory usage
+        import pympler
+        all_objects = pympler.muppy.get_objects()
+        summary1 = pympler.summary.summarize(all_objects)
+        formatted = pympler.summary.format_(summary1)
+        logging.warning("Received SIGUSR1 - Dumping Debug Output" + "\n".join(formatted) + "\n")
+        # Dump a stack trace on each thread
+        id2name = dict([(th.ident, th.name) for th in threading.enumerate()])
+        code = []
+        for threadId, stack in sys._current_frames().items():
+            code.append("\n# Thread: %s(%d)" % (id2name.get(threadId,""), threadId))
+            for filename, lineno, name, line in traceback.extract_stack(stack):
+                code.append('File: "%s", line %d, in %s' % (filename, lineno, name))
+                if line:
+                    code.append("  %s" % (line.strip()))
+        logging.warning("\n".join(code))
```

### Comparing `aegis-tools-2.5.5/aegis/templates/build.html` & `aegis-tools-2.5.6/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/build_confirm.html` & `aegis-tools-2.5.6/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/build_form.html` & `aegis-tools-2.5.6/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/build_view.html` & `aegis-tools-2.5.6/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/frame.html` & `aegis-tools-2.5.6/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/hydra.html` & `aegis-tools-2.5.6/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/hydra_form.html` & `aegis-tools-2.5.6/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/hydra_queue.html` & `aegis-tools-2.5.6/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/report.html` & `aegis-tools-2.5.6/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/report_form.html` & `aegis-tools-2.5.6/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/reports.html` & `aegis-tools-2.5.6/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/templates/w3.css` & `aegis-tools-2.5.6/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/threadpool.py` & `aegis-tools-2.5.6/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis/webapp.py` & `aegis-tools-2.5.6/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.5.6/aegis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.5.5
+Version: 2.5.6
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.5.5/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.5.6/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.5.5/setup.py` & `aegis-tools-2.5.6/setup.py`

 * *Files identical despite different names*

