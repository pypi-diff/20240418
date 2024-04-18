# Comparing `tmp/edc-microbiology-0.3.8.tar.gz` & `tmp/edc-microbiology-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-microbiology-0.3.8.tar", last modified: Fri Mar  8 06:12:29 2024, max compression
+gzip compressed data, was "edc-microbiology-0.3.9.tar", last modified: Tue Mar 26 05:04:07 2024, max compression
```

## Comparing `edc-microbiology-0.3.8.tar` & `edc-microbiology-0.3.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.482862 edc-microbiology-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      108 2022-02-16 18:04:06.000000 edc-microbiology-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-02-16 18:04:06.000000 edc-microbiology-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.468072 edc-microbiology-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.471821 edc-microbiology-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1920 2024-03-08 06:12:21.000000 edc-microbiology-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 06:12:21.000000 edc-microbiology-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-26 02:09:03.000000 edc-microbiology-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-02-16 14:40:34.000000 edc-microbiology-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-09-28 02:07:22.000000 edc-microbiology-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1553 2024-03-08 06:12:29.482787 edc-microbiology-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-12-14 21:33:01.000000 edc-microbiology-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-26 02:09:03.000000 edc-microbiology-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.474315 edc-microbiology-0.3.8/edc_microbiology/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:04:06.000000 edc-microbiology-0.3.8/edc_microbiology/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      536 2022-08-26 02:09:03.000000 edc-microbiology-0.3.8/edc_microbiology/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-06-01 18:29:20.000000 edc-microbiology-0.3.8/edc_microbiology/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      195 2022-02-28 17:41:48.000000 edc-microbiology-0.3.8/edc_microbiology/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      607 2022-06-01 18:29:26.000000 edc-microbiology-0.3.8/edc_microbiology/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      378 2022-02-16 18:04:06.000000 edc-microbiology-0.3.8/edc_microbiology/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1851 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/edc_microbiology/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/edc_microbiology/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-01 18:29:42.000000 edc-microbiology-0.3.8/edc_microbiology/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7482 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      419 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.477290 edc-microbiology-0.3.8/edc_microbiology/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    41347 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      935 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0002_auto_20220223_2236.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3476 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0003_auto_20220223_2256.py
--rw-r--r--   0 erikvw     (501) staff       (20)      588 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0004_auto_20220223_2258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1960 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0005_auto_20220224_1509.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4650 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0006_auto_20220224_1826.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2620 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0007_auto_20220224_1910.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6340 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0008_auto_20220224_1926.py
--rw-r--r--   0 erikvw     (501) staff       (20)      802 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0009_auto_20220711_1230.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3724 2023-12-13 23:10:08.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0010_alter_microbiology_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2702 2024-01-06 04:00:29.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0011_alter_microbiology_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1040 2024-01-24 18:34:28.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/0012_alter_historicalmicrobiology_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.478587 edc-microbiology-0.3.8/edc_microbiology/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2022-02-28 17:41:48.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1837 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/blood_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-06-01 18:59:45.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/csf_genexpert.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1708 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/histopathology.py
--rw-r--r--   0 erikvw     (501) staff       (20)      890 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_afb.py
--rw-r--r--   0 erikvw     (501) staff       (20)      877 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_genexpert.py
--rw-r--r--   0 erikvw     (501) staff       (20)      997 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/urinary_lam.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1236 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/model_mixins/urine_culture.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.479382 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-02-28 17:41:48.000000 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      494 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/blood_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      448 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/histopathology.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1028 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/microbiology.py
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-04-22 18:06:41.000000 edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/urine_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1231 2024-01-06 04:00:29.000000 edc-microbiology-0.3.8/edc_microbiology/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.479526 edc-microbiology-0.3.8/edc_microbiology/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.480767 edc-microbiology-0.3.8/edc_microbiology/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.481263 edc-microbiology-0.3.8/edc_microbiology/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-26 02:09:03.000000 edc-microbiology-0.3.8/edc_microbiology/tests/tests/test_auth.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16252 2024-01-24 05:36:57.000000 edc-microbiology-0.3.8/edc_microbiology/tests/tests/test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      307 2022-02-16 18:20:26.000000 edc-microbiology-0.3.8/edc_microbiology/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.482519 edc-microbiology-0.3.8/edc_microbiology.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1553 2024-03-08 06:12:29.000000 edc-microbiology-0.3.8/edc_microbiology.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2935 2024-03-08 06:12:29.000000 edc-microbiology-0.3.8/edc_microbiology.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-08 06:12:29.000000 edc-microbiology-0.3.8/edc_microbiology.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-16 17:07:31.000000 edc-microbiology-0.3.8/edc_microbiology.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       34 2024-03-08 06:12:29.000000 edc-microbiology-0.3.8/edc_microbiology.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-08 06:12:29.482277 edc-microbiology-0.3.8/microbiology_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-10-10 03:24:26.000000 edc-microbiology-0.3.8/microbiology_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-10-10 03:24:26.000000 edc-microbiology-0.3.8/microbiology_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      467 2024-03-08 06:12:21.000000 edc-microbiology-0.3.8/microbiology_app/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2210 2024-03-08 06:12:21.000000 edc-microbiology-0.3.8/microbiology_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2023-10-10 03:24:26.000000 edc-microbiology-0.3.8/microbiology_app/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1671 2024-01-24 05:36:57.000000 edc-microbiology-0.3.8/microbiology_app/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1695 2023-10-10 03:24:26.000000 edc-microbiology-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2486 2024-01-29 05:45:18.000000 edc-microbiology-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1148 2024-03-08 06:12:29.483176 edc-microbiology-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.301489 edc-microbiology-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      108 2022-02-16 18:04:06.000000 edc-microbiology-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-02-16 18:04:06.000000 edc-microbiology-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.285699 edc-microbiology-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.289734 edc-microbiology-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1920 2024-03-08 06:12:21.000000 edc-microbiology-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-03-08 06:12:21.000000 edc-microbiology-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-26 02:09:03.000000 edc-microbiology-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-02-16 14:40:34.000000 edc-microbiology-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2023-09-28 02:07:22.000000 edc-microbiology-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1553 2024-03-26 05:04:07.301422 edc-microbiology-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2023-12-14 21:33:01.000000 edc-microbiology-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-26 02:09:03.000000 edc-microbiology-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.292707 edc-microbiology-0.3.9/edc_microbiology/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:04:06.000000 edc-microbiology-0.3.9/edc_microbiology/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      536 2022-08-26 02:09:03.000000 edc-microbiology-0.3.9/edc_microbiology/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-06-01 18:29:20.000000 edc-microbiology-0.3.9/edc_microbiology/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      195 2022-02-28 17:41:48.000000 edc-microbiology-0.3.9/edc_microbiology/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      607 2022-06-01 18:29:26.000000 edc-microbiology-0.3.9/edc_microbiology/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      378 2022-02-16 18:04:06.000000 edc-microbiology-0.3.9/edc_microbiology/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1851 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/edc_microbiology/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/edc_microbiology/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-01 18:29:42.000000 edc-microbiology-0.3.9/edc_microbiology/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7482 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      419 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/forms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.295870 edc-microbiology-0.3.9/edc_microbiology/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    41347 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      935 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0002_auto_20220223_2236.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3476 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0003_auto_20220223_2256.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      588 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0004_auto_20220223_2258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1960 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0005_auto_20220224_1509.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4650 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0006_auto_20220224_1826.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2620 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0007_auto_20220224_1910.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6340 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0008_auto_20220224_1926.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      802 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0009_auto_20220711_1230.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3724 2023-12-13 23:10:08.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0010_alter_microbiology_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2702 2024-01-06 04:00:29.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0011_alter_microbiology_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1040 2024-01-24 18:34:28.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/0012_alter_historicalmicrobiology_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.297223 edc-microbiology-0.3.9/edc_microbiology/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2022-02-28 17:41:48.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1837 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/blood_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-06-01 18:59:45.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/csf_genexpert.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1708 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/histopathology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      890 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_afb.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      877 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      959 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_genexpert.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      997 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/urinary_lam.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1236 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/model_mixins/urine_culture.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.298004 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-02-28 17:41:48.000000 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      494 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/blood_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      448 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/histopathology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1028 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/microbiology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2023-04-22 18:06:41.000000 edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/urine_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1231 2024-01-06 04:00:29.000000 edc-microbiology-0.3.9/edc_microbiology/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.298140 edc-microbiology-0.3.9/edc_microbiology/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.299364 edc-microbiology-0.3.9/edc_microbiology/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.299767 edc-microbiology-0.3.9/edc_microbiology/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-26 02:09:03.000000 edc-microbiology-0.3.9/edc_microbiology/tests/tests/test_auth.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16252 2024-01-24 05:36:57.000000 edc-microbiology-0.3.9/edc_microbiology/tests/tests/test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      307 2022-02-16 18:20:26.000000 edc-microbiology-0.3.9/edc_microbiology/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.301146 edc-microbiology-0.3.9/edc_microbiology.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1553 2024-03-26 05:04:07.000000 edc-microbiology-0.3.9/edc_microbiology.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2935 2024-03-26 05:04:07.000000 edc-microbiology-0.3.9/edc_microbiology.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-26 05:04:07.000000 edc-microbiology-0.3.9/edc_microbiology.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-16 17:07:31.000000 edc-microbiology-0.3.9/edc_microbiology.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       34 2024-03-26 05:04:07.000000 edc-microbiology-0.3.9/edc_microbiology.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-26 05:04:07.300881 edc-microbiology-0.3.9/microbiology_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-10-10 03:24:26.000000 edc-microbiology-0.3.9/microbiology_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      119 2023-10-10 03:24:26.000000 edc-microbiology-0.3.9/microbiology_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      467 2024-03-08 06:12:21.000000 edc-microbiology-0.3.9/microbiology_app/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2383 2024-03-26 05:03:58.000000 edc-microbiology-0.3.9/microbiology_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2023-10-10 03:24:26.000000 edc-microbiology-0.3.9/microbiology_app/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1671 2024-01-24 05:36:57.000000 edc-microbiology-0.3.9/microbiology_app/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1695 2023-10-10 03:24:26.000000 edc-microbiology-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2486 2024-01-29 05:45:18.000000 edc-microbiology-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1148 2024-03-26 05:04:07.301803 edc-microbiology-0.3.9/setup.cfg
```

### Comparing `edc-microbiology-0.3.8/.github/workflows/build.yml` & `edc-microbiology-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/.gitignore` & `edc-microbiology-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/.pre-commit-config.yaml` & `edc-microbiology-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/LICENSE` & `edc-microbiology-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/PKG-INFO` & `edc-microbiology-0.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microbiology
-Version: 0.3.8
+Version: 0.3.9
 Summary: Microbiology model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microbiology
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microbiology,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microbiology-0.3.8/README.rst` & `edc-microbiology-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/admin.py` & `edc-microbiology-0.3.9/edc_microbiology/admin.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/auth_objects.py` & `edc-microbiology-0.3.9/edc_microbiology/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/choices.py` & `edc-microbiology-0.3.9/edc_microbiology/choices.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/fieldsets.py` & `edc-microbiology-0.3.9/edc_microbiology/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/form_validators.py` & `edc-microbiology-0.3.9/edc_microbiology/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0001_initial.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0002_auto_20220223_2236.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0002_auto_20220223_2236.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0003_auto_20220223_2256.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0003_auto_20220223_2256.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0004_auto_20220223_2258.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0004_auto_20220223_2258.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0005_auto_20220224_1509.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0005_auto_20220224_1509.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0006_auto_20220224_1826.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0006_auto_20220224_1826.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0007_auto_20220224_1910.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0007_auto_20220224_1910.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0008_auto_20220224_1926.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0008_auto_20220224_1926.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0009_auto_20220711_1230.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0009_auto_20220711_1230.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0010_alter_microbiology_options_and_more.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0010_alter_microbiology_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0011_alter_microbiology_options_and_more.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0011_alter_microbiology_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/migrations/0012_alter_historicalmicrobiology_site_and_more.py` & `edc-microbiology-0.3.9/edc_microbiology/migrations/0012_alter_historicalmicrobiology_site_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/blood_culture.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/blood_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/csf_genexpert.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/csf_genexpert.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/histopathology.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/histopathology.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_afb.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_afb.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_culture.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/sputum_genexpert.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/sputum_genexpert.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/urinary_lam.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/urinary_lam.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/model_mixins/urine_culture.py` & `edc-microbiology-0.3.9/edc_microbiology/model_mixins/urine_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/modeladmin_mixins/microbiology.py` & `edc-microbiology-0.3.9/edc_microbiology/modeladmin_mixins/microbiology.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/models.py` & `edc-microbiology-0.3.9/edc_microbiology/models.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-local-private.pem` & `edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/tests/etc/user-rsa-restricted-private.pem` & `edc-microbiology-0.3.9/edc_microbiology/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology/tests/tests/test_form.py` & `edc-microbiology-0.3.9/edc_microbiology/tests/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/edc_microbiology.egg-info/PKG-INFO` & `edc-microbiology-0.3.9/edc_microbiology.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microbiology
-Version: 0.3.8
+Version: 0.3.9
 Summary: Microbiology model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microbiology
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microbiology,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microbiology-0.3.8/edc_microbiology.egg-info/SOURCES.txt` & `edc-microbiology-0.3.9/edc_microbiology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/microbiology_app/models.py` & `edc-microbiology-0.3.9/microbiology_app/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import date
 
 from django.db import models
 from django.db.models import PROTECT
+from edc_consent.managers import ConsentObjectsByCdefManager, CurrentSiteByCdefManager
 from edc_consent.model_mixins import ConsentVersionModelMixin
 from edc_crf.model_mixins import CrfModelMixin
 from edc_identifier.managers import SubjectIdentifierManager
 from edc_identifier.model_mixins import NonUniqueSubjectIdentifierModelMixin
 from edc_model.models import BaseUuidModel
 from edc_registration.model_mixins import UpdatesOrCreatesRegistrationModelMixin
 from edc_screening.model_mixins import ScreeningModelMixin
@@ -34,14 +35,17 @@
 
     confirm_identity = models.CharField(max_length=25)
 
     dob = models.DateField(default=date(1995, 1, 1))
 
 
 class SubjectConsentV1(SubjectConsent):
+    objects = ConsentObjectsByCdefManager()
+    on_site = CurrentSiteByCdefManager()
+
     class Meta:
         proxy = True
 
 
 class SubjectScreening(ScreeningModelMixin, BaseUuidModel):
     consent_definition = consent_v1
     objects = SubjectIdentifierManager()
```

### Comparing `edc-microbiology-0.3.8/microbiology_app/visit_schedule.py` & `edc-microbiology-0.3.9/microbiology_app/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/pyproject.toml` & `edc-microbiology-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/runtests.py` & `edc-microbiology-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.3.8/setup.cfg` & `edc-microbiology-0.3.9/setup.cfg`

 * *Files identical despite different names*

