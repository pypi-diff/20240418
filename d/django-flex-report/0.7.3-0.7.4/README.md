# Comparing `tmp/django-flex-report-0.7.3.tar.gz` & `tmp/django-flex-report-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.7.3.tar", last modified: Thu Apr 18 14:37:15 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.4.tar", last modified: Thu Apr 18 14:37:53 2024, max compression
```

## Comparing `django-flex-report-0.7.3.tar` & `django-flex-report-0.7.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:15.453499 django-flex-report-0.7.3/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.3/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.3/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:37:15.453499 django-flex-report-0.7.3/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:15.449499 django-flex-report-0.7.3/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:15.449499 django-flex-report-0.7.3/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1819 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 14:37:15.000000 django-flex-report-0.7.3/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4066 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:15.449499 django-flex-report-0.7.3/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    13811 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:15.449499 django-flex-report-0.7.3/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1673 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    25046 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11192 2024-04-18 14:36:56.000000 django-flex-report-0.7.3/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.3/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.3/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 14:37:15.453499 django-flex-report-0.7.3/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.3/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.4/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.4/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1819 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 14:37:53.000000 django-flex-report-0.7.4/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4710 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4066 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    13811 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    25046 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11192 2024-04-18 14:37:43.000000 django-flex-report-0.7.4/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.4/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.4/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 14:37:53.804138 django-flex-report-0.7.4/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.4/setup.py
```

### Comparing `django-flex-report-0.7.3/LICENSE` & `django-flex-report-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/MANIFEST.in` & `django-flex-report-0.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/PKG-INFO` & `django-flex-report-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.3/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.4/django_flex_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.3/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.4/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/__init__.py` & `django-flex-report-0.7.4/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/admin.py` & `django-flex-report-0.7.4/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/app_settings.py` & `django-flex-report-0.7.4/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/constants.py` & `django-flex-report-0.7.4/flex_report/constants.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/fields.py` & `django-flex-report-0.7.4/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/filterset.py` & `django-flex-report-0.7.4/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/forms.py` & `django-flex-report-0.7.4/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.4/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.4/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.4/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.4/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.4/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.4/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.4/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.4/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.4/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.4/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.4/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.7.4/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/mixins.py` & `django-flex-report-0.7.4/flex_report/mixins.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/models.py` & `django-flex-report-0.7.4/flex_report/models.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.4/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/urls.py` & `django-flex-report-0.7.4/flex_report/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 VIEWS = app_settings.VIEWS
 
 
 app_name = "flex_report"
 template_urls = [
     path("", VIEWS["TEMPLATE_LIST"], name="index"),
-    path("export/", VIEWS["GENERAL_QS_EXPORT"], name="index"),
+    path("export/", VIEWS["GENERAL_QS_EXPORT"], name="export"),
     path(
         "new/",
         VIEWS["TEMPLATE_CREATE_INIT"],
         name="create",
     ),
     path(
         "new/<int:pk>/",
```

### Comparing `django-flex-report-0.7.3/flex_report/utils.py` & `django-flex-report-0.7.4/flex_report/utils.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/flex_report/views.py` & `django-flex-report-0.7.4/flex_report/views.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.3/pyproject.toml` & `django-flex-report-0.7.4/pyproject.toml`

 * *Files identical despite different names*

