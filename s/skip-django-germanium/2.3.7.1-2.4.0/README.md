# Comparing `tmp/skip-django-germanium-2.3.7.1.tar.gz` & `tmp/skip_django_germanium-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-germanium-2.3.7.1.tar", last modified: Mon Jan 30 01:28:17 2023, max compression
+gzip compressed data, was "skip_django_germanium-2.4.0.tar", last modified: Thu Apr 18 10:31:49 2024, max compression
```

## Comparing `skip-django-germanium-2.3.7.1.tar` & `skip_django_germanium-2.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.916445 skip-django-germanium-2.3.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-30 01:28:17.916445 skip-django-germanium-2.3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20406 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.912445 skip-django-germanium-2.3.7.1/germanium/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.912445 skip-django-germanium-2.3.7.1/germanium/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/django/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/django/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/sugar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.912445 skip-django-germanium-2.3.7.1/germanium/test_cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/test_cases/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.912445 skip-django-germanium-2.3.7.1/germanium/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/germanium/tools/trivials.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 01:28:17.916445 skip-django-germanium-2.3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-01-30 01:28:06.000000 skip-django-germanium-2.3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:28:17.916445 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 01:28:17.000000 skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.938346 skip_django_germanium-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-18 10:31:49.938346 skip_django_germanium-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.934346 skip_django_germanium-2.4.0/germanium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.934346 skip_django_germanium-2.4.0/germanium/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/django/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/sugar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.934346 skip_django_germanium-2.4.0/germanium/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/test_cases/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.934346 skip_django_germanium-2.4.0/germanium/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/germanium/tools/trivials.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:31:49.938346 skip_django_germanium-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 10:31:42.000000 skip_django_germanium-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:31:49.938346 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 10:31:49.000000 skip_django_germanium-2.4.0/skip_django_germanium.egg-info/top_level.txt
```

### Comparing `skip-django-germanium-2.3.7.1/LICENSE` & `skip_django_germanium-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/README.md` & `skip_django_germanium-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/config.py` & `skip_django_germanium-2.4.0/germanium/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/crawler.py` & `skip_django_germanium-2.4.0/germanium/crawler.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/decorators.py` & `skip_django_germanium-2.4.0/germanium/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/django/runner.py` & `skip_django_germanium-2.4.0/germanium/django/runner.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/django/utils.py` & `skip_django_germanium-2.4.0/germanium/django/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/patch.py` & `skip_django_germanium-2.4.0/germanium/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/storage.py` & `skip_django_germanium-2.4.0/germanium/storage.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/sugar.py` & `skip_django_germanium-2.4.0/germanium/sugar.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/auth.py` & `skip_django_germanium-2.4.0/germanium/test_cases/auth.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/client.py` & `skip_django_germanium-2.4.0/germanium/test_cases/client.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/default.py` & `skip_django_germanium-2.4.0/germanium/test_cases/default.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/migrations.py` & `skip_django_germanium-2.4.0/germanium/test_cases/migrations.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/models.py` & `skip_django_germanium-2.4.0/germanium/test_cases/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/test_cases/rest.py` & `skip_django_germanium-2.4.0/germanium/test_cases/rest.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/tools/django.py` & `skip_django_germanium-2.4.0/germanium/tools/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from contextlib import contextmanager
 
 from django.core.management import call_command
 from django.db import DEFAULT_DB_ALIAS, connections
 
 
+RUN_PRE_COMMIT = "run_pre_commit"
+RUN_ON_COMMIT = "run_on_commit"
+
+
 class CatchCallbacks:
 
     def __init__(self, connection, callback_name):
         self._connection = connection
         self._callback_name = callback_name
         self._start_count = len(self._watching_callbacks)
         self._end_count = None
@@ -24,19 +28,26 @@
 
     def end(self):
         self._end_count = len(self._watching_callbacks)
 
     def get_callbacks(self, start_count=None):
         start_count = self._start_count if start_count is None else start_count
 
-        if self._end_count == None:
+        if self._end_count is None:
             watching_callbacks = self._watching_callbacks[start_count:]
         else:
             watching_callbacks = self._watching_callbacks[start_count:self._end_count]
-        return [callbacks[-1] for callbacks in watching_callbacks]
+
+        callbacks = []
+        for watching_callback in watching_callbacks:
+            if self._callback_name == RUN_PRE_COMMIT:
+                callbacks.append(watching_callback[-1])
+            elif self._callback_name == RUN_ON_COMMIT:
+                callbacks.append(watching_callback[-2])
+        return callbacks
 
     def execute(self):
         if self._executed:
             raise RuntimeError('callback was already executed')
 
         executed_callbacks = []
         start_count = self._start_count
@@ -56,16 +67,16 @@
 
         return executed_callbacks
 
 
 class CommitCallbacks:
 
     def __init__(self, connection):
-        self.pre_commit = CatchCallbacks(connection, 'run_pre_commit')
-        self.on_commit = CatchCallbacks(connection, 'run_on_commit')
+        self.pre_commit = CatchCallbacks(connection, RUN_PRE_COMMIT)
+        self.on_commit = CatchCallbacks(connection, RUN_ON_COMMIT)
 
     def end(self):
         self.pre_commit.end()
         self.on_commit.end()
 
     def execute_pre_commit(self):
         return self.pre_commit.execute()
```

### Comparing `skip-django-germanium-2.3.7.1/germanium/tools/http.py` & `skip_django_germanium-2.4.0/germanium/tools/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from urllib.parse import urlencode
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from .trivials import assert_equal, assert_in
 
 
 def get_full_path(*paths):
-    string_paths = (force_text(path) for path in paths)
+    string_paths = (force_str(path) for path in paths)
     full_path = '/'.join((path[:-1] if path.endswith('/') else path for path in string_paths))
     return full_path if full_path.endswith('/') else full_path + '/'
 
 
 def build_url(*paths, **querystring_dict):
     return (
         '{}?{}'.format(get_full_path(*paths), urlencode(querystring_dict))
```

### Comparing `skip-django-germanium-2.3.7.1/germanium/tools/models.py` & `skip_django_germanium-2.4.0/germanium/tools/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/germanium/tools/rest.py` & `skip_django_germanium-2.4.0/germanium/tools/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from .trivials import assert_true, assert_equal, assert_in, fail
 from .http import assert_http_ok, assert_http_created
 
 
 def assert_valid_JSON(data, msg='Json is not valid'):
     """
     Given the provided ``data`` as a string, ensures that it is valid JSON &
     can be loaded properly.
     """
     try:
-        json.loads(force_text(data))
+        json.loads(force_str(data))
     except:
         fail(msg)
 
 
 def assert_valid_JSON_response(resp, msg=None):
     """
     Given a ``HttpResponse`` coming back from using the ``client``, assert that
```

### Comparing `skip-django-germanium-2.3.7.1/germanium/tools/trivials.py` & `skip_django_germanium-2.4.0/germanium/tools/trivials.py`

 * *Files identical despite different names*

### Comparing `skip-django-germanium-2.3.7.1/skip_django_germanium.egg-info/SOURCES.txt` & `skip_django_germanium-2.4.0/skip_django_germanium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

