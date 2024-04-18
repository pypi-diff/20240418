# Comparing `tmp/matrix-alertbot-0.1.6.tar.gz` & `tmp/matrix_alertbot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix-alertbot-0.1.6.tar", last modified: Sun Jan 29 21:30:44 2023, max compression
+gzip compressed data, was "matrix_alertbot-0.2.0.tar", last modified: Wed Apr 17 14:49:38 2024, max compression
```

## Comparing `matrix-alertbot-0.1.6.tar` & `matrix_alertbot-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.090166 matrix-alertbot-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2486 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1491 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    34523 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2912 2023-01-29 21:30:44.094165 matrix-alertbot-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2031 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4024 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/SETUP.md
--rw-rw-rw-   0 root         (0) root         (0)     2847 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/config.sample.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.058167 matrix-alertbot-0.1.6/docker/
--rw-rw-rw-   0 root         (0) root         (0)      172 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/.env
--rw-rw-rw-   0 root         (0) root         (0)     3127 2022-10-29 12:18:36.000000 matrix-alertbot-0.1.6/docker/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2757 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.058167 matrix-alertbot-0.1.6/docker/alertmanager/
--rw-rw-rw-   0 root         (0) root         (0)      272 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/alertmanager/alertmanager.sample.yml
--rwxrwxrwx   0 root         (0) root         (0)      910 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/build_and_install_libolm.sh
--rw-rw-rw-   0 root         (0) root         (0)     1275 2022-10-29 12:18:36.000000 matrix-alertbot-0.1.6/docker/docker-compose.yml
--rw-rw-rw-   0 root         (0) root         (0)      366 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/matrix-alertbot.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.058167 matrix-alertbot-0.1.6/docker/prometheus/
--rw-rw-rw-   0 root         (0) root         (0)      884 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/prometheus/prometheus.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.058167 matrix-alertbot-0.1.6/docker/prometheus/rules.d/
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/docker/prometheus/rules.d/health.yml
--rwxrwxrwx   0 root         (0) root         (0)      202 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix-alertbot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.070166 matrix-alertbot-0.1.6/matrix_alertbot/
--rw-rw-rw-   0 root         (0) root         (0)      363 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/alert.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/alertmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    14180 2022-10-26 15:31:44.000000 matrix-alertbot-0.1.6/matrix_alertbot/callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2022-11-25 18:33:11.000000 matrix-alertbot-0.1.6/matrix_alertbot/chat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    10409 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/command.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2022-10-26 16:02:44.000000 matrix-alertbot-0.1.6/matrix_alertbot/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6973 2022-11-25 18:22:41.000000 matrix-alertbot-0.1.6/matrix_alertbot/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.034167 matrix-alertbot-0.1.6/matrix_alertbot/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.078166 matrix-alertbot-0.1.6/matrix_alertbot/resources/templates/
--rw-rw-rw-   0 root         (0) root         (0)      205 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/resources/templates/alert.html.j2
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/matrix_alertbot/resources/templates/alert.txt.j2
--rw-rw-rw-   0 root         (0) root         (0)     7596 2023-01-29 20:44:48.000000 matrix-alertbot-0.1.6/matrix_alertbot/webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.074166 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2912 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1491 2023-01-29 21:30:44.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      659 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-29 21:30:43.000000 matrix-alertbot-0.1.6/matrix_alertbot.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.078166 matrix-alertbot-0.1.6/scripts-dev/
--rwxrwxrwx   0 root         (0) root         (0)      360 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/scripts-dev/lint.sh
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-01-29 21:30:44.102165 matrix-alertbot-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       93 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.086166 matrix-alertbot-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.038167 matrix-alertbot-0.1.6/tests/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.090166 matrix-alertbot-0.1.6/tests/resources/config/
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/resources/config/config.full.yml
--rw-rw-rw-   0 root         (0) root         (0)      933 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/resources/config/config.minimal.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 21:30:44.090166 matrix-alertbot-0.1.6/tests/resources/templates/
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/resources/templates/alert.html.j2
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/resources/templates/alert.txt.j2
--rw-rw-rw-   0 root         (0) root         (0)     6039 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/test_alert.py
--rw-rw-rw-   0 root         (0) root         (0)    35742 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/test_alertmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    37680 2022-10-26 15:31:44.000000 matrix-alertbot-0.1.6/tests/test_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8343 2022-11-25 18:53:44.000000 matrix-alertbot-0.1.6/tests/test_chat_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    27299 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)    11913 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)    14925 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/test_webhook.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2022-10-26 15:13:16.000000 matrix-alertbot-0.1.6/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.091632 matrix_alertbot-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-04-17 14:30:34.000000 matrix_alertbot-0.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-17 14:49:38.091632 matrix_alertbot-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4024 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/SETUP.md
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-17 13:57:06.000000 matrix_alertbot-0.2.0/config.sample.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.075631 matrix_alertbot-0.2.0/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/.env
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2757 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.075631 matrix_alertbot-0.2.0/docker/alertmanager/
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/alertmanager/alertmanager.sample.yml
+-rwxrwxrwx   0 root         (0) root         (0)      910 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/build_and_install_libolm.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/docker-compose.yml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/matrix-alertbot.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.075631 matrix_alertbot-0.2.0/docker/prometheus/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/prometheus/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.075631 matrix_alertbot-0.2.0/docker/prometheus/rules.d/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/docker/prometheus/rules.d/health.yml
+-rwxrwxrwx   0 root         (0) root         (0)      202 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix-alertbot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.079631 matrix_alertbot-0.2.0/matrix_alertbot/
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/alert.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/alertmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    17597 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/matrix_alertbot/callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3559 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/chat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10639 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     7346 2024-04-17 13:57:06.000000 matrix_alertbot-0.2.0/matrix_alertbot/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9654 2024-01-22 10:50:25.000000 matrix_alertbot-0.2.0/matrix_alertbot/matrix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.067631 matrix_alertbot-0.2.0/matrix_alertbot/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.079631 matrix_alertbot-0.2.0/matrix_alertbot/resources/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/resources/templates/alert.html.j2
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/matrix_alertbot/resources/templates/alert.txt.j2
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2024-01-22 10:43:28.000000 matrix_alertbot-0.2.0/matrix_alertbot/webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.083632 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-04-17 14:49:38.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      695 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 14:49:37.000000 matrix_alertbot-0.2.0/matrix_alertbot.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-17 14:42:10.000000 matrix_alertbot-0.2.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.079631 matrix_alertbot-0.2.0/scripts-dev/
+-rwxrwxrwx   0 root         (0) root         (0)      360 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/scripts-dev/lint.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2024-04-17 14:49:38.095632 matrix_alertbot-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.083632 matrix_alertbot-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 14:49:14.000000 matrix_alertbot-0.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.067631 matrix_alertbot-0.2.0/tests/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.083632 matrix_alertbot-0.2.0/tests/resources/config/
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-04-17 13:57:06.000000 matrix_alertbot-0.2.0/tests/resources/config/config.full.yml
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/tests/resources/config/config.minimal.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:49:38.083632 matrix_alertbot-0.2.0/tests/resources/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/tests/resources/templates/alert.html.j2
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/tests/resources/templates/alert.txt.j2
+-rw-rw-rw-   0 root         (0) root         (0)     6039 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/tests/test_alert.py
+-rw-rw-rw-   0 root         (0) root         (0)    35542 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/tests/test_alertmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    47486 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/tests/test_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     7908 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/tests/test_chat_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27112 2024-01-22 10:35:45.000000 matrix_alertbot-0.2.0/tests/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)    15829 2024-04-17 14:00:04.000000 matrix_alertbot-0.2.0/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/tests/test_matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)    22094 2024-04-17 13:00:17.000000 matrix_alertbot-0.2.0/tests/test_webhook.py
```

### Comparing `matrix-alertbot-0.1.6/.gitlab-ci.yml` & `matrix_alertbot-0.2.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -56,26 +56,24 @@
       artifacts: false
 
 tests:
   extends: .pip template
   stage: test
   script:
     - apk add --no-cache libstdc++
-    - coverage run --source matrix_alertbot -m pytest --junitxml=report.xml
-    - coverage report --precision 2
-    - coverage xml -o coverage.xml
+    - pytest --junitxml report.xml
   cache:
     policy: pull
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: report.xml
-  coverage: '/^TOTAL\s+\d+\s+\d+\s+(\d+\.\d+\%)$/'
+  coverage: '/Total coverage: ([\d\.]+\%)$/'
   needs:
     - job: linting
       artifacts: false
 
 publish test:
   extends: .pip template
   stage: publish
```

### Comparing `matrix-alertbot-0.1.6/CONTRIBUTING.md` & `matrix_alertbot-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/LICENSE` & `matrix_alertbot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/PKG-INFO` & `matrix_alertbot-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: matrix-alertbot
-Version: 0.1.6
-Summary: A matrix bot to manage alerts from Alertmanager
-Home-page: https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
-Project-URL: Documentation, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/blob/master/README.md
-Project-URL: Source, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot
-Project-URL: Tracker, https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/issues
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: test
-Provides-Extra: e2e
-Provides-Extra: all
-License-File: LICENSE
-
 # Matrix AlertBot [![Built with matrix-nio](https://img.shields.io/badge/built%20with-matrix--nio-brightgreen)](https://github.com/poljar/matrix-nio) [![coverage report](https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/badges/master/coverage.svg)](https://gitlab.domainepublic.net/Neutrinet/matrix-alertbot/-/commits/master) 
 
 A bot that receives alert from [Alertmanager](https://prometheus.io/docs/alerting/latest/alertmanager) to send them to a Matrix room. Users can interract with the bot to create silences for the alerts.
 
 Features include:
 
 * Send alerts from Alertmanager to a Matrix room
```

### Comparing `matrix-alertbot-0.1.6/SETUP.md` & `matrix_alertbot-0.2.0/SETUP.md`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/config.sample.yaml` & `matrix_alertbot-0.2.0/config.sample.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 # Default values are shown
 
 # The string to prefix messages with to talk to the bot in group chats
 command_prefix: "!alert"
 
 # Options for connecting to the bot's Matrix account
 matrix:
-  # The Matrix User ID of the bot account
-  user_id: "@bot:matrix.example.com"
-
-  # Matrix account password (optional if access token used)
-  user_password: "password"
-
-  # Matrix account access token (optional if password used)
-  # If not set, the server will provide an access token after log in,
-  # which will be stored in the user token file (see below)
-  #user_token: ""
-
-  # Path to the file where to store the user access token
-  user_token_file: "token.json"
-
-  # The URL of the homeserver to connect to
-  url: https://matrix.example.com
-
-  # The device ID that is **non pre-existing** device
-  # If this device ID already exists, messages will be dropped silently in encrypted rooms
-  # If not set the server will provide a device ID after log in. Note that this ID
-  # will change each time the bot reconnects.
-  # device_id: ABCDEFGHIJ
+  accounts:
+    - # The Matrix User IDs of the bot account
+      id: "@bot:matrix.example.com"
+
+      # Matrix account password (optional if access token used)
+      password: "password"
+
+      # Matrix account access token (optional if password used)
+      # If not set, the server will provide an access token after log in,
+      # which will be stored in the user token file (see below)
+      #token: ""
+
+      # Path to the file where to store the user access token
+      token_file: "token.json"
+
+      # The URL of the homeserver to connect to
+      url: https://matrix.example.com
+
+      # The device ID that is **non pre-existing** device
+      # If this device ID already exists, messages will be dropped silently in encrypted rooms
+      # If not set the server will provide a device ID after log in. Note that this ID
+      # will change each time the bot reconnects.
+      # device_id: ABCDEFGHIJ
 
   # What to name the logged in device
   device_name: matrix-alertbot
 
   # List of rooms where the bot can interact
   allowed_rooms:
     - "!abcdefgh:matrix.example.com"
@@ -68,20 +69,23 @@
   # and must respect Jinja2 templating format.
   # Default is to use templates provided by the matrix_alertbot package. 
   # These templates are available in "matrix_alertbot/resources/templates".
   path: "data/templates"
 
 # Logging setup
 logging:
-  # Logging level
-  # Allowed levels are 'INFO', 'WARNING', 'ERROR', 'DEBUG' where DEBUG is most verbose
-  level: INFO
+
   # Configure logging to a file
   file_logging:
     # Whether logging to a file is enabled
     enabled: false
+    # Logging level specific to file logging (optional)
+    level: DEBUG
     # The path to the file to log to. May be relative or absolute
     filepath: matrix-alertbot.log
   # Configure logging to the console output
   console_logging:
     # Whether logging to the console is enabled
     enabled: true
+    # Logging level specific to console (optional)
+    # Allowed levels are 'INFO', 'WARNING', 'ERROR', 'DEBUG' where DEBUG is most verbose
+    level: INFO
```

### Comparing `matrix-alertbot-0.1.6/docker/Dockerfile` & `matrix_alertbot-0.2.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/docker/README.md` & `matrix_alertbot-0.2.0/docker/README.md`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/docker/build_and_install_libolm.sh` & `matrix_alertbot-0.2.0/docker/build_and_install_libolm.sh`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/docker/docker-compose.yml` & `matrix_alertbot-0.2.0/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/docker/prometheus/prometheus.yml` & `matrix_alertbot-0.2.0/docker/prometheus/prometheus.yml`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/alert.py` & `matrix_alertbot-0.2.0/matrix_alertbot/alert.py`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/alertmanager.py` & `matrix_alertbot-0.2.0/matrix_alertbot/alertmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime, timedelta
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional, Tuple, TypedDict, cast
 
 import aiohttp
 from aiohttp import ClientError
 from aiohttp_prometheus_exporter.trace import PrometheusTraceConfig
 from diskcache import Cache
 
 from matrix_alertbot.errors import (
@@ -19,50 +19,68 @@
 
 DEFAULT_DURATION = timedelta(hours=3)
 MAX_DURATION = timedelta(days=3652)
 
 
 logger = logging.getLogger(__name__)
 
+AlertDict = TypedDict(
+    "AlertDict",
+    {
+        "fingerprint": str,
+        "labels": Dict[str, str],
+    },
+)
+
+SilenceDict = TypedDict(
+    "SilenceDict",
+    {
+        "id": str,
+        "matchers": List[Dict[str, Any]],
+        "createdBy": str,
+        "status": Dict[str, str],
+    },
+)
+
 
 class AlertmanagerClient:
     def __init__(self, url: str, cache: Cache) -> None:
         self.api_url = f"{url}/api/v2"
         self.cache = cache
         self.session = aiohttp.ClientSession(trace_configs=[PrometheusTraceConfig()])
 
     async def close(self) -> None:
         await self.session.close()
 
-    async def get_alerts(self) -> List[Dict]:
+    async def get_alerts(self) -> List[AlertDict]:
         try:
             async with self.session.get(f"{self.api_url}/alerts") as response:
                 response.raise_for_status()
                 return await response.json()
         except ClientError as e:
             raise AlertmanagerServerError(
                 "Cannot fetch alerts from Alertmanager"
             ) from e
 
-    async def get_alert(self, fingerprint: str) -> Dict:
+    async def get_alert(self, fingerprint: str) -> AlertDict:
         logger.debug(f"Fetching details for alert with fingerprint {fingerprint}")
         alerts = await self.get_alerts()
         return self._find_alert(fingerprint, alerts)
 
-    async def get_silences(self) -> List[Dict]:
+    async def get_silences(self) -> List[SilenceDict]:
         try:
             async with self.session.get(f"{self.api_url}/silences") as response:
                 response.raise_for_status()
                 return await response.json()
         except ClientError as e:
             raise AlertmanagerServerError(
                 "Cannot fetch silences from Alertmanager"
             ) from e
 
-    async def get_silence(self, silence_id: str) -> Dict:
+    async def get_silence(self, silence_id: str) -> SilenceDict:
         logger.debug(f"Fetching details for silence with ID {silence_id}")
         silences = await self.get_silences()
         return self._find_silence(silence_id, silences)
 
     async def create_silence(
         self,
         fingerprint: str,
@@ -89,20 +107,23 @@
         duration_seconds: Optional[int] = None,
         *,
         force: bool = False,
     ) -> str:
         logger.debug(
             f"Reading silence for alert with fingerprint {fingerprint} from cache"
         )
-        try:
-            silence_id: Optional[str]
-            expire_time: Optional[int]
-            silence_id, expire_time = self.cache.get(fingerprint, expire_time=True)
-        except TypeError:
+
+        cache_result = cast(
+            Optional[Tuple[str, int]], self.cache.get(fingerprint, expire_time=True)
+        )
+        if cache_result is not None:
+            silence_id, expire_time = cache_result
+        else:
             silence_id = None
+            expire_time = None
 
         if silence_id is None:
             raise SilenceNotFoundError(
                 f"Cannot find silence for alert with fingerprint {fingerprint} in cache."
             )
 
         logger.debug(
@@ -198,19 +219,19 @@
                 response.raise_for_status()
         except ClientError as e:
             raise AlertmanagerServerError(
                 f"Cannot delete silence with ID {silence_id}"
             ) from e
 
     @staticmethod
-    def _find_alert(fingerprint: str, alerts: List[Dict]) -> Dict:
+    def _find_alert(fingerprint: str, alerts: List[AlertDict]) -> AlertDict:
         for alert in alerts:
             if alert["fingerprint"] == fingerprint:
                 return alert
         raise AlertNotFoundError(f"Cannot find alert with fingerprint {fingerprint}")
 
     @staticmethod
-    def _find_silence(silence_id: str, silences: List[Dict]) -> Dict:
+    def _find_silence(silence_id: str, silences: List[SilenceDict]) -> SilenceDict:
         for silence in silences:
             if silence["id"] == silence_id:
                 return silence
         raise SilenceNotFoundError(f"Cannot find silence with ID {silence_id}")
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/chat_functions.py` & `matrix_alertbot-0.2.0/matrix_alertbot/chat_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,15 @@
+from __future__ import annotations
+
 import logging
 from typing import Dict, Optional, TypedDict, Union
 
-from nio import (
-    AsyncClient,
-    ErrorResponse,
-    Response,
-    RoomSendError,
-    RoomSendResponse,
-    SendRetryError,
-)
+from nio.client import AsyncClient
+from nio.exceptions import SendRetryError
+from nio.responses import ErrorResponse, Response, RoomSendError, RoomSendResponse
 from typing_extensions import NotRequired
 
 logger = logging.getLogger(__name__)
 
 
 ContentEventDict = TypedDict(
     "ContentEventDict",
@@ -26,15 +23,15 @@
 )
 
 
 async def send_text_to_room(
     matrix_client: AsyncClient,
     room_id: str,
     plaintext: str,
-    html: str = None,
+    html: Optional[str] = None,
     notice: bool = True,
     reply_to_event_id: Optional[str] = None,
 ) -> RoomSendResponse:
     """Send text to a matrix room.
 
     Args:
         client: The client to communicate to matrix with.
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/command.py` & `matrix_alertbot-0.2.0/matrix_alertbot/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import logging
-from typing import Optional, Tuple
+from typing import Optional, Tuple, cast
 
 import pytimeparse2
 from diskcache import Cache
-from nio import AsyncClient, MatrixRoom
+from nio.client import AsyncClient
+from nio.rooms import MatrixRoom
 
 from matrix_alertbot.alertmanager import AlertmanagerClient
 from matrix_alertbot.chat_functions import send_text_to_room
 from matrix_alertbot.config import Config
 from matrix_alertbot.errors import (
     AlertmanagerError,
     AlertNotFoundError,
@@ -24,15 +27,15 @@
         matrix_client: AsyncClient,
         cache: Cache,
         alertmanager_client: AlertmanagerClient,
         config: Config,
         room: MatrixRoom,
         sender: str,
         event_id: str,
-        args: Tuple[str, ...] = None,
+        args: Tuple[str, ...] = (),
     ) -> None:
         """A command made by a user.
 
         Args:
             client: The client to communicate with Matrix.
 
             cache: Bot cache.
@@ -73,15 +76,15 @@
         cache: Cache,
         alertmanager: AlertmanagerClient,
         config: Config,
         room: MatrixRoom,
         sender: str,
         event_id: str,
         reacted_to_event_id: str,
-        args: Tuple[str, ...] = None,
+        args: Tuple[str, ...] = (),
     ) -> None:
         super().__init__(
             client, cache, alertmanager, config, room, sender, event_id, args
         )
 
         self.reacted_to_event_id = reacted_to_event_id
 
@@ -90,15 +93,15 @@
     async def process(self) -> None:
         """Acknowledge an alert and silence it for a certain duration in Alertmanager"""
         durations = self.args
         if len(durations) > 0:
             duration = " ".join(durations)
             logger.debug(f"Receiving a command to create a silence for {duration}.")
 
-            duration_seconds = pytimeparse2.parse(duration)
+            duration_seconds = cast(Optional[int], pytimeparse2.parse(duration))
             if duration_seconds is None:
                 logger.error(f"Unable to create silence: Invalid duration '{duration}'")
                 await send_text_to_room(
                     self.matrix_client,
                     self.room.room_id,
                     f"I tried really hard, but I can't convert the duration '{duration}' to a number of seconds.",
                 )
@@ -119,25 +122,29 @@
                 "Receiving a command to create a silence for an indefinite period"
             )
 
         logger.debug(
             f"Reading alert fingerprint for event {self.reacted_to_event_id} from cache"
         )
         try:
-            alert_fingerprint: str = self.cache[self.reacted_to_event_id]
+            alert_fingerprint = cast(str, self.cache[self.reacted_to_event_id])
         except KeyError:
             logger.error(
                 f"Cannot find fingerprint for alert event {self.reacted_to_event_id} in cache"
             )
             return
 
+        sender_user_name = self.room.user_name(self.sender)
+        if sender_user_name is None:
+            sender_user_name = self.sender
+
         try:
             silence_id = await self.alertmanager_client.create_or_update_silence(
                 alert_fingerprint,
-                self.room.user_name(self.sender),
+                sender_user_name,
                 duration_seconds,
                 force=True,
             )
         except AlertNotFoundError as e:
             logger.warning(f"Unable to create silence: {e}")
             await send_text_to_room(
                 self.matrix_client,
@@ -169,27 +176,27 @@
         """Delete an alert's acknowledgement of an alert and remove corresponding silence in Alertmanager"""
         logger.debug("Receiving a command to delete a silence")
 
         logger.debug(
             f"Reading alert fingerprint for event {self.reacted_to_event_id} from cache."
         )
         try:
-            alert_fingerprint: str = self.cache[self.reacted_to_event_id]
+            alert_fingerprint = cast(str, self.cache[self.reacted_to_event_id])
         except KeyError:
             logger.error(
                 f"Cannot find fingerprint for alert event {self.reacted_to_event_id} in cache."
             )
             return
         logger.debug(f"Found alert fingerprint {alert_fingerprint} in cache.")
 
         logger.debug(
             f"Reading silence ID for alert fingerprint {alert_fingerprint} from cache."
         )
         try:
-            silence_id: str = self.cache[alert_fingerprint]
+            silence_id = cast(str, self.cache[alert_fingerprint])
         except KeyError:
             logger.error(
                 f"Cannot find silence for alert fingerprint {alert_fingerprint} in cache"
             )
             return
         logger.debug(f"Found silence ID {silence_id} in cache.")
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/config.py` & `matrix_alertbot-0.2.0/matrix_alertbot/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import logging
 import os
 import re
 import sys
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional
 
 import pytimeparse2
 import yaml
 
 from matrix_alertbot.errors import (
     InvalidConfigError,
     ParseConfigError,
@@ -18,14 +20,35 @@
     logging.INFO
 )  # Prevent debug messages from peewee lib
 
 
 DEFAULT_REACTIONS = {"🤫", "😶", "🤐", "🙊", "🔇", "🔕"}
 
 
+class AccountConfig:
+    def __init__(self, account: Dict[str, str]) -> None:
+        self.id: str = account["id"]
+        if not re.match("@.+:.+", self.id):
+            raise InvalidConfigError("matrix.user_id must be in the form @name:domain")
+
+        self.password: Optional[str] = account.get("password")
+        self.token: Optional[str] = account.get("token")
+
+        if self.password is None and self.token is None:
+            raise RequiredConfigKeyError("Must supply either user token or password")
+
+        self.device_id: Optional[str] = account.get("device_id")
+        self.token_file: str = account.get("token_file", "token.json")
+
+        self.homeserver_url: str = account["url"]
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.id})"
+
+
 class Config:
     """Creates a Config object from a YAML-encoded config file from a given filepath"""
 
     def __init__(self, filepath: str):
         self.filepath = filepath
         if not os.path.isfile(filepath):
             raise ParseConfigError(f"Config file '{filepath}' does not exist")
@@ -40,34 +63,45 @@
     def _parse_config_values(self) -> None:
         """Read and validate each config option"""
         # Logging setup
         formatter = logging.Formatter(
             "%(asctime)s | %(name)s [%(levelname)s] %(message)s"
         )
 
-        log_level = self._get_cfg(["logging", "level"], default="INFO")
-        logger.setLevel(log_level)
+        # this must be DEBUG to allow debug messages
+        # actual log levels are defined in the handlers below
+        logger.setLevel("DEBUG")
 
         file_logging_enabled = self._get_cfg(
             ["logging", "file_logging", "enabled"], default=False
         )
         file_logging_filepath = self._get_cfg(
             ["logging", "file_logging", "filepath"], default="matrix-alertbot.log"
         )
+        file_logging_log_level = self._get_cfg(
+            ["logging", "file_logging", "level"], default="INFO"
+        )
         if file_logging_enabled:
             file_handler = logging.FileHandler(file_logging_filepath)
             file_handler.setFormatter(formatter)
+            if file_logging_log_level:
+                file_handler.setLevel(file_logging_log_level)
             logger.addHandler(file_handler)
 
         console_logging_enabled = self._get_cfg(
             ["logging", "console_logging", "enabled"], default=True
         )
+        console_logging_log_level = self._get_cfg(
+            ["logging", "console_logging", "level"], default="INFO"
+        )
         if console_logging_enabled:
             console_handler = logging.StreamHandler(sys.stdout)
             console_handler.setFormatter(formatter)
+            if console_logging_log_level:
+                console_handler.setLevel(console_logging_log_level)
             logger.addHandler(console_handler)
 
         # Storage setup
         self.store_dir: str = self._get_cfg(["storage", "path"], required=True)
 
         # Create the store folder if it doesn't exist
         if not os.path.isdir(self.store_dir):
@@ -87,34 +121,30 @@
         self.cache_expire_time = pytimeparse2.parse(expire_time)
 
         # Alertmanager client setup
         self.alertmanager_url: str = self._get_cfg(
             ["alertmanager", "url"], required=True
         )
 
-        # Matrix bot account setup
-        self.user_id: str = self._get_cfg(["matrix", "user_id"], required=True)
-        if not re.match("@.+:.+", self.user_id):
-            raise InvalidConfigError("matrix.user_id must be in the form @name:domain")
-
-        self.user_password: str = self._get_cfg(
-            ["matrix", "user_password"], required=False
-        )
-        self.user_token: str = self._get_cfg(["matrix", "user_token"], required=False)
-        if not self.user_token and not self.user_password:
-            raise RequiredConfigKeyError("Must supply either user token or password")
-
-        self.device_id: str = self._get_cfg(["matrix", "device_id"], required=False)
+        # Matrix bot accounts setup
+        self.accounts: List[AccountConfig] = []
+        accounts_dict: list = self._get_cfg(["matrix", "accounts"], required=True)
+        for i, account_dict in enumerate(accounts_dict):
+            try:
+                account = AccountConfig(account_dict)
+            except KeyError as e:
+                key_name = e.args[0]
+                raise RequiredConfigKeyError(
+                    f"Config option matrix.accounts.{i}.{key_name} is required"
+                )
+            self.accounts.append(account)
+        self.user_ids = {account.id for account in self.accounts}
         self.device_name: str = self._get_cfg(
             ["matrix", "device_name"], default="matrix-alertbot"
         )
-        self.user_token_file: str = self._get_cfg(
-            ["matrix", "user_token_file"], default="token.json"
-        )
-        self.homeserver_url: str = self._get_cfg(["matrix", "url"], required=True)
         self.allowed_rooms: list = self._get_cfg(
             ["matrix", "allowed_rooms"], required=True
         )
         self.allowed_reactions = set(
             self._get_cfg(["matrix", "allowed_reactions"], default=DEFAULT_REACTIONS)
         )
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/errors.py` & `matrix_alertbot-0.2.0/matrix_alertbot/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,7 +59,13 @@
     pass
 
 
 class AlertmanagerServerError(AlertmanagerError):
     """An error encountered with Alertmanager server."""
 
     pass
+
+
+class MatrixClientError(MatrixAlertbotError):
+    """An error encountered with the Matrix client"""
+
+    pass
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/main.py` & `matrix_alertbot-0.2.0/matrix_alertbot/matrix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,252 @@
-#!/usr/bin/env python3
+from __future__ import annotations
+
 import asyncio
 import json
 import logging
 import os
-import sys
-from asyncio import TimeoutError
+import random
+from typing import Dict, List, Optional, Tuple
 
 from aiohttp import ClientConnectionError, ServerDisconnectedError
 from diskcache import Cache
-from nio import (
-    AsyncClient,
-    AsyncClientConfig,
+from nio.client import AsyncClient, AsyncClientConfig
+from nio.events import (
     InviteMemberEvent,
     KeyVerificationCancel,
     KeyVerificationKey,
     KeyVerificationMac,
     KeyVerificationStart,
-    LocalProtocolError,
-    LoginError,
     MegolmEvent,
+    ReactionEvent,
     RedactionEvent,
     RoomMessageText,
-    UnknownEvent,
+    RoomMessageUnknown,
 )
+from nio.exceptions import LocalProtocolError
+from nio.responses import LoginError, WhoamiError
 
+import matrix_alertbot.callback
 from matrix_alertbot.alertmanager import AlertmanagerClient
-from matrix_alertbot.callback import Callbacks
-from matrix_alertbot.config import Config
-from matrix_alertbot.webhook import Webhook
+from matrix_alertbot.config import AccountConfig, Config
 
 logger = logging.getLogger(__name__)
 
 
-def create_matrix_client(config: Config) -> AsyncClient:
-    # Configuration options for the AsyncClient
-    try:
-        matrix_client_config = AsyncClientConfig(
-            max_limit_exceeded=5,
-            max_timeouts=3,
-            store_sync_tokens=True,
-            encryption_enabled=True,
-        )
-    except ImportWarning as e:
-        logger.warning(e)
-        matrix_client_config = AsyncClientConfig(
-            max_limit_exceeded=5,
-            max_timeouts=3,
-            store_sync_tokens=True,
-            encryption_enabled=False,
-        )
-
-    # Load credentials from a previous session
-    if os.path.exists(config.user_token_file):
-        with open(config.user_token_file, "r") as ifd:
-            credentials = json.load(ifd)
-            config.user_token = credentials["access_token"]
-            config.device_id = credentials["device_id"]
-
-    # Initialize the matrix client based on stored credentials
-    matrix_client = AsyncClient(
-        config.homeserver_url,
-        config.user_id,
-        device_id=config.device_id,
-        store_path=config.store_dir,
-        config=matrix_client_config,
-    )
-
-    return matrix_client
-
-
-async def start_matrix_client(
-    matrix_client: AsyncClient, cache: Cache, config: Config
-) -> bool:
-    # Keep trying to reconnect on failure (with some time in-between)
-    while True:
-        try:
-            if config.device_id and config.user_token:
-                matrix_client.restore_login(
-                    user_id=config.user_id,
-                    device_id=config.device_id,
-                    access_token=config.user_token,
-                )
+class MatrixClientPool:
+    def __init__(
+        self, alertmanager_client: AlertmanagerClient, cache: Cache, config: Config
+    ) -> None:
+        self._lock = asyncio.Lock()
+        self._matrix_clients: Dict[AccountConfig, AsyncClient] = {}
+        self._accounts: List[AccountConfig] = []
+
+        self._accounts = config.accounts
+        for account in self._accounts:
+            matrix_client = self._create_matrix_client(
+                account, alertmanager_client, cache, config
+            )
+            self._matrix_clients[account] = matrix_client
+
+        self.account = next(iter(self._accounts))
+        self.matrix_client = self._matrix_clients[self.account]
+
+    async def switch_active_client(
+        self,
+    ) -> Optional[Tuple[AsyncClient, AccountConfig]]:
+        async with self._lock:
+            for account in random.sample(self._accounts, len(self._accounts)):
+                if account is self.account:
+                    continue
 
-                # Sync encryption keys with the server
-                if matrix_client.should_upload_keys:
-                    await matrix_client.keys_upload()
-            else:
-                # Try to login with the configured username/password
+                matrix_client = self._matrix_clients[account]
                 try:
-                    login_response = await matrix_client.login(
-                        password=config.user_password,
-                        device_name=config.device_name,
-                    )
+                    whoami = await matrix_client.whoami()
+                    logged_in = not isinstance(whoami, WhoamiError)
+                except Exception:
+                    logged_in = False
+
+                if logged_in:
+                    self.account = account
+                    self.matrix_client = matrix_client
 
-                    # Check if login failed
-                    if type(login_response) == LoginError:
-                        logger.error("Failed to login: %s", login_response.message)
-                        return False
-                except LocalProtocolError as e:
-                    # There's an edge case here where the user hasn't installed the correct C
-                    # dependencies. In that case, a LocalProtocolError is raised on login.
-                    logger.fatal(
-                        "Failed to login. Have you installed the correct dependencies? "
-                        "https://github.com/poljar/matrix-nio#installation "
-                        "Error: %s",
-                        e,
+                    logger.warning(
+                        f"Bot {self.account.id} | Matrix client for homeserver {self.account.homeserver_url} selected as new leader."
                     )
-                    return False
 
-                # Save user's access token and device ID
-                # See https://stackoverflow.com/a/45368120
-                user_token_fd = os.open(
-                    config.user_token_file,
-                    flags=os.O_CREAT | os.O_WRONLY | os.O_TRUNC,
-                    mode=0o640,
+                    return matrix_client, account
+
+            if self.matrix_client.logged_in:
+                logger.warning(
+                    f"Bot {self.account.id} | No active Matrix client available, keeping Matrix client for {self.account.homeserver_url} as the leader."
+                )
+            else:
+                logger.error(
+                    f"Bot {self.account.id} | No active Matrix client connected."
                 )
-                with os.fdopen(user_token_fd, "w") as ofd:
-                    json.dump(
-                        {
-                            "device_id": login_response.device_id,
-                            "access_token": login_response.access_token,
-                        },
-                        ofd,
+        return None
+
+    async def close(self) -> None:
+        for matrix_client in self._matrix_clients.values():
+            await matrix_client.close()
+
+    def _create_matrix_client(
+        self,
+        account: AccountConfig,
+        alertmanager_client: AlertmanagerClient,
+        cache: Cache,
+        config: Config,
+    ) -> AsyncClient:
+        # Configuration options for the AsyncClient
+        try:
+            matrix_client_config = AsyncClientConfig(
+                max_limit_exceeded=5,
+                max_timeouts=3,
+                store_sync_tokens=True,
+                encryption_enabled=True,
+            )
+        except ImportWarning as e:
+            logger.warning(e)
+            matrix_client_config = AsyncClientConfig(
+                max_limit_exceeded=5,
+                max_timeouts=3,
+                store_sync_tokens=True,
+                encryption_enabled=False,
+            )
+
+        # Load credentials from a previous session
+        if os.path.exists(account.token_file):
+            with open(account.token_file, "r") as ifd:
+                credentials = json.load(ifd)
+                account.token = credentials["access_token"]
+                account.device_id = credentials["device_id"]
+
+        # Initialize the matrix client based on stored credentials
+        matrix_client = AsyncClient(
+            account.homeserver_url,
+            account.id,
+            device_id=account.device_id,
+            store_path=config.store_dir,
+            config=matrix_client_config,
+        )
+
+        # Set up event callbacks
+        callbacks = matrix_alertbot.callback.Callbacks(
+            matrix_client, alertmanager_client, cache, config, self
+        )
+
+        matrix_client.add_event_callback(callbacks.message, (RoomMessageText,))
+        matrix_client.add_event_callback(
+            callbacks.invite_event_filtered_callback, (InviteMemberEvent,)
+        )
+        # matrix_client.add_event_callback(callbacks.debug, (Event,))
+        matrix_client.add_event_callback(callbacks.decryption_failure, (MegolmEvent,))
+        matrix_client.add_event_callback(callbacks.reaction, (ReactionEvent,))
+        matrix_client.add_event_callback(callbacks.redaction, (RedactionEvent,))
+        matrix_client.add_event_callback(
+            callbacks.unknown_message, (RoomMessageUnknown,)
+        )
+        matrix_client.add_to_device_callback(
+            callbacks.key_verification_start, (KeyVerificationStart,)
+        )
+        matrix_client.add_to_device_callback(
+            callbacks.key_verification_cancel, (KeyVerificationCancel,)
+        )
+        matrix_client.add_to_device_callback(
+            callbacks.key_verification_confirm, (KeyVerificationKey,)
+        )
+        matrix_client.add_to_device_callback(
+            callbacks.key_verification_end, (KeyVerificationMac,)
+        )
+
+        return matrix_client
+
+    async def start(
+        self,
+        account: AccountConfig,
+        config: Config,
+    ):
+        matrix_client = self._matrix_clients[account]
+
+        # Keep trying to reconnect on failure (with some time in-between)
+        # We switch homeserver after some retries
+        while True:
+            try:
+                if account.device_id and account.token:
+                    matrix_client.restore_login(
+                        user_id=account.id,
+                        device_id=account.device_id,
+                        access_token=account.token,
                     )
 
-                # Login succeeded!
+                    # Sync encryption keys with the server
+                    if matrix_client.should_upload_keys:
+                        await matrix_client.keys_upload()
+                else:
+                    # Try to login with the configured username/password
+                    try:
+                        login_response = await matrix_client.login(
+                            password=account.password,
+                            device_name=config.device_name,
+                        )
+
+                        # Check if login failed
+                        if isinstance(login_response, LoginError):
+                            logger.error(
+                                f"Bot {account.id} | Failed to login: {login_response.message}"
+                            )
+                            return False
+                    except LocalProtocolError as e:
+                        # There's an edge case here where the user hasn't installed the correct C
+                        # dependencies. In that case, a LocalProtocolError is raised on login.
+                        logger.fatal(
+                            f"Bot {account.id} | Failed to login. Have you installed the correct dependencies? "
+                            "https://github.com/poljar/matrix-nio#installation "
+                            "Error: %s",
+                            e,
+                        )
+                        return False
 
-            logger.info(f"Logged in as {config.user_id}")
-            await matrix_client.sync_forever(timeout=30000, full_state=True)
-        except (ClientConnectionError, ServerDisconnectedError, TimeoutError):
-            logger.warning("Unable to connect to homeserver, retrying in 15s...")
-
-            # Sleep so we don't bombard the server with login requests
-            await asyncio.sleep(15)
-        finally:
-            await matrix_client.close()
+                    if isinstance(login_response, LoginError):
+                        logger.fatal(
+                            f"Bot {account.id} | Failed to login: {login_response.message}"
+                        )
+                        return False
 
+                    # Save user's access token and device ID
+                    # See https://stackoverflow.com/a/45368120
+                    account_token_fd = os.open(
+                        account.token_file,
+                        flags=os.O_CREAT | os.O_WRONLY | os.O_TRUNC,
+                        mode=0o640,
+                    )
+                    with os.fdopen(account_token_fd, "w") as ofd:
+                        json.dump(
+                            {
+                                "device_id": login_response.device_id,
+                                "access_token": login_response.access_token,
+                            },
+                            ofd,
+                        )
+
+                    # Login succeeded!
+
+                logger.info(f"Bot {account.id} | Logged in.")
+
+                await matrix_client.sync_forever(timeout=30000, full_state=True)
+            except (ClientConnectionError, ServerDisconnectedError, TimeoutError):
+                await matrix_client.close()
+
+                logger.warning(
+                    f"Bot {account.id} | Matrix client disconnected, retrying in 15s..."
+                )
 
-def main() -> None:
-    """The first function that is run when starting the bot"""
+                if len(self._accounts) > 1 and self.matrix_client is matrix_client:
+                    logger.warning(
+                        f"Bot {account.id} | Selecting another Matrix client as leader..."
+                    )
+                    await self.switch_active_client()
 
-    # Read user-configured options from a config file.
-    # A different config file path can be specified as the first command line argument
-    if len(sys.argv) > 1:
-        config_path = sys.argv[1]
-    else:
-        config_path = "config.yaml"
-
-    # Read the parsed config file and create a Config object
-    config = Config(config_path)
-
-    matrix_client = create_matrix_client(config)
-
-    # Configure the cache
-    cache = Cache(config.cache_dir)
-
-    # Configure Alertmanager client
-    alertmanager_client = AlertmanagerClient(config.alertmanager_url, cache)
-
-    # Set up event callbacks
-    callbacks = Callbacks(matrix_client, alertmanager_client, cache, config)
-    matrix_client.add_event_callback(callbacks.message, (RoomMessageText,))
-    matrix_client.add_event_callback(
-        callbacks.invite_event_filtered_callback, (InviteMemberEvent,)
-    )
-    matrix_client.add_event_callback(callbacks.decryption_failure, (MegolmEvent,))
-    matrix_client.add_event_callback(callbacks.unknown, (UnknownEvent,))
-    matrix_client.add_event_callback(callbacks.redaction, (RedactionEvent,))
-    matrix_client.add_to_device_callback(
-        callbacks.key_verification_start, (KeyVerificationStart,)
-    )
-    matrix_client.add_to_device_callback(
-        callbacks.key_verification_cancel, (KeyVerificationCancel,)
-    )
-    matrix_client.add_to_device_callback(
-        callbacks.key_verification_confirm, (KeyVerificationKey,)
-    )
-    matrix_client.add_to_device_callback(
-        callbacks.key_verification_end, (KeyVerificationMac,)
-    )
-    # Configure webhook server
-    webhook_server = Webhook(matrix_client, alertmanager_client, cache, config)
-
-    loop = asyncio.get_event_loop()
-    loop.create_task(webhook_server.start())
-    loop.create_task(start_matrix_client(matrix_client, cache, config))
-
-    try:
-        loop.run_forever()
-    except Exception as e:
-        logger.error(e)
-    finally:
-        loop.run_until_complete(webhook_server.close())
-        loop.run_until_complete(alertmanager_client.close())
-        loop.run_until_complete(matrix_client.close())
-        cache.close()
+                # Sleep so we don't bombard the server with login requests
+                await asyncio.sleep(15)
+            finally:
+                await matrix_client.close()
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot/webhook.py` & `matrix_alertbot-0.2.0/matrix_alertbot/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
 import logging
+from typing import List
 
 import prometheus_client
 from aiohttp import ClientError, web, web_request
 from aiohttp.abc import AbstractAccessLogger
 from aiohttp_prometheus_exporter.handler import metrics
 from aiohttp_prometheus_exporter.middleware import prometheus_middleware_factory
 from diskcache import Cache
-from nio import AsyncClient, LocalProtocolError, SendRetryError
+from nio.exceptions import LocalProtocolError, SendRetryError
 
 from matrix_alertbot.alert import Alert, AlertRenderer
 from matrix_alertbot.alertmanager import AlertmanagerClient
 from matrix_alertbot.chat_functions import send_text_to_room
 from matrix_alertbot.config import Config
 from matrix_alertbot.errors import (
     AlertmanagerError,
+    MatrixClientError,
     SilenceExtendError,
     SilenceNotFoundError,
 )
+from matrix_alertbot.matrix import MatrixClientPool
 
 logger = logging.getLogger(__name__)
 
 routes = web.RouteTableDef()
 
 
 class AccessLogger(AbstractAccessLogger):
@@ -78,32 +81,32 @@
     if "alerts" not in data:
         logger.error("Received data without 'alerts' key")
         return web.Response(status=400, body="Data must contain 'alerts' key.")
 
     alert_dicts = data["alerts"]
 
     if not isinstance(data["alerts"], list):
-        alerts_type = type(alert_dicts).__name__
+        alerts_type = alert_dicts.__class__.__name__
         logger.error(f"Received data with invalid alerts type '{alerts_type}'.")
         return web.Response(
             status=400, body=f"Alerts must be a list, got '{alerts_type}'."
         )
 
     logger.info(f"Received {len(alert_dicts)} alerts for room ID {room_id}: {data}")
 
     if len(data["alerts"]) == 0:
         return web.Response(status=400, body="Alerts cannot be empty.")
 
-    alerts = []
-    for alert in alert_dicts:
+    alerts: List[Alert] = []
+    for alert_dict in alert_dicts:
         try:
-            alert = Alert.from_dict(alert)
+            alert = Alert.from_dict(alert_dict)
         except KeyError as e:
             logger.error(f"Cannot parse alert dict: {e}")
-            return web.Response(status=400, body=f"Invalid alert: {alert}.")
+            return web.Response(status=400, body=f"Invalid alert: {alert_dict}.")
         alerts.append(alert)
 
     for alert in alerts:
         try:
             await create_alert(alert, room_id, request)
         except AlertmanagerError as e:
             logger.error(
@@ -117,14 +120,22 @@
             logger.error(
                 f"Unable to send alert {alert.fingerprint} to Matrix room {room_id}: {e}"
             )
             return web.Response(
                 status=500,
                 body=f"An error occured when sending alert with fingerprint '{alert.fingerprint}' to Matrix room.",
             )
+        except MatrixClientError as e:
+            logger.error(
+                f"Unable to send alert {alert.fingerprint} to Matrix room {room_id}: {e}"
+            )
+            return web.Response(
+                status=500,
+                body=f"An error occured when sending alert with fingerprint '{alert.fingerprint}' to Matrix room.",
+            )
         except Exception as e:
             logger.error(
                 f"Unable to send alert {alert.fingerprint} to Matrix room {room_id}: {e}"
             )
             return web.Response(
                 status=500,
                 body=f"An exception occured when sending alert with fingerprint '{alert.fingerprint}' to Matrix room.",
@@ -134,15 +145,15 @@
 
 
 async def create_alert(
     alert: Alert, room_id: str, request: web_request.Request
 ) -> None:
     alertmanager_client: AlertmanagerClient = request.app["alertmanager_client"]
     alert_renderer: AlertRenderer = request.app["alert_renderer"]
-    matrix_client: AsyncClient = request.app["matrix_client"]
+    matrix_client_pool: MatrixClientPool = request.app["matrix_client_pool"]
     cache: Cache = request.app["cache"]
     config: Config = request.app["config"]
 
     if alert.firing:
         try:
             silence_id = await alertmanager_client.update_silence(alert.fingerprint)
             logger.debug(
@@ -158,34 +169,37 @@
             logger.debug(
                 f"Unable to extend silence for alert with fingerprint {alert.fingerprint}: {e}"
             )
 
     plaintext = alert_renderer.render(alert, html=False)
     html = alert_renderer.render(alert, html=True)
 
-    event = await send_text_to_room(
-        matrix_client, room_id, plaintext, html, notice=False
-    )
+    if matrix_client_pool.matrix_client is not None:
+        event = await send_text_to_room(
+            matrix_client_pool.matrix_client, room_id, plaintext, html, notice=False
+        )
+    else:
+        raise MatrixClientError("No matrix client available")
 
     if alert.firing:
         cache.set(event.event_id, alert.fingerprint, expire=config.cache_expire_time)
     else:
         cache.delete(alert.fingerprint)
 
 
 class Webhook:
     def __init__(
         self,
-        matrix_client: AsyncClient,
+        matrix_client_pool: MatrixClientPool,
         alertmanager_client: AlertmanagerClient,
         cache: Cache,
         config: Config,
     ) -> None:
         self.app = web.Application(logger=logger)
-        self.app["matrix_client"] = matrix_client
+        self.app["matrix_client_pool"] = matrix_client_pool
         self.app["alertmanager_client"] = alertmanager_client
         self.app["config"] = config
         self.app["cache"] = cache
         self.app["alert_renderer"] = AlertRenderer(config.template_dir)
         self.app.add_routes(routes)
 
         prometheus_registry = prometheus_client.CollectorRegistry(auto_describe=True)
```

### Comparing `matrix-alertbot-0.1.6/matrix_alertbot.egg-info/SOURCES.txt` & `matrix_alertbot-0.2.0/matrix_alertbot.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 matrix_alertbot/alertmanager.py
 matrix_alertbot/callback.py
 matrix_alertbot/chat_functions.py
 matrix_alertbot/command.py
 matrix_alertbot/config.py
 matrix_alertbot/errors.py
 matrix_alertbot/main.py
+matrix_alertbot/matrix.py
 matrix_alertbot/webhook.py
 matrix_alertbot.egg-info/PKG-INFO
 matrix_alertbot.egg-info/SOURCES.txt
 matrix_alertbot.egg-info/dependency_links.txt
 matrix_alertbot.egg-info/entry_points.txt
 matrix_alertbot.egg-info/not-zip-safe
 matrix_alertbot.egg-info/requires.txt
@@ -46,13 +47,13 @@
 tests/__init__.py
 tests/test_alert.py
 tests/test_alertmanager.py
 tests/test_callback.py
 tests/test_chat_functions.py
 tests/test_command.py
 tests/test_config.py
+tests/test_matrix.py
 tests/test_webhook.py
-tests/utils.py
 tests/resources/config/config.full.yml
 tests/resources/config/config.minimal.yml
 tests/resources/templates/alert.html.j2
 tests/resources/templates/alert.txt.j2
```

### Comparing `matrix-alertbot-0.1.6/setup.cfg` & `matrix_alertbot-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 include_package_data = True
 install_requires = 
 	aiohttp>=3.8.1
 	aiohttp-prometheus-exporter>=0.2.4
 	aiotools>=1.5.9
 	diskcache>=5.4.0
 	jinja2>=3.1.2
-	matrix-nio>=0.19.0
+	matrix-nio>=0.24.0
 	Markdown>=3.3.7
 	pytimeparse2>=1.4.0
 	PyYAML>=5.4.1
 	typing-extensions>=4.3.0
 python_requires = >=3.9
 setup_requires = 
 	setuptools_scm
@@ -46,21 +46,22 @@
 test = 
 	coverage>=6.4.1
 	black>=22.6.0
 	flake8>=4.0.1
 	flake8-comprehensions>=3.10.0
 	isort>=5.10.1
 	mypy>=0.961
-	pytest>=7.1.2
+	pytest>=7.4.0
+	pytest-cov>=4.1.0
 	pytest-asyncio>=0.18.3
 	freezegun>=1.2.1
 	types-PyYAML>=6.0.9
 	types-setuptools>=62.6.0
 e2e = 
-	matrix-nio[e2e]>=0.19.0
+	matrix-nio[e2e]>=0.24.0
 all = 
 	%(test)s
 	%(e2e)s
 
 [flake8]
 ignore = W503,W504,E203,E731,E501
 exclude =
```

### Comparing `matrix-alertbot-0.1.6/tests/resources/config/config.full.yml` & `matrix_alertbot-0.2.0/tests/resources/config/config.full.yml`

 * *Files 24% similar despite different names*

```diff
@@ -3,36 +3,60 @@
 # Default values are shown
 
 # The string to prefix messages with to talk to the bot in group chats
 command_prefix: "!alert"
 
 # Options for connecting to the bot's Matrix account
 matrix:
-  # The Matrix User ID of the bot account
-  user_id: "@fakes_user:matrix.example.com"
-
-  # Matrix account password (optional if access token used)
-  user_password: "password"
-
-  # Matrix account access token (optional if password used)
-  # If not set, the server will provide an access token after log in,
-  # which will be stored in the user token file (see below)
-  #user_token: ""
-
-  # Path to the file where to store the user access token
-  user_token_file: "token.json"
-
-  # The URL of the homeserver to connect to
-  url: https://matrix.example.com
-
-  # The device ID that is **non pre-existing** device
-  # If this device ID already exists, messages will be dropped silently in encrypted rooms
-  # If not set the server will provide a device ID after log in. Note that this ID
-  # will change each time the bot reconnects.
-  device_id: ABCDEFGHIJ
+  accounts:
+    - # The Matrix User ID of the bot account
+      id: "@fakes_user:matrix.example.com"
+
+      # Matrix account password (optional if access token used)
+      password: "password"
+
+      # Matrix account access token (optional if password used)
+      # If not set, the server will provide an access token after log in,
+      # which will be stored in the user token file (see below)
+      #token: ""
+
+      # Path to the file where to store the user access token
+      token_file: "fake_token.json"
+
+      # The URL of the homeserver to connect to
+      url: https://matrix.example.com
+
+      # The device ID that is **non pre-existing** device
+      # If this device ID already exists, messages will be dropped silently in encrypted rooms
+      # If not set the server will provide a device ID after log in. Note that this ID
+      # will change each time the bot reconnects.
+      device_id: ABCDEFGHIJ
+
+    - # The Matrix User ID of the bot account
+      id: "@other_user:matrix.domain.tld"
+
+      # Matrix account password (optional if access token used)
+      #password: "password"
+
+      # Matrix account access token (optional if password used)
+      # If not set, the server will provide an access token after log in,
+      # which will be stored in the user token file (see below)
+      token: "token"
+
+      # Path to the file where to store the user access token
+      token_file: "other_token.json"
+
+      # The URL of the homeserver to connect to
+      url: https://matrix.domain.tld
+
+      # The device ID that is **non pre-existing** device
+      # If this device ID already exists, messages will be dropped silently in encrypted rooms
+      # If not set the server will provide a device ID after log in. Note that this ID
+      # will change each time the bot reconnects.
+      device_id: KLMNOPQRST
 
   # What to name the logged in device
   device_name: fake_device_name
 
   # List of rooms where the bot can interact
   allowed_rooms:
     - "!abcdefgh:matrix.example.com"
@@ -62,20 +86,20 @@
   # Path to directory that contains templates for rendering alerts.
   # The directory must contains the files "alert.html.j2" and "alert.txt.j2"
   # and must respect Jinja2 templating format.
   path: "data/templates"
 
 # Logging setup
 logging:
-  # Logging level
-  # Allowed levels are 'INFO', 'WARNING', 'ERROR', 'DEBUG' where DEBUG is most verbose
-  level: DEBUG
   # Configure logging to a file
   file_logging:
     # Whether logging to a file is enabled
     enabled: true
     # The path to the file to log to. May be relative or absolute
     filepath: fake.log
+    # Logging level specific to file (optional)
+    # Allowed levels are 'INFO', 'WARNING', 'ERROR', 'DEBUG' where DEBUG is most verbose
+    level: INFO
   # Configure logging to the console output
   console_logging:
     # Whether logging to the console is enabled
     enabled: false
```

### Comparing `matrix-alertbot-0.1.6/tests/resources/config/config.minimal.yml` & `matrix_alertbot-0.2.0/tests/resources/config/config.minimal.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Welcome to the sample config file
 # Below you will find various config sections and options
 # Default values are shown
 
 # Options for connecting to the bot's Matrix account
 matrix:
-  # The Matrix User ID of the bot account
-  user_id: "@fakes_user:matrix.example.com"
+  accounts:
+    - # The Matrix User ID of the bot account
+      id: "@fakes_user:matrix.example.com"
 
-  # Matrix account password (optional if access token used)
-  user_password: "password"
+      # Matrix account password (optional if access token used)
+      password: "password"
 
-  # The URL of the homeserver to connect to
-  url: https://matrix.example.com
+      # The URL of the homeserver to connect to
+      url: https://matrix.example.com
 
   # List of rooms where the bot can interact
   allowed_rooms:
     - "!abcdefgh:matrix.example.com"
 
 webhook:
   # Address and port for which the bot should listen to
```

### Comparing `matrix-alertbot-0.1.6/tests/test_alert.py` & `matrix_alertbot-0.2.0/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `matrix-alertbot-0.1.6/tests/test_alertmanager.py` & `matrix_alertbot-0.2.0/tests/test_alertmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,14 @@
     AlertNotFoundError,
     SilenceExpiredError,
     SilenceExtendError,
     SilenceNotFoundError,
 )
 
 
-async def update_silence_raise_silence_not_found(
-    fingerprint: str, user: str, duration_seconds: int, *, force: bool = False
-) -> str:
-    raise SilenceNotFoundError
-
-
 class FakeCache:
     def __init__(self, cache_dict: Optional[Dict] = None) -> None:
         if cache_dict is None:
             cache_dict = {}
         self.cache = cache_dict
 
     def get(
@@ -529,22 +523,28 @@
                 "endsAt": "1970-01-11T00:00:00",
                 "comment": "Acknowledge alert from Matrix",
             },
             silence2,
         )
         self.assertEqual({"fingerprint1": ("silence2", 864000)}, fake_cache.cache)
 
-    @patch.object(matrix_alertbot.alertmanager.AlertmanagerClient, "update_silence")
-    @patch.object(matrix_alertbot.alertmanager.AlertmanagerClient, "create_silence")
+    @patch.object(
+        matrix_alertbot.alertmanager.AlertmanagerClient,
+        "update_silence",
+        side_effect=SilenceNotFoundError,
+    )
+    @patch.object(
+        matrix_alertbot.alertmanager.AlertmanagerClient,
+        "create_silence",
+        return_value="silence1",
+    )
     async def test_create_or_update_silence_with_duration_and_silence_not_found(
         self, fake_create_silence: Mock, fake_update_silence: Mock
     ) -> None:
         fake_cache = Mock(spec=Cache)
-        fake_update_silence.side_effect = update_silence_raise_silence_not_found
-        fake_create_silence.return_value = "silence1"
 
         alertmanager_client = AlertmanagerClient("http://localhost", fake_cache)
         async with aiotools.closing_async(alertmanager_client):
             silence_id1 = await alertmanager_client.create_or_update_silence(
                 "fingerprint1", "user", 86400
             )
 
@@ -647,22 +647,28 @@
                 "endsAt": "1970-01-01T03:00:00",
                 "comment": "Acknowledge alert from Matrix",
             },
             silence,
         )
         self.assertEqual({"fingerprint1": ("silence2", None)}, fake_cache.cache)
 
-    @patch.object(matrix_alertbot.alertmanager.AlertmanagerClient, "update_silence")
-    @patch.object(matrix_alertbot.alertmanager.AlertmanagerClient, "create_silence")
+    @patch.object(
+        matrix_alertbot.alertmanager.AlertmanagerClient,
+        "update_silence",
+        side_effect=SilenceNotFoundError,
+    )
+    @patch.object(
+        matrix_alertbot.alertmanager.AlertmanagerClient,
+        "create_silence",
+        return_value="silence1",
+    )
     async def test_create_or_update_silence_without_duration_and_silence_not_found(
         self, fake_create_silence: Mock, fake_update_silence: Mock
     ) -> None:
         fake_cache = Mock(spec=Cache)
-        fake_update_silence.side_effect = update_silence_raise_silence_not_found
-        fake_create_silence.return_value = "silence1"
 
         alertmanager_client = AlertmanagerClient("http://localhost", fake_cache)
         async with aiotools.closing_async(alertmanager_client):
             silence_id1 = await alertmanager_client.create_or_update_silence(
                 "fingerprint1", "user"
             )
```

### Comparing `matrix-alertbot-0.1.6/tests/test_callback.py` & `matrix_alertbot-0.2.0/tests/test_callback.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,142 @@
+from __future__ import annotations
+
 import unittest
 from typing import Dict
-from unittest.mock import MagicMock, Mock, patch
+from unittest.mock import MagicMock, Mock, call, patch
 
 import nio
 import nio.crypto
 from diskcache import Cache
 
+import matrix_alertbot.alertmanager
 import matrix_alertbot.callback
 import matrix_alertbot.command
-from matrix_alertbot.alertmanager import AlertmanagerClient
-from matrix_alertbot.callback import Callbacks
-from matrix_alertbot.command import BaseCommand
-
-from tests.utils import make_awaitable
-
-
-def key_verification_get_mac_raise_protocol_error():
-    raise nio.LocalProtocolError
+import matrix_alertbot.matrix
 
 
 class CallbacksTestCase(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         # Create a Callbacks object and give it some Mock'd objects to use
         self.fake_matrix_client = Mock(spec=nio.AsyncClient)
-        self.fake_matrix_client.user = "@fake_user:example.com"
+        self.fake_matrix_client.user_id = "@fake_user:example.com"
+        # self.fake_matrix_client.user = "@fake_user"
 
         self.fake_cache = MagicMock(spec=Cache)
-        self.fake_alertmanager_client = Mock(spec=AlertmanagerClient)
+        self.fake_alertmanager_client = Mock(
+            spec=matrix_alertbot.alertmanager.AlertmanagerClient
+        )
 
         # Create a fake room to play with
         self.fake_room = Mock(spec=nio.MatrixRoom)
         self.fake_room.room_id = "!abcdefg:example.com"
         self.fake_room.display_name = "Fake Room"
 
         # We don't spec config, as it doesn't currently have well defined attributes
         self.fake_config = Mock()
         self.fake_config.allowed_rooms = [self.fake_room.room_id]
         self.fake_config.allowed_reactions = ["🤫"]
         self.fake_config.command_prefix = "!alert "
+        self.fake_config.user_ids = [self.fake_matrix_client.user_id]
 
-        self.callbacks = Callbacks(
+        self.fake_matrix_client_pool = Mock(
+            spec=matrix_alertbot.matrix.MatrixClientPool
+        )
+        self.fake_matrix_client_pool.matrix_client = self.fake_matrix_client
+
+        self.callbacks = matrix_alertbot.callback.Callbacks(
             self.fake_matrix_client,
             self.fake_alertmanager_client,
             self.fake_cache,
             self.fake_config,
+            self.fake_matrix_client_pool,
         )
 
     async def test_invite(self) -> None:
         """Tests the callback for InviteMemberEvents"""
         # Tests that the bot attempts to join a room after being invited to it
         fake_invite_event = Mock(spec=nio.InviteMemberEvent)
         fake_invite_event.sender = "@some_other_fake_user:example.com"
 
-        # Pretend that attempting to join a room is always successful
-        self.fake_matrix_client.join.return_value = make_awaitable()
-
         # Pretend that we received an invite event
         await self.callbacks.invite(self.fake_room, fake_invite_event)
 
         # Check that we attempted to join the room
         self.fake_matrix_client.join.assert_called_once_with(self.fake_room.room_id)
 
+    async def test_invite_in_unauthorized_room(self) -> None:
+        """Tests the callback for InviteMemberEvents"""
+        # Tests that the bot attempts to join a room after being invited to it
+        fake_invite_event = Mock(spec=nio.InviteMemberEvent)
+        fake_invite_event.sender = "@some_other_fake_user:example.com"
+
+        self.fake_room.room_id = "!unauthorizedroom@example.com"
+
+        # Pretend that we received an invite event
+        await self.callbacks.invite(self.fake_room, fake_invite_event)
+
+        # Check that we attempted to join the room
+        self.fake_matrix_client.join.assert_not_called()
+
+    async def test_invite_raise_join_error(self) -> None:
+        """Tests the callback for InviteMemberEvents"""
+        # Tests that the bot attempts to join a room after being invited to it
+        fake_invite_event = Mock(spec=nio.InviteMemberEvent)
+        fake_invite_event.sender = "@some_other_fake_user:example.com"
+
+        fake_join_error = Mock(spec=nio.JoinError)
+        fake_join_error.message = "error message"
+        self.fake_matrix_client.join.return_value = fake_join_error
+
+        # Pretend that we received an invite event
+        await self.callbacks.invite(self.fake_room, fake_invite_event)
+
+        # Check that we attempted to join the room
+        self.fake_matrix_client.join.assert_has_calls(
+            [
+                call("!abcdefg:example.com"),
+                call("!abcdefg:example.com"),
+                call("!abcdefg:example.com"),
+            ]
+        )
+
     @patch.object(matrix_alertbot.callback.CommandFactory, "create", autospec=True)
     async def test_message_without_prefix(self, fake_command_create: Mock) -> None:
         """Tests the callback for RoomMessageText without any command prefix"""
         # Tests that the bot process messages in the room
         fake_message_event = Mock(spec=nio.RoomMessageText)
         fake_message_event.sender = "@some_other_fake_user:example.com"
         fake_message_event.body = "Hello world!"
+        fake_message_event.event_id = "some event id"
 
         # Pretend that we received a text message event
         await self.callbacks.message(self.fake_room, fake_message_event)
 
         # Check that the command was not executed
         fake_command_create.assert_not_called()
 
     @patch.object(matrix_alertbot.command, "HelpCommand", autospec=True)
+    async def test_message_help_client_not_in_pool(self, fake_command: Mock) -> None:
+        """Tests the callback for RoomMessageText without any command prefix"""
+        # Tests that the bot process messages in the room
+        fake_message_event = Mock(spec=nio.RoomMessageText)
+        fake_message_event.event_id = "some event id"
+        fake_message_event.sender = "@some_other_fake_user:example.com"
+        fake_message_event.body = "!alert help"
+        fake_message_event.source = {"content": {}}
+
+        self.fake_matrix_client_pool.matrix_client = None
+
+        # Pretend that we received a text message event
+        await self.callbacks.message(self.fake_room, fake_message_event)
+
+        # Check that the command was not executed
+        fake_command.assert_not_called()
+
+    @patch.object(matrix_alertbot.command, "HelpCommand", autospec=True)
     async def test_message_help_not_in_reply_with_prefix(
         self, fake_command: Mock
     ) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_message_event = Mock(spec=nio.RoomMessageText)
         fake_message_event.event_id = "some event id"
@@ -136,15 +193,15 @@
 
     @patch.object(matrix_alertbot.command.CommandFactory, "create", autospec=True)
     async def test_ignore_message_sent_by_bot(self, fake_create_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
 
         fake_message_event = Mock(spec=nio.RoomMessageText)
-        fake_message_event.sender = self.fake_matrix_client.user
+        fake_message_event.sender = self.fake_matrix_client.user_id
 
         # Pretend that we received a text message event
         await self.callbacks.message(self.fake_room, fake_message_event)
 
         # Check that we attempted to execute the command
         fake_create_command.assert_not_called()
 
@@ -260,44 +317,100 @@
             fake_message_event.sender,
             fake_message_event.event_id,
             "some alert event id",
             (),
         )
         fake_command.return_value.process.assert_called_once()
 
+    @patch.object(matrix_alertbot.callback, "logger", autospec=True)
+    @patch.object(matrix_alertbot.command, "AckAlertCommand", autospec=True)
+    async def test_message_raise_exception(
+        self, fake_command: Mock, fake_logger
+    ) -> None:
+        """Tests the callback for RoomMessageText with the command prefix"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_message_event = Mock(spec=nio.RoomMessageText)
+        fake_message_event.event_id = "some event id"
+        fake_message_event.sender = "@some_other_fake_user:example.com"
+        fake_message_event.body = "!alert ack"
+        fake_message_event.source = {
+            "content": {
+                "m.relates_to": {"m.in_reply_to": {"event_id": "some alert event id"}}
+            }
+        }
+
+        fake_command.return_value.process.side_effect = (
+            nio.exceptions.LocalProtocolError
+        )
+
+        # Pretend that we received a text message event
+        await self.callbacks.message(self.fake_room, fake_message_event)
+
+        # Check that the command was not executed
+        fake_command.assert_called_once_with(
+            self.fake_matrix_client,
+            self.fake_cache,
+            self.fake_alertmanager_client,
+            self.fake_config,
+            self.fake_room,
+            fake_message_event.sender,
+            fake_message_event.event_id,
+            "some alert event id",
+            (),
+        )
+        fake_command.return_value.process.assert_called_once()
+
+        fake_logger.exception.assert_called_once()
+
+    @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
+    async def test_reaction_client_not_in_pool(self, fake_command: Mock) -> None:
+        """Tests the callback for RoomMessageText with the command prefix"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_alert_event = Mock(spec=nio.RoomMessageText)
+        fake_alert_event.event_id = "some alert event id"
+        fake_alert_event.sender = self.fake_matrix_client.user_id
+
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
+        fake_reaction_event.event_id = "some event id"
+        fake_reaction_event.sender = "@some_other_fake_user:example.com"
+        fake_reaction_event.reacts_to = fake_alert_event.event_id
+        fake_reaction_event.key = "🤫"
+
+        fake_event_response = Mock(spec=nio.RoomGetEventResponse)
+        fake_event_response.event = fake_alert_event
+        self.fake_matrix_client.room_get_event.return_value = fake_event_response
+
+        self.fake_matrix_client_pool.matrix_client = None
+
+        # Pretend that we received a text message event
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
+
+        # Check that we attempted to execute the command
+        fake_command.assert_not_called()
+
     @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
     async def test_reaction_to_existing_alert(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event = Mock(spec=nio.RoomMessageText)
         fake_alert_event.event_id = "some alert event id"
-        fake_alert_event.sender = self.fake_config.user_id
+        fake_alert_event.sender = self.fake_matrix_client.user_id
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
-        fake_reaction_event.type = "m.reaction"
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.event_id = "some event id"
         fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event.event_id,
-                    "key": "🤫",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.reacts_to = fake_alert_event.event_id
+        fake_reaction_event.key = "🤫"
 
         fake_event_response = Mock(spec=nio.RoomGetEventResponse)
         fake_event_response.event = fake_alert_event
-        self.fake_matrix_client.room_get_event.return_value = make_awaitable(
-            fake_event_response
-        )
+        self.fake_matrix_client.room_get_event.return_value = fake_event_response
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_called_once_with(
             self.fake_matrix_client,
             self.fake_cache,
             self.fake_alertmanager_client,
             self.fake_config,
@@ -313,35 +426,26 @@
 
     @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
     async def test_reaction_to_inexistent_event(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event_id = "some alert event id"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.type = "m.reaction"
         fake_reaction_event.event_id = "some event id"
         fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event_id,
-                    "key": "🤫",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.reacts_to = fake_alert_event_id
+        fake_reaction_event.key = "🤫"
 
         fake_event_response = Mock(spec=nio.RoomGetEventError)
-        self.fake_matrix_client.room_get_event.return_value = make_awaitable(
-            fake_event_response
-        )
+        self.fake_matrix_client.room_get_event.return_value = fake_event_response
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_not_called()
         self.fake_cache.set.assert_not_called()
         self.fake_matrix_client.room_get_event.assert_called_once_with(
             self.fake_room.room_id, fake_alert_event_id
         )
@@ -352,96 +456,116 @@
     ) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event = Mock(spec=nio.RoomMessageText)
         fake_alert_event.event_id = "some alert event id"
         fake_alert_event.sender = "@some_other_fake_user.example.com"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.type = "m.reaction"
         fake_reaction_event.event_id = "some event id"
         fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event.event_id,
-                    "key": "🤫",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.reacts_to = fake_alert_event.event_id
+        fake_reaction_event.key = "🤫"
 
         fake_event_response = Mock(spec=nio.RoomGetEventResponse)
         fake_event_response.event = fake_alert_event
-        self.fake_matrix_client.room_get_event.return_value = make_awaitable(
-            fake_event_response
-        )
+        self.fake_matrix_client.room_get_event.return_value = fake_event_response
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_not_called()
         self.fake_cache.set.assert_not_called()
         self.fake_matrix_client.room_get_event.assert_called_once_with(
             self.fake_room.room_id, fake_alert_event.event_id
         )
 
+    @patch.object(matrix_alertbot.callback, "logger", autospec=True)
+    @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
+    async def test_reaction_raise_exception(
+        self, fake_command: Mock, fake_logger: Mock
+    ) -> None:
+        """Tests the callback for RoomMessageText with the command prefix"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_alert_event = Mock(spec=nio.RoomMessageText)
+        fake_alert_event.event_id = "some alert event id"
+        fake_alert_event.sender = self.fake_matrix_client.user_id
+
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
+        fake_reaction_event.event_id = "some event id"
+        fake_reaction_event.sender = "@some_other_fake_user:example.com"
+        fake_reaction_event.reacts_to = fake_alert_event.event_id
+        fake_reaction_event.key = "🤫"
+
+        fake_event_response = Mock(spec=nio.RoomGetEventResponse)
+        fake_event_response.event = fake_alert_event
+        self.fake_matrix_client.room_get_event.return_value = fake_event_response
+
+        fake_command.return_value.process.side_effect = (
+            nio.exceptions.LocalProtocolError
+        )
+
+        # Pretend that we received a text message event
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
+
+        # Check that we attempted to execute the command
+        fake_command.assert_called_once_with(
+            self.fake_matrix_client,
+            self.fake_cache,
+            self.fake_alertmanager_client,
+            self.fake_config,
+            self.fake_room,
+            fake_reaction_event.sender,
+            fake_reaction_event.event_id,
+            "some alert event id",
+        )
+        fake_command.return_value.process.assert_called_once()
+        self.fake_matrix_client.room_get_event.assert_called_once_with(
+            self.fake_room.room_id, fake_alert_event.event_id
+        )
+
+        fake_logger.exception.assert_called_once()
+
     @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
     async def test_reaction_unknown(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event_id = "some alert event id"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.type = "m.reaction"
         fake_reaction_event.event_id = "some event id"
         fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event_id,
-                    "key": "unknown",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.reacts_to = fake_alert_event_id
+        fake_reaction_event.key = "unknown"
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_not_called()
         self.fake_matrix_client.room_get_event.assert_not_called()
 
     @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
     async def test_ignore_reaction_sent_by_bot_user(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event_id = "some alert event id"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.type = "m.reaction"
         fake_reaction_event.event_id = "some event id"
-        fake_reaction_event.sender = self.fake_matrix_client.user
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event_id,
-                    "key": "unknown",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.sender = self.fake_matrix_client.user_id
+        fake_reaction_event.reacts_to = fake_alert_event_id
+        fake_reaction_event.key = "unknown"
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
-        await self.callbacks._reaction(
-            self.fake_room, fake_reaction_event, fake_alert_event_id
-        )
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_not_called()
         self.fake_matrix_client.room_get_event.assert_not_called()
 
     @patch.object(matrix_alertbot.callback, "AckAlertCommand", autospec=True)
     async def test_ignore_reaction_in_unauthorized_room(
@@ -449,39 +573,51 @@
     ) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         self.fake_room.room_id = "!unauthorizedroom@example.com"
 
         fake_alert_event_id = "some alert event id"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
+        fake_reaction_event = Mock(spec=nio.ReactionEvent)
         fake_reaction_event.type = "m.reaction"
         fake_reaction_event.event_id = "some event id"
         fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {
-            "content": {
-                "m.relates_to": {
-                    "event_id": fake_alert_event_id,
-                    "key": "unknown",
-                    "rel_type": "m.annotation",
-                }
-            }
-        }
+        fake_reaction_event.reacts_to = fake_alert_event_id
+        fake_reaction_event.key = "unknown"
 
         # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
-        await self.callbacks._reaction(
-            self.fake_room, fake_reaction_event, fake_alert_event_id
-        )
+        await self.callbacks.reaction(self.fake_room, fake_reaction_event)
 
         # Check that we attempted to execute the command
         fake_command.assert_not_called()
         self.fake_matrix_client.room_get_event.assert_not_called()
 
     @patch.object(matrix_alertbot.callback, "UnackAlertCommand", autospec=True)
+    async def test_redaction_client_not_in_pool(self, fake_command: Mock) -> None:
+        """Tests the callback for RoomMessageText with the command prefix"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_alert_event_id = "some alert event id"
+
+        fake_redaction_event = Mock(spec=nio.RedactionEvent)
+        fake_redaction_event.redacts = "some other event id"
+        fake_redaction_event.event_id = "some event id"
+        fake_redaction_event.sender = "@some_other_fake_user:example.com"
+
+        fake_cache_dict = {fake_redaction_event.redacts: fake_alert_event_id}
+        self.fake_cache.__getitem__.side_effect = fake_cache_dict.__getitem__
+
+        self.fake_matrix_client_pool.matrix_client = None
+
+        # Pretend that we received a text message event
+        await self.callbacks.redaction(self.fake_room, fake_redaction_event)
+
+        # Check that we attempted to execute the command
+        fake_command.assert_not_called()
+
+    @patch.object(matrix_alertbot.callback, "UnackAlertCommand", autospec=True)
     async def test_redaction(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_alert_event_id = "some alert event id"
 
         fake_redaction_event = Mock(spec=nio.RedactionEvent)
         fake_redaction_event.redacts = "some other event id"
@@ -503,20 +639,59 @@
             self.fake_room,
             fake_redaction_event.sender,
             fake_redaction_event.event_id,
             fake_redaction_event.redacts,
         )
         fake_command.return_value.process.assert_called_once()
 
+    @patch.object(matrix_alertbot.callback, "logger", autospec=True)
+    @patch.object(matrix_alertbot.callback, "UnackAlertCommand", autospec=True)
+    async def test_redaction_raise_exception(
+        self, fake_command: Mock, fake_logger
+    ) -> None:
+        """Tests the callback for RoomMessageText with the command prefix"""
+        # Tests that the bot process messages in the room that contain a command
+        fake_alert_event_id = "some alert event id"
+
+        fake_redaction_event = Mock(spec=nio.RedactionEvent)
+        fake_redaction_event.redacts = "some other event id"
+        fake_redaction_event.event_id = "some event id"
+        fake_redaction_event.sender = "@some_other_fake_user:example.com"
+
+        fake_cache_dict = {fake_redaction_event.redacts: fake_alert_event_id}
+        self.fake_cache.__getitem__.side_effect = fake_cache_dict.__getitem__
+
+        fake_command.return_value.process.side_effect = (
+            nio.exceptions.LocalProtocolError
+        )
+
+        # Pretend that we received a text message event
+        await self.callbacks.redaction(self.fake_room, fake_redaction_event)
+
+        # Check that we attempted to execute the command
+        fake_command.assert_called_once_with(
+            self.fake_matrix_client,
+            self.fake_cache,
+            self.fake_alertmanager_client,
+            self.fake_config,
+            self.fake_room,
+            fake_redaction_event.sender,
+            fake_redaction_event.event_id,
+            fake_redaction_event.redacts,
+        )
+        fake_command.return_value.process.assert_called_once()
+
+        fake_logger.exception.assert_called_once()
+
     @patch.object(matrix_alertbot.callback, "UnackAlertCommand", autospec=True)
     async def test_ignore_redaction_sent_by_bot_user(self, fake_command: Mock) -> None:
         """Tests the callback for RoomMessageText with the command prefix"""
         # Tests that the bot process messages in the room that contain a command
         fake_redaction_event = Mock(spec=nio.RedactionEvent)
-        fake_redaction_event.sender = self.fake_matrix_client.user
+        fake_redaction_event.sender = self.fake_matrix_client.user_id
 
         fake_cache_dict: Dict = {}
         self.fake_cache.__getitem__.side_effect = fake_cache_dict.__getitem__
 
         # Pretend that we received a text message event
         await self.callbacks.redaction(self.fake_room, fake_redaction_event)
 
@@ -552,17 +727,14 @@
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.from_device = "ABCDEFGH"
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.short_authentication_string = ["emoji"]
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.accept_key_verification.return_value = make_awaitable()
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
-
         fake_sas = Mock()
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_start(fake_key_verification_event)
 
@@ -579,17 +751,14 @@
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.from_device = "ABCDEFGH"
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.short_authentication_string = []
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.accept_key_verification.return_value = make_awaitable()
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
-
         fake_sas = Mock()
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_start(fake_key_verification_event)
 
@@ -606,18 +775,17 @@
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.from_device = "ABCDEFGH"
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.short_authentication_string = ["emoji"]
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.accept_key_verification.return_value = make_awaitable(
-            Mock(spec=nio.ToDeviceError)
+        self.fake_matrix_client.accept_key_verification.return_value = Mock(
+            spec=nio.ToDeviceError
         )
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
 
         fake_sas = Mock()
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_start(fake_key_verification_event)
@@ -637,18 +805,15 @@
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.from_device = "ABCDEFGH"
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.short_authentication_string = ["emoji"]
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.accept_key_verification.return_value = make_awaitable()
-        self.fake_matrix_client.to_device.return_value = make_awaitable(
-            Mock(spec=nio.ToDeviceError)
-        )
+        self.fake_matrix_client.to_device.return_value = Mock(spec=nio.ToDeviceError)
 
         fake_sas = Mock()
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_start(fake_key_verification_event)
@@ -676,18 +841,14 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.confirm_short_auth_string.return_value = (
-            make_awaitable()
-        )
-
         fake_sas = Mock()
         fake_sas.get_emoji.return_value = [
             ("emoji1", "alt text1"),
             ("emoji2", "alt text2"),
         ]
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
@@ -705,16 +866,16 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.confirm_short_auth_string.return_value = make_awaitable(
-            Mock(spec=nio.ToDeviceError)
+        self.fake_matrix_client.confirm_short_auth_string.return_value = Mock(
+            spec=nio.ToDeviceError
         )
 
         fake_sas = Mock()
         fake_sas.get_emoji.return_value = [
             ("emoji1", "alt text1"),
             ("emoji2", "alt text2"),
         ]
@@ -734,16 +895,14 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
-
         fake_sas = Mock()
         fake_sas.verified_devices = ["HGFEDCBA"]
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_end(fake_key_verification_event)
@@ -757,16 +916,14 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
-
         fake_sas = Mock()
         fake_transactions_dict = {}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_end(fake_key_verification_event)
 
@@ -779,18 +936,16 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.to_device.return_value = make_awaitable()
-
         fake_sas = Mock()
-        fake_sas.get_mac.side_effect = key_verification_get_mac_raise_protocol_error
+        fake_sas.get_mac.side_effect = nio.exceptions.LocalProtocolError
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_end(fake_key_verification_event)
 
         # Check that we attempted to execute the command
@@ -802,44 +957,98 @@
         # Tests that the bot process messages in the room that contain a command
         fake_transaction_id = "fake transaction id"
 
         fake_key_verification_event = Mock(spec=nio.KeyVerificationStart)
         fake_key_verification_event.sender = "@some_other_fake_user:example.com"
         fake_key_verification_event.transaction_id = fake_transaction_id
 
-        self.fake_matrix_client.to_device.return_value = make_awaitable(
-            Mock(spec=nio.ToDeviceError)
-        )
+        self.fake_matrix_client.to_device.return_value = Mock(spec=nio.ToDeviceError)
 
         fake_sas = Mock()
         fake_transactions_dict = {fake_transaction_id: fake_sas}
         self.fake_matrix_client.key_verifications = fake_transactions_dict
 
         # Pretend that we received a text message event
         await self.callbacks.key_verification_end(fake_key_verification_event)
 
         # Check that we attempted to execute the command
         fake_sas.get_mac.assert_called_once_with()
         self.fake_matrix_client.to_device.assert_called_once_with(fake_sas.get_mac())
 
-    @patch.object(matrix_alertbot.callback.CommandFactory, "create", autospec=True)
-    async def test_unknown(self, fake_command_create: Mock) -> None:
-        """Tests the callback for RoomMessageText with the command prefix"""
-        # Tests that the bot process messages in the room that contain a command
-        fake_command = Mock(spec=BaseCommand)
-        fake_command_create.return_value = fake_command
+    @patch.object(matrix_alertbot.callback, "logger", autospec=True)
+    async def test_decryption_failure(self, fake_logger) -> None:
+        fake_megolm_event = Mock(spec=nio.MegolmEvent)
+        fake_megolm_event.sender = "@some_other_fake_user:example.com"
+        fake_megolm_event.event_id = "some event id"
+
+        await self.callbacks.decryption_failure(self.fake_room, fake_megolm_event)
+
+        fake_logger.error.assert_called_once()
+
+    @patch.object(matrix_alertbot.callback, "logger", autospec=True)
+    async def test_decryption_failure_in_unauthorized_room(self, fake_logger) -> None:
+        fake_megolm_event = Mock(spec=nio.MegolmEvent)
+        fake_megolm_event.sender = "@some_other_fake_user:example.com"
+        fake_megolm_event.event_id = "some event id"
 
-        fake_reaction_event = Mock(spec=nio.UnknownEvent)
-        fake_reaction_event.type = "m.reaction"
-        fake_reaction_event.event_id = "some event id"
-        fake_reaction_event.sender = "@some_other_fake_user:example.com"
-        fake_reaction_event.source = {}
+        self.fake_room.room_id = "!unauthorizedroom@example.com"
 
-        # Pretend that we received a text message event
-        await self.callbacks.unknown(self.fake_room, fake_reaction_event)
+        await self.callbacks.decryption_failure(self.fake_room, fake_megolm_event)
 
-        # Check that we attempted to execute the command
-        fake_command_create.assert_not_called()
+        fake_logger.error.assert_not_called()
+
+    async def test_unknown_message(self) -> None:
+        fake_room_unknown_event = Mock(spec=nio.RoomMessageUnknown)
+        fake_room_unknown_event.source = {
+            "content": {
+                "msgtype": "m.key.verification.request",
+                "methods": ["m.sas.v1"],
+            }
+        }
+        fake_room_unknown_event.event_id = "some event id"
+
+        await self.callbacks.unknown_message(self.fake_room, fake_room_unknown_event)
+
+        self.fake_matrix_client.room_send.assert_called_once_with(
+            self.fake_room.room_id,
+            "m.room.message",
+            {
+                "msgtype": "m.key.verification.ready",
+                "methods": ["m.sas.v1"],
+                "m.relates_to": {
+                    "rel_type": "m.reference",
+                    "event_id": fake_room_unknown_event.event_id,
+                },
+            },
+        )
+
+    async def test_unknown_message_with_msgtype_not_verification_request(self) -> None:
+        fake_room_unknown_event = Mock(spec=nio.RoomMessageUnknown)
+        fake_room_unknown_event.source = {
+            "content": {
+                "msgtype": "unknown",
+                "methods": ["m.sas.v1"],
+            }
+        }
+        fake_room_unknown_event.event_id = "some event id"
+
+        await self.callbacks.unknown_message(self.fake_room, fake_room_unknown_event)
+
+        self.fake_matrix_client.room_send.assert_not_called()
+
+    async def test_unknown_message_with_method_not_sas_v1(self) -> None:
+        fake_room_unknown_event = Mock(spec=nio.RoomMessageUnknown)
+        fake_room_unknown_event.source = {
+            "content": {
+                "msgtype": "m.key.verification.request",
+                "methods": [],
+            }
+        }
+        fake_room_unknown_event.event_id = "some event id"
+
+        await self.callbacks.unknown_message(self.fake_room, fake_room_unknown_event)
+
+        self.fake_matrix_client.room_send.assert_not_called()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `matrix-alertbot-0.1.6/tests/test_chat_functions.py` & `matrix_alertbot-0.2.0/tests/test_chat_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 import unittest
-from typing import Any, Dict, Optional
 from unittest.mock import Mock
 
 import nio
 
 from matrix_alertbot.chat_functions import (
     react_to_event,
     send_text_to_room,
     strip_fallback,
 )
 
-from tests.utils import make_awaitable
-
-
-async def send_room_raise_send_retry_error(
-    room_id: str,
-    message_type: str,
-    content: Dict[Any, Any],
-    tx_id: Optional[str] = None,
-    ignore_unverified_devices: bool = False,
-) -> nio.RoomSendResponse:
-    raise nio.SendRetryError
-
 
 class ChatFunctionsTestCase(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         pass
 
     def test_strip_fallback(self) -> None:
         fake_body = "> some message\n\nsome reply"
@@ -35,19 +22,20 @@
         fake_body = "some message"
         message = strip_fallback(fake_body)
         self.assertEqual(fake_body, message)
 
     async def test_react_to_event(self) -> None:
         fake_response = Mock(spec=nio.RoomSendResponse)
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send = Mock(return_value=make_awaitable(fake_response))
         fake_room_id = "!abcdefgh:example.com"
         fake_event_id = "some event id"
         fake_reaction_text = "some reaction"
 
+        fake_matrix_client.room_send.return_value = fake_response
+
         response = await react_to_event(
             fake_matrix_client, fake_room_id, fake_event_id, fake_reaction_text
         )
 
         fake_matrix_client.room_send.assert_called_once_with(
             fake_room_id,
             "m.reaction",
@@ -63,15 +51,15 @@
         self.assertEqual(fake_response, response)
 
     async def test_react_to_event_return_room_send_error(self) -> None:
         fake_response = Mock(spec=nio.RoomSendError)
         fake_response.message = "some error"
         fake_response.status_code = "some status code"
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send.return_value = make_awaitable(fake_response)
+        fake_matrix_client.room_send.return_value = fake_response
         fake_room_id = "!abcdefgh:example.com"
         fake_event_id = "some event id"
         fake_reaction_text = "some reaction"
 
         with self.assertRaises(nio.SendRetryError):
             await react_to_event(
                 fake_matrix_client, fake_room_id, fake_event_id, fake_reaction_text
@@ -89,19 +77,20 @@
             },
             ignore_unverified_devices=True,
         )
 
     async def test_send_text_to_room_as_notice(self) -> None:
         fake_response = Mock(spec=nio.RoomSendResponse)
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send = Mock(return_value=make_awaitable(fake_response))
         fake_room_id = "!abcdefgh:example.com"
         fake_plaintext_body = "some plaintext message"
         fake_html_body = "some html message"
 
+        fake_matrix_client.room_send.return_value = fake_response
+
         response = await send_text_to_room(
             fake_matrix_client, fake_room_id, fake_plaintext_body, fake_html_body
         )
 
         fake_matrix_client.room_send.assert_called_once_with(
             fake_room_id,
             "m.room.message",
@@ -114,19 +103,20 @@
             ignore_unverified_devices=True,
         )
         self.assertEqual(fake_response, response)
 
     async def test_send_text_to_room_as_message(self) -> None:
         fake_response = Mock(spec=nio.RoomSendResponse)
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send.return_value = make_awaitable(fake_response)
         fake_room_id = "!abcdefgh:example.com"
         fake_plaintext_body = "some plaintext message"
         fake_html_body = "some html message"
 
+        fake_matrix_client.room_send.return_value = fake_response
+
         response = await send_text_to_room(
             fake_matrix_client,
             fake_room_id,
             fake_plaintext_body,
             fake_html_body,
             notice=False,
         )
@@ -143,20 +133,21 @@
             ignore_unverified_devices=True,
         )
         self.assertEqual(fake_response, response)
 
     async def test_send_text_to_room_in_reply_to_event(self) -> None:
         fake_response = Mock(spec=nio.RoomSendResponse)
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send.return_value = make_awaitable(fake_response)
         fake_room_id = "!abcdefgh:example.com"
         fake_plaintext_body = "some plaintext message"
         fake_html_body = "some html message"
         fake_event_id = "some event id"
 
+        fake_matrix_client.room_send.return_value = fake_response
+
         response = await send_text_to_room(
             fake_matrix_client,
             fake_room_id,
             fake_plaintext_body,
             fake_html_body,
             reply_to_event_id=fake_event_id,
         )
@@ -173,15 +164,15 @@
             },
             ignore_unverified_devices=True,
         )
         self.assertEqual(fake_response, response)
 
     async def test_send_text_to_room_raise_send_retry_error(self) -> None:
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send.side_effect = send_room_raise_send_retry_error
+        fake_matrix_client.room_send.side_effect = nio.exceptions.SendRetryError
 
         fake_room_id = "!abcdefgh:example.com"
         fake_plaintext_body = "some plaintext message"
         fake_html_body = "some html message"
 
         with self.assertRaises(nio.SendRetryError):
             await send_text_to_room(
@@ -204,19 +195,20 @@
         )
 
     async def test_send_text_to_room_return_room_send_error(self) -> None:
         fake_response = Mock(spec=nio.RoomSendError)
         fake_response.status_code = "some status_code"
         fake_response.message = "some error"
         fake_matrix_client = Mock(spec=nio.AsyncClient)
-        fake_matrix_client.room_send.return_value = make_awaitable(fake_response)
         fake_room_id = "!abcdefgh:example.com"
         fake_plaintext_body = "some plaintext message"
         fake_html_body = "some html message"
 
+        fake_matrix_client.room_send.return_value = fake_response
+
         with self.assertRaises(nio.SendRetryError):
             await send_text_to_room(
                 fake_matrix_client,
                 fake_room_id,
                 fake_plaintext_body,
                 fake_html_body,
             )
```

### Comparing `matrix-alertbot-0.1.6/tests/test_command.py` & `matrix_alertbot-0.2.0/tests/test_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 )
 from matrix_alertbot.errors import (
     AlertmanagerError,
     AlertNotFoundError,
     SilenceNotFoundError,
 )
 
-from tests.utils import make_awaitable
-
 
 def cache_get_item(key: str) -> str:
     return {
         "some alert event id": "fingerprint1",
         "fingerprint1": "silence1",
     }[key]
 
@@ -80,16 +78,14 @@
 
 
 class CommandTestCase(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         # Create a Command object and give it some Mock'd objects to use
         self.fake_matrix_client = Mock(spec=nio.AsyncClient)
         self.fake_matrix_client.user = "@fake_user:example.com"
-        # Pretend that attempting to send a message is always successful
-        self.fake_matrix_client.room_send.return_value = make_awaitable()
 
         self.fake_cache = MagicMock(spec=Cache)
         self.fake_cache.__getitem__.side_effect = cache_get_item
         self.fake_cache.__contains__.return_value = True
 
         self.fake_alertmanager_client = Mock(spec=AlertmanagerClient)
         self.fake_alertmanager_client.create_or_update_silence.side_effect = (
```

### Comparing `matrix-alertbot-0.1.6/tests/test_config.py` & `matrix_alertbot-0.2.0/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
+import sys
 import unittest
 from datetime import timedelta
 from unittest.mock import Mock, patch
 
 import yaml
 
+import matrix_alertbot.config
 from matrix_alertbot.config import DEFAULT_REACTIONS, Config
 from matrix_alertbot.errors import (
     InvalidConfigError,
     ParseConfigError,
     RequiredConfigKeyError,
 )
 
@@ -34,33 +36,48 @@
     return True
 
 
 class ConfigTestCase(unittest.TestCase):
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
+    @patch.object(matrix_alertbot.config, "logger", autospec=True)
+    @patch.object(matrix_alertbot.config, "logging", autospec=True)
     def test_read_minimal_config(
-        self, fake_mkdir: Mock, fake_path_exists: Mock, fake_path_isdir: Mock
+        self,
+        fake_logging: Mock,
+        fake_logger: Mock,
+        fake_mkdir: Mock,
+        fake_path_exists: Mock,
+        fake_path_isdir: Mock,
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = Config(config_path)
 
         fake_path_isdir.assert_called_once_with("data/store")
         fake_path_exists.assert_called_once_with("data/store")
         fake_mkdir.assert_called_once_with("data/store")
 
-        self.assertEqual("@fakes_user:matrix.example.com", config.user_id)
-        self.assertEqual("password", config.user_password)
-        self.assertIsNone(config.user_token)
-        self.assertIsNone(config.device_id)
+        fake_logger.setLevel.assert_called_once_with("DEBUG")
+        fake_logger.addHandler.assert_called_once()
+        fake_logging.StreamHandler.return_value.setLevel.assert_called_once_with("INFO")
+        fake_logging.StreamHandler.assert_called_once_with(sys.stdout)
+
+        self.assertEqual({"@fakes_user:matrix.example.com"}, config.user_ids)
+        self.assertEqual(1, len(config.accounts))
+        self.assertEqual("password", config.accounts[0].password)
+        self.assertIsNone(config.accounts[0].token)
+        self.assertIsNone(config.accounts[0].device_id)
         self.assertEqual("matrix-alertbot", config.device_name)
-        self.assertEqual("https://matrix.example.com", config.homeserver_url)
+        self.assertEqual(
+            "https://matrix.example.com", config.accounts[0].homeserver_url
+        )
         self.assertEqual(["!abcdefgh:matrix.example.com"], config.allowed_rooms)
         self.assertEqual(DEFAULT_REACTIONS, config.allowed_reactions)
 
         self.assertEqual("0.0.0.0", config.address)
         self.assertEqual(8080, config.port)
         self.assertIsNone(config.socket)
 
@@ -75,34 +92,57 @@
         self.assertIsNone(config.template_dir)
 
         self.assertEqual("!alert ", config.command_prefix)
 
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
+    @patch.object(matrix_alertbot.config, "logger", autospec=True)
+    @patch.object(matrix_alertbot.config, "logging", autospec=True)
     def test_read_full_config(
-        self, fake_mkdir: Mock, fake_path_exists: Mock, fake_path_isdir: Mock
+        self,
+        fake_logging: Mock,
+        fake_logger: Mock,
+        fake_mkdir: Mock,
+        fake_path_exists: Mock,
+        fake_path_isdir: Mock,
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.full.yml")
         config = Config(config_path)
 
         fake_path_isdir.assert_called_once_with("data/store")
         fake_path_exists.assert_called_once_with("data/store")
         fake_mkdir.assert_called_once_with("data/store")
 
-        self.assertEqual("@fakes_user:matrix.example.com", config.user_id)
-        self.assertEqual("password", config.user_password)
-        self.assertIsNone(config.user_token)
-        self.assertEqual("token.json", config.user_token_file)
-        self.assertEqual("ABCDEFGHIJ", config.device_id)
+        fake_logger.setLevel.assert_called_once_with("DEBUG")
+        fake_logger.addHandler.assert_called_once()
+        fake_logging.FileHandler.return_value.setLevel.assert_called_once_with("INFO")
+        fake_logging.FileHandler.assert_called_once_with("fake.log")
+
+        self.assertEqual(
+            {"@fakes_user:matrix.example.com", "@other_user:matrix.domain.tld"},
+            config.user_ids,
+        )
+        self.assertEqual(2, len(config.accounts))
+        self.assertEqual("password", config.accounts[0].password)
+        self.assertIsNone(config.accounts[0].token)
+        self.assertEqual("fake_token.json", config.accounts[0].token_file)
+        self.assertEqual("ABCDEFGHIJ", config.accounts[0].device_id)
+        self.assertEqual(
+            "https://matrix.example.com", config.accounts[0].homeserver_url
+        )
+        self.assertIsNone(config.accounts[1].password)
+        self.assertEqual("token", config.accounts[1].token)
+        self.assertEqual("other_token.json", config.accounts[1].token_file)
+        self.assertEqual("KLMNOPQRST", config.accounts[1].device_id)
+        self.assertEqual("https://matrix.domain.tld", config.accounts[1].homeserver_url)
         self.assertEqual("fake_device_name", config.device_name)
-        self.assertEqual("https://matrix.example.com", config.homeserver_url)
         self.assertEqual(["!abcdefgh:matrix.example.com"], config.allowed_rooms)
         self.assertEqual({"🤫", "😶", "🤐"}, config.allowed_reactions)
 
         self.assertIsNone(config.address)
         self.assertIsNone(config.port)
         self.assertEqual("matrix-alertbot.socket", config.socket)
 
@@ -146,15 +186,15 @@
         self, fake_mkdir: Mock, fake_path_exists: Mock, fake_path_isdir: Mock
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = DummyConfig(config_path)
-        del config.config_dict["matrix"]["user_id"]
+        del config.config_dict["matrix"]["accounts"]
 
         with self.assertRaises(RequiredConfigKeyError):
             config._parse_config_values()
 
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
@@ -162,15 +202,15 @@
         self, fake_mkdir: Mock, fake_path_exists: Mock, fake_path_isdir: Mock
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = DummyConfig(config_path)
-        del config.config_dict["matrix"]["user_password"]
+        del config.config_dict["matrix"]["accounts"][0]["password"]
 
         with self.assertRaises(RequiredConfigKeyError):
             config._parse_config_values()
 
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
@@ -178,15 +218,15 @@
         self, fake_mkdir: Mock, fake_path_exists: Mock, fake_path_isdir: Mock
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = DummyConfig(config_path)
-        del config.config_dict["matrix"]["url"]
+        del config.config_dict["matrix"]["accounts"][0]["url"]
 
         with self.assertRaises(RequiredConfigKeyError):
             config._parse_config_values()
 
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
@@ -275,35 +315,35 @@
     ) -> None:
         fake_path_isdir.return_value = False
         fake_path_exists.return_value = False
 
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = DummyConfig(config_path)
 
-        config.config_dict["matrix"]["user_id"] = ""
+        config.config_dict["matrix"]["accounts"][0]["id"] = ""
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
-        config.config_dict["matrix"]["user_id"] = "@fake_user"
+        config.config_dict["matrix"]["accounts"][0]["id"] = "@fake_user"
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
-        config.config_dict["matrix"]["user_id"] = "@fake_user:"
+        config.config_dict["matrix"]["accounts"][0]["id"] = "@fake_user:"
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
-        config.config_dict["matrix"]["user_id"] = ":matrix.example.com"
+        config.config_dict["matrix"]["accounts"][0]["id"] = ":matrix.example.com"
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
-        config.config_dict["matrix"]["user_id"] = "@:matrix.example.com"
+        config.config_dict["matrix"]["accounts"][0]["id"] = "@:matrix.example.com"
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
-        config.config_dict["matrix"]["user_id"] = "@:"
+        config.config_dict["matrix"]["accounts"][0]["id"] = "@:"
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
     @patch("os.path.isdir")
     @patch("os.path.exists")
     @patch("os.mkdir")
     def test_parse_config_with_both_webhook_socket_and_address(
@@ -315,10 +355,66 @@
         config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.minimal.yml")
         config = DummyConfig(config_path)
         config.config_dict["webhook"]["socket"] = "matrix-alertbot.socket"
 
         with self.assertRaises(InvalidConfigError):
             config._parse_config_values()
 
+    @patch("os.path.isdir")
+    @patch("os.path.exists")
+    @patch("os.mkdir")
+    @patch.object(matrix_alertbot.config, "logger")
+    def test_parse_config_with_both_logging_disabled(
+        self,
+        fake_logger: Mock,
+        fake_mkdir: Mock,
+        fake_path_exists: Mock,
+        fake_path_isdir: Mock,
+    ) -> None:
+        fake_path_isdir.return_value = False
+        fake_path_exists.return_value = False
+
+        config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.full.yml")
+        config = DummyConfig(config_path)
+        config.config_dict["logging"]["file_logging"]["enabled"] = False
+        config.config_dict["logging"]["console_logging"]["enabled"] = False
+
+        config._parse_config_values()
+
+        fake_logger.addHandler.assert_not_called()
+        fake_logger.setLevel.assert_called_once_with("DEBUG")
+
+    @patch("os.path.isdir")
+    @patch("os.path.exists")
+    @patch("os.mkdir")
+    @patch.object(matrix_alertbot.config, "logger", autospec=True)
+    @patch.object(matrix_alertbot.config, "logging", autospec=True)
+    def test_parse_config_with_level_logging_different(
+        self,
+        fake_logging: Mock,
+        fake_logger: Mock,
+        fake_mkdir: Mock,
+        fake_path_exists: Mock,
+        fake_path_isdir: Mock,
+    ) -> None:
+        fake_path_isdir.return_value = False
+        fake_path_exists.return_value = False
+
+        config_path = os.path.join(CONFIG_RESOURCES_DIR, "config.full.yml")
+        config = DummyConfig(config_path)
+        config.config_dict["logging"]["file_logging"]["enabled"] = True
+        config.config_dict["logging"]["file_logging"]["level"] = "WARN"
+        config.config_dict["logging"]["console_logging"]["enabled"] = True
+        config.config_dict["logging"]["console_logging"]["level"] = "ERROR"
+
+        config._parse_config_values()
+
+        self.assertEqual(2, fake_logger.addHandler.call_count)
+        fake_logger.setLevel.assert_called_once_with("DEBUG")
+        fake_logging.FileHandler.return_value.setLevel.assert_called_once_with("WARN")
+        fake_logging.StreamHandler.return_value.setLevel.assert_called_once_with(
+            "ERROR"
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `matrix-alertbot-0.1.6/tests/test_webhook.py` & `matrix_alertbot-0.2.0/tests/test_webhook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import unittest
 from typing import Dict
 from unittest.mock import Mock, call, patch
 
 import aiohttp.test_utils
 import nio
-from aiohttp import web
+from aiohttp import web, web_request
 from diskcache import Cache
-from nio import LocalProtocolError, RoomSendResponse
 
 import matrix_alertbot.webhook
+from matrix_alertbot.alert import Alert, AlertRenderer
 from matrix_alertbot.alertmanager import AlertmanagerClient
 from matrix_alertbot.config import Config
 from matrix_alertbot.errors import (
     AlertmanagerError,
+    MatrixClientError,
     SilenceExtendError,
     SilenceNotFoundError,
 )
-from matrix_alertbot.webhook import Webhook
-
-
-def send_text_to_room_raise_error(
-    client: nio.AsyncClient, room_id: str, plaintext: str, html: str, notice: bool
-) -> RoomSendResponse:
-    raise LocalProtocolError
+from matrix_alertbot.matrix import MatrixClientPool
+from matrix_alertbot.webhook import Webhook, create_alert
 
 
 def update_silence_raise_silence_not_found(fingerprint: str) -> str:
     raise SilenceNotFoundError
 
 
 def update_silence_raise_silence_extend_error(fingerprint: str) -> str:
@@ -36,56 +32,70 @@
 def update_silence_raise_alertmanager_error(fingerprint: str) -> str:
     raise AlertmanagerError
 
 
 class WebhookApplicationTestCase(aiohttp.test_utils.AioHTTPTestCase):
     async def get_application(self) -> web.Application:
         self.fake_matrix_client = Mock(spec=nio.AsyncClient)
+        self.fake_matrix_client_pool = Mock(spec=MatrixClientPool)
+        self.fake_matrix_client_pool.matrix_client = self.fake_matrix_client
         self.fake_alertmanager_client = Mock(spec=AlertmanagerClient)
+        self.fake_alert_renderer = Mock(spec=AlertRenderer)
         self.fake_cache = Mock(spec=Cache)
 
         self.fake_room_id = "!abcdefg:example.com"
 
         self.fake_config = Mock(spec=Config)
         self.fake_config.port = aiohttp.test_utils.unused_port()
         self.fake_config.address = "localhost"
         self.fake_config.socket = "webhook.sock"
         self.fake_config.allowed_rooms = [self.fake_room_id]
         self.fake_config.cache_expire_time = 0
         self.fake_config.template_dir = None
 
+        self.fake_request = Mock(spec=web_request.Request)
+        self.fake_request.app = {
+            "alertmanager_client": self.fake_alertmanager_client,
+            "alert_renderer": self.fake_alert_renderer,
+            "matrix_client_pool": self.fake_matrix_client_pool,
+            "cache": self.fake_cache,
+            "config": self.fake_config,
+        }
+
+        self.fake_alert_1 = {
+            "fingerprint": "fingerprint1",
+            "generatorURL": "http://example.com/alert1",
+            "status": "firing",
+            "labels": {
+                "alertname": "alert1",
+                "severity": "critical",
+                "job": "job1",
+            },
+            "annotations": {"description": "some description1"},
+        }
+        self.fake_alert_2 = {
+            "fingerprint": "fingerprint2",
+            "generatorURL": "http://example.com/alert2",
+            "status": "resolved",
+            "labels": {
+                "alertname": "alert2",
+                "severity": "warning",
+                "job": "job2",
+            },
+            "annotations": {"description": "some description2"},
+        }
         self.fake_alerts = {
             "alerts": [
-                {
-                    "fingerprint": "fingerprint1",
-                    "generatorURL": "http://example.com/alert1",
-                    "status": "firing",
-                    "labels": {
-                        "alertname": "alert1",
-                        "severity": "critical",
-                        "job": "job1",
-                    },
-                    "annotations": {"description": "some description1"},
-                },
-                {
-                    "fingerprint": "fingerprint2",
-                    "generatorURL": "http://example.com/alert2",
-                    "status": "resolved",
-                    "labels": {
-                        "alertname": "alert2",
-                        "severity": "warning",
-                        "job": "job2",
-                    },
-                    "annotations": {"description": "some description2"},
-                },
+                self.fake_alert_1,
+                self.fake_alert_2,
             ]
         }
 
         webhook = Webhook(
-            self.fake_matrix_client,
+            self.fake_matrix_client_pool,
             self.fake_alertmanager_client,
             self.fake_cache,
             self.fake_config,
         )
         return webhook.app
 
     @patch.object(matrix_alertbot.webhook, "send_text_to_room")
@@ -306,21 +316,22 @@
             error_msg = await response.text()
 
         self.assertEqual("Invalid alert: {}.", error_msg)
         fake_send_text_to_room.assert_not_called()
         self.fake_cache.set.assert_not_called()
         self.fake_cache.delete.assert_not_called()
 
+    @patch.object(matrix_alertbot.webhook, "logger", autospec=True)
     @patch.object(
         matrix_alertbot.webhook,
         "send_text_to_room",
-        side_effect=send_text_to_room_raise_error,
+        side_effect=nio.exceptions.LocalProtocolError("Local protocol error"),
     )
     async def test_post_alerts_raise_send_error(
-        self, fake_send_text_to_room: Mock
+        self, fake_send_text_to_room: Mock, fake_logger: Mock
     ) -> None:
         self.fake_alertmanager_client.update_silence.side_effect = (
             update_silence_raise_silence_not_found
         )
 
         data = self.fake_alerts
         async with self.client.request(
@@ -333,14 +344,186 @@
             "An error occured when sending alert with fingerprint 'fingerprint1' to Matrix room.",
             error_msg,
         )
         fake_send_text_to_room.assert_called_once()
         self.fake_cache.set.assert_not_called()
         self.fake_cache.delete.assert_called_once_with("fingerprint1")
 
+        fake_logger.error.assert_called_once_with(
+            "Unable to send alert fingerprint1 to Matrix room !abcdefg:example.com: Local protocol error"
+        )
+
+    @patch.object(matrix_alertbot.webhook, "logger", autospec=True)
+    @patch.object(
+        matrix_alertbot.webhook,
+        "create_alert",
+        side_effect=MatrixClientError("Matrix client error"),
+    )
+    async def test_post_alerts_raise_matrix_client_error(
+        self, fake_create_alert: Mock, fake_logger: Mock
+    ) -> None:
+        self.fake_alertmanager_client.update_silence.side_effect = (
+            update_silence_raise_silence_not_found
+        )
+
+        data = self.fake_alerts
+        async with self.client.request(
+            "POST", f"/alerts/{self.fake_room_id}", json=data
+        ) as response:
+            self.assertEqual(500, response.status)
+            error_msg = await response.text()
+
+        self.assertEqual(
+            "An error occured when sending alert with fingerprint 'fingerprint1' to Matrix room.",
+            error_msg,
+        )
+        fake_create_alert.assert_called_once()
+
+        fake_logger.error.assert_called_once_with(
+            "Unable to send alert fingerprint1 to Matrix room !abcdefg:example.com: Matrix client error"
+        )
+
+    @patch.object(matrix_alertbot.webhook, "logger", autospec=True)
+    @patch.object(
+        matrix_alertbot.webhook,
+        "send_text_to_room",
+        side_effect=Exception("Exception"),
+    )
+    async def test_post_alerts_raise_exception(
+        self, fake_send_text_to_room: Mock, fake_logger: Mock
+    ) -> None:
+        self.fake_alertmanager_client.update_silence.side_effect = (
+            update_silence_raise_silence_not_found
+        )
+
+        data = self.fake_alerts
+        async with self.client.request(
+            "POST", f"/alerts/{self.fake_room_id}", json=data
+        ) as response:
+            self.assertEqual(500, response.status)
+            error_msg = await response.text()
+
+        self.assertEqual(
+            "An exception occured when sending alert with fingerprint 'fingerprint1' to Matrix room.",
+            error_msg,
+        )
+        fake_send_text_to_room.assert_called_once()
+        self.fake_cache.set.assert_not_called()
+        self.fake_cache.delete.assert_called_once_with("fingerprint1")
+
+        fake_logger.error.assert_called_once_with(
+            "Unable to send alert fingerprint1 to Matrix room !abcdefg:example.com: Exception"
+        )
+
+    async def test_create_alert_update_silence(self) -> None:
+        fake_alert = Mock(spec=Alert)
+        fake_alert.firing = True
+        fake_alert.fingerprint = "fingerprint"
+
+        await create_alert(fake_alert, self.fake_room_id, self.fake_request)
+
+        self.fake_alertmanager_client.update_silence.assert_called_once_with(
+            fake_alert.fingerprint
+        )
+        self.fake_alert_renderer.render.assert_not_called()
+
+    @patch.object(matrix_alertbot.webhook, "send_text_to_room", autospec=True)
+    async def test_create_alert_with_silence_not_found_error(
+        self, fake_send_text_to_room: Mock
+    ) -> None:
+        fake_alert = Mock(spec=Alert)
+        fake_alert.firing = True
+        fake_alert.fingerprint = "fingerprint"
+
+        self.fake_alertmanager_client.update_silence.side_effect = SilenceNotFoundError
+
+        await create_alert(fake_alert, self.fake_room_id, self.fake_request)
+
+        self.fake_alertmanager_client.update_silence.assert_called_once_with(
+            fake_alert.fingerprint
+        )
+        self.fake_alert_renderer.render.assert_has_calls(
+            [call(fake_alert, html=False), call(fake_alert, html=True)]
+        )
+
+        fake_send_text_to_room.assert_called_once()
+
+        self.fake_cache.set.assert_called_once_with(
+            fake_send_text_to_room.return_value.event_id,
+            fake_alert.fingerprint,
+            expire=self.fake_config.cache_expire_time,
+        )
+        self.fake_cache.delete.assert_called_once_with(fake_alert.fingerprint)
+
+    @patch.object(matrix_alertbot.webhook, "send_text_to_room", autospec=True)
+    async def test_create_alert_with_silence_extend_error(
+        self, fake_send_text_to_room: Mock
+    ) -> None:
+        fake_alert = Mock(spec=Alert)
+        fake_alert.firing = True
+        fake_alert.fingerprint = "fingerprint"
+
+        self.fake_alertmanager_client.update_silence.side_effect = SilenceExtendError
+
+        await create_alert(fake_alert, self.fake_room_id, self.fake_request)
+
+        self.fake_alertmanager_client.update_silence.assert_called_once_with(
+            fake_alert.fingerprint
+        )
+        self.fake_alert_renderer.render.assert_has_calls(
+            [call(fake_alert, html=False), call(fake_alert, html=True)]
+        )
+
+        fake_send_text_to_room.assert_called_once()
+
+        self.fake_cache.set.assert_called_once_with(
+            fake_send_text_to_room.return_value.event_id,
+            fake_alert.fingerprint,
+            expire=self.fake_config.cache_expire_time,
+        )
+        self.fake_cache.delete.assert_not_called()
+
+    @patch.object(matrix_alertbot.webhook, "send_text_to_room", autospec=True)
+    async def test_create_alert_not_firing(self, fake_send_text_to_room: Mock) -> None:
+        fake_alert = Mock(spec=Alert)
+        fake_alert.firing = False
+        fake_alert.fingerprint = "fingerprint"
+
+        await create_alert(fake_alert, self.fake_room_id, self.fake_request)
+
+        self.fake_alertmanager_client.update_silence.assert_not_called()
+        self.fake_alert_renderer.render.assert_has_calls(
+            [call(fake_alert, html=False), call(fake_alert, html=True)]
+        )
+
+        fake_send_text_to_room.assert_called_once()
+
+        self.fake_cache.set.assert_not_called()
+        self.fake_cache.delete.assert_called_once_with(fake_alert.fingerprint)
+
+    @patch.object(matrix_alertbot.webhook, "send_text_to_room", autospec=True)
+    async def test_create_alert_not_firing_raise_matrix_client_error(
+        self, fake_send_text_to_room: Mock
+    ) -> None:
+        fake_alert = Mock(spec=Alert)
+        fake_alert.firing = False
+        fake_alert.fingerprint = "fingerprint"
+
+        self.fake_matrix_client_pool.matrix_client = None
+
+        with self.assertRaises(MatrixClientError):
+            await create_alert(fake_alert, self.fake_room_id, self.fake_request)
+
+        self.fake_alertmanager_client.update_silence.assert_not_called()
+        self.fake_alert_renderer.render.assert_has_calls(
+            [call(fake_alert, html=False), call(fake_alert, html=True)]
+        )
+
+        fake_send_text_to_room.assert_not_called()
+
     async def test_health(self) -> None:
         async with self.client.request("GET", "/health") as response:
             self.assertEqual(200, response.status)
 
     async def test_metrics(self) -> None:
         async with self.client.request("GET", "/metrics") as response:
             self.assertEqual(200, response.status)
```

