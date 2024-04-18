# Comparing `tmp/krypper_tgstat-0.1.8.tar.gz` & `tmp/krypper_tgstat-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krypper_tgstat-0.1.8.tar", last modified: Thu Apr 18 13:47:27 2024, max compression
+gzip compressed data, was "krypper_tgstat-0.1.8.1.tar", last modified: Thu Apr 18 14:05:54 2024, max compression
```

## Comparing `krypper_tgstat-0.1.8.tar` & `krypper_tgstat-0.1.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8/LICENSE
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8/README.md
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.361109 krypper_tgstat-0.1.8/krypper_tgstat/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      242 2024-04-18 13:44:27.000000 krypper_tgstat-0.1.8/krypper_tgstat/__init__.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    10375 2024-04-18 13:25:29.000000 krypper_tgstat-0.1.8/krypper_tgstat/classes.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-18 13:20:59.000000 krypper_tgstat-0.1.8/krypper_tgstat/enums.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-18 13:43:39.000000 krypper_tgstat-0.1.8/krypper_tgstat/exceptions.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8067 2024-04-18 13:43:49.000000 krypper_tgstat-0.1.8/krypper_tgstat/tg_stat.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      955 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/SOURCES.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/dependency_links.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/requires.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-18 13:47:27.000000 krypper_tgstat-0.1.8/krypper_tgstat.egg-info/top_level.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-18 13:47:27.363109 krypper_tgstat-0.1.8/setup.cfg
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1287 2024-04-18 13:44:16.000000 krypper_tgstat-0.1.8/setup.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 13:47:27.362110 krypper_tgstat-0.1.8/tests/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 07:20:55.000000 krypper_tgstat-0.1.8/tests/test_TGStatSync.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 14:05:54.241129 krypper_tgstat-0.1.8.1/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8.1/LICENSE
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 14:05:54.241129 krypper_tgstat-0.1.8.1/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-15 06:40:20.000000 krypper_tgstat-0.1.8.1/README.md
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 14:05:54.239129 krypper_tgstat-0.1.8.1/krypper_tgstat/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      244 2024-04-18 14:05:15.000000 krypper_tgstat-0.1.8.1/krypper_tgstat/__init__.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    10375 2024-04-18 13:25:29.000000 krypper_tgstat-0.1.8.1/krypper_tgstat/classes.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-18 13:20:59.000000 krypper_tgstat-0.1.8.1/krypper_tgstat/enums.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      666 2024-04-18 13:43:39.000000 krypper_tgstat-0.1.8.1/krypper_tgstat/exceptions.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     8057 2024-04-18 14:04:57.000000 krypper_tgstat-0.1.8.1/krypper_tgstat/tg_stat.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 14:05:54.241129 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      957 2024-04-18 14:05:54.000000 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-18 14:05:54.000000 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/SOURCES.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-18 14:05:54.000000 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/dependency_links.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-18 14:05:54.000000 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/requires.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-18 14:05:54.000000 krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/top_level.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-18 14:05:54.241129 krypper_tgstat-0.1.8.1/setup.cfg
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1289 2024-04-18 14:05:23.000000 krypper_tgstat-0.1.8.1/setup.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-18 14:05:54.240129 krypper_tgstat-0.1.8.1/tests/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    37040 2024-04-15 07:20:55.000000 krypper_tgstat-0.1.8.1/tests/test_TGStatSync.py
```

### Comparing `krypper_tgstat-0.1.8/LICENSE` & `krypper_tgstat-0.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.8/PKG-INFO` & `krypper_tgstat-0.1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.8/krypper_tgstat/classes.py` & `krypper_tgstat-0.1.8.1/krypper_tgstat/classes.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.8/krypper_tgstat/enums.py` & `krypper_tgstat-0.1.8.1/krypper_tgstat/enums.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.8/krypper_tgstat/exceptions.py` & `krypper_tgstat-0.1.8.1/krypper_tgstat/exceptions.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.8/krypper_tgstat/tg_stat.py` & `krypper_tgstat-0.1.8.1/krypper_tgstat/tg_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         
     def _send_request(self, method: RequestsMethods, url: str, **kwargs):
         kwargs["token"] = self.token
         response = self.session.request(method=method.value, url=url, params=kwargs)
         return response.json()
     
     
-    def _check_catgory(self, category, api_request):
+    def _check_catgory(self, api_request):
         if not type(api_request) in [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                                         CallbackRequests, UsageRequests, DatabaseRequests]:
             raise TGStatTypeError(type(api_request), [ChannelsRequests, PostsRequests, StoriesRequests, WordsRequests,
                                         CallbackRequests, UsageRequests, DatabaseRequests], api_request._name_)
         
         return True
```

### Comparing `krypper_tgstat-0.1.8/krypper_tgstat.egg-info/PKG-INFO` & `krypper_tgstat-0.1.8.1/krypper_tgstat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krypper_tgstat
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: Wrapper for TG Stat API writing on Python
 Home-page: https://github.com/KrymmyEM/krypper_tgstat
 Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krypper_tgstat-0.1.8/setup.py` & `krypper_tgstat-0.1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 :authors: Evgeny Momotov (KrymmyEM)
 :license: MIT License
 Copyright: (c) 2024 Evgeny
 """
 
-version = "0.1.8"
+version = "0.1.8.1"
 
 long_description = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
```

### Comparing `krypper_tgstat-0.1.8/tests/test_TGStatSync.py` & `krypper_tgstat-0.1.8.1/tests/test_TGStatSync.py`

 * *Files identical despite different names*

