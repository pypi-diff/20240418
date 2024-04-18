# Comparing `tmp/django-jalali-6.2.0.tar.gz` & `tmp/django_jalali-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jalali-6.2.0.tar", last modified: Fri Mar 29 16:24:49 2024, max compression
+gzip compressed data, was "django_jalali-6.2.1.tar", last modified: Thu Apr 18 13:59:12 2024, max compression
```

## Comparing `django-jalali-6.2.0.tar` & `django_jalali-6.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.861552 django-jalali-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-29 16:24:43.000000 django-jalali-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-29 16:24:43.000000 django-jalali-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-03-29 16:24:49.861552 django-jalali-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-03-29 16:24:43.000000 django-jalali-6.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.849552 django-jalali-6.2.0/django_jalali/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.849552 django-jalali-6.2.0/django_jalali/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/admin/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/admin/filterspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/admin/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/serializers/serializerfield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.849552 django-jalali-6.2.0/django_jalali/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/static/admin/css/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/default.htm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    45960 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
--rw-r--r--   0 runner    (1001) docker     (127)    93107 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   140036 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
--rw-r--r--   0 runner    (1001) docker     (127)    77969 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.849552 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.853552 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.857552 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/animated-overlay.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/icon-calendar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_flat_30_cccccc_40x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_flat_50_5c5c5c_40x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_20_555555_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_40_0078a3_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_gloss-wave_25_333333_500x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_inset-soft_25_000000_1x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_inset-soft_30_f58400_1x100.png
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_a83300_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)    28561 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    17109 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery.ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/static/admin/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.857552 django-jalali-6.2.0/django_jalali/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-29 16:24:43.000000 django-jalali-6.2.0/django_jalali/templatetags/jformat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.857552 django-jalali-6.2.0/django_jalali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 16:24:49.000000 django-jalali-6.2.0/django_jalali.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-29 16:24:49.861552 django-jalali-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-29 16:24:43.000000 django-jalali-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:24:49.857552 django-jalali-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-29 16:24:43.000000 django-jalali-6.2.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-29 16:24:43.000000 django-jalali-6.2.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-29 16:24:43.000000 django-jalali-6.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-29 16:24:43.000000 django-jalali-6.2.0/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-29 16:24:43.000000 django-jalali-6.2.0/tests/test_templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.393978 django_jalali-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 13:59:08.000000 django_jalali-6.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 13:59:08.000000 django_jalali-6.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-18 13:59:12.393978 django_jalali-6.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-18 13:59:08.000000 django_jalali-6.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.381978 django_jalali-6.2.1/django_jalali/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.381978 django_jalali-6.2.1/django_jalali/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/admin/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/admin/filterspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/admin/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16913 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/serializers/serializerfield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.381978 django_jalali-6.2.1/django_jalali/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/static/admin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/default.htm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    45960 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js
+-rw-r--r--   0 runner    (1001) docker     (127)    93107 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140036 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77969 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.381978 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.385979 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.389979 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/animated-overlay.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/icon-calendar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_flat_30_cccccc_40x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_flat_50_5c5c5c_40x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_20_555555_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_40_0078a3_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_40_ffc73d_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_gloss-wave_25_333333_500x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_inset-soft_25_000000_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_inset-soft_30_f58400_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_4b8e0b_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_a83300_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cccccc_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28561 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17109 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery.ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/static/admin/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.389979 django_jalali-6.2.1/django_jalali/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 13:59:08.000000 django_jalali-6.2.1/django_jalali/templatetags/jformat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.393978 django_jalali-6.2.1/django_jalali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:59:12.000000 django_jalali-6.2.1/django_jalali.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 13:59:12.393978 django_jalali-6.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 13:59:08.000000 django_jalali-6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:59:12.393978 django_jalali-6.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-18 13:59:08.000000 django_jalali-6.2.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-18 13:59:08.000000 django_jalali-6.2.1/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-18 13:59:08.000000 django_jalali-6.2.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-18 13:59:08.000000 django_jalali-6.2.1/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-18 13:59:08.000000 django_jalali-6.2.1/tests/test_templatetags.py
```

### Comparing `django-jalali-6.2.0/LICENSE` & `django_jalali-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/PKG-INFO` & `django_jalali-6.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalali
-Version: 6.2.0
+Version: 6.2.1
 Summary: Jalali Date support for Django model and admin interface
 Home-page: http://github.com/slashmili/django-jalali
 Download-URL: http://github.com/slashmili/django-jalali/tarball/master
 Author: Milad Rastian
 Author-email: eslashmili@gmail.com
 License: Python Software Foundation License
 Keywords: django jalali
@@ -57,14 +57,20 @@
 
 -  jdatetime_
 -  Django_ > 3.2
 
     Looking for Django 1.X support? Checkout *2.4.6* version in pypi.org
 - `Django REST Framework`_ > 3.12 (If install with ``drf`` dependency)
 
+Supported Databases
+-------------------
+
+- SQLite
+- PostgreSQL
+
 Install
 -------
 .. code:: bash
 
    pip install django_jalali
 
 To use DRF serializer field:
```

### Comparing `django-jalali-6.2.0/README.rst` & `django_jalali-6.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 -  jdatetime_
 -  Django_ > 3.2
 
     Looking for Django 1.X support? Checkout *2.4.6* version in pypi.org
 - `Django REST Framework`_ > 3.12 (If install with ``drf`` dependency)
 
+Supported Databases
+-------------------
+
+- SQLite
+- PostgreSQL
+
 Install
 -------
 .. code:: bash
 
    pip install django_jalali
 
 To use DRF serializer field:
```

### Comparing `django-jalali-6.2.0/django_jalali/admin/__init__.py` & `django_jalali-6.2.1/django_jalali/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/admin/filters.py` & `django_jalali-6.2.1/django_jalali/admin/filters.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
         now = jdatetime.datetime.fromgregorian(datetime=timezone.now())
         if timezone.is_aware(now):
             now = timezone.localtime(now)
 
         if isinstance(field, models.jDateTimeField):
             today = now.replace(hour=0, minute=0, second=0, microsecond=0)
+            format = "%Y-%m-%d %H:%M:%S"
         else:
+            format = "%Y-%m-%d"
             today = now.date()
 
         tomorrow = today + jdatetime.timedelta(days=1)
 
         if today.month == 12:
             next_month = today.replace(year=today.year + 1, month=1, day=1)
         else:
@@ -36,43 +38,41 @@
         self.lookup_kwarg_since = "%s__gte" % field_path
         self.lookup_kwarg_until = "%s__lt" % field_path
         self.links = (
             (_("Any date"), {}),
             (
                 _("Today"),
                 {
-                    self.lookup_kwarg_since: today.strftime("%Y-%m-%d %H:%M:%S"),
-                    self.lookup_kwarg_until: tomorrow.strftime("%Y-%m-%d %H:%M:%S"),
+                    self.lookup_kwarg_since: today.strftime(format),
+                    self.lookup_kwarg_until: tomorrow.strftime(format),
                 },
             ),
             (
                 _("Past 7 days"),
                 {
                     self.lookup_kwarg_since: (
                         today - jdatetime.timedelta(days=7)
-                    ).strftime("%Y-%m-%d %H:%M:%S"),
-                    self.lookup_kwarg_until: tomorrow.strftime("%Y-%m-%d %H:%M:%S"),
+                    ).strftime(format),
+                    self.lookup_kwarg_until: tomorrow.strftime(format),
                 },
             ),
             (
                 _("This month"),
                 {
-                    self.lookup_kwarg_since: (today.replace(day=1)).strftime(
-                        "%Y-%m-%d %H:%M:%S"
-                    ),
-                    self.lookup_kwarg_until: next_month.strftime("%Y-%m-%d %H:%M:%S"),
+                    self.lookup_kwarg_since: (today.replace(day=1)).strftime(format),
+                    self.lookup_kwarg_until: next_month.strftime(format),
                 },
             ),
             (
                 _("This year"),
                 {
                     self.lookup_kwarg_since: (today.replace(month=1, day=1)).strftime(
-                        "%Y-%m-%d %H:%M:%S"
+                        format
                     ),
-                    self.lookup_kwarg_until: next_year.strftime("%Y-%m-%d %H:%M:%S"),
+                    self.lookup_kwarg_until: next_year.strftime(format),
                 },
             ),
         )
 
         super().__init__(field, request, params, model, model_admin, field_path)
 
     def queryset(self, request, queryset):
```

### Comparing `django-jalali-6.2.0/django_jalali/admin/filterspecs.py` & `django_jalali-6.2.1/django_jalali/admin/filterspecs.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/admin/widgets.py` & `django_jalali-6.2.1/django_jalali/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/db/models.py` & `django_jalali-6.2.1/django_jalali/db/models.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/forms/__init__.py` & `django_jalali-6.2.1/django_jalali/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/forms/widgets.py` & `django_jalali-6.2.1/django_jalali/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/serializers/serializerfield.py` & `django_jalali-6.2.1/django_jalali/serializers/serializerfield.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/default.htm` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/default.htm`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.all.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/calendar.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery-1.10.2.min.map`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.core.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc-fa.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/scripts/jquery.ui.datepicker-cc.js`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/.DS_Store` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/animated-overlay.gif` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/icon-calendar.svg` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_gloss-wave_25_333333_500x100.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-bg_gloss-wave_25_333333_500x100.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_222222_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_454545_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_4b8e0b_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_4b8e0b_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_a83300_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_a83300_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cccccc_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_cccccc_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.css` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery.ui.theme.css` & `django_jalali-6.2.1/django_jalali/static/admin/jquery.ui.datepicker.jalali/themes/base/jquery.ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali/templatetags/jformat.py` & `django_jalali-6.2.1/django_jalali/templatetags/jformat.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/django_jalali.egg-info/PKG-INFO` & `django_jalali-6.2.1/django_jalali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jalali
-Version: 6.2.0
+Version: 6.2.1
 Summary: Jalali Date support for Django model and admin interface
 Home-page: http://github.com/slashmili/django-jalali
 Download-URL: http://github.com/slashmili/django-jalali/tarball/master
 Author: Milad Rastian
 Author-email: eslashmili@gmail.com
 License: Python Software Foundation License
 Keywords: django jalali
@@ -57,14 +57,20 @@
 
 -  jdatetime_
 -  Django_ > 3.2
 
     Looking for Django 1.X support? Checkout *2.4.6* version in pypi.org
 - `Django REST Framework`_ > 3.12 (If install with ``drf`` dependency)
 
+Supported Databases
+-------------------
+
+- SQLite
+- PostgreSQL
+
 Install
 -------
 .. code:: bash
 
    pip install django_jalali
 
 To use DRF serializer field:
```

### Comparing `django-jalali-6.2.0/django_jalali.egg-info/SOURCES.txt` & `django_jalali-6.2.1/django_jalali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/setup.cfg` & `django_jalali-6.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-jalali
-version = 6.2.0
+version = 6.2.1
 description = Jalali Date support for Django model and admin interface
 url = http://github.com/slashmili/django-jalali
 download_url = http://github.com/slashmili/django-jalali/tarball/master
 author = Milad Rastian
 author_email = eslashmili@gmail.com
 keywords = django jalali
 license = Python Software Foundation License
```

### Comparing `django-jalali-6.2.0/tests/test_admin.py` & `django_jalali-6.2.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/tests/test_forms.py` & `django_jalali-6.2.1/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/tests/test_models.py` & `django_jalali-6.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/tests/test_serializer.py` & `django_jalali-6.2.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `django-jalali-6.2.0/tests/test_templatetags.py` & `django_jalali-6.2.1/tests/test_templatetags.py`

 * *Files identical despite different names*

