# Comparing `tmp/firebase_functions-0.4.0.tar.gz` & `tmp/firebase_functions-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_functions-0.4.0.tar", last modified: Tue Apr 16 15:19:01 2024, max compression
+gzip compressed data, was "firebase_functions-0.4.1.tar", last modified: Thu Apr 18 18:03:02 2024, max compression
```

## Comparing `firebase_functions-0.4.0.tar` & `firebase_functions-0.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.481245 firebase_functions-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.481245 firebase_functions-0.4.0/src/firebase_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/app_distribution_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/billing_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/crashlytics_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts/performance_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/db_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21791 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/https_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    38950 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions/private/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/_alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/private/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/src/firebase_functions/test_lab_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.485245 firebase_functions-0.4.0/src/firebase_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 15:19:01.000000 firebase_functions-0.4.0/src/firebase_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:19:01.489246 firebase_functions-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_https_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_test_lab_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-16 15:18:28.000000 firebase_functions-0.4.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.770367 firebase_functions-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 18:03:02.770367 firebase_functions-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:03:02.770367 firebase_functions-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.758367 firebase_functions-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.762367 firebase_functions-0.4.1/src/firebase_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.766367 firebase_functions-0.4.1/src/firebase_functions/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts/app_distribution_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts/billing_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts/crashlytics_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts/performance_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/db_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21795 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38950 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.766367 firebase_functions-0.4.1/src/firebase_functions/private/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/_alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/private/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/src/firebase_functions/test_lab_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.762367 firebase_functions-0.4.1/src/firebase_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-18 18:03:02.000000 firebase_functions-0.4.1/src/firebase_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-18 18:03:02.000000 firebase_functions-0.4.1/src/firebase_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:03:02.000000 firebase_functions-0.4.1/src/firebase_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-18 18:03:02.000000 firebase_functions-0.4.1/src/firebase_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 18:03:02.000000 firebase_functions-0.4.1/src/firebase_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:03:02.766367 firebase_functions-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_test_lab_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-18 18:02:34.000000 firebase_functions-0.4.1/tests/test_util.py
```

### Comparing `firebase_functions-0.4.0/LICENSE` & `firebase_functions-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/PKG-INFO` & `firebase_functions-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase_functions
-Version: 0.4.0
+Version: 0.4.1
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.4.0/README.md` & `firebase_functions-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/setup.py` & `firebase_functions-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/__init__.py` & `firebase_functions-0.4.1/src/firebase_functions/private/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,11 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Firebase Functions for Python.
+Firebase Functions for Python - Private/Internals
 """
-
-__version__ = "0.4.0"
```

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts/__init__.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts/app_distribution_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts/app_distribution_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts/billing_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts/billing_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts/crashlytics_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts/crashlytics_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts/performance_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts/performance_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/alerts_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/core.py` & `firebase_functions-0.4.1/src/firebase_functions/core.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/db_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/db_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/eventarc_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/firestore_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/firestore_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,16 +130,14 @@
                         f"'{actual_type}' and content type '{content_type}'.")
 
     event_location = event_attributes["location"]
     event_project = event_attributes["project"]
     event_namespace = event_attributes["namespace"]
     event_document = event_attributes["document"]
     event_database = event_attributes["database"]
-    event_auth_type = event_attributes["authtype"]
-    event_auth_id = event_attributes["authid"]
 
     time = event_attributes["time"]
     event_time = _util.timestamp_conversion(time)
 
     if _DEFAULT_APP_NAME not in _apps:
         initialize_app()
     app = get_app()
@@ -204,14 +202,16 @@
         subject=event_attributes["subject"],
         params=params,
     )
 
     func = _core._with_init(func)
 
     if event_type.endswith(".withAuthContext"):
+        event_auth_type = event_attributes["authtype"]
+        event_auth_id = event_attributes["authid"]
         database_event_with_auth_context = AuthEvent(**vars(database_event),
                                                      auth_type=event_auth_type,
                                                      auth_id=event_auth_id)
         func(database_event_with_auth_context)
     else:
         # mypy cannot infer that the event type is correct, hence the cast
         _typing.cast(_C1 | _C2, func)(database_event)
@@ -266,15 +266,15 @@
 
 
 @_util.copy_func_kwargs(FirestoreOptions)
 def on_document_written_with_auth_context(**kwargs
                                          ) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler that triggers when a document is created, updated, or deleted in Firestore.
-    This trigger will also provide the authentication context of the principal who triggered 
+    This trigger will also provide the authentication context of the principal who triggered
     the event.
 
     Example:
 
     .. code-block:: python
 
       @on_document_written_with_auth_context(document="*")
@@ -365,15 +365,15 @@
 
 
 @_util.copy_func_kwargs(FirestoreOptions)
 def on_document_updated_with_auth_context(**kwargs
                                          ) -> _typing.Callable[[_C1], _C1]:
     """
     Event handler that triggers when a document is updated in Firestore.
-    This trigger will also provide the authentication context of the principal who triggered 
+    This trigger will also provide the authentication context of the principal who triggered
     the event.
 
     Example:
 
     .. code-block:: python
 
       @on_document_updated_with_auth_context(document="*")
@@ -464,15 +464,15 @@
 
 
 @_util.copy_func_kwargs(FirestoreOptions)
 def on_document_created_with_auth_context(**kwargs
                                          ) -> _typing.Callable[[_C2], _C2]:
     """
     Event handler that triggers when a document is created in Firestore.
-    This trigger will also provide the authentication context of the principal who triggered 
+    This trigger will also provide the authentication context of the principal who triggered
     the event.
 
     Example:
 
     .. code-block:: python
 
         @on_document_created_with_auth_context(document="*")
@@ -563,15 +563,15 @@
 
 
 @_util.copy_func_kwargs(FirestoreOptions)
 def on_document_deleted_with_auth_context(**kwargs
                                          ) -> _typing.Callable[[_C2], _C2]:
     """
     Event handler that triggers when a document is deleted in Firestore.
-    This trigger will also provide the authentication context of the principal who triggered 
+    This trigger will also provide the authentication context of the principal who triggered
     the event.
 
     Example:
 
     .. code-block:: python
 
       @on_document_deleted_with_auth_context(document="*")
```

### Comparing `firebase_functions-0.4.0/src/firebase_functions/https_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/https_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/identity_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/logger.py` & `firebase_functions-0.4.1/src/firebase_functions/logger.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/options.py` & `firebase_functions-0.4.1/src/firebase_functions/options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/params.py` & `firebase_functions-0.4.1/src/firebase_functions/params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/_alerts_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/private/_alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/_identity_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/private/_identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/manifest.py` & `firebase_functions-0.4.1/src/firebase_functions/private/manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/path_pattern.py` & `firebase_functions-0.4.1/src/firebase_functions/private/path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/serving.py` & `firebase_functions-0.4.1/src/firebase_functions/private/serving.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/token_verifier.py` & `firebase_functions-0.4.1/src/firebase_functions/private/token_verifier.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/private/util.py` & `firebase_functions-0.4.1/src/firebase_functions/private/util.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/pubsub_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/remote_config_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/scheduler_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/storage_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/storage_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/tasks_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions/test_lab_fn.py` & `firebase_functions-0.4.1/src/firebase_functions/test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/src/firebase_functions.egg-info/PKG-INFO` & `firebase_functions-0.4.1/src/firebase_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase-functions
-Version: 0.4.0
+Version: 0.4.1
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.4.0/src/firebase_functions.egg-info/SOURCES.txt` & `firebase_functions-0.4.1/src/firebase_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_db.py` & `firebase_functions-0.4.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_eventarc_fn.py` & `firebase_functions-0.4.1/tests/test_eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_firestore_fn.py` & `firebase_functions-0.4.1/tests/test_firestore_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_https_fn.py` & `firebase_functions-0.4.1/tests/test_https_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_identity_fn.py` & `firebase_functions-0.4.1/tests/test_identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_logger.py` & `firebase_functions-0.4.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_manifest.py` & `firebase_functions-0.4.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_options.py` & `firebase_functions-0.4.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_params.py` & `firebase_functions-0.4.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_path_pattern.py` & `firebase_functions-0.4.1/tests/test_path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_pubsub_fn.py` & `firebase_functions-0.4.1/tests/test_pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_remote_config_fn.py` & `firebase_functions-0.4.1/tests/test_remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_scheduler_fn.py` & `firebase_functions-0.4.1/tests/test_scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_storage_fn.py` & `firebase_functions-0.4.1/tests/test_storage_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_tasks_fn.py` & `firebase_functions-0.4.1/tests/test_tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_test_lab_fn.py` & `firebase_functions-0.4.1/tests/test_test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.4.0/tests/test_util.py` & `firebase_functions-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

