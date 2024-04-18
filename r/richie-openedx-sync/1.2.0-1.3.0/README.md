# Comparing `tmp/richie-openedx-sync-1.2.0.tar.gz` & `tmp/richie_openedx_sync-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richie-openedx-sync-1.2.0.tar", last modified: Thu Aug 25 08:28:17 2022, max compression
+gzip compressed data, was "richie_openedx_sync-1.3.0.tar", last modified: Thu Apr 18 13:47:52 2024, max compression
```

## Comparing `richie-openedx-sync-1.2.0.tar` & `richie_openedx_sync-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)    34523 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      107 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2510 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1823 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:17.969406 richie-openedx-sync-1.2.0/richie_openedx_sync/
--rw-r--r--   0 runner    (1001) docker     (116)      201 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/richie_openedx_sync/management/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/richie_openedx_sync/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2990 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py
--rw-r--r--   0 runner    (1001) docker     (116)      884 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1889 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/signals.py
--rw-r--r--   0 runner    (1001) docker     (116)     4694 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/richie_openedx_sync/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2510 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      653 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      175 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       46 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2022-08-25 08:28:17.000000 richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-08-25 08:28:17.973406 richie-openedx-sync-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3333 2022-08-25 08:28:05.000000 richie-openedx-sync-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.969602 richie_openedx_sync-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/richie_openedx_sync/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:47:52.965602 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 13:47:52.000000 richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:47:52.969602 richie_openedx_sync-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-18 13:47:49.000000 richie_openedx_sync-1.3.0/setup.py
```

### Comparing `richie-openedx-sync-1.2.0/LICENSE` & `richie_openedx_sync-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/PKG-INFO` & `richie_openedx_sync-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richie-openedx-sync
-Version: 1.2.0
+Version: 1.3.0
 Summary: Richie Open edX Synchronization application
 Home-page: https://github.com/fccn/richie-openedx-sync
 Author: FCT|FCCN NAU
 Author-email: info@nau.edu.pt
 License: AGPL 3.0
 Keywords: Django,Open edX,MOOC,Richie
 Platform: any
@@ -13,14 +13,18 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: edx-celeryutils
+Requires-Dist: requests
+Requires-Dist: celery
+Requires-Dist: django-celery
 
 # Richie Open edX Synchronization application
 
 ## Overview
 
 The aim of this Django application is to synchronize the Open edX courses to the Richie marketing site.
 Whenever a course schedule or details are updated on Studio a hook is run that sends the updated information to Richie.
```

### Comparing `richie-openedx-sync-1.2.0/README.md` & `richie_openedx_sync-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync/apps.py` & `richie_openedx_sync-1.3.0/richie_openedx_sync/apps.py`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py` & `richie_openedx_sync-1.3.0/richie_openedx_sync/management/commands/sync_courses_to_richie.py`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync/settings.py` & `richie_openedx_sync-1.3.0/richie_openedx_sync/settings.py`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync/signals.py` & `richie_openedx_sync-1.3.0/richie_openedx_sync/signals.py`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync/tasks.py` & `richie_openedx_sync-1.3.0/richie_openedx_sync/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         signature = hmac.new(
             hook["secret"].encode("utf-8"),
             msg=json.dumps(data).encode("utf-8"),
             digestmod=hashlib.sha256,
         ).hexdigest()
 
         richie_url = hook.get("url")
-        timeout = int(hook.get("timeout", 5))
+        timeout = int(hook.get("timeout", 20))
 
         try:
             response = requests.post(
                 richie_url,
                 json=data,
                 headers={
                     "Authorization": "SIG-HMAC-SHA256 {:s}".format(signature)},
@@ -115,21 +115,21 @@
                 log.info(msg)
                 log.info(response.content)
         except requests.exceptions.HTTPError as e:
             status_code = response.status_code
             msg = "Error synchronizing course {} to richie site {} it returned the HTTP status code {}".format(
                 course_key, richie_url, status_code
             )
-            log.error(e, exc_info=True)
-            log.error(msg)
-            log.error(response.content)
+            log.warning(e, exc_info=True)
+            log.warning(msg)
+            log.warning(response.content)
             result[richie_url] = False
 
         except requests.exceptions.RequestException as e:
             msg = "Error synchronizing course {} to richie site {}".format(
                 course_key, richie_url
             )
-            log.error(e, exc_info=True)
-            log.error(msg)
+            log.warning(e, exc_info=True)
+            log.warning(msg)
             result[richie_url] = False
 
     return result
```

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/PKG-INFO` & `richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richie-openedx-sync
-Version: 1.2.0
+Version: 1.3.0
 Summary: Richie Open edX Synchronization application
 Home-page: https://github.com/fccn/richie-openedx-sync
 Author: FCT|FCCN NAU
 Author-email: info@nau.edu.pt
 License: AGPL 3.0
 Keywords: Django,Open edX,MOOC,Richie
 Platform: any
@@ -13,14 +13,18 @@
 Classifier: Framework :: Django :: 2.2
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: edx-celeryutils
+Requires-Dist: requests
+Requires-Dist: celery
+Requires-Dist: django-celery
 
 # Richie Open edX Synchronization application
 
 ## Overview
 
 The aim of this Django application is to synchronize the Open edX courses to the Richie marketing site.
 Whenever a course schedule or details are updated on Studio a hook is run that sends the updated information to Richie.
```

### Comparing `richie-openedx-sync-1.2.0/richie_openedx_sync.egg-info/SOURCES.txt` & `richie_openedx_sync-1.3.0/richie_openedx_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `richie-openedx-sync-1.2.0/setup.py` & `richie_openedx_sync-1.3.0/setup.py`

 * *Files identical despite different names*

