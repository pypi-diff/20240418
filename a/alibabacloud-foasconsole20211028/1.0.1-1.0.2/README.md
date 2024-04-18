# Comparing `tmp/alibabacloud_foasconsole20211028-1.0.1.tar.gz` & `tmp/alibabacloud_foasconsole20211028-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_foasconsole20211028-1.0.1.tar", last modified: Thu Mar  7 17:08:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_foasconsole20211028-1.0.2.tar", last modified: Thu Apr 18 17:13:56 2024, max compression
```

## Comparing `alibabacloud_foasconsole20211028-1.0.1.tar` & `alibabacloud_foasconsole20211028-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       74 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83988 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/client.py
--rw-r--r--   0 root         (0) root         (0)   181665 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-07 17:08:53.000000 alibabacloud_foasconsole20211028-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84520 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/client.py
+-rw-r--r--   0 root         (0) root         (0)   197318 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-18 17:13:56.000000 alibabacloud_foasconsole20211028-1.0.2/setup.py
```

### Comparing `alibabacloud_foasconsole20211028-1.0.1/LICENSE` & `alibabacloud_foasconsole20211028-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028-1.0.1/PKG-INFO` & `alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_foasconsole20211028
-Version: 1.0.1
+Name: alibabacloud-foasconsole20211028
+Version: 1.0.2
 Summary: Alibaba Cloud foasconsole (20211028) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20211028-1.0.1/README-CN.md` & `alibabacloud_foasconsole20211028-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028-1.0.1/README.md` & `alibabacloud_foasconsole20211028-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/client.py` & `alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,16 @@
             request.ha_resource_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ha_resource_spec, 'HaResourceSpec', 'json')
         if not UtilClient.is_unset(tmp_req.ha_vswitch_ids):
             request.ha_vswitch_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ha_vswitch_ids, 'HaVSwitchIds', 'json')
         if not UtilClient.is_unset(tmp_req.resource_spec):
             request.resource_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_spec, 'ResourceSpec', 'json')
         if not UtilClient.is_unset(tmp_req.storage):
             request.storage_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage, 'Storage', 'json')
+        if not UtilClient.is_unset(tmp_req.tag):
+            request.tag_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag, 'Tag', 'json')
         if not UtilClient.is_unset(tmp_req.v_switch_ids):
             request.v_switch_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.v_switch_ids, 'VSwitchIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.architecture_type):
             body['ArchitectureType'] = request.architecture_type
         if not UtilClient.is_unset(request.auto_renew):
             body['AutoRenew'] = request.auto_renew
@@ -188,14 +190,16 @@
             body['Region'] = request.region
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_spec_shrink):
             body['ResourceSpec'] = request.resource_spec_shrink
         if not UtilClient.is_unset(request.storage_shrink):
             body['Storage'] = request.storage_shrink
+        if not UtilClient.is_unset(request.tag_shrink):
+            body['Tag'] = request.tag_shrink
         if not UtilClient.is_unset(request.use_promotion_code):
             body['UsePromotionCode'] = request.use_promotion_code
         if not UtilClient.is_unset(request.v_switch_ids_shrink):
             body['VSwitchIds'] = request.v_switch_ids_shrink
         if not UtilClient.is_unset(request.vpc_id):
             body['VpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.zone_id):
@@ -231,14 +235,16 @@
             request.ha_resource_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ha_resource_spec, 'HaResourceSpec', 'json')
         if not UtilClient.is_unset(tmp_req.ha_vswitch_ids):
             request.ha_vswitch_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ha_vswitch_ids, 'HaVSwitchIds', 'json')
         if not UtilClient.is_unset(tmp_req.resource_spec):
             request.resource_spec_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_spec, 'ResourceSpec', 'json')
         if not UtilClient.is_unset(tmp_req.storage):
             request.storage_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.storage, 'Storage', 'json')
+        if not UtilClient.is_unset(tmp_req.tag):
+            request.tag_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag, 'Tag', 'json')
         if not UtilClient.is_unset(tmp_req.v_switch_ids):
             request.v_switch_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.v_switch_ids, 'VSwitchIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.architecture_type):
             body['ArchitectureType'] = request.architecture_type
         if not UtilClient.is_unset(request.auto_renew):
             body['AutoRenew'] = request.auto_renew
@@ -268,14 +274,16 @@
             body['Region'] = request.region
         if not UtilClient.is_unset(request.resource_group_id):
             body['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_spec_shrink):
             body['ResourceSpec'] = request.resource_spec_shrink
         if not UtilClient.is_unset(request.storage_shrink):
             body['Storage'] = request.storage_shrink
+        if not UtilClient.is_unset(request.tag_shrink):
+            body['Tag'] = request.tag_shrink
         if not UtilClient.is_unset(request.use_promotion_code):
             body['UsePromotionCode'] = request.use_promotion_code
         if not UtilClient.is_unset(request.v_switch_ids_shrink):
             body['VSwitchIds'] = request.v_switch_ids_shrink
         if not UtilClient.is_unset(request.vpc_id):
             body['VpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.zone_id):
```

### Comparing `alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028/models.py` & `alibabacloud_foasconsole20211028-1.0.2/alibabacloud_foasconsole20211028/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -392,14 +392,47 @@
         m = m or dict()
         if m.get('Oss') is not None:
             temp_model = CreateInstanceRequestStorageOss()
             self.oss = temp_model.from_map(m['Oss'])
         return self
 
 
+class CreateInstanceRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateInstanceRequest(TeaModel):
     def __init__(
         self,
         architecture_type: str = None,
         auto_renew: bool = None,
         charge_type: str = None,
         duration: int = None,
@@ -412,14 +445,15 @@
         monitor_type: str = None,
         pricing_cycle: str = None,
         promotion_code: str = None,
         region: str = None,
         resource_group_id: str = None,
         resource_spec: CreateInstanceRequestResourceSpec = None,
         storage: CreateInstanceRequestStorage = None,
+        tag: List[CreateInstanceRequestTag] = None,
         use_promotion_code: bool = None,
         v_switch_ids: List[str] = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
         self.architecture_type = architecture_type
         self.auto_renew = auto_renew
@@ -434,26 +468,31 @@
         self.monitor_type = monitor_type
         self.pricing_cycle = pricing_cycle
         self.promotion_code = promotion_code
         self.region = region
         self.resource_group_id = resource_group_id
         self.resource_spec = resource_spec
         self.storage = storage
+        self.tag = tag
         self.use_promotion_code = use_promotion_code
         self.v_switch_ids = v_switch_ids
         self.vpc_id = vpc_id
         self.zone_id = zone_id
 
     def validate(self):
         if self.ha_resource_spec:
             self.ha_resource_spec.validate()
         if self.resource_spec:
             self.resource_spec.validate()
         if self.storage:
             self.storage.validate()
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -487,14 +526,18 @@
             result['Region'] = self.region
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.resource_spec is not None:
             result['ResourceSpec'] = self.resource_spec.to_map()
         if self.storage is not None:
             result['Storage'] = self.storage.to_map()
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.use_promotion_code is not None:
             result['UsePromotionCode'] = self.use_promotion_code
         if self.v_switch_ids is not None:
             result['VSwitchIds'] = self.v_switch_ids
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         if self.zone_id is not None:
@@ -536,14 +579,19 @@
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceSpec') is not None:
             temp_model = CreateInstanceRequestResourceSpec()
             self.resource_spec = temp_model.from_map(m['ResourceSpec'])
         if m.get('Storage') is not None:
             temp_model = CreateInstanceRequestStorage()
             self.storage = temp_model.from_map(m['Storage'])
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateInstanceRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('UsePromotionCode') is not None:
             self.use_promotion_code = m.get('UsePromotionCode')
         if m.get('VSwitchIds') is not None:
             self.v_switch_ids = m.get('VSwitchIds')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('ZoneId') is not None:
@@ -567,14 +615,15 @@
         monitor_type: str = None,
         pricing_cycle: str = None,
         promotion_code: str = None,
         region: str = None,
         resource_group_id: str = None,
         resource_spec_shrink: str = None,
         storage_shrink: str = None,
+        tag_shrink: str = None,
         use_promotion_code: bool = None,
         v_switch_ids_shrink: str = None,
         vpc_id: str = None,
         zone_id: str = None,
     ):
         self.architecture_type = architecture_type
         self.auto_renew = auto_renew
@@ -589,14 +638,15 @@
         self.monitor_type = monitor_type
         self.pricing_cycle = pricing_cycle
         self.promotion_code = promotion_code
         self.region = region
         self.resource_group_id = resource_group_id
         self.resource_spec_shrink = resource_spec_shrink
         self.storage_shrink = storage_shrink
+        self.tag_shrink = tag_shrink
         self.use_promotion_code = use_promotion_code
         self.v_switch_ids_shrink = v_switch_ids_shrink
         self.vpc_id = vpc_id
         self.zone_id = zone_id
 
     def validate(self):
         pass
@@ -637,14 +687,16 @@
             result['Region'] = self.region
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.resource_spec_shrink is not None:
             result['ResourceSpec'] = self.resource_spec_shrink
         if self.storage_shrink is not None:
             result['Storage'] = self.storage_shrink
+        if self.tag_shrink is not None:
+            result['Tag'] = self.tag_shrink
         if self.use_promotion_code is not None:
             result['UsePromotionCode'] = self.use_promotion_code
         if self.v_switch_ids_shrink is not None:
             result['VSwitchIds'] = self.v_switch_ids_shrink
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         if self.zone_id is not None:
@@ -683,14 +735,16 @@
             self.region = m.get('Region')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceSpec') is not None:
             self.resource_spec_shrink = m.get('ResourceSpec')
         if m.get('Storage') is not None:
             self.storage_shrink = m.get('Storage')
+        if m.get('Tag') is not None:
+            self.tag_shrink = m.get('Tag')
         if m.get('UsePromotionCode') is not None:
             self.use_promotion_code = m.get('UsePromotionCode')
         if m.get('VSwitchIds') is not None:
             self.v_switch_ids_shrink = m.get('VSwitchIds')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('ZoneId') is not None:
@@ -3568,14 +3622,71 @@
         if m.get('PricingCycle') is not None:
             self.pricing_cycle = m.get('PricingCycle')
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
+class QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -3651,31 +3762,41 @@
 
 
 class QueryConvertInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryConvertInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -3687,54 +3808,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryConvertInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryConvertInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4190,14 +4328,71 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
+class QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -4273,31 +4468,41 @@
 
 
 class QueryCreateInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryCreateInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -4309,54 +4514,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryCreateInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryCreateInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4633,14 +4855,71 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         if m.get('ResourceSpec') is not None:
             self.resource_spec_shrink = m.get('ResourceSpec')
         return self
 
 
+class QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -4716,31 +4995,41 @@
 
 
 class QueryModifyInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryModifyInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -4752,54 +5041,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryModifyInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryModifyInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4924,14 +5230,71 @@
         if m.get('PricingCycle') is not None:
             self.pricing_cycle = m.get('PricingCycle')
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
+class QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -5007,31 +5370,41 @@
 
 
 class QueryRenewInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryRenewInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -5043,54 +5416,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryRenewInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryRenewInstancePriceResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_foasconsole20211028-1.0.1/alibabacloud_foasconsole20211028.egg-info/PKG-INFO` & `alibabacloud_foasconsole20211028-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-foasconsole20211028
-Version: 1.0.1
+Name: alibabacloud_foasconsole20211028
+Version: 1.0.2
 Summary: Alibaba Cloud foasconsole (20211028) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20211028-1.0.1/setup.py` & `alibabacloud_foasconsole20211028-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_foasconsole20211028.
 
-Created on 07/03/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_foasconsole20211028"
 NAME = "alibabacloud_foasconsole20211028" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud foasconsole (20211028) SDK Library for Python"
```

