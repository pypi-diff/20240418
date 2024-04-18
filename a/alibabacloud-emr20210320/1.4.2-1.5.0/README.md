# Comparing `tmp/alibabacloud_emr20210320-1.4.2.tar.gz` & `tmp/alibabacloud_emr20210320-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr20210320-1.4.2.tar", last modified: Tue Mar 26 17:11:10 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr20210320-1.5.0.tar", last modified: Wed Apr 17 17:15:44 2024, max compression
```

## Comparing `alibabacloud_emr20210320-1.4.2.tar` & `alibabacloud_emr20210320-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/
--rw-r--r--   0 root         (0) root         (0)     1251 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   237980 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/client.py
--rw-r--r--   0 root         (0) root         (0)  1638747 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-03-26 17:11:10.000000 alibabacloud_emr20210320-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252698 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/client.py
+-rw-r--r--   0 root         (0) root         (0)  1657374 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-17 17:15:44.000000 alibabacloud_emr20210320-1.5.0/setup.py
```

### Comparing `alibabacloud_emr20210320-1.4.2/ChangeLog.md` & `alibabacloud_emr20210320-1.5.0/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-26 Version: 1.4.2
+- Generated python 2021-03-20 for Emr.
+
 2024-03-15 Version: 1.4.1
 - Update API GetAutoScalingPolicy: update response param.
 
 
 2024-03-14 Version: 1.4.0
 - Support API ListScripts.
 - Delete API GetApmData.
```

### Comparing `alibabacloud_emr20210320-1.4.2/LICENSE` & `alibabacloud_emr20210320-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.4.2/PKG-INFO` & `alibabacloud_emr20210320-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr20210320
-Version: 1.4.2
+Version: 1.5.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320-1.4.2/README-CN.md` & `alibabacloud_emr20210320-1.5.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.4.2/README.md` & `alibabacloud_emr20210320-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/client.py` & `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,14 +394,122 @@
         
         @param request: DecreaseNodesRequest
         @return: DecreaseNodesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.decrease_nodes_with_options_async(request, runtime)
 
+    def delete_api_template_with_options(
+        self,
+        request: emr_20210320_models.DeleteApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.DeleteApiTemplateResponse:
+        """
+        创建集群模板
+        
+        @param request: DeleteApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.DeleteApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_api_template_with_options_async(
+        self,
+        request: emr_20210320_models.DeleteApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.DeleteApiTemplateResponse:
+        """
+        创建集群模板
+        
+        @param request: DeleteApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.DeleteApiTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_api_template(
+        self,
+        request: emr_20210320_models.DeleteApiTemplateRequest,
+    ) -> emr_20210320_models.DeleteApiTemplateResponse:
+        """
+        创建集群模板
+        
+        @param request: DeleteApiTemplateRequest
+        @return: DeleteApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.delete_api_template_with_options(request, runtime)
+
+    async def delete_api_template_async(
+        self,
+        request: emr_20210320_models.DeleteApiTemplateRequest,
+    ) -> emr_20210320_models.DeleteApiTemplateResponse:
+        """
+        创建集群模板
+        
+        @param request: DeleteApiTemplateRequest
+        @return: DeleteApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_api_template_with_options_async(request, runtime)
+
     def delete_cluster_with_options(
         self,
         request: emr_20210320_models.DeleteClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.DeleteClusterResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -468,14 +576,88 @@
     async def delete_cluster_async(
         self,
         request: emr_20210320_models.DeleteClusterRequest,
     ) -> emr_20210320_models.DeleteClusterResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_cluster_with_options_async(request, runtime)
 
+    def get_api_template_with_options(
+        self,
+        request: emr_20210320_models.GetApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.GetApiTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.GetApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_api_template_with_options_async(
+        self,
+        request: emr_20210320_models.GetApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.GetApiTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.GetApiTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_api_template(
+        self,
+        request: emr_20210320_models.GetApiTemplateRequest,
+    ) -> emr_20210320_models.GetApiTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_api_template_with_options(request, runtime)
+
+    async def get_api_template_async(
+        self,
+        request: emr_20210320_models.GetApiTemplateRequest,
+    ) -> emr_20210320_models.GetApiTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_api_template_with_options_async(request, runtime)
+
     def get_application_with_options(
         self,
         request: emr_20210320_models.GetApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.GetApplicationResponse:
         """
         查询应用详情。
@@ -2720,14 +2902,112 @@
     async def join_resource_group_async(
         self,
         request: emr_20210320_models.JoinResourceGroupRequest,
     ) -> emr_20210320_models.JoinResourceGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.join_resource_group_with_options_async(request, runtime)
 
+    def list_api_templates_with_options(
+        self,
+        request: emr_20210320_models.ListApiTemplatesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.ListApiTemplatesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.template_ids):
+            query['TemplateIds'] = request.template_ids
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListApiTemplates',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.ListApiTemplatesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_api_templates_with_options_async(
+        self,
+        request: emr_20210320_models.ListApiTemplatesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.ListApiTemplatesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.template_ids):
+            query['TemplateIds'] = request.template_ids
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListApiTemplates',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.ListApiTemplatesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_api_templates(
+        self,
+        request: emr_20210320_models.ListApiTemplatesRequest,
+    ) -> emr_20210320_models.ListApiTemplatesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_api_templates_with_options(request, runtime)
+
+    async def list_api_templates_async(
+        self,
+        request: emr_20210320_models.ListApiTemplatesRequest,
+    ) -> emr_20210320_models.ListApiTemplatesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_api_templates_with_options_async(request, runtime)
+
     def list_application_configs_with_options(
         self,
         request: emr_20210320_models.ListApplicationConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.ListApplicationConfigsResponse:
         """
         查询应用配置。
@@ -5648,14 +5928,122 @@
     async def remove_auto_scaling_policy_async(
         self,
         request: emr_20210320_models.RemoveAutoScalingPolicyRequest,
     ) -> emr_20210320_models.RemoveAutoScalingPolicyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.remove_auto_scaling_policy_with_options_async(request, runtime)
 
+    def run_api_template_with_options(
+        self,
+        request: emr_20210320_models.RunApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.RunApiTemplateResponse:
+        """
+        执行集群模板
+        
+        @param request: RunApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RunApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RunApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.RunApiTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def run_api_template_with_options_async(
+        self,
+        request: emr_20210320_models.RunApiTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_20210320_models.RunApiTemplateResponse:
+        """
+        执行集群模板
+        
+        @param request: RunApiTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RunApiTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RunApiTemplate',
+            version='2021-03-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_20210320_models.RunApiTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def run_api_template(
+        self,
+        request: emr_20210320_models.RunApiTemplateRequest,
+    ) -> emr_20210320_models.RunApiTemplateResponse:
+        """
+        执行集群模板
+        
+        @param request: RunApiTemplateRequest
+        @return: RunApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.run_api_template_with_options(request, runtime)
+
+    async def run_api_template_async(
+        self,
+        request: emr_20210320_models.RunApiTemplateRequest,
+    ) -> emr_20210320_models.RunApiTemplateResponse:
+        """
+        执行集群模板
+        
+        @param request: RunApiTemplateRequest
+        @return: RunApiTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.run_api_template_with_options_async(request, runtime)
+
     def run_application_action_with_options(
         self,
         request: emr_20210320_models.RunApplicationActionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> emr_20210320_models.RunApplicationActionResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320/models.py` & `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,84 @@
             self.node_pool_id = m.get('NodePoolId')
         if m.get('NodeSelector') is not None:
             temp_model = AckNodeSelector()
             self.node_selector = temp_model.from_map(m['NodeSelector'])
         return self
 
 
+class ApiTemplate(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        content: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        status: str = None,
+        template_id: str = None,
+        template_name: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 模版接口参数。
+        self.content = content
+        # 区域ID。
+        self.region_id = region_id
+        # 资源组ID。
+        self.resource_group_id = resource_group_id
+        # 模板状态。
+        self.status = status
+        # 模板ID。
+        self.template_id = template_id
+        # 模板ID。
+        self.template_name = template_name
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
 class Application(TeaModel):
     def __init__(
         self,
         application_name: str = None,
     ):
         # 应用名称。从EMR控制台集群创建页面可查看到指定发行版的应用名称列表。
         self.application_name = application_name
@@ -7554,14 +7624,138 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DecreaseNodesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteApiTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        template_id: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 区域ID。
+        self.region_id = region_id
+        # 资源组ID。
+        self.resource_group_id = resource_group_id
+        # 集群模板id。
+        self.template_id = template_id
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class DeleteApiTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # 请求ID。
+        self.request_id = request_id
+        self.success = success
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
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DeleteApiTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteApiTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
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
+            temp_model = DeleteApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteClusterRequest(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         region_id: str = None,
     ):
         # The ID of the cluster.
@@ -7665,14 +7859,126 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteClusterResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetApiTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        template_id: str = None,
+    ):
+        # 区域ID。
+        self.region_id = region_id
+        # 集群模板id。
+        self.template_id = template_id
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
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class GetApiTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: ApiTemplate = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        # 请求ID。
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = ApiTemplate()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetApiTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetApiTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
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
+            temp_model = GetApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetApplicationRequest(TeaModel):
     def __init__(
         self,
         application_name: str = None,
         cluster_id: str = None,
         region_id: str = None,
     ):
@@ -28783,14 +29089,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = JoinResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListApiTemplatesRequest(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        max_results: int = None,
+        next_token: str = None,
+        region_id: str = None,
+        resource_group_id: str = None,
+        template_id: str = None,
+        template_ids: List[str] = None,
+        template_name: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        # 标记当前开始读取的位置，置空表示从头开始。
+        self.next_token = next_token
+        # 区域ID。
+        self.region_id = region_id
+        # 资源组ID。
+        self.resource_group_id = resource_group_id
+        # 集群模板id。
+        self.template_id = template_id
+        # 集群模板id列表。
+        self.template_ids = template_ids
+        # 集群模板名字。
+        self.template_name = template_name
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.template_ids is not None:
+            result['TemplateIds'] = self.template_ids
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('TemplateIds') is not None:
+            self.template_ids = m.get('TemplateIds')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class ListApiTemplatesResponseBody(TeaModel):
+    def __init__(
+        self,
+        api_templates: List[ApiTemplate] = None,
+        max_results: int = None,
+        next_token: str = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.api_templates = api_templates
+        # 本次请求所返回的最大记录条数。
+        self.max_results = max_results
+        # 返回读取到的数据位置，空代表数据已经读取完毕。
+        self.next_token = next_token
+        # 请求ID。
+        self.request_id = request_id
+        # 本次请求条件下的数据总量。
+        self.total_count = total_count
+
+    def validate(self):
+        if self.api_templates:
+            for k in self.api_templates:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ApiTemplates'] = []
+        if self.api_templates is not None:
+            for k in self.api_templates:
+                result['ApiTemplates'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.api_templates = []
+        if m.get('ApiTemplates') is not None:
+            for k in m.get('ApiTemplates'):
+                temp_model = ApiTemplate()
+                self.api_templates.append(temp_model.from_map(k))
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListApiTemplatesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListApiTemplatesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
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
+            temp_model = ListApiTemplatesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListApplicationConfigsRequest(TeaModel):
     def __init__(
         self,
         application_name: str = None,
         cluster_id: str = None,
         config_file_name: str = None,
         config_item_key: str = None,
@@ -45659,14 +46146,138 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveAutoScalingPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RunApiTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        api_name: str = None,
+        client_token: str = None,
+        region_id: str = None,
+        template_id: str = None,
+    ):
+        # 接口名。
+        self.api_name = api_name
+        # 幂等客户端TOKEN。
+        self.client_token = client_token
+        # 地域ID。
+        self.region_id = region_id
+        # 集群模板id。
+        self.template_id = template_id
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
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class RunApiTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: str = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        # 请求ID。
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
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RunApiTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RunApiTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
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
+            temp_model = RunApiTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RunApplicationActionRequest(TeaModel):
     def __init__(
         self,
         action_name: str = None,
         batch_size: int = None,
         cluster_id: str = None,
         component_instance_selector: ComponentInstanceSelector = None,
```

### Comparing `alibabacloud_emr20210320-1.4.2/alibabacloud_emr20210320.egg-info/PKG-INFO` & `alibabacloud_emr20210320-1.5.0/alibabacloud_emr20210320.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr20210320
-Version: 1.4.2
+Version: 1.5.0
 Summary: Alibaba Cloud Emr (20210320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr20210320-1.4.2/setup.py` & `alibabacloud_emr20210320-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr20210320.
 
-Created on 26/03/2024
+Created on 17/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr20210320"
 NAME = "alibabacloud_emr20210320" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Emr (20210320) SDK Library for Python"
```

