# Comparing `tmp/python-ipware-2.0.3.tar.gz` & `tmp/python_ipware-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ipware-2.0.3.tar", last modified: Thu Apr 11 23:10:05 2024, max compression
+gzip compressed data, was "python_ipware-2.0.4.tar", last modified: Thu Apr 18 15:32:55 2024, max compression
```

## Comparing `python-ipware-2.0.3.tar` & `python_ipware-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 23:09:55.000000 python-ipware-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-11 23:10:05.723339 python-ipware-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-04-11 23:09:55.000000 python-ipware-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-11 23:09:55.000000 python-ipware-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/python_ipware/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/python_ipware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/python_ipware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:10:05.723339 python-ipware-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-04-11 23:09:55.000000 python-ipware-2.0.3/tests/tests_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-11 23:09:55.000000 python-ipware-2.0.3/tests/tests_ipv6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 15:32:51.000000 python_ipware-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 15:32:55.889346 python_ipware-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-04-18 15:32:51.000000 python_ipware-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 15:32:51.000000 python_ipware-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/python_ipware/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/python_ipware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/python_ipware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:32:55.889346 python_ipware-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18211 2024-04-18 15:32:51.000000 python_ipware-2.0.4/tests/tests_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-18 15:32:51.000000 python_ipware-2.0.4/tests/tests_ipv6.py
```

### Comparing `python-ipware-2.0.3/LICENSE` & `python_ipware-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ipware-2.0.3/PKG-INFO` & `python_ipware-2.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
@@ -212,31 +212,49 @@
 ### Proxy Count
 
 If your python server is behind a `known` number of proxies, but you deploy on multiple providers and don't want to track proxy IPs, you still can filter out unwanted requests by providing proxy `count`.
 
 You can customize the proxy count by providing your `proxy_count` during initialization when calling `IpWare(proxy_count=2)`.
 
 ```python
-# In the above scenario, the total number of proxies can be used as a way to filter out unwanted requests.
 from python_ipware import IpWare
 
-# enforce proxy count
-ipw = IpWare(proxy_count=1)
+# Enforce proxy count
+# proxy_count=0 is valid
+# proxy_count=None to disable proxy_count check
+ipw = IpWare(proxy_count=2)
+
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# enforce proxy count and trusted proxies
-ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>, <proxy2>
+# Exact `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
+```
 
+### Proxy Count & Trusted Proxy List Combo
+In this example, we utilize the total number of proxies as a method to filter out unwanted requests while verifying the trust proxies.
 
-# usage: non-strict mode (X-Forwarded-For: <fake>, <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are greater than the total count
-ip, trusted_route = ipw.get_client_ip(meta=request.META)
+```python
+from python_ipware import IpWare
+
+# Enforce both proxy count and trusted proxies
+ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
 
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# usage: strict mode (X-Forwarded-For: <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are exactly equal to client ip + proxy_count
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>
+# Exact `proxy_count` number of proxies
 ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
 ```
 
 In the following `example`, your public load balancer (LB) can be seen as the `only` proxy.
 
 ```
 `Real` Client <public> <-> <public> LB (Server) <private> <---> <private> Node Server
```

### Comparing `python-ipware-2.0.3/README.md` & `python_ipware-2.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -181,31 +181,49 @@
 ### Proxy Count
 
 If your python server is behind a `known` number of proxies, but you deploy on multiple providers and don't want to track proxy IPs, you still can filter out unwanted requests by providing proxy `count`.
 
 You can customize the proxy count by providing your `proxy_count` during initialization when calling `IpWare(proxy_count=2)`.
 
 ```python
-# In the above scenario, the total number of proxies can be used as a way to filter out unwanted requests.
 from python_ipware import IpWare
 
-# enforce proxy count
-ipw = IpWare(proxy_count=1)
+# Enforce proxy count
+# proxy_count=0 is valid
+# proxy_count=None to disable proxy_count check
+ipw = IpWare(proxy_count=2)
+
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# enforce proxy count and trusted proxies
-ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>, <proxy2>
+# Exact `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
+```
 
+### Proxy Count & Trusted Proxy List Combo
+In this example, we utilize the total number of proxies as a method to filter out unwanted requests while verifying the trust proxies.
 
-# usage: non-strict mode (X-Forwarded-For: <fake>, <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are greater than the total count
-ip, trusted_route = ipw.get_client_ip(meta=request.META)
+```python
+from python_ipware import IpWare
 
+# Enforce both proxy count and trusted proxies
+ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
+
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# usage: strict mode (X-Forwarded-For: <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are exactly equal to client ip + proxy_count
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>
+# Exact `proxy_count` number of proxies
 ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
 ```
 
 In the following `example`, your public load balancer (LB) can be seen as the `only` proxy.
 
 ```
 `Real` Client <public> <-> <public> LB (Server) <private> <---> <private> Node Server
```

### Comparing `python-ipware-2.0.3/pyproject.toml` & `python_ipware-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-ipware-2.0.3/python_ipware/python_ipware.py` & `python_ipware-2.0.4/python_ipware/python_ipware.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,20 +140,17 @@
 class IpWareProxy:
     """
     A class that handles proxy data from an HTTP request.
     """
 
     def __init__(
         self,
-        proxy_count: int = 0,
+        proxy_count: Optional[int] = None,
         proxy_list: Optional[List[str]] = None,
     ) -> None:
-        if proxy_count is None or proxy_count < 0:
-            raise ValueError("proxy_count must be a positive integer")
-
         self.proxy_count = proxy_count
         self.proxy_list = self._is_valid_proxy_trusted_list(proxy_list or [])
 
     def _is_valid_proxy_trusted_list(self, proxy_list: Any) -> List[str]:
         """
         Checks if the proxy list is a valid list of strings
         @return: proxy list or raises an exception
@@ -168,23 +165,22 @@
 
     def is_proxy_count_valid(
         self, ip_list: List[IpAddressType], strict: bool = False
     ) -> bool:
         """
         Checks if the proxy count is valid
         @param ip_list: list of ip addresses
-        @param strict: if True, we must have exactly proxy_count proxies
+        @param strict: if True, we must have exactly proxy_count proxies, including `0` proxies
         @return: True if the proxy count is valid, False otherwise
         """
-        if self.proxy_count < 1:
+        # No proxy count check is required
+        if self.proxy_count is None:
             return True
 
         ip_count: int = len(ip_list)
-        if ip_count < 1:
-            return False
 
         if strict:
             # our first proxy takes the last ip address and treats it as client ip
             return self.proxy_count == ip_count - 1
 
         # the client could have gone through their own proxy and included extra ips
         # client could be sending in the header: X-Forwarded-For: <fake_ip>, <client_ip>
@@ -217,35 +213,31 @@
 
         # start from the end, slice the incoming ip list to the same length as the trusted proxy list
         ip_list_slice = ip_list[-proxy_list_count:]
         for index, value in enumerate(ip_list_slice):
             if not str(value).startswith(self.proxy_list[index]):
                 return False
 
-        # now all we need is to return the first ip in the list that is not in the trusted proxy list
-        # best_client_ip_index = proxy_list_count + 1
-        # best_client_ip = ip_list[-best_client_ip_index]
-
         return True
 
 
 class IpWare(IpWareMeta, IpWareProxy, IpWareIpAddress):
     """
     A class that makes best effort to determine the client's IP address.
     """
 
     def __init__(
         self,
         precedence: Optional[Tuple[str, ...]] = None,
         leftmost: bool = True,
-        proxy_count: int = 0,
+        proxy_count: Optional[int] = None,
         proxy_list: Optional[List[str]] = None,
     ) -> None:
         IpWareMeta.__init__(self, precedence, leftmost)
-        IpWareProxy.__init__(self, proxy_count or 0, proxy_list or [])
+        IpWareProxy.__init__(self, proxy_count, proxy_list)
 
     def get_meta_value(self, meta: Dict[str, str], key: str) -> str:
         """
         Given a key, it returns a cleaned up version of the value
         @param key: the key to lookup
         @return: the value of the key or empty string
         """
@@ -253,31 +245,35 @@
         return meta.get(key, meta.get(key.replace("_", "-"), "")).strip()
 
     def get_meta_values(self, meta: Dict[str, str]) -> List[str]:
         """
         Given a list of keys, it returns a list of cleaned up values
         @return: a list of values
         """
-        return [self.get_meta_value(meta, key) for key in self.precedence]
+        meta_list: List[str] = []
+        for key in self.precedence:
+            value = self.get_meta_value(meta, key).strip()
+            if value:
+                meta_list.append(value)
+
+        return meta_list
 
     def get_client_ip(
         self,
         meta: Dict[str, str],
         strict: bool = False,
     ) -> Tuple[OptionalIpAddressType, bool]:
         """
         Returns the client's IP address.
         """
 
         loopback_list: List[IpAddressType] = []
         private_list: List[OptionalIpAddressType] = []
 
         for ip_str in self.get_meta_values(meta):
-            if not ip_str:
-                continue
 
             ip_list = self.get_ips_from_string(ip_str)
             if not ip_list:
                 continue
 
             proxy_count_validated = self.is_proxy_count_valid(ip_list, strict)
             if not proxy_count_validated:
@@ -333,14 +329,18 @@
         # the incoming ips match our trusted proxy list
         if len(self.proxy_list) > 0 and proxy_list_validated:
             best_client_ip_index = len(self.proxy_list) + 1
             best_client_ip = ip_list[-best_client_ip_index]
             return best_client_ip, True
 
         # the incoming ips match our proxy count
-        if self.proxy_count > 0 and proxy_count_validated:
+        if (
+            self.proxy_count is not None
+            and self.proxy_count > 0
+            and proxy_count_validated
+        ):
             best_client_ip_index = self.proxy_count + 1
             best_client_ip = ip_list[-best_client_ip_index]
             return best_client_ip, True
 
         # we don't track proxy related info, so we just return the first ip
         return ip_list[0], False
```

### Comparing `python-ipware-2.0.3/python_ipware.egg-info/PKG-INFO` & `python_ipware-2.0.4/python_ipware.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
@@ -212,31 +212,49 @@
 ### Proxy Count
 
 If your python server is behind a `known` number of proxies, but you deploy on multiple providers and don't want to track proxy IPs, you still can filter out unwanted requests by providing proxy `count`.
 
 You can customize the proxy count by providing your `proxy_count` during initialization when calling `IpWare(proxy_count=2)`.
 
 ```python
-# In the above scenario, the total number of proxies can be used as a way to filter out unwanted requests.
 from python_ipware import IpWare
 
-# enforce proxy count
-ipw = IpWare(proxy_count=1)
+# Enforce proxy count
+# proxy_count=0 is valid
+# proxy_count=None to disable proxy_count check
+ipw = IpWare(proxy_count=2)
+
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# enforce proxy count and trusted proxies
-ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>, <proxy2>
+# Exact `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
+```
 
+### Proxy Count & Trusted Proxy List Combo
+In this example, we utilize the total number of proxies as a method to filter out unwanted requests while verifying the trust proxies.
 
-# usage: non-strict mode (X-Forwarded-For: <fake>, <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are greater than the total count
-ip, trusted_route = ipw.get_client_ip(meta=request.META)
+```python
+from python_ipware import IpWare
+
+# Enforce both proxy count and trusted proxies
+ipw = IpWare(proxy_count=1, proxy_list=["198.84.193.157"])
 
+# Example usage in non-strict mode:
+# X-Forwarded-For format: <fake>, <client>, <proxy1>, <proxy2>
+# At least `proxy_count` number of proxies
+ip, trusted_route = ipw.get_client_ip(meta=request.META)
 
-# usage: strict mode (X-Forwarded-For: <client>, <proxy1>, <proxy2>)
-# total number of ip addresses are exactly equal to client ip + proxy_count
+# Example usage in strict mode:
+# X-Forwarded-For format: <client>, <proxy1>
+# Exact `proxy_count` number of proxies
 ip, trusted_route = ipw.get_client_ip(meta=request.META, strict=True)
 ```
 
 In the following `example`, your public load balancer (LB) can be seen as the `only` proxy.
 
 ```
 `Real` Client <public> <-> <public> LB (Server) <private> <---> <private> Node Server
```

### Comparing `python-ipware-2.0.3/tests/tests_ipv4.py` & `python_ipware-2.0.4/tests/tests_ipv4.py`

 * *Files 19% similar despite different names*

```diff
@@ -171,47 +171,77 @@
         r = ipware.get_client_ip(meta)
         self.assertEqual(r, (IPv4Address("198.84.193.158"), False))
 
 
 class TestIPv4ProxyCount(unittest.TestCase):
     """IPv4 Proxy Count Test"""
 
-    def setUp(self):
-        self.ipware = IpWare(proxy_count=1)
-
-    def tearDown(self):
-        self.ipware = None
-
-    def test_singleton_proxy_count(self):
+    def test_proxy_count_one_missing_proxy_fail(self):
+        ipware = IpWare(proxy_count=1)
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139",
         }
-        r = self.ipware.get_client_ip(meta)
+        r = ipware.get_client_ip(meta)
+
         self.assertEqual(r, (None, False))
 
-    def test_singleton_proxy_count_private(self):
+    def test_proxy_count_one_at_least_one_proxy_pass(self):
+        ipware = IpWare(proxy_count=1)
         meta = {
-            "HTTP_X_FORWARDED_FOR": "10.0.0.0",
-            "HTTP_X_REAL_IP": "177.139.233.139",
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
-        r = self.ipware.get_client_ip(meta)
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("198.84.193.157"), True))
+
+    def test_proxy_count_one_exactly_one_proxy_fail(self):
+        ipware = IpWare(proxy_count=1)
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta, strict=True)
         self.assertEqual(r, (None, False))
 
-    def test_proxy_count_relax(self):
+    def test_proxy_count_one_exactly_one_proxy_pass(self):
+        ipware = IpWare(proxy_count=1)
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157",
+        }
+        r = ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
+
+    def test_proxy_count_one_dont_care_proxy_pass(self):
+        ipware = IpWare()
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
-        r = self.ipware.get_client_ip(meta, strict=False)
-        self.assertEqual(r, (IPv4Address("198.84.193.157"), True))
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
 
-    def test_proxy_count_strict(self):
+    def test_proxy_count_zero_dont_care_proxy_pass(self):
+        ipware = IpWare(proxy_count=0)
         meta = {
-            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.158",
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
-        r = self.ipware.get_client_ip(meta, strict=True)
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
+
+    def test_proxy_count_zero_exact_zero_proxy_pass(self):
+        ipware = IpWare(proxy_count=0)
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139",
+        }
+        r = ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
+
+    def test_proxy_count_zero_exact_zero_proxy_fail(self):
+        ipware = IpWare(proxy_count=0)
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta, strict=True)
         self.assertEqual(r, (None, False))
 
 
 class TestIPv4ProxyList(unittest.TestCase):
     """IPv4 Proxy List Test"""
 
     def setUp(self):
@@ -241,34 +271,76 @@
         r = self.ipware.get_client_ip(meta)
         self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
 
 
 class TestIPv4ProxyCountProxyList(unittest.TestCase):
     """IPv4 Proxy Count Test"""
 
-    def setUp(self):
-        self.ipware = IpWare(
-            proxy_count=2, proxy_list=["198.84.193.157", "198.84.193.158"]
-        )
+    def test_proxy_list_relax(self):
+        ipware = IpWare(proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
 
-    def tearDown(self):
-        self.ipware = None
+    def test_proxy_list_strict_pass(self):
+        ipware = IpWare(proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
 
-    def test_proxy_list_relax(self):
+    def test_proxy_list_strict_fail(self):
+        ipware = IpWare(proxy_list=["198.84.193.157", "198.84.193.158"])
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
-        r = self.ipware.get_client_ip(meta)
+        r = ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (None, False))
+
+    def test_proxy_list_relax_exact_pass(self):
+        ipware = IpWare(proxy_count=2, proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta)
         self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
 
-    def test_proxy_list_strict(self):
+    def test_proxy_list_relax_count_under_pass(self):
+        ipware = IpWare(proxy_count=1, proxy_list=["198.84.193.157", "198.84.193.158"])
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
-        r = self.ipware.get_client_ip(meta, strict=True)
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
+
+    def test_proxy_list_relax_count_over_pass(self):
+        ipware = IpWare(proxy_count=5, proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (None, False))
+
+    def test_proxy_list_count_exact_pass(self):
+        ipware = IpWare(proxy_count=2, proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
+
+    def test_proxy_list_count_exact_fail(self):
+        ipware = IpWare(proxy_count=4, proxy_list=["198.84.193.157", "198.84.193.158"])
+        meta = {
+            "HTTP_X_FORWARDED_FOR": "177.139.233.138, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = ipware.get_client_ip(meta)
         self.assertEqual(r, (None, False))
 
 
 class TestIPv4Port(unittest.TestCase):
     """IPv4 Port - IP address Test"""
 
     def setUp(self):
```

### Comparing `python-ipware-2.0.3/tests/tests_ipv6.py` & `python_ipware-2.0.4/tests/tests_ipv6.py`

 * *Files identical despite different names*

