# Comparing `tmp/dj_anonymizer-0.6.0.tar.gz` & `tmp/dj_anonymizer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_anonymizer-0.6.0.tar", last modified: Tue Jan  9 12:32:56 2024, max compression
+gzip compressed data, was "dj_anonymizer-0.6.1.tar", last modified: Thu Apr 18 20:06:19 2024, max compression
```

## Comparing `dj_anonymizer-0.6.0.tar` & `dj_anonymizer-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1055 2024-01-09 12:08:04.000000 dj_anonymizer-0.6.0/LICENSE.txt
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       50 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.0/MANIFEST.in
--rw-r--r--   0 chinskiy  (1000) chinskiy  (1000)     1906 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/PKG-INFO
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      739 2024-01-09 12:28:11.000000 dj_anonymizer-0.6.0/README.md
-drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/dj_anonymizer/
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       52 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.0/dj_anonymizer/__init__.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     3132 2024-01-09 12:08:04.000000 dj_anonymizer-0.6.0/dj_anonymizer/anonymizer.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       86 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.0/dj_anonymizer/apps.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      418 2022-01-11 20:07:58.000000 dj_anonymizer-0.6.0/dj_anonymizer/conf.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      822 2022-02-07 12:28:12.000000 dj_anonymizer-0.6.0/dj_anonymizer/fields.py
-drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/dj_anonymizer/management/
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        0 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.0/dj_anonymizer/management/__init__.py
-drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/dj_anonymizer/management/commands/
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        0 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.0/dj_anonymizer/management/commands/__init__.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     2526 2022-02-07 09:06:34.000000 dj_anonymizer-0.6.0/dj_anonymizer/management/commands/anonymize_db.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     5075 2024-01-09 10:12:24.000000 dj_anonymizer-0.6.0/dj_anonymizer/register_models.py
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1704 2024-01-09 10:12:24.000000 dj_anonymizer-0.6.0/dj_anonymizer/utils.py
-drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/
--rw-r--r--   0 chinskiy  (1000) chinskiy  (1000)     1906 2024-01-09 12:32:56.000000 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/PKG-INFO
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      547 2024-01-09 12:32:56.000000 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/SOURCES.txt
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        1 2024-01-09 12:32:56.000000 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/dependency_links.txt
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       12 2024-01-09 12:32:56.000000 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/requires.txt
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       14 2024-01-09 12:32:56.000000 dj_anonymizer-0.6.0/dj_anonymizer.egg-info/top_level.txt
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      294 2024-01-09 12:32:56.094681 dj_anonymizer-0.6.0/setup.cfg
--rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1550 2024-01-09 12:22:42.000000 dj_anonymizer-0.6.0/setup.py
+drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-04-18 20:06:19.058105 dj_anonymizer-0.6.1/
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1055 2024-01-09 12:08:04.000000 dj_anonymizer-0.6.1/LICENSE.txt
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       50 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.1/MANIFEST.in
+-rw-r--r--   0 chinskiy  (1000) chinskiy  (1000)     2026 2024-04-18 20:06:19.058105 dj_anonymizer-0.6.1/PKG-INFO
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      818 2024-04-18 19:50:00.000000 dj_anonymizer-0.6.1/README.md
+drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-04-18 20:06:19.054105 dj_anonymizer-0.6.1/dj_anonymizer/
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       52 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.1/dj_anonymizer/__init__.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     3441 2024-04-18 19:50:00.000000 dj_anonymizer-0.6.1/dj_anonymizer/anonymizer.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       86 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.1/dj_anonymizer/apps.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      822 2022-02-07 12:28:12.000000 dj_anonymizer-0.6.1/dj_anonymizer/fields.py
+drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-04-18 20:06:19.054105 dj_anonymizer-0.6.1/dj_anonymizer/management/
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        0 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.1/dj_anonymizer/management/__init__.py
+drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-04-18 20:06:19.058105 dj_anonymizer-0.6.1/dj_anonymizer/management/commands/
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        0 2019-09-16 08:55:35.000000 dj_anonymizer-0.6.1/dj_anonymizer/management/commands/__init__.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     2526 2022-02-07 09:06:34.000000 dj_anonymizer-0.6.1/dj_anonymizer/management/commands/anonymize_db.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     5075 2024-01-09 10:12:24.000000 dj_anonymizer-0.6.1/dj_anonymizer/register_models.py
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1800 2024-04-18 19:50:00.000000 dj_anonymizer-0.6.1/dj_anonymizer/utils.py
+drwxrwxr-x   0 chinskiy  (1000) chinskiy  (1000)        0 2024-04-18 20:06:19.058105 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/
+-rw-r--r--   0 chinskiy  (1000) chinskiy  (1000)     2026 2024-04-18 20:06:19.000000 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/PKG-INFO
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      525 2024-04-18 20:06:19.000000 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)        1 2024-04-18 20:06:19.000000 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       12 2024-04-18 20:06:19.000000 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/requires.txt
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)       14 2024-04-18 20:06:19.000000 dj_anonymizer-0.6.1/dj_anonymizer.egg-info/top_level.txt
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)      286 2024-04-18 20:06:19.058105 dj_anonymizer-0.6.1/setup.cfg
+-rw-rw-r--   0 chinskiy  (1000) chinskiy  (1000)     1613 2024-04-18 19:50:28.000000 dj_anonymizer-0.6.1/setup.py
```

### Comparing `dj_anonymizer-0.6.0/LICENSE.txt` & `dj_anonymizer-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj_anonymizer-0.6.0/PKG-INFO` & `dj_anonymizer-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dj_anonymizer
-Version: 0.6.0
-Summary: This project helps anonymize production database with fake data of any kind.
+Version: 0.6.1
+Summary: dj_anonymizer is a utility designed to anonymize production databases with various types of mock data, specifically designed for use within Django projects.
 Home-page: https://github.com/preply/dj_anonymizer
 Author: Tim Pagurets
 License: MIT
 Keywords: django,data,database,anonymization,dj-anonymizer
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -16,25 +16,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.2
 
 dj_anonymizer [![Build Status](https://github.com/preply/dj_anonymizer/actions/workflows/test.yml/badge.svg)](https://travis-ci.com/preply/dj_anonymizer) [![codecov.io](https://codecov.io/github/preply/dj_anonymizer/coverage.svg?branch=master)](https://codecov.io/github/preply/dj_anonymizer?branch=master) [![PyPI version](https://badge.fury.io/py/dj-anonymizer.svg)](https://badge.fury.io/py/dj_anonymizer)
 ==================================
 
-dj_anonymizer helps anonymize production database with any kind of fake data.
+dj_anonymizer is a utility designed to anonymize production databases with various types of mock data, specifically designed for use within Django projects.
 
-Project works with Django 2.2 or higher and Python 3.5 or higher.
+Project works with Django 4.2 or higher and Python 3.8 or higher.
 
 Documentation
 ==================================
 [https://dj-anonymizer.readthedocs.io/en/latest/](https://dj-anonymizer.readthedocs.io/en/latest/)
```

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer/anonymizer.py` & `dj_anonymizer-0.6.1/dj_anonymizer/anonymizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import django
+from django.conf import settings
 
-from dj_anonymizer.conf import settings
 from dj_anonymizer.utils import import_if_exist, truncate_table
 
 
 class Anonymizer:
     anonym_models = {}
     clean_models = {}
     skip_models = []
@@ -47,40 +47,48 @@
         Keys that used for referencing Django models in Anonymizer
         """
         return f'{model.__module__}.{model.__name__}'
 
     def anonymize(self, only=None):
         anon_list = self.anonym_models.values() if only is None \
             else [self.anonym_models[only]]
+        # Size of chunks what will be used to select data from table.
+        select_batch_size = getattr(
+            settings, "ANONYMIZER_SELECT_BATCH_SIZE", 20000
+        )
+        # Size of chunks what will be used to update data in table.
+        update_batch_size = getattr(
+            settings, "ANONYMIZER_UPDATE_BATCH_SIZE", 500
+        )
         for anonym_cls in anon_list:
 
             if not anonym_cls.get_fields_names():
                 continue
 
             queryset = anonym_cls.Meta.queryset.only(
                 *anonym_cls.get_fields_names()
             )
             print(f'Anonymizing model {self.key(queryset.model)}')
 
             i = 0
             total = queryset.count()
             for j in list(range(0, total,
-                          settings.ANONYMIZER_SELECT_BATCH_SIZE)) + [None]:
+                                select_batch_size)) + [None]:
                 subset = queryset.order_by('pk')[i:j]
                 for obj in subset:
                     i += 1
 
                     for name in anonym_cls.get_fields_names():
                         setattr(obj, name, next(
                             getattr(anonym_cls, name))
                         )
                 queryset.bulk_update(
                     subset,
                     anonym_cls.get_fields_names(),
-                    batch_size=settings.ANONYMIZER_UPDATE_BATCH_SIZE,
+                    batch_size=update_batch_size,
                 )
 
     def clean(self, only=None):
         clean_list = self.clean_models.values() if only is None \
             else [self.clean_models[only]]
         for queryset in clean_list:
             print(f'Cleaning {self.key(queryset.model)}')
```

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer/fields.py` & `dj_anonymizer-0.6.1/dj_anonymizer/fields.py`

 * *Files identical despite different names*

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer/management/commands/anonymize_db.py` & `dj_anonymizer-0.6.1/dj_anonymizer/management/commands/anonymize_db.py`

 * *Files identical despite different names*

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer/register_models.py` & `dj_anonymizer-0.6.1/dj_anonymizer/register_models.py`

 * *Files identical despite different names*

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer/utils.py` & `dj_anonymizer-0.6.1/dj_anonymizer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import importlib
 import os
 
+from django.conf import settings
 from django.db import connections, router
 
-from dj_anonymizer.conf import settings
-
 
 VENDOR_TO_TRUNCATE = {
     'postgresql': 'TRUNCATE TABLE',
     'mysql': 'TRUNCATE TABLE',
     'sqlite': 'DELETE FROM',
     'oracle': 'TRUNCATE TABLE',
 }
@@ -19,15 +18,20 @@
 }
 
 
 def import_if_exist(filename):
     """
     Check if file exist in appropriate path and import it
     """
-    filepath = os.path.join(settings.ANONYMIZER_MODEL_DEFINITION_DIR, filename)
+    model_devinition_dir = getattr(
+        settings,
+        'ANONYMIZER_MODEL_DEFINITION_DIR',
+        'anonymizer'
+    )
+    filepath = os.path.join(model_devinition_dir, filename)
     full_filepath = os.path.abspath(filepath + '.py')
 
     if os.path.isfile(full_filepath):
         spec = importlib.util.spec_from_file_location(filename, full_filepath)
         mod = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(mod)
```

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer.egg-info/PKG-INFO` & `dj_anonymizer-0.6.1/dj_anonymizer.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dj_anonymizer
-Version: 0.6.0
-Summary: This project helps anonymize production database with fake data of any kind.
+Version: 0.6.1
+Summary: dj_anonymizer is a utility designed to anonymize production databases with various types of mock data, specifically designed for use within Django projects.
 Home-page: https://github.com/preply/dj_anonymizer
 Author: Tim Pagurets
 License: MIT
 Keywords: django,data,database,anonymization,dj-anonymizer
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -16,25 +16,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: Django>=3.2
+Requires-Dist: Django>=4.2
 
 dj_anonymizer [![Build Status](https://github.com/preply/dj_anonymizer/actions/workflows/test.yml/badge.svg)](https://travis-ci.com/preply/dj_anonymizer) [![codecov.io](https://codecov.io/github/preply/dj_anonymizer/coverage.svg?branch=master)](https://codecov.io/github/preply/dj_anonymizer?branch=master) [![PyPI version](https://badge.fury.io/py/dj-anonymizer.svg)](https://badge.fury.io/py/dj_anonymizer)
 ==================================
 
-dj_anonymizer helps anonymize production database with any kind of fake data.
+dj_anonymizer is a utility designed to anonymize production databases with various types of mock data, specifically designed for use within Django projects.
 
-Project works with Django 2.2 or higher and Python 3.5 or higher.
+Project works with Django 4.2 or higher and Python 3.8 or higher.
 
 Documentation
 ==================================
 [https://dj-anonymizer.readthedocs.io/en/latest/](https://dj-anonymizer.readthedocs.io/en/latest/)
```

### Comparing `dj_anonymizer-0.6.0/dj_anonymizer.egg-info/SOURCES.txt` & `dj_anonymizer-0.6.1/dj_anonymizer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 dj_anonymizer/__init__.py
 dj_anonymizer/anonymizer.py
 dj_anonymizer/apps.py
-dj_anonymizer/conf.py
 dj_anonymizer/fields.py
 dj_anonymizer/register_models.py
 dj_anonymizer/utils.py
 dj_anonymizer.egg-info/PKG-INFO
 dj_anonymizer.egg-info/SOURCES.txt
 dj_anonymizer.egg-info/dependency_links.txt
 dj_anonymizer.egg-info/requires.txt
```

### Comparing `dj_anonymizer-0.6.0/setup.py` & `dj_anonymizer-0.6.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 setup(
     name='dj_anonymizer',
     packages=['dj_anonymizer'],
     include_package_data=True,
-    version='0.6.0',
-    description='This project helps anonymize production database '
-                + 'with fake data of any kind.',
+    version='0.6.1',
+    description='dj_anonymizer is a utility designed to anonymize '
+                + 'production databases with various types of mock data, '
+                + 'specifically designed for use within Django projects.',
     long_description=(read('README.md')),
     long_description_content_type='text/markdown',
     license='MIT',
     author='Tim Pagurets',
     url='https://github.com/preply/dj_anonymizer',
     keywords=['django', 'data', 'database', 'anonymization', 'dj-anonymizer'],
     classifiers=[
@@ -33,16 +34,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
         'Framework :: Django :: 5.0',
         'Topic :: Database'
     ],
     install_requires=[
-        'Django>=3.2',
+        'Django>=4.2',
     ]
 )
```

