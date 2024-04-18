# Comparing `tmp/alibabacloud_polardb20170801_py2-4.0.7.tar.gz` & `tmp/alibabacloud_polardb20170801_py2-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.0.7.tar", last modified: Tue Apr  9 17:13:45 2024, max compression
+gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.0.8.tar", last modified: Thu Apr 18 17:12:33 2024, max compression
```

## Comparing `alibabacloud_polardb20170801_py2-4.0.7.tar` & `alibabacloud_polardb20170801_py2-4.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/
--rw-r--r--   0 root         (0) root         (0)     4113 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   318134 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/client.py
--rw-r--r--   0 root         (0) root         (0)  1221376 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2936 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/
+-rw-r--r--   0 root         (0) root         (0)     4281 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   318134 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/client.py
+-rw-r--r--   0 root         (0) root         (0)  1223147 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/setup.py
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/ChangeLog.md` & `alibabacloud_polardb20170801_py2-4.0.8/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2024-04-09 Version: 4.0.7
+- Update API DescribeDBClusters: update response param.
+
+
+2024-04-09 Version: 4.0.7
+- Update API DescribeDBClusters: update response param.
+
+
 2024-03-14 Version: 4.0.6
 - Update API DescribeDBClusterAttribute: update response param.
 - Update API DescribeDBClusterParameters: update response param.
 - Update API DescribeDBClusterPerformance: add param Interval.
 - Update API DescribeDBClusterVersion: update response param.
 - Update API DescribeDBNodePerformance: add param Interval.
 - Update API DescribeDBNodePerformance: add param Type.
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/LICENSE` & `alibabacloud_polardb20170801_py2-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_polardb20170801_py2
-Version: 4.0.7
+Version: 4.0.8
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/README-CN.md` & `alibabacloud_polardb20170801_py2-4.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/README.md` & `alibabacloud_polardb20170801_py2-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/client.py` & `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/models.py` & `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7185,29 +7185,48 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeClassListRequest(TeaModel):
     def __init__(self, commodity_code=None, master_ha=None, order_type=None, owner_account=None, owner_id=None,
                  region_id=None, resource_group_id=None, resource_owner_account=None, resource_owner_id=None):
-        # The maximum number of IOPS.
+        # The code of the commodity. Valid values:
+        # 
+        # *   polardb_sub: the subscription cluster in regions in the Chinese mainland
+        # *   polardb_sub \_intl: the subscription cluster in regions outside the Chinese mainland
+        # *   polardb_payg: the pay-as-you-go cluster in regions in the Chinese mainland
+        # *   polardb_payg_intl: the pay-as-you-go cluster in regions outside the Chinese mainland
+        # *   polardb_sub_jushita: the subscription cluster for CloudTmall
+        # *   polardb_payg_jushita: the pay-as-you-go cluster for CloudTmall
+        # *   polardb_sub_cainiao: the subscription cluster for Cainiao
+        # *   polardb_payg_cainiao: the pay-as-you-go cluster for Cainiao
+        # 
+        # > *   If you use an Alibaba Cloud account on the China site, you can view only the codes of the commodities that are available in the Chinese mainland.
+        # >*   If you are using an Alibaba Cloud international account, you can view only the codes of the commodities that are available outside the Chinese mainland.
+        # >*   If you use a CloudTmall account, you can view only the codes of the commodities that are available in CloudTmall.
+        # >*   If you use a Cainiao account, you can view only the codes of the commodities that are available in Cainiao.
         self.commodity_code = commodity_code  # type: str
         # The number of nodes. Valid values:
         # 
-        # *   single
-        # *   cluster
-        # *   all
+        # *   single: Standalone Edition.
+        # *   cluster: Cluster Edition.
+        # *   all: both Standalone Edition and Cluster Edition.
         self.master_ha = master_ha  # type: str
-        # The specification type of the cluster.
+        # The type of the order. Valid values:
+        # 
+        # *   BUY: The order is used to purchase a cluster.
+        # *   UPGRADE: The order is used to change the specifications of a cluster.
+        # *   RENEW: The order is used to renew a cluster.
+        # *   CONVERT: The order is used to change the billing method of a cluster.
         self.order_type = order_type  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The number of CPU cores.
+        # The region ID of the cluster.
         self.region_id = region_id  # type: str
-        # The ID of the request.
+        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
@@ -7386,21 +7405,17 @@
         return self
 
 
 class DescribeClassListResponseBody(TeaModel):
     def __init__(self, items=None, region_id=None, request_id=None):
         # The specifications of the cluster.
         self.items = items  # type: list[DescribeClassListResponseBodyItems]
+        # The region ID of the cluster.
         self.region_id = region_id  # type: str
-        # The price.
-        # 
-        # Unit: cents (US dollars).
-        # 
-        # > *   If you set the CommodityCode parameter to a value that indicates the pay-as-you-go billing method, the ReferencePrice parameter specifies the hourly fee that you must pay.
-        # > *   If you set the CommodityCode parameter to a value that indicates the subscription billing method, the ReferencePrice parameter specifies the monthly fee that you must pay.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.items:
             for k in self.items:
                 if k:
                     k.validate()
@@ -8000,16 +8015,16 @@
                  dbtype=None, dbversion=None, dbversion_status=None, data_level_1backup_chain_size=None,
                  data_sync_mode=None, deletion_lock=None, engine=None, expire_time=None, expired=None,
                  has_complete_standby_res=None, hot_standby_cluster=None, inode_total=None, inode_used=None, is_latest_version=None,
                  is_proxy_latest_version=None, lock_mode=None, maintain_time=None, pay_type=None, provisioned_iops=None,
                  proxy_cpu_cores=None, proxy_serverless_type=None, proxy_standard_cpu_cores=None, proxy_status=None,
                  proxy_type=None, region_id=None, request_id=None, resource_group_id=None, sqlsize=None, serverless_type=None,
                  standby_hamode=None, storage_max=None, storage_pay_type=None, storage_space=None, storage_type=None,
-                 storage_used=None, strict_consistency=None, sub_category=None, tags=None, vpcid=None, v_switch_id=None,
-                 zone_ids=None):
+                 storage_used=None, strict_consistency=None, sub_category=None, support_instant_switch_with_imci=None,
+                 tags=None, vpcid=None, v_switch_id=None, zone_ids=None):
         self.ai_creating_time = ai_creating_time  # type: str
         # The information status of the AI node. Valid values:
         # 
         # *   SearchNode: search node.
         # *   DLNode: AI node
         self.ai_type = ai_type  # type: str
         self.architecture = architecture  # type: str
@@ -8163,14 +8178,15 @@
         # The specification type of the compute node. Valid values:
         # 
         # *   **Exclusive**: dedicated.
         # *   **General**: general-purpose.
         # 
         # > This parameter is supported only for PolarDB for MySQL clusters of Cluster Edition.
         self.sub_category = sub_category  # type: str
+        self.support_instant_switch_with_imci = support_instant_switch_with_imci  # type: str
         # Details about the tags.
         self.tags = tags  # type: list[DescribeDBClusterAttributeResponseBodyTags]
         # The VPC ID of the cluster.
         self.vpcid = vpcid  # type: str
         # The vSwitch ID of the cluster.
         self.v_switch_id = v_switch_id  # type: str
         # The zone ID of the cluster.
@@ -8292,14 +8308,16 @@
             result['StorageType'] = self.storage_type
         if self.storage_used is not None:
             result['StorageUsed'] = self.storage_used
         if self.strict_consistency is not None:
             result['StrictConsistency'] = self.strict_consistency
         if self.sub_category is not None:
             result['SubCategory'] = self.sub_category
+        if self.support_instant_switch_with_imci is not None:
+            result['SupportInstantSwitchWithImci'] = self.support_instant_switch_with_imci
         result['Tags'] = []
         if self.tags is not None:
             for k in self.tags:
                 result['Tags'].append(k.to_map() if k else None)
         if self.vpcid is not None:
             result['VPCId'] = self.vpcid
         if self.v_switch_id is not None:
@@ -8411,14 +8429,16 @@
             self.storage_type = m.get('StorageType')
         if m.get('StorageUsed') is not None:
             self.storage_used = m.get('StorageUsed')
         if m.get('StrictConsistency') is not None:
             self.strict_consistency = m.get('StrictConsistency')
         if m.get('SubCategory') is not None:
             self.sub_category = m.get('SubCategory')
+        if m.get('SupportInstantSwitchWithImci') is not None:
+            self.support_instant_switch_with_imci = m.get('SupportInstantSwitchWithImci')
         self.tags = []
         if m.get('Tags') is not None:
             for k in m.get('Tags'):
                 temp_model = DescribeDBClusterAttributeResponseBodyTags()
                 self.tags.append(temp_model.from_map(k))
         if m.get('VPCId') is not None:
             self.vpcid = m.get('VPCId')
@@ -22917,15 +22937,15 @@
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class ModifyDBClusterMaintainTimeResponseBody(TeaModel):
     def __init__(self, request_id=None):
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDBClusterMaintainTimeResponseBody, self).to_map()
@@ -24070,22 +24090,22 @@
         # The earliest time to upgrade the specifications within the scheduled time period. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # >- This parameter takes effect only when `ModifyType` is set to `Upgrade`.
         # >- The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in the time that ranges from `2021-01-14T09:00:00Z` to `2021-01-15T09:00:00Z`.
         # >- If this parameter is left empty, the upgrade task is immediately performed.
         self.planned_start_time = planned_start_time  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        # The new storage capacity. Unit: GB.
+        # The storage capacity that you can select when you change the cluster. Unit: GB.
         # 
-        # > Valid values for PolarDB for MySQL Standard Edition are 20 to 32000.
+        # >  You can set this parameter for PolarDB for MySQL clusters of Standard Edition to a value that ranges from 20 to 32000.
         self.storage_space = storage_space  # type: long
         # The category of the cluster. Default value: ON. Valid values:
         # 
         # *   **normal_exclusive**: dedicated
-        # *   **normal_general**: genera-purpose
+        # *   **normal_general**: general-purpose
         self.sub_category = sub_category  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDBClusterStorageSpaceRequest, self).to_map()
@@ -25002,22 +25022,22 @@
         # *   **Upgrade**\
         # *   **Downgrade**\
         self.modify_type = modify_type  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The latest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
-        # > *   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
-        # >*   By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to a value that is calculated by using the following formula: `Value of PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is set to `2021-01-14T09:30:00Z`.
+        # >*   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
+        # >*   By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to `Value of PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is `2021-01-14T09:30:00Z`.
         self.planned_end_time = planned_end_time  # type: str
         # The earliest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # > *   This parameter takes effect only when `ModifyType` is set to `Upgrade`.
-        # >*   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in the time range from `2021-01-14T09:00:00Z` to `2021-01-15T09:00:00Z`.
-        # >*   If this parameter is empty, the upgrade task is immediately performed.
+        # >*   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in the time that ranges from `2021-01-14T09:00:00Z` to `2021-01-15T09:00:00Z`.
+        # >*   If this parameter is left empty, the upgrade task is immediately performed.
         self.planned_start_time = planned_start_time  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The category of the cluster. Valid values:
         # 
         # *   **normal_exclusive**: dedicated
         # *   **normal_general**: genera-purpose
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-polardb20170801-py2
-Version: 4.0.7
+Version: 4.0.8
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.7/setup.py` & `alibabacloud_polardb20170801_py2-4.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_polardb20170801_py2.
 
-Created on 09/04/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_polardb20170801"
 NAME = "alibabacloud_polardb20170801_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2"
```

