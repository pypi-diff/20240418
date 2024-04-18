# Comparing `tmp/autoutils-0.9.0.tar.gz` & `tmp/autoutils-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils-0.9.0.tar", max compression
+gzip compressed data, was "autoutils-0.9.1.tar", max compression
```

## Comparing `autoutils-0.9.0.tar` & `autoutils-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1067 2023-07-25 01:56:35.774830 autoutils-0.9.0/LICENSE
--rw-r--r--   0        0        0       11 2023-07-25 01:56:35.774830 autoutils-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/__init__.py
--rw-r--r--   0        0        0     3014 2024-02-05 10:16:29.597483 autoutils-0.9.0/autoutils/api.py
--rw-r--r--   0        0        0     8739 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/color.py
--rw-r--r--   0        0        0     3411 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/file.py
--rw-r--r--   0        0        0    20748 2023-11-13 09:24:49.207147 autoutils-0.9.0/autoutils/log.py
--rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/matrixcli/__init__.py
--rw-r--r--   0        0        0    35272 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/matrixcli/api.py
--rw-r--r--   0        0        0     7437 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/matrixcli/client.py
--rw-r--r--   0        0        0     1765 2023-07-25 01:56:35.774830 autoutils-0.9.0/autoutils/matrixcli/errors.py
--rw-r--r--   0        0        0    24836 2023-07-25 01:56:35.778830 autoutils-0.9.0/autoutils/matrixcli/room.py
--rw-r--r--   0        0        0     1509 2023-07-25 01:56:35.778830 autoutils-0.9.0/autoutils/matrixcli/user.py
--rw-r--r--   0        0        0     3253 2023-07-25 01:56:35.778830 autoutils-0.9.0/autoutils/redis.py
--rw-r--r--   0        0        0     4243 2023-07-25 01:56:35.778830 autoutils-0.9.0/autoutils/script.py
--rw-r--r--   0        0        0    12052 2023-11-25 06:17:00.273785 autoutils-0.9.0/autoutils/server.py
--rw-r--r--   0        0        0     6437 2023-07-25 01:56:35.778830 autoutils-0.9.0/autoutils/thread.py
--rw-r--r--   0        0        0      808 2024-02-05 10:16:29.613484 autoutils-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 autoutils-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 01:56:35.774830 autoutils-0.9.1/LICENSE
+-rw-r--r--   0        0        0       11 2023-07-25 01:56:35.774830 autoutils-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/__init__.py
+-rw-r--r--   0        0        0     3081 2024-02-05 11:39:08.521097 autoutils-0.9.1/autoutils/api.py
+-rw-r--r--   0        0        0     8739 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/color.py
+-rw-r--r--   0        0        0     3411 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/file.py
+-rw-r--r--   0        0        0    20748 2023-11-13 09:24:49.207147 autoutils-0.9.1/autoutils/log.py
+-rw-r--r--   0        0        0        0 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/__init__.py
+-rw-r--r--   0        0        0    35272 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/api.py
+-rw-r--r--   0        0        0     7437 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/client.py
+-rw-r--r--   0        0        0     1765 2023-07-25 01:56:35.774830 autoutils-0.9.1/autoutils/matrixcli/errors.py
+-rw-r--r--   0        0        0    24836 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/matrixcli/room.py
+-rw-r--r--   0        0        0     1509 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/matrixcli/user.py
+-rw-r--r--   0        0        0     3253 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/redis.py
+-rw-r--r--   0        0        0     4243 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/script.py
+-rw-r--r--   0        0        0    12052 2023-11-25 06:17:00.273785 autoutils-0.9.1/autoutils/server.py
+-rw-r--r--   0        0        0     6437 2023-07-25 01:56:35.778830 autoutils-0.9.1/autoutils/thread.py
+-rw-r--r--   0        0        0      808 2024-02-05 11:06:58.808667 autoutils-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 autoutils-0.9.1/PKG-INFO
```

### Comparing `autoutils-0.9.0/LICENSE` & `autoutils-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/api.py` & `autoutils-0.9.1/autoutils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     connection_timeout: int = 60
     validate_cert: bool = True
     user_agent: str = "autoutils"
     retry_count: int = 1
     retry_delay: int = 3
     token_name: str = "Bearer"
     supported_http_methods: List[str] = None
+    proxies: dict = None
 
     def __post_init__(self):
         if not self.supported_http_methods:
             self.supported_http_methods = ["GET", "PUT", "DELETE", "POST", "PATCH"]
         self.session = Session()
 
     def _send(self, method: str, path: str, content: dict = None, files=None,
@@ -76,14 +77,15 @@
             try:
                 response = self.session.request(
                     method, endpoint,
                     params=query_params,
                     headers=headers,
                     verify=self.validate_cert,
                     timeout=self.connection_timeout,
+                    proxies=self.proxies,
                     **send_data
                 )
                 logger.info(
                     f"{self.name} api: method {method} with url {endpoint} end. status code {response.status_code}")
                 return ServerResponse(response=response)
             except Exception as e:
                 logger.error(f"{self.name} api: method {method} with url {endpoint} has error {e}")
```

### Comparing `autoutils-0.9.0/autoutils/color.py` & `autoutils-0.9.1/autoutils/color.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/file.py` & `autoutils-0.9.1/autoutils/file.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/log.py` & `autoutils-0.9.1/autoutils/log.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/matrixcli/api.py` & `autoutils-0.9.1/autoutils/matrixcli/api.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/matrixcli/client.py` & `autoutils-0.9.1/autoutils/matrixcli/client.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/matrixcli/errors.py` & `autoutils-0.9.1/autoutils/matrixcli/errors.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/matrixcli/room.py` & `autoutils-0.9.1/autoutils/matrixcli/room.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/matrixcli/user.py` & `autoutils-0.9.1/autoutils/matrixcli/user.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/redis.py` & `autoutils-0.9.1/autoutils/redis.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/script.py` & `autoutils-0.9.1/autoutils/script.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/server.py` & `autoutils-0.9.1/autoutils/server.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/autoutils/thread.py` & `autoutils-0.9.1/autoutils/thread.py`

 * *Files identical despite different names*

### Comparing `autoutils-0.9.0/pyproject.toml` & `autoutils-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils"
-version = "0.9.0"
+version = "0.9.1"
 description = "Some Good Function"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils"
 repository = "https://github.com/rezazeiny/autoutils"
 keywords = ["autoutils"]
```

### Comparing `autoutils-0.9.0/PKG-INFO` & `autoutils-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoutils
-Version: 0.9.0
+Version: 0.9.1
 Summary: Some Good Function
 Home-page: https://github.com/rezazeiny/autoutils
 License: MIT
 Keywords: autoutils
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.6,<4.0
```

