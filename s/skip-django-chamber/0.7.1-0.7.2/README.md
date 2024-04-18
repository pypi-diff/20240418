# Comparing `tmp/skip-django-chamber-0.7.1.tar.gz` & `tmp/skip_django_chamber-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-chamber-0.7.1.tar", last modified: Tue Apr  9 15:11:45 2024, max compression
+gzip compressed data, was "skip_django_chamber-0.7.2.tar", last modified: Thu Apr 18 11:50:23 2024, max compression
```

## Comparing `skip-django-chamber-0.7.1.tar` & `skip_django_chamber-0.7.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.015735 skip-django-chamber-0.7.1/chamber/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/contrib/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/contrib/auth_token/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/formatters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/initdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/makemessages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/batch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/changed_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/models/humanized_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/humanized_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/multidomains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/multidomains/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/urlresolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/storages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/storages/boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/utils/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/migrations/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 15:11:45.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.776338 skip_django_chamber-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-18 11:50:23.776338 skip_django_chamber-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.760338 skip_django_chamber-0.7.2/chamber/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/contrib/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/contrib/auth_token/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/forms/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.764338 skip_django_chamber-0.7.2/chamber/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/management/commands/initdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/management/commands/makemessages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/batch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/changed_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/models/humanized_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/humanized_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/models/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.768338 skip_django_chamber-0.7.2/chamber/multidomains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.772338 skip_django_chamber-0.7.2/chamber/multidomains/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/auth/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/auth/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/multidomains/urlresolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.772338 skip_django_chamber-0.7.2/chamber/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/storages/boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.772338 skip_django_chamber-0.7.2/chamber/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.772338 skip_django_chamber-0.7.2/chamber/utils/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/migrations/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/chamber/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:50:23.776338 skip_django_chamber-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 11:50:20.000000 skip_django_chamber-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:50:23.772338 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-18 11:50:23.000000 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-18 11:50:23.000000 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:50:23.000000 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 11:50:23.000000 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 11:50:23.000000 skip_django_chamber-0.7.2/skip_django_chamber.egg-info/top_level.txt
```

### Comparing `skip-django-chamber-0.7.1/LICENSE` & `skip_django_chamber-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/PKG-INFO` & `skip_django_chamber-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-chamber
-Version: 0.7.1
+Version: 0.7.2
 Summary: Utilities library meant as a complement to django-is-core.
 Home-page: http://github.com/skip-pay/django-chamber
 Author: Lubos Matl, Oskar Hollmann
 Author-email: matllubos@gmail.com, oskar@hollmann.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: django<5.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: Unidecode>=1.1.1
 Requires-Dist: pyprind>=2.11.2
 Requires-Dist: python-magic>=0.4.27
 Provides-Extra: boto3storage
 Requires-Dist: django-storages<2.0; extra == "boto3storage"
 Requires-Dist: boto3; extra == "boto3storage"
```

### Comparing `skip-django-chamber-0.7.1/README.md` & `skip_django_chamber-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/commands/__init__.py` & `skip_django_chamber-0.7.2/chamber/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/config.py` & `skip_django_chamber-0.7.2/chamber/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/formatters/__init__.py` & `skip_django_chamber-0.7.2/chamber/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/forms/fields.py` & `skip_django_chamber-0.7.2/chamber/forms/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/forms/validators.py` & `skip_django_chamber-0.7.2/chamber/forms/validators.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/importers/__init__.py` & `skip_django_chamber-0.7.2/chamber/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.mo` & `skip_django_chamber-0.7.2/chamber/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.po` & `skip_django_chamber-0.7.2/chamber/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/management/commands/makemessages.py` & `skip_django_chamber-0.7.2/chamber/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/base.py` & `skip_django_chamber-0.7.2/chamber/models/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/batch_iterator.py` & `skip_django_chamber-0.7.2/chamber/models/batch_iterator.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/changed_fields.py` & `skip_django_chamber-0.7.2/chamber/models/changed_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/dispatchers.py` & `skip_django_chamber-0.7.2/chamber/models/dispatchers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/fields.py` & `skip_django_chamber-0.7.2/chamber/models/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/models/handlers.py` & `skip_django_chamber-0.7.2/chamber/models/handlers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/multidomains/auth/backends.py` & `skip_django_chamber-0.7.2/chamber/multidomains/auth/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/multidomains/auth/middleware.py` & `skip_django_chamber-0.7.2/chamber/multidomains/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/multidomains/domain.py` & `skip_django_chamber-0.7.2/chamber/multidomains/domain.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/multidomains/urlresolvers.py` & `skip_django_chamber-0.7.2/chamber/multidomains/urlresolvers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/patch.py` & `skip_django_chamber-0.7.2/chamber/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/shortcuts.py` & `skip_django_chamber-0.7.2/chamber/shortcuts.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/storages/boto3.py` & `skip_django_chamber-0.7.2/chamber/storages/boto3.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/__init__.py` & `skip_django_chamber-0.7.2/chamber/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/datastructures.py` & `skip_django_chamber-0.7.2/chamber/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/datetimes.py` & `skip_django_chamber-0.7.2/chamber/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/decorators.py` & `skip_django_chamber-0.7.2/chamber/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/json.py` & `skip_django_chamber-0.7.2/chamber/utils/json.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/logging.py` & `skip_django_chamber-0.7.2/chamber/utils/logging.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/migrations/fixtures.py` & `skip_django_chamber-0.7.2/chamber/utils/migrations/fixtures.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/tqdm.py` & `skip_django_chamber-0.7.2/chamber/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/chamber/utils/transaction.py` & `skip_django_chamber-0.7.2/chamber/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.1/setup.py` & `skip_django_chamber-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
     ],
     install_requires=[
-        'django>=2.2, <5.0',
+        'django>=4.2',
         'Unidecode>=1.1.1',
         'pyprind>=2.11.2',
         'python-magic>=0.4.27'
     ],
     extras_require={
         'boto3storage': ['django-storages<2.0', 'boto3'],
     },
```

### Comparing `skip-django-chamber-0.7.1/skip_django_chamber.egg-info/PKG-INFO` & `skip_django_chamber-0.7.2/skip_django_chamber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-chamber
-Version: 0.7.1
+Version: 0.7.2
 Summary: Utilities library meant as a complement to django-is-core.
 Home-page: http://github.com/skip-pay/django-chamber
 Author: Lubos Matl, Oskar Hollmann
 Author-email: matllubos@gmail.com, oskar@hollmann.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: django<5.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: Unidecode>=1.1.1
 Requires-Dist: pyprind>=2.11.2
 Requires-Dist: python-magic>=0.4.27
 Provides-Extra: boto3storage
 Requires-Dist: django-storages<2.0; extra == "boto3storage"
 Requires-Dist: boto3; extra == "boto3storage"
```

### Comparing `skip-django-chamber-0.7.1/skip_django_chamber.egg-info/SOURCES.txt` & `skip_django_chamber-0.7.2/skip_django_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

