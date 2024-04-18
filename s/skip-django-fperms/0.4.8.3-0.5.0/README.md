# Comparing `tmp/skip-django-fperms-0.4.8.3.tar.gz` & `tmp/skip_django_fperms-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-fperms-0.4.8.3.tar", last modified: Thu Jan 19 15:46:52 2023, max compression
+gzip compressed data, was "skip_django_fperms-0.5.0.tar", last modified: Thu Apr 18 13:47:19 2024, max compression
```

## Comparing `skip-django-fperms-0.4.8.3.tar` & `skip_django_fperms-0.5.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.673506 skip-django-fperms-0.4.8.3/fperms/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.673506 skip-django-fperms-0.4.8.3/fperms/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/0002_auto_20180713_1450.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/0003_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/0004_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/0005_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.673506 skip-django-fperms-0.4.8.3/fperms/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/static/css/django_perms.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/static/js/django_perms.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.673506 skip-django-fperms-0.4.8.3/fperms/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/fperms/templates/django_perms/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/templates/django_perms/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/fperms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2269 2023-01-19 15:46:40.000000 skip-django-fperms-0.4.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 15:46:52.677506 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-19 15:46:52.000000 skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.302885 skip_django_fperms-0.5.0/fperms/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.298885 skip_django_fperms-0.5.0/fperms/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.298885 skip_django_fperms-0.5.0/fperms/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.302885 skip_django_fperms-0.5.0/fperms/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/fperms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/0002_auto_20180713_1450.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/0003_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/0004_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/0005_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.302885 skip_django_fperms-0.5.0/fperms/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/fperms/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/static/css/django_perms.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/fperms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/static/js/django_perms.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.302885 skip_django_fperms-0.5.0/fperms/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/fperms/templates/django_perms/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/templates/django_perms/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/fperms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2268 2024-04-18 13:47:14.000000 skip_django_fperms-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:19.306885 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 13:47:19.000000 skip_django_fperms-0.5.0/skip_django_fperms.egg-info/top_level.txt
```

### Comparing `skip-django-fperms-0.4.8.3/CONTRIBUTING.rst` & `skip_django_fperms-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/LICENSE` & `skip_django_fperms-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/PKG-INFO` & `skip_django_fperms-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skip-django-fperms
-Version: 0.4.8.3
+Version: 0.5.0
 Summary: Flexible Django permissions backend
 Home-page: https://github.com/skip-pay/django-fperms
-Download-URL: https://github.com/skip-pay/django-fperms/archive/0.4.8.3.tar.gz
+Download-URL: https://github.com/skip-pay/django-fperms/archive/0.5.0.tar.gz
 Author: Petr Olah
 Author-email: djangoguru@gmail.com
 License: MIT
 Keywords: django-fperms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2.0
 
 =============================
 django-fperms
 =============================
 
 .. image:: https://badge.fury.io/py/django-fperms.svg
     :target: https://badge.fury.io/py/django-fperms
```

### Comparing `skip-django-fperms-0.4.8.3/README.rst` & `skip_django_fperms-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/__init__.py` & `skip_django_fperms-0.5.0/fperms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.4.8.3'
+__version__ = '0.5.0'
 
 from django.apps import apps as django_apps
 from fperms.conf import settings
 
 from fperms.exceptions import ImproperlyConfigured
```

### Comparing `skip-django-fperms-0.4.8.3/fperms/admin.py` & `skip_django_fperms-0.5.0/fperms/admin.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/backends.py` & `skip_django_fperms-0.5.0/fperms/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/base.py` & `skip_django_fperms-0.5.0/fperms/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/conf.py` & `skip_django_fperms-0.5.0/fperms/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/enums.py` & `skip_django_fperms-0.5.0/fperms/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fperms.conf import settings
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 PERM_CODENAME_ADD = 'add'
 PERM_CODENAME_CHANGE = 'change'
 PERM_CODENAME_DELETE = 'delete'
 PERM_CODENAME_WILDCARD = '*'
```

### Comparing `skip-django-fperms-0.4.8.3/fperms/locale/cs/LC_MESSAGES/django.mo` & `skip_django_fperms-0.5.0/fperms/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/locale/cs/LC_MESSAGES/django.po` & `skip_django_fperms-0.5.0/fperms/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/managers.py` & `skip_django_fperms-0.5.0/fperms/managers.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/migrations/0001_initial.py` & `skip_django_fperms-0.5.0/fperms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/migrations/0002_auto_20180713_1450.py` & `skip_django_fperms-0.5.0/fperms/migrations/0002_auto_20180713_1450.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/migrations/0003_migration.py` & `skip_django_fperms-0.5.0/fperms/migrations/0003_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/migrations/0005_migration.py` & `skip_django_fperms-0.5.0/fperms/migrations/0005_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/templates/django_perms/base.html` & `skip_django_fperms-0.5.0/fperms/templates/django_perms/base.html`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/fperms/utils.py` & `skip_django_fperms-0.5.0/fperms/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-fperms-0.4.8.3/setup.py` & `skip_django_fperms-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     url='https://github.com/skip-pay/django-fperms',
     download_url='https://github.com/skip-pay/django-fperms/archive/{}.tar.gz'.format(version),
     packages=[
         'fperms',
     ],
     include_package_data=True,
     install_requires=[
-        "django>=2.2.15",
+        "django>=4.2.0",
     ],
     license="MIT",
     zip_safe=False,
     keywords='django-fperms',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
```

### Comparing `skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/PKG-INFO` & `skip_django_fperms-0.5.0/skip_django_fperms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: skip-django-fperms
-Version: 0.4.8.3
+Version: 0.5.0
 Summary: Flexible Django permissions backend
 Home-page: https://github.com/skip-pay/django-fperms
-Download-URL: https://github.com/skip-pay/django-fperms/archive/0.4.8.3.tar.gz
+Download-URL: https://github.com/skip-pay/django-fperms/archive/0.5.0.tar.gz
 Author: Petr Olah
 Author-email: djangoguru@gmail.com
 License: MIT
 Keywords: django-fperms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django>=4.2.0
 
 =============================
 django-fperms
 =============================
 
 .. image:: https://badge.fury.io/py/django-fperms.svg
     :target: https://badge.fury.io/py/django-fperms
```

### Comparing `skip-django-fperms-0.4.8.3/skip_django_fperms.egg-info/SOURCES.txt` & `skip_django_fperms-0.5.0/skip_django_fperms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

