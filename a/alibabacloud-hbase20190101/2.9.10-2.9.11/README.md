# Comparing `tmp/alibabacloud_hbase20190101-2.9.10.tar.gz` & `tmp/alibabacloud_hbase20190101-2.9.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_hbase20190101-2.9.10.tar", last modified: Thu Apr 14 07:27:05 2022, max compression
+gzip compressed data, was "dist/alibabacloud_hbase20190101-2.9.11.tar", last modified: Tue Aug 15 08:42:48 2023, max compression
```

## Comparing `alibabacloud_hbase20190101-2.9.10.tar` & `alibabacloud_hbase20190101-2.9.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/
--rw-r--r--   0 root         (0) root         (0)       87 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/
--rw-r--r--   0 root         (0) root         (0)       22 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   331145 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/client.py
--rw-r--r--   0 root         (0) root         (0)   576733 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2633 2022-04-14 07:27:05.000000 alibabacloud_hbase20190101-2.9.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   332714 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/client.py
+-rw-r--r--   0 root         (0) root         (0)   613784 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-08-15 08:42:48.000000 alibabacloud_hbase20190101-2.9.11/setup.py
```

### Comparing `alibabacloud_hbase20190101-2.9.10/LICENSE` & `alibabacloud_hbase20190101-2.9.11/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101-2.9.10/PKG-INFO` & `alibabacloud_hbase20190101-2.9.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_hbase20190101
-Version: 2.9.10
+Version: 2.9.11
 Summary: Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hbase20190101-2.9.10/README-CN.md` & `alibabacloud_hbase20190101-2.9.11/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101-2.9.10/README.md` & `alibabacloud_hbase20190101-2.9.11/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/client.py` & `alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,57 +19,26 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
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
 
     def get_endpoint(
         self,
         product_id: str,
@@ -781,14 +750,16 @@
     ) -> hbase_20190101_models.CreateGlobalResourceResponse:
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
@@ -815,14 +786,16 @@
     ) -> hbase_20190101_models.CreateGlobalResourceResponse:
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
@@ -1435,14 +1408,16 @@
         request: hbase_20190101_models.DeleteGlobalResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> hbase_20190101_models.DeleteGlobalResourceResponse:
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
@@ -1467,14 +1442,16 @@
         request: hbase_20190101_models.DeleteGlobalResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> hbase_20190101_models.DeleteGlobalResourceResponse:
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
@@ -7656,14 +7633,92 @@
     async def switch_hbase_ha_slb_async(
         self,
         request: hbase_20190101_models.SwitchHbaseHaSlbRequest,
     ) -> hbase_20190101_models.SwitchHbaseHaSlbResponse:
         runtime = util_models.RuntimeOptions()
         return await self.switch_hbase_ha_slb_with_options_async(request, runtime)
 
+    def switch_service_with_options(
+        self,
+        request: hbase_20190101_models.SwitchServiceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> hbase_20190101_models.SwitchServiceResponse:
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
+    async def switch_service_with_options_async(
+        self,
+        request: hbase_20190101_models.SwitchServiceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> hbase_20190101_models.SwitchServiceResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def switch_service(
+        self,
+        request: hbase_20190101_models.SwitchServiceRequest,
+    ) -> hbase_20190101_models.SwitchServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.switch_service_with_options(request, runtime)
+
+    async def switch_service_async(
+        self,
+        request: hbase_20190101_models.SwitchServiceRequest,
+    ) -> hbase_20190101_models.SwitchServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.switch_service_with_options_async(request, runtime)
+
     def tag_resources_with_options(
         self,
         request: hbase_20190101_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> hbase_20190101_models.TagResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101/models.py` & `alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,41 +70,48 @@
         return self
 
 
 class AddUserHdfsInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: AddUserHdfsInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -167,41 +174,48 @@
         return self
 
 
 class AllocatePublicNetworkAddressResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: AllocatePublicNetworkAddressResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -294,41 +308,48 @@
         return self
 
 
 class CancelActiveOperationTasksResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CancelActiveOperationTasksResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -467,41 +488,48 @@
         return self
 
 
 class CheckComponentsVersionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CheckComponentsVersionResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -558,41 +586,48 @@
         return self
 
 
 class CloseBackupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CloseBackupResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -673,41 +708,48 @@
         return self
 
 
 class ConvertInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ConvertInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -764,41 +806,48 @@
         return self
 
 
 class CreateBackupPlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateBackupPlanResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -987,57 +1036,66 @@
         return self
 
 
 class CreateClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         client_token: str = None,
         cluster_id: str = None,
+        region_id: str = None,
         resource_name: str = None,
         resource_type: str = None,
     ):
         self.client_token = client_token
         self.cluster_id = cluster_id
+        self.region_id = region_id
         self.resource_name = resource_name
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1046,26 +1104,30 @@
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
 
     def from_map(self, m: dict = None):
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
 
 
@@ -1096,41 +1158,48 @@
         return self
 
 
 class CreateGlobalResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateGlobalResourceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1199,41 +1268,48 @@
         return self
 
 
 class CreateHBaseSlbServerResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateHBaseSlbServerResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1314,41 +1390,48 @@
         return self
 
 
 class CreateHbaseHaSlbResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateHbaseHaSlbResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1585,41 +1668,48 @@
         return self
 
 
 class CreateMultiZoneClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateMultiZoneClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1706,41 +1796,48 @@
         return self
 
 
 class CreateRestorePlanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateRestorePlanResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -1917,79 +2014,92 @@
         return self
 
 
 class CreateServerlessClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateServerlessClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         cluster_id: str = None,
+        region_id: str = None,
         resource_name: str = None,
         resource_type: str = None,
     ):
         self.cluster_id = cluster_id
+        self.region_id = region_id
         self.resource_name = resource_name
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
 
 
@@ -2020,41 +2130,48 @@
         return self
 
 
 class DeleteGlobalResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteGlobalResourceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2117,41 +2234,48 @@
         return self
 
 
 class DeleteHBaseHaDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteHBaseHaDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2214,41 +2338,48 @@
         return self
 
 
 class DeleteHBaseSlbServerResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteHBaseSlbServerResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2317,41 +2448,48 @@
         return self
 
 
 class DeleteHbaseHaSlbResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteHbaseHaSlbResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2414,41 +2552,48 @@
         return self
 
 
 class DeleteInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2511,41 +2656,48 @@
         return self
 
 
 class DeleteMultiZoneClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteMultiZoneClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2614,41 +2766,48 @@
         return self
 
 
 class DeleteServerlessClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteServerlessClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2711,41 +2870,48 @@
         return self
 
 
 class DeleteUserHdfsInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteUserHdfsInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -2891,41 +3057,48 @@
         return self
 
 
 class DescribeActiveOperationTaskTypeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeActiveOperationTaskTypeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -3281,41 +3454,48 @@
         return self
 
 
 class DescribeActiveOperationTasksResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeActiveOperationTasksResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4041,41 +4221,48 @@
         return self
 
 
 class DescribeAvailableResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeAvailableResourceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4185,41 +4372,48 @@
         return self
 
 
 class DescribeBackupPlanConfigResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupPlanConfigResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4306,41 +4500,48 @@
         return self
 
 
 class DescribeBackupPolicyResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupPolicyResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4415,41 +4616,48 @@
         return self
 
 
 class DescribeBackupStatusResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupStatusResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -4749,41 +4957,48 @@
         return self
 
 
 class DescribeBackupSummaryResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupSummaryResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -5024,41 +5239,48 @@
         return self
 
 
 class DescribeBackupTablesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupTablesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -5317,41 +5539,48 @@
         return self
 
 
 class DescribeBackupsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeBackupsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -5858,41 +6087,48 @@
         return self
 
 
 class DescribeClusterConnectionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeClusterConnectionResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -5991,41 +6227,48 @@
         return self
 
 
 class DescribeColdStorageResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeColdStorageResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -6088,41 +6331,48 @@
         return self
 
 
 class DescribeDBInstanceUsageResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDBInstanceUsageResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -6345,41 +6595,48 @@
         return self
 
 
 class DescribeDeletedInstancesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDeletedInstancesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -6442,41 +6699,48 @@
         return self
 
 
 class DescribeDiskWarningLineResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDiskWarningLineResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -6645,41 +6909,48 @@
         return self
 
 
 class DescribeEndpointsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeEndpointsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -6819,25 +7090,27 @@
         core_disk_size: int = None,
         core_disk_type: str = None,
         core_instance_type: str = None,
         core_node_count: int = None,
         created_time: str = None,
         created_time_utc: str = None,
         duration: int = None,
+        enable_hbase_proxy: bool = None,
         encryption_key: str = None,
         encryption_type: str = None,
         engine: str = None,
         expire_time: str = None,
         expire_time_utc: str = None,
         instance_id: str = None,
         instance_name: str = None,
         is_deletion_protection: bool = None,
         is_ha: bool = None,
         is_latest_version: bool = None,
         is_multi_model: bool = None,
+        lproxy_minor_version: str = None,
         maintain_end_time: str = None,
         maintain_start_time: str = None,
         major_version: str = None,
         master_disk_size: int = None,
         master_disk_type: str = None,
         master_instance_type: str = None,
         master_node_count: int = None,
@@ -6871,25 +7144,27 @@
         self.core_disk_size = core_disk_size
         self.core_disk_type = core_disk_type
         self.core_instance_type = core_instance_type
         self.core_node_count = core_node_count
         self.created_time = created_time
         self.created_time_utc = created_time_utc
         self.duration = duration
+        self.enable_hbase_proxy = enable_hbase_proxy
         self.encryption_key = encryption_key
         self.encryption_type = encryption_type
         self.engine = engine
         self.expire_time = expire_time
         self.expire_time_utc = expire_time_utc
         self.instance_id = instance_id
         self.instance_name = instance_name
         self.is_deletion_protection = is_deletion_protection
         self.is_ha = is_ha
         self.is_latest_version = is_latest_version
         self.is_multi_model = is_multi_model
+        self.lproxy_minor_version = lproxy_minor_version
         self.maintain_end_time = maintain_end_time
         self.maintain_start_time = maintain_start_time
         self.major_version = major_version
         self.master_disk_size = master_disk_size
         self.master_disk_type = master_disk_type
         self.master_instance_type = master_instance_type
         self.master_node_count = master_node_count
@@ -6951,14 +7226,16 @@
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
@@ -6973,14 +7250,16 @@
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
@@ -7057,14 +7336,16 @@
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
@@ -7079,14 +7360,16 @@
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
@@ -7136,41 +7419,48 @@
         return self
 
 
 class DescribeInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -7309,41 +7599,48 @@
         return self
 
 
 class DescribeInstanceTypeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeInstanceTypeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -7863,41 +8160,48 @@
         return self
 
 
 class DescribeInstancesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeInstancesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -8065,41 +8369,48 @@
         return self
 
 
 class DescribeIpWhitelistResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeIpWhitelistResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -8343,41 +8654,48 @@
         return self
 
 
 class DescribeMultiZoneAvailableRegionsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeMultiZoneAvailableRegionsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -9079,41 +9397,48 @@
         return self
 
 
 class DescribeMultiZoneAvailableResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeMultiZoneAvailableResourceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -9142,53 +9467,77 @@
             self.cluster_id = m.get('ClusterId')
         return self
 
 
 class DescribeMultiZoneClusterResponseBodyMultiZoneInstanceModelsMultiZoneInstanceModel(TeaModel):
     def __init__(
         self,
+        hdfs_minor_version: str = None,
         ins_name: str = None,
+        is_hdfs_latest_version: str = None,
         is_latest_version: bool = None,
+        latest_hdfs_minor_version: str = None,
+        latest_minor_version: str = None,
         minor_version: str = None,
         role: str = None,
         status: str = None,
     ):
+        self.hdfs_minor_version = hdfs_minor_version
         self.ins_name = ins_name
+        self.is_hdfs_latest_version = is_hdfs_latest_version
         self.is_latest_version = is_latest_version
+        self.latest_hdfs_minor_version = latest_hdfs_minor_version
+        self.latest_minor_version = latest_minor_version
         self.minor_version = minor_version
         self.role = role
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -9301,14 +9650,15 @@
     def __init__(
         self,
         arbiter_vswitch_ids: str = None,
         arbiter_zone_id: str = None,
         auto_renewal: bool = None,
         cluster_id: str = None,
         cluster_name: str = None,
+        cold_storage_size: int = None,
         core_disk_count: str = None,
         core_disk_size: int = None,
         core_disk_type: str = None,
         core_instance_type: str = None,
         core_node_count: int = None,
         created_time: str = None,
         created_time_utc: str = None,
@@ -9352,14 +9702,15 @@
         vpc_id: str = None,
     ):
         self.arbiter_vswitch_ids = arbiter_vswitch_ids
         self.arbiter_zone_id = arbiter_zone_id
         self.auto_renewal = auto_renewal
         self.cluster_id = cluster_id
         self.cluster_name = cluster_name
+        self.cold_storage_size = cold_storage_size
         self.core_disk_count = core_disk_count
         self.core_disk_size = core_disk_size
         self.core_disk_type = core_disk_type
         self.core_instance_type = core_instance_type
         self.core_node_count = core_node_count
         self.created_time = created_time
         self.created_time_utc = created_time_utc
@@ -9420,14 +9771,16 @@
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
@@ -9524,14 +9877,16 @@
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
@@ -9623,41 +9978,48 @@
         return self
 
 
 class DescribeMultiZoneClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeMultiZoneClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -9726,41 +10088,48 @@
         return self
 
 
 class DescribeRecoverableTimeRangeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRecoverableTimeRangeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -9975,41 +10344,48 @@
         return self
 
 
 class DescribeRegionsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRegionsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -10267,41 +10643,48 @@
         return self
 
 
 class DescribeRestoreFullDetailsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRestoreFullDetailsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -10435,41 +10818,48 @@
         return self
 
 
 class DescribeRestoreIncrDetailResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRestoreIncrDetailResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -10697,41 +11087,48 @@
         return self
 
 
 class DescribeRestoreSchemaDetailsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRestoreSchemaDetailsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -10936,41 +11333,48 @@
         return self
 
 
 class DescribeRestoreSummaryResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRestoreSummaryResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -11544,41 +11948,48 @@
         return self
 
 
 class DescribeRestoreTablesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRestoreTablesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -11670,41 +12081,48 @@
         return self
 
 
 class DescribeSecurityGroupsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeSecurityGroupsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -11917,41 +12335,48 @@
         return self
 
 
 class DescribeServerlessClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeServerlessClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12020,41 +12445,48 @@
         return self
 
 
 class DescribeSubDomainResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeSubDomainResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12141,41 +12573,48 @@
         return self
 
 
 class EnableHBaseueBackupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: EnableHBaseueBackupResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12346,41 +12785,48 @@
         return self
 
 
 class EnableHBaseueModuleResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: EnableHBaseueModuleResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12605,41 +13051,48 @@
         return self
 
 
 class EvaluateMultiZoneResourceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: EvaluateMultiZoneResourceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12714,41 +13167,48 @@
         return self
 
 
 class GetMultimodeCmsUrlResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: GetMultimodeCmsUrlResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -12887,41 +13347,48 @@
         return self
 
 
 class ListHBaseInstancesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ListHBaseInstancesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13102,41 +13569,48 @@
         return self
 
 
 class ListInstanceServiceConfigHistoriesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ListInstanceServiceConfigHistoriesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13329,41 +13803,48 @@
         return self
 
 
 class ListInstanceServiceConfigurationsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ListInstanceServiceConfigurationsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13573,41 +14054,48 @@
         return self
 
 
 class ListTagResourcesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ListTagResourcesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13740,41 +14228,48 @@
         return self
 
 
 class ListTagsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ListTagsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13879,41 +14374,48 @@
         return self
 
 
 class ModifyActiveOperationTasksResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyActiveOperationTasksResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -13994,41 +14496,48 @@
         return self
 
 
 class ModifyBackupPlanConfigResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyBackupPlanConfigResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14109,41 +14618,48 @@
         return self
 
 
 class ModifyBackupPolicyResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyBackupPolicyResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14206,41 +14722,48 @@
         return self
 
 
 class ModifyClusterDeletionProtectionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyClusterDeletionProtectionResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14303,41 +14826,48 @@
         return self
 
 
 class ModifyDiskWarningLineResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyDiskWarningLineResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14406,41 +14936,48 @@
         return self
 
 
 class ModifyInstanceMaintainTimeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyInstanceMaintainTimeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14521,41 +15058,48 @@
         return self
 
 
 class ModifyInstanceNameResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyInstanceNameResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14636,41 +15180,48 @@
         return self
 
 
 class ModifyInstanceServiceConfigResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyInstanceServiceConfigResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14745,41 +15296,48 @@
         return self
 
 
 class ModifyInstanceTypeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyInstanceTypeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14854,41 +15412,48 @@
         return self
 
 
 class ModifyIpWhitelistResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyIpWhitelistResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -14969,41 +15534,48 @@
         return self
 
 
 class ModifyMultiZoneClusterNodeTypeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyMultiZoneClusterNodeTypeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15066,41 +15638,48 @@
         return self
 
 
 class ModifySecurityGroupsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifySecurityGroupsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15169,41 +15748,48 @@
         return self
 
 
 class ModifyUIAccountPasswordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyUIAccountPasswordResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15266,41 +15852,48 @@
         return self
 
 
 class MoveResourceGroupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: MoveResourceGroupResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15357,41 +15950,48 @@
         return self
 
 
 class OpenBackupResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: OpenBackupResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15448,41 +16048,48 @@
         return self
 
 
 class PurgeInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: PurgeInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15592,14 +16199,15 @@
         active_name: str = None,
         bds_name: str = None,
         ha_name: str = None,
         ha_slb_conn_list: QueryHBaseHaDBResponseBodyClusterListClusterHaSlbConnList = None,
         standby_name: str = None,
     ):
         self.active_name = active_name
+        # bdsId
         self.bds_name = bds_name
         self.ha_name = ha_name
         self.ha_slb_conn_list = ha_slb_conn_list
         self.standby_name = standby_name
 
     def validate(self):
         if self.ha_slb_conn_list:
@@ -15727,41 +16335,48 @@
         return self
 
 
 class QueryHBaseHaDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: QueryHBaseHaDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -15936,41 +16551,48 @@
         return self
 
 
 class QueryXpackRelateDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: QueryXpackRelateDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16147,41 +16769,48 @@
         return self
 
 
 class RelateDbForHBaseHaResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RelateDbForHBaseHaResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16238,41 +16867,48 @@
         return self
 
 
 class ReleasePublicNetworkAddressResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ReleasePublicNetworkAddressResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16347,41 +16983,48 @@
         return self
 
 
 class RenewInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RenewInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16450,41 +17093,48 @@
         return self
 
 
 class ResizeColdStorageSizeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResizeColdStorageSizeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16553,41 +17203,48 @@
         return self
 
 
 class ResizeDiskSizeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResizeDiskSizeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16662,41 +17319,48 @@
         return self
 
 
 class ResizeMultiZoneClusterDiskSizeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResizeMultiZoneClusterDiskSizeResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16801,41 +17465,48 @@
         return self
 
 
 class ResizeMultiZoneClusterNodeCountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResizeMultiZoneClusterNodeCountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -16916,41 +17587,48 @@
         return self
 
 
 class ResizeNodeCountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ResizeNodeCountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17013,41 +17691,48 @@
         return self
 
 
 class RestartInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RestartInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17122,47 +17807,164 @@
         return self
 
 
 class SwitchHbaseHaSlbResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: SwitchHbaseHaSlbResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        cluster_id: str = None,
+        operate: str = None,
+        service_name: str = None,
+    ):
+        self.cluster_id = cluster_id
+        self.operate = operate
+        self.service_name = service_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SwitchServiceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SwitchServiceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -17266,41 +18068,48 @@
         return self
 
 
 class TagResourcesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: TagResourcesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17375,41 +18184,48 @@
         return self
 
 
 class UnTagResourcesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: UnTagResourcesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17478,41 +18294,48 @@
         return self
 
 
 class UpgradeMinorVersionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: UpgradeMinorVersionResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17605,41 +18428,48 @@
         return self
 
 
 class UpgradeMultiZoneClusterResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: UpgradeMultiZoneClusterResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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
@@ -17708,40 +18538,47 @@
         return self
 
 
 class XpackRelateDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: XpackRelateDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_hbase20190101-2.9.10/alibabacloud_hbase20190101.egg-info/PKG-INFO` & `alibabacloud_hbase20190101-2.9.11/alibabacloud_hbase20190101.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-hbase20190101
-Version: 2.9.10
+Version: 2.9.11
 Summary: Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_hbase20190101-2.9.10/setup.py` & `alibabacloud_hbase20190101-2.9.11/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_hbase20190101.
 
-Created on 14/04/2022
+Created on 15/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_hbase20190101"
 NAME = "alibabacloud_hbase20190101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for Hbase (20190101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

