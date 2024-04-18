# Comparing `tmp/django_activity_log-2.0.1.tar.gz` & `tmp/django_activity_log-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_activity_log-2.0.1.tar", last modified: Wed Apr 17 14:31:57 2024, max compression
+gzip compressed data, was "django_activity_log-2.0.2.tar", last modified: Thu Apr 18 12:30:16 2024, max compression
```

## Comparing `django_activity_log-2.0.1.tar` & `django_activity_log-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.124338 django_activity_log-2.0.1/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/LICENSE
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-17 14:31:57.123497 django_activity_log-2.0.1/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4186 2024-04-17 14:31:45.000000 django_activity_log-2.0.1/README.md
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.112660 django_activity_log-2.0.1/activity_log/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/activity_log/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      848 2024-04-17 14:11:41.000000 django_activity_log-2.0.1/activity_log/admin.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django_activity_log-2.0.1/activity_log/conf.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     3523 2024-04-17 14:10:18.000000 django_activity_log-2.0.1/activity_log/middleware.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.115016 django_activity_log-2.0.1/activity_log/migrations/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2083 2024-04-17 14:18:24.000000 django_activity_log-2.0.1/activity_log/migrations/0001_initial.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.1/activity_log/migrations/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2786 2024-04-17 14:18:46.000000 django_activity_log-2.0.1/activity_log/models.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django_activity_log-2.0.1/activity_log/router.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-17 14:31:57.122669 django_activity_log-2.0.1/django_activity_log.egg-info/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/SOURCES.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/dependency_links.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       28 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/requires.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-04-17 14:31:57.000000 django_activity_log-2.0.1/django_activity_log.egg-info/top_level.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-17 14:31:57.124473 django_activity_log-2.0.1/setup.cfg
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1397 2024-04-17 14:29:17.000000 django_activity_log-2.0.1/setup.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-18 12:30:16.304521 django_activity_log-2.0.2/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1081 2024-02-10 07:53:01.000000 django_activity_log-2.0.2/LICENSE
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-18 12:30:16.303638 django_activity_log-2.0.2/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     4186 2024-04-17 14:31:45.000000 django_activity_log-2.0.2/README.md
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-18 12:30:16.293337 django_activity_log-2.0.2/activity_log/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.2/activity_log/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      848 2024-04-17 14:11:41.000000 django_activity_log-2.0.2/activity_log/admin.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2207 2024-02-10 07:57:03.000000 django_activity_log-2.0.2/activity_log/conf.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     3464 2024-04-18 12:23:02.000000 django_activity_log-2.0.2/activity_log/middleware.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-18 12:30:16.295988 django_activity_log-2.0.2/activity_log/migrations/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2083 2024-04-17 14:18:24.000000 django_activity_log-2.0.2/activity_log/migrations/0001_initial.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-02-10 07:53:01.000000 django_activity_log-2.0.2/activity_log/migrations/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2786 2024-04-17 14:18:46.000000 django_activity_log-2.0.2/activity_log/models.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1464 2024-02-10 07:56:50.000000 django_activity_log-2.0.2/activity_log/router.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-18 12:30:16.302781 django_activity_log-2.0.2/django_activity_log.egg-info/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     5084 2024-04-18 12:30:16.000000 django_activity_log-2.0.2/django_activity_log.egg-info/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      457 2024-04-18 12:30:16.000000 django_activity_log-2.0.2/django_activity_log.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-18 12:30:16.000000 django_activity_log-2.0.2/django_activity_log.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       28 2024-04-18 12:30:16.000000 django_activity_log-2.0.2/django_activity_log.egg-info/requires.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       13 2024-04-18 12:30:16.000000 django_activity_log-2.0.2/django_activity_log.egg-info/top_level.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-18 12:30:16.304704 django_activity_log-2.0.2/setup.cfg
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1397 2024-04-18 12:30:02.000000 django_activity_log-2.0.2/setup.py
```

### Comparing `django_activity_log-2.0.1/LICENSE` & `django_activity_log-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/PKG-INFO` & `django_activity_log-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 2.0.1
+Version: 2.0.2
 Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
```

### Comparing `django_activity_log-2.0.1/README.md` & `django_activity_log-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/activity_log/admin.py` & `django_activity_log-2.0.2/activity_log/admin.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/activity_log/conf.py` & `django_activity_log-2.0.2/activity_log/conf.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/activity_log/middleware.py` & `django_activity_log-2.0.2/activity_log/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,12 +88,10 @@
             payload =  request.body
         )
     def __call__(self, request):
         ip_address = get_ip_address(request)
         network_address =re.findall(r"([\.\d]+)\.",ip_address)[0]
         query = Q(block_network_address=True , ip_address__startswith = network_address , blocked = True) | Q(ip_address=ip_address , blocked = True)
         if BlackListIPAdress.objects.filter(query).exists() :
-            response = HttpResponseForbidden()
-        else: 
-            response = self.get_response(request)
+            return HttpResponseForbidden()
 
-        return response
+        return super().__call__()
```

### Comparing `django_activity_log-2.0.1/activity_log/migrations/0001_initial.py` & `django_activity_log-2.0.2/activity_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/activity_log/models.py` & `django_activity_log-2.0.2/activity_log/models.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/activity_log/router.py` & `django_activity_log-2.0.2/activity_log/router.py`

 * *Files identical despite different names*

### Comparing `django_activity_log-2.0.1/django_activity_log.egg-info/PKG-INFO` & `django_activity_log-2.0.2/django_activity_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-activity-log
-Version: 2.0.1
+Version: 2.0.2
 Summary: HTTP queries logger with flexible filters and ip block manager.
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein SayyedMousavi
 Author-email: hossein.sayyedmousavi@gmail.com
 License: MIT License
 Keywords: django,database,user,activity log
 Classifier: Framework :: Django
```

### Comparing `django_activity_log-2.0.1/setup.py` & `django_activity_log-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 
 DESCRIPTION = open('README.md').read()
 setup(
     name='django-activity-log',
-    version='2.0.1',
+    version='2.0.2',
     description='HTTP queries logger with flexible filters and ip block manager.',
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     author='Hossein SayyedMousavi',
     author_email='hossein.sayyedmousavi@gmail.com',
     keywords=[
         "django",
```

