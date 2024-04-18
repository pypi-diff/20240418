# Comparing `tmp/skip-django-psycopg2-extension-0.1.1.3.tar.gz` & `tmp/skip_django_psycopg2_extension-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-psycopg2-extension-0.1.1.3.tar", last modified: Wed Jan 17 15:19:51 2024, max compression
+gzip compressed data, was "skip_django_psycopg2_extension-0.2.0.tar", last modified: Thu Apr 18 13:53:16 2024, max compression
```

## Comparing `skip-django-psycopg2-extension-0.1.1.3.tar` & `skip_django_psycopg2_extension-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:51.790190 skip-django-psycopg2-extension-0.1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-17 15:19:51.790190 skip-django-psycopg2-extension-0.1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:51.786189 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/base_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:51.786189 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:51.790190 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlclean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlsnapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/patch_database_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 15:19:51.790190 skip-django-psycopg2-extension-0.1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-17 15:19:44.000000 skip-django-psycopg2-extension-0.1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 15:19:51.790190 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-17 15:19:51.000000 skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:16.788723 skip_django_psycopg2_extension-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-18 13:53:16.784723 skip_django_psycopg2_extension-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:16.784723 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/base_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:16.784723 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:16.784723 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlclean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlsnapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/patch_database_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/psycopg2_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:53:16.788723 skip_django_psycopg2_extension-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 13:53:12.000000 skip_django_psycopg2_extension-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:53:16.784723 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 13:53:16.000000 skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/top_level.txt
```

### Comparing `skip-django-psycopg2-extension-0.1.1.3/LICENSE` & `skip_django_psycopg2_extension-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/PKG-INFO` & `skip_django_psycopg2_extension-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: skip-django-psycopg2-extension
-Version: 0.1.1.3
+Version: 0.2.0
 Summary: Library contains django commands which helps to prepare and manage PostgreSQL database.
 Home-page: https://github.com/skip-pay/django-psycopg2-extension
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<4.0,>=3.1
+Requires-Dist: django>=4.2
 
 # Django-psycopg2-extension
 
 Library contains django commands which helps to prepare and manage PostgreSQL database.
 
 ## Quickstart
```

### Comparing `skip-django-psycopg2-extension-0.1.1.3/README.md` & `skip_django_psycopg2_extension-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/base_command.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/base_command.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlclean.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlclean.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlinit.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlinit.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/management/commands/psqlsnapshot.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/management/commands/psqlsnapshot.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/patch_database_creation.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/patch_database_creation.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/psycopg2_extension/utils.py` & `skip_django_psycopg2_extension-0.2.0/psycopg2_extension/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-psycopg2-extension-0.1.1.3/setup.py` & `skip_django_psycopg2_extension-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="skip-django-psycopg2-extension",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    version="0.1.1.3",
+    version="0.2.0",
     description="Library contains django commands which helps to prepare and manage PostgreSQL database.",
     url="https://github.com/skip-pay/django-psycopg2-extension",
     license="MIT",
     package_dir={"psycopg2_extension": "psycopg2_extension"},
     include_package_data=True,
     packages=find_packages(),
     classifiers=[
@@ -24,11 +24,11 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
     ],
     install_requires=[
-        "django>=3.1,<4.0",
+        "django>=4.2",
     ],
     zip_safe=False,
 )
```

### Comparing `skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/PKG-INFO` & `skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: skip-django-psycopg2-extension
-Version: 0.1.1.3
+Version: 0.2.0
 Summary: Library contains django commands which helps to prepare and manage PostgreSQL database.
 Home-page: https://github.com/skip-pay/django-psycopg2-extension
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<4.0,>=3.1
+Requires-Dist: django>=4.2
 
 # Django-psycopg2-extension
 
 Library contains django commands which helps to prepare and manage PostgreSQL database.
 
 ## Quickstart
```

### Comparing `skip-django-psycopg2-extension-0.1.1.3/skip_django_psycopg2_extension.egg-info/SOURCES.txt` & `skip_django_psycopg2_extension-0.2.0/skip_django_psycopg2_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

