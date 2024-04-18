# Comparing `tmp/skip-django-pynotify-0.5.5.2.tar.gz` & `tmp/skip_django_pynotify-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pynotify-0.5.5.2.tar", last modified: Mon Apr 17 11:54:22 2023, max compression
+gzip compressed data, was "skip_django_pynotify-0.6.0.tar", last modified: Thu Apr 18 14:53:05 2024, max compression
```

## Comparing `skip-django-pynotify-0.5.5.2.tar` & `skip_django_pynotify-0.6.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.423822 skip-django-pynotify-0.5.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/example_project.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/extra_tips.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.423822 skip-django-pynotify-0.5.5.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/images/pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.419822 skip-django-pynotify-0.5.5.2/pynotify/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.419822 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0002_notification_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0003_related_object_name_not_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0004_add_admin_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0005_adminnotificationtemplate_is_active.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0006_add_send_push.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0007_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0008_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0009_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-17 11:54:22.431822 skip-django-pynotify-0.5.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.062456 skip_django_pynotify-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3648 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/example_project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/extra_tips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.062456 skip_django_pynotify-0.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/images/pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/pynotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.058456 skip_django_pynotify-0.6.0/pynotify/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.058456 skip_django_pynotify-0.6.0/pynotify/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/pynotify/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/pynotify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0002_notification_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0003_related_object_name_not_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0004_add_admin_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0005_adminnotificationtemplate_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0006_add_send_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0007_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0008_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/0009_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11599 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/pynotify/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 14:53:05.070456 skip_django_pynotify-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 14:53:01.000000 skip_django_pynotify-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:05.066456 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-18 14:53:05.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-18 14:53:05.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:53:05.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:53:04.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 14:53:05.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 14:53:05.000000 skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/top_level.txt
```

### Comparing `skip-django-pynotify-0.5.5.2/CONTRIBUTING.rst` & `skip_django_pynotify-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/HISTORY.rst` & `skip_django_pynotify-0.6.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/LICENSE` & `skip_django_pynotify-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/PKG-INFO` & `skip_django_pynotify-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pynotify
-Version: 0.5.5.2
+Version: 0.6.0
 Summary: General purpose notification library for Django
 Home-page: https://github.com/skip-pay/django-pynotify
 Author: Ondřej Kulatý
 Author-email: kulaty.o@gmail.com
 License: MIT license
 Keywords: django-pynotify
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: beautifulsoup4>=4.8.0
+Requires-Dist: celery>=4.2.0
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: lxml>=4.6.2
 
 ===============
 Django PyNotify
 ===============
 
 
 .. image:: https://img.shields.io/pypi/v/django-pynotify.svg
```

### Comparing `skip-django-pynotify-0.5.5.2/README.rst` & `skip_django_pynotify-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/Makefile` & `skip_django_pynotify-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/conf.py` & `skip_django_pynotify-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/configuration.rst` & `skip_django_pynotify-0.6.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/example_project.rst` & `skip_django_pynotify-0.6.0/docs/example_project.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/extra_tips.rst` & `skip_django_pynotify-0.6.0/docs/extra_tips.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/images/pipeline.svg` & `skip_django_pynotify-0.6.0/docs/images/pipeline.svg`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/installation.rst` & `skip_django_pynotify-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/reference.rst` & `skip_django_pynotify-0.6.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/docs/usage.rst` & `skip_django_pynotify-0.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/config.py` & `skip_django_pynotify-0.6.0/pynotify/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/handlers.py` & `skip_django_pynotify-0.6.0/pynotify/handlers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/helpers.py` & `skip_django_pynotify-0.6.0/pynotify/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from importlib import import_module
 from pydoc import locate
 
 from bs4 import BeautifulSoup
 from django.apps import apps
 from django.core.exceptions import ImproperlyConfigured
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from .config import settings
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.mo` & `skip_django_pynotify-0.6.0/pynotify/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.po` & `skip_django_pynotify-0.6.0/pynotify/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/migrations/0001_initial.py` & `skip_django_pynotify-0.6.0/pynotify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/migrations/0004_add_admin_template.py` & `skip_django_pynotify-0.6.0/pynotify/migrations/0004_add_admin_template.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/migrations/0008_migration.py` & `skip_django_pynotify-0.6.0/pynotify/migrations/0008_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/models.py` & `skip_django_pynotify-0.6.0/pynotify/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,17 @@
     def _render(self, field):
         return self.template.render(field, self.context)
 
     def clean_extra_data(self):
         return self._clean_json_value(self.extra_data)
 
     def clean(self):
+        if self.is_adding:
+            return
+
         keys = set(self.extra_data or {}) & set(obj.name for obj in self.related_objects.all() if obj.name)
         if keys:
             raise ValidationError('Related objects and extra data contain same key(s): {}'.format(', '.join(keys)))
 
     @cached_property
     def related_objects_dict(self):
         """
```

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/notify.py` & `skip_django_pynotify-0.6.0/pynotify/notify.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/receivers.py` & `skip_django_pynotify-0.6.0/pynotify/receivers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/pynotify/serializers.py` & `skip_django_pynotify-0.6.0/pynotify/serializers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.2/setup.py` & `skip_django_pynotify-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     'beautifulsoup4 >=4.8.0',
     'celery >= 4.2.0',
-    'django ~= 3.0',
-    'skip-django-chamber >= 0.6.16.3',
+    'django>=4.2',
+    'skip-django-chamber>=0.7.2',
     'lxml >= 4.6.2',
 ]
 
 setup(
     python_requires=">=3.6",
     author="Ondřej Kulatý",
     author_email='kulaty.o@gmail.com',
@@ -40,10 +40,10 @@
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='django-pynotify',
     name='skip-django-pynotify',
     packages=find_packages(include=['pynotify']),
     url='https://github.com/skip-pay/django-pynotify',
-    version='0.5.5.2',
+    version='0.6.0',
     zip_safe=False,
 )
```

### Comparing `skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/PKG-INFO` & `skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pynotify
-Version: 0.5.5.2
+Version: 0.6.0
 Summary: General purpose notification library for Django
 Home-page: https://github.com/skip-pay/django-pynotify
 Author: Ondřej Kulatý
 Author-email: kulaty.o@gmail.com
 License: MIT license
 Keywords: django-pynotify
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: beautifulsoup4>=4.8.0
+Requires-Dist: celery>=4.2.0
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: lxml>=4.6.2
 
 ===============
 Django PyNotify
 ===============
 
 
 .. image:: https://img.shields.io/pypi/v/django-pynotify.svg
```

### Comparing `skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/SOURCES.txt` & `skip_django_pynotify-0.6.0/skip_django_pynotify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

