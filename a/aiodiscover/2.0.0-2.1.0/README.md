# Comparing `tmp/aiodiscover-2.0.0.tar.gz` & `tmp/aiodiscover-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiscover-2.0.0.tar", last modified: Wed Mar 13 22:50:53 2024, max compression
+gzip compressed data, was "aiodiscover-2.1.0.tar", last modified: Thu Apr 18 21:05:25 2024, max compression
```

## Comparing `aiodiscover-2.0.0.tar` & `aiodiscover-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/aiodiscover/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/aiodiscover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/aiodiscover/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/aiodiscover/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/aiodiscover/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/aiodiscover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-13 22:50:53.000000 aiodiscover-2.0.0/aiodiscover.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-13 22:50:53.309108 aiodiscover-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-13 22:50:48.000000 aiodiscover-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/aiodiscover/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/aiodiscover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/aiodiscover/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/aiodiscover/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/aiodiscover/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/aiodiscover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:05:25.000000 aiodiscover-2.1.0/aiodiscover.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-18 21:05:25.730413 aiodiscover-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-18 21:05:21.000000 aiodiscover-2.1.0/setup.py
```

### Comparing `aiodiscover-2.0.0/CONTRIBUTING.md` & `aiodiscover-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/LICENSE` & `aiodiscover-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/PKG-INFO` & `aiodiscover-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiscover
-Version: 2.0.0
+Version: 2.1.0
 Summary: Discover hosts by arp and ptr lookup
 Home-page: https://github.com/bdraco/aiodiscover
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: aiodiscover
 Platform: UNKNOWN
```

### Comparing `aiodiscover-2.0.0/README.md` & `aiodiscover-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/aiodiscover/discovery.py` & `aiodiscover-2.1.0/aiodiscover/discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from contextlib import suppress
+from functools import lru_cache, partial
 from ipaddress import IPv4Address
-from typing import TYPE_CHECKING, Any
-from functools import lru_cache
+from itertools import islice
+from typing import TYPE_CHECKING, Any, Iterable, cast
+
 from aiodns import DNSResolver
 
 from .network import SystemNetworkData
 
 if TYPE_CHECKING:
     from pyroute2.iproute import IPRoute  # noqa: F401
 
 HOSTNAME = "hostname"
 MAC_ADDRESS = "macaddress"
 IP_ADDRESS = "ip"
 MAX_ADDRESSES = 2048
+QUERY_BUCKET_SIZE = 64
 
 DNS_RESPONSE_TIMEOUT = 2
 
+
 _LOGGER = logging.getLogger(__name__)
 
 
 @lru_cache(maxsize=MAX_ADDRESSES)
 def decode_idna(name: str) -> str:
     """Decode an idna name."""
     try:
@@ -43,21 +47,43 @@
 
 
 async def async_query_for_ptrs(
     nameserver: str, ips_to_lookup: list[IPv4Address]
 ) -> list[Any | None]:
     """Fetch PTR records for a list of ips."""
     resolver = DNSResolver(nameservers=[nameserver], timeout=DNS_RESPONSE_TIMEOUT)
-    futures = [resolver.query(ip.reverse_pointer, "PTR") for ip in ips_to_lookup]
-    await asyncio.wait(futures)
-    results = [None if future.exception() else future.result() for future in futures]
+    results: list[Any | None] = []
+    for ip_chunk in chunked(ips_to_lookup, QUERY_BUCKET_SIZE):
+        if TYPE_CHECKING:
+            ip_chunk = cast("list[IPv4Address]", ip_chunk)
+        futures = [resolver.query(ip.reverse_pointer, "PTR") for ip in ip_chunk]
+        await asyncio.wait(futures)
+        results.extend(
+            None if future.exception() else future.result() for future in futures
+        )
     resolver.cancel()
     return results
 
 
+def take(take_num: int, iterable: Iterable) -> list[Any]:
+    """Return first n items of the iterable as a list.
+
+    From itertools recipes
+    """
+    return list(islice(iterable, take_num))
+
+
+def chunked(iterable: Iterable, chunked_num: int) -> Iterable[Any]:
+    """Break *iterable* into lists of length *n*.
+
+    From more-itertools
+    """
+    return iter(partial(take, chunked_num, iter(iterable)), [])
+
+
 class DiscoverHosts:
     """Discover hosts on the network by ARP and PTR lookup."""
 
     def __init__(self) -> None:
         """Init the discovery hosts."""
         self._sys_network_data: SystemNetworkData | None = None
```

### Comparing `aiodiscover-2.0.0/aiodiscover/network.py` & `aiodiscover-2.1.0/aiodiscover/network.py`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/aiodiscover.egg-info/PKG-INFO` & `aiodiscover-2.1.0/aiodiscover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiscover
-Version: 2.0.0
+Version: 2.1.0
 Summary: Discover hosts by arp and ptr lookup
 Home-page: https://github.com/bdraco/aiodiscover
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: aiodiscover
 Platform: UNKNOWN
```

### Comparing `aiodiscover-2.0.0/aiodiscover.egg-info/requires.txt` & `aiodiscover-2.1.0/aiodiscover.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/docs/Makefile` & `aiodiscover-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/docs/conf.py` & `aiodiscover-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/docs/installation.rst` & `aiodiscover-2.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/docs/make.bat` & `aiodiscover-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiscover-2.0.0/setup.py` & `aiodiscover-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,10 +81,10 @@
     setup_requires=setup_requirements,
     test_suite="aiodiscover/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/bdraco/aiodiscover",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="2.0.0",
+    version="2.1.0",
     zip_safe=False,
 )
```

