# Comparing `tmp/django_activity_log-2.0.0.tar.gz` & `tmp/django_activity_log-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_activity_log-2.0.0.tar", last modified: Wed Apr 17 14:23:16 2024, max compression
+gzip compressed data, was "django_activity_log-2.0.1.tar", last modified: Wed Apr 17 14:31:57 2024, max compression
```

## Comparing `django_activity_log-2.0.0.tar` & `django_activity_log-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.578669 django_activity_log-2.0.0/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/LICENSE
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4917 2024-04-17 14:23:16.577216 django_activity_log-2.0.0/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4028 2024-02-15 13:02:30.000000 django_activity_log-2.0.0/README.md
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.564616 django_activity_log-2.0.0/activity_log/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/activity_log/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      848 2024-04-17 14:11:41.000000 django_activity_log-2.0.0/activity_log/admin.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django_activity_log-2.0.0/activity_log/conf.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     3523 2024-04-17 14:10:18.000000 django_activity_log-2.0.0/activity_log/middleware.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.567510 django_activity_log-2.0.0/activity_log/migrations/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2083 2024-04-17 14:18:24.000000 django_activity_log-2.0.0/activity_log/migrations/0001_initial.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.0/activity_log/migrations/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2786 2024-04-17 14:18:46.000000 django_activity_log-2.0.0/activity_log/models.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django_activity_log-2.0.0/activity_log/router.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:23:16.575626 django_activity_log-2.0.0/django_activity_log.egg-info/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4917 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/SOURCES.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/dependency_links.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       16 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/requires.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-04-17 14:23:16.000000 django_activity_log-2.0.0/django_activity_log.egg-info/top_level.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-17 14:23:16.578867 django_activity_log-2.0.0/setup.cfg
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1385 2024-04-17 14:22:29.000000 django_activity_log-2.0.0/setup.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.124338 django_activity_log-2.0.1/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/LICENSE
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-17 14:31:57.123497 django_activity_log-2.0.1/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4186 2024-04-17 14:31:45.000000 django_activity_log-2.0.1/README.md
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.112660 django_activity_log-2.0.1/activity_log/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/activity_log/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      848 2024-04-17 14:11:41.000000 django_activity_log-2.0.1/activity_log/admin.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django_activity_log-2.0.1/activity_log/conf.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     3523 2024-04-17 14:10:18.000000 django_activity_log-2.0.1/activity_log/middleware.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.115016 django_activity_log-2.0.1/activity_log/migrations/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2083 2024-04-17 14:18:24.000000 django_activity_log-2.0.1/activity_log/migrations/0001_initial.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/activity_log/migrations/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2786 2024-04-17 14:18:46.000000 django_activity_log-2.0.1/activity_log/models.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django_activity_log-2.0.1/activity_log/router.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.122669 django_activity_log-2.0.1/django_activity_log.egg-info/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       28 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/requires.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/top_level.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-17 14:31:57.124473 django_activity_log-2.0.1/setup.cfg
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1397 2024-04-17 14:29:17.000000 django_activity_log-2.0.1/setup.py
```

### Comparing `django_activity_log-2.0.0/LICENSE` & `django_activity_log-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/PKG-INFO` & `django_activity_log-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 2.0.0
+Version: 2.0.1
 Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: pprintpp
+Requires-Dist: django<5.0.0
+Requires-Dist: pprintpp<1.0.0
 
 # django-activity-log
 
 Forked from : 
 [scailer/django-user-activity-log](https://github.com/scailer/django-user-activity-log)
 __________________________________________________________
 ## Owner's Expressions :
@@ -146,9 +146,12 @@
 
 #### 7. Test on django version 4.0.1:
 It works well with Django version 4.0.1.
 
 #### 8. change migration files:
 Delete old migrations and create one file to migrate models of this library.
 
+#### 9. IP Management:
+In admin panel , Model BlackListIPAdress you can archive or block every ip address would you like with its network address or not.
+
 Repository : 
 [HosseinSayyedMousavi/django-user-activity-log](https://github.com/HosseinSayyedMousavi/django-user-activity-log/)
```

### Comparing `django_activity_log-2.0.0/README.md` & `django_activity_log-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,9 +120,12 @@
 
 #### 7. Test on django version 4.0.1:
 It works well with Django version 4.0.1.
 
 #### 8. change migration files:
 Delete old migrations and create one file to migrate models of this library.
 
+#### 9. IP Management:
+In admin panel , Model BlackListIPAdress you can archive or block every ip address would you like with its network address or not.
+
 Repository : 
 [HosseinSayyedMousavi/django-user-activity-log](https://github.com/HosseinSayyedMousavi/django-user-activity-log/)
```

### Comparing `django_activity_log-2.0.0/activity_log/admin.py` & `django_activity_log-2.0.1/activity_log/admin.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/activity_log/conf.py` & `django_activity_log-2.0.1/activity_log/conf.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/activity_log/middleware.py` & `django_activity_log-2.0.1/activity_log/middleware.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/activity_log/migrations/0001_initial.py` & `django_activity_log-2.0.1/activity_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/activity_log/models.py` & `django_activity_log-2.0.1/activity_log/models.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/activity_log/router.py` & `django_activity_log-2.0.1/activity_log/router.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.0/django_activity_log.egg-info/PKG-INFO` & `django_activity_log-2.0.1/django_activity_log.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 2.0.0
+Version: 2.0.1
 Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
@@ -17,16 +17,16 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django
-Requires-Dist: pprintpp
+Requires-Dist: django<5.0.0
+Requires-Dist: pprintpp<1.0.0
 
 # django-activity-log
 
 Forked from : 
 [scailer/django-user-activity-log](https://github.com/scailer/django-user-activity-log)
 __________________________________________________________
 ## Owner's Expressions :
@@ -146,9 +146,12 @@
 
 #### 7. Test on django version 4.0.1:
 It works well with Django version 4.0.1.
 
 #### 8. change migration files:
 Delete old migrations and create one file to migrate models of this library.
 
+#### 9. IP Management:
+In admin panel , Model BlackListIPAdress you can archive or block every ip address would you like with its network address or not.
+
 Repository : 
 [HosseinSayyedMousavi/django-user-activity-log](https://github.com/HosseinSayyedMousavi/django-user-activity-log/)
```

### Comparing `django_activity_log-2.0.0/setup.py` & `django_activity_log-2.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 
 DESCRIPTION = open('README.md').read()
 setup(
     name='django-activity-log',
-    version='2.0.0',
+    version='2.0.1',
     description='HTTP queries logger with flexible filters and ip block manager.',
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     author='Hossein SayyedMousavi',
     author_email='hossein.sayyedmousavi@gmail.com',
     keywords=[
         "django",
@@ -22,16 +22,16 @@
         'activity_log',
         'activity_log.migrations',
     ],
     url='https://github.com/HosseinSayyedMousavi',
     license='MIT License',
     readme="README.md",
     install_requires=[
-        'django',
-        'pprintpp',
+        'django<5.0.0',
+        'pprintpp<1.0.0',
     ],
 
     include_package_data=True,
     classifiers=[
         'Framework :: Django',
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
```

