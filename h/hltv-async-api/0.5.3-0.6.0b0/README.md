# Comparing `tmp/hltv_async_api-0.5.3.tar.gz` & `tmp/hltv_async_api-0.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.5.3.tar", max compression
+gzip compressed data, was "hltv_async_api-0.6.0b0.tar", max compression
```

## Comparing `hltv_async_api-0.5.3.tar` & `hltv_async_api-0.6.0b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      124 2024-04-17 22:10:26.232259 hltv_async_api-0.5.3/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    38403 2024-04-17 22:10:04.481202 hltv_async_api-0.5.3/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.5.3/LICENSE
--rw-r--r--   0        0        0      648 2024-04-17 22:10:26.247497 hltv_async_api-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.5.3/README.md
--rw-r--r--   0        0        0    15814 1970-01-01 00:00:00.000000 hltv_async_api-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-17 22:38:57.763245 hltv_async_api-0.6.0b0/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    38144 2024-04-17 22:38:34.849213 hltv_async_api-0.6.0b0/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.6.0b0/LICENSE
+-rw-r--r--   0        0        0      649 2024-04-17 22:38:57.771204 hltv_async_api-0.6.0b0/pyproject.toml
+-rw-r--r--   0        0        0    15288 2024-04-15 21:37:37.703676 hltv_async_api-0.6.0b0/README.md
+-rw-r--r--   0        0        0    15816 1970-01-01 00:00:00.000000 hltv_async_api-0.6.0b0/PKG-INFO
```

### Comparing `hltv_async_api-0.5.3/hltv_async_api/aiohltv.py` & `hltv_async_api-0.6.0b0/hltv_async_api/aiohltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,23 +45,24 @@
         self.logger = logging.getLogger(__name__)
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
         self.TRUE_SESSION = true_session
-        self.session = None
+        self._create_session()
 
     def _configure_logging(self):
         level = logging.DEBUG if self.DEBUG else logging.INFO
         logging.basicConfig(level=level, format="%(message)s")
 
-    async def _create_session(self):
-        self.logger.debug('Creating Session')
-        self.session = ClientSession()
+    def _create_session(self):
+        if not self.session:
+            self.logger.debug('Creating Session')
+            self.session = ClientSession()
 
     async def close_session(self):
         if self.session:
             self.logger.debug('Closing Session')
             await self.session.close()
             self.session = None
 
@@ -95,23 +96,23 @@
         if debug is not None:
             self.DEBUG = debug
             self._configure_logging()
         if proxy_file_path:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
-    async def _get_proxy(self):
+    def _get_proxy(self):
         proxy = self.PROXY_LIST[0]
 
         if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
             proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
 
-    async def _switch_proxy(self):
+    def _switch_proxy(self):
         if self.PROXY_ONCE:
             self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
             self.PROXY_LIST = self.PROXY_LIST[1:]
         else:
             self.logger.debug(f"Switching proxy {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
             self.PROXY_LIST = self.PROXY_LIST[1:] + [(self.PROXY_LIST[0])]
             self.logger.info(f"New proxy: {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
@@ -125,56 +126,54 @@
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
             if "Enable JavaScript and cookies to continue" in challenge_page.get_text():
                 self.logger.debug("Got cloudflare challenge page")
                 return True
         return False
 
-    async def _parse_error_handler(self, delay: int = 0) -> int:
+    def _parse_error_handler(self, delay: int = 0) -> int:
         if self.USE_PROXY:
-            await self._switch_proxy()
+            self._switch_proxy()
         else:
             if delay < self.MAX_DELAY:
                 delay += 1
             else:
                 self.logger.debug("Reached max delay limit, try to use proxy")
             self.logger.info(f"Calling again, increasing delay to {delay}s")
 
         return delay
 
     async def _parse(self, url, delay):
         proxy = ''
         # setup new proxy, cuz old one was switched
         if self.USE_PROXY:
-            proxy = await self._get_proxy()
+            proxy = self._get_proxy()
         else:
             # delay, only for non proxy users. (default = 1-15s)
             await asyncio.sleep(delay)
         try:
             async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout, ) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 403 or response.status == 404:
                     self.logger.debug("Got 403 forbitten")
-                    return False, await self._parse_error_handler(delay)
+                    return False, self._parse_error_handler(delay)
 
                 # checking for challenge page.
                 result = await response.text()
                 if await self._cloudflare_check(result):
-                    return False, await self._parse_error_handler(delay)
+                    return False, self._parse_error_handler(delay)
 
                 return True, result
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
             self.logger.debug(e)
-            delay = await self._parse_error_handler(delay)
+            delay = self._parse_error_handler(delay)
             return False, delay
 
     async def _fetch(self, url, delay: int = 0):
-        if not self.session:
-            await self._create_session()
 
         status = False
         try_ = 1
         result = None
 
         # parse until success or not maxretries
         while (not status) and (try_ != self.max_retries):
@@ -184,19 +183,14 @@
             # if status = False, result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
-        # After Parse
-        if not self.TRUE_SESSION:
-            # Automatically close session after parse
-            await self.close_session()
-
         if status:
             loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
             return None
@@ -943,15 +937,15 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv(debug=True, timeout=1, max_delay=5, true_session=True, use_proxy=True, proxy_path='proxies.txt',
+    hltv = Hltv(debug=True, timeout=1, max_delay=5, use_proxy=True, proxy_path='proxies.txt',
                 proxy_protocol='http')
     print(await hltv.get_matches())
 
     await hltv.close_session()
 
 
 if __name__ == "__main__":
```

### Comparing `hltv_async_api-0.5.3/LICENSE` & `hltv_async_api-0.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.3/pyproject.toml` & `hltv_async_api-0.6.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.5.3"
+version = "0.6.0b"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.5.3/README.md` & `hltv_async_api-0.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.5.3/PKG-INFO` & `hltv_async_api-0.6.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.5.3
+Version: 0.6.0b0
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

