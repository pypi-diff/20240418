# Comparing `tmp/alibabacloud_foasconsole20211028_py2-1.0.2.tar.gz` & `tmp/alibabacloud_foasconsole20211028_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_foasconsole20211028_py2-1.0.2.tar", last modified: Thu Mar  7 17:09:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_foasconsole20211028_py2-1.0.3.tar", last modified: Thu Apr 18 17:10:43 2024, max compression
```

## Comparing `alibabacloud_foasconsole20211028_py2-1.0.2.tar` & `alibabacloud_foasconsole20211028_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      145 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36446 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/client.py
--rw-r--r--   0 root         (0) root         (0)   183353 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-07 17:09:18.000000 alibabacloud_foasconsole20211028_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2943 2024-03-07 17:09:17.000000 alibabacloud_foasconsole20211028_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1815 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36712 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/client.py
+-rw-r--r--   0 root         (0) root         (0)   199246 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-18 17:10:43.000000 alibabacloud_foasconsole20211028_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/LICENSE` & `alibabacloud_foasconsole20211028_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/PKG-INFO` & `alibabacloud_foasconsole20211028_py2-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_foasconsole20211028_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20211028) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/README-CN.md` & `alibabacloud_foasconsole20211028_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/README.md` & `alibabacloud_foasconsole20211028_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/client.py` & `alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
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
@@ -117,14 +119,16 @@
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

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028/models.py` & `alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -345,19 +345,48 @@
         m = m or dict()
         if m.get('Oss') is not None:
             temp_model = CreateInstanceRequestStorageOss()
             self.oss = temp_model.from_map(m['Oss'])
         return self
 
 
+class CreateInstanceRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateInstanceRequestTag, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateInstanceRequest(TeaModel):
     def __init__(self, architecture_type=None, auto_renew=None, charge_type=None, duration=None, extra=None, ha=None,
                  ha_resource_spec=None, ha_vswitch_ids=None, ha_zone_id=None, instance_name=None, monitor_type=None,
                  pricing_cycle=None, promotion_code=None, region=None, resource_group_id=None, resource_spec=None, storage=None,
-                 use_promotion_code=None, v_switch_ids=None, vpc_id=None, zone_id=None):
+                 tag=None, use_promotion_code=None, v_switch_ids=None, vpc_id=None, zone_id=None):
         self.architecture_type = architecture_type  # type: str
         self.auto_renew = auto_renew  # type: bool
         self.charge_type = charge_type  # type: str
         self.duration = duration  # type: int
         self.extra = extra  # type: str
         self.ha = ha  # type: bool
         self.ha_resource_spec = ha_resource_spec  # type: CreateInstanceRequestHaResourceSpec
@@ -367,26 +396,31 @@
         self.monitor_type = monitor_type  # type: str
         self.pricing_cycle = pricing_cycle  # type: str
         self.promotion_code = promotion_code  # type: str
         self.region = region  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.resource_spec = resource_spec  # type: CreateInstanceRequestResourceSpec
         self.storage = storage  # type: CreateInstanceRequestStorage
+        self.tag = tag  # type: list[CreateInstanceRequestTag]
         self.use_promotion_code = use_promotion_code  # type: bool
         self.v_switch_ids = v_switch_ids  # type: list[str]
         self.vpc_id = vpc_id  # type: str
         self.zone_id = zone_id  # type: str
 
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
         _map = super(CreateInstanceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -420,14 +454,18 @@
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
@@ -469,14 +507,19 @@
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
@@ -484,15 +527,16 @@
         return self
 
 
 class CreateInstanceShrinkRequest(TeaModel):
     def __init__(self, architecture_type=None, auto_renew=None, charge_type=None, duration=None, extra=None, ha=None,
                  ha_resource_spec_shrink=None, ha_vswitch_ids_shrink=None, ha_zone_id=None, instance_name=None, monitor_type=None,
                  pricing_cycle=None, promotion_code=None, region=None, resource_group_id=None, resource_spec_shrink=None,
-                 storage_shrink=None, use_promotion_code=None, v_switch_ids_shrink=None, vpc_id=None, zone_id=None):
+                 storage_shrink=None, tag_shrink=None, use_promotion_code=None, v_switch_ids_shrink=None, vpc_id=None,
+                 zone_id=None):
         self.architecture_type = architecture_type  # type: str
         self.auto_renew = auto_renew  # type: bool
         self.charge_type = charge_type  # type: str
         self.duration = duration  # type: int
         self.extra = extra  # type: str
         self.ha = ha  # type: bool
         self.ha_resource_spec_shrink = ha_resource_spec_shrink  # type: str
@@ -502,14 +546,15 @@
         self.monitor_type = monitor_type  # type: str
         self.pricing_cycle = pricing_cycle  # type: str
         self.promotion_code = promotion_code  # type: str
         self.region = region  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.resource_spec_shrink = resource_spec_shrink  # type: str
         self.storage_shrink = storage_shrink  # type: str
+        self.tag_shrink = tag_shrink  # type: str
         self.use_promotion_code = use_promotion_code  # type: bool
         self.v_switch_ids_shrink = v_switch_ids_shrink  # type: str
         self.vpc_id = vpc_id  # type: str
         self.zone_id = zone_id  # type: str
 
     def validate(self):
         pass
@@ -550,14 +595,16 @@
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
@@ -596,14 +643,16 @@
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
@@ -3134,14 +3183,64 @@
         if m.get('PricingCycle') is not None:
             self.pricing_cycle = m.get('PricingCycle')
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
+class QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -3203,26 +3302,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryConvertInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryConvertInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -3234,54 +3340,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -3680,14 +3803,64 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
+class QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -3749,26 +3922,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryCreateInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryCreateInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -3780,54 +3960,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -4070,14 +4267,64 @@
         if m.get('Region') is not None:
             self.region = m.get('Region')
         if m.get('ResourceSpec') is not None:
             self.resource_spec_shrink = m.get('ResourceSpec')
         return self
 
 
+class QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -4139,26 +4386,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryModifyInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryModifyInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -4170,54 +4424,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -4326,14 +4597,64 @@
         if m.get('PricingCycle') is not None:
             self.pricing_cycle = m.get('PricingCycle')
         if m.get('Region') is not None:
             self.region = m.get('Region')
         return self
 
 
+class QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -4395,26 +4716,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryRenewInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryRenewInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -4426,54 +4754,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
```

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/alibabacloud_foasconsole20211028_py2.egg-info/PKG-INFO` & `alibabacloud_foasconsole20211028_py2-1.0.3/alibabacloud_foasconsole20211028_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-foasconsole20211028-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20211028) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20211028_py2-1.0.2/setup.py` & `alibabacloud_foasconsole20211028_py2-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_foasconsole20211028_py2.
 
-Created on 07/03/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_foasconsole20211028"
 NAME = "alibabacloud_foasconsole20211028_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud foasconsole (20211028) SDK Library for Python2"
```

