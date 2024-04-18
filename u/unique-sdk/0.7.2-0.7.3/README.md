# Comparing `tmp/unique_sdk-0.7.2.tar.gz` & `tmp/unique_sdk-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_sdk-0.7.2.tar", max compression
+gzip compressed data, was "unique_sdk-0.7.3.tar", max compression
```

## Comparing `unique_sdk-0.7.2.tar` & `unique_sdk-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1065 2024-02-22 20:34:45.135463 unique_sdk-0.7.2/LICENSE
--rw-r--r--   0        0        0    12693 2024-03-27 13:36:17.907620 unique_sdk-0.7.2/README.md
--rw-r--r--   0        0        0     1400 2024-04-12 09:11:24.414465 unique_sdk-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2594 2024-03-22 15:16:21.679272 unique_sdk-0.7.2/unique_sdk/__init__.py
--rw-r--r--   0        0        0    11523 2024-03-22 15:16:21.683007 unique_sdk-0.7.2/unique_sdk/_api_requestor.py
--rw-r--r--   0        0        0     3603 2024-02-27 19:23:40.262420 unique_sdk-0.7.2/unique_sdk/_api_resource.py
--rw-r--r--   0        0        0       46 2024-02-22 20:34:45.142217 unique_sdk-0.7.2/unique_sdk/_api_version.py
--rw-r--r--   0        0        0     2912 2024-02-22 20:34:45.142578 unique_sdk-0.7.2/unique_sdk/_error.py
--rw-r--r--   0        0        0     2512 2024-02-22 20:34:45.142765 unique_sdk-0.7.2/unique_sdk/_http_client.py
--rw-r--r--   0        0        0     3949 2024-02-22 20:34:45.142939 unique_sdk-0.7.2/unique_sdk/_list_object.py
--rw-r--r--   0        0        0      270 2024-02-22 20:34:45.143185 unique_sdk-0.7.2/unique_sdk/_object_classes.py
--rw-r--r--   0        0        0      255 2024-02-22 20:34:45.143412 unique_sdk-0.7.2/unique_sdk/_request_options.py
--rw-r--r--   0        0        0    10525 2024-02-22 20:34:45.143669 unique_sdk-0.7.2/unique_sdk/_unique_object.py
--rw-r--r--   0        0        0      576 2024-02-22 20:34:45.143826 unique_sdk-0.7.2/unique_sdk/_unique_response.py
--rw-r--r--   0        0        0     5902 2024-02-22 20:34:45.144184 unique_sdk-0.7.2/unique_sdk/_util.py
--rw-r--r--   0        0        0       18 2024-02-22 20:34:45.144336 unique_sdk-0.7.2/unique_sdk/_version.py
--rw-r--r--   0        0        0     2855 2024-02-22 20:34:45.144492 unique_sdk-0.7.2/unique_sdk/_webhook.py
--rw-r--r--   0        0        0        0 2024-02-22 20:34:45.144734 unique_sdk-0.7.2/unique_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0     1738 2024-02-22 20:34:45.144922 unique_sdk-0.7.2/unique_sdk/api_resources/_chat_completion.py
--rw-r--r--   0        0        0     3005 2024-04-11 09:50:40.483379 unique_sdk-0.7.2/unique_sdk/api_resources/_content.py
--rw-r--r--   0        0        0      374 2024-02-22 20:34:45.145139 unique_sdk-0.7.2/unique_sdk/api_resources/_event.py
--rw-r--r--   0        0        0     2310 2024-04-12 09:11:24.416488 unique_sdk-0.7.2/unique_sdk/api_resources/_integrated.py
--rw-r--r--   0        0        0     4937 2024-03-22 15:16:21.690047 unique_sdk-0.7.2/unique_sdk/api_resources/_message.py
--rw-r--r--   0        0        0     1235 2024-04-11 09:50:40.488785 unique_sdk-0.7.2/unique_sdk/api_resources/_search.py
--rw-r--r--   0        0        0     1366 2024-02-22 20:34:45.147647 unique_sdk-0.7.2/unique_sdk/api_resources/_search_string.py
--rw-r--r--   0        0        0    13153 1970-01-01 00:00:00.000000 unique_sdk-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-22 20:34:45.135463 unique_sdk-0.7.3/LICENSE
+-rw-r--r--   0        0        0    12693 2024-03-27 13:36:17.907620 unique_sdk-0.7.3/README.md
+-rw-r--r--   0        0        0     1400 2024-04-18 07:34:45.921205 unique_sdk-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2594 2024-03-22 15:16:21.679272 unique_sdk-0.7.3/unique_sdk/__init__.py
+-rw-r--r--   0        0        0    11523 2024-03-22 15:16:21.683007 unique_sdk-0.7.3/unique_sdk/_api_requestor.py
+-rw-r--r--   0        0        0     3603 2024-02-27 19:23:40.262420 unique_sdk-0.7.3/unique_sdk/_api_resource.py
+-rw-r--r--   0        0        0       46 2024-02-22 20:34:45.142217 unique_sdk-0.7.3/unique_sdk/_api_version.py
+-rw-r--r--   0        0        0     2912 2024-02-22 20:34:45.142578 unique_sdk-0.7.3/unique_sdk/_error.py
+-rw-r--r--   0        0        0     2513 2024-04-18 07:34:45.931494 unique_sdk-0.7.3/unique_sdk/_http_client.py
+-rw-r--r--   0        0        0     3949 2024-02-22 20:34:45.142939 unique_sdk-0.7.3/unique_sdk/_list_object.py
+-rw-r--r--   0        0        0      270 2024-02-22 20:34:45.143185 unique_sdk-0.7.3/unique_sdk/_object_classes.py
+-rw-r--r--   0        0        0      255 2024-02-22 20:34:45.143412 unique_sdk-0.7.3/unique_sdk/_request_options.py
+-rw-r--r--   0        0        0    10525 2024-02-22 20:34:45.143669 unique_sdk-0.7.3/unique_sdk/_unique_object.py
+-rw-r--r--   0        0        0      576 2024-02-22 20:34:45.143826 unique_sdk-0.7.3/unique_sdk/_unique_response.py
+-rw-r--r--   0        0        0     5902 2024-02-22 20:34:45.144184 unique_sdk-0.7.3/unique_sdk/_util.py
+-rw-r--r--   0        0        0       18 2024-02-22 20:34:45.144336 unique_sdk-0.7.3/unique_sdk/_version.py
+-rw-r--r--   0        0        0     2855 2024-02-22 20:34:45.144492 unique_sdk-0.7.3/unique_sdk/_webhook.py
+-rw-r--r--   0        0        0        0 2024-02-22 20:34:45.144734 unique_sdk-0.7.3/unique_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0     1738 2024-02-22 20:34:45.144922 unique_sdk-0.7.3/unique_sdk/api_resources/_chat_completion.py
+-rw-r--r--   0        0        0     3005 2024-04-11 09:50:40.483379 unique_sdk-0.7.3/unique_sdk/api_resources/_content.py
+-rw-r--r--   0        0        0      374 2024-02-22 20:34:45.145139 unique_sdk-0.7.3/unique_sdk/api_resources/_event.py
+-rw-r--r--   0        0        0     2310 2024-04-12 09:11:24.416488 unique_sdk-0.7.3/unique_sdk/api_resources/_integrated.py
+-rw-r--r--   0        0        0     4937 2024-03-22 15:16:21.690047 unique_sdk-0.7.3/unique_sdk/api_resources/_message.py
+-rw-r--r--   0        0        0     1235 2024-04-11 09:50:40.488785 unique_sdk-0.7.3/unique_sdk/api_resources/_search.py
+-rw-r--r--   0        0        0     1366 2024-02-22 20:34:45.147647 unique_sdk-0.7.3/unique_sdk/api_resources/_search_string.py
+-rw-r--r--   0        0        0    13153 1970-01-01 00:00:00.000000 unique_sdk-0.7.3/PKG-INFO
```

### Comparing `unique_sdk-0.7.2/LICENSE` & `unique_sdk-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/README.md` & `unique_sdk-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/pyproject.toml` & `unique_sdk-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unique-sdk"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = [
     "Konstantin Krauss <konstantin@unique.ch>",
     "Andreas Hauri <andreas@unique.ch>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `unique_sdk-0.7.2/unique_sdk/__init__.py` & `unique_sdk-0.7.3/unique_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_api_requestor.py` & `unique_sdk-0.7.3/unique_sdk/_api_requestor.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_api_resource.py` & `unique_sdk-0.7.3/unique_sdk/_api_resource.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_error.py` & `unique_sdk-0.7.3/unique_sdk/_error.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_http_client.py` & `unique_sdk-0.7.3/unique_sdk/_http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def request(self, method, url, headers, post_data=None):
         raise NotImplementedError("HTTPClient subclasses must implement `request`")
 
 
 class RequestsClient(HTTPClient):
     name = "requests"
 
-    def __init__(self, timeout=80, session=None, **kwargs):
+    def __init__(self, timeout=600, session=None, **kwargs):
         super(RequestsClient, self).__init__(**kwargs)
         self._timeout = timeout
         self._session = session
 
         assert requests is not None
         self.requests = requests
```

### Comparing `unique_sdk-0.7.2/unique_sdk/_list_object.py` & `unique_sdk-0.7.3/unique_sdk/_list_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_unique_object.py` & `unique_sdk-0.7.3/unique_sdk/_unique_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_unique_response.py` & `unique_sdk-0.7.3/unique_sdk/_unique_response.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_util.py` & `unique_sdk-0.7.3/unique_sdk/_util.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/_webhook.py` & `unique_sdk-0.7.3/unique_sdk/_webhook.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_chat_completion.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_chat_completion.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_content.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_content.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_integrated.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_integrated.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_message.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_message.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_search.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_search.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/unique_sdk/api_resources/_search_string.py` & `unique_sdk-0.7.3/unique_sdk/api_resources/_search_string.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.2/PKG-INFO` & `unique_sdk-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-sdk
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 License: MIT
 Author: Konstantin Krauss
 Author-email: konstantin@unique.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

