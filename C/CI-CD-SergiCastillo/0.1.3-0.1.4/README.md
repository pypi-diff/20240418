# Comparing `tmp/CI-CD-SergiCastillo-0.1.3.tar.gz` & `tmp/CI-CD-SergiCastillo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.3.tar", last modified: Thu Apr 18 19:09:32 2024, max compression
+gzip compressed data, was "dist/CI-CD-SergiCastillo-0.1.4.tar", last modified: Thu Apr 18 20:08:21 2024, max compression
```

## Comparing `CI-CD-SergiCastillo-0.1.3.tar` & `CI-CD-SergiCastillo-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 19:09:32.013970 CI-CD-SergiCastillo-0.1.3/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 19:09:32.013970 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 19:09:31.000000 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 19:09:32.000000 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 19:09:31.000000 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 19:09:31.000000 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 19:09:31.000000 CI-CD-SergiCastillo-0.1.3/CI_CD_SergiCastillo.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 19:09:32.013970 CI-CD-SergiCastillo-0.1.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 19:08:20.000000 CI-CD-SergiCastillo-0.1.3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 19:09:32.013970 CI-CD-SergiCastillo-0.1.3/app/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 19:09:20.000000 CI-CD-SergiCastillo-0.1.3/app/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 19:08:20.000000 CI-CD-SergiCastillo-0.1.3/app/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 19:09:32.013970 CI-CD-SergiCastillo-0.1.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 19:08:20.000000 CI-CD-SergiCastillo-0.1.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:08:21.488221 CI-CD-SergiCastillo-0.1.4/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:08:21.488221 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:08:21.000000 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      259 2024-04-18 20:08:21.000000 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-18 20:08:21.000000 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2024-04-18 20:08:21.000000 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2024-04-18 20:08:21.000000 CI-CD-SergiCastillo-0.1.4/CI_CD_SergiCastillo.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2024-04-18 20:08:21.488221 CI-CD-SergiCastillo-0.1.4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-04-18 20:07:15.000000 CI-CD-SergiCastillo-0.1.4/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:08:21.488221 CI-CD-SergiCastillo-0.1.4/app/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-18 20:08:07.000000 CI-CD-SergiCastillo-0.1.4/app/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3678 2024-04-18 20:07:15.000000 CI-CD-SergiCastillo-0.1.4/app/app.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-04-18 20:08:21.492221 CI-CD-SergiCastillo-0.1.4/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2024-04-18 20:07:15.000000 CI-CD-SergiCastillo-0.1.4/setup.py
```

### Comparing `CI-CD-SergiCastillo-0.1.3/app/app.py` & `CI-CD-SergiCastillo-0.1.4/app/app.py`

 * *Files identical despite different names*

