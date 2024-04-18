# Comparing `tmp/pydantic_client-0.1.8.tar.gz` & `tmp/pydantic_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_client-0.1.8.tar", max compression
+gzip compressed data, was "pydantic_client-0.1.9.tar", max compression
```

## Comparing `pydantic_client-0.1.8.tar` & `pydantic_client-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-07-27 06:51:55.648483 pydantic_client-0.1.8/LICENSE
--rw-r--r--   0        0        0      853 2023-08-02 10:15:45.513842 pydantic_client-0.1.8/README.md
--rw-r--r--   0        0        0      272 2023-08-02 10:15:45.514567 pydantic_client-0.1.8/pydantic_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 06:12:48.636631 pydantic_client-0.1.8/pydantic_client/clients/__init__.py
--rw-r--r--   0        0        0      489 2023-08-09 10:54:27.689566 pydantic_client-0.1.8/pydantic_client/clients/abstract_client.py
--rw-r--r--   0        0        0     1041 2023-08-11 07:48:23.469171 pydantic_client-0.1.8/pydantic_client/clients/aiohttp_client.py
--rw-r--r--   0        0        0      836 2023-08-10 08:37:50.580282 pydantic_client-0.1.8/pydantic_client/clients/requests_client.py
--rw-r--r--   0        0        0      606 2023-07-28 06:12:48.637757 pydantic_client-0.1.8/pydantic_client/decorators.py
--rw-r--r--   0        0        0       78 2023-07-28 06:12:48.638209 pydantic_client-0.1.8/pydantic_client/errors.py
--rw-r--r--   0        0        0     2929 2023-08-11 07:42:10.773218 pydantic_client-0.1.8/pydantic_client/proxy.py
--rw-r--r--   0        0        0        0 2023-07-28 06:12:48.638486 pydantic_client-0.1.8/pydantic_client/schema/__init__.py
--rw-r--r--   0        0        0      192 2023-07-28 06:12:48.638876 pydantic_client-0.1.8/pydantic_client/schema/http_request.py
--rw-r--r--   0        0        0      455 2023-08-10 07:56:21.846276 pydantic_client-0.1.8/pydantic_client/schema/method_info.py
--rw-r--r--   0        0        0      622 2023-08-10 07:52:56.012981 pydantic_client-0.1.8/pydantic_client/utility.py
--rw-r--r--   0        0        0      581 2023-08-11 07:48:37.546009 pydantic_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 pydantic_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 06:51:55.648483 pydantic_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1349 2023-08-11 08:35:25.989459 pydantic_client-0.1.9/README.md
+-rw-r--r--   0        0        0      128 2023-08-11 08:30:05.235301 pydantic_client-0.1.9/pydantic_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:12:48.636631 pydantic_client-0.1.9/pydantic_client/clients/__init__.py
+-rw-r--r--   0        0        0      489 2023-08-09 10:54:27.689566 pydantic_client-0.1.9/pydantic_client/clients/abstract_client.py
+-rw-r--r--   0        0        0     1041 2023-08-11 08:23:18.674263 pydantic_client-0.1.9/pydantic_client/clients/aiohttp_client.py
+-rw-r--r--   0        0        0      836 2023-08-10 08:37:50.580282 pydantic_client-0.1.9/pydantic_client/clients/requests_client.py
+-rw-r--r--   0        0        0      606 2023-07-28 06:12:48.637757 pydantic_client-0.1.9/pydantic_client/decorators.py
+-rw-r--r--   0        0        0       78 2023-07-28 06:12:48.638209 pydantic_client-0.1.9/pydantic_client/errors.py
+-rw-r--r--   0        0        0     2929 2023-08-11 07:57:14.614901 pydantic_client-0.1.9/pydantic_client/proxy.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:12:48.638486 pydantic_client-0.1.9/pydantic_client/schema/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-28 06:12:48.638876 pydantic_client-0.1.9/pydantic_client/schema/http_request.py
+-rw-r--r--   0        0        0      455 2023-08-10 07:56:21.846276 pydantic_client-0.1.9/pydantic_client/schema/method_info.py
+-rw-r--r--   0        0        0      622 2023-08-10 07:52:56.012981 pydantic_client-0.1.9/pydantic_client/utility.py
+-rw-r--r--   0        0        0      745 2023-08-11 08:35:36.047042 pydantic_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 pydantic_client-0.1.9/PKG-INFO
```

### Comparing `pydantic_client-0.1.8/LICENSE` & `pydantic_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/README.md` & `pydantic_client-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 # pydantic-client
+[![codecov](https://codecov.io/gh/ponytailer/pydantic-client/branch/main/graph/badge.svg?token=CZX5V1YP22)](https://codecov.io/gh/ponytailer/pydantic-client)
 
 Http client base pydantic, with requests or aiohttp
 
+### How to install
+
+1. only support requests:
+
+   `pip install pydantic-client`
+2. support aiohttp and requests:
+
+   `pip install pydantic-client[aiohttp]`
+
+3. support httpx and requests:
+
+   `pip install pydantic-client[httpx]`
+
+4. support all:
+
+   `pip install pydantic-client[all]`
+
 ### How to use
 
 ```python
 
 
 
 from pydantic import BaseModel
 
-from pydantic_client import delete, get, post, put, RequestsClient
+from pydantic_client import delete, get, post, put
+from pydantic_client.clients.requests_client import RequestsClient
 
 
 class Book(BaseModel):
     name: str
     age: int
 
 
@@ -37,8 +56,8 @@
     @delete("/books/{book_id}")
     def change_book(self, book_id: int) -> Book:
         ...
 
 
 my_client = R("http://localhost/v1")
 get_book: Book = my_client.get_book(1)
-```
+```
```

### Comparing `pydantic_client-0.1.8/pydantic_client/clients/aiohttp_client.py` & `pydantic_client-0.1.9/pydantic_client/clients/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/pydantic_client/clients/requests_client.py` & `pydantic_client-0.1.9/pydantic_client/clients/requests_client.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/pydantic_client/decorators.py` & `pydantic_client-0.1.9/pydantic_client/decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/pydantic_client/proxy.py` & `pydantic_client-0.1.9/pydantic_client/proxy.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/pydantic_client/utility.py` & `pydantic_client-0.1.9/pydantic_client/utility.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.8/pyproject.toml` & `pydantic_client-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-client"
-version = "0.1.8"
+version = "0.1.9"
 description = "Http client base pydantic, with requests or aiohttp"
 authors = ["ponytailer <huangxiaohen2738@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pydantic_client" }]
 homepage = "https://github.com/ponytailer/pydantic-client"
 
 [[tool.poetry.source]]
@@ -14,12 +14,19 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 pydantic = "*"
 requests = "*"
-aiohttp = "*"
+
+aiohttp = { version = "*", optional = true }
+httpx = { version = "*", optional = true }
+
+[tool.poetry.extras]
+httpx = ["httpx"]
+aiohttp = ["aiohttp"]
+all = ["httpx", "aiohttp"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_client-0.1.8/PKG-INFO` & `pydantic_client-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,61 @@
 Metadata-Version: 2.1
 Name: pydantic-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Http client base pydantic, with requests or aiohttp
 Home-page: https://github.com/ponytailer/pydantic-client
 Author: ponytailer
 Author-email: huangxiaohen2738@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp
+Provides-Extra: aiohttp
+Provides-Extra: all
+Provides-Extra: httpx
+Requires-Dist: aiohttp ; extra == "aiohttp" or extra == "all"
+Requires-Dist: httpx ; extra == "httpx" or extra == "all"
 Requires-Dist: pydantic
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # pydantic-client
+[![codecov](https://codecov.io/gh/ponytailer/pydantic-client/branch/main/graph/badge.svg?token=CZX5V1YP22)](https://codecov.io/gh/ponytailer/pydantic-client)
 
 Http client base pydantic, with requests or aiohttp
 
+### How to install
+
+1. only support requests:
+
+   `pip install pydantic-client`
+2. support aiohttp and requests:
+
+   `pip install pydantic-client[aiohttp]`
+
+3. support httpx and requests:
+
+   `pip install pydantic-client[httpx]`
+
+4. support all:
+
+   `pip install pydantic-client[all]`
+
 ### How to use
 
 ```python
 
 
 
 from pydantic import BaseModel
 
-from pydantic_client import delete, get, post, put, RequestsClient
+from pydantic_client import delete, get, post, put
+from pydantic_client.clients.requests_client import RequestsClient
 
 
 class Book(BaseModel):
     name: str
     age: int
 
 
@@ -56,7 +79,8 @@
     def change_book(self, book_id: int) -> Book:
         ...
 
 
 my_client = R("http://localhost/v1")
 get_book: Book = my_client.get_book(1)
 ```
+
```

