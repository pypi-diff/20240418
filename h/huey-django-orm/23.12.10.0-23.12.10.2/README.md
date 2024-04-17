# Comparing `tmp/huey_django_orm-23.12.10.0.tar.gz` & `tmp/huey_django_orm-23.12.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huey_django_orm-23.12.10.0.tar", last modified: Sun Dec 10 19:17:19 2023, max compression
+gzip compressed data, was "huey_django_orm-23.12.10.2.tar", last modified: Wed Apr 17 22:00:14 2024, max compression
```

## Comparing `huey_django_orm-23.12.10.0.tar` & `huey_django_orm-23.12.10.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-12-10 19:17:19.355282 huey_django_orm-23.12.10.0/
--rw-rw-rw-   0        0        0     1068 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/LICENSE
--rw-rw-rw-   0        0        0       97 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3161 2023-12-10 19:17:19.354282 huey_django_orm-23.12.10.0/PKG-INFO
--rw-rw-rw-   0        0        0     2105 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-10 19:17:19.328735 huey_django_orm-23.12.10.0/huey_django_orm/
--rw-rw-rw-   0        0        0       52 2023-12-10 19:12:02.000000 huey_django_orm-23.12.10.0/huey_django_orm/__init__.py
--rw-rw-rw-   0        0        0      647 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/admin.py
--rw-rw-rw-   0        0        0      160 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/apps.py
-drwxrwxrwx   0        0        0        0 2023-12-10 19:17:19.353282 huey_django_orm-23.12.10.0/huey_django_orm/migrations/
--rw-rw-rw-   0        0        0     1776 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/migrations/__init__.py
--rw-rw-rw-   0        0        0     1044 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/models.py
--rw-rw-rw-   0        0        0     4679 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/storage.py
--rw-rw-rw-   0        0        0       60 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/tests.py
--rw-rw-rw-   0        0        0       63 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/huey_django_orm/views.py
-drwxrwxrwx   0        0        0        0 2023-12-10 19:17:19.354282 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/
--rw-rw-rw-   0        0        0     3161 2023-12-10 19:17:19.000000 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-12-10 19:17:19.000000 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-10 19:17:19.000000 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-12-10 19:17:19.000000 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-12-10 19:17:19.000000 huey_django_orm-23.12.10.0/huey_django_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       11 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/requirements.txt
--rw-rw-rw-   0        0        0       68 2023-12-10 19:17:19.359281 huey_django_orm-23.12.10.0/setup.cfg
--rw-rw-rw-   0        0        0     1267 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.0/setup.py
+drwxr-xr-x   0 avryhof   (1000) avryhof   (1000)        0 2024-04-17 22:00:14.784192 huey_django_orm-23.12.10.2/
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     1068 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/LICENSE
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       97 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/MANIFEST.in
+-rw-r--r--   0 avryhof   (1000) avryhof   (1000)     3063 2024-04-17 22:00:14.781186 huey_django_orm-23.12.10.2/PKG-INFO
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     2105 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/README.md
+drwxr-xr-x   0 avryhof   (1000) avryhof   (1000)        0 2024-04-17 22:00:14.687133 huey_django_orm-23.12.10.2/huey_django_orm/
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       52 2024-04-17 21:55:45.000000 huey_django_orm-23.12.10.2/huey_django_orm/__init__.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)      647 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/admin.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)      160 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/apps.py
+drwxr-xr-x   0 avryhof   (1000) avryhof   (1000)        0 2024-04-17 22:00:14.762185 huey_django_orm-23.12.10.2/huey_django_orm/migrations/
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     1881 2024-04-17 21:46:23.000000 huey_django_orm-23.12.10.2/huey_django_orm/migrations/0001_initial.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)        0 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/migrations/__init__.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     1044 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/models.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     4679 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/storage.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       60 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/tests.py
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       63 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/huey_django_orm/views.py
+drwxr-xr-x   0 avryhof   (1000) avryhof   (1000)        0 2024-04-17 22:00:14.776186 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/
+-rw-r--r--   0 avryhof   (1000) avryhof   (1000)     3063 2024-04-17 22:00:13.000000 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/PKG-INFO
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)      521 2024-04-17 22:00:14.000000 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/SOURCES.txt
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)        1 2024-04-17 22:00:13.000000 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/dependency_links.txt
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       12 2024-04-17 22:00:13.000000 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/requires.txt
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       16 2024-04-17 22:00:13.000000 huey_django_orm-23.12.10.2/huey_django_orm.egg-info/top_level.txt
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       11 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/requirements.txt
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)       61 2024-04-17 22:00:14.788192 huey_django_orm-23.12.10.2/setup.cfg
+-rwxr--r--   0 avryhof   (1000) avryhof   (1000)     1267 2023-12-10 13:46:24.000000 huey_django_orm-23.12.10.2/setup.py
```

### Comparing `huey_django_orm-23.12.10.0/LICENSE` & `huey_django_orm-23.12.10.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/PKG-INFO` & `huey_django_orm-23.12.10.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: huey_django_orm
-Version: 23.12.10.0
-Summary: A module to use Django ORM for storage with huey.
-Home-page: https://github.com/avryhof/huey_django_orm
-Author: Amos Vryhof
-Author-email: avryhof@gmail.com
-License: MIT
-Project-URL: GitHub Repo, https://github.com/avryhof/huey_django_orm
-Project-URL: Bug Tracker, https://github.com/avryhof/huey_django_orm/issues
-Keywords: huey,django,huey.contrib.djhuey
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Django
-Requires-Dist: huey
-
-[![PyPI version](http://img.shields.io/pypi/v/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
-[![license](http://img.shields.io/pypi/l/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?style=flat-square)](https://paypal.me/avryhof?country.x=US&locale.x=en_US)
-
-huey_django_orm
-=
-A module to use Django ORM for storage with [huey](https://pypi.org/project/huey/)
-
-This project originally started because I wanted to just update [huey-pg](https://pypi.org/project/huey-pg/). That
-proved to be more of a full rewrite than just an update.
-
-Anyway, I didn't want to use SqliteHuey, or FileHuey, since I already have a perfectly good data store in my Django
-project.
-
-So, I took a copy of SqliteHuey, and re-implemented the class functionality using Django ORM.
-
-Huey doesn't do anything too crazy, so it should work with any database backend supported by Django. We also don't use
-any non-standard Django stuff, so it should work with any modern Django version.
-
-## Installation
-
-Install with pip
-
-```bash
-pip install huey-django-orm
-```
-
-### settings.py
-
-Add to INSTALLED_APPS
-
-```python
-INSTALLED_APPS = [
-    "...",
-    "huey_django_orm",
-    "...",
-]
-```
-
-Configure Huey to use DjangoORMHuey
-
-```python
-from huey_django_orm.storage import DjangoORMHuey
-
-HUEY = DjangoORMHuey()
-```
-
-or if you need other options
-
-```python
-HUEY = {
-    "...": "...",
-    'huey_class': 'huey_django_orm.storage.DjangoORMHuey',
-    "......": "...",
-}
-```
-
-### Run Migrations
-
-```bash
-python manage.py migrate huey_django_orm
-```
-
-That's it!  Now you can use Huey just like you normally would.
-
-## Admin
-
-Since this project is specific to Django, and will likely never be used without it, you get a few Django goodies rolled
-right in.
-
-* Each Model has a ModelAdmin
-* There is an auto_now_add field in each model so we can see when an object was created within the admin
-* Ordering is defined at the model level, so objects will appear in the admin in the same way they will be processed.
+Metadata-Version: 2.1
+Name: huey_django_orm
+Version: 23.12.10.2
+Summary: A module to use Django ORM for storage with huey.
+Home-page: https://github.com/avryhof/huey_django_orm
+Author: Amos Vryhof
+Author-email: avryhof@gmail.com
+License: MIT
+Project-URL: GitHub Repo, https://github.com/avryhof/huey_django_orm
+Project-URL: Bug Tracker, https://github.com/avryhof/huey_django_orm/issues
+Keywords: huey,django,huey.contrib.djhuey
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: huey
+
+[![PyPI version](http://img.shields.io/pypi/v/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
+[![license](http://img.shields.io/pypi/l/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?style=flat-square)](https://paypal.me/avryhof?country.x=US&locale.x=en_US)
+
+huey_django_orm
+=
+A module to use Django ORM for storage with [huey](https://pypi.org/project/huey/)
+
+This project originally started because I wanted to just update [huey-pg](https://pypi.org/project/huey-pg/). That
+proved to be more of a full rewrite than just an update.
+
+Anyway, I didn't want to use SqliteHuey, or FileHuey, since I already have a perfectly good data store in my Django
+project.
+
+So, I took a copy of SqliteHuey, and re-implemented the class functionality using Django ORM.
+
+Huey doesn't do anything too crazy, so it should work with any database backend supported by Django. We also don't use
+any non-standard Django stuff, so it should work with any modern Django version.
+
+## Installation
+
+Install with pip
+
+```bash
+pip install huey-django-orm
+```
+
+### settings.py
+
+Add to INSTALLED_APPS
+
+```python
+INSTALLED_APPS = [
+    "...",
+    "huey_django_orm",
+    "...",
+]
+```
+
+Configure Huey to use DjangoORMHuey
+
+```python
+from huey_django_orm.storage import DjangoORMHuey
+
+HUEY = DjangoORMHuey()
+```
+
+or if you need other options
+
+```python
+HUEY = {
+    "...": "...",
+    'huey_class': 'huey_django_orm.storage.DjangoORMHuey',
+    "......": "...",
+}
+```
+
+### Run Migrations
+
+```bash
+python manage.py migrate huey_django_orm
+```
+
+That's it!  Now you can use Huey just like you normally would.
+
+## Admin
+
+Since this project is specific to Django, and will likely never be used without it, you get a few Django goodies rolled
+right in.
+
+* Each Model has a ModelAdmin
+* There is an auto_now_add field in each model so we can see when an object was created within the admin
+* Ordering is defined at the model level, so objects will appear in the admin in the same way they will be processed.
```

### Comparing `huey_django_orm-23.12.10.0/README.md` & `huey_django_orm-23.12.10.2/README.md`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm/admin.py` & `huey_django_orm-23.12.10.2/huey_django_orm/admin.py`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm/migrations/0001_initial.py` & `huey_django_orm-23.12.10.2/huey_django_orm/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,19 +26,21 @@
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('queue', models.TextField(default='default')),
                 ('data', models.BinaryField(blank=True, null=True)),
                 ('timestamp', models.DateTimeField(blank=True, null=True)),
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
             ],
+            options={'ordering': ('timestamp',)},
         ),
         migrations.CreateModel(
             name='HueyTask',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('queue', models.TextField(default='default')),
                 ('data', models.BinaryField(blank=True, null=True)),
                 ('priority', models.DecimalField(blank=True, decimal_places=4, max_digits=5, null=True)),
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
             ],
+            options={'ordering': ('-priority', 'id')},
         ),
     ]
```

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm/models.py` & `huey_django_orm-23.12.10.2/huey_django_orm/models.py`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm/storage.py` & `huey_django_orm-23.12.10.2/huey_django_orm/storage.py`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm.egg-info/PKG-INFO` & `huey_django_orm-23.12.10.2/huey_django_orm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: huey-django-orm
-Version: 23.12.10.0
-Summary: A module to use Django ORM for storage with huey.
-Home-page: https://github.com/avryhof/huey_django_orm
-Author: Amos Vryhof
-Author-email: avryhof@gmail.com
-License: MIT
-Project-URL: GitHub Repo, https://github.com/avryhof/huey_django_orm
-Project-URL: Bug Tracker, https://github.com/avryhof/huey_django_orm/issues
-Keywords: huey,django,huey.contrib.djhuey
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Django
-Requires-Dist: huey
-
-[![PyPI version](http://img.shields.io/pypi/v/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
-[![license](http://img.shields.io/pypi/l/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?style=flat-square)](https://paypal.me/avryhof?country.x=US&locale.x=en_US)
-
-huey_django_orm
-=
-A module to use Django ORM for storage with [huey](https://pypi.org/project/huey/)
-
-This project originally started because I wanted to just update [huey-pg](https://pypi.org/project/huey-pg/). That
-proved to be more of a full rewrite than just an update.
-
-Anyway, I didn't want to use SqliteHuey, or FileHuey, since I already have a perfectly good data store in my Django
-project.
-
-So, I took a copy of SqliteHuey, and re-implemented the class functionality using Django ORM.
-
-Huey doesn't do anything too crazy, so it should work with any database backend supported by Django. We also don't use
-any non-standard Django stuff, so it should work with any modern Django version.
-
-## Installation
-
-Install with pip
-
-```bash
-pip install huey-django-orm
-```
-
-### settings.py
-
-Add to INSTALLED_APPS
-
-```python
-INSTALLED_APPS = [
-    "...",
-    "huey_django_orm",
-    "...",
-]
-```
-
-Configure Huey to use DjangoORMHuey
-
-```python
-from huey_django_orm.storage import DjangoORMHuey
-
-HUEY = DjangoORMHuey()
-```
-
-or if you need other options
-
-```python
-HUEY = {
-    "...": "...",
-    'huey_class': 'huey_django_orm.storage.DjangoORMHuey',
-    "......": "...",
-}
-```
-
-### Run Migrations
-
-```bash
-python manage.py migrate huey_django_orm
-```
-
-That's it!  Now you can use Huey just like you normally would.
-
-## Admin
-
-Since this project is specific to Django, and will likely never be used without it, you get a few Django goodies rolled
-right in.
-
-* Each Model has a ModelAdmin
-* There is an auto_now_add field in each model so we can see when an object was created within the admin
-* Ordering is defined at the model level, so objects will appear in the admin in the same way they will be processed.
+Metadata-Version: 2.1
+Name: huey_django_orm
+Version: 23.12.10.2
+Summary: A module to use Django ORM for storage with huey.
+Home-page: https://github.com/avryhof/huey_django_orm
+Author: Amos Vryhof
+Author-email: avryhof@gmail.com
+License: MIT
+Project-URL: GitHub Repo, https://github.com/avryhof/huey_django_orm
+Project-URL: Bug Tracker, https://github.com/avryhof/huey_django_orm/issues
+Keywords: huey,django,huey.contrib.djhuey
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Django
+Requires-Dist: huey
+
+[![PyPI version](http://img.shields.io/pypi/v/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
+[![license](http://img.shields.io/pypi/l/huey-django-orm.svg?style=flat-square)](https://pypi.python.org/pypi/huey-django-orm)
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?style=flat-square)](https://paypal.me/avryhof?country.x=US&locale.x=en_US)
+
+huey_django_orm
+=
+A module to use Django ORM for storage with [huey](https://pypi.org/project/huey/)
+
+This project originally started because I wanted to just update [huey-pg](https://pypi.org/project/huey-pg/). That
+proved to be more of a full rewrite than just an update.
+
+Anyway, I didn't want to use SqliteHuey, or FileHuey, since I already have a perfectly good data store in my Django
+project.
+
+So, I took a copy of SqliteHuey, and re-implemented the class functionality using Django ORM.
+
+Huey doesn't do anything too crazy, so it should work with any database backend supported by Django. We also don't use
+any non-standard Django stuff, so it should work with any modern Django version.
+
+## Installation
+
+Install with pip
+
+```bash
+pip install huey-django-orm
+```
+
+### settings.py
+
+Add to INSTALLED_APPS
+
+```python
+INSTALLED_APPS = [
+    "...",
+    "huey_django_orm",
+    "...",
+]
+```
+
+Configure Huey to use DjangoORMHuey
+
+```python
+from huey_django_orm.storage import DjangoORMHuey
+
+HUEY = DjangoORMHuey()
+```
+
+or if you need other options
+
+```python
+HUEY = {
+    "...": "...",
+    'huey_class': 'huey_django_orm.storage.DjangoORMHuey',
+    "......": "...",
+}
+```
+
+### Run Migrations
+
+```bash
+python manage.py migrate huey_django_orm
+```
+
+That's it!  Now you can use Huey just like you normally would.
+
+## Admin
+
+Since this project is specific to Django, and will likely never be used without it, you get a few Django goodies rolled
+right in.
+
+* Each Model has a ModelAdmin
+* There is an auto_now_add field in each model so we can see when an object was created within the admin
+* Ordering is defined at the model level, so objects will appear in the admin in the same way they will be processed.
```

### Comparing `huey_django_orm-23.12.10.0/huey_django_orm.egg-info/SOURCES.txt` & `huey_django_orm-23.12.10.2/huey_django_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huey_django_orm-23.12.10.0/setup.py` & `huey_django_orm-23.12.10.2/setup.py`

 * *Files identical despite different names*

