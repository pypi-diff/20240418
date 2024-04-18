# Comparing `tmp/ipl_pipeline_py_common-0.8.2.tar.gz` & `tmp/ipl_pipeline_py_common-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipl_pipeline_py_common-0.8.2.tar", max compression
+gzip compressed data, was "ipl_pipeline_py_common-0.9.0.tar", max compression
```

## Comparing `ipl_pipeline_py_common-0.8.2.tar` & `ipl_pipeline_py_common-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      635 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/README.md
--rw-r--r--   0        0        0     1336 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/CommonFunctions/StartupCommon.py
--rw-r--r--   0        0        0       71 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/CommonFunctions/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/CommonFunctions/urn.py
--rw-r--r--   0        0        0      113 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/__init__.py
--rw-r--r--   0        0        0     3007 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/dBCommonConnector.py
--rw-r--r--   0        0        0       45 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/models/__init__.py
--rw-r--r--   0        0        0      434 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/models/base.py
--rw-r--r--   0        0        0      156 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/QueueModels/__init__.py
--rw-r--r--   0        0        0      166 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/QueueModels/serviceRequest.py
--rw-r--r--   0        0        0     1023 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/QueueModels/serviceResponse.py
--rw-r--r--   0        0        0       58 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pipeline/__init__.py
--rw-r--r--   0        0        0      551 2024-04-12 00:28:39.221281 ipl_pipeline_py_common-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      635 2024-04-12 10:52:59.187207 ipl_pipeline_py_common-0.9.0/README.md
+-rw-r--r--   0        0        0     1336 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/CommonFunctions/StartupCommon.py
+-rw-r--r--   0        0        0       71 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/CommonFunctions/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/CommonFunctions/urn.py
+-rw-r--r--   0        0        0      113 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/__init__.py
+-rw-r--r--   0        0        0     3007 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/dBCommonConnector.py
+-rw-r--r--   0        0        0       45 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/models/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/models/base.py
+-rw-r--r--   0        0        0      156 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/QueueModels/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/QueueModels/serviceRequest.py
+-rw-r--r--   0        0        0     1473 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/QueueModels/serviceResponse.py
+-rw-r--r--   0        0        0       58 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pipeline/__init__.py
+-rw-r--r--   0        0        0      551 2024-04-12 10:52:59.191207 ipl_pipeline_py_common-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.9.0/PKG-INFO
```

### Comparing `ipl_pipeline_py_common-0.8.2/README.md` & `ipl_pipeline_py_common-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.8.2/pipeline/CommonFunctions/StartupCommon.py` & `ipl_pipeline_py_common-0.9.0/pipeline/CommonFunctions/StartupCommon.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.8.2/pipeline/CommonFunctions/urn.py` & `ipl_pipeline_py_common-0.9.0/pipeline/CommonFunctions/urn.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.8.2/pipeline/DBCommon/dBCommonConnector.py` & `ipl_pipeline_py_common-0.9.0/pipeline/DBCommon/dBCommonConnector.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.8.2/pipeline/QueueModels/serviceResponse.py` & `ipl_pipeline_py_common-0.9.0/pipeline/QueueModels/serviceResponse.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 
 
 class ServiceResponse(BaseModel, Generic[T]):
     response_node_id: Optional[str] = Field("unknown")
     response_node_version: Optional[str] = Field("unknown")
     request_error: bool = Field(False, description="Error in request")
     server_error: bool = Field(False, description="Error in server")
-    response_code: Optional[int] = Field(None, description="Response Code")
     request_error_message: Optional[str] = Field(None, description="Error Message")
     response_data: Optional[T] = Field(None, description="Response Data")
 
+    def set_error(self, **kwargs):
+        """
+        Set error in response
+        :param kwargs: server_error, request_error, message
+        :return:
+        """
+        if kwargs.get('server_error', False) and kwargs.get('request_error', False):
+            raise ValueError("Both server_error and request_error cannot be True")
+        self.server_error = kwargs.get('server_error', False)
+        self.request_error = kwargs.get('request_error', False)
+        self.request_error_message = kwargs.get('message', None)
+
     @model_validator(mode='after')
     def check_state(self):
         """
         Check if response data is None if request error is True
         :return:
         """
         if self.request_error and self.response_data:
```

### Comparing `ipl_pipeline_py_common-0.8.2/pyproject.toml` & `ipl_pipeline_py_common-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipl-pipeline-py-common"
-version = "0.8.2"
+version = "0.9.0"
 description = "Common functions and modules for Python based IPL Pipeline Services"
 authors = ["Vincent Lee <vlee@vlee.me.uk>"]
 license = "All Rights Reserved"
 readme = "README.md"
 packages = [{include = "pipeline"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ipl_pipeline_py_common-0.8.2/PKG-INFO` & `ipl_pipeline_py_common-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipl-pipeline-py-common
-Version: 0.8.2
+Version: 0.9.0
 Summary: Common functions and modules for Python based IPL Pipeline Services
 License: All Rights Reserved
 Author: Vincent Lee
 Author-email: vlee@vlee.me.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

