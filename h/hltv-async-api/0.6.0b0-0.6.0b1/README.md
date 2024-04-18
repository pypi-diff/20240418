# Comparing `tmp/hltv_async_api-0.6.0b0.tar.gz` & `tmp/hltv_async_api-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.6.0b0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.6.0b1.tar", max compression
```

## Comparing `hltv_async_api-0.6.0b0.tar` & `hltv_async_api-0.6.0b1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      125 2024-04-17 22:38:57.763245 hltv_async_api-0.6.0b0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    38144 2024-04-17 22:38:34.849213 hltv_async_api-0.6.0b0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.0b0/LICENSE
--rw-r--r--   0        0        0      649 2024-04-17 22:38:57.771204 hltv_async_api-0.6.0b0/pyproject.toml
--rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.6.0b0/README.md
--rw-r--r--   0        0        0    15816 1970-01-01 00:00:00.000000 hltv_async_api-0.6.0b0/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-18 13:03:32.828125 hltv_async_api-0.6.0b1/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    38315 2024-04-18 12:36:50.601884 hltv_async_api-0.6.0b1/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.0b1/LICENSE
+-rw-r--r--   0        0        0      650 2024-04-18 13:03:32.841238 hltv_async_api-0.6.0b1/pyproject.toml
+-rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.6.0b1/README.md
+-rw-r--r--   0        0        0    15816 1970-01-01 00:00:00.000000 hltv_async_api-0.6.0b1/PKG-INFO
```

### Comparing `hltv_async_api-0.6.0b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.6.0b1/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from typing import Any, List
 from datetime import date, datetime, timedelta
 import pytz
 
 from bs4 import BeautifulSoup
 import asyncio
 from asyncio import get_running_loop
@@ -14,45 +15,49 @@
 
 import logging
 
 
 class Hltv:
     def __init__(self, max_delay: int = 15,
                  timeout: int = 5,
-                 use_proxy: bool = False,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
                  debug: bool = False,
                  max_retries: int = 0,
                  proxy_protocol: str | None = None,
                  proxy_one_time: bool = False,
-                 true_session: bool = False,
+                 one_time_session: bool = True,
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "UTC"
         }
         self.MAX_DELAY = max_delay
         self.timeout = timeout
         self.max_retries = max_retries
-        self.USE_PROXY = use_proxy
         self.PROXY_PATH = proxy_path
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
         self.PROXY_ONCE = proxy_one_time
+        self.ONE_TIME_SESSION = one_time_session
+        self.session = None
         self.DEBUG = debug
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
-        self.TRUE_SESSION = true_session
+        if proxy_path or proxy_list:
+            self.USE_PROXY = True
+        else:
+            self.USE_PROXY = False
+
         self._create_session()
 
     def _configure_logging(self):
         level = logging.DEBUG if self.DEBUG else logging.INFO
         logging.basicConfig(level=level, format="%(message)s")
 
     def _create_session(self):
@@ -71,15 +76,15 @@
                use_proxy: bool | None = None,
                proxy_file_path: str | None = None,
                proxy_list: list | None = None,
                debug: bool | None = None,
                max_retries: int | None = None,
                proxy_protocol: str | None = None,
                proxy_one_time: bool | None = None,
-               true_session: bool | None = None,
+               one_time_session: bool | None = None,
                ):
         if max_delay:
             self.MAX_DELAY = max_delay
         if timeout:
             self.timeout = timeout
         if use_proxy is not None:
             self.USE_PROXY = use_proxy
@@ -87,16 +92,16 @@
             self.PROXY_LIST = proxy_list
         if max_retries:
             self.max_retries = max_retries
         if proxy_protocol:
             self.PROXY_PROTOCOL = proxy_protocol
         if proxy_one_time is not None:
             self.PROXY_ONCE = proxy_one_time
-        if true_session is not None:
-            self.TRUE_SESSION = true_session
+        if one_time_session is not None:
+            self.ONE_TIME_SESSION = one_time_session
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
@@ -164,17 +169,20 @@
 
                 return True, result
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
             self.logger.debug(e)
             delay = self._parse_error_handler(delay)
             return False, delay
+        except ClientTimeout:
+            return False, delay
 
     async def _fetch(self, url, delay: int = 0):
-
+        if not self.session:
+            self._create_session()
         status = False
         try_ = 1
         result = None
 
         # parse until success or not maxretries
         while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
@@ -183,14 +191,16 @@
             # if status = False, result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
+        if not self.ONE_TIME_SESSION:
+            await self.close_session()
         if status:
             loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
             return None
@@ -936,17 +946,13 @@
 
             if only_today:
                 break
 
         return news
 
 
-async def test():
-    hltv = Hltv(debug=True, timeout=1, max_delay=5, use_proxy=True, proxy_path='proxies.txt',
-                proxy_protocol='http')
+async def main():
+    hltv = Hltv()
     print(await hltv.get_matches())
 
-    await hltv.close_session()
-
-
-if __name__ == "__main__":
-    asyncio.run(test())
+if __name__ == '__main__':
+    asyncio.run(main())
```

### Comparing `hltv_async_api-0.6.0b0/LICENSE` & `hltv_async_api-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.0b0/pyproject.toml` & `hltv_async_api-0.6.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.6.0b"
+version = "0.6.0b1"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.6.0b0/README.md` & `hltv_async_api-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.6.0b0/PKG-INFO` & `hltv_async_api-0.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.6.0b0
+Version: 0.6.0b1
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

