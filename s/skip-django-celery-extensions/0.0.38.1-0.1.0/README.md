# Comparing `tmp/skip-django-celery-extensions-0.0.38.1.tar.gz` & `tmp/skip_django_celery_extensions-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-celery-extensions-0.0.38.1.tar", last modified: Mon Jan 30 01:10:43 2023, max compression
+gzip compressed data, was "skip_django_celery_extensions-0.1.0.tar", last modified: Thu Apr 18 13:48:33 2024, max compression
```

## Comparing `skip-django-celery-extensions-0.0.38.1.tar` & `skip_django_celery_extensions-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/bin/celeryautoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    26724 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/django_celery_extensions/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/example/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/example/app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/example/app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/management/commands/create_user.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/app/tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/example/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/settings/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/example/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-01-30 01:10:34.000000 skip-django-celery-extensions-0.0.38.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:10:43.481888 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-30 01:10:43.000000 skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.776831 skip_django_celery_extensions-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 13:48:33.776831 skip_django_celery_extensions-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/django_celery_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/django_celery_extensions/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/bin/celeryautoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26724 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/django_celery_extensions/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/example/app/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.772831 skip_django_celery_extensions-0.1.0/example/app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/management/commands/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/app/tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.776831 skip_django_celery_extensions-0.1.0/example/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/settings/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/example/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 13:48:33.776831 skip_django_celery_extensions-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 13:48:30.000000 skip_django_celery_extensions-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:48:33.776831 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 13:48:33.000000 skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/top_level.txt
```

### Comparing `skip-django-celery-extensions-0.0.38.1/LICENSE` & `skip_django_celery_extensions-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/PKG-INFO` & `skip_django_celery_extensions-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-celery-extensions
-Version: 0.0.38.1
+Version: 0.1.0
 Summary: Django celery extensions library.
 Home-page: https://github.com/skip-pay/django-celery-extensions
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,celery
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2.0
+Requires-Dist: import_string>=0.1.0
+Requires-Dist: celery<5.3,>=5.2
 
 ========================
 Django Celery Extensions
 ========================
 
 
 .. image:: https://img.shields.io/pypi/v/django-celery-extensions.svg
```

### Comparing `skip-django-celery-extensions-0.0.38.1/README.rst` & `skip_django_celery_extensions-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/django_celery_extensions/beat.py` & `skip_django_celery_extensions-0.1.0/django_celery_extensions/beat.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/django_celery_extensions/checks.py` & `skip_django_celery_extensions-0.1.0/django_celery_extensions/checks.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/django_celery_extensions/config.py` & `skip_django_celery_extensions-0.1.0/django_celery_extensions/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/django_celery_extensions/task.py` & `skip_django_celery_extensions-0.1.0/django_celery_extensions/task.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/example/app/tasks.py` & `skip_django_celery_extensions-0.1.0/example/app/tasks.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/example/app/tests.py` & `skip_django_celery_extensions-0.1.0/example/app/tests.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/example/settings/settings.py` & `skip_django_celery_extensions-0.1.0/example/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/example/wsgi.py` & `skip_django_celery_extensions-0.1.0/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-celery-extensions-0.0.38.1/setup.py` & `skip_django_celery_extensions-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = readme_file.read()
 
 
 setup(
     name='skip-django-celery-extensions',
     long_description=readme,
     long_description_content_type='text/markdown',
-    version='0.0.38.1',
+    version='0.1.0',
     description="Django celery extensions library.",
     keywords='django, celery',
     author='Lubos Matl',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/django-celery-extensions',
     license='MIT',
     package_dir={'django_celery_extensions': 'django_celery_extensions'},
@@ -34,15 +34,15 @@
         'Natural Language :: Czech',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
     ],
     install_requires=[
-        'django>=2.2.14, <4.0',
+        'django>=4.2.0',
         'import_string>=0.1.0',
         'celery>=5.2, <5.3'
     ],
     entry_points={'console_scripts': [
         'celeryautoreload=django_celery_extensions.bin.celeryautoreload:celery_autoreload',
     ]},
     zip_safe=False
```

### Comparing `skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/PKG-INFO` & `skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-celery-extensions
-Version: 0.0.38.1
+Version: 0.1.0
 Summary: Django celery extensions library.
 Home-page: https://github.com/skip-pay/django-celery-extensions
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,celery
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2.0
+Requires-Dist: import_string>=0.1.0
+Requires-Dist: celery<5.3,>=5.2
 
 ========================
 Django Celery Extensions
 ========================
 
 
 .. image:: https://img.shields.io/pypi/v/django-celery-extensions.svg
```

### Comparing `skip-django-celery-extensions-0.0.38.1/skip_django_celery_extensions.egg-info/SOURCES.txt` & `skip_django_celery_extensions-0.1.0/skip_django_celery_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

