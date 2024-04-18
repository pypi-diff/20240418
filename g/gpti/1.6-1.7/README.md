# Comparing `tmp/gpti-1.6.tar.gz` & `tmp/gpti-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpti-1.6.tar", last modified: Wed Apr 17 23:32:03 2024, max compression
+gzip compressed data, was "gpti-1.7.tar", last modified: Thu Apr 18 01:59:14 2024, max compression
```

## Comparing `gpti-1.6.tar` & `gpti-1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 23:32:03.574653 gpti-1.6/
--rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.6/LICENSE
--rw-rw-rw-   0        0        0    68607 2024-04-17 23:32:03.569745 gpti-1.6/PKG-INFO
--rw-rw-rw-   0        0        0    66390 2024-04-17 23:29:48.000000 gpti-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 23:32:03.547066 gpti-1.6/gpti/
--rw-rw-rw-   0        0        0   121628 2024-04-17 23:13:43.000000 gpti-1.6/gpti/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 23:32:03.567219 gpti-1.6/gpti.egg-info/
--rw-rw-rw-   0        0        0    68607 2024-04-17 23:32:03.000000 gpti-1.6/gpti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-17 23:32:03.000000 gpti-1.6/gpti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 23:32:03.000000 gpti-1.6/gpti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 23:32:03.000000 gpti-1.6/gpti.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 23:32:03.000000 gpti-1.6/gpti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 23:32:03.574653 gpti-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1180 2024-04-17 23:14:12.000000 gpti-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 01:59:14.616904 gpti-1.7/
+-rw-rw-rw-   0        0        0     1084 2024-01-24 17:14:27.000000 gpti-1.7/LICENSE
+-rw-rw-rw-   0        0        0    68491 2024-04-18 01:59:14.616904 gpti-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    66276 2024-04-18 01:56:18.000000 gpti-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 01:59:14.600902 gpti-1.7/gpti/
+-rw-rw-rw-   0        0        0   121628 2024-04-17 23:13:43.000000 gpti-1.7/gpti/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 01:59:14.616904 gpti-1.7/gpti.egg-info/
+-rw-rw-rw-   0        0        0    68491 2024-04-18 01:59:14.000000 gpti-1.7/gpti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-18 01:59:14.000000 gpti-1.7/gpti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 01:59:14.000000 gpti-1.7/gpti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 01:59:14.000000 gpti-1.7/gpti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 01:59:14.000000 gpti-1.7/gpti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 01:59:14.632733 gpti-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2024-04-18 01:58:13.000000 gpti-1.7/setup.py
```

### Comparing `gpti-1.6/LICENSE` & `gpti-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpti-1.6/PKG-INFO` & `gpti-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.6
+Version: 1.7
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -211,15 +211,14 @@
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
 
 #### JSON
 
 ```json
-{"message":"Hello! How are you today?","original":null,"finish":false,"error":false}
 {"message":"","original":null,"finish":false,"error":false}
 {"message":"Of","original":null,"finish":false,"error":false}
 {"message":"Of course","original":null,"finish":false,"error":false}
 {"message":"Of course,","original":null,"finish":false,"error":false}
 {"message":"Of course, Yand","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri!","original":null,"finish":false,"error":false}
@@ -270,17 +269,16 @@
 import json
 from gpti import gpt
 
 res = gpt.prompts(lang="en", limit=4, offset=0)
 
 if res.error != None:
     print(json.dumps(res.error))
-else:
-    for chunk in res.stream():
-        print(json.dumps(chunk))
+else: 
+    print(json.dumps(res.result))
 ```
 
 #### JSON
 
 ```json
 {
     "code": 200,
```

### Comparing `gpti-1.6/README.md` & `gpti-1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,14 @@
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
 
 #### JSON
 
 ```json
-{"message":"Hello! How are you today?","original":null,"finish":false,"error":false}
 {"message":"","original":null,"finish":false,"error":false}
 {"message":"Of","original":null,"finish":false,"error":false}
 {"message":"Of course","original":null,"finish":false,"error":false}
 {"message":"Of course,","original":null,"finish":false,"error":false}
 {"message":"Of course, Yand","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri!","original":null,"finish":false,"error":false}
@@ -254,17 +253,16 @@
 import json
 from gpti import gpt
 
 res = gpt.prompts(lang="en", limit=4, offset=0)
 
 if res.error != None:
     print(json.dumps(res.error))
-else:
-    for chunk in res.stream():
-        print(json.dumps(chunk))
+else: 
+    print(json.dumps(res.result))
 ```
 
 #### JSON
 
 ```json
 {
     "code": 200,
```

### Comparing `gpti-1.6/gpti/__init__.py` & `gpti-1.7/gpti/__init__.py`

 * *Files identical despite different names*

### Comparing `gpti-1.6/gpti.egg-info/PKG-INFO` & `gpti-1.7/gpti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpti
-Version: 1.6
+Version: 1.7
 Summary: This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT
 Home-page: https://github.com/yandricr/gpti-py/
 Author: yandricr
 Author-email: yandribret@gmail.com
 License: MIT
 Project-URL: Documentation, https://nexra.aryahcr.cc/
 Project-URL: Funding, https://ko-fi.com/yandricr
@@ -211,15 +211,14 @@
     for chunk in res.stream():
         print(json.dumps(chunk))
 ```
 
 #### JSON
 
 ```json
-{"message":"Hello! How are you today?","original":null,"finish":false,"error":false}
 {"message":"","original":null,"finish":false,"error":false}
 {"message":"Of","original":null,"finish":false,"error":false}
 {"message":"Of course","original":null,"finish":false,"error":false}
 {"message":"Of course,","original":null,"finish":false,"error":false}
 {"message":"Of course, Yand","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri","original":null,"finish":false,"error":false}
 {"message":"Of course, Yandri!","original":null,"finish":false,"error":false}
@@ -270,17 +269,16 @@
 import json
 from gpti import gpt
 
 res = gpt.prompts(lang="en", limit=4, offset=0)
 
 if res.error != None:
     print(json.dumps(res.error))
-else:
-    for chunk in res.stream():
-        print(json.dumps(chunk))
+else: 
+    print(json.dumps(res.result))
 ```
 
 #### JSON
 
 ```json
 {
     "code": 200,
```

### Comparing `gpti-1.6/setup.py` & `gpti-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as f:
         _long_description = f.read()
 except Exception as e:
     _long_description = ''
 
 setup(
     name='gpti',
-    version='1.6',
+    version='1.7',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='yandricr',
     author_email='yandribret@gmail.com',
     description='This package simplifies your interaction with various GPT models, removing the need for tokens or other methods to access GPT',
```

