# Comparing `tmp/mytoyota-2.1.1.tar.gz` & `tmp/mytoyota-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytoyota-2.1.1.tar", max compression
+gzip compressed data, was "mytoyota-2.1.2.tar", max compression
```

## Comparing `mytoyota-2.1.1.tar` & `mytoyota-2.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1090 2024-03-28 14:27:43.425545 mytoyota-2.1.1/LICENSE
--rw-r--r--   0        0        0     3183 2024-03-28 14:27:43.425545 mytoyota-2.1.1/README.md
--rw-r--r--   0        0        0      153 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/__init__.py
--rw-r--r--   0        0        0    10086 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/api.py
--rw-r--r--   0        0        0     2038 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/client.py
--rw-r--r--   0        0        0     1389 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/const.py
--rw-r--r--   0        0        0    11447 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/controller.py
--rw-r--r--   0        0        0      630 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/exceptions.py
--rw-r--r--   0        0        0     6354 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/dashboard.py
--rw-r--r--   0        0        0     2483 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/account.py
--rw-r--r--   0        0        0     1399 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/common.py
--rw-r--r--   0        0        0     2168 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/electric.py
--rw-r--r--   0        0        0     1476 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/location.py
--rw-r--r--   0        0        0     2364 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/notifications.py
--rw-r--r--   0        0        0     2390 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/service_history.py
--rw-r--r--   0        0        0     2650 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/status.py
--rw-r--r--   0        0        0     1265 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/telemetry.py
--rw-r--r--   0        0        0     6992 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/trips.py
--rw-r--r--   0        0        0    24998 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/vehicle_guid.py
--rw-r--r--   0        0        0     1342 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/endpoints/vehicle_health.py
--rw-r--r--   0        0        0     1794 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/location.py
--rw-r--r--   0        0        0     8449 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/lock_status.py
--rw-r--r--   0        0        0     1776 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/nofication.py
--rw-r--r--   0        0        0     3502 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/service_history.py
--rw-r--r--   0        0        0     5328 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/summary.py
--rw-r--r--   0        0        0     4690 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/trips.py
--rw-r--r--   0        0        0    19334 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/models/vehicle.py
--rw-r--r--   0        0        0        0 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/py.typed
--rw-r--r--   0        0        0       30 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/__init__.py
--rw-r--r--   0        0        0     1339 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/conversions.py
--rw-r--r--   0        0        0      374 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/formatters.py
--rw-r--r--   0        0        0      261 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/helpers.py
--rw-r--r--   0        0        0      368 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/locale.py
--rw-r--r--   0        0        0     4291 2024-03-28 14:27:43.425545 mytoyota-2.1.1/mytoyota/utils/log_utils.py
--rw-r--r--   0        0        0     1973 2024-03-28 14:27:56.713817 mytoyota-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 mytoyota-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-18 06:13:11.520937 mytoyota-2.1.2/LICENSE
+-rw-r--r--   0        0        0     3183 2024-04-18 06:13:11.520937 mytoyota-2.1.2/README.md
+-rw-r--r--   0        0        0      153 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/__init__.py
+-rw-r--r--   0        0        0    10086 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/api.py
+-rw-r--r--   0        0        0     2038 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/client.py
+-rw-r--r--   0        0        0     1389 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/const.py
+-rw-r--r--   0        0        0    11447 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/controller.py
+-rw-r--r--   0        0        0      630 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/exceptions.py
+-rw-r--r--   0        0        0     6418 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/dashboard.py
+-rw-r--r--   0        0        0     2483 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/account.py
+-rw-r--r--   0        0        0     1399 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/common.py
+-rw-r--r--   0        0        0     2188 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/electric.py
+-rw-r--r--   0        0        0     1476 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/location.py
+-rw-r--r--   0        0        0     2364 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/notifications.py
+-rw-r--r--   0        0        0     2390 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/service_history.py
+-rw-r--r--   0        0        0     2650 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/status.py
+-rw-r--r--   0        0        0     1265 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/telemetry.py
+-rw-r--r--   0        0        0     6992 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/trips.py
+-rw-r--r--   0        0        0    25022 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/vehicle_guid.py
+-rw-r--r--   0        0        0     1342 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/endpoints/vehicle_health.py
+-rw-r--r--   0        0        0     1794 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/location.py
+-rw-r--r--   0        0        0     8449 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/lock_status.py
+-rw-r--r--   0        0        0     1776 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/nofication.py
+-rw-r--r--   0        0        0     3502 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/service_history.py
+-rw-r--r--   0        0        0     5328 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/summary.py
+-rw-r--r--   0        0        0     4690 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/trips.py
+-rw-r--r--   0        0        0    19334 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/models/vehicle.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/py.typed
+-rw-r--r--   0        0        0       30 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/__init__.py
+-rw-r--r--   0        0        0     1339 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/conversions.py
+-rw-r--r--   0        0        0      374 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/formatters.py
+-rw-r--r--   0        0        0      261 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/helpers.py
+-rw-r--r--   0        0        0      368 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/locale.py
+-rw-r--r--   0        0        0     4291 2024-04-18 06:13:11.520937 mytoyota-2.1.2/mytoyota/utils/log_utils.py
+-rw-r--r--   0        0        0     1973 2024-04-18 06:13:25.972925 mytoyota-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 mytoyota-2.1.2/PKG-INFO
```

### Comparing `mytoyota-2.1.1/LICENSE` & `mytoyota-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/README.md` & `mytoyota-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/api.py` & `mytoyota-2.1.2/mytoyota/api.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/client.py` & `mytoyota-2.1.2/mytoyota/client.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/const.py` & `mytoyota-2.1.2/mytoyota/const.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/controller.py` & `mytoyota-2.1.2/mytoyota/controller.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/exceptions.py` & `mytoyota-2.1.2/mytoyota/exceptions.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/dashboard.py` & `mytoyota-2.1.2/mytoyota/models/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         -------
             The range in the currently selected unit.
 
             If vehicle is fuel only returns None
             If vehicle doesn't support battery range returns None
 
         """
-        if self._electric:
+        if self._electric and self._electric.ev_range:
             return convert_distance(
                 self._distance_unit,
                 self._electric.ev_range.unit,
                 self._electric.ev_range.value,
             )
 
         return None
@@ -143,15 +143,15 @@
         -------
             The range in the currently selected unit.
 
             If vehicle is fuel only returns 0
             If vehicle doesn't support battery range returns 0
 
         """
-        if self._electric:
+        if self._electric and self._electric.ev_range_with_ac:
             return convert_distance(
                 self._distance_unit,
                 self._electric.ev_range_with_ac.unit,
                 self._electric.ev_range_with_ac.value,
             )
 
         return None
```

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/account.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/account.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/common.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/electric.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/electric.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     """
 
     battery_level: int = Field(alias="batteryLevel")
     can_set_next_charging_event: Optional[bool] = Field(
         alias="canSetNextChargingEvent", default=None
     )
     charging_status: str = Field(alias="chargingStatus")
-    ev_range: UnitValueModel = Field(alias="evRange")
-    ev_range_with_ac: UnitValueModel = Field(alias="evRangeWithAc")
+    ev_range: Optional[UnitValueModel] = Field(alias="evRange")
+    ev_range_with_ac: Optional[UnitValueModel] = Field(alias="evRangeWithAc")
     fuel_level: Optional[int] = Field(alias="fuelLevel", default=None)
     fuel_range: Optional[UnitValueModel] = Field(alias="fuelRange", default=None)
     last_update_timestamp: datetime = Field(alias="lastUpdateTimestamp")
     remaining_charge_time: Optional[int] = Field(
         alias="remainingChargeTime",
         default=None,
     )  # TODO: Use field serializer to create timedelta
```

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/location.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/notifications.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/notifications.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/service_history.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/service_history.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/status.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/status.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/telemetry.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/telemetry.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/trips.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/trips.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/vehicle_guid.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/vehicle_guid.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 class _DcmModel(BaseModel):  # Data connection model
     country_code: Optional[str] = Field(alias="countryCode", default=None)
     destination: str = Field(alias="dcmDestination")
     grade: str = Field(alias="dcmGrade")
     car_model_year: str = Field(alias="dcmModelYear")
     supplier: str = Field(alias="dcmSupplier")
-    supplier_name: str = Field(alias="dcmSupplierName")
+    supplier_name: Optional[str] = Field(alias="dcmSupplierName", default=None)
     euicc_id: str = Field(alias="euiccid")
     hardware_type: Optional[str] = Field(alias="hardwareType")
     vehicle_unit_terminal_number: Optional[str] = Field(alias="vehicleUnitTerminalNumber")
 
 
 class _HeadUnitModel(BaseModel):
     description: Optional[Any] = Field(alias="huDescription")  # TODO unsure what this returns
```

### Comparing `mytoyota-2.1.1/mytoyota/models/endpoints/vehicle_health.py` & `mytoyota-2.1.2/mytoyota/models/endpoints/vehicle_health.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/location.py` & `mytoyota-2.1.2/mytoyota/models/location.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/lock_status.py` & `mytoyota-2.1.2/mytoyota/models/lock_status.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/nofication.py` & `mytoyota-2.1.2/mytoyota/models/nofication.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/service_history.py` & `mytoyota-2.1.2/mytoyota/models/service_history.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/summary.py` & `mytoyota-2.1.2/mytoyota/models/summary.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/trips.py` & `mytoyota-2.1.2/mytoyota/models/trips.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/models/vehicle.py` & `mytoyota-2.1.2/mytoyota/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/utils/conversions.py` & `mytoyota-2.1.2/mytoyota/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/mytoyota/utils/log_utils.py` & `mytoyota-2.1.2/mytoyota/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `mytoyota-2.1.1/pyproject.toml` & `mytoyota-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "mytoyota"
 description = "Python client for Toyota Connected Services."
 authors = ["Simon Grud Hansen <simongrud@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-version = "2.1.1"
+version = "2.1.2"
 packages = [
   {include = "mytoyota"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
```

### Comparing `mytoyota-2.1.1/PKG-INFO` & `mytoyota-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytoyota
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python client for Toyota Connected Services.
 Home-page: https://github.com/DurgNomis-drol/mytoyota
 License: MIT
 Keywords: Toyota,Car,MYT
 Author: Simon Grud Hansen
 Author-email: simongrud@gmail.com
 Requires-Python: >=3.9,<4.0
```

