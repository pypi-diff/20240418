# Comparing `tmp/airbyte_source_salesforce-2.5.2.tar.gz` & `tmp/airbyte_source_salesforce-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.5.2.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.5.3.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.5.2.tar` & `airbyte_source_salesforce-2.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/README.md
--rw-r--r--   0        0        0      826 2024-04-15 13:05:24.893506 airbyte_source_salesforce-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/__init__.py
--rw-r--r--   0        0        0    17451 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/api.py
--rw-r--r--   0        0        0     1621 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3946 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    15225 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    41478 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-04-15 13:01:59.401905 airbyte_source_salesforce-2.5.2/source_salesforce/utils.py
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/README.md
+-rw-r--r--   0        0        0      826 2024-04-17 14:25:35.121389 airbyte_source_salesforce-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    17451 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/api.py
+-rw-r--r--   0        0        0     1621 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/run.py
+-rw-r--r--   0        0        0     9747 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    15502 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41478 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-04-17 13:10:59.000000 airbyte_source_salesforce-2.5.3/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.3/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.5.2/README.md` & `airbyte_source_salesforce-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/pyproject.toml` & `airbyte_source_salesforce-2.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.2"
+version = "2.5.3"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/api.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/run.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.5.3/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/source.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 error_data = error.response.json()[0]
             except (KeyError, requests.exceptions.JSONDecodeError):
                 pass
             else:
                 error_code = error_data.get("errorCode")
                 if error.response.status_code == codes.FORBIDDEN and error_code == "REQUEST_LIMIT_EXCEEDED":
                     logger.warn(f"API Call limit is exceeded. Error message: '{error_data.get('message')}'")
-                    error_msg = "API Call limit is exceeded"
+                    error_msg = "API Call limit is exceeded. Make sure that you have enough API allocation for your organization needs or retry later. For more information, see https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm"
             return False, error_msg
         return True, None
 
     @classmethod
     def _get_api_type(cls, stream_name: str, json_schema: Mapping[str, Any], force_use_bulk_api: bool) -> str:
         """Get proper API type: rest or bulk"""
         # Salesforce BULK API currently does not support loading fields with data type base64 and compound data
```

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.5.3/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/streams.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/source_salesforce/utils.py` & `airbyte_source_salesforce-2.5.3/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.5.2/PKG-INFO` & `airbyte_source_salesforce-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.5.2
+Version: 2.5.3
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

