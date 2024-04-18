# Comparing `tmp/suprsend-py-sdk-0.8.0.tar.gz` & `tmp/suprsend-py-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suprsend-py-sdk-0.8.0.tar", last modified: Mon Oct 16 11:41:25 2023, max compression
+gzip compressed data, was "suprsend-py-sdk-0.9.0.tar", last modified: Tue Oct 31 14:14:02 2023, max compression
```

## Comparing `suprsend-py-sdk-0.8.0.tar` & `suprsend-py-sdk-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-16 11:41:25.818632 suprsend-py-sdk-0.8.0/
--rw-r--r--   0 skme      (1000) skme      (1000)     1066 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/LICENSE
--rw-r--r--   0 skme      (1000) skme      (1000)       52 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/MANIFEST.in
--rw-r--r--   0 skme      (1000) skme      (1000)    18955 2023-10-16 11:41:25.818632 suprsend-py-sdk-0.8.0/PKG-INFO
--rw-r--r--   0 skme      (1000) skme      (1000)    18262 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/README.md
--rw-r--r--   0 skme      (1000) skme      (1000)      155 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/pyproject.toml
--rw-r--r--   0 skme      (1000) skme      (1000)      823 2023-10-16 11:41:25.822632 suprsend-py-sdk-0.8.0/setup.cfg
-drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-16 11:41:25.810632 suprsend-py-sdk-0.8.0/src/
-drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-16 11:41:25.818632 suprsend-py-sdk-0.8.0/src/suprsend/
--rw-r--r--   0 skme      (1000) skme      (1000)      772 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/__init__.py
--rw-r--r--   0 skme      (1000) skme      (1000)     1936 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/attachment.py
--rw-r--r--   0 skme      (1000) skme      (1000)     3439 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/brand.py
--rw-r--r--   0 skme      (1000) skme      (1000)     1747 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/bulk_response.py
--rw-r--r--   0 skme      (1000) skme      (1000)     1256 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/constants.py
--rw-r--r--   0 skme      (1000) skme      (1000)     6942 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/event.py
--rw-r--r--   0 skme      (1000) skme      (1000)     8267 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/events_bulk.py
--rw-r--r--   0 skme      (1000) skme      (1000)     2165 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/exception.py
--rw-r--r--   0 skme      (1000) skme      (1000)     4475 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/language_codes.py
-drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-16 11:41:25.818632 suprsend-py-sdk-0.8.0/src/suprsend/request_json/
--rw-r--r--   0 skme      (1000) skme      (1000)     1441 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/request_json/event.json
--rw-r--r--   0 skme      (1000) skme      (1000)     2332 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/request_json/list_broadcast.json
--rw-r--r--   0 skme      (1000) skme      (1000)    12236 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/request_json/workflow.json
--rw-r--r--   0 skme      (1000) skme      (1000)      977 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/request_log.py
--rw-r--r--   0 skme      (1000) skme      (1000)      992 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/request_schema.py
--rw-r--r--   0 skme      (1000) skme      (1000)     5798 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/sdkinstance.py
--rw-r--r--   0 skme      (1000) skme      (1000)     1198 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/signature.py
--rw-r--r--   0 skme      (1000) skme      (1000)    15221 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/subscriber.py
--rw-r--r--   0 skme      (1000) skme      (1000)    15755 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/subscriber_helper.py
--rw-r--r--   0 skme      (1000) skme      (1000)    17117 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/subscriber_list.py
--rw-r--r--   0 skme      (1000) skme      (1000)     8991 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/subscribers_bulk.py
--rw-r--r--   0 skme      (1000) skme      (1000)     7064 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/utils.py
--rw-r--r--   0 skme      (1000) skme      (1000)       22 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.8.0/src/suprsend/version.py
--rw-r--r--   0 skme      (1000) skme      (1000)     4798 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/workflow.py
--rw-r--r--   0 skme      (1000) skme      (1000)     8291 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.8.0/src/suprsend/workflows_bulk.py
-drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-16 11:41:25.818632 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/
--rw-r--r--   0 skme      (1000) skme      (1000)    18955 2023-10-16 11:41:25.000000 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/PKG-INFO
--rw-r--r--   0 skme      (1000) skme      (1000)      969 2023-10-16 11:41:25.000000 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 skme      (1000) skme      (1000)        1 2023-10-16 11:41:25.000000 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 skme      (1000) skme      (1000)       33 2023-10-16 11:41:25.000000 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/requires.txt
--rw-r--r--   0 skme      (1000) skme      (1000)        9 2023-10-16 11:41:25.000000 suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-31 14:14:02.677452 suprsend-py-sdk-0.9.0/
+-rw-r--r--   0 skme      (1000) skme      (1000)     1066 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/LICENSE
+-rw-r--r--   0 skme      (1000) skme      (1000)       52 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/MANIFEST.in
+-rw-r--r--   0 skme      (1000) skme      (1000)    18955 2023-10-31 14:14:02.677452 suprsend-py-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 skme      (1000) skme      (1000)    18262 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.9.0/README.md
+-rw-r--r--   0 skme      (1000) skme      (1000)      155 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 skme      (1000) skme      (1000)      823 2023-10-31 14:14:02.677452 suprsend-py-sdk-0.9.0/setup.cfg
+drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-31 14:14:02.669452 suprsend-py-sdk-0.9.0/src/
+drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-31 14:14:02.673452 suprsend-py-sdk-0.9.0/src/suprsend/
+-rw-r--r--   0 skme      (1000) skme      (1000)      772 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/__init__.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     1936 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/attachment.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     3439 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/brand.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     1747 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/bulk_response.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     1256 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/constants.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     6942 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/event.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     8267 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/events_bulk.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     2165 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/exception.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     4475 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/language_codes.py
+drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-31 14:14:02.673452 suprsend-py-sdk-0.9.0/src/suprsend/request_json/
+-rw-r--r--   0 skme      (1000) skme      (1000)     1441 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/request_json/event.json
+-rw-r--r--   0 skme      (1000) skme      (1000)     2332 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.9.0/src/suprsend/request_json/list_broadcast.json
+-rw-r--r--   0 skme      (1000) skme      (1000)    12236 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.9.0/src/suprsend/request_json/workflow.json
+-rw-r--r--   0 skme      (1000) skme      (1000)      977 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/request_log.py
+-rw-r--r--   0 skme      (1000) skme      (1000)      992 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/request_schema.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     5798 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/sdkinstance.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     1198 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/signature.py
+-rw-r--r--   0 skme      (1000) skme      (1000)    18002 2023-10-31 14:13:30.000000 suprsend-py-sdk-0.9.0/src/suprsend/subscriber.py
+-rw-r--r--   0 skme      (1000) skme      (1000)    17013 2023-10-31 14:13:30.000000 suprsend-py-sdk-0.9.0/src/suprsend/subscriber_helper.py
+-rw-r--r--   0 skme      (1000) skme      (1000)    17117 2023-10-16 10:30:16.000000 suprsend-py-sdk-0.9.0/src/suprsend/subscriber_list.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     8991 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/subscribers_bulk.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     7064 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/utils.py
+-rw-r--r--   0 skme      (1000) skme      (1000)       22 2023-10-31 14:13:30.000000 suprsend-py-sdk-0.9.0/src/suprsend/version.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     4798 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/workflow.py
+-rw-r--r--   0 skme      (1000) skme      (1000)     8291 2023-07-05 01:48:19.000000 suprsend-py-sdk-0.9.0/src/suprsend/workflows_bulk.py
+drwxr-xr-x   0 skme      (1000) skme      (1000)        0 2023-10-31 14:14:02.673452 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/
+-rw-r--r--   0 skme      (1000) skme      (1000)    18955 2023-10-31 14:14:02.000000 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 skme      (1000) skme      (1000)      969 2023-10-31 14:14:02.000000 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 skme      (1000) skme      (1000)        1 2023-10-31 14:14:02.000000 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 skme      (1000) skme      (1000)       33 2023-10-31 14:14:02.000000 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/requires.txt
+-rw-r--r--   0 skme      (1000) skme      (1000)        9 2023-10-31 14:14:02.000000 suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/top_level.txt
```

### Comparing `suprsend-py-sdk-0.8.0/LICENSE` & `suprsend-py-sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/PKG-INFO` & `suprsend-py-sdk-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suprsend-py-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Suprsend library for Python
 Home-page: https://github.com/suprsend/suprsend-py-sdk
 Author: Suprsend
 Author-email: sanjeev@suprsend.com
 Project-URL: Bug Tracker, https://github.com/suprsend/suprsend-py-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `suprsend-py-sdk-0.8.0/README.md` & `suprsend-py-sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/setup.cfg` & `suprsend-py-sdk-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/__init__.py` & `suprsend-py-sdk-0.9.0/src/suprsend/__init__.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/attachment.py` & `suprsend-py-sdk-0.9.0/src/suprsend/attachment.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/brand.py` & `suprsend-py-sdk-0.9.0/src/suprsend/brand.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/bulk_response.py` & `suprsend-py-sdk-0.9.0/src/suprsend/bulk_response.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/constants.py` & `suprsend-py-sdk-0.9.0/src/suprsend/constants.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/event.py` & `suprsend-py-sdk-0.9.0/src/suprsend/event.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/events_bulk.py` & `suprsend-py-sdk-0.9.0/src/suprsend/events_bulk.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/exception.py` & `suprsend-py-sdk-0.9.0/src/suprsend/exception.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/language_codes.py` & `suprsend-py-sdk-0.9.0/src/suprsend/language_codes.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/request_json/event.json` & `suprsend-py-sdk-0.9.0/src/suprsend/request_json/event.json`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/request_json/list_broadcast.json` & `suprsend-py-sdk-0.9.0/src/suprsend/request_json/list_broadcast.json`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/request_json/workflow.json` & `suprsend-py-sdk-0.9.0/src/suprsend/request_json/workflow.json`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/request_log.py` & `suprsend-py-sdk-0.9.0/src/suprsend/request_log.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/request_schema.py` & `suprsend-py-sdk-0.9.0/src/suprsend/request_schema.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/sdkinstance.py` & `suprsend-py-sdk-0.9.0/src/suprsend/sdkinstance.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/signature.py` & `suprsend-py-sdk-0.9.0/src/suprsend/signature.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/subscriber.py` & `suprsend-py-sdk-0.9.0/src/suprsend/subscriber.py`

 * *Files 12% similar despite different names*

```diff
@@ -190,14 +190,92 @@
                 self._collect_event(discard_if_error=True)
         else:
             for k, v in arg1.items():
                 self._helper._append_kv(k, v, arg1, caller=caller)
             # --
             self._collect_event(discard_if_error=False)
 
+    def set(self, arg1, arg2=None):
+        """
+        1. set(k, v)
+        2. set({k1: v1, k2, v2})
+
+        :param arg1: required, one of  [str, dict]
+        :param arg2: required if arg1 is str
+        :return:
+        """
+        caller = "set"
+        if not isinstance(arg1, (str, dict)):
+            self.__errors.append(f"[{caller}] arg1 must be String or a dict")
+            return
+        if isinstance(arg1, (str,)):
+            if arg2 is None:
+                self.__errors.append(f"[{caller}] if arg1 is a string, then arg2 must be passed")
+                return
+            else:
+                self._helper._set_kv(arg1, arg2, caller=caller)
+                self._collect_event(discard_if_error=True)
+        else:
+            for k, v in arg1.items():
+                self._helper._set_kv(k, v, caller=caller)
+            # --
+            self._collect_event(discard_if_error=True)
+
+    def set_once(self, arg1, arg2=None):
+        """
+        1. set_once(k, v)
+        2. set_once({k1: v1, k2, v2})
+
+        :param arg1: required, one of  [str, dict]
+        :param arg2: required if arg1 is str
+        :return:
+        """
+        caller = "set_once"
+        if not isinstance(arg1, (str, dict)):
+            self.__errors.append(f"[{caller}] arg1 must be String or a dict")
+            return
+        if isinstance(arg1, (str,)):
+            if arg2 is None:
+                self.__errors.append(f"[{caller}] if arg1 is a string, then arg2 must be passed")
+                return
+            else:
+                self._helper._set_once_kv(arg1, arg2, caller=caller)
+                self._collect_event(discard_if_error=True)
+        else:
+            for k, v in arg1.items():
+                self._helper._set_once_kv(k, v, caller=caller)
+            # --
+            self._collect_event(discard_if_error=True)
+
+    def increment(self, arg1, arg2=None):
+        """
+        1. increment(k, v)
+        2. increment({k1: v1, k2, v2})
+
+        :param arg1: required, one of  [str, dict]
+        :param arg2: required if arg1 is str
+        :return:
+        """
+        caller = "increment"
+        if not isinstance(arg1, (str, dict)):
+            self.__errors.append(f"[{caller}] arg1 must be String or a dict")
+            return
+        if isinstance(arg1, (str,)):
+            if arg2 is None:
+                self.__errors.append(f"[{caller}] if arg1 is a string, then arg2 must be passed")
+                return
+            else:
+                self._helper._increment_kv(arg1, arg2, caller=caller)
+                self._collect_event(discard_if_error=True)
+        else:
+            for k, v in arg1.items():
+                self._helper._increment_kv(k, v, caller=caller)
+            # --
+            self._collect_event(discard_if_error=True)
+
     def remove(self, arg1, arg2=None):
         """
         Usage:
         1. remove(k, v)
         2. remove({k1: v1, k2, v2})
 
         :param arg1: one of [str, dict]
```

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/subscriber_helper.py` & `suprsend-py-sdk-0.9.0/src/suprsend/subscriber_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,26 @@
 
 class _SubscriberInternalHelper:
     """
     Internal helper class
     """
     def __init__(self):
         self.__dict_set = {}
+        self.__dict_set_once = {}
+        self.__dict_increment = {}
         self.__dict_append = {}
         self.__dict_remove = {}
         self.__list_unset = []
         #
         self.__errors = []
         self.__info = []
 
     def reset(self):
         self.__dict_set, self.__dict_append, self.__dict_remove, self.__list_unset = {}, {}, {}, []
+        self.__dict_set_once, self.__dict_increment = {}, {}
         self.__errors = []
         self.__info = []
 
     def get_identity_event(self):
         evt = self.__form_event()
         ret_val = {
             "errors": self.__errors,
@@ -71,14 +74,18 @@
         self.reset()
         return ret_val
 
     def __form_event(self):
         event = {}
         if self.__dict_set:
             event["$set"] = self.__dict_set
+        if self.__dict_set_once:
+            event["$set_once"] = self.__dict_set_once
+        if self.__dict_increment:
+            event["$add"] = self.__dict_increment
         if self.__dict_append:
             event["$append"] = self.__dict_append
         if self.__dict_remove:
             event["$remove"] = self.__dict_remove
         if self.__list_unset:
             event["$unset"] = self.__list_unset
         return event
@@ -133,14 +140,41 @@
     def _unset_k(self, key, caller="unset"):
         k, is_k_valid = self.__validate_key_basic(key, caller)
         if not is_k_valid:
             return
         # ----
         self.__list_unset.append(k)
 
+    def _set_kv(self, key, val, caller="set"):
+        key, is_k_valid = self.__validate_key_basic(key, caller)
+        if not is_k_valid:
+            return
+        else:
+            is_k_valid = self.__validate_key_prefix(key, caller)
+            if is_k_valid:
+                self.__dict_set[key] = val
+
+    def _set_once_kv(self, key, val, caller="set_once"):
+        key, is_k_valid = self.__validate_key_basic(key, caller)
+        if not is_k_valid:
+            return
+        else:
+            is_k_valid = self.__validate_key_prefix(key, caller)
+            if is_k_valid:
+                self.__dict_set_once[key] = val
+
+    def _increment_kv(self, key, val, caller="increment"):
+        key, is_k_valid = self.__validate_key_basic(key, caller)
+        if not is_k_valid:
+            return
+        else:
+            is_k_valid = self.__validate_key_prefix(key, caller)
+            if is_k_valid:
+                self.__dict_increment[key] = val
+
     def _set_preferred_language(self, lang_code, caller):
         # Check language code is in the list
         if lang_code not in ALL_LANG_CODES:
             self.__info.append(f"[{caller}] invalid value {lang_code}")
             return
         # ---
         self.__dict_set[KEY_PREFERRED_LANGUAGE] = lang_code
```

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/subscriber_list.py` & `suprsend-py-sdk-0.9.0/src/suprsend/subscriber_list.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/subscribers_bulk.py` & `suprsend-py-sdk-0.9.0/src/suprsend/subscribers_bulk.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/utils.py` & `suprsend-py-sdk-0.9.0/src/suprsend/utils.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/workflow.py` & `suprsend-py-sdk-0.9.0/src/suprsend/workflow.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend/workflows_bulk.py` & `suprsend-py-sdk-0.9.0/src/suprsend/workflows_bulk.py`

 * *Files identical despite different names*

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/PKG-INFO` & `suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suprsend-py-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Suprsend library for Python
 Home-page: https://github.com/suprsend/suprsend-py-sdk
 Author: Suprsend
 Author-email: sanjeev@suprsend.com
 Project-URL: Bug Tracker, https://github.com/suprsend/suprsend-py-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `suprsend-py-sdk-0.8.0/src/suprsend_py_sdk.egg-info/SOURCES.txt` & `suprsend-py-sdk-0.9.0/src/suprsend_py_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

