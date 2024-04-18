# Comparing `tmp/alibabacloud_sddp20190103-1.2.0.tar.gz` & `tmp/alibabacloud_sddp20190103-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sddp20190103-1.2.0.tar", last modified: Mon Mar 25 08:03:48 2024, max compression
+gzip compressed data, was "dist/alibabacloud_sddp20190103-1.2.1.tar", last modified: Thu Apr 18 17:11:47 2024, max compression
```

## Comparing `alibabacloud_sddp20190103-1.2.0.tar` & `alibabacloud_sddp20190103-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:03:48.000000 alibabacloud_sddp20190103-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      935 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2443 2024-03-25 08:03:48.000000 alibabacloud_sddp20190103-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:03:48.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254616 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/client.py
--rw-r--r--   0 root         (0) root         (0)   493707 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 08:03:48.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2443 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 08:03:48.000000 alibabacloud_sddp20190103-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-25 08:03:47.000000 alibabacloud_sddp20190103-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   255572 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/client.py
+-rw-r--r--   0 root         (0) root         (0)   497053 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-18 17:11:47.000000 alibabacloud_sddp20190103-1.2.1/setup.py
```

### Comparing `alibabacloud_sddp20190103-1.2.0/ChangeLog.md` & `alibabacloud_sddp20190103-1.2.1/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-25 Version: 1.2.0
+- Support API DescribeParentInstance.
+
+
 2024-01-16 Version: 1.1.2
 - Generated python 2019-01-03 for Sddp.
 
 2023-12-27 Version: 1.1.1
 - Generated python 2019-01-03 for Sddp.
 
 2023-08-29 Version: 1.1.0
```

### Comparing `alibabacloud_sddp20190103-1.2.0/LICENSE` & `alibabacloud_sddp20190103-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.2.0/PKG-INFO` & `alibabacloud_sddp20190103-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sddp20190103
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sddp20190103-1.2.0/README-CN.md` & `alibabacloud_sddp20190103-1.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.2.0/README.md` & `alibabacloud_sddp20190103-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/client.py` & `alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1807,14 +1807,16 @@
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.engine_type):
             query['EngineType'] = request.engine_type
         if not UtilClient.is_unset(request.feature_type):
             query['FeatureType'] = request.feature_type
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_id):
             query['ParentId'] = request.parent_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.service_region_id):
@@ -1861,14 +1863,16 @@
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.engine_type):
             query['EngineType'] = request.engine_type
         if not UtilClient.is_unset(request.feature_type):
             query['FeatureType'] = request.feature_type
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_id):
             query['ParentId'] = request.parent_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.service_region_id):
@@ -2385,14 +2389,16 @@
             query['FileCategoryCode'] = request.file_category_code
         if not UtilClient.is_unset(request.file_type):
             query['FileType'] = request.file_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.model_ids):
             query['ModelIds'] = request.model_ids
         if not UtilClient.is_unset(request.model_tag_ids):
             query['ModelTagIds'] = request.model_tag_ids
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_category_ids):
@@ -2443,14 +2449,16 @@
             query['FileCategoryCode'] = request.file_category_code
         if not UtilClient.is_unset(request.file_type):
             query['FileType'] = request.file_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.model_ids):
             query['ModelIds'] = request.model_ids
         if not UtilClient.is_unset(request.model_tag_ids):
             query['ModelTagIds'] = request.model_tag_ids
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_category_ids):
@@ -2894,17 +2902,18 @@
 
     def describe_instance_sources_with_options(
         self,
         request: sddp_20190103_models.DescribeInstanceSourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> sddp_20190103_models.DescribeInstanceSourcesResponse:
         """
-        You can call this operation to query the data assets that DSC is not authorized to access. This helps you obtain information about the data assets.
-        # Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        You can query a list of unauthorized or authorized data assets based on the value of AuthStatus.
+        This operation is no longer used for the KMS console of the new version.
+        # [](#qps-)QPS limits
+        This operation can be called up to 10 times per second for each Alibaba Cloud account. If the number of calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: DescribeInstanceSourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeInstanceSourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2955,17 +2964,18 @@
 
     async def describe_instance_sources_with_options_async(
         self,
         request: sddp_20190103_models.DescribeInstanceSourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> sddp_20190103_models.DescribeInstanceSourcesResponse:
         """
-        You can call this operation to query the data assets that DSC is not authorized to access. This helps you obtain information about the data assets.
-        # Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        You can query a list of unauthorized or authorized data assets based on the value of AuthStatus.
+        This operation is no longer used for the KMS console of the new version.
+        # [](#qps-)QPS limits
+        This operation can be called up to 10 times per second for each Alibaba Cloud account. If the number of calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: DescribeInstanceSourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeInstanceSourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3015,32 +3025,34 @@
         )
 
     def describe_instance_sources(
         self,
         request: sddp_20190103_models.DescribeInstanceSourcesRequest,
     ) -> sddp_20190103_models.DescribeInstanceSourcesResponse:
         """
-        You can call this operation to query the data assets that DSC is not authorized to access. This helps you obtain information about the data assets.
-        # Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        You can query a list of unauthorized or authorized data assets based on the value of AuthStatus.
+        This operation is no longer used for the KMS console of the new version.
+        # [](#qps-)QPS limits
+        This operation can be called up to 10 times per second for each Alibaba Cloud account. If the number of calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: DescribeInstanceSourcesRequest
         @return: DescribeInstanceSourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_sources_with_options(request, runtime)
 
     async def describe_instance_sources_async(
         self,
         request: sddp_20190103_models.DescribeInstanceSourcesRequest,
     ) -> sddp_20190103_models.DescribeInstanceSourcesResponse:
         """
-        You can call this operation to query the data assets that DSC is not authorized to access. This helps you obtain information about the data assets.
-        # Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        You can query a list of unauthorized or authorized data assets based on the value of AuthStatus.
+        This operation is no longer used for the KMS console of the new version.
+        # [](#qps-)QPS limits
+        This operation can be called up to 10 times per second for each Alibaba Cloud account. If the number of calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: DescribeInstanceSourcesRequest
         @return: DescribeInstanceSourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instance_sources_with_options_async(request, runtime)
 
@@ -3639,14 +3651,16 @@
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.engine_type):
             query['EngineType'] = request.engine_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.service_region_id):
             query['ServiceRegionId'] = request.service_region_id
         req = open_api_models.OpenApiRequest(
@@ -3687,14 +3701,16 @@
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.engine_type):
             query['EngineType'] = request.engine_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lang):
             query['Lang'] = request.lang
+        if not UtilClient.is_unset(request.member_account):
+            query['MemberAccount'] = request.member_account
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.service_region_id):
             query['ServiceRegionId'] = request.service_region_id
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103/models.py` & `alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,20 +18,22 @@
         # 
         # *   **access_failed_cnt**: the maximum number of access attempts allowed when Data Security Center (DSC) fails to access an unauthorized resource.
         # *   **access_permission_exprie_max_days**: the maximum idle period allowed for access permissions before an alert is triggered.
         # *   **log_datasize_avg_days**: the minimum percentage of the volume of logs of a specific type generated on the current day to the average volume of logs generated in the previous 10 days before an alert is triggered.
         self.code = code
         # The description of the common configuration item.
         self.description = description
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Chinese
         # *   **en_us**: English
         self.lang = lang
+        # This parameter is deprecated.
         self.source_ip = source_ip
         # The value of the common configuration item. The meaning of this parameter varies with the value of the Code parameter.
         # 
         # *   If you set the Code parameter to **access_failed_cnt**, the Value parameter specifies the maximum number of access attempts allowed when DSC fails to access an unauthorized resource.
         # *   If you set the Code parameter to **access_permission_exprie_max_days**, the Value parameter specifies the maximum idle period allowed for access permissions before an alert is triggered.
         # *   If you set the Code parameter to **log_datasize_avg_days**, the Value parameter specifies the minimum percentage of the volume of logs of a specific type generated on the current day to the average amount of logs generated in the previous 10 days before an alert is triggered.
         self.value = value
@@ -204,14 +206,15 @@
         # *   **SQLServer**\
         self.engine_type = engine_type
         # Specifies whether to enable anomalous event detection. Valid values:
         # 
         # *   **0**: no
         # *   **1**: yes (default)
         self.event_status = event_status
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Chinese
         # *   **en_us**: English
         self.lang = lang
         # The retention period of raw logs after you enable the security audit feature. Unit: days. Valid values:
@@ -252,14 +255,15 @@
         # *   **cn-zhangjiakou**: China (Zhangjiakou)
         # *   **cn-huhehaote**: China (Hohhot)
         # *   **cn-hangzhou**: China (Hangzhou)
         # *   **cn-shanghai**: China (Shanghai)
         # *   **cn-shenzhen**: China (Shenzhen)
         # *   **cn-hongkong**: China (Hong Kong)
         self.service_region_id = service_region_id
+        # This parameter is deprecated.
         self.source_ip = source_ip
         # The username that is used to access the database.
         self.user_name = user_name
 
     def validate(self):
         pass
 
@@ -483,14 +487,15 @@
         # The type of the sensitive data detection rule. Valid values:
         # 
         # *   **1**: sensitive data detection rule
         # *   **2**: audit rule
         # *   **3**: anomalous event detection rule
         # *   **99**: custom rule
         self.rule_type = rule_type
+        # This parameter is deprecated.
         self.source_ip = source_ip
         # The statistical expression.
         self.stat_express = stat_express
         # Specifies whether to enable the sensitive data detection rule. Valid values:
         # 
         # *   **1**: yes
         # *   **0**: no
@@ -687,14 +692,15 @@
         scan_range_content: str = None,
         source_ip: str = None,
         task_name: str = None,
         task_user_name: str = None,
     ):
         # The unique ID of the data asset, such as an instance, a database, and a bucket. You can call the [DescribeDataLimits](~~DescribeDataLimits~~) operation to query the unique ID.
         self.data_limit_id = data_limit_id
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The interval between two consecutive custom scan tasks. Unit: days. Valid values: 1 to 2147483648.
         self.interval_day = interval_day
         # The language of the content within the request and response.
         # 
         # *   **zh**: Chinese
         # *   **en**: English
@@ -712,14 +718,15 @@
         # *   **0**: exact match
         # *   **1**: prefix match
         # *   **2**: suffix match
         # *   **3**: regular expression match
         self.scan_range = scan_range
         # The data to be scanned in a structured data asset. Prefix match, suffix match, and regular expression match are supported.
         self.scan_range_content = scan_range_content
+        # This parameter is deprecated.
         self.source_ip = source_ip
         # The name of the scan task.
         self.task_name = task_name
         # The account that is used to create the scan task.
         self.task_user_name = task_user_name
 
     def validate(self):
@@ -869,20 +876,22 @@
 class CreateSlrRoleRequest(TeaModel):
     def __init__(
         self,
         feature_type: int = None,
         lang: str = None,
         source_ip: str = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Simplified Chinese
         # *   **en_us**: English
         self.lang = lang
+        # This parameter is deprecated.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -992,24 +1001,26 @@
     def __init__(
         self,
         feature_type: int = None,
         id: int = None,
         lang: str = None,
         source_ip: str = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The ID of the data asset.
         # 
         # You can call the DescribeDataLimits operation to query the IDs of data assets. The value of the Id response parameter indicates the ID of a data asset.
         self.id = id
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Chinese
         # *   **en_us**: English
         self.lang = lang
+        # This parameter is deprecated.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1113,19 +1124,21 @@
     def __init__(
         self,
         feature_type: int = None,
         id: int = None,
         lang: str = None,
         source_ip: str = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The ID of the sensitive data detection rule.
         self.id = id
         # The language of the content within the request and response. Valid values: **zh** and **en**. The value zh indicates Chinese, and the value en indicates English.
         self.lang = lang
+        # This parameter is deprecated.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1471,14 +1484,15 @@
         lang: str = None,
         page_size: int = None,
         risk_level_id: int = None,
         status: int = None,
     ):
         # The number of the page to return. Default value: **1**.
         self.current_page = current_page
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Simplified Chinese
         # *   **en_us**: English
         self.lang = lang
         # The number of entries to return on each page. Default value: **10**.
@@ -3188,14 +3202,15 @@
     def __init__(
         self,
         feature_type: int = None,
         id: int = None,
         lang: str = None,
         network_type: int = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The unique ID of the data asset that you want to query.
         # 
         # > You can call the [DescribeDataLimits](~~DescribeDataLimits~~) operation to query the ID of the data asset.
         self.id = id
         # The language of the content within the request and response. Valid values:
         # 
@@ -3440,14 +3455,15 @@
     def __init__(
         self,
         feature_type: int = None,
         lang: str = None,
         parent_id: str = None,
         resource_type: int = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values:
         # 
         # *   **zh_cn**: Simplified Chinese (default)
         # *   **en_us**: English
         self.lang = lang
         # The parent asset ID of the data asset.
@@ -3866,14 +3882,15 @@
         current_page: int = None,
         datamask_status: int = None,
         enable: int = None,
         end_time: int = None,
         engine_type: str = None,
         feature_type: int = None,
         lang: str = None,
+        member_account: int = None,
         page_size: int = None,
         parent_id: str = None,
         resource_type: int = None,
         service_region_id: str = None,
         start_time: int = None,
     ):
         # Specifies whether to enable the security audit feature. Valid values:
@@ -3901,20 +3918,22 @@
         # *   **1**: yes
         # *   **0**: no
         self.enable = enable
         # The end of the time range to query The value is a UNIX timestamp. Unit: milliseconds.
         self.end_time = end_time
         # The type of the database engine. Valid values include **MySQL**, **SQLServer**, **Oracle**, **PostgreSQL**, and **MongoDB**.
         self.engine_type = engine_type
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values:
         # 
         # *   **zh**: Chinese
         # *   **en**: English
         self.lang = lang
+        self.member_account = member_account
         # The number of entries to return on each page.
         self.page_size = page_size
         # The parent ID of the data asset to be queried. Valid values:
         # 
         # *   The name or ID of the MaxCompute project.
         # *   The name or ID of the OSS bucket.
         # *   The name or ID of the ApsaraDB RDS instance or database.
@@ -3956,14 +3975,16 @@
             result['EndTime'] = self.end_time
         if self.engine_type is not None:
             result['EngineType'] = self.engine_type
         if self.feature_type is not None:
             result['FeatureType'] = self.feature_type
         if self.lang is not None:
             result['Lang'] = self.lang
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.parent_id is not None:
             result['ParentId'] = self.parent_id
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         if self.service_region_id is not None:
@@ -3988,14 +4009,16 @@
             self.end_time = m.get('EndTime')
         if m.get('EngineType') is not None:
             self.engine_type = m.get('EngineType')
         if m.get('FeatureType') is not None:
             self.feature_type = m.get('FeatureType')
         if m.get('Lang') is not None:
             self.lang = m.get('Lang')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ParentId') is not None:
             self.parent_id = m.get('ParentId')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         if m.get('ServiceRegionId') is not None:
@@ -4022,14 +4045,15 @@
         gmt_create: int = None,
         id: int = None,
         instance_description: str = None,
         instance_id: str = None,
         last_finished_time: int = None,
         local_name: str = None,
         log_store_day: int = None,
+        member_account: int = None,
         next_start_time: int = None,
         ocr_status: int = None,
         parent_id: str = None,
         port: int = None,
         process_status: int = None,
         process_total_count: int = None,
         region_id: str = None,
@@ -4104,14 +4128,15 @@
         # *   The value is a UNIX timestamp.
         # *   Unit: milliseconds.
         self.last_finished_time = last_finished_time
         # The region in which the data asset resides.
         self.local_name = local_name
         # The retention period of raw logs. Unit: days.
         self.log_store_day = log_store_day
+        self.member_account = member_account
         # The next time when the data asset is scanned. The value is a UNIX timestamp. Unit: milliseconds.
         self.next_start_time = next_start_time
         # Indicates whether the optical character recognition (OCR) feature is enabled. Valid values:
         # 
         # *   **0**: no
         # *   **1**: yes
         self.ocr_status = ocr_status
@@ -4223,14 +4248,16 @@
             result['InstanceId'] = self.instance_id
         if self.last_finished_time is not None:
             result['LastFinishedTime'] = self.last_finished_time
         if self.local_name is not None:
             result['LocalName'] = self.local_name
         if self.log_store_day is not None:
             result['LogStoreDay'] = self.log_store_day
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         if self.next_start_time is not None:
             result['NextStartTime'] = self.next_start_time
         if self.ocr_status is not None:
             result['OcrStatus'] = self.ocr_status
         if self.parent_id is not None:
             result['ParentId'] = self.parent_id
         if self.port is not None:
@@ -4305,14 +4332,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('LastFinishedTime') is not None:
             self.last_finished_time = m.get('LastFinishedTime')
         if m.get('LocalName') is not None:
             self.local_name = m.get('LocalName')
         if m.get('LogStoreDay') is not None:
             self.log_store_day = m.get('LogStoreDay')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         if m.get('NextStartTime') is not None:
             self.next_start_time = m.get('NextStartTime')
         if m.get('OcrStatus') is not None:
             self.ocr_status = m.get('OcrStatus')
         if m.get('ParentId') is not None:
             self.parent_id = m.get('ParentId')
         if m.get('Port') is not None:
@@ -4913,31 +4942,34 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDataMaskingTasksResponseBodyItems(TeaModel):
     def __init__(
         self,
+        dst_member_account: int = None,
         dst_path: str = None,
         dst_type: int = None,
         dst_type_code: str = None,
         gmt_create: int = None,
         has_unfinish_process: bool = None,
         id: int = None,
         original_table: bool = None,
         owner: str = None,
         run_count: int = None,
+        src_member_account: int = None,
         src_path: str = None,
         src_type: int = None,
         src_type_code: str = None,
         status: int = None,
         task_id: str = None,
         task_name: str = None,
         trigger_type: int = None,
     ):
+        self.dst_member_account = dst_member_account
         # The destination directory.
         self.dst_path = dst_path
         # The service to which the data to be de-identified belongs. Valid values: **1**, **2**, **3**, **4**, and **5**. The value 1 indicates MaxCompute. The value 2 indicates OSS. The value 3 indicates AnalyticDB for MySQL. The value 4 indicates Tablestore. The value 5 indicates ApsaraDB RDS.
         self.dst_type = dst_type
         # The service to which the de-identified data belongs. Valid values include **MaxCompute, OSS, ADS, OTS, and RDS**.
         self.dst_type_code = dst_type_code
         # The time when the task was created. The value is a UNIX timestamp. Unit: milliseconds.
@@ -4948,14 +4980,15 @@
         self.id = id
         # Indicates whether the source table is de-identified.
         self.original_table = original_table
         # The user who created the de-identification task.
         self.owner = owner
         # The number of times that the de-identification task is run.
         self.run_count = run_count
+        self.src_member_account = src_member_account
         # The source path.
         self.src_path = src_path
         # The code of the service to which the data to be de-identified belongs. Valid values: **1**, **2**, **3**, **4**, and **5**. The value 1 indicates MaxCompute. The value 2 indicates OSS. The value indicates AnalyticDB for MySQL. The value 4 indicates Tablestore. The value 5 indicates ApsaraDB RDS.
         self.src_type = src_type
         # The service to which the data to be de-identified belongs. Valid values include **MaxCompute, OSS, ADS, OTS, and RDS**.
         self.src_type_code = src_type_code
         # The status of the task. Valid values:
@@ -4979,14 +5012,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.dst_member_account is not None:
+            result['DstMemberAccount'] = self.dst_member_account
         if self.dst_path is not None:
             result['DstPath'] = self.dst_path
         if self.dst_type is not None:
             result['DstType'] = self.dst_type
         if self.dst_type_code is not None:
             result['DstTypeCode'] = self.dst_type_code
         if self.gmt_create is not None:
@@ -4997,14 +5032,16 @@
             result['Id'] = self.id
         if self.original_table is not None:
             result['OriginalTable'] = self.original_table
         if self.owner is not None:
             result['Owner'] = self.owner
         if self.run_count is not None:
             result['RunCount'] = self.run_count
+        if self.src_member_account is not None:
+            result['SrcMemberAccount'] = self.src_member_account
         if self.src_path is not None:
             result['SrcPath'] = self.src_path
         if self.src_type is not None:
             result['SrcType'] = self.src_type
         if self.src_type_code is not None:
             result['SrcTypeCode'] = self.src_type_code
         if self.status is not None:
@@ -5015,14 +5052,16 @@
             result['TaskName'] = self.task_name
         if self.trigger_type is not None:
             result['TriggerType'] = self.trigger_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DstMemberAccount') is not None:
+            self.dst_member_account = m.get('DstMemberAccount')
         if m.get('DstPath') is not None:
             self.dst_path = m.get('DstPath')
         if m.get('DstType') is not None:
             self.dst_type = m.get('DstType')
         if m.get('DstTypeCode') is not None:
             self.dst_type_code = m.get('DstTypeCode')
         if m.get('GmtCreate') is not None:
@@ -5033,14 +5072,16 @@
             self.id = m.get('Id')
         if m.get('OriginalTable') is not None:
             self.original_table = m.get('OriginalTable')
         if m.get('Owner') is not None:
             self.owner = m.get('Owner')
         if m.get('RunCount') is not None:
             self.run_count = m.get('RunCount')
+        if m.get('SrcMemberAccount') is not None:
+            self.src_member_account = m.get('SrcMemberAccount')
         if m.get('SrcPath') is not None:
             self.src_path = m.get('SrcPath')
         if m.get('SrcType') is not None:
             self.src_type = m.get('SrcType')
         if m.get('SrcTypeCode') is not None:
             self.src_type_code = m.get('SrcTypeCode')
         if m.get('Status') is not None:
@@ -5747,14 +5788,15 @@
         current_page: int = None,
         domain_id: int = None,
         feature_type: int = None,
         file_category_code: int = None,
         file_type: int = None,
         instance_id: str = None,
         lang: str = None,
+        member_account: int = None,
         model_ids: str = None,
         model_tag_ids: str = None,
         page_size: int = None,
         parent_category_ids: str = None,
         product_ids: str = None,
         query_name: str = None,
         risk_levels: str = None,
@@ -5764,14 +5806,15 @@
         self.current_page = current_page
         self.domain_id = domain_id
         self.feature_type = feature_type
         self.file_category_code = file_category_code
         self.file_type = file_type
         self.instance_id = instance_id
         self.lang = lang
+        self.member_account = member_account
         self.model_ids = model_ids
         self.model_tag_ids = model_tag_ids
         self.page_size = page_size
         self.parent_category_ids = parent_category_ids
         self.product_ids = product_ids
         self.query_name = query_name
         self.risk_levels = risk_levels
@@ -5797,14 +5840,16 @@
             result['FileCategoryCode'] = self.file_category_code
         if self.file_type is not None:
             result['FileType'] = self.file_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.lang is not None:
             result['Lang'] = self.lang
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         if self.model_ids is not None:
             result['ModelIds'] = self.model_ids
         if self.model_tag_ids is not None:
             result['ModelTagIds'] = self.model_tag_ids
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.parent_category_ids is not None:
@@ -5833,14 +5878,16 @@
             self.file_category_code = m.get('FileCategoryCode')
         if m.get('FileType') is not None:
             self.file_type = m.get('FileType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('Lang') is not None:
             self.lang = m.get('Lang')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         if m.get('ModelIds') is not None:
             self.model_ids = m.get('ModelIds')
         if m.get('ModelTagIds') is not None:
             self.model_tag_ids = m.get('ModelTagIds')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ParentCategoryIds') is not None:
@@ -5946,14 +5993,15 @@
     def __init__(
         self,
         categories: List[str] = None,
         id: str = None,
         instance_description: str = None,
         instance_id: str = None,
         last_scan_time: int = None,
+        member_account: int = None,
         model_tags: List[DescribeDataObjectsResponseBodyItemsModelTags] = None,
         name: str = None,
         object_file_category: str = None,
         object_type: str = None,
         path: str = None,
         product_code: str = None,
         product_id: int = None,
@@ -5963,14 +6011,15 @@
         template_id: int = None,
     ):
         self.categories = categories
         self.id = id
         self.instance_description = instance_description
         self.instance_id = instance_id
         self.last_scan_time = last_scan_time
+        self.member_account = member_account
         self.model_tags = model_tags
         self.name = name
         self.object_file_category = object_file_category
         self.object_type = object_type
         self.path = path
         self.product_code = product_code
         self.product_id = product_id
@@ -6001,14 +6050,16 @@
             result['Id'] = self.id
         if self.instance_description is not None:
             result['InstanceDescription'] = self.instance_description
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.last_scan_time is not None:
             result['LastScanTime'] = self.last_scan_time
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         result['ModelTags'] = []
         if self.model_tags is not None:
             for k in self.model_tags:
                 result['ModelTags'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
         if self.object_file_category is not None:
@@ -6041,14 +6092,16 @@
             self.id = m.get('Id')
         if m.get('InstanceDescription') is not None:
             self.instance_description = m.get('InstanceDescription')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('LastScanTime') is not None:
             self.last_scan_time = m.get('LastScanTime')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         self.model_tags = []
         if m.get('ModelTags') is not None:
             for k in m.get('ModelTags'):
                 temp_model = DescribeDataObjectsResponseBodyItemsModelTags()
                 self.model_tags.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
@@ -6969,14 +7022,15 @@
         self,
         feature_type: int = None,
         lang: str = None,
         parent_type_id: int = None,
         resource_id: int = None,
         status: int = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values:
         # 
         # *   **zh**: Chinese
         # *   **en**: English
         self.lang = lang
         # The type of anomalous event for which you want to query the anomalous events of subtypes. Valid values:
@@ -7737,14 +7791,15 @@
         # *   **0**: no
         # *   **1**: yes
         self.auth_status = auth_status
         # The number of the page to return. Default value: **1**.
         self.current_page = current_page
         # The type of the database engine. Valid values: **MySQL, MariaDB, Oracle, PostgreSQL, and SQLServer**.
         self.engine_type = engine_type
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The ID of the instance.
         self.instance_id = instance_id
         # The language of the content within the request and response. Valid values:
         # 
         # *   **zh_cn**: Simplified Chinese (default)
         # *   **en_us**: English
@@ -9906,26 +9961,28 @@
         check_status: int = None,
         cluster_status: str = None,
         current_page: int = None,
         db_name: str = None,
         engine_type: str = None,
         instance_id: str = None,
         lang: str = None,
+        member_account: int = None,
         page_size: int = None,
         resource_type: int = None,
         service_region_id: str = None,
     ):
         self.auth_status = auth_status
         self.check_status = check_status
         self.cluster_status = cluster_status
         self.current_page = current_page
         self.db_name = db_name
         self.engine_type = engine_type
         self.instance_id = instance_id
         self.lang = lang
+        self.member_account = member_account
         self.page_size = page_size
         self.resource_type = resource_type
         self.service_region_id = service_region_id
 
     def validate(self):
         pass
 
@@ -9947,14 +10004,16 @@
             result['DbName'] = self.db_name
         if self.engine_type is not None:
             result['EngineType'] = self.engine_type
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.lang is not None:
             result['Lang'] = self.lang
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         if self.service_region_id is not None:
             result['ServiceRegionId'] = self.service_region_id
         return result
@@ -9973,14 +10032,16 @@
             self.db_name = m.get('DbName')
         if m.get('EngineType') is not None:
             self.engine_type = m.get('EngineType')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('Lang') is not None:
             self.lang = m.get('Lang')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         if m.get('ServiceRegionId') is not None:
             self.service_region_id = m.get('ServiceRegionId')
         return self
@@ -9995,14 +10056,15 @@
         connect_node: str = None,
         db_num: str = None,
         engine_type: str = None,
         instance_description: str = None,
         instance_id: str = None,
         instance_size: int = None,
         local_name: str = None,
+        member_account: int = None,
         parent_id: str = None,
         resource_type: str = None,
         support_connect_nodes: str = None,
         tenant_id: str = None,
         tenant_name: str = None,
         un_connect_db_count: str = None,
         un_support_one_click_auth_reason: str = None,
@@ -10013,14 +10075,15 @@
         self.connect_node = connect_node
         self.db_num = db_num
         self.engine_type = engine_type
         self.instance_description = instance_description
         self.instance_id = instance_id
         self.instance_size = instance_size
         self.local_name = local_name
+        self.member_account = member_account
         self.parent_id = parent_id
         self.resource_type = resource_type
         self.support_connect_nodes = support_connect_nodes
         self.tenant_id = tenant_id
         self.tenant_name = tenant_name
         self.un_connect_db_count = un_connect_db_count
         self.un_support_one_click_auth_reason = un_support_one_click_auth_reason
@@ -10050,14 +10113,16 @@
             result['InstanceDescription'] = self.instance_description
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.instance_size is not None:
             result['InstanceSize'] = self.instance_size
         if self.local_name is not None:
             result['LocalName'] = self.local_name
+        if self.member_account is not None:
+            result['MemberAccount'] = self.member_account
         if self.parent_id is not None:
             result['ParentId'] = self.parent_id
         if self.resource_type is not None:
             result['ResourceType'] = self.resource_type
         if self.support_connect_nodes is not None:
             result['SupportConnectNodes'] = self.support_connect_nodes
         if self.tenant_id is not None:
@@ -10088,14 +10153,16 @@
             self.instance_description = m.get('InstanceDescription')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('InstanceSize') is not None:
             self.instance_size = m.get('InstanceSize')
         if m.get('LocalName') is not None:
             self.local_name = m.get('LocalName')
+        if m.get('MemberAccount') is not None:
+            self.member_account = m.get('MemberAccount')
         if m.get('ParentId') is not None:
             self.parent_id = m.get('ParentId')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         if m.get('SupportConnectNodes') is not None:
             self.support_connect_nodes = m.get('SupportConnectNodes')
         if m.get('TenantId') is not None:
@@ -10212,14 +10279,15 @@
 class DescribeRiskLevelsRequest(TeaModel):
     def __init__(
         self,
         feature_type: int = None,
         lang: str = None,
         template_id: int = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values:
         # 
         # *   zh_cn: Chinese (default)
         # *   en_us: English
         self.lang = lang
         # The ID of the industry-specific rule template.
@@ -11613,15 +11681,15 @@
         # *   **POSTPAY**: pay-as-you-go
         self.charge_type = charge_type
         # The permissions that the current account has. Valid values:
         # 
         # *   **0**: The current account has the administrative permissions or read-only permissions on Data Security Center.
         # *   **1**: The current account has the permissions to manage data domains.
         self.data_manager_role = data_manager_role
-        # The ID of the instance within the current account.
+        # The ID of the data security center instance purchased by the main account.
         self.instance_id = instance_id
         # The number of instances within the current account.
         self.instance_num = instance_num
         # The total number of instances.
         self.instance_total_count = instance_total_count
         # Indicates whether the data security lab feature is enabled. Valid values:
         # 
@@ -11837,14 +11905,15 @@
         self,
         code: str = None,
         feature_type: int = None,
         lang: str = None,
     ):
         # The code of the configuration item. You can call the [DescribeConfigs](~~DescribeConfigs~~) operation to obtain the code of the configuration item.
         self.code = code
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values:
         # 
         # *   **zh_cn**: Chinese (default)
         # *   **en_us**: English
         self.lang = lang
 
@@ -11955,14 +12024,15 @@
     ):
         # The sensitive data to be de-identified. The value is a JSON string that contains the following parameters:
         # 
         # *   **dataHeaderList**: the names of the columns in which data needs to be de-identified. Specify the column names in accordance with the order of data that needs to be de-identified.
         # *   **dataList**: the data that needs to be de-identified.
         # *   **ruleList**: the IDs of sensitive data detection rules used to detect data that needs to be de-identified. Specify the rule IDs in accordance with the order of data that needs to be de-identified. Each ID identifies a sensitive data detection rule that is used to detect a type of sensitive data. You can call the [DescribeRules](~~DescribeRules~~) operation to query the IDs of sensitive data detection rules.
         self.data = data
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Default value: **zh_cn**. Valid values:
         # 
         # *   **zh_cn**: Simplified Chinese
         # *   **en_us**: English
         self.lang = lang
         # The ID of the de-identification template. The ID is generated after you create the de-identification template in the [Data Security Center (DSC) console](https://yundun.console.aliyun.com/?\&p=sddpnext#/sddp/dm/template). You can choose **Data desensitization** > **Desensitization Template** in the left-side navigation pane and obtain the ID of the de-identification template from the **Desensitization Template** page.
@@ -12226,14 +12296,15 @@
         # > When a re-scan is triggered, DSC scans all data in your data asset.
         self.auto_scan = auto_scan
         # The database engine that is run by the instance. Valid values:
         # 
         # *   **MySQL**\
         # *   **SQLServer**\
         self.engine_type = engine_type
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The unique ID of the data asset for which you want to modify configuration items.
         # 
         # > You can call the [DescribeDataLimits](~~DescribeDataLimits~~) operation to query the ID of the data asset.
         self.id = id
         # The language of the content within the request and response. Valid values:
         # 
@@ -12707,14 +12778,15 @@
 class ModifyEventTypeStatusRequest(TeaModel):
     def __init__(
         self,
         feature_type: int = None,
         lang: str = None,
         sub_type_ids: str = None,
     ):
+        # This parameter is deprecated.
         self.feature_type = feature_type
         # The language of the content within the request and response. Valid values: **zh** and **en**. The value zh indicates Chinese, and the value en indicates English.
         self.lang = lang
         # The ID of the anomalous event subtype. Separate multiple IDs with commas (,).
         # 
         # > You can call the **DescribeEventTypes** operation to query the ID of anomalous event subtype.
         self.sub_type_ids = sub_type_ids
```

### Comparing `alibabacloud_sddp20190103-1.2.0/alibabacloud_sddp20190103.egg-info/PKG-INFO` & `alibabacloud_sddp20190103-1.2.1/alibabacloud_sddp20190103.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sddp20190103
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sddp20190103-1.2.0/setup.py` & `alibabacloud_sddp20190103-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sddp20190103.
 
-Created on 25/03/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sddp20190103"
 NAME = "alibabacloud_sddp20190103" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Sensitive Data Discovery and Protection (20190103) SDK Library for Python"
```

