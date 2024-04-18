# Comparing `tmp/django-flex-report-0.6.7.tar.gz` & `tmp/django-flex-report-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.6.7.tar", last modified: Mon Apr 15 12:57:23 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.0.tar", last modified: Thu Apr 18 09:39:35 2024, max compression
```

## Comparing `django-flex-report-0.6.7.tar` & `django-flex-report-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1627 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.000964 django-flex-report-0.6.7/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1568 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-15 12:57:22.000000 django-flex-report-0.6.7/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4764 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2139 2024-04-15 12:53:15.000000 django-flex-report-0.6.7/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3118 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    13307 2024-04-15 12:54:34.000000 django-flex-report-0.6.7/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8341 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5671 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    24649 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11116 2024-04-10 14:31:59.000000 django-flex-report-0.6.7/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-15 12:57:23.004963 django-flex-report-0.6.7/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.6.7/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 09:39:35.802260 django-flex-report-0.7.0/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.0/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.0/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 09:39:35.798258 django-flex-report-0.7.0/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 09:39:35.798258 django-flex-report-0.7.0/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 09:39:35.798258 django-flex-report-0.7.0/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1819 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 09:39:35.000000 django-flex-report-0.7.0/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4633 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3990 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 09:39:35.798258 django-flex-report-0.7.0/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    13440 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 09:39:35.798258 django-flex-report-0.7.0/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    25046 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11064 2024-04-18 09:38:37.000000 django-flex-report-0.7.0/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.0/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.0/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 09:39:35.802260 django-flex-report-0.7.0/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.0/setup.py
```

### Comparing `django-flex-report-0.6.7/LICENSE` & `django-flex-report-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/MANIFEST.in` & `django-flex-report-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/PKG-INFO` & `django-flex-report-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.6.7
+Version: 0.7.0
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.6.7/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.0/django_flex_report.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.6.7
+Version: 0.7.0
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.6.7/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.0/django_flex_report.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -35,10 +35,12 @@
 flex_report/migrations/0008_template_buttons.py
 flex_report/migrations/0009_alter_template_buttons.py
 flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
 flex_report/migrations/0011_alter_template_model_user_path.py
 flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
 flex_report/migrations/0013_column_column_type.py
 flex_report/migrations/0014_alter_column_column_type.py
+flex_report/migrations/0015_remove_column_column_type.py
+flex_report/migrations/0016_column_column_type.py
 flex_report/migrations/__init__.py
 flex_report/templatetags/__init__.py
 flex_report/templatetags/flex_report_filters.py
```

### Comparing `django-flex-report-0.6.7/flex_report/__init__.py` & `django-flex-report-0.7.0/flex_report/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,30 +3,36 @@
 import contextlib
 
 import django.db.models.options as options
 from django_filters import utils as django_filter_utils
 from django.utils.translation import gettext as _
 
 from ._version import get_version
-from .constants import META_REPORT_KEY, BaseExportFormat, ReportModel
+from .constants import META_REPORT_KEY, BaseExportFormat, BaseQuerysetExporter, ReportModel, BaseDynamicField, DynamicSubField
 
 options.DEFAULT_NAMES = options.DEFAULT_NAMES + (META_REPORT_KEY,)
 
 
 export_format = BaseExportFormat
-
+queryset_exporter = BaseQuerysetExporter
 report_model = ReportModel
+dynamic_field = BaseDynamicField
 
 
 __version__ = get_version()
 __all__ = [
     "ReportModel",
     "report_model",
     "BaseExportFormat",
     "export_format",
+    "queryset_exporter",
+    "BaseQuerysetExporter",
+    "BaseDynamicField",
+    "DynamicSubField",
+    "dynamic_field",
 ]
 
 
 _verbose_field_name = copy.deepcopy(django_filter_utils.verbose_field_name)
 
 
 def verbose_field_name(model, field_name):
```

### Comparing `django-flex-report-0.6.7/flex_report/admin.py` & `django-flex-report-0.7.0/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/app_settings.py` & `django-flex-report-0.7.0/flex_report/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,14 @@
         return self._settings("DEFAULT_CELL_VALUE", "&mdash;")
 
     @property
     def EDITORS_GROUP_NAME(self):
         return self._settings("EDITORS_GROUP_NAME", "report_editors")
 
     @property
-    def DYNAMIC_FIELD_FUNC_PREFIX(self):
-        return self._settings("DYNAMIC_FIELD_FUNC_PREFIX", "get_dynamic_")
-
-    @property
     def TIME_FORMATS(self):
         dflt = time_formats = {
             models.DateTimeField: "%H:%M %Y/%m/%d",
             models.DateField: "%Y/%m/%d",
             models.TimeField: "%H:%M:%S",
             jmodels.jDateField: "%H:%M:%S",
             jmodels.jDateTimeField: "%H:%M %Y/%m/%d",
```

### Comparing `django-flex-report-0.6.7/flex_report/fields.py` & `django-flex-report-0.7.0/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/filterset.py` & `django-flex-report-0.7.0/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/forms.py` & `django-flex-report-0.7.0/flex_report/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,30 +53,14 @@
                     attrs={"class": "selectize-field"}
                 ),
                 required=True,
                 label=_("columns"),
                 initial=col_initial,
                 choices=list(get_model_columns(model).items()),
             ),
-            "users": forms.ModelMultipleChoiceField(
-                widget=forms.MultipleChoiceField.widget(
-                    attrs={"class": "selectize-field"}
-                ),
-                required=False,
-                queryset=get_user_model().objects.all(),
-                label=_("Users"),
-            ),
-            "groups": forms.ModelMultipleChoiceField(
-                widget=forms.MultipleChoiceField.widget(
-                    attrs={"class": "selectize-field"}
-                ),
-                required=False,
-                queryset=Group.objects.all(),
-                label=_("Groups"),
-            ),
         },
     )
 
 
 def generate_column_create_form(form):
     form.fields["model"].queryset = ContentType.objects.filter(
         pk__in=[m.pk for m in get_report_models().values()]
```

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.0/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.0/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.0/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.0/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.0/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.0/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.0/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.0/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.0/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.0/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.0/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/mixins.py` & `django-flex-report-0.7.0/flex_report/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 from functools import partial
 from logging import getLogger
 
 from django.core.exceptions import PermissionDenied
 from django.db.models import Subquery
 from django.core.paginator import EmptyPage, Paginator
 from django.http import HttpResponseBadRequest, HttpResponseForbidden
-from django.shortcuts import HttpResponse, redirect
+from django.shortcuts import HttpResponse
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import View
 
-from flex_report import export_format
+from flex_report import export_format, queryset_exporter, BaseExportFormat
 
 from .app_settings import app_settings
 from .templatetags.flex_report_filters import get_column_verbose_name
 from .filterset import (
     generate_filterset_from_model,
     generate_quicksearch_filterset_from_model,
 )
 from .models import Template
 from .utils import (
     generate_filterset_form,
     get_template_columns,
     get_choice_field_choices,
     string_to_q,
+    FieldTypes
 )
 
 logger = getLogger(__file__)
 
 
 class PaginationMixin(View):
     pages = [25, 75, 100, 200]
@@ -103,15 +104,14 @@
         pass
 
     def template_not_ready(self):
         pass
 
 
 class QuerySetExportMixin(View):
-    valid_file_exports = ["xls", "csv", "pdf"]
     export_format = None
     export_file_name = None
     export_qs = None
     export_columns = None
     export_headers = None
     sheet_name = None
 
@@ -130,37 +130,42 @@
             "columns": self.get_export_columns(),
             "headers": self.get_export_headers(),
         }
 
     def dispatch(self, *args, **kwargs):
         if not self.export_format and (
             not (format_ := self.request.GET.get("format", "").lower())
-            or format_ not in self.valid_file_exports
+            or format_ not in queryset_exporter.exporters.keys()
         ):
             return HttpResponseBadRequest()
+        
         self.export_format = self.export_format or format_
+        
         return super().dispatch(*args, **kwargs)
+    
+    def get_exporter(self) -> BaseExportFormat:
+        try:
+            return export_format.formats[self.export_format]
+        except KeyError as e:
+            raise NotImplementedError(f"The wanted format '{self.export_format}' isn't handled.") from e
+        
+    def get_export_file_name(self):
+        return self.export_file_name
 
     def get(self, *args, **kwargs):
-        filename = f"{self.export_file_name and f'{self.export_file_name}.' or ''}{self.export_format}"
         response = HttpResponse(
             content_type=mimetypes.types_map.get(
                 f".{self.export_format}",
                 "application/octet-stream",
             ),
             headers={"Content-Disposition": f'attachment; filename="{filename}"'},
         )
-
-        try:
-            format_ = export_format.formats[self.export_format]
-        except KeyError:
-            logger.critical(f"The wanted format '{self.export_format}' isn't handled.")
-            return redirect(self.request.META.get("HTTP_REFERER", "/"))
-
-        print(self.get_handle_kwargs())
+        
+        format_ = self.get_exporter()
+        filename = f"{self.get_export_file_name()}{format_.format_ext}"
         response = format_.handle_response(
             response=response,
             **self.get_handle_kwargs(),
         )
 
         return response
 
@@ -209,17 +214,15 @@
             self.report_model, list(self.template_searchable_fields.values())
         )(initials)
 
     def apply_user_path(self):
         LOGICAL_OPERATORS = ["()", "&", "|", "!="]
         paths = self.template_object.model_user_path or {}
         path_func = getattr(
-            self.report_model,
-            app_settings.MODEL_USER_PATH_FUNC_NAME,
-            lambda request: {},
+            self.report_model, app_settings.MODEL_USER_PATH_FUNC_NAME, lambda request: {}
         )
 
         accessed_paths = {
             path_name: path_dict
             for path_name, path in paths.items()
             if (
                 path_dict := {
@@ -237,131 +240,122 @@
             else list(filter(partial(ne, "__all__"), accessed_paths))[0]
         )
         if accessed_path == "__all__":
             return
 
         accessed_path, accessed_val = accessed_paths[accessed_path].popitem()
         if not any(map(lambda op: op in accessed_path, LOGICAL_OPERATORS)):
-            self.report_qs = self.report_qs.filter(**{accessed_path: accessed_val})
+            self.report_qs = self.report_qs.filter(
+                **{accessed_path: accessed_val}
+            ).distinct()
             return
 
-        self.report_qs = self.report_qs.filter(string_to_q(accessed_path, accessed_val))
-
+        self.report_qs = self.report_qs.filter(
+            string_to_q(accessed_path, accessed_val)
+        ).distinct()
+        
     def _format_used_filter(self, col_name, val):
         formats = {
             **{k: "بله" for k in ["true", "True", True]},
             **{k: "خیر" for k in ["false", "False", False]},
         }
-
+        
         if formatted_val := formats.get(val, False):
             return formatted_val
 
         if choices := get_choice_field_choices(self.report_model, col_name):
             return dict(choices).get(val, val)
 
         return str(val)
 
-    def used_filter_format(self, col_name, val):
+    def used_filter_format(self, col_name, val):        
         if isinstance(val, list):
             return ", ".join(
                 map(
                     lambda v: self._format_used_filter(col_name, v),
                     val,
                 )
             )
-
+            
         return self._format_used_filter(col_name, val) or val
 
     def setup(self, request, *args, **kwargs):
         super().setup(request, *args, **kwargs)
 
         obj = self.template_object
         if not obj:
             self.have_template = False
             return
 
         self.report_model = obj.model.model_class()
-        self.template_columns = get_template_columns(obj)
+        self.template_columns = get_template_columns(obj, as_dict=False)
         self.template_searchable_fields = get_template_columns(obj, searchables=True)
 
         self.get_filters()
-        self.report_qs = methodcaller(
-            "none" if self.template_filters.get_filters() else "all"
-        )(self.report_model.objects)
+        self.report_qs = methodcaller("none" if self.template_filters.get_filters() else "all")(self.report_model.objects)
         self.apply_user_path()
-
-        if all(
-            map(
-                methodcaller("get_filters"),
-                [self.filters, self.quicksearch, self.template_filters],
-            )
-        ) and all(
-            map(
-                methodcaller("is_valid"),
-                [self.filters, self.quicksearch, self.template_filters],
-            )
+        
+        if (
+            all(map(methodcaller("get_filters"), [self.filters, self.quicksearch, self.template_filters]))
+            and all(map(methodcaller("is_valid"), [self.filters, self.quicksearch, self.template_filters]))
         ):
             self.report_qs = self.template_filters.qs.distinct().filter(
                 pk__in=Subquery(
                     (
                         self.quicksearch.qs.distinct() & self.filters.qs.distinct()
                     ).values("pk")
                 )
             )
 
             self.report_qs = self.report_qs.distinct().order_by(
                 *self.report_model._meta.ordering or ["pk"]
             )
-
+            
             cleaned_data = (
                 self.quicksearch.form.cleaned_data | self.filters.form.cleaned_data
             )
             self.used_filters = self.get_used_filters(
                 {
-                    get_column_verbose_name(
-                        self.report_model, k
-                    ): self.used_filter_format(k, v)
+                    get_column_verbose_name(self.report_model, k): self.used_filter_format(
+                        k, v
+                    )
                     for k, v in cleaned_data.items()
                     if bool(v)
                 }
             )
 
     def get_used_filters(self, cleaned_data):
         return _(" and ").join(
             [
                 f'{k} = {",".join(map(str, v)) if isinstance(v, list) else v}'
                 for k, v in cleaned_data.items()
                 if str(k).lower() != "search"
             ]
         )
-
+        
     def _prepare_initial(self, initial):
         if initial.lower() in ["true", "false"]:
             return initial.lower() == "true"
 
-        if (initial.startswith("[") and initial.endswith("]")) or (
-            not initial.startswith("0") and initial.isnumeric()
-        ):
+        if (initial.startswith("[") and initial.endswith("]")) or (not initial.startswith("0") and initial.isnumeric()):
             return ast.literal_eval(initial)
 
     def get_initial_value(self, initial, *, key=""):
         initial = str(initial)
 
         if key.endswith("__in"):
             return list(map(self._prepare_initial, self.request.GET.getlist(key)))
 
         return self._prepare_initial(initial)
 
     def get_initials(self):
         return {
             k: self.get_initial_value(v, key=k)
             for k, v in self.request.GET.dict().items()
-            if str(v)
-            and v.strip() not in self.ignore_search_values
-            and k.lower() != "search"
+            if str(v) and v.strip() not in self.ignore_search_values and k.lower() != "search"
         }
 
     def get_form_classes(self):
         if not self.template_object:
             return []
         return [generate_filterset_form(self.report_model)]
 
@@ -374,29 +368,30 @@
         else:
             return super(TemplateObjectMixin, self).get_context_data(**kwargs)
 
         context["report"] = {
             "columns": self.template_columns,
             "columns_count": len(self.template_columns)
             + self.template_object.buttons.count()
+            + sum(len(field.get_dynamic_obj().unpack_field()) for field in self.template_columns.filter(column_type=FieldTypes.dynamic).only("pk"))
             + 1,
             "filters": self.filters,
             "buttons": self.template_object.buttons.all(),
             "searchable_fields": self.template_searchable_fields,
             "quicksearch": self.quicksearch,
             "used_filters": self.used_filters,
             "template": self.template_object,
             "templates": self.get_page_templates(),
             "initials": self.get_initials(),
             "pagination": self.pagination,
             "page_template_keyword": self.page_template_keyword,
             "is_page_table": self.is_page_table,
             "have_template": self.have_template,
             "export_formats": [
-                {"name": format_.format_name, "slug": format_.format_slug, "ext": (format_.format_ext or format_.format_slug)}
+                {"name": format_.format_name, "slug": format_.format_slug}
                 for format_ in export_format.formats.values()
             ],
             "page_title": getattr(
                 self.template_object.page, "title", self.template_object.title
             ),
         }
         return context
```

### Comparing `django-flex-report-0.6.7/flex_report/models.py` & `django-flex-report-0.7.0/flex_report/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from django.db.models import F
 from django.template.defaultfilters import truncatechars
 from django.utils.translation import gettext_lazy as _
 from django_better_admin_arrayfield.models.fields import ArrayField
 from django_jalali.db.models import jDateTimeField
 from sortedm2m.fields import SortedManyToManyField
 
-from flex_report import report_model
+from flex_report import report_model, dynamic_field, BaseDynamicField
 
 from .managers import ColumnManager
-from .utils import get_view_name_url, is_field_valid
+from .utils import get_view_name_url, is_field_valid, get_column_type
+from .constants import FieldTypes
 
 
 class TablePage(models.Model):
     title = models.CharField(max_length=200, verbose_name=_("Title"))
     url_name = models.CharField(max_length=200, verbose_name=_("URL Name"))
     users = models.ManyToManyField(
         settings.AUTH_USER_MODEL,
@@ -37,17 +38,17 @@
 
     def __str__(self):
         return f"{self.title}"
 
 
 class Column(models.Model):
     class COLUMN_TYPES(models.TextChoices):
+        model =  "model", _("Model")
         dynamic = "dynamic", _("Dynamic")
-        model = "model", _("model")
-
+    
     title = models.CharField(verbose_name=_("Title"), max_length=150, db_index=True)
     searchable = models.BooleanField(default=False)
     creator = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
         related_name="created_columns",
         blank=True,
@@ -64,34 +65,32 @@
         blank=True,
     )
     model = models.ForeignKey(
         ContentType,
         on_delete=models.CASCADE,
         related_name="flex_columns",
     )
-    column_type = models.CharField(
-        verbose_name=_("Column Type"),
-        choices=COLUMN_TYPES.choices,
-        max_length=10,
-        default=COLUMN_TYPES.model,
-    )
+    column_type = models.CharField(choices=COLUMN_TYPES.choices, verbose_name=_("Column Type"), default=COLUMN_TYPES.model)
 
     objects = ColumnManager()
 
-    def get_column_choices(self):
-        if self.column_type == self.COLUMN_TYPES.model:
-            return {self.id: self.title}
-        
-        return 
-
     def __str__(self):
         return f"{self.model}: {self.title}"
+    
+    def get_dynamic_obj(self) -> None | BaseDynamicField:
+        if self.column_type != self.COLUMN_TYPES.dynamic:
+            return
+        
+        return dynamic_field.get_by_slug(self.title)
 
     def clean(self):
-        if not is_field_valid(self.model.model_class(), self.title):
+        if (column_type:=get_column_type(self.model, self.title)) == FieldTypes.dynamic and self.model != (dynamic_model:=self.get_dynamic_obj().model):
+            raise ValidationError({"title": _("This dynamic column has been registered for another model, which is %(title).") % {"title": dynamic_field}})
+        
+        if column_type and not is_field_valid(self.model.model_class(), self.title):
             raise ValidationError(
                 {
                     "title": _(
                         "The field name is not valid. It should be a field on the model."
                     )
                 }
             )
@@ -289,11 +288,14 @@
     @property
     def filters_count(self):
         return len(list(filter(None, (self.filters or {}).values())))
 
     @property
     def user_fullname(self):
         return getattr(self.creator, "full_name", _("Not Set"))
+        
+    def __str__(self):
+        return self.title
 
     class Meta:
         verbose_name = _("Template")
         verbose_name_plural = _("Templates")
```

### Comparing `django-flex-report-0.6.7/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.0/flex_report/templatetags/flex_report_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django.db import models
 from django.db.models import Model, Q, QuerySet
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 from django.utils.safestring import mark_safe
 
 from flex_report.app_settings import app_settings
-from flex_report.utils import get_column_cell, get_model_field, field_to_db_field
+from flex_report.utils import get_column_cell, get_model_field, field_to_db_field, get_related_property
 
 register = template.Library()
 
 
 @register.filter(name="enumerate")
 def enum(iterable: Iterable):
     return enumerate(iterable)
@@ -119,25 +119,27 @@
 def is_row_value_valid(f, v):
     return v or isinstance(f, models.BooleanField) or v == 0
 
 
 @register.filter
 def get_column_verbose_name(obj, column):
     lookup_exprs = list(map(lambda i: f"__{i}", ["in"]))
+    
     for lookup in filter(lambda i: column.endswith(i), lookup_exprs):
         column = column.rstrip(lookup)
-
+                        
     field_col = getattr(field_to_db_field(obj, column), "verbose_name", False)
-    if (
-        getattr(obj, column, False)
-        and not field_col
-        and (property_col := getattr(getattr(obj, column), "fget", False))
-    ):
-        field_col = getattr(property_col, "verbose_name", False)
-
+    if field_col:
+        return mark_safe(field_col or column.replace("_", "").title())
+        
+    if (field:=getattr(obj, column, False)) and hasattr(field, "fget"):
+        field_col = field.fget.verbose_name
+    elif (field:=get_related_property(obj, column)):
+        field_col = field.fget.verbose_name
+    
     return mark_safe(field_col or column.replace("_", " ").title())
 
 
 @register.filter
 def get_columns_verbose_names(cols: Iterable, obj):
     return list(map(lambda c: get_column_verbose_name(obj, c), cols))
```

### Comparing `django-flex-report-0.6.7/flex_report/urls.py` & `django-flex-report-0.7.0/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.6.7/flex_report/utils.py` & `django-flex-report-0.7.0/flex_report/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from django_filters import FilterSet
 from django_filters.constants import ALL_FIELDS
 from django_filters.utils import LOOKUP_SEP, get_all_model_fields, get_model_field
 from djmoney.models import fields as money_fields
 from djmoney.money import Money
 from phonenumber_field.phonenumber import PhoneNumber
 
-from flex_report import BaseExportFormat, ReportModel, export_format
+from flex_report import BaseExportFormat, ReportModel, export_format, queryset_exporter, BaseQuerysetExporter, dynamic_field
 from flex_report.fields import FieldFileAbsoluteURL
 
 from .app_settings import app_settings
 from .constants import (
     REPORT_CELL_STYLE_MAP,
     REPORT_CUSTOM_FIELDS_KEY,
     REPORT_EXCULDE_KEY,
@@ -285,15 +285,15 @@
         return FieldTypes.field
 
     field = get_model_property(model, column)
 
     if isinstance(field, property):
         return FieldTypes.property
 
-    if callable(field):
+    if field in dynamic_field.fields:
         return FieldTypes.dynamic
 
     return None
 
 
 def get_fields_lookups(model, fields):
     """
@@ -402,24 +402,27 @@
     return type(
         f"{getattr(model, '__name__', '')}DynamicFilterSetForm",
         tuple(form_classes),
         fields,
     )
 
 
-def get_template_columns(template, searchables=False):
+def get_template_columns(template, searchables=False, as_dict=True):
     """
     Takes in a template object and returns an dict of fields and custom fields defined on the model,
     where the keys are the name of the field, and the value is the display name evaluated for the field-name.
     """
     qs = template.columns.all()
     if searchables:
         qs = qs.filter(searchable=True)
 
-    return {col_id: col_title for col_id, col_title in qs.values_list("id", "title")}
+    if as_dict:
+        return {col_id: col_title for col_id, col_title in qs.values_list("id", "title")}
+    
+    return qs
 
 
 def get_column_cell(obj, name, *, absolute_url=True):
     """
     Takes in an object and a column name, and returns the value of the column for the object.
     If the column is a custom field, it returns the value of the custom field.
     """
@@ -466,70 +469,34 @@
             attr = FieldFileAbsoluteURL(file=attr, absolute=absolute_url)
         elif isinstance(field, PhoneNumberField):
             attr = str(attr).replace(" ", "-")
 
     return (attr and str(attr)) or app_settings.DEFAULT_CELL_VALUE
 
 
-@export_format.register
-class ExportXls(BaseExportFormat):
-    format_slug = "xls"
-    format_name = "Excel"
-
-    @classmethod
-    def handle(cls, *args, **kwargs):
-        """
-        Convert queryset or list of rows as dict to XLS file.
-        ### Parameters
-        Get ``columns`` as list of keys to get from object and
-        ``headers`` can be as mapping of column and label for file headers.
-
-        ### Returns
-        ``xlwt.Workbook`` object.
-
-        ### Example
-            >>> response = HttpResponse(....)
-            qs = Users.objects.all()
-            columns = ["first_name", "last_name"]
-            headers = {"first_name": "First Name", "last_name": "Last Name"}
-            wb = export_queryset_to_xls(qs, columns, headers)
-            wb.save(response)
-
-        """
-        headers_name = kwargs.get("headers_name")
-        queryset = kwargs.get("queryset")
-        columns = kwargs.get("columns")
-        cell_fn = kwargs.get("cell_fn")
-        sheet_name = kwargs.get("sheet_name")
-
-        required_args = ["queryset", "columns"]
-        for arg in required_args:
-            if arg not in kwargs:
-                raise TypeError(f"missing required argument: '{arg}'")
-
-        if headers_name is None:
-            headers_name = {}
+@queryset_exporter.register
+class XlsQuerysetExporter(BaseQuerysetExporter):
+    exporter_slug = "xls"
+    
+    def export(self):
+        headers_name = self.export_headers
+        columns = self.export_columns
+        queryset = self.export_qs
+        sheet_name = self.export_kwargs.get("sheet_name")
+        cell_fn = self.export_kwargs.get("cell_fn")
+        
         workbook = xlwt.Workbook(encoding="utf-8")
         default_style = xlwt.XFStyle()
-        sheet = workbook.add_sheet(
-            sheet_name
-            or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet"))
-        )
+        sheet = workbook.add_sheet(sheet_name or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet")))
 
         for num, column in enumerate(columns):
             value = headers_name.get(column, column)
             style = default_style
             if cell_fn:
-                style, value = cell_fn(
-                    obj=None,
-                    row_number=0,
-                    column=column,
-                    style=default_style,
-                    value=value,
-                )
+                style, value = cell_fn(obj=None, row_number=0, column=column, style=default_style, value=value)
             sheet.write(0, num, value, style)
 
         for x, obj in enumerate(queryset, start=1):
             for y, column in enumerate(columns):
                 value = get_column_cell(obj, column)
                 style = default_style
                 for value_type, cell_style in REPORT_CELL_STYLE_MAP:
@@ -537,73 +504,96 @@
                         if callable(cell_style):
                             style = default_style
                             value = cell_style(value)
                         else:
                             style = cell_style
                         break
                 if cell_fn:
-                    style, value = cell_fn(
-                        obj=obj, row_number=x, column=column, style=style, value=value
-                    )
+                    style, value = cell_fn(obj=obj, row_number=x, column=column, style=style, value=value)
                 args = [x, y]
                 if style:
                     args.extend([value, style])
                 else:
                     args.append(value)
                 sheet.write(*args)
 
         return workbook
 
+
+@queryset_exporter.register
+class CsvQuerysetExporter(BaseQuerysetExporter):
+    exporter_slug = "csv"
+    
+    def export(self):
+        headers_name = self.export_headers
+        columns = self.export_columns
+        queryset = self.export_qs
+        
+        output = io.StringIO()
+        writer = csv.writer(output)
+        writer.writerow([headers_name.get(column, column) for column in columns])
+        writer.writerows([[get_column_cell(obj, column) for column in columns] for obj in queryset])
+        
+        return output
+
+
+@export_format.register
+class ExportXls(BaseExportFormat):
+    format_slug = "xls"
+    format_name = "Excel"
+    queryset_exporter = "xls"
+    format_ext = ".xlsx"
+
+    @classmethod
+    def handle(cls, *args, **kwargs):
+        headers_name = kwargs.get("headers_name", {})
+        queryset = kwargs.get("queryset", [])
+        columns = kwargs.get("columns", [])
+        cell_fn = kwargs.get("cell_fn")
+        sheet_name = kwargs.get("sheet_name")
+        required_args = ["queryset", "columns"]
+        for arg in required_args:
+            if arg not in kwargs:
+                raise TypeError(f"missing required argument: '{arg}'")
+    
+        workbook = cls.construct_qs_exporter(
+            export_headers=headers_name,
+            export_columns=columns,
+            export_qs=queryset,
+            export_kwargs={"sheet_name": sheet_name, "cell_fn": cell_fn},
+        ).export()
+        return workbook
+
     @classmethod
     def handle_response(cls, response, *args, **kwargs):
         wb = cls.handle(*args, **kwargs)
         wb.save(response)
         return response
 
 
 @export_format.register
 class ExportCsv(BaseExportFormat):
     format_slug = "csv"
     format_name = "CSV"
+    queryset_exporter = "csv"
+    format_ext = ".csv"
 
     @classmethod
     def handle(cls, *args, **kwargs):
-        """
-        Convert queryset or list rows as dict to CSV file.
-        ### Parameters
-        Get ``columns`` as list of keys to get from object and
-        ``headers`` can be as mapping of column and label for file headers.
-
-        ### Returns
-        ``io.StringIO`` object.
-
-        ### Example
-            >>> response = HttpResponse(....)
-            qs = Users.objects.all()
-            columns = ["first_name", "last_name"]
-            headers = {"first_name": "First Name", "last_name": "Last Name"}
-            buff = export_queryset_to_csv(qs, columns, headers)
-            response.write(buff.getvalue())
-
-        """
-        if not (queryset := kwargs.get("queryset", False)):
-            raise TypeError("missing required argument: 'queryset'")
-
-        if not (columns := kwargs.get("columns", False)):
-            raise TypeError("missing required argument: 'columns'")
-
-        if (headers := kwargs.get("headers")) is None:
-            headers = {}
-        output = io.StringIO()
-        writer = csv.writer(output)
-        writer.writerow([headers.get(column, column) for column in columns])
-        writer.writerows(
-            [[get_column_cell(obj, column) for column in columns] for obj in queryset]
-        )
-        return output
+        headers_name = kwargs.get("headers_name", {})
+        queryset = kwargs.get("queryset", [])
+        columns = kwargs.get("columns", [])
+        cell_fn = kwargs.get("cell_fn")
+        
+        return cls.construct_qs_exporter(
+            export_headers=headers_name,
+            export_columns=columns,
+            export_qs=queryset,
+            export_kwargs={"cell_fn": cell_fn},
+        ).export()
 
     @classmethod
     def handle_response(cls, response, *args, **kwargs):
         buff = cls.handle(*args, **kwargs)
         response.write(buff.getvalue())
         return response
 
@@ -755,7 +745,35 @@
 
     tree = ast.parse(q_str, mode="eval")
 
     builder = QBuilder()
     q_obj = builder.visit(tree.body)
 
     return q_obj
+
+
+def get_related_property(model, field_name):
+    fields = field_name.split(LOOKUP_SEP)
+
+    latest_model = model
+    for field in fields[:-1]:
+        field = get_model_field(latest_model, field)
+
+        if isinstance(field, RelatedField):
+            field_model = field.remote_field.model
+        elif isinstance(field, ForeignObjectRel):
+            field_model = field.related_model
+        else:
+            return None
+
+        latest_model = field_model
+
+    property_name = fields[-1]
+
+    if (
+        hasattr(latest_model, property_name)
+        and (field := getattr(latest_model, property_name))
+        and (isinstance(field, property) or callable(field))
+    ):
+        return field
+
+    return None
```

### Comparing `django-flex-report-0.6.7/flex_report/views.py` & `django-flex-report-0.7.0/flex_report/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         return redirect("flex_report:template:edit", pk=self.template_object.pk)
 
 
 template_create_complete_view = TemplateCreateCompleteView.as_view()
 
 
 class TemplateUpdateView(UpdateView, TemplateUpsertViewBase):
-    fields = ["title", "page", "users", "groups"]
+    fields = ["title", "page"]
     template_name_suffix = "_form"
 
     def get_form_classes(self):
         return [
             super(TemplateUpsertViewBase, self).get_form_class(),
             generate_report_create_form(
                 self.template_model,
@@ -319,15 +319,15 @@
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         context.update(
             {
                 "object": self.object,
-                "meta_fields_name": [*self.fields, "columns", "users", "groups"],
+                "meta_fields_name": self.fields,
             }
         )
 
         return context
 
     def get_success_url(self):
         return reverse("flex_report:template:index")
```

### Comparing `django-flex-report-0.6.7/pyproject.toml` & `django-flex-report-0.7.0/pyproject.toml`

 * *Files identical despite different names*

