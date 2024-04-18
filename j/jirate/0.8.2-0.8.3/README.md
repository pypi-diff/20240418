# Comparing `tmp/jirate-0.8.2.tar.gz` & `tmp/jirate-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jirate-0.8.2.tar", last modified: Tue Mar 26 14:52:34 2024, max compression
+gzip compressed data, was "jirate-0.8.3.tar", last modified: Thu Apr 18 14:29:37 2024, max compression
```

## Comparing `jirate-0.8.2.tar` & `jirate-0.8.3.tar`

### file list

```diff
@@ -1,24 +1,53 @@
-drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-03-26 14:52:34.452787 jirate-0.8.2/
--rw-rw-r--   0 lhh       (3368) lhh       (3368)     1352 2021-03-15 13:10:12.000000 jirate-0.8.2/LICENSE.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)     1606 2024-03-26 14:52:34.451787 jirate-0.8.2/PKG-INFO
--rw-r--r--   0 lhh       (3368) lhh       (3368)     2909 2024-03-08 19:31:58.000000 jirate-0.8.2/README.md
-drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-03-26 14:52:34.451787 jirate-0.8.2/jirate/
--rw-r--r--   0 lhh       (3368) lhh       (3368)       42 2024-03-26 14:52:16.000000 jirate-0.8.2/jirate/__init__.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)     2493 2023-09-14 15:10:20.000000 jirate-0.8.2/jirate/args.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)    22297 2023-09-14 15:10:20.000000 jirate-0.8.2/jirate/board.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)    21651 2023-09-14 15:10:20.000000 jirate-0.8.2/jirate/cli.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)      465 2023-09-18 21:35:46.000000 jirate-0.8.2/jirate/config.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)     9390 2024-01-25 18:46:21.000000 jirate-0.8.2/jirate/decor.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)    32183 2024-03-26 14:52:16.000000 jirate-0.8.2/jirate/jboard.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)    44434 2024-03-08 19:43:27.000000 jirate-0.8.2/jirate/jira_cli.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)    14909 2024-03-08 19:31:58.000000 jirate-0.8.2/jirate/jira_fields.py
--rw-r--r--   0 lhh       (3368) lhh       (3368)     4599 2024-02-08 22:08:42.000000 jirate-0.8.2/jirate/jira_input.py
-drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-03-26 14:52:34.451787 jirate-0.8.2/jirate.egg-info/
--rw-r--r--   0 lhh       (3368) lhh       (3368)     1606 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/PKG-INFO
--rw-r--r--   0 lhh       (3368) lhh       (3368)      388 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/SOURCES.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)        1 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/dependency_links.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)       74 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/entry_points.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)      139 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/requires.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)        7 2024-03-26 14:52:34.000000 jirate-0.8.2/jirate.egg-info/top_level.txt
--rw-r--r--   0 lhh       (3368) lhh       (3368)       38 2024-03-26 14:52:34.452787 jirate-0.8.2/setup.cfg
--rw-r--r--   0 lhh       (3368) lhh       (3368)     2783 2024-01-25 18:46:21.000000 jirate-0.8.2/setup.py
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.682371 jirate-0.8.3/
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.679371 jirate-0.8.3/.github/
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.680372 jirate-0.8.3/.github/workflows/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1420 2024-04-17 16:22:13.000000 jirate-0.8.3/.github/workflows/python-package.yml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      203 2024-01-25 20:49:14.000000 jirate-0.8.3/Containerfile
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1352 2022-12-21 18:20:21.000000 jirate-0.8.3/LICENSE.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      365 2024-01-25 20:49:14.000000 jirate-0.8.3/Makefile
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1569 2024-04-18 14:29:37.682371 jirate-0.8.3/PKG-INFO
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     6543 2024-04-17 17:01:20.000000 jirate-0.8.3/README.md
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1021 2024-02-05 13:16:54.000000 jirate-0.8.3/TODO
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.680372 jirate-0.8.3/contrib/
+-rwxr-xr-x   0 lhh       (3368) lhh       (3368)      718 2024-01-17 18:02:50.000000 jirate-0.8.3/contrib/checklist2jira
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1313 2024-02-07 18:53:43.000000 jirate-0.8.3/contrib/example-template.yaml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1341 2024-04-17 16:44:13.000000 jirate-0.8.3/contrib/jirate.json
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.681372 jirate-0.8.3/jirate/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)       42 2024-04-18 14:29:01.000000 jirate-0.8.3/jirate/__init__.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     2493 2024-01-17 18:02:50.000000 jirate-0.8.3/jirate/args.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    22297 2024-01-17 18:02:50.000000 jirate-0.8.3/jirate/board.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    21651 2024-01-17 18:02:50.000000 jirate-0.8.3/jirate/cli.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      465 2024-01-17 18:02:50.000000 jirate-0.8.3/jirate/config.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     9390 2024-01-25 16:03:01.000000 jirate-0.8.3/jirate/decor.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    32183 2024-04-16 18:02:45.000000 jirate-0.8.3/jirate/jboard.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    44434 2024-04-17 16:22:12.000000 jirate-0.8.3/jirate/jira_cli.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    14909 2024-03-08 19:14:59.000000 jirate-0.8.3/jirate/jira_fields.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     4599 2024-02-13 16:06:37.000000 jirate-0.8.3/jirate/jira_input.py
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.681372 jirate-0.8.3/jirate/schemas/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      764 2024-02-07 18:53:43.000000 jirate-0.8.3/jirate/schemas/issue.yaml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      558 2024-02-07 18:53:43.000000 jirate-0.8.3/jirate/schemas/subtask.yaml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      444 2024-02-05 13:05:08.000000 jirate-0.8.3/jirate/schemas/template.yaml
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.682371 jirate-0.8.3/jirate/tests/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    48144 2024-03-08 19:14:59.000000 jirate-0.8.3/jirate/tests/__init__.py
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.682371 jirate-0.8.3/jirate/tests/templates/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1212 2024-02-07 18:53:43.000000 jirate-0.8.3/jirate/tests/templates/bad-template.yaml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1312 2024-02-07 18:53:43.000000 jirate-0.8.3/jirate/tests/templates/good-template.yaml
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1386 2024-01-25 16:03:01.000000 jirate-0.8.3/jirate/tests/test_decor.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1553 2024-01-17 18:02:50.000000 jirate-0.8.3/jirate/tests/test_fields.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     3796 2024-02-08 21:50:58.000000 jirate-0.8.3/jirate/tests/test_input.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)    11963 2024-03-08 19:14:59.000000 jirate-0.8.3/jirate/tests/test_jira_cli.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     4496 2024-02-13 16:06:37.000000 jirate-0.8.3/jirate/tests/test_jirate.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     5634 2024-03-08 19:14:59.000000 jirate-0.8.3/jirate/tests/test_render.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      545 2024-01-24 18:22:46.000000 jirate-0.8.3/jirate/tests/test_schemas.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      178 2024-01-25 20:35:06.000000 jirate-0.8.3/jirate-c.in
+drwxr-xr-x   0 lhh       (3368) lhh       (3368)        0 2024-04-18 14:29:37.681372 jirate-0.8.3/jirate.egg-info/
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     1569 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/PKG-INFO
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      974 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/SOURCES.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)        1 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/dependency_links.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)       73 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/entry_points.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      139 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/requires.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)        7 2024-04-18 14:29:37.000000 jirate-0.8.3/jirate.egg-info/top_level.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)      139 2024-04-17 16:22:13.000000 jirate-0.8.3/requirements.txt
+-rw-r--r--   0 lhh       (3368) lhh       (3368)       38 2024-04-18 14:29:37.682371 jirate-0.8.3/setup.cfg
+-rw-r--r--   0 lhh       (3368) lhh       (3368)     2783 2024-04-18 13:59:10.000000 jirate-0.8.3/setup.py
+-rw-r--r--   0 lhh       (3368) lhh       (3368)        7 2024-01-24 18:22:46.000000 jirate-0.8.3/test-requirements.txt
```

### Comparing `jirate-0.8.2/LICENSE.txt` & `jirate-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/PKG-INFO` & `jirate-0.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: jirate
-Version: 0.8.2
-Summary: UNKNOWN
+Version: 0.8.3
 Home-page: http://github.com/lhh/jirate
 Author: Red Hat
 Author-email: lhh@redhat.com
 Maintainer: Lon Hohberger
 Maintainer-email: lon@metamorphism.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
@@ -51,9 +49,7 @@
 
     https://docs.atlassian.com/software/jira/docs/api/REST/latest/
 
 Documentation for the Trello API at:
 
     https://developers.trello.com/reference/
 
-
-
```

### Comparing `jirate-0.8.2/jirate/args.py` & `jirate-0.8.3/jirate/args.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/board.py` & `jirate-0.8.3/jirate/board.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/cli.py` & `jirate-0.8.3/jirate/cli.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/decor.py` & `jirate-0.8.3/jirate/decor.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/jboard.py` & `jirate-0.8.3/jirate/jboard.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/jira_cli.py` & `jirate-0.8.3/jirate/jira_cli.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/jira_fields.py` & `jirate-0.8.3/jirate/jira_fields.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate/jira_input.py` & `jirate-0.8.3/jirate/jira_input.py`

 * *Files identical despite different names*

### Comparing `jirate-0.8.2/jirate.egg-info/PKG-INFO` & `jirate-0.8.3/jirate.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: jirate
-Version: 0.8.2
-Summary: UNKNOWN
+Version: 0.8.3
 Home-page: http://github.com/lhh/jirate
 Author: Red Hat
 Author-email: lhh@redhat.com
 Maintainer: Lon Hohberger
 Maintainer-email: lon@metamorphism.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
@@ -51,9 +49,7 @@
 
     https://docs.atlassian.com/software/jira/docs/api/REST/latest/
 
 Documentation for the Trello API at:
 
     https://developers.trello.com/reference/
 
-
-
```

### Comparing `jirate-0.8.2/setup.py` & `jirate-0.8.3/setup.py`

 * *Files identical despite different names*

