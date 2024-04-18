# Comparing `tmp/skip-django-GDPR-0.2.23.2.tar.gz` & `tmp/skip_django_gdpr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-GDPR-0.2.23.2.tar", last modified: Tue Jan 17 15:58:17 2023, max compression
+gzip compressed data, was "skip_django_gdpr-0.3.0.tar", last modified: Thu Apr 18 14:45:58 2024, max compression
```

## Comparing `skip-django-GDPR-0.2.23.2.tar` & `skip_django_gdpr-0.3.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/generic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/gis.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/hash_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/local/cs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20592 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/anonymizers/model_anonymizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/ipcypher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.013001 skip-django-GDPR-0.2.23.2/gdpr/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.013001 skip-django-GDPR-0.2.23.2/gdpr/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/management/commands/anonymize_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/management/commands/deactivate_expired_reasons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0002_auto_20180509_1518.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0003.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0004.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0005_anon_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0006_auto_20190228_0725.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0007_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0008_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0009_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0010_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/0011_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.017001 skip-django-GDPR-0.2.23.2/gdpr/purposes/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/purposes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/purposes/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/gdpr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/test_cs_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/test_gis_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/tests/test_ipcypher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/gdpr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-01-17 15:58:16.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-01-17 15:58:17.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:58:16.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:58:16.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-17 15:58:16.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-17 15:58:16.000000 skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/anonymizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0002_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0003_IBAN.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0004_facebook_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0005_avatar.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0006_auto_20190305_0323.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0007_childe_extraparentd_parentb_parentc_topparenta.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/0008_customerregistration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/purposes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:17.021001 skip-django-GDPR-0.2.23.2/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/test_deactivate_expired_reasons.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/test_legal_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)    24933 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/test_model_anonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-01-17 15:58:05.000000 skip-django-GDPR-0.2.23.2/tests/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.382362 skip_django_gdpr-0.3.0/gdpr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.382362 skip_django_gdpr-0.3.0/gdpr/anonymizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/generic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/gis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/hash_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.382362 skip_django_gdpr-0.3.0/gdpr/anonymizers/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/local/cs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20592 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/anonymizers/model_anonymizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/ipcypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.378362 skip_django_gdpr-0.3.0/gdpr/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.378362 skip_django_gdpr-0.3.0/gdpr/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.386362 skip_django_gdpr-0.3.0/gdpr/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.386362 skip_django_gdpr-0.3.0/gdpr/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.386362 skip_django_gdpr-0.3.0/gdpr/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/management/commands/anonymize_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/management/commands/deactivate_expired_reasons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.386362 skip_django_gdpr-0.3.0/gdpr/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0002_auto_20180509_1518.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0003.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0005_anon_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0006_auto_20190228_0725.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0007_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0008_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0009_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0010_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/0011_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.386362 skip_django_gdpr-0.3.0/gdpr/purposes/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/purposes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/purposes/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.390362 skip_django_gdpr-0.3.0/gdpr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/test_cs_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/test_gis_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/tests/test_ipcypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/gdpr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 14:45:58.000000 skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.390362 skip_django_gdpr-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/anonymizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0002_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0003_IBAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0004_facebook_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0005_avatar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0006_auto_20190305_0323.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0007_childe_extraparentd_parentb_parentc_topparenta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/0008_customerregistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/purposes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:58.394362 skip_django_gdpr-0.3.0/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/test_deactivate_expired_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/test_legal_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/test_model_anonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-18 14:45:54.000000 skip_django_gdpr-0.3.0/tests/validators.py
```

### Comparing `skip-django-GDPR-0.2.23.2/LICENSE` & `skip_django_gdpr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/PKG-INFO` & `skip_django_gdpr-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: skip-django-GDPR
-Version: 0.2.23.2
-Summary: Library for GDPR implementation
-Home-page: https://github.com/skip-pay/django-GDPR
-Author: Druids
-Author-email: matllubos@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.10
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django-GDPR [![Build Status](https://travis-ci.org/BrnoPCmaniak/django-GDPR.svg?branch=develop)](https://travis-ci.org/BrnoPCmaniak/django-GDPR)
 
 This library enables you to store user's consent for data retention easily
 and to anonymize/deanonymize user's data accordingly.
 
 For brief overview you can check example app in `tests` directory.
```

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/__init__.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/base.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/fields.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/generic_relation.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/generic_relation.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/gis.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/gis.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/hash_fields.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/hash_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/local/cs.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/local/cs.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/anonymizers/model_anonymizers.py` & `skip_django_gdpr-0.3.0/gdpr/anonymizers/model_anonymizers.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/encryption.py` & `skip_django_gdpr-0.3.0/gdpr/encryption.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/fields.py` & `skip_django_gdpr-0.3.0/gdpr/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/ipcypher.py` & `skip_django_gdpr-0.3.0/gdpr/ipcypher.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/loading.py` & `skip_django_gdpr-0.3.0/gdpr/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from importlib import import_module
 from typing import TYPE_CHECKING, Any, Generic, Iterator, Optional, Type, TypeVar, Union
 
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models import Model
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from .utils import str_to_class
 
 if TYPE_CHECKING:
     from gdpr.anonymizers import ModelAnonymizer
     from gdpr.purposes import AbstractPurpose
 
@@ -30,15 +30,15 @@
     def import_modules(self) -> None:
         for app in apps.get_app_configs():
             if app.name == 'gdpr':
                 continue
             try:
                 import_module(f'{app.name}.{self.module_name}')
             except ImportError as ex:
-                if force_text(ex) != f'No module named \'{app.name}.{self.module_name}\'':
+                if force_str(ex) != f'No module named \'{app.name}.{self.module_name}\'':
                     raise ex
 
 
 class SettingsListLoader(BaseLoader):
     """Import all modules from list `list_name` in settings."""
 
     list_name: str
```

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/locale/cs/LC_MESSAGES/django.mo` & `skip_django_gdpr-0.3.0/gdpr/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/locale/cs/LC_MESSAGES/django.po` & `skip_django_gdpr-0.3.0/gdpr/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/management/commands/anonymize_data.py` & `skip_django_gdpr-0.3.0/gdpr/management/commands/anonymize_data.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/management/commands/deactivate_expired_reasons.py` & `skip_django_gdpr-0.3.0/gdpr/management/commands/deactivate_expired_reasons.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0001_initial.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0002_auto_20180509_1518.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0002_auto_20180509_1518.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0003.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0003.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0004.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0004.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0005_anon_2_0.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0005_anon_2_0.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0006_auto_20190228_0725.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0006_auto_20190228_0725.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0007_migration.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0007_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0008_migration.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0008_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/migrations/0011_migration.py` & `skip_django_gdpr-0.3.0/gdpr/migrations/0011_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/mixins.py` & `skip_django_gdpr-0.3.0/gdpr/mixins.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/models.py` & `skip_django_gdpr-0.3.0/gdpr/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/purposes/default.py` & `skip_django_gdpr-0.3.0/gdpr/purposes/default.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/tests/test_cs_fields.py` & `skip_django_gdpr-0.3.0/gdpr/tests/test_cs_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/tests/test_encryption.py` & `skip_django_gdpr-0.3.0/gdpr/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/tests/test_fields.py` & `skip_django_gdpr-0.3.0/gdpr/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/tests/test_gis_fields.py` & `skip_django_gdpr-0.3.0/gdpr/tests/test_gis_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/tests/test_ipcypher.py` & `skip_django_gdpr-0.3.0/gdpr/tests/test_ipcypher.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/gdpr/utils.py` & `skip_django_gdpr-0.3.0/gdpr/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/setup.py` & `skip_django_gdpr-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3 :: Only',
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     install_requires=[
-        'django>=2.2,<4.0',
-        'skip-django-chamber>=0.6.16.3',
+        'django>=4.2',
+        'skip-django-chamber>=0.7.2',
         'tqdm>=4.28.1',
         'pyaes>=1.6.1',
         'unidecode',
         'skip-django-choice-enumfields>=1.1.3.2',
     ],
     zip_safe=False,
 )
```

### Comparing `skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/PKG-INFO` & `skip_django_gdpr-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-GDPR
-Version: 0.2.23.2
+Version: 0.3.0
 Summary: Library for GDPR implementation
 Home-page: https://github.com/skip-pay/django-GDPR
 Author: Druids
 Author-email: matllubos@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
@@ -19,14 +19,20 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: tqdm>=4.28.1
+Requires-Dist: pyaes>=1.6.1
+Requires-Dist: unidecode
+Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
 
 # Django-GDPR [![Build Status](https://travis-ci.org/BrnoPCmaniak/django-GDPR.svg?branch=develop)](https://travis-ci.org/BrnoPCmaniak/django-GDPR)
 
 This library enables you to store user's consent for data retention easily
 and to anonymize/deanonymize user's data accordingly.
 
 For brief overview you can check example app in `tests` directory.
```

### Comparing `skip-django-GDPR-0.2.23.2/skip_django_GDPR.egg-info/SOURCES.txt` & `skip_django_gdpr-0.3.0/skip_django_GDPR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/anonymizers.py` & `skip_django_gdpr-0.3.0/tests/anonymizers.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0001_initial.py` & `skip_django_gdpr-0.3.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0002_note.py` & `skip_django_gdpr-0.3.0/tests/migrations/0002_note.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0003_IBAN.py` & `skip_django_gdpr-0.3.0/tests/migrations/0003_IBAN.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0004_facebook_id.py` & `skip_django_gdpr-0.3.0/tests/migrations/0004_facebook_id.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0005_avatar.py` & `skip_django_gdpr-0.3.0/tests/migrations/0005_avatar.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0007_childe_extraparentd_parentb_parentc_topparenta.py` & `skip_django_gdpr-0.3.0/tests/migrations/0007_childe_extraparentd_parentb_parentc_topparenta.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/migrations/0008_customerregistration.py` & `skip_django_gdpr-0.3.0/tests/migrations/0008_customerregistration.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/models.py` & `skip_django_gdpr-0.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/purposes.py` & `skip_django_gdpr-0.3.0/tests/purposes.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/test_settings.py` & `skip_django_gdpr-0.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/data.py` & `skip_django_gdpr-0.3.0/tests/tests/data.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/test_deactivate_expired_reasons.py` & `skip_django_gdpr-0.3.0/tests/tests/test_deactivate_expired_reasons.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/test_fields.py` & `skip_django_gdpr-0.3.0/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/test_legal_reason.py` & `skip_django_gdpr-0.3.0/tests/tests/test_legal_reason.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/test_model_anonymization.py` & `skip_django_gdpr-0.3.0/tests/tests/test_model_anonymization.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/tests/utils.py` & `skip_django_gdpr-0.3.0/tests/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-GDPR-0.2.23.2/tests/validators.py` & `skip_django_gdpr-0.3.0/tests/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from datetime import date
 
 from django.core.exceptions import ValidationError
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 
 
 def get_day_from_personal_id(personal_id):
     day = int(personal_id[4:6])
     if day > 50:
         day -= 50
     return day
@@ -43,15 +43,15 @@
 class CZBirthNumberValidator:
     """
     Czech birth number field validator.
     """
     BIRTH_NUMBER = re.compile(r'^(?P<birth>\d{6})/?(?P<id>\d{3,4})$')
 
     def __call__(self, value):
-        value = force_text(value)
+        value = force_str(value)
 
         match = re.match(self.BIRTH_NUMBER, value)
         if not match:
             raise ValidationError(_('Enter a birth number in the format XXXXXX/XXXX.'))
 
         birth, id = match.groupdict()['birth'], match.groupdict()['id']
 
@@ -77,15 +77,15 @@
 class IDCardNoValidator:
     """
     Czech id card number field validator.
     """
     ID_CARD_NUMBER = re.compile(r'^\d{9}$')
 
     def __call__(self, value):
-        value = force_text(value)
+        value = force_str(value)
 
         match = re.match(self.ID_CARD_NUMBER, value)
         if not match:
             raise ValidationError(_('Enter an ID card in the format XXXXXXXXX.'))
         elif value[0] == '0':
             raise ValidationError(_('Enter a valid ID card number.'))
         else:
@@ -93,15 +93,15 @@
 
 
 class BankAccountValidator:
     BANK_ACCOUNT_NUMBER_REVERSE_PATTERN = re.compile(
         r'^(?P<bank>\d{1,6})/(?P<number>\d{1,10})(-?(?P<prefix>\d{1,6}))?$')
 
     def __call__(self, value):
-        match = re.match(self.BANK_ACCOUNT_NUMBER_REVERSE_PATTERN, force_text(value)[::-1])
+        match = re.match(self.BANK_ACCOUNT_NUMBER_REVERSE_PATTERN, force_str(value)[::-1])
         if match:
             return construct_bank_account_number((match.groupdict()['prefix'] or '')[::-1],
                                                  match.groupdict()['number'][::-1],
                                                  match.groupdict()['bank'][::-1])
         else:
             raise ValidationError(_('Enter a valid bank account number.'))
```

