# Comparing `tmp/django-tsso-0.0.1b1.tar.gz` & `tmp/django-tsso-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tsso-0.0.1b1.tar", last modified: Fri Mar 29 11:49:06 2024, max compression
+gzip compressed data, was "django-tsso-0.0.1b2.tar", last modified: Thu Apr 18 07:40:01 2024, max compression
```

## Comparing `django-tsso-0.0.1b1.tar` & `django-tsso-0.0.1b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/
--rw-rw-r--   0 seva      (1000) seva      (1000)     7652 2022-05-09 07:47:47.000000 django-tsso-0.0.1b1/LICENSE
--rw-rw-r--   0 seva      (1000) seva      (1000)     1147 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/PKG-INFO
--rw-rw-r--   0 seva      (1000) seva      (1000)     7696 2024-03-29 11:28:07.000000 django-tsso-0.0.1b1/README.md
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.978979 django-tsso-0.0.1b1/django_tsso.egg-info/
--rw-rw-r--   0 seva      (1000) seva      (1000)     1147 2024-03-29 11:49:06.000000 django-tsso-0.0.1b1/django_tsso.egg-info/PKG-INFO
--rw-rw-r--   0 seva      (1000) seva      (1000)      504 2024-03-29 11:49:06.000000 django-tsso-0.0.1b1/django_tsso.egg-info/SOURCES.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)        1 2024-03-29 11:49:06.000000 django-tsso-0.0.1b1/django_tsso.egg-info/dependency_links.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)        1 2024-03-29 10:11:57.000000 django-tsso-0.0.1b1/django_tsso.egg-info/not-zip-safe
--rw-rw-r--   0 seva      (1000) seva      (1000)       35 2024-03-29 11:49:06.000000 django-tsso-0.0.1b1/django_tsso.egg-info/requires.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)        5 2024-03-29 11:49:06.000000 django-tsso-0.0.1b1/django_tsso.egg-info/top_level.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)     1569 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/setup.cfg
--rwxrwxr-x   0 seva      (1000) seva      (1000)       62 2024-03-08 08:50:29.000000 django-tsso-0.0.1b1/setup.py
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/tsso/
--rw-rw-r--   0 seva      (1000) seva      (1000)      119 2024-03-26 14:09:34.000000 django-tsso-0.0.1b1/tsso/__init__.py
--rw-rw-r--   0 seva      (1000) seva      (1000)      919 2024-03-27 15:29:07.000000 django-tsso-0.0.1b1/tsso/admin.py
--rw-rw-r--   0 seva      (1000) seva      (1000)      232 2024-03-28 06:37:08.000000 django-tsso-0.0.1b1/tsso/apps.py
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/tsso/contrib/
--rw-rw-r--   0 seva      (1000) seva      (1000)       65 2024-03-29 10:20:34.000000 django-tsso-0.0.1b1/tsso/contrib/__init__.py
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/tsso/contrib/rest/
--rw-rw-r--   0 seva      (1000) seva      (1000)       60 2024-03-29 10:20:23.000000 django-tsso-0.0.1b1/tsso/contrib/rest/__init__.py
--rw-rw-r--   0 seva      (1000) seva      (1000)      717 2024-03-29 10:20:11.000000 django-tsso-0.0.1b1/tsso/contrib/rest/authentication.py
--rw-rw-r--   0 seva      (1000) seva      (1000)      869 2024-03-29 06:23:41.000000 django-tsso-0.0.1b1/tsso/middleware.py
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-03-29 11:49:06.982979 django-tsso-0.0.1b1/tsso/migrations/
--rw-rw-r--   0 seva      (1000) seva      (1000)     2958 2024-03-27 14:28:04.000000 django-tsso-0.0.1b1/tsso/migrations/0001_initial.py
--rw-rw-r--   0 seva      (1000) seva      (1000)        0 2024-03-27 14:28:04.000000 django-tsso-0.0.1b1/tsso/migrations/__init__.py
--rw-rw-r--   0 seva      (1000) seva      (1000)     4169 2024-03-29 10:18:48.000000 django-tsso-0.0.1b1/tsso/mixins.py
--rw-rw-r--   0 seva      (1000) seva      (1000)     2023 2024-03-29 10:16:31.000000 django-tsso-0.0.1b1/tsso/models.py
--rw-rw-r--   0 seva      (1000) seva      (1000)       24 2024-03-26 13:36:07.000000 django-tsso-0.0.1b1/tsso/version.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/
+-rw-rw-r--   0 seva      (1000) seva      (1000)     7652 2022-05-09 07:47:47.000000 django-tsso-0.0.1b2/LICENSE
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1147 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/PKG-INFO
+-rw-rw-r--   0 seva      (1000) seva      (1000)     7696 2024-03-29 11:28:07.000000 django-tsso-0.0.1b2/README.md
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.509968 django-tsso-0.0.1b2/django_tsso.egg-info/
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1147 2024-04-18 07:40:01.000000 django-tsso-0.0.1b2/django_tsso.egg-info/PKG-INFO
+-rw-rw-r--   0 seva      (1000) seva      (1000)      504 2024-04-18 07:40:01.000000 django-tsso-0.0.1b2/django_tsso.egg-info/SOURCES.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)        1 2024-04-18 07:40:01.000000 django-tsso-0.0.1b2/django_tsso.egg-info/dependency_links.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)        1 2024-03-29 10:11:57.000000 django-tsso-0.0.1b2/django_tsso.egg-info/not-zip-safe
+-rw-rw-r--   0 seva      (1000) seva      (1000)       35 2024-04-18 07:40:01.000000 django-tsso-0.0.1b2/django_tsso.egg-info/requires.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)        5 2024-04-18 07:40:01.000000 django-tsso-0.0.1b2/django_tsso.egg-info/top_level.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1569 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/setup.cfg
+-rwxrwxr-x   0 seva      (1000) seva      (1000)       62 2024-03-08 08:50:29.000000 django-tsso-0.0.1b2/setup.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/tsso/
+-rw-rw-r--   0 seva      (1000) seva      (1000)      119 2024-03-26 14:09:34.000000 django-tsso-0.0.1b2/tsso/__init__.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)      919 2024-03-27 15:29:07.000000 django-tsso-0.0.1b2/tsso/admin.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)      232 2024-03-28 06:37:08.000000 django-tsso-0.0.1b2/tsso/apps.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/tsso/contrib/
+-rw-rw-r--   0 seva      (1000) seva      (1000)       65 2024-03-29 10:20:34.000000 django-tsso-0.0.1b2/tsso/contrib/__init__.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/tsso/contrib/rest/
+-rw-rw-r--   0 seva      (1000) seva      (1000)       60 2024-03-29 10:20:23.000000 django-tsso-0.0.1b2/tsso/contrib/rest/__init__.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)      717 2024-03-29 10:20:11.000000 django-tsso-0.0.1b2/tsso/contrib/rest/authentication.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)      869 2024-03-29 06:23:41.000000 django-tsso-0.0.1b2/tsso/middleware.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2024-04-18 07:40:01.513968 django-tsso-0.0.1b2/tsso/migrations/
+-rw-rw-r--   0 seva      (1000) seva      (1000)     2958 2024-03-27 14:28:04.000000 django-tsso-0.0.1b2/tsso/migrations/0001_initial.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)        0 2024-03-27 14:28:04.000000 django-tsso-0.0.1b2/tsso/migrations/__init__.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)     4169 2024-03-29 10:18:48.000000 django-tsso-0.0.1b2/tsso/mixins.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)     2023 2024-03-29 10:16:31.000000 django-tsso-0.0.1b2/tsso/models.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)       24 2024-04-18 07:39:23.000000 django-tsso-0.0.1b2/tsso/version.py
```

### Comparing `django-tsso-0.0.1b1/LICENSE` & `django-tsso-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/PKG-INFO` & `django-tsso-0.0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tsso
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Transparent Single Sign On for Django-based Service Provider
 Home-page: http://pypi.python.org/pypi/django-tsso
 Author: Vsevolod Novikov
 Author-email: nnseva@gmail.com
 Keywords: authentication,authorization,SSO,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-tsso-0.0.1b1/README.md` & `django-tsso-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/django_tsso.egg-info/PKG-INFO` & `django-tsso-0.0.1b2/django_tsso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tsso
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Transparent Single Sign On for Django-based Service Provider
 Home-page: http://pypi.python.org/pypi/django-tsso
 Author: Vsevolod Novikov
 Author-email: nnseva@gmail.com
 Keywords: authentication,authorization,SSO,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-tsso-0.0.1b1/setup.cfg` & `django-tsso-0.0.1b2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,14 @@
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 python_requires = >=3.0
 install_requires = 
-	django >= 4.1
+	django >= 3.0
 	social-auth-app-django
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-tsso-0.0.1b1/tsso/admin.py` & `django-tsso-0.0.1b2/tsso/admin.py`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/tsso/contrib/rest/authentication.py` & `django-tsso-0.0.1b2/tsso/contrib/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/tsso/middleware.py` & `django-tsso-0.0.1b2/tsso/middleware.py`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/tsso/migrations/0001_initial.py` & `django-tsso-0.0.1b2/tsso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/tsso/mixins.py` & `django-tsso-0.0.1b2/tsso/mixins.py`

 * *Files identical despite different names*

### Comparing `django-tsso-0.0.1b1/tsso/models.py` & `django-tsso-0.0.1b2/tsso/models.py`

 * *Files identical despite different names*

