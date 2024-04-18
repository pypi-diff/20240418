# Comparing `tmp/cassettedeck-2.2.1.tar.gz` & `tmp/cassettedeck-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassettedeck-2.2.1.tar", last modified: Fri Apr  7 19:48:03 2023, max compression
+gzip compressed data, was "dist/cassettedeck-3.0.0.tar", last modified: Thu Apr 18 11:47:19 2024, max compression
```

## Comparing `cassettedeck-2.2.1.tar` & `cassettedeck-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.519632 cassettedeck-2.2.1/
--rw-r--r--   0 ismael     (502) staff       (20)      359 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/MANIFEST.in
--rw-r--r--   0 ismael     (502) staff       (20)      633 2023-04-07 19:48:03.520080 cassettedeck-2.2.1/PKG-INFO
--rw-r--r--   0 ismael     (502) staff       (20)     3295 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/README.md
-drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.516685 cassettedeck-2.2.1/cassettedeck/
--rw-r--r--   0 ismael     (502) staff       (20)      122 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/__init__.py
--rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/cassette.py
--rw-r--r--   0 ismael     (502) staff       (20)     3708 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/deck.py
--rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/request.py
--rw-r--r--   0 ismael     (502) staff       (20)     2405 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/service.py
--rw-r--r--   0 ismael     (502) staff       (20)     5887 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/store.py
-drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.519460 cassettedeck-2.2.1/cassettedeck/tests/
--rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/__init__.py
--rw-r--r--   0 ismael     (502) staff       (20)       49 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/conftest.py
--rw-r--r--   0 ismael     (502) staff       (20)     1333 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/fixtures.py
--rw-r--r--   0 ismael     (502) staff       (20)      594 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/test_vcr.py
--rw-r--r--   0 ismael     (502) staff       (20)     5898 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/test_works.py
--rw-r--r--   0 ismael     (502) staff       (20)      593 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/vcr.py
-drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.518436 cassettedeck-2.2.1/cassettedeck.egg-info/
--rw-r--r--   0 ismael     (502) staff       (20)      633 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/PKG-INFO
--rw-r--r--   0 ismael     (502) staff       (20)      590 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/SOURCES.txt
--rw-r--r--   0 ismael     (502) staff       (20)        1 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/dependency_links.txt
--rw-r--r--   0 ismael     (502) staff       (20)       41 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/requires.txt
--rw-r--r--   0 ismael     (502) staff       (20)       13 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/top_level.txt
--rw-r--r--   0 ismael     (502) staff       (20)        1 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/zip-safe
--rw-r--r--   0 ismael     (502) staff       (20)       80 2023-04-07 19:48:03.521123 cassettedeck-2.2.1/setup.cfg
--rw-r--r--   0 ismael     (502) staff       (20)      980 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/setup.py
--rw-r--r--   0 ismael     (502) staff       (20)       58 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/test-requirements.txt
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2024-04-18 11:47:19.539110 cassettedeck-3.0.0/
+-rw-r--r--   0 ismael     (502) staff       (20)      359 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/MANIFEST.in
+-rw-r--r--   0 ismael     (502) staff       (20)      633 2024-04-18 11:47:19.539216 cassettedeck-3.0.0/PKG-INFO
+-rw-r--r--   0 ismael     (502) staff       (20)     3295 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/README.md
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2024-04-18 11:47:19.536972 cassettedeck-3.0.0/cassettedeck/
+-rw-r--r--   0 ismael     (502) staff       (20)      122 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/__init__.py
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/cassette.py
+-rw-r--r--   0 ismael     (502) staff       (20)     3708 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/deck.py
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/request.py
+-rw-r--r--   0 ismael     (502) staff       (20)     2491 2024-04-18 11:44:42.000000 cassettedeck-3.0.0/cassettedeck/service.py
+-rw-r--r--   0 ismael     (502) staff       (20)     5928 2024-04-18 11:44:42.000000 cassettedeck-3.0.0/cassettedeck/store.py
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2024-04-18 11:47:19.538852 cassettedeck-3.0.0/cassettedeck/tests/
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/tests/__init__.py
+-rw-r--r--   0 ismael     (502) staff       (20)       49 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/tests/conftest.py
+-rw-r--r--   0 ismael     (502) staff       (20)     1333 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/tests/fixtures.py
+-rw-r--r--   0 ismael     (502) staff       (20)      594 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/tests/test_vcr.py
+-rw-r--r--   0 ismael     (502) staff       (20)     5876 2024-04-18 11:44:42.000000 cassettedeck-3.0.0/cassettedeck/tests/test_works.py
+-rw-r--r--   0 ismael     (502) staff       (20)      593 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/cassettedeck/vcr.py
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2024-04-18 11:47:19.537906 cassettedeck-3.0.0/cassettedeck.egg-info/
+-rw-r--r--   0 ismael     (502) staff       (20)      633 2024-04-18 11:47:19.000000 cassettedeck-3.0.0/cassettedeck.egg-info/PKG-INFO
+-rw-r--r--   0 ismael     (502) staff       (20)      590 2024-04-18 11:47:19.000000 cassettedeck-3.0.0/cassettedeck.egg-info/SOURCES.txt
+-rw-r--r--   0 ismael     (502) staff       (20)        1 2024-04-18 11:47:19.000000 cassettedeck-3.0.0/cassettedeck.egg-info/dependency_links.txt
+-rw-r--r--   0 ismael     (502) staff       (20)       41 2024-04-18 11:47:19.000000 cassettedeck-3.0.0/cassettedeck.egg-info/requires.txt
+-rw-r--r--   0 ismael     (502) staff       (20)       13 2024-04-18 11:47:19.000000 cassettedeck-3.0.0/cassettedeck.egg-info/top_level.txt
+-rw-r--r--   0 ismael     (502) staff       (20)        1 2023-04-07 19:48:03.000000 cassettedeck-3.0.0/cassettedeck.egg-info/zip-safe
+-rw-r--r--   0 ismael     (502) staff       (20)       80 2024-04-18 11:47:19.539543 cassettedeck-3.0.0/setup.cfg
+-rw-r--r--   0 ismael     (502) staff       (20)      980 2024-04-18 11:44:42.000000 cassettedeck-3.0.0/setup.py
+-rw-r--r--   0 ismael     (502) staff       (20)       58 2023-04-07 19:47:24.000000 cassettedeck-3.0.0/test-requirements.txt
```

### Comparing `cassettedeck-2.2.1/PKG-INFO` & `cassettedeck-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassettedeck
-Version: 2.2.1
+Version: 3.0.0
 Summary: A library store and replay aiohttp requests
 Home-page: http://github.com/onna/cassettedeck
 Author: Developer team at Onna Technologies
 Author-email: dev@onna.com
 License: Public
 Description: To simplify and speed up tests that make HTTP requests
 Platform: UNKNOWN
```

### Comparing `cassettedeck-2.2.1/README.md` & `cassettedeck-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/cassettedeck/deck.py` & `cassettedeck-3.0.0/cassettedeck/deck.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/cassettedeck/service.py` & `cassettedeck-3.0.0/cassettedeck/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,28 @@
             'headers': headers
         })
         url = URL(url)
         url_parts = [p.split('?')[-1] for p in url.parts]
 
         if data is None and 'json' in kwargs:
             data = json.dumps(kwargs['json'])
+        session = Mock()
+        session._resolve_charset = Mock(return_value="utf-8")
+
         resp = ClientResponse(
             method,
             url,
             request_info=Mock(),
-            writer=Mock(),
+            writer=None,
             continue100=None,
             timer=TimerNoop(),
             traces=[],
             loop=Mock(),
-            session=Mock(),
-        )
+            session=session)
+        
         func_name = '_'.join(url_parts[-2:])
         func = None
         if hasattr(self, func_name):
             func = getattr(self, func_name)
         else:
             func_name = url_parts[-1]
             if hasattr(self, func_name):
```

### Comparing `cassettedeck-2.2.1/cassettedeck/store.py` & `cassettedeck-3.0.0/cassettedeck/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,15 @@
         # Update cache
         self._cassette_cache[cassette._path] = cassette
 
     def use_cassette(self, cassette=None):
         self._cassette = cassette
 
     def skip(self, url):
-        for ignore in self.ignore:
-            if ignore in url:
-                return True
-        return False
+        return any(ignore in url for ignore in self.ignore)
 
     async def store_response(self, method, url, params0, data0, headers0,
                              response):
         """This function is called for when we want to add a new record in the cassette
         """
         params = copy.deepcopy(params0)
         data = copy.deepcopy(data0)
@@ -156,25 +153,28 @@
             resp_json = cassette.play_response(request)
         except UnhandledHTTPRequestError:
             # Response not seen yet in cassette
             return None, False
 
         # Response was found in cassette
         cassette.play_counts = collections.Counter()
+        session = Mock()
+        session._resolve_charset = Mock(return_value="utf-8")
+        
         # Create the response
         resp = ClientResponse(
             method,
             URL(url),
             request_info=Mock(),
-            writer=Mock(),
+            writer=None,
             continue100=None,
             timer=TimerNoop(),
             traces=[],
             loop=Mock(),
-            session=Mock(),
+            session=session,
         )
         # Replicate status code and reason
         resp.status = resp_json['status']['code']
         resp.reason = resp_json['status']['message']
 
         # Set headers and content
         resp._headers = CIMultiDict(resp_json['headers'])
```

### Comparing `cassettedeck-2.2.1/cassettedeck/tests/fixtures.py` & `cassettedeck-3.0.0/cassettedeck/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/cassettedeck/tests/test_vcr.py` & `cassettedeck-3.0.0/cassettedeck/tests/test_vcr.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/cassettedeck/tests/test_works.py` & `cassettedeck-3.0.0/cassettedeck/tests/test_works.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,18 @@
     async with aiohttp.ClientSession() as sess:
         async with sess.get(url) as resp:
             return await resp.text()
 
 
 async def calling_mocked_service(path):
     url = os.path.join('http://mocked.service.com', path)
-    async with aiohttp.ClientSession() as s, s.get(url) as resp:
+    async with (aiohttp.ClientSession() as s, s.get(url) as resp):
         assert resp.status == 200
         assert resp.headers.get('Content-Type') == 'text/plain'
-        result = await resp.text()
-        return result
+        return await resp.text()
 
 
 async def download(url, data_type):
     async with aiohttp.ClientSession() as sess:
         async with sess.get(url) as resp:
             if str(resp.status).startswith('2'):
                 if data_type == 'text':
```

### Comparing `cassettedeck-2.2.1/cassettedeck/vcr.py` & `cassettedeck-3.0.0/cassettedeck/vcr.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/cassettedeck.egg-info/PKG-INFO` & `cassettedeck-3.0.0/cassettedeck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassettedeck
-Version: 2.2.1
+Version: 3.0.0
 Summary: A library store and replay aiohttp requests
 Home-page: http://github.com/onna/cassettedeck
 Author: Developer team at Onna Technologies
 Author-email: dev@onna.com
 License: Public
 Description: To simplify and speed up tests that make HTTP requests
 Platform: UNKNOWN
```

### Comparing `cassettedeck-2.2.1/cassettedeck.egg-info/SOURCES.txt` & `cassettedeck-3.0.0/cassettedeck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.1/setup.py` & `cassettedeck-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 
 setup(
     name="cassettedeck",
-    version="2.2.1",
+    version="3.0.0",
     description="A library store and replay aiohttp requests",
     long_description="To simplify and speed up tests that make HTTP requests",
     author="Developer team at Onna Technologies",
     author_email="dev@onna.com",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Development Status :: 3 - Alpha",
```

