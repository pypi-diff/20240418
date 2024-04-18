# Comparing `tmp/baseapp-django-push-notifications-3.0.3rc2.tar.gz` & `tmp/baseapp-django-push-notifications-3.0.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseapp-django-push-notifications-3.0.3rc2.tar", last modified: Thu Apr 11 18:51:25 2024, max compression
+gzip compressed data, was "baseapp-django-push-notifications-3.0.3rc3.tar", last modified: Thu Apr 18 16:11:04 2024, max compression
```

## Comparing `baseapp-django-push-notifications-3.0.3rc2.tar` & `baseapp-django-push-notifications-3.0.3rc3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.093996 baseapp-django-push-notifications-3.0.3rc2/
--rw-r--r--   0 alisson    (501) staff       (20)      288 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/.editorconfig
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.081465 baseapp-django-push-notifications-3.0.3rc2/.github/
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.084319 baseapp-django-push-notifications-3.0.3rc2/.github/workflows/
--rw-r--r--   0 alisson    (501) staff       (20)     1021 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/.github/workflows/release.yml
--rw-r--r--   0 alisson    (501) staff       (20)     1271 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/.github/workflows/test.yml
--rw-r--r--   0 alisson    (501) staff       (20)      193 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/.gitignore
--rw-r--r--   0 alisson    (501) staff       (20)      415 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/.pre-commit-config.yaml
--rw-r--r--   0 alisson    (501) staff       (20)      436 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/ACKNOWLEDGEMENTS.md
--rw-r--r--   0 alisson    (501) staff       (20)     5682 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/CHANGELOG.md
--rw-r--r--   0 alisson    (501) staff       (20)     2375 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 alisson    (501) staff       (20)     1774 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/CONTRIBUTING.md
--rw-r--r--   0 alisson    (501) staff       (20)     1074 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/LICENSE
--rw-r--r--   0 alisson    (501) staff       (20)       55 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/MANIFEST.in
--rw-r--r--   0 alisson    (501) staff       (20)    19425 2024-04-11 18:51:25.093882 baseapp-django-push-notifications-3.0.3rc2/PKG-INFO
--rw-r--r--   0 alisson    (501) staff       (20)    17717 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/README.rst
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.093076 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/
--rw-r--r--   0 alisson    (501) staff       (20)    19425 2024-04-11 18:51:25.000000 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/PKG-INFO
--rw-r--r--   0 alisson    (501) staff       (20)     2271 2024-04-11 18:51:25.000000 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 alisson    (501) staff       (20)        1 2024-04-11 18:51:25.000000 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 alisson    (501) staff       (20)      145 2024-04-11 18:51:25.000000 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/requires.txt
--rw-r--r--   0 alisson    (501) staff       (20)       19 2024-04-11 18:51:25.000000 baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/top_level.txt
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.085213 baseapp-django-push-notifications-3.0.3rc2/docs/
--rw-r--r--   0 alisson    (501) staff       (20)     2467 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/docs/APNS.rst
--rw-r--r--   0 alisson    (501) staff       (20)     6782 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/docs/WebPush.rst
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.087103 baseapp-django-push-notifications-3.0.3rc2/push_notifications/
--rw-r--r--   0 alisson    (501) staff       (20)      224 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/__init__.py
--rw-r--r--   0 alisson    (501) staff       (20)     4383 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/admin.py
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.087333 baseapp-django-push-notifications-3.0.3rc2/push_notifications/api/
--rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/api/__init__.py
--rw-r--r--   0 alisson    (501) staff       (20)     6382 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/api/rest_framework.py
--rw-r--r--   0 alisson    (501) staff       (20)     5183 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/apns.py
--rw-r--r--   0 alisson    (501) staff       (20)    10328 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/apns_async.py
--rw-r--r--   0 alisson    (501) staff       (20)      128 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/compat.py
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.088028 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/
--rw-r--r--   0 alisson    (501) staff       (20)      527 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/__init__.py
--rw-r--r--   0 alisson    (501) staff       (20)    12804 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/app.py
--rw-r--r--   0 alisson    (501) staff       (20)      181 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/appmodel.py
--rw-r--r--   0 alisson    (501) staff       (20)     1844 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/base.py
--rw-r--r--   0 alisson    (501) staff       (20)     5529 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/legacy.py
--rw-r--r--   0 alisson    (501) staff       (20)      365 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/exceptions.py
--rw-r--r--   0 alisson    (501) staff       (20)     3523 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/fields.py
--rw-r--r--   0 alisson    (501) staff       (20)     7319 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/gcm.py
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.089628 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/
--rw-r--r--   0 alisson    (501) staff       (20)     2534 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0001_initial.py
--rw-r--r--   0 alisson    (501) staff       (20)      444 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0002_auto_20160106_0850.py
--rw-r--r--   0 alisson    (501) staff       (20)     1416 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0003_wnsdevice.py
--rw-r--r--   0 alisson    (501) staff       (20)      605 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0004_fcm.py
--rw-r--r--   0 alisson    (501) staff       (20)     1261 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0005_applicationid.py
--rw-r--r--   0 alisson    (501) staff       (20)     1856 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0006_webpushdevice.py
--rw-r--r--   0 alisson    (501) staff       (20)     1140 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0007_uniquesetting.py
--rw-r--r--   0 alisson    (501) staff       (20)      616 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0008_webpush_add_edge.py
--rw-r--r--   0 alisson    (501) staff       (20)      502 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0009_alter_apnsdevice_device_id.py
--rw-r--r--   0 alisson    (501) staff       (20)      827 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0010_alter_gcmdevice_cloud_message_type.py
--rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/__init__.py
--rw-r--r--   0 alisson    (501) staff       (20)     7453 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/models.py
--rw-r--r--   0 alisson    (501) staff       (20)     2023 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/settings.py
--rw-r--r--   0 alisson    (501) staff       (20)     1542 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/webpush.py
--rw-r--r--   0 alisson    (501) staff       (20)    11319 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/push_notifications/wns.py
--rw-r--r--   0 alisson    (501) staff       (20)      251 2024-04-11 18:48:42.000000 baseapp-django-push-notifications-3.0.3rc2/pyproject.toml
--rw-r--r--   0 alisson    (501) staff       (20)     1399 2024-04-11 18:51:25.094298 baseapp-django-push-notifications-3.0.3rc2/setup.cfg
--rwxr-xr-x   0 alisson    (501) staff       (20)      330 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/setup.py
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.092401 baseapp-django-push-notifications-3.0.3rc2/tests/
--rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/__init__.py
--rw-r--r--   0 alisson    (501) staff       (20)     2221 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/responses.py
--rw-r--r--   0 alisson    (501) staff       (20)      496 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/settings.py
--rw-r--r--   0 alisson    (501) staff       (20)      520 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/settings_unique.py
--rw-r--r--   0 alisson    (501) staff       (20)     5607 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_async_models.py
--rw-r--r--   0 alisson    (501) staff       (20)     5029 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_async_push_payload.py
--rw-r--r--   0 alisson    (501) staff       (20)     4924 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_models.py
--rw-r--r--   0 alisson    (501) staff       (20)     4532 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_push_payload.py
--rw-r--r--   0 alisson    (501) staff       (20)     7087 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_app_config.py
-drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-11 18:51:25.092883 baseapp-django-push-notifications-3.0.3rc2/tests/test_data/
--rw-r--r--   0 alisson    (501) staff       (20)     4248 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_data/good_revoked.pem
--rw-r--r--   0 alisson    (501) staff       (20)     3900 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_data/good_with_passwd.pem
--rw-r--r--   0 alisson    (501) staff       (20)     1992 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_data/without_private.pem
--rw-r--r--   0 alisson    (501) staff       (20)      995 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_fields.py
--rw-r--r--   0 alisson    (501) staff       (20)     3213 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_gcm_push_payload.py
--rw-r--r--   0 alisson    (501) staff       (20)     1936 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_legacy_config.py
--rw-r--r--   0 alisson    (501) staff       (20)    19720 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_models.py
--rw-r--r--   0 alisson    (501) staff       (20)     4503 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_rest_framework.py
--rw-r--r--   0 alisson    (501) staff       (20)     2945 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_webpush.py
--rw-r--r--   0 alisson    (501) staff       (20)     5330 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/test_wns.py
--rw-r--r--   0 alisson    (501) staff       (20)     1618 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tests/tst_unique.py
--rw-r--r--   0 alisson    (501) staff       (20)     1209 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc2/tox.ini
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.348600 baseapp-django-push-notifications-3.0.3rc3/
+-rw-r--r--   0 alisson    (501) staff       (20)      288 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/.editorconfig
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.333762 baseapp-django-push-notifications-3.0.3rc3/.github/
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.337426 baseapp-django-push-notifications-3.0.3rc3/.github/workflows/
+-rw-r--r--   0 alisson    (501) staff       (20)     1021 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/.github/workflows/release.yml
+-rw-r--r--   0 alisson    (501) staff       (20)     1271 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/.github/workflows/test.yml
+-rw-r--r--   0 alisson    (501) staff       (20)      193 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/.gitignore
+-rw-r--r--   0 alisson    (501) staff       (20)      415 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/.pre-commit-config.yaml
+-rw-r--r--   0 alisson    (501) staff       (20)      436 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/ACKNOWLEDGEMENTS.md
+-rw-r--r--   0 alisson    (501) staff       (20)     5682 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/CHANGELOG.md
+-rw-r--r--   0 alisson    (501) staff       (20)     2375 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 alisson    (501) staff       (20)     1774 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/CONTRIBUTING.md
+-rw-r--r--   0 alisson    (501) staff       (20)     1074 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/LICENSE
+-rw-r--r--   0 alisson    (501) staff       (20)       55 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/MANIFEST.in
+-rw-r--r--   0 alisson    (501) staff       (20)    19425 2024-04-18 16:11:04.348459 baseapp-django-push-notifications-3.0.3rc3/PKG-INFO
+-rw-r--r--   0 alisson    (501) staff       (20)    17717 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/README.rst
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.347543 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/
+-rw-r--r--   0 alisson    (501) staff       (20)    19425 2024-04-18 16:11:04.000000 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 alisson    (501) staff       (20)     2271 2024-04-18 16:11:04.000000 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 alisson    (501) staff       (20)        1 2024-04-18 16:11:04.000000 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 alisson    (501) staff       (20)      145 2024-04-18 16:11:04.000000 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/requires.txt
+-rw-r--r--   0 alisson    (501) staff       (20)       19 2024-04-18 16:11:04.000000 baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.338348 baseapp-django-push-notifications-3.0.3rc3/docs/
+-rw-r--r--   0 alisson    (501) staff       (20)     2467 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/docs/APNS.rst
+-rw-r--r--   0 alisson    (501) staff       (20)     6782 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/docs/WebPush.rst
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.340906 baseapp-django-push-notifications-3.0.3rc3/push_notifications/
+-rw-r--r--   0 alisson    (501) staff       (20)      232 2024-04-18 16:09:40.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/__init__.py
+-rw-r--r--   0 alisson    (501) staff       (20)     4383 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/admin.py
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.341254 baseapp-django-push-notifications-3.0.3rc3/push_notifications/api/
+-rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/api/__init__.py
+-rw-r--r--   0 alisson    (501) staff       (20)     6382 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/api/rest_framework.py
+-rw-r--r--   0 alisson    (501) staff       (20)     5183 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/apns.py
+-rw-r--r--   0 alisson    (501) staff       (20)    10328 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/apns_async.py
+-rw-r--r--   0 alisson    (501) staff       (20)      128 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/compat.py
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.342123 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/
+-rw-r--r--   0 alisson    (501) staff       (20)      527 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/__init__.py
+-rw-r--r--   0 alisson    (501) staff       (20)    12804 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/app.py
+-rw-r--r--   0 alisson    (501) staff       (20)      181 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/appmodel.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1844 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/base.py
+-rw-r--r--   0 alisson    (501) staff       (20)     5529 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/legacy.py
+-rw-r--r--   0 alisson    (501) staff       (20)      365 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/exceptions.py
+-rw-r--r--   0 alisson    (501) staff       (20)     3523 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/fields.py
+-rw-r--r--   0 alisson    (501) staff       (20)     7319 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/gcm.py
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.343729 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/
+-rw-r--r--   0 alisson    (501) staff       (20)     2534 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0001_initial.py
+-rw-r--r--   0 alisson    (501) staff       (20)      444 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0002_auto_20160106_0850.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1416 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0003_wnsdevice.py
+-rw-r--r--   0 alisson    (501) staff       (20)      605 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0004_fcm.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1261 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0005_applicationid.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1856 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0006_webpushdevice.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1140 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0007_uniquesetting.py
+-rw-r--r--   0 alisson    (501) staff       (20)      616 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0008_webpush_add_edge.py
+-rw-r--r--   0 alisson    (501) staff       (20)      502 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0009_alter_apnsdevice_device_id.py
+-rw-r--r--   0 alisson    (501) staff       (20)      827 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0010_alter_gcmdevice_cloud_message_type.py
+-rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/__init__.py
+-rw-r--r--   0 alisson    (501) staff       (20)     7453 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/models.py
+-rw-r--r--   0 alisson    (501) staff       (20)     2023 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/settings.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1542 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/webpush.py
+-rw-r--r--   0 alisson    (501) staff       (20)    11319 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/push_notifications/wns.py
+-rw-r--r--   0 alisson    (501) staff       (20)      251 2024-04-18 16:09:40.000000 baseapp-django-push-notifications-3.0.3rc3/pyproject.toml
+-rw-r--r--   0 alisson    (501) staff       (20)     1399 2024-04-18 16:11:04.348918 baseapp-django-push-notifications-3.0.3rc3/setup.cfg
+-rwxr-xr-x   0 alisson    (501) staff       (20)      330 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/setup.py
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.346726 baseapp-django-push-notifications-3.0.3rc3/tests/
+-rw-r--r--   0 alisson    (501) staff       (20)        0 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/__init__.py
+-rw-r--r--   0 alisson    (501) staff       (20)     2221 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/responses.py
+-rw-r--r--   0 alisson    (501) staff       (20)      496 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/settings.py
+-rw-r--r--   0 alisson    (501) staff       (20)      520 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/settings_unique.py
+-rw-r--r--   0 alisson    (501) staff       (20)     5607 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_async_models.py
+-rw-r--r--   0 alisson    (501) staff       (20)     5029 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_async_push_payload.py
+-rw-r--r--   0 alisson    (501) staff       (20)     4924 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_models.py
+-rw-r--r--   0 alisson    (501) staff       (20)     4532 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_push_payload.py
+-rw-r--r--   0 alisson    (501) staff       (20)     7087 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_app_config.py
+drwxr-xr-x   0 alisson    (501) staff       (20)        0 2024-04-18 16:11:04.347325 baseapp-django-push-notifications-3.0.3rc3/tests/test_data/
+-rw-r--r--   0 alisson    (501) staff       (20)     4248 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_data/good_revoked.pem
+-rw-r--r--   0 alisson    (501) staff       (20)     3900 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_data/good_with_passwd.pem
+-rw-r--r--   0 alisson    (501) staff       (20)     1992 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_data/without_private.pem
+-rw-r--r--   0 alisson    (501) staff       (20)      995 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_fields.py
+-rw-r--r--   0 alisson    (501) staff       (20)     3213 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_gcm_push_payload.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1936 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_legacy_config.py
+-rw-r--r--   0 alisson    (501) staff       (20)    19720 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_models.py
+-rw-r--r--   0 alisson    (501) staff       (20)     4503 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_rest_framework.py
+-rw-r--r--   0 alisson    (501) staff       (20)     2945 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_webpush.py
+-rw-r--r--   0 alisson    (501) staff       (20)     5330 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/test_wns.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1618 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tests/tst_unique.py
+-rw-r--r--   0 alisson    (501) staff       (20)     1209 2024-04-11 18:36:29.000000 baseapp-django-push-notifications-3.0.3rc3/tox.ini
```

### Comparing `baseapp-django-push-notifications-3.0.3rc2/.github/workflows/release.yml` & `baseapp-django-push-notifications-3.0.3rc3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/.github/workflows/test.yml` & `baseapp-django-push-notifications-3.0.3rc3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/CHANGELOG.md` & `baseapp-django-push-notifications-3.0.3rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/CODE_OF_CONDUCT.md` & `baseapp-django-push-notifications-3.0.3rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/CONTRIBUTING.md` & `baseapp-django-push-notifications-3.0.3rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/LICENSE` & `baseapp-django-push-notifications-3.0.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/PKG-INFO` & `baseapp-django-push-notifications-3.0.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-django-push-notifications
-Version: 3.0.3rc2
+Version: 3.0.3rc3
 Summary: Send push notifications to mobile devices through GCM, APNS or WNS and to WebPush (Chrome, Firefox and Opera) in Django
 Home-page: https://github.com/silverlogic/django-push-notifications
 Download-URL: https://github.com/silverlogic/django-push-notifications/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `baseapp-django-push-notifications-3.0.3rc2/README.rst` & `baseapp-django-push-notifications-3.0.3rc3/README.rst`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/PKG-INFO` & `baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseapp-django-push-notifications
-Version: 3.0.3rc2
+Version: 3.0.3rc3
 Summary: Send push notifications to mobile devices through GCM, APNS or WNS and to WebPush (Chrome, Firefox and Opera) in Django
 Home-page: https://github.com/silverlogic/django-push-notifications
 Download-URL: https://github.com/silverlogic/django-push-notifications/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `baseapp-django-push-notifications-3.0.3rc2/baseapp_django_push_notifications.egg-info/SOURCES.txt` & `baseapp-django-push-notifications-3.0.3rc3/baseapp_django_push_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/docs/APNS.rst` & `baseapp-django-push-notifications-3.0.3rc3/docs/APNS.rst`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/docs/WebPush.rst` & `baseapp-django-push-notifications-3.0.3rc3/docs/WebPush.rst`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/admin.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/api/rest_framework.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/api/rest_framework.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/apns.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/apns.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/apns_async.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/apns_async.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/__init__.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/app.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/app.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/base.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/base.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/conf/legacy.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/conf/legacy.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/fields.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/fields.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/gcm.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/gcm.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0001_initial.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0003_wnsdevice.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0003_wnsdevice.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0004_fcm.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0004_fcm.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0005_applicationid.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0005_applicationid.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0006_webpushdevice.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0006_webpushdevice.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0007_uniquesetting.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0007_uniquesetting.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0008_webpush_add_edge.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0008_webpush_add_edge.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/migrations/0010_alter_gcmdevice_cloud_message_type.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/migrations/0010_alter_gcmdevice_cloud_message_type.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/models.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/models.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/settings.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/settings.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/webpush.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/webpush.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/push_notifications/wns.py` & `baseapp-django-push-notifications-3.0.3rc3/push_notifications/wns.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/setup.cfg` & `baseapp-django-push-notifications-3.0.3rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/responses.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/responses.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/settings_unique.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/settings_unique.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_async_models.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_async_models.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_async_push_payload.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_async_push_payload.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_models.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_models.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_apns_push_payload.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_apns_push_payload.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_app_config.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_data/good_revoked.pem` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_data/good_revoked.pem`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_data/good_with_passwd.pem` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_data/good_with_passwd.pem`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_data/without_private.pem` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_data/without_private.pem`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_fields.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_gcm_push_payload.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_gcm_push_payload.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_legacy_config.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_legacy_config.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_models.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_rest_framework.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_rest_framework.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_webpush.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_webpush.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/test_wns.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/test_wns.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tests/tst_unique.py` & `baseapp-django-push-notifications-3.0.3rc3/tests/tst_unique.py`

 * *Files identical despite different names*

### Comparing `baseapp-django-push-notifications-3.0.3rc2/tox.ini` & `baseapp-django-push-notifications-3.0.3rc3/tox.ini`

 * *Files identical despite different names*

