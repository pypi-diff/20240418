# Comparing `tmp/ourJWT-0.1.1.tar.gz` & `tmp/ourJWT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.1.1.tar", last modified: Tue Apr 16 14:00:32 2024, max compression
+gzip compressed data, was "ourJWT-0.1.2.tar", last modified: Thu Apr 18 13:09:02 2024, max compression
```

## Comparing `ourJWT-0.1.1.tar` & `ourJWT-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 14:00:32.546739 ourJWT-0.1.1/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 14:00:32.546739 ourJWT-0.1.1/PKG-INFO
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 14:00:32.546739 ourJWT-0.1.1/ourJWT/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3404 2024-04-16 13:56:23.000000 ourJWT-0.1.1/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.1/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.1/ourJWT/__init__.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      850 2024-04-16 13:50:22.000000 ourJWT-0.1.1/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-16 14:00:32.546739 ourJWT-0.1.1/ourJWT.egg-info/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-16 14:00:32.000000 ourJWT-0.1.1/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-16 14:00:32.000000 ourJWT-0.1.1/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-16 14:00:32.000000 ourJWT-0.1.1/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-16 14:00:32.000000 ourJWT-0.1.1/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-16 14:00:32.000000 ourJWT-0.1.1/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-16 14:00:32.546739 ourJWT-0.1.1/setup.cfg
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-16 14:00:23.000000 ourJWT-0.1.1/setup.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-18 13:09:02.197737 ourJWT-0.1.2/PKG-INFO
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/ourJWT/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3404 2024-04-16 13:56:23.000000 ourJWT-0.1.2/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.2/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.2/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      859 2024-04-18 13:07:16.000000 ourJWT-0.1.2/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-18 13:09:02.197737 ourJWT-0.1.2/setup.cfg
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-18 13:07:59.000000 ourJWT-0.1.2/setup.py
```

### Comparing `ourJWT-0.1.1/ourJWT/OUR_class.py` & `ourJWT-0.1.2/ourJWT/OUR_class.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.1.1/ourJWT/decorators.py` & `ourJWT-0.1.2/ourJWT/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,11 +14,11 @@
             if auth is None:
                 return response.HttpResponseBadRequest(reason="No auth cookie sent")
             try:
                 auth_decoded = decoder.decode(auth)
             except (OUR_exception.BadSubject,
                     OUR_exception.RefusedToken,
                     OUR_exception.ExpiredToken):
-                return HttpResponseUnauthorized(reason="Bad auth token")
+                return response.HttpResponse(status=469, reason="Bad auth token")
             return function(request, token=auth_decoded)
         return wrapper
     return decorator
```

### Comparing `ourJWT-0.1.1/setup.py` & `ourJWT-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.1.1',
+    version='0.1.2',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

