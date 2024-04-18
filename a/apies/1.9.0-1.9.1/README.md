# Comparing `tmp/apies-1.9.0.tar.gz` & `tmp/apies-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apies-1.9.0.tar", last modified: Sun Feb 12 17:47:55 2023, max compression
+gzip compressed data, was "apies-1.9.1.tar", last modified: Sun Feb 12 18:05:57 2023, max compression
```

## Comparing `apies-1.9.0.tar` & `apies-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 17:47:55.513769 apies-1.9.0/
--rw-r--r--   0 adam       (501) staff       (20)      123 2021-02-03 16:35:37.000000 apies-1.9.0/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      453 2021-02-03 16:35:37.000000 apies-1.9.0/Makefile
--rw-r--r--   0 adam       (501) staff       (20)    11776 2023-02-12 17:47:55.514035 apies-1.9.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     9090 2022-12-21 11:12:39.000000 apies-1.9.0/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 17:47:55.510437 apies-1.9.0/apies/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-02-12 17:45:18.000000 apies-1.9.0/apies/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       57 2021-02-03 16:35:37.000000 apies-1.9.0/apies/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     9539 2022-11-13 16:01:08.000000 apies-1.9.0/apies/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)     9200 2023-02-12 17:34:20.000000 apies-1.9.0/apies/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      263 2021-02-03 16:35:37.000000 apies-1.9.0/apies/logger.py
--rw-r--r--   0 adam       (501) staff       (20)    12327 2022-12-26 09:57:14.000000 apies-1.9.0/apies/query.py
--rw-r--r--   0 adam       (501) staff       (20)     1906 2022-09-27 16:37:49.000000 apies-1.9.0/apies/sources.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 17:47:55.513236 apies-1.9.0/apies/utils/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-02-03 16:35:37.000000 apies-1.9.0/apies/utils/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7488 2021-02-03 16:35:37.000000 apies-1.9.0/apies/utils/file_maker.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 17:47:55.512776 apies-1.9.0/apies.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)    11776 2023-02-12 17:47:54.000000 apies-1.9.0/apies.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      399 2023-02-12 17:47:55.000000 apies-1.9.0/apies.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-02-12 17:47:54.000000 apies-1.9.0/apies.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-02-04 08:42:07.000000 apies-1.9.0/apies.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      194 2023-02-12 17:47:54.000000 apies-1.9.0/apies.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        6 2023-02-12 17:47:54.000000 apies-1.9.0/apies.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-02-12 17:47:55.514570 apies-1.9.0/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1937 2022-07-22 17:26:58.000000 apies-1.9.0/setup.py
--rw-r--r--   0 adam       (501) staff       (20)      363 2021-02-03 16:35:37.000000 apies-1.9.0/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 18:05:57.496302 apies-1.9.1/
+-rw-r--r--   0 adam       (501) staff       (20)      123 2021-02-03 16:35:37.000000 apies-1.9.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      453 2021-02-03 16:35:37.000000 apies-1.9.1/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)    11776 2023-02-12 18:05:57.496629 apies-1.9.1/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     9090 2022-12-21 11:12:39.000000 apies-1.9.1/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 18:05:57.492186 apies-1.9.1/apies/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-02-12 18:05:31.000000 apies-1.9.1/apies/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       57 2021-02-03 16:35:37.000000 apies-1.9.1/apies/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     9539 2022-11-13 16:01:08.000000 apies-1.9.1/apies/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)     9269 2023-02-12 18:04:55.000000 apies-1.9.1/apies/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      263 2021-02-03 16:35:37.000000 apies-1.9.1/apies/logger.py
+-rw-r--r--   0 adam       (501) staff       (20)    12327 2022-12-26 09:57:14.000000 apies-1.9.1/apies/query.py
+-rw-r--r--   0 adam       (501) staff       (20)     1906 2022-09-27 16:37:49.000000 apies-1.9.1/apies/sources.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 18:05:57.495491 apies-1.9.1/apies/utils/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-02-03 16:35:37.000000 apies-1.9.1/apies/utils/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7488 2021-02-03 16:35:37.000000 apies-1.9.1/apies/utils/file_maker.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-12 18:05:57.494953 apies-1.9.1/apies.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)    11776 2023-02-12 18:05:56.000000 apies-1.9.1/apies.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      399 2023-02-12 18:05:57.000000 apies-1.9.1/apies.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-02-12 18:05:56.000000 apies-1.9.1/apies.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-02-04 08:42:07.000000 apies-1.9.1/apies.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      194 2023-02-12 18:05:56.000000 apies-1.9.1/apies.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        6 2023-02-12 18:05:56.000000 apies-1.9.1/apies.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-02-12 18:05:57.497277 apies-1.9.1/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1937 2022-07-22 17:26:58.000000 apies-1.9.1/setup.py
+-rw-r--r--   0 adam       (501) staff       (20)      363 2021-02-03 16:35:37.000000 apies-1.9.1/tox.ini
```

### Comparing `apies-1.9.0/PKG-INFO` & `apies-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apies
-Version: 1.9.0
+Version: 1.9.1
 Summary: A flask blueprint providing an API for accessing and searching an ElasticSearch index created from source datapackages
 Home-page: https://github.com/OpenBudget/apies
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # apies
```

### Comparing `apies-1.9.0/README.md` & `apies-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `apies-1.9.0/apies/blueprint.py` & `apies-1.9.1/apies/blueprint.py`

 * *Files identical despite different names*

### Comparing `apies-1.9.0/apies/controllers.py` & `apies-1.9.1/apies/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,23 @@
                 field_parts = field.split('.')
                 out_field = []
                 src = [source]
                 as_list = False
                 while len(field_parts) > 0:
                     field = field_parts.pop(0)
                     out_field.append(field)
-                    if isinstance(src[0].get(field), list):
-                        as_list = True
-                        src_ = []
-                        for s in src:
-                            src_.extend(s[field])
-                        src = src_
-                    elif isinstance(src[0], dict):
-                        src = [s[field] for s in src]
+                    if all(isinstance(s, dict) for s in src):
+                        if isinstance(src[0].get(field), list):
+                            as_list = True
+                            src_ = []
+                            for s in src:
+                                src_.extend(s[field])
+                            src = src_
+                        else:
+                            src = [s[field] for s in src]
                     else:
                         break
                 out_field = '.'.join(out_field)
                 if as_list:
                     cleaned = [h.replace('<em>', '').replace('</em>', '') for h in highlighted]
                     out = []
                     for s in src:
```

### Comparing `apies-1.9.0/apies/query.py` & `apies-1.9.1/apies/query.py`

 * *Files identical despite different names*

### Comparing `apies-1.9.0/apies/sources.py` & `apies-1.9.1/apies/sources.py`

 * *Files identical despite different names*

### Comparing `apies-1.9.0/apies/utils/file_maker.py` & `apies-1.9.1/apies/utils/file_maker.py`

 * *Files identical despite different names*

### Comparing `apies-1.9.0/apies.egg-info/PKG-INFO` & `apies-1.9.1/apies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apies
-Version: 1.9.0
+Version: 1.9.1
 Summary: A flask blueprint providing an API for accessing and searching an ElasticSearch index created from source datapackages
 Home-page: https://github.com/OpenBudget/apies
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # apies
```

### Comparing `apies-1.9.0/setup.py` & `apies-1.9.1/setup.py`

 * *Files identical despite different names*

