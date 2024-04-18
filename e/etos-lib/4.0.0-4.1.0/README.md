# Comparing `tmp/etos_lib-4.0.0.tar.gz` & `tmp/etos_lib-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_lib-4.0.0.tar", last modified: Tue Nov  7 11:11:06 2023, max compression
+gzip compressed data, was "etos_lib-4.1.0.tar", last modified: Thu Apr 18 12:51:13 2024, max compression
```

## Comparing `etos_lib-4.0.0.tar` & `etos_lib-4.1.0.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.724103 etos_lib-4.0.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-03-09 08:23:58.000000 etos_lib-4.0.0/.coveragerc
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.716103 etos_lib-4.0.0/.github/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/.github/workflows/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_lib-4.0.0/.github/workflows/main.yml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-02 11:08:37.000000 etos_lib-4.0.0/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_lib-4.0.0/AUTHORS.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_lib-4.0.0/CODEOWNERS
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_lib-4.0.0/LICENSE.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-11-07 11:11:06.724103 etos_lib-4.0.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-03-09 08:23:58.000000 etos_lib-4.0.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-05-31 11:37:56.000000 etos_lib-4.0.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_lib-4.0.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-10-19 09:56:44.000000 etos_lib-4.0.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1413 2023-11-07 11:11:06.724103 etos_lib-4.0.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-03-09 08:23:58.000000 etos_lib-4.0.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/src/etos_lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4915 2023-10-19 09:56:44.000000 etos_lib-4.0.0/src/etos_lib/etos.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/src/etos_lib/graphql/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2595 2023-10-19 09:56:44.000000 etos_lib-4.0.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/src/etos_lib/kubernetes/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3103 2023-10-19 09:56:44.000000 etos_lib-4.0.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3288 2023-10-19 09:56:44.000000 etos_lib-4.0.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.724103 etos_lib-4.0.0/src/etos_lib/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-02 11:08:37.000000 etos_lib-4.0.0/src/etos_lib/lib/config.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-06-02 12:36:16.000000 etos_lib-4.0.0/src/etos_lib/lib/database.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5179 2023-10-19 09:56:44.000000 etos_lib-4.0.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-05-31 11:37:56.000000 etos_lib-4.0.0/src/etos_lib/lib/events.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-05-31 11:37:56.000000 etos_lib-4.0.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3312 2023-10-19 10:54:16.000000 etos_lib-4.0.0/src/etos_lib/lib/http.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-06-09 07:27:46.000000 etos_lib-4.0.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.724103 etos_lib-4.0.0/src/etos_lib/logging/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-05-26 11:19:01.000000 etos_lib-4.0.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-03-09 08:23:58.000000 etos_lib-4.0.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-02 11:08:37.000000 etos_lib-4.0.0/src/etos_lib/logging/log_publisher.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     6850 2023-10-19 09:56:46.000000 etos_lib-4.0.0/src/etos_lib/logging/logger.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-02 11:08:37.000000 etos_lib-4.0.0/src/etos_lib/logging/rabbitmq_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.720103 etos_lib-4.0.0/src/etos_lib.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-11-07 11:11:06.000000 etos_lib-4.0.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1316 2023-11-07 11:11:06.000000 etos_lib-4.0.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-11-07 11:11:06.000000 etos_lib-4.0.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-02 13:03:49.000000 etos_lib-4.0.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-11-07 11:11:06.000000 etos_lib-4.0.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-11-07 11:11:06.000000 etos_lib-4.0.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-03-09 08:23:58.000000 etos_lib-4.0.0/test-requirements.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-11-07 11:11:06.724103 etos_lib-4.0.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-03-09 08:23:58.000000 etos_lib-4.0.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-03-09 08:23:58.000000 etos_lib-4.0.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-03-09 08:23:58.000000 etos_lib-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.174860 etos_lib-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-18 12:51:07.000000 etos_lib-4.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.162860 etos_lib-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.166860 etos_lib-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-18 12:51:07.000000 etos_lib-4.1.0/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 12:51:07.000000 etos_lib-4.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 12:51:07.000000 etos_lib-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 12:51:07.000000 etos_lib-4.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:51:07.000000 etos_lib-4.1.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-18 12:51:07.000000 etos_lib-4.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-18 12:51:13.174860 etos_lib-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 12:51:07.000000 etos_lib-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.166860 etos_lib-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.166860 etos_lib-4.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 12:51:07.000000 etos_lib-4.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 12:51:07.000000 etos_lib-4.1.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 12:51:07.000000 etos_lib-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 12:51:13.174860 etos_lib-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 12:51:07.000000 etos_lib-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.162860 etos_lib-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.166860 etos_lib-4.1.0/src/etos_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.170860 etos_lib-4.1.0/src/etos_lib/eiffel/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/eiffel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/eiffel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/eiffel/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/eiffel/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/etos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.170860 etos_lib-4.1.0/src/etos_lib/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.170860 etos_lib-4.1.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.170860 etos_lib-4.1.0/src/etos_lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10922 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.174860 etos_lib-4.1.0/src/etos_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/log_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-18 12:51:07.000000 etos_lib-4.1.0/src/etos_lib/logging/rabbitmq_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.174860 etos_lib-4.1.0/src/etos_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 12:51:13.000000 etos_lib-4.1.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-18 12:51:07.000000 etos_lib-4.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:51:13.174860 etos_lib-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 12:51:07.000000 etos_lib-4.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 12:51:07.000000 etos_lib-4.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-18 12:51:07.000000 etos_lib-4.1.0/tox.ini
```

### Comparing `etos_lib-4.0.0/.coveragerc` & `etos_lib-4.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/.github/workflows/main.yml` & `etos_lib-4.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/.gitignore` & `etos_lib-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/LICENSE.txt` & `etos_lib-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/README.rst` & `etos_lib-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/docs/Makefile` & `etos_lib-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/docs/conf.py` & `etos_lib-4.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 """Sphinx configuration."""
 
 import os
 import sys
 import inspect
 import shutil
 
-__location__ = os.path.join(
-    os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe()))
-)
+__location__ = os.path.join(os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe())))
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.join(__location__, "../src"))
 
 # -- Run sphinx-apidoc ------------------------------------------------------
```

### Comparing `etos_lib-4.0.0/setup.cfg` & `etos_lib-4.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 install_requires = 
 	gql[requests]~=3.4
 	redis~=4.5
 	eiffellib[rabbitmq]~=2.4
 	requests~=2.31
 	kubernetes~=26.1
 	pyyaml~=6.0
+	opentelemetry-api~=1.21
+	opentelemetry-semantic-conventions~=0.42b0
 python_requires = >=3.4
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `etos_lib-4.0.0/setup.py` & `etos_lib-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/__init__.py` & `etos_lib-4.1.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/etos.py` & `etos_lib-4.1.0/src/etos_lib/etos.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS Library module."""
-from eiffellib.subscribers import RabbitMQSubscriber
-from eiffellib.publishers import RabbitMQPublisher
+from .eiffel.publisher import TracingRabbitMQPublisher as RabbitMQPublisher
+from .eiffel.subscriber import TracingRabbitMQSubscriber as RabbitMQSubscriber
+from .graphql.query_handler import GraphQLQueryHandler
 from .lib.config import Config
-from .lib.events import Events
-from .lib.monitor import Monitor
-from .lib.utils import Utils
-from .lib.http import Http
-from .lib.debug import Debug
-from .lib.feature_flags import FeatureFlags
 from .lib.database import Database
+from .lib.debug import Debug
+from .lib.events import Events
 from .lib.exceptions import (
     PublisherConfigurationMissing,
-    SubscriberConfigurationMissing,
     PublisherNotStarted,
+    SubscriberConfigurationMissing,
 )
-from .graphql.query_handler import GraphQLQueryHandler
+from .lib.feature_flags import FeatureFlags
+from .lib.http import Http
+from .lib.monitor import Monitor
+from .lib.utils import Utils
 
 
 class ETOS:  # pylint: disable=too-many-instance-attributes
     """ETOS Library."""
 
     publisher = None
     subscriber = None
```

### Comparing `etos_lib-4.0.0/src/etos_lib/graphql/__init__.py` & `etos_lib-4.1.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-4.1.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-4.1.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/kubernetes/base.py` & `etos_lib-4.1.0/src/etos_lib/kubernetes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 class Kubernetes:
     """Base kubernetes library."""
 
     __batch = None
     __core = None
     __apps = None
 
-    def __init__(
-        self, namespace=os.getenv("ETOS_NAMESPACE"), context=None, in_cluster=True
-    ):
+    def __init__(self, namespace=os.getenv("ETOS_NAMESPACE"), context=None, in_cluster=True):
         """Initialize kubernetes library and load kubernetes configuration.
 
         :param namespace: Which namespace to operate in.
         :type namespace: str
         :param context: From which Kubernetes context should we load config from.
                         This is only relevant when running locally (in_cluster=False).
         :type context: str
```

### Comparing `etos_lib-4.0.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-4.1.0/src/etos_lib/kubernetes/jobs.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,17 +40,15 @@
                         Default: 5 minutes.
         :type timeout: int
         :return: Job response.
         :rtype: dict
         """
         timeout = time.time() + timeout
         while time.time() < timeout:
-            response = self.batch_v1.read_namespaced_job_status(
-                job_name, self.namespace
-            )
+            response = self.batch_v1.read_namespaced_job_status(job_name, self.namespace)
             status = response.status
             if status.active is not None:
                 print(f"Started at: {status.start_time}")
                 break
             time.sleep(1)
         return response
 
@@ -64,17 +62,15 @@
         :type timeout: int
         :return: Result of the job.
         :rtype: bool
         """
         timeout = time.time() + timeout
         result = False
         while time.time() < timeout:
-            response = self.batch_v1.read_namespaced_job_status(
-                job_name, self.namespace
-            )
+            response = self.batch_v1.read_namespaced_job_status(job_name, self.namespace)
             status = response.status
             # pylint:disable=no-else-break
             if status.failed is not None:
                 print(f"Finished, but failed: {status}")
                 result = False
                 break
             elif status.succeeded is not None:
```

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/__init__.py` & `etos_lib-4.1.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/config.py` & `etos_lib-4.1.0/src/etos_lib/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/database.py` & `etos_lib-4.1.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/debug.py` & `etos_lib-4.1.0/src/etos_lib/lib/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 from pathlib import Path
 from collections import deque
 
 
 class Debug:
     """Debug flags for ETOS."""
 
-    __events_published = deque(
-        maxlen=int(os.getenv("ETOS_PUBLISHED_EVENT_HISTORY_SIZE", "100"))
-    )
-    __events_received = deque(
-        maxlen=int(os.getenv("ETOS_RECEIVED_EVENT_HISTORY_SIZE", "100"))
-    )
+    __events_published = deque(maxlen=int(os.getenv("ETOS_PUBLISHED_EVENT_HISTORY_SIZE", "100")))
+    __events_received = deque(maxlen=int(os.getenv("ETOS_RECEIVED_EVENT_HISTORY_SIZE", "100")))
 
     @property
     def default_log_path(self):
         """Log path."""
         path = os.getenv("ETOS_LOG_PATH")
         if path is None:
             path = Path.home().joinpath("logs/log.json")
```

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/events.py` & `etos_lib-4.1.0/src/etos_lib/lib/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,15 @@
         :type optional: dict
         """
         if (
             optional.get("image") is None
             and optional.get("host") is None
             and optional.get("uri") is None
         ):
-            raise ValueError(
-                "At least one of 'host', 'image' or 'uri' must be provided"
-            )
+            raise ValueError("At least one of 'host', 'image' or 'uri' must be provided")
         links = links if links is not None else {}
         data = {"name": name}
         data.update(**optional)
         return self.send(EiffelEnvironmentDefinedEvent(), links, data)
 
     def send_test_suite_started(self, name, links=None, **optional):
         """Publish a test suite started event.
@@ -200,17 +198,15 @@
         :type optional: dict
         """
         links = links if links is not None else {}
         links.update({"TEST_SUITE_EXECUTION": test_suite})
         data = optional
         return self.send(EiffelTestSuiteFinishedEvent(), links, data)
 
-    def send_announcement_published(
-        self, heading, body, severity, links=None, **optional
-    ):
+    def send_announcement_published(self, heading, body, severity, links=None, **optional):
         """Publish an announcement event.
 
         https://github.com/eiffel-community/eiffel/blob/master/eiffel-vocabulary/EiffelAnnouncementPublishedEvent.md
 
         :param heading: Heading for the announcement.
         :type heading: str
         :param body: Body for the announcement.
@@ -238,17 +234,15 @@
         :type selection_strategy: dict
         :param links: Optional links to add to event.
         :type links: dict
         :param optional: Dictionary of optional data to add.
         :type optional: dict
         """
         if optional.get("batches") is None and optional.get("batchesUri") is None:
-            raise ValueError(
-                "At least one of 'batches' or 'batchesUri' must be provided"
-            )
+            raise ValueError("At least one of 'batches' or 'batchesUri' must be provided")
         links = links if links is not None else {}
         data = {"selectionStrategy": selection_strategy}
         data.update(**optional)
         return self.send(EiffelTestExecutionRecipeCollectionCreatedEvent(), links, data)
 
     def send_confidence_level_modified(self, name, value, links=None, **optional):
         """Publish a confidence level event.
@@ -339,17 +333,15 @@
         :type optional: dict
         """
         links = links if links is not None else {}
         data = {"identity": identity}
         data.update(**optional)
         return self.send(EiffelArtifactCreatedEvent(), links, data)
 
-    def send_artifact_published_event(
-        self, locations, artifact, links=None, **optional
-    ):
+    def send_artifact_published_event(self, locations, artifact, links=None, **optional):
         """Publish an artifact created event.
 
         https://github.com/eiffel-community/eiffel/blob/master/eiffel-vocabulary/EiffelArtifactPublishedEvent.md
 
         :param locations: Locations for this artifact.
         :type locations: list
         :param artifact: Artifact created link.
```

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/exceptions.py` & `etos_lib-4.1.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-4.1.0/src/etos_lib/lib/feature_flags.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/http.py` & `etos_lib-4.1.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/monitor.py` & `etos_lib-4.1.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/lib/utils.py` & `etos_lib-4.1.0/src/etos_lib/lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,17 +230,15 @@
                             Set this to False on commands that we're
                             not in control of.
         :type wait_output: boolean
         :return: Result and output from command.
         :rtype: tuple
         """
         out = []
-        for _, line in self.iterable_call(
-            cmd, shell, env, executable, output, wait_output
-        ):
+        for _, line in self.iterable_call(cmd, shell, env, executable, output, wait_output):
             if isinstance(line, str):
                 out.append(line)
             else:
                 success = line
                 break
         return success, out
```

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/__init__.py` & `etos_lib-4.1.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/filter.py` & `etos_lib-4.1.0/src/etos_lib/logging/filter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/formatter.py` & `etos_lib-4.1.0/src/etos_lib/logging/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,10 +94,8 @@
             NotImplementedError: If the `datefmt` parameter is not None.
         """
         if datefmt is not None:
             raise NotImplementedError("Only default time format is supported.")
         # Make Logstash's @timestamp parser happy by including a "T"
         # between the date and the time. Append 'Z' to make it clear
         # that the timestamp is UTC.
-        return datetime.datetime.utcfromtimestamp(record.created).strftime(
-            "%Y-%m-%dT%H:%M:%S.%fZ"
-        )
+        return datetime.datetime.utcfromtimestamp(record.created).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
```

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/log_publisher.py` & `etos_lib-4.1.0/src/etos_lib/logging/log_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 
         This method differs slightly from its parent in that it takes the routing_key as input.
         """
         if block:
             self.wait_start()
             while self._channel is None or not self._channel.is_open:
                 time.sleep(0.1)
-        properties = pika.BasicProperties(
-            content_type="application/json", delivery_mode=2
-        )
+        properties = pika.BasicProperties(content_type="application/json", delivery_mode=2)
         if not isinstance(event, str):
             event = json.dumps(event)
 
         with self._lock:
             try:
                 self._channel.basic_publish(
                     self.exchange,
```

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/logger.py` & `etos_lib-4.1.0/src/etos_lib/logging/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,17 +132,15 @@
 
     # These have to be removed as they create a loop.
     # They will still work with the other handlers.
     logging.getLogger("pika").propagate = False
     logging.getLogger("eiffellib.publishers.rabbitmq_publisher").propagate = False
     logging.getLogger("base_rabbitmq").propagate = False
 
-    rabbitmq = RabbitMQLogPublisher(
-        **Config().etos_rabbitmq_publisher_data(), routing_key=None
-    )
+    rabbitmq = RabbitMQLogPublisher(**Config().etos_rabbitmq_publisher_data(), routing_key=None)
     if Debug().enable_sending_logs:
         rabbitmq.start()
         atexit.register(close_rabbit, rabbitmq)
 
     rabbit_handler = RabbitMQHandler(rabbitmq)
     rabbit_handler.setFormatter(EtosLogFormatter())
     rabbit_handler.setLevel(loglevel)
```

### Comparing `etos_lib-4.0.0/src/etos_lib/logging/rabbitmq_handler.py` & `etos_lib-4.1.0/src/etos_lib/logging/rabbitmq_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-4.0.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-4.1.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 .coveragerc
 .gitignore
 AUTHORS.rst
 CODEOWNERS
 LICENSE.txt
 README.rst
+pylintrc
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
+.github/workflows/build-publish.yml
 .github/workflows/main.yml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/license.rst
@@ -23,14 +25,18 @@
 src/etos_lib/etos.py
 src/etos_lib.egg-info/PKG-INFO
 src/etos_lib.egg-info/SOURCES.txt
 src/etos_lib.egg-info/dependency_links.txt
 src/etos_lib.egg-info/not-zip-safe
 src/etos_lib.egg-info/requires.txt
 src/etos_lib.egg-info/top_level.txt
+src/etos_lib/eiffel/__init__.py
+src/etos_lib/eiffel/common.py
+src/etos_lib/eiffel/publisher.py
+src/etos_lib/eiffel/subscriber.py
 src/etos_lib/graphql/__init__.py
 src/etos_lib/graphql/query_handler.py
 src/etos_lib/kubernetes/__init__.py
 src/etos_lib/kubernetes/base.py
 src/etos_lib/kubernetes/jobs.py
 src/etos_lib/lib/__init__.py
 src/etos_lib/lib/config.py
```

### Comparing `etos_lib-4.0.0/tests/__init__.py` & `etos_lib-4.1.0/tests/__init__.py`

 * *Files identical despite different names*

