# Comparing `tmp/aiosseclient-0.1.1.tar.gz` & `tmp/aiosseclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosseclient-0.1.1.tar", last modified: Sat Nov 18 06:50:33 2023, max compression
+gzip compressed data, was "aiosseclient-0.1.2.tar", last modified: Thu Apr 18 16:45:04 2024, max compression
```

## Comparing `aiosseclient-0.1.1.tar` & `aiosseclient-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 06:50:33.530853 aiosseclient-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       16 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-18 06:50:33.530853 aiosseclient-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 06:50:33.530853 aiosseclient-0.1.1/aiosseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-18 06:50:33.000000 aiosseclient-0.1.1/aiosseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-18 06:50:33.000000 aiosseclient-0.1.1/aiosseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 06:50:33.000000 aiosseclient-0.1.1/aiosseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-18 06:50:33.000000 aiosseclient-0.1.1/aiosseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-18 06:50:33.000000 aiosseclient-0.1.1/aiosseclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/aiosseclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-18 06:50:33.530853 aiosseclient-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      808 2023-11-18 06:50:23.000000 aiosseclient-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       16 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:45:04.011905 aiosseclient-0.1.2/aiosseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 16:45:04.000000 aiosseclient-0.1.2/aiosseclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/aiosseclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 16:45:04.015905 aiosseclient-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      808 2024-04-18 16:44:59.000000 aiosseclient-0.1.2/setup.py
```

### Comparing `aiosseclient-0.1.1/LICENSE` & `aiosseclient-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosseclient-0.1.1/PKG-INFO` & `aiosseclient-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosseclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Server Sent Event streams client.
 Home-page: https://github.com/ebraminio/aiosseclient
 Author: Ebrahim Byagowi
 Author-email: ebrahim@gnu.org
 License: Copyright (c) 2017 Ebrahim Byagowi
```

### Comparing `aiosseclient-0.1.1/README.md` & `aiosseclient-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aiosseclient-0.1.1/aiosseclient.egg-info/PKG-INFO` & `aiosseclient-0.1.2/aiosseclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosseclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Server Sent Event streams client.
 Home-page: https://github.com/ebraminio/aiosseclient
 Author: Ebrahim Byagowi
 Author-email: ebrahim@gnu.org
 License: Copyright (c) 2017 Ebrahim Byagowi
```

### Comparing `aiosseclient-0.1.1/aiosseclient.py` & `aiosseclient-0.1.2/aiosseclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,65 +83,72 @@
                 else:
                     msg.data = value
             elif name == 'event':
                 msg.event = value
             elif name == 'id':
                 msg.id = value
             elif name == 'retry':
-                msg.retry = int(value)
+                msg.retry = bool(value)
 
         return msg
 
     def __str__(self) -> str:
         return self.data
 
 
 # pylint: disable=too-many-arguments, dangerous-default-value
 async def aiosseclient(
     url: str,
     last_id: Optional[str] = None,
     valid_http_codes: List[int] = [200, 301, 307],
     exit_events: List[str] = [],
     timeout_total: Optional[float] = None,
-    headers: Optional[dict[str, str]] = {},
+    headers: Optional[dict[str, str]] = None,
 ) -> AsyncGenerator[Event, None]:
     '''Canonical API of the library'''
+    if headers is None:
+        headers = {}
     # The SSE spec requires making requests with Cache-Control: nocache
     headers['Cache-Control'] = 'no-cache'
 
     # The 'Accept' header is not required, but explicit > implicit
     headers['Accept'] = 'text/event-stream'
 
     if last_id:
         headers['Last-Event-ID'] = last_id
 
     # Override default timeout of 5 minutes
     timeout = aiohttp.ClientTimeout(total=timeout_total, connect=None,
                                     sock_connect=None, sock_read=None)
     async with aiohttp.ClientSession(timeout=timeout) as session:
+        response = None
         try:
             _LOGGER.info('Session created: %s', session)
             response = await session.get(url, headers=headers)
             if response.status not in valid_http_codes:
                 _LOGGER.error('Invalid HTTP response.status: %s', response.status)
                 await session.close()
             lines = []
             async for line in response.content:
                 line = line.decode('utf8')
 
                 if line in {'\n', '\r', '\r\n'}:
+                    if not lines:
+                        continue
                     if lines[0] == ':ok\n':
                         lines = []
                         continue
 
                     current_event = Event.parse(''.join(lines))
                     yield current_event
                     if current_event.event in exit_events:
                         await session.close()
                     lines = []
                 else:
                     lines.append(line)
         except TimeoutError as sseerr:
             _LOGGER.error('TimeoutError: %s', sseerr)
         finally:
+            if response:
+                response.close()
             if not session.closed:
                 await session.close()
```

### Comparing `aiosseclient-0.1.1/setup.py` & `aiosseclient-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf8') as f:
     readme = f.read()
 with open('LICENSE', 'r', encoding='utf8') as f:
     license_txt = f.read()
 
 setup(
     name='aiosseclient',
-    version='0.1.1',
+    version='0.1.2',
     description='Asynchronous Server Sent Event streams client.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Ebrahim Byagowi',
     author_email='ebrahim@gnu.org',
     url='https://github.com/ebraminio/aiosseclient',
     license=license_txt,
```

