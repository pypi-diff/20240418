# Comparing `tmp/django-flex-report-0.7.1.tar.gz` & `tmp/django-flex-report-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.7.1.tar", last modified: Thu Apr 18 10:10:18 2024, max compression
+gzip compressed data, was "django-flex-report-0.7.2.tar", last modified: Thu Apr 18 14:34:25 2024, max compression
```

## Comparing `django-flex-report-0.7.1.tar` & `django-flex-report-0.7.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.1/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.1/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 10:10:18.000000 django-flex-report-0.7.1/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1819 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 10:10:17.000000 django-flex-report-0.7.1/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4633 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3990 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    13568 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    25046 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11064 2024-04-18 10:10:08.000000 django-flex-report-0.7.1/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.1/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.1/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 10:10:18.093728 django-flex-report-0.7.1/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.1/setup.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:25.077324 django-flex-report-0.7.2/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.7.2/LICENSE
+-rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.7.2/MANIFEST.in
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:34:25.077324 django-flex-report-0.7.2/PKG-INFO
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:25.077324 django-flex-report-0.7.2/django_flex_report.egg-info/
+-rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/PKG-INFO
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/SOURCES.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/dependency_links.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/not-zip-safe
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/requires.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-04-18 14:34:25.000000 django-flex-report-0.7.2/django_flex_report.egg-info/top_level.txt
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:25.073326 django-flex-report-0.7.2/flex_report/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1819 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-04-18 14:34:24.000000 django-flex-report-0.7.2/flex_report/_version.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/admin.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4633 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/app_settings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/apps.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/choices.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     4066 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/constants.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/fields.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     3985 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/filterset.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2483 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/forms.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/managers.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:25.073326 django-flex-report-0.7.2/flex_report/migrations/
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0001_initial.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0002_alter_column_title.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0004_column_creator.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0005_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0006_tablebutton_query_strings.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0008_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0009_alter_template_buttons.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0011_alter_template_model_user_path.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0013_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      573 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0014_alter_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      343 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0015_remove_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)      547 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/0016_column_column_type.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/migrations/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    13811 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/mixins.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     8813 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/models.py
+drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:25.077324 django-flex-report-0.7.2/flex_report/templatetags/
+-rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/templatetags/__init__.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     5819 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/templatetags/flex_report_filters.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1610 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/urls.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    25046 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/utils.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)    11064 2024-04-18 14:34:10.000000 django-flex-report-0.7.2/flex_report/views.py
+-rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.7.2/pyproject.toml
+-rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.7.2/requirements.txt
+-rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-04-18 14:34:25.077324 django-flex-report-0.7.2/setup.cfg
+-rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.7.2/setup.py
```

### Comparing `django-flex-report-0.7.1/LICENSE` & `django-flex-report-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/MANIFEST.in` & `django-flex-report-0.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/PKG-INFO` & `django-flex-report-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.1/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.7.2/django_flex_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.7.1
+Version: 0.7.2
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.7.1/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.7.2/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/__init__.py` & `django-flex-report-0.7.2/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/admin.py` & `django-flex-report-0.7.2/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/app_settings.py` & `django-flex-report-0.7.2/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/constants.py` & `django-flex-report-0.7.2/flex_report/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,18 @@
     formats = {}
     queryset_exporter = None
     format_slug = None
     format_name = None
     format_ext = None
     
     @classmethod
+    def check_auth(cls, request):
+        return True
+    
+    @classmethod
     def construct_qs_exporter(cls, *args, **kwargs):
         qs_exporter = BaseQuerysetExporter.exporters[cls.queryset_exporter]
         return qs_exporter(*args, **kwargs)
 
     @classmethod
     def __str__(cls):
         return cls.format_name
```

### Comparing `django-flex-report-0.7.1/flex_report/fields.py` & `django-flex-report-0.7.2/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/filterset.py` & `django-flex-report-0.7.2/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/forms.py` & `django-flex-report-0.7.2/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0001_initial.py` & `django-flex-report-0.7.2/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.7.2/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.7.2/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.7.2/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.7.2/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.7.2/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.7.2/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.7.2/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.7.2/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.7.2/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.7.2/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.7.2/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/mixins.py` & `django-flex-report-0.7.2/flex_report/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,24 +126,31 @@
 
     def get_handle_kwargs(self):
         return {
             "queryset": self.get_export_qs(),
             "columns": self.get_export_columns(),
             "headers": self.get_export_headers(),
         }
+        
+    def check_auth(self):
+        try:
+            if not self.get_exporter().check_auth(self.request):
+                raise HttpResponseForbidden(content="403 Forbidden")
+        except AttributeError:
+            return
 
     def dispatch(self, *args, **kwargs):
         if not self.export_format and (
             not (format_ := self.request.GET.get("format", "").lower())
-            or format_ not in queryset_exporter.exporters.keys()
+            or format_ not in export_format.formats.keys()
         ):
             return HttpResponseBadRequest()
         
         self.export_format = self.export_format or format_
-        
+        self.check_auth()
         return super().dispatch(*args, **kwargs)
     
     def get_exporter(self) -> BaseExportFormat:
         try:
             return export_format.formats[self.export_format]
         except KeyError as e:
             raise NotImplementedError(f"The wanted format '{self.export_format}' isn't handled.") from e
```

### Comparing `django-flex-report-0.7.1/flex_report/models.py` & `django-flex-report-0.7.2/flex_report/models.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.7.2/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/urls.py` & `django-flex-report-0.7.2/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/utils.py` & `django-flex-report-0.7.2/flex_report/utils.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/flex_report/views.py` & `django-flex-report-0.7.2/flex_report/views.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.7.1/pyproject.toml` & `django-flex-report-0.7.2/pyproject.toml`

 * *Files identical despite different names*

