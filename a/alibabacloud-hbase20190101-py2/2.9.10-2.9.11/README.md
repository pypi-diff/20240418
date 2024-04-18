# Comparing `tmp/alibabacloud_hbase20190101_py2-2.9.10.tar.gz` & `tmp/alibabacloud_hbase20190101_py2-2.9.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hbase20190101_py2-2.9.10.tar", last modified: Thu Apr 14 07:26:55 2022, max compression
+gzip compressed data, was "dist/alibabacloud_hbase20190101_py2-2.9.11.tar", last modified: Tue Aug 15 08:42:28 2023, max compression
```

## Comparing `alibabacloud_hbase20190101_py2-2.9.10.tar` & `alibabacloud_hbase20190101_py2-2.9.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:26:55.000000 alibabacloud_hbase20190101_py2-2.9.10/
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2498 2022-04-14 07:26:55.000000 alibabacloud_hbase20190101_py2-2.9.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:26:55.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/
--rw-r--r--   0 root         (0) root         (0)       22 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136860 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/client.py
--rw-r--r--   0 root         (0) root         (0)   587287 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:26:55.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2498 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-14 07:26:55.000000 alibabacloud_hbase20190101_py2-2.9.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2926 2022-04-14 07:26:54.000000 alibabacloud_hbase20190101_py2-2.9.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136465 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)   624163 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-08-15 08:42:28.000000 alibabacloud_hbase20190101_py2-2.9.11/setup.py
```

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/LICENSE` & `alibabacloud_hbase20190101_py2-2.9.11/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/PKG-INFO` & `alibabacloud_hbase20190101_py2-2.9.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_hbase20190101_py2
-Version: 2.9.10
+Version: 2.9.11
 Summary: Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/README-CN.md` & `alibabacloud_hbase20190101_py2-2.9.11/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/README.md` & `alibabacloud_hbase20190101_py2-2.9.11/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/client.py` & `alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,57 +17,26 @@
     """
     *\
     """
     def __init__(self, config):
         super(Client, self).__init__(config)
         self._endpoint_rule = 'regional'
         self._endpoint_map = {
-            'ap-northeast-2-pop': 'hbase.aliyuncs.com',
             'ap-southeast-1': 'hbase.aliyuncs.com',
             'cn-beijing': 'hbase.aliyuncs.com',
-            'cn-beijing-finance-1': 'hbase.aliyuncs.com',
-            'cn-beijing-finance-pop': 'hbase.aliyuncs.com',
-            'cn-beijing-gov-1': 'hbase.aliyuncs.com',
-            'cn-beijing-nu16-b01': 'hbase.aliyuncs.com',
-            'cn-edge-1': 'hbase.aliyuncs.com',
-            'cn-fujian': 'hbase.aliyuncs.com',
-            'cn-haidian-cm12-c01': 'hbase.aliyuncs.com',
             'cn-hangzhou': 'hbase.aliyuncs.com',
-            'cn-hangzhou-bj-b01': 'hbase.aliyuncs.com',
             'cn-hangzhou-finance': 'hbase.aliyuncs.com',
-            'cn-hangzhou-internal-prod-1': 'hbase.aliyuncs.com',
-            'cn-hangzhou-internal-test-1': 'hbase.aliyuncs.com',
-            'cn-hangzhou-internal-test-2': 'hbase.aliyuncs.com',
-            'cn-hangzhou-internal-test-3': 'hbase.aliyuncs.com',
-            'cn-hangzhou-test-306': 'hbase.aliyuncs.com',
             'cn-hongkong': 'hbase.aliyuncs.com',
-            'cn-hongkong-finance-pop': 'hbase.aliyuncs.com',
             'cn-north-2-gov-1': 'hbase.aliyuncs.com',
             'cn-qingdao': 'hbase.aliyuncs.com',
-            'cn-qingdao-nebula': 'hbase.aliyuncs.com',
             'cn-shanghai': 'hbase.aliyuncs.com',
-            'cn-shanghai-et15-b01': 'hbase.aliyuncs.com',
-            'cn-shanghai-et2-b01': 'hbase.aliyuncs.com',
             'cn-shanghai-finance-1': 'hbase.aliyuncs.com',
-            'cn-shanghai-inner': 'hbase.aliyuncs.com',
-            'cn-shanghai-internal-test-1': 'hbase.aliyuncs.com',
             'cn-shenzhen': 'hbase.aliyuncs.com',
             'cn-shenzhen-finance-1': 'hbase.aliyuncs.com',
-            'cn-shenzhen-inner': 'hbase.aliyuncs.com',
-            'cn-shenzhen-st4-d01': 'hbase.aliyuncs.com',
-            'cn-shenzhen-su18-b01': 'hbase.aliyuncs.com',
-            'cn-wuhan': 'hbase.aliyuncs.com',
-            'cn-yushanfang': 'hbase.aliyuncs.com',
-            'cn-zhangbei-na61-b01': 'hbase.aliyuncs.com',
-            'cn-zhangjiakou-na62-a01': 'hbase.aliyuncs.com',
-            'cn-zhengzhou-nebula-1': 'hbase.aliyuncs.com',
-            'eu-west-1-oxs': 'hbase.ap-northeast-1.aliyuncs.com',
-            'rus-west-1-pop': 'hbase.ap-northeast-1.aliyuncs.com',
-            'us-east-1': 'hbase.aliyuncs.com',
-            'us-west-1': 'hbase.aliyuncs.com'
+            'cn-guangzhou': 'hbase.aliyuncs.com'
         }
         self.check_config(config)
         self._endpoint = self.get_endpoint('hbase', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
 
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
@@ -366,14 +335,16 @@
     def create_global_resource_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_name):
             query['ResourceName'] = request.resource_name
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -650,14 +621,16 @@
         return self.create_serverless_cluster_with_options(request, runtime)
 
     def delete_global_resource_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_name):
             query['ResourceName'] = request.resource_name
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3221,14 +3194,46 @@
             self.call_api(params, req, runtime)
         )
 
     def switch_hbase_ha_slb(self, request):
         runtime = util_models.RuntimeOptions()
         return self.switch_hbase_ha_slb_with_options(request, runtime)
 
+    def switch_service_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cluster_id):
+            query['ClusterId'] = request.cluster_id
+        if not UtilClient.is_unset(request.operate):
+            query['Operate'] = request.operate
+        if not UtilClient.is_unset(request.service_name):
+            query['ServiceName'] = request.service_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SwitchService',
+            version='2019-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            hbase_20190101_models.SwitchServiceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def switch_service(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.switch_service_with_options(request, runtime)
+
     def tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
```

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101/models.py` & `alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,40 +58,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class AddUserHdfsInfoResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: AddUserHdfsInfoResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(AddUserHdfsInfoResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddUserHdfsInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AllocatePublicNetworkAddressRequest(TeaModel):
@@ -144,40 +150,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class AllocatePublicNetworkAddressResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: AllocatePublicNetworkAddressResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(AllocatePublicNetworkAddressResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AllocatePublicNetworkAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CancelActiveOperationTasksRequest(TeaModel):
@@ -256,40 +268,46 @@
             self.ids = m.get('Ids')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CancelActiveOperationTasksResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CancelActiveOperationTasksResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CancelActiveOperationTasksResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CancelActiveOperationTasksResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CheckComponentsVersionRequest(TeaModel):
@@ -410,40 +428,46 @@
             self.components = temp_model.from_map(m['Components'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CheckComponentsVersionResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CheckComponentsVersionResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CheckComponentsVersionResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CheckComponentsVersionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CloseBackupRequest(TeaModel):
@@ -491,40 +515,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CloseBackupResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CloseBackupResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CloseBackupResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CloseBackupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ConvertInstanceRequest(TeaModel):
@@ -592,40 +622,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ConvertInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ConvertInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ConvertInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ConvertInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateBackupPlanRequest(TeaModel):
@@ -673,40 +709,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateBackupPlanResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateBackupPlanResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateBackupPlanResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateBackupPlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateClusterRequest(TeaModel):
@@ -867,50 +909,57 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateGlobalResourceRequest(TeaModel):
-    def __init__(self, client_token=None, cluster_id=None, resource_name=None, resource_type=None):
+    def __init__(self, client_token=None, cluster_id=None, region_id=None, resource_name=None, resource_type=None):
         self.client_token = client_token  # type: str
         self.cluster_id = cluster_id  # type: str
+        self.region_id = region_id  # type: str
         self.resource_name = resource_name  # type: str
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -919,26 +968,30 @@
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
         if self.resource_name is not None:
             result['ResourceName'] = self.resource_name
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
         if m.get('ResourceName') is not None:
             self.resource_name = m.get('ResourceName')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
@@ -963,40 +1016,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateGlobalResourceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateGlobalResourceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateGlobalResourceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateGlobalResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateHBaseSlbServerRequest(TeaModel):
@@ -1054,40 +1113,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateHBaseSlbServerResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateHBaseSlbServerResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateHBaseSlbServerResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateHBaseSlbServerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateHbaseHaSlbRequest(TeaModel):
@@ -1155,40 +1220,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateHbaseHaSlbResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateHbaseHaSlbResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateHbaseHaSlbResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateHbaseHaSlbResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateMultiZoneClusterRequest(TeaModel):
@@ -1391,40 +1462,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateMultiZoneClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateMultiZoneClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateMultiZoneClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateMultiZoneClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateRestorePlanRequest(TeaModel):
@@ -1498,40 +1575,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateRestorePlanResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateRestorePlanResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateRestorePlanResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateRestorePlanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateServerlessClusterRequest(TeaModel):
@@ -1682,73 +1765,84 @@
             self.pass_word = m.get('PassWord')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class CreateServerlessClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateServerlessClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateServerlessClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateServerlessClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteGlobalResourceRequest(TeaModel):
-    def __init__(self, cluster_id=None, resource_name=None, resource_type=None):
+    def __init__(self, cluster_id=None, region_id=None, resource_name=None, resource_type=None):
         self.cluster_id = cluster_id  # type: str
+        self.region_id = region_id  # type: str
         self.resource_name = resource_name  # type: str
         self.resource_type = resource_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteGlobalResourceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
         if self.resource_name is not None:
             result['ResourceName'] = self.resource_name
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
         if m.get('ResourceName') is not None:
             self.resource_name = m.get('ResourceName')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
@@ -1773,40 +1867,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteGlobalResourceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteGlobalResourceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteGlobalResourceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteGlobalResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteHBaseHaDBRequest(TeaModel):
@@ -1859,40 +1959,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteHBaseHaDBResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteHBaseHaDBResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteHBaseHaDBResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHBaseHaDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteHBaseSlbServerRequest(TeaModel):
@@ -1945,40 +2051,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteHBaseSlbServerResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteHBaseSlbServerResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteHBaseSlbServerResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHBaseSlbServerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteHbaseHaSlbRequest(TeaModel):
@@ -2036,40 +2148,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteHbaseHaSlbResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteHbaseHaSlbResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteHbaseHaSlbResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHbaseHaSlbResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteInstanceRequest(TeaModel):
@@ -2122,40 +2240,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteMultiZoneClusterRequest(TeaModel):
@@ -2208,40 +2332,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteMultiZoneClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteMultiZoneClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteMultiZoneClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteMultiZoneClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteServerlessClusterRequest(TeaModel):
@@ -2299,40 +2429,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteServerlessClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteServerlessClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteServerlessClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteServerlessClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteUserHdfsInfoRequest(TeaModel):
@@ -2385,40 +2521,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DeleteUserHdfsInfoResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteUserHdfsInfoResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteUserHdfsInfoResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteUserHdfsInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeActiveOperationTaskTypeRequest(TeaModel):
@@ -2544,40 +2686,46 @@
             for k in m.get('TypeList'):
                 temp_model = DescribeActiveOperationTaskTypeResponseBodyTypeList()
                 self.type_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeActiveOperationTaskTypeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeActiveOperationTaskTypeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeActiveOperationTaskTypeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeActiveOperationTaskTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeActiveOperationTasksRequest(TeaModel):
@@ -2883,40 +3031,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalRecordCount') is not None:
             self.total_record_count = m.get('TotalRecordCount')
         return self
 
 
 class DescribeActiveOperationTasksResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeActiveOperationTasksResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeActiveOperationTasksResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeActiveOperationTasksResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAvailableResourceRequest(TeaModel):
@@ -3562,40 +3716,46 @@
             self.available_zones = temp_model.from_map(m['AvailableZones'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeAvailableResourceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeAvailableResourceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeAvailableResourceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAvailableResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupPlanConfigRequest(TeaModel):
@@ -3690,40 +3850,46 @@
         if m.get('Tables') is not None:
             temp_model = DescribeBackupPlanConfigResponseBodyTables()
             self.tables = temp_model.from_map(m['Tables'])
         return self
 
 
 class DescribeBackupPlanConfigResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupPlanConfigResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupPlanConfigResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupPlanConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupPolicyRequest(TeaModel):
@@ -3797,40 +3963,46 @@
             self.preferred_backup_time = m.get('PreferredBackupTime')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeBackupPolicyResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupPolicyResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupPolicyResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupStatusRequest(TeaModel):
@@ -3893,40 +4065,46 @@
             self.cluster_id = m.get('ClusterId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeBackupStatusResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupStatusResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupStatusResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupSummaryRequest(TeaModel):
@@ -4188,40 +4366,46 @@
             self.incr = temp_model.from_map(m['Incr'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeBackupSummaryResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupSummaryResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupSummaryResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupSummaryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupTablesRequest(TeaModel):
@@ -4431,40 +4615,46 @@
             self.tables = temp_model.from_map(m['Tables'])
         if m.get('Total') is not None:
             self.total = m.get('Total')
         return self
 
 
 class DescribeBackupTablesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupTablesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupTablesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupTablesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeBackupsRequest(TeaModel):
@@ -4689,40 +4879,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeBackupsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeBackupsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeBackupsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeClusterConnectionRequest(TeaModel):
@@ -5169,40 +5365,46 @@
         if m.get('ZkConnAddrs') is not None:
             temp_model = DescribeClusterConnectionResponseBodyZkConnAddrs()
             self.zk_conn_addrs = temp_model.from_map(m['ZkConnAddrs'])
         return self
 
 
 class DescribeClusterConnectionResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeClusterConnectionResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeClusterConnectionResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeClusterConnectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeColdStorageRequest(TeaModel):
@@ -5286,40 +5488,46 @@
             self.pay_type = m.get('PayType')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeColdStorageResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeColdStorageResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeColdStorageResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeColdStorageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDBInstanceUsageRequest(TeaModel):
@@ -5372,40 +5580,46 @@
             self.request_id = m.get('RequestId')
         if m.get('Result') is not None:
             self.result = m.get('Result')
         return self
 
 
 class DescribeDBInstanceUsageResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeDBInstanceUsageResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeDBInstanceUsageResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDBInstanceUsageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDeletedInstancesRequest(TeaModel):
@@ -5598,40 +5812,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeDeletedInstancesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeDeletedInstancesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeDeletedInstancesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDeletedInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDiskWarningLineRequest(TeaModel):
@@ -5684,40 +5904,46 @@
             self.request_id = m.get('RequestId')
         if m.get('WarningLine') is not None:
             self.warning_line = m.get('WarningLine')
         return self
 
 
 class DescribeDiskWarningLineResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeDiskWarningLineResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeDiskWarningLineResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDiskWarningLineResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeEndpointsRequest(TeaModel):
@@ -5863,40 +6089,46 @@
             self.v_switch_id = m.get('VSwitchId')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeEndpointsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeEndpointsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeEndpointsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeEndpointsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceRequest(TeaModel):
@@ -6008,21 +6240,22 @@
         return self
 
 
 class DescribeInstanceResponseBody(TeaModel):
     def __init__(self, auto_renewal=None, backup_status=None, cluster_id=None, cluster_name=None, cluster_type=None,
                  cold_storage_size=None, cold_storage_status=None, confirm_maintain_time=None, core_disk_count=None,
                  core_disk_size=None, core_disk_type=None, core_instance_type=None, core_node_count=None, created_time=None,
-                 created_time_utc=None, duration=None, encryption_key=None, encryption_type=None, engine=None, expire_time=None,
-                 expire_time_utc=None, instance_id=None, instance_name=None, is_deletion_protection=None, is_ha=None,
-                 is_latest_version=None, is_multi_model=None, maintain_end_time=None, maintain_start_time=None, major_version=None,
-                 master_disk_size=None, master_disk_type=None, master_instance_type=None, master_node_count=None,
-                 minor_version=None, module_id=None, module_stack_version=None, need_upgrade=None, need_upgrade_comps=None,
-                 network_type=None, parent_id=None, pay_type=None, region_id=None, request_id=None, resource_group_id=None,
-                 status=None, tags=None, task_progress=None, vpc_id=None, vswitch_id=None, zone_id=None):
+                 created_time_utc=None, duration=None, enable_hbase_proxy=None, encryption_key=None, encryption_type=None,
+                 engine=None, expire_time=None, expire_time_utc=None, instance_id=None, instance_name=None,
+                 is_deletion_protection=None, is_ha=None, is_latest_version=None, is_multi_model=None, lproxy_minor_version=None,
+                 maintain_end_time=None, maintain_start_time=None, major_version=None, master_disk_size=None, master_disk_type=None,
+                 master_instance_type=None, master_node_count=None, minor_version=None, module_id=None, module_stack_version=None,
+                 need_upgrade=None, need_upgrade_comps=None, network_type=None, parent_id=None, pay_type=None, region_id=None,
+                 request_id=None, resource_group_id=None, status=None, tags=None, task_progress=None, vpc_id=None,
+                 vswitch_id=None, zone_id=None):
         self.auto_renewal = auto_renewal  # type: bool
         self.backup_status = backup_status  # type: str
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.cluster_type = cluster_type  # type: str
         self.cold_storage_size = cold_storage_size  # type: int
         self.cold_storage_status = cold_storage_status  # type: str
@@ -6031,25 +6264,27 @@
         self.core_disk_size = core_disk_size  # type: int
         self.core_disk_type = core_disk_type  # type: str
         self.core_instance_type = core_instance_type  # type: str
         self.core_node_count = core_node_count  # type: int
         self.created_time = created_time  # type: str
         self.created_time_utc = created_time_utc  # type: str
         self.duration = duration  # type: int
+        self.enable_hbase_proxy = enable_hbase_proxy  # type: bool
         self.encryption_key = encryption_key  # type: str
         self.encryption_type = encryption_type  # type: str
         self.engine = engine  # type: str
         self.expire_time = expire_time  # type: str
         self.expire_time_utc = expire_time_utc  # type: str
         self.instance_id = instance_id  # type: str
         self.instance_name = instance_name  # type: str
         self.is_deletion_protection = is_deletion_protection  # type: bool
         self.is_ha = is_ha  # type: bool
         self.is_latest_version = is_latest_version  # type: bool
         self.is_multi_model = is_multi_model  # type: bool
+        self.lproxy_minor_version = lproxy_minor_version  # type: str
         self.maintain_end_time = maintain_end_time  # type: str
         self.maintain_start_time = maintain_start_time  # type: str
         self.major_version = major_version  # type: str
         self.master_disk_size = master_disk_size  # type: int
         self.master_disk_type = master_disk_type  # type: str
         self.master_instance_type = master_instance_type  # type: str
         self.master_node_count = master_node_count  # type: int
@@ -6111,14 +6346,16 @@
             result['CoreNodeCount'] = self.core_node_count
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
         if self.created_time_utc is not None:
             result['CreatedTimeUTC'] = self.created_time_utc
         if self.duration is not None:
             result['Duration'] = self.duration
+        if self.enable_hbase_proxy is not None:
+            result['EnableHbaseProxy'] = self.enable_hbase_proxy
         if self.encryption_key is not None:
             result['EncryptionKey'] = self.encryption_key
         if self.encryption_type is not None:
             result['EncryptionType'] = self.encryption_type
         if self.engine is not None:
             result['Engine'] = self.engine
         if self.expire_time is not None:
@@ -6133,14 +6370,16 @@
             result['IsDeletionProtection'] = self.is_deletion_protection
         if self.is_ha is not None:
             result['IsHa'] = self.is_ha
         if self.is_latest_version is not None:
             result['IsLatestVersion'] = self.is_latest_version
         if self.is_multi_model is not None:
             result['IsMultiModel'] = self.is_multi_model
+        if self.lproxy_minor_version is not None:
+            result['LproxyMinorVersion'] = self.lproxy_minor_version
         if self.maintain_end_time is not None:
             result['MaintainEndTime'] = self.maintain_end_time
         if self.maintain_start_time is not None:
             result['MaintainStartTime'] = self.maintain_start_time
         if self.major_version is not None:
             result['MajorVersion'] = self.major_version
         if self.master_disk_size is not None:
@@ -6217,14 +6456,16 @@
             self.core_node_count = m.get('CoreNodeCount')
         if m.get('CreatedTime') is not None:
             self.created_time = m.get('CreatedTime')
         if m.get('CreatedTimeUTC') is not None:
             self.created_time_utc = m.get('CreatedTimeUTC')
         if m.get('Duration') is not None:
             self.duration = m.get('Duration')
+        if m.get('EnableHbaseProxy') is not None:
+            self.enable_hbase_proxy = m.get('EnableHbaseProxy')
         if m.get('EncryptionKey') is not None:
             self.encryption_key = m.get('EncryptionKey')
         if m.get('EncryptionType') is not None:
             self.encryption_type = m.get('EncryptionType')
         if m.get('Engine') is not None:
             self.engine = m.get('Engine')
         if m.get('ExpireTime') is not None:
@@ -6239,14 +6480,16 @@
             self.is_deletion_protection = m.get('IsDeletionProtection')
         if m.get('IsHa') is not None:
             self.is_ha = m.get('IsHa')
         if m.get('IsLatestVersion') is not None:
             self.is_latest_version = m.get('IsLatestVersion')
         if m.get('IsMultiModel') is not None:
             self.is_multi_model = m.get('IsMultiModel')
+        if m.get('LproxyMinorVersion') is not None:
+            self.lproxy_minor_version = m.get('LproxyMinorVersion')
         if m.get('MaintainEndTime') is not None:
             self.maintain_end_time = m.get('MaintainEndTime')
         if m.get('MaintainStartTime') is not None:
             self.maintain_start_time = m.get('MaintainStartTime')
         if m.get('MajorVersion') is not None:
             self.major_version = m.get('MajorVersion')
         if m.get('MasterDiskSize') is not None:
@@ -6293,40 +6536,46 @@
             self.vswitch_id = m.get('VswitchId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
 class DescribeInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstanceTypeRequest(TeaModel):
@@ -6447,40 +6696,46 @@
             self.instance_type_spec_list = temp_model.from_map(m['InstanceTypeSpecList'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeInstanceTypeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeInstanceTypeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeInstanceTypeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstanceTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstancesRequestTag(TeaModel):
@@ -6933,40 +7188,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class DescribeInstancesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeInstancesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeInstancesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeIpWhitelistRequest(TeaModel):
@@ -7113,40 +7374,46 @@
             self.groups = temp_model.from_map(m['Groups'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeIpWhitelistResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeIpWhitelistResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeIpWhitelistResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeIpWhitelistResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeMultiZoneAvailableRegionsRequest(TeaModel):
@@ -7361,40 +7628,46 @@
             self.regions = temp_model.from_map(m['Regions'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeMultiZoneAvailableRegionsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeMultiZoneAvailableRegionsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeMultiZoneAvailableRegionsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeMultiZoneAvailableRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeMultiZoneAvailableResourceRequest(TeaModel):
@@ -8019,40 +8292,46 @@
             self.available_zones = temp_model.from_map(m['AvailableZones'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeMultiZoneAvailableResourceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeMultiZoneAvailableResourceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeMultiZoneAvailableResourceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeMultiZoneAvailableResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeMultiZoneClusterRequest(TeaModel):
@@ -8076,48 +8355,69 @@
         m = m or dict()
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         return self
 
 
 class DescribeMultiZoneClusterResponseBodyMultiZoneInstanceModelsMultiZoneInstanceModel(TeaModel):
-    def __init__(self, ins_name=None, is_latest_version=None, minor_version=None, role=None, status=None):
+    def __init__(self, hdfs_minor_version=None, ins_name=None, is_hdfs_latest_version=None, is_latest_version=None,
+                 latest_hdfs_minor_version=None, latest_minor_version=None, minor_version=None, role=None, status=None):
+        self.hdfs_minor_version = hdfs_minor_version  # type: str
         self.ins_name = ins_name  # type: str
+        self.is_hdfs_latest_version = is_hdfs_latest_version  # type: str
         self.is_latest_version = is_latest_version  # type: bool
+        self.latest_hdfs_minor_version = latest_hdfs_minor_version  # type: str
+        self.latest_minor_version = latest_minor_version  # type: str
         self.minor_version = minor_version  # type: str
         self.role = role  # type: str
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeMultiZoneClusterResponseBodyMultiZoneInstanceModelsMultiZoneInstanceModel, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.hdfs_minor_version is not None:
+            result['HdfsMinorVersion'] = self.hdfs_minor_version
         if self.ins_name is not None:
             result['InsName'] = self.ins_name
+        if self.is_hdfs_latest_version is not None:
+            result['IsHdfsLatestVersion'] = self.is_hdfs_latest_version
         if self.is_latest_version is not None:
             result['IsLatestVersion'] = self.is_latest_version
+        if self.latest_hdfs_minor_version is not None:
+            result['LatestHdfsMinorVersion'] = self.latest_hdfs_minor_version
+        if self.latest_minor_version is not None:
+            result['LatestMinorVersion'] = self.latest_minor_version
         if self.minor_version is not None:
             result['MinorVersion'] = self.minor_version
         if self.role is not None:
             result['Role'] = self.role
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('HdfsMinorVersion') is not None:
+            self.hdfs_minor_version = m.get('HdfsMinorVersion')
         if m.get('InsName') is not None:
             self.ins_name = m.get('InsName')
+        if m.get('IsHdfsLatestVersion') is not None:
+            self.is_hdfs_latest_version = m.get('IsHdfsLatestVersion')
         if m.get('IsLatestVersion') is not None:
             self.is_latest_version = m.get('IsLatestVersion')
+        if m.get('LatestHdfsMinorVersion') is not None:
+            self.latest_hdfs_minor_version = m.get('LatestHdfsMinorVersion')
+        if m.get('LatestMinorVersion') is not None:
+            self.latest_minor_version = m.get('LatestMinorVersion')
         if m.get('MinorVersion') is not None:
             self.minor_version = m.get('MinorVersion')
         if m.get('Role') is not None:
             self.role = m.get('Role')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
@@ -8214,29 +8514,30 @@
                 temp_model = DescribeMultiZoneClusterResponseBodyTagsTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeMultiZoneClusterResponseBody(TeaModel):
     def __init__(self, arbiter_vswitch_ids=None, arbiter_zone_id=None, auto_renewal=None, cluster_id=None,
-                 cluster_name=None, core_disk_count=None, core_disk_size=None, core_disk_type=None, core_instance_type=None,
-                 core_node_count=None, created_time=None, created_time_utc=None, duration=None, encryption_key=None,
-                 encryption_type=None, engine=None, expire_time=None, expire_time_utc=None, instance_id=None, instance_name=None,
-                 is_deletion_protection=None, log_disk_count=None, log_disk_size=None, log_disk_type=None, log_instance_type=None,
-                 log_node_count=None, maintain_end_time=None, maintain_start_time=None, major_version=None, master_disk_size=None,
-                 master_disk_type=None, master_instance_type=None, master_node_count=None, module_id=None,
+                 cluster_name=None, cold_storage_size=None, core_disk_count=None, core_disk_size=None, core_disk_type=None,
+                 core_instance_type=None, core_node_count=None, created_time=None, created_time_utc=None, duration=None,
+                 encryption_key=None, encryption_type=None, engine=None, expire_time=None, expire_time_utc=None, instance_id=None,
+                 instance_name=None, is_deletion_protection=None, log_disk_count=None, log_disk_size=None, log_disk_type=None,
+                 log_instance_type=None, log_node_count=None, maintain_end_time=None, maintain_start_time=None, major_version=None,
+                 master_disk_size=None, master_disk_type=None, master_instance_type=None, master_node_count=None, module_id=None,
                  module_stack_version=None, multi_zone_combination=None, multi_zone_instance_models=None, network_type=None,
                  parent_id=None, pay_type=None, primary_vswitch_ids=None, primary_zone_id=None, region_id=None,
                  request_id=None, resource_group_id=None, standby_vswitch_ids=None, standby_zone_id=None, status=None,
                  tags=None, vpc_id=None):
         self.arbiter_vswitch_ids = arbiter_vswitch_ids  # type: str
         self.arbiter_zone_id = arbiter_zone_id  # type: str
         self.auto_renewal = auto_renewal  # type: bool
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
+        self.cold_storage_size = cold_storage_size  # type: int
         self.core_disk_count = core_disk_count  # type: str
         self.core_disk_size = core_disk_size  # type: int
         self.core_disk_type = core_disk_type  # type: str
         self.core_instance_type = core_instance_type  # type: str
         self.core_node_count = core_node_count  # type: int
         self.created_time = created_time  # type: str
         self.created_time_utc = created_time_utc  # type: str
@@ -8297,14 +8598,16 @@
             result['ArbiterZoneId'] = self.arbiter_zone_id
         if self.auto_renewal is not None:
             result['AutoRenewal'] = self.auto_renewal
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.cluster_name is not None:
             result['ClusterName'] = self.cluster_name
+        if self.cold_storage_size is not None:
+            result['ColdStorageSize'] = self.cold_storage_size
         if self.core_disk_count is not None:
             result['CoreDiskCount'] = self.core_disk_count
         if self.core_disk_size is not None:
             result['CoreDiskSize'] = self.core_disk_size
         if self.core_disk_type is not None:
             result['CoreDiskType'] = self.core_disk_type
         if self.core_instance_type is not None:
@@ -8401,14 +8704,16 @@
             self.arbiter_zone_id = m.get('ArbiterZoneId')
         if m.get('AutoRenewal') is not None:
             self.auto_renewal = m.get('AutoRenewal')
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('ClusterName') is not None:
             self.cluster_name = m.get('ClusterName')
+        if m.get('ColdStorageSize') is not None:
+            self.cold_storage_size = m.get('ColdStorageSize')
         if m.get('CoreDiskCount') is not None:
             self.core_disk_count = m.get('CoreDiskCount')
         if m.get('CoreDiskSize') is not None:
             self.core_disk_size = m.get('CoreDiskSize')
         if m.get('CoreDiskType') is not None:
             self.core_disk_type = m.get('CoreDiskType')
         if m.get('CoreInstanceType') is not None:
@@ -8497,40 +8802,46 @@
             self.tags = temp_model.from_map(m['Tags'])
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeMultiZoneClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeMultiZoneClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeMultiZoneClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeMultiZoneClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRecoverableTimeRangeRequest(TeaModel):
@@ -8588,40 +8899,46 @@
             self.time_begin = m.get('TimeBegin')
         if m.get('TimeEnd') is not None:
             self.time_end = m.get('TimeEnd')
         return self
 
 
 class DescribeRecoverableTimeRangeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRecoverableTimeRangeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRecoverableTimeRangeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRecoverableTimeRangeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRegionsRequest(TeaModel):
@@ -8810,40 +9127,46 @@
             self.regions = temp_model.from_map(m['Regions'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class DescribeRegionsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRegionsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRegionsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRestoreFullDetailsRequest(TeaModel):
@@ -9067,40 +9390,46 @@
         if m.get('RestoreFull') is not None:
             temp_model = DescribeRestoreFullDetailsResponseBodyRestoreFull()
             self.restore_full = temp_model.from_map(m['RestoreFull'])
         return self
 
 
 class DescribeRestoreFullDetailsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRestoreFullDetailsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRestoreFullDetailsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRestoreFullDetailsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRestoreIncrDetailRequest(TeaModel):
@@ -9215,40 +9544,46 @@
         if m.get('RestoreIncrDetail') is not None:
             temp_model = DescribeRestoreIncrDetailResponseBodyRestoreIncrDetail()
             self.restore_incr_detail = temp_model.from_map(m['RestoreIncrDetail'])
         return self
 
 
 class DescribeRestoreIncrDetailResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRestoreIncrDetailResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRestoreIncrDetailResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRestoreIncrDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRestoreSchemaDetailsRequest(TeaModel):
@@ -9446,40 +9781,46 @@
         if m.get('RestoreSchema') is not None:
             temp_model = DescribeRestoreSchemaDetailsResponseBodyRestoreSchema()
             self.restore_schema = temp_model.from_map(m['RestoreSchema'])
         return self
 
 
 class DescribeRestoreSchemaDetailsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRestoreSchemaDetailsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRestoreSchemaDetailsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRestoreSchemaDetailsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRestoreSummaryRequest(TeaModel):
@@ -9657,40 +9998,46 @@
             self.rescords = temp_model.from_map(m['Rescords'])
         if m.get('Total') is not None:
             self.total = m.get('Total')
         return self
 
 
 class DescribeRestoreSummaryResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRestoreSummaryResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRestoreSummaryResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRestoreSummaryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRestoreTablesRequest(TeaModel):
@@ -10194,40 +10541,46 @@
         if m.get('Tables') is not None:
             temp_model = DescribeRestoreTablesResponseBodyTables()
             self.tables = temp_model.from_map(m['Tables'])
         return self
 
 
 class DescribeRestoreTablesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRestoreTablesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRestoreTablesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRestoreTablesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSecurityGroupsRequest(TeaModel):
@@ -10306,40 +10659,46 @@
         if m.get('SecurityGroupIds') is not None:
             temp_model = DescribeSecurityGroupsResponseBodySecurityGroupIds()
             self.security_group_ids = temp_model.from_map(m['SecurityGroupIds'])
         return self
 
 
 class DescribeSecurityGroupsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeSecurityGroupsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeSecurityGroupsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSecurityGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeServerlessClusterRequest(TeaModel):
@@ -10521,40 +10880,46 @@
             self.vpc_id = m.get('VpcId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
 class DescribeServerlessClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeServerlessClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeServerlessClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeServerlessClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSubDomainRequest(TeaModel):
@@ -10612,40 +10977,46 @@
             self.request_id = m.get('RequestId')
         if m.get('SubDomain') is not None:
             self.sub_domain = m.get('SubDomain')
         return self
 
 
 class DescribeSubDomainResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeSubDomainResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeSubDomainResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSubDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableHBaseueBackupRequest(TeaModel):
@@ -10718,40 +11089,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class EnableHBaseueBackupResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: EnableHBaseueBackupResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(EnableHBaseueBackupResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableHBaseueBackupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableHBaseueModuleRequest(TeaModel):
@@ -10897,40 +11274,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class EnableHBaseueModuleResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: EnableHBaseueModuleResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(EnableHBaseueModuleResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableHBaseueModuleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EvaluateMultiZoneResourceRequest(TeaModel):
@@ -11123,40 +11506,46 @@
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class EvaluateMultiZoneResourceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: EvaluateMultiZoneResourceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(EvaluateMultiZoneResourceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EvaluateMultiZoneResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetMultimodeCmsUrlRequest(TeaModel):
@@ -11219,40 +11608,46 @@
             self.multimod_cms_url = m.get('MultimodCmsUrl')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class GetMultimodeCmsUrlResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: GetMultimodeCmsUrlResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetMultimodeCmsUrlResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetMultimodeCmsUrlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListHBaseInstancesRequest(TeaModel):
@@ -11373,40 +11768,46 @@
             self.instances = temp_model.from_map(m['Instances'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ListHBaseInstancesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ListHBaseInstancesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListHBaseInstancesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListHBaseInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstanceServiceConfigHistoriesRequest(TeaModel):
@@ -11563,40 +11964,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalRecordCount') is not None:
             self.total_record_count = m.get('TotalRecordCount')
         return self
 
 
 class ListInstanceServiceConfigHistoriesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceServiceConfigHistoriesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceServiceConfigHistoriesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListInstanceServiceConfigHistoriesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListInstanceServiceConfigurationsRequest(TeaModel):
@@ -11764,40 +12171,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalRecordCount') is not None:
             self.total_record_count = m.get('TotalRecordCount')
         return self
 
 
 class ListInstanceServiceConfigurationsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ListInstanceServiceConfigurationsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstanceServiceConfigurationsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListInstanceServiceConfigurationsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTagResourcesRequestTag(TeaModel):
@@ -11980,40 +12393,46 @@
         if m.get('TagResources') is not None:
             temp_model = ListTagResourcesResponseBodyTagResources()
             self.tag_resources = temp_model.from_map(m['TagResources'])
         return self
 
 
 class ListTagResourcesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ListTagResourcesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListTagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListTagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTagsRequest(TeaModel):
@@ -12129,40 +12548,46 @@
         if m.get('Tags') is not None:
             temp_model = ListTagsResponseBodyTags()
             self.tags = temp_model.from_map(m['Tags'])
         return self
 
 
 class ListTagsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ListTagsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListTagsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListTagsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyActiveOperationTasksRequest(TeaModel):
@@ -12251,40 +12676,46 @@
             self.ids = m.get('Ids')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyActiveOperationTasksResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyActiveOperationTasksResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyActiveOperationTasksResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyActiveOperationTasksResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyBackupPlanConfigRequest(TeaModel):
@@ -12353,40 +12784,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyBackupPlanConfigResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyBackupPlanConfigResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyBackupPlanConfigResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyBackupPlanConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyBackupPolicyRequest(TeaModel):
@@ -12455,40 +12892,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyBackupPolicyResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyBackupPolicyResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyBackupPolicyResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyBackupPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyClusterDeletionProtectionRequest(TeaModel):
@@ -12541,40 +12984,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyClusterDeletionProtectionResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyClusterDeletionProtectionResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyClusterDeletionProtectionResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyClusterDeletionProtectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDiskWarningLineRequest(TeaModel):
@@ -12627,40 +13076,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyDiskWarningLineResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyDiskWarningLineResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyDiskWarningLineResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDiskWarningLineResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceMaintainTimeRequest(TeaModel):
@@ -12718,40 +13173,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyInstanceMaintainTimeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyInstanceMaintainTimeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyInstanceMaintainTimeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceMaintainTimeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceNameRequest(TeaModel):
@@ -12819,40 +13280,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyInstanceNameResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyInstanceNameResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyInstanceNameResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceNameResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceServiceConfigRequest(TeaModel):
@@ -12920,40 +13387,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyInstanceServiceConfigResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyInstanceServiceConfigResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyInstanceServiceConfigResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceServiceConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyInstanceTypeRequest(TeaModel):
@@ -13016,40 +13489,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyInstanceTypeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyInstanceTypeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyInstanceTypeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyIpWhitelistRequest(TeaModel):
@@ -13112,40 +13591,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyIpWhitelistResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyIpWhitelistResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyIpWhitelistResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyIpWhitelistResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyMultiZoneClusterNodeTypeRequest(TeaModel):
@@ -13213,40 +13698,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyMultiZoneClusterNodeTypeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyMultiZoneClusterNodeTypeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyMultiZoneClusterNodeTypeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyMultiZoneClusterNodeTypeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifySecurityGroupsRequest(TeaModel):
@@ -13299,40 +13790,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifySecurityGroupsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifySecurityGroupsResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifySecurityGroupsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifySecurityGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyUIAccountPasswordRequest(TeaModel):
@@ -13390,40 +13887,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ModifyUIAccountPasswordResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ModifyUIAccountPasswordResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ModifyUIAccountPasswordResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyUIAccountPasswordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class MoveResourceGroupRequest(TeaModel):
@@ -13476,40 +13979,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class MoveResourceGroupResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: MoveResourceGroupResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(MoveResourceGroupResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = MoveResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class OpenBackupRequest(TeaModel):
@@ -13557,40 +14066,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class OpenBackupResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: OpenBackupResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(OpenBackupResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = OpenBackupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class PurgeInstanceRequest(TeaModel):
@@ -13638,40 +14153,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class PurgeInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: PurgeInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(PurgeInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PurgeInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryHBaseHaDBRequest(TeaModel):
@@ -13763,14 +14284,15 @@
                 self.ha_slb_conn.append(temp_model.from_map(k))
         return self
 
 
 class QueryHBaseHaDBResponseBodyClusterListCluster(TeaModel):
     def __init__(self, active_name=None, bds_name=None, ha_name=None, ha_slb_conn_list=None, standby_name=None):
         self.active_name = active_name  # type: str
+        # bdsId
         self.bds_name = bds_name  # type: str
         self.ha_name = ha_name  # type: str
         self.ha_slb_conn_list = ha_slb_conn_list  # type: QueryHBaseHaDBResponseBodyClusterListClusterHaSlbConnList
         self.standby_name = standby_name  # type: str
 
     def validate(self):
         if self.ha_slb_conn_list:
@@ -13885,40 +14407,46 @@
             self.request_id = m.get('RequestId')
         if m.get('TotalCount') is not None:
             self.total_count = m.get('TotalCount')
         return self
 
 
 class QueryHBaseHaDBResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: QueryHBaseHaDBResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(QueryHBaseHaDBResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryHBaseHaDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryXpackRelateDBRequest(TeaModel):
@@ -14070,40 +14598,46 @@
             self.cluster_list = temp_model.from_map(m['ClusterList'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class QueryXpackRelateDBResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: QueryXpackRelateDBResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(QueryXpackRelateDBResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryXpackRelateDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RelateDbForHBaseHaRequest(TeaModel):
@@ -14255,40 +14789,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class RelateDbForHBaseHaResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: RelateDbForHBaseHaResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(RelateDbForHBaseHaResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RelateDbForHBaseHaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ReleasePublicNetworkAddressRequest(TeaModel):
@@ -14336,40 +14876,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ReleasePublicNetworkAddressResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ReleasePublicNetworkAddressResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ReleasePublicNetworkAddressResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ReleasePublicNetworkAddressResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RenewInstanceRequest(TeaModel):
@@ -14432,40 +14978,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class RenewInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: RenewInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(RenewInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RenewInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResizeColdStorageSizeRequest(TeaModel):
@@ -14523,40 +15075,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ResizeColdStorageSizeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResizeColdStorageSizeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResizeColdStorageSizeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResizeColdStorageSizeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResizeDiskSizeRequest(TeaModel):
@@ -14614,40 +15172,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ResizeDiskSizeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResizeDiskSizeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResizeDiskSizeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResizeDiskSizeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResizeMultiZoneClusterDiskSizeRequest(TeaModel):
@@ -14710,40 +15274,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ResizeMultiZoneClusterDiskSizeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResizeMultiZoneClusterDiskSizeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResizeMultiZoneClusterDiskSizeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResizeMultiZoneClusterDiskSizeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResizeMultiZoneClusterNodeCountRequest(TeaModel):
@@ -14832,40 +15402,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ResizeMultiZoneClusterNodeCountResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResizeMultiZoneClusterNodeCountResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResizeMultiZoneClusterNodeCountResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResizeMultiZoneClusterNodeCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResizeNodeCountRequest(TeaModel):
@@ -14933,40 +15509,46 @@
             self.order_id = m.get('OrderId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class ResizeNodeCountResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: ResizeNodeCountResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ResizeNodeCountResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResizeNodeCountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RestartInstanceRequest(TeaModel):
@@ -15019,40 +15601,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class RestartInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: RestartInstanceResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(RestartInstanceResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RestartInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SwitchHbaseHaSlbRequest(TeaModel):
@@ -15115,46 +15703,149 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class SwitchHbaseHaSlbResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: SwitchHbaseHaSlbResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(SwitchHbaseHaSlbResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SwitchHbaseHaSlbResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SwitchServiceRequest(TeaModel):
+    def __init__(self, cluster_id=None, operate=None, service_name=None):
+        self.cluster_id = cluster_id  # type: str
+        self.operate = operate  # type: str
+        self.service_name = service_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SwitchServiceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cluster_id is not None:
+            result['ClusterId'] = self.cluster_id
+        if self.operate is not None:
+            result['Operate'] = self.operate
+        if self.service_name is not None:
+            result['ServiceName'] = self.service_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClusterId') is not None:
+            self.cluster_id = m.get('ClusterId')
+        if m.get('Operate') is not None:
+            self.operate = m.get('Operate')
+        if m.get('ServiceName') is not None:
+            self.service_name = m.get('ServiceName')
+        return self
+
+
+class SwitchServiceResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SwitchServiceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SwitchServiceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SwitchServiceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SwitchServiceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SwitchServiceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class TagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
         self.key = key  # type: str
         self.value = value  # type: str
 
     def validate(self):
         pass
@@ -15243,40 +15934,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class TagResourcesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: TagResourcesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(TagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UnTagResourcesRequest(TeaModel):
@@ -15339,40 +16036,46 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class UnTagResourcesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: UnTagResourcesResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UnTagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UnTagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpgradeMinorVersionRequest(TeaModel):
@@ -15430,40 +16133,46 @@
             self.request_id = m.get('RequestId')
         if m.get('UpgradingComponents') is not None:
             self.upgrading_components = m.get('UpgradingComponents')
         return self
 
 
 class UpgradeMinorVersionResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: UpgradeMinorVersionResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpgradeMinorVersionResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpgradeMinorVersionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpgradeMultiZoneClusterRequest(TeaModel):
@@ -15542,40 +16251,46 @@
             self.request_id = m.get('RequestId')
         if m.get('UpgradingComponents') is not None:
             self.upgrading_components = m.get('UpgradingComponents')
         return self
 
 
 class UpgradeMultiZoneClusterResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: UpgradeMultiZoneClusterResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpgradeMultiZoneClusterResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpgradeMultiZoneClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class XpackRelateDBRequest(TeaModel):
@@ -15633,39 +16348,45 @@
         m = m or dict()
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
 class XpackRelateDBResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: XpackRelateDBResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(XpackRelateDBResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = XpackRelateDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/alibabacloud_hbase20190101_py2.egg-info/PKG-INFO` & `alibabacloud_hbase20190101_py2-2.9.11/alibabacloud_hbase20190101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-hbase20190101-py2
-Version: 2.9.10
+Version: 2.9.11
 Summary: Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hbase20190101_py2-2.9.10/setup.py` & `alibabacloud_hbase20190101_py2-2.9.11/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hbase20190101_py2.
 
-Created on 14/04/2022
+Created on 15/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hbase20190101"
 NAME = "alibabacloud_hbase20190101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.1, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

