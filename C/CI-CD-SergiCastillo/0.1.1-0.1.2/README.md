# Comparing `tmp/CI-CD-SergiCastillo-0.1.1.tar.gz` & `tmp/CI-CD-SergiCastillo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.1.tar", last modified: Thu Apr 18 18:01:07 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.2.tar", last modified: Thu Apr 18 18:04:25 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.1.1.tar` & `CI-CD-SergiCastillo-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:01:07.385658 CI-CD-SergiCastillo-0.1.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:01:07.385658 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 18:01:07.000000 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 18:01:07.000000 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 18:01:07.000000 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 18:01:07.000000 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 18:01:07.000000 CI-CD-SergiCastillo-0.1.1/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 18:01:07.385658 CI-CD-SergiCastillo-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 18:00:02.000000 CI-CD-SergiCastillo-0.1.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:01:07.385658 CI-CD-SergiCastillo-0.1.1/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:00:56.000000 CI-CD-SergiCastillo-0.1.1/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 18:00:02.000000 CI-CD-SergiCastillo-0.1.1/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 18:01:07.385658 CI-CD-SergiCastillo-0.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 18:00:02.000000 CI-CD-SergiCastillo-0.1.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:04:25.631396 CI-CD-SergiCastillo-0.1.2/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:04:25.631396 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 18:04:25.000000 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 18:04:25.000000 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 18:04:25.000000 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 18:04:25.000000 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 18:04:25.000000 CI-CD-SergiCastillo-0.1.2/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 18:04:25.631396 CI-CD-SergiCastillo-0.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 18:03:23.000000 CI-CD-SergiCastillo-0.1.2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:04:25.631396 CI-CD-SergiCastillo-0.1.2/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 18:04:13.000000 CI-CD-SergiCastillo-0.1.2/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 18:03:23.000000 CI-CD-SergiCastillo-0.1.2/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 18:04:25.631396 CI-CD-SergiCastillo-0.1.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 18:03:23.000000 CI-CD-SergiCastillo-0.1.2/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.1.1/app/app.py` & `CI-CD-SergiCastillo-0.1.2/app/app.py`

 * *Files identical despite different names*
