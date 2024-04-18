# Comparing `tmp/newswacafi-0.6.tar.gz` & `tmp/newswacafi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newswacafi-0.6.tar", last modified: Wed Apr 17 08:06:03 2024, max compression
+gzip compressed data, was "newswacafi-0.7.tar", last modified: Thu Apr 18 17:13:18 2024, max compression
```

## Comparing `newswacafi-0.6.tar` & `newswacafi-0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-17 08:06:03.970917 newswacafi-0.6/
--rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-17 08:06:03.970674 newswacafi-0.6/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.6/README.md
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-17 08:06:03.968926 newswacafi-0.6/examples/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.6/examples/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.6/examples/base.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-17 08:06:03.969413 newswacafi-0.6/newswacafi/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.6/newswacafi/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)     2023 2024-04-17 08:01:51.000000 newswacafi-0.6/newswacafi/api.py
--rw-r--r--   0 moussier   (501) staff       (20)      430 2024-04-16 17:27:17.000000 newswacafi-0.6/newswacafi/response.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-17 08:06:03.970366 newswacafi-0.6/newswacafi.egg-info/
--rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-17 08:06:03.000000 newswacafi-0.6/newswacafi.egg-info/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-17 08:06:03.000000 newswacafi-0.6/newswacafi.egg-info/SOURCES.txt
--rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-17 08:06:03.000000 newswacafi-0.6/newswacafi.egg-info/dependency_links.txt
--rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-17 08:06:03.000000 newswacafi-0.6/newswacafi.egg-info/requires.txt
--rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-17 08:06:03.000000 newswacafi-0.6/newswacafi.egg-info/top_level.txt
--rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-17 08:06:03.970969 newswacafi-0.6/setup.cfg
--rw-r--r--   0 moussier   (501) staff       (20)      775 2024-04-17 08:05:50.000000 newswacafi-0.6/setup.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-18 17:13:18.030949 newswacafi-0.7/
+-rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-18 17:13:18.030702 newswacafi-0.7/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.7/README.md
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-18 17:13:18.028717 newswacafi-0.7/examples/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.7/examples/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.7/examples/base.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-18 17:13:18.029406 newswacafi-0.7/newswacafi/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.7/newswacafi/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)     2104 2024-04-18 16:52:14.000000 newswacafi-0.7/newswacafi/api.py
+-rw-r--r--   0 moussier   (501) staff       (20)      430 2024-04-16 17:27:17.000000 newswacafi-0.7/newswacafi/response.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-18 17:13:18.030418 newswacafi-0.7/newswacafi.egg-info/
+-rw-r--r--   0 moussier   (501) staff       (20)     1474 2024-04-18 17:13:18.000000 newswacafi-0.7/newswacafi.egg-info/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-18 17:13:18.000000 newswacafi-0.7/newswacafi.egg-info/SOURCES.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-18 17:13:18.000000 newswacafi-0.7/newswacafi.egg-info/dependency_links.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-18 17:13:18.000000 newswacafi-0.7/newswacafi.egg-info/requires.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-18 17:13:18.000000 newswacafi-0.7/newswacafi.egg-info/top_level.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-18 17:13:18.030995 newswacafi-0.7/setup.cfg
+-rw-r--r--   0 moussier   (501) staff       (20)      775 2024-04-18 17:13:14.000000 newswacafi-0.7/setup.py
```

### Comparing `newswacafi-0.6/PKG-INFO` & `newswacafi-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newswacafi
-Version: 0.6
+Version: 0.7
 Summary: Une bibliothèque Python pour interagir avec l'API de Newswacafi.
 Home-page: https://newswacafi.online
 Author: DRC WANALA
 Author-email: contact@newswacafi.online
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newswacafi-0.6/README.md` & `newswacafi-0.7/README.md`

 * *Files identical despite different names*

### Comparing `newswacafi-0.6/newswacafi/api.py` & `newswacafi-0.7/newswacafi/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from datetime import date
 from .response import NewsWacafiResponse, NewswacafiNews
 from typing import List
-
+import urllib.parse
 class NewswacafiClient:
     def __init__(self, api_key, api_secret):
         self.base_url = 'https://api.newswacafi.online/api'
         self.api_key = api_key
         self.api_secret = api_secret
 
     def get_news(self, start_date: date, end_date: date, source: List[str] = None, category: List[str] = None, country: List[str] = None, query: str = None) -> NewsWacafiResponse:
@@ -38,14 +38,16 @@
             req_url += f'&category={category}'
         if country:
             country = ','.join(country)
             req_url += f'&country={country}'
         if query:
             req_url += f'&query={query}'
 
+        req_url = urllib.parse.quote(req_url, safe=':/?&=,')
+
         response = requests.get(req_url, headers=headers)
         
         if response.ok:
             news_list = [NewswacafiNews(**news) for news in response.json()['data']]
             return NewsWacafiResponse(status=response.json()['status'], data=news_list)
         
         error = response.json()
```

### Comparing `newswacafi-0.6/newswacafi.egg-info/PKG-INFO` & `newswacafi-0.7/newswacafi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newswacafi
-Version: 0.6
+Version: 0.7
 Summary: Une bibliothèque Python pour interagir avec l'API de Newswacafi.
 Home-page: https://newswacafi.online
 Author: DRC WANALA
 Author-email: contact@newswacafi.online
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `newswacafi-0.6/setup.py` & `newswacafi-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='newswacafi',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     install_requires=['requests'],
     author='DRC WANALA',
     author_email='contact@newswacafi.online',
     description='Une bibliothèque Python pour interagir avec l\'API de Newswacafi.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

