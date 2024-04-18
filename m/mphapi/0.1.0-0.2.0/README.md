# Comparing `tmp/mphapi-0.1.0.tar.gz` & `tmp/mphapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mphapi-0.1.0.tar", max compression
+gzip compressed data, was "mphapi-0.2.0.tar", max compression
```

## Comparing `mphapi-0.1.0.tar` & `mphapi-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      210 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/__init__.py
--rw-r--r--   0        0        0    10561 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/claim.py
--rw-r--r--   0        0        0     6297 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/client.py
--rw-r--r--   0        0        0     1504 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/date.py
--rw-r--r--   0        0        0    11445 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/pricing.py
--rw-r--r--   0        0        0     2958 2024-04-08 21:43:22.845085 mphapi-0.1.0/mphapi/response.py
--rw-r--r--   0        0        0      342 2024-04-08 21:43:22.845085 mphapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mphapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      210 2024-04-10 01:49:16.715908 mphapi-0.2.0/mphapi/__init__.py
+-rw-r--r--   0        0        0    10567 2024-04-18 05:33:37.948236 mphapi-0.2.0/mphapi/claim.py
+-rw-r--r--   0        0        0     6297 2024-04-10 01:49:16.715908 mphapi-0.2.0/mphapi/client.py
+-rw-r--r--   0        0        0     1504 2024-04-10 01:49:16.715908 mphapi-0.2.0/mphapi/date.py
+-rw-r--r--   0        0        0     9776 2024-04-18 05:33:37.948236 mphapi-0.2.0/mphapi/pricing.py
+-rw-r--r--   0        0        0     2958 2024-04-10 01:49:16.715908 mphapi-0.2.0/mphapi/response.py
+-rw-r--r--   0        0        0      342 2024-04-18 05:33:37.948236 mphapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 mphapi-0.2.0/PKG-INFO
```

### Comparing `mphapi-0.1.0/mphapi/claim.py` & `mphapi-0.2.0/mphapi/claim.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     rev_code: Optional[str] = None
     """Revenue code (from SV2_01)"""
 
     procedure_code: Optional[str] = None
     """Procedure code (from SV101_02 / SV202_02)"""
 
-    procedure_modifiers: Optional[str] = None
+    procedure_modifiers: Optional[list[str]] = None
     """Procedure modifiers (from SV101_03, 4, 5, 6 / SV202_03, 4, 5, 6)"""
 
     drug_code: Optional[str] = None
     """National Drug Code (from LIN03)"""
 
     date_from: Optional[Date] = None
     """Begin date of service (from DTP 472)"""
```

### Comparing `mphapi-0.1.0/mphapi/client.py` & `mphapi-0.2.0/mphapi/client.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.1.0/mphapi/date.py` & `mphapi-0.2.0/mphapi/date.py`

 * *Files identical despite different names*

### Comparing `mphapi-0.1.0/mphapi/pricing.py` & `mphapi-0.2.0/mphapi/pricing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
-from typing import Any, Optional
+from typing import Optional
 
-from pydantic import BaseModel, Field, GetCoreSchemaHandler
-from pydantic_core import core_schema
+from pydantic import BaseModel, Field
 
 from .claim import Service, camel_case_model_config
 from .response import ResponseError
 
 
 class ClaimRepricingCode(str, Enum):
     """claim-level repricing codes"""
@@ -111,59 +110,14 @@
 
 
 class RuralIndicator(str, Enum):
     RURAL = "R"
     SUPER_RURAL = "B"
     URBAN = ""
 
-    @classmethod
-    def __get_pydantic_core_schema__(
-        cls,
-        _source_type: Any,
-        _handler: GetCoreSchemaHandler,
-    ) -> core_schema.CoreSchema:
-        def from_int(value: int) -> RuralIndicator:
-            if value == 82:
-                return RuralIndicator.RURAL
-            elif value == 66:
-                return RuralIndicator.SUPER_RURAL
-            elif value == 32:
-                return RuralIndicator.URBAN
-            else:
-                raise ValueError(f"Unknown rural indicator value: {value}")
-
-        def to_int(instance: RuralIndicator) -> int:
-            if instance == RuralIndicator.RURAL:
-                return 82
-            elif instance == RuralIndicator.SUPER_RURAL:
-                return 66
-            elif instance == RuralIndicator.URBAN:
-                return 32
-            else:
-                raise ValueError(f"Unknown rural indicator: {instance}")
-
-        from_int_schema = core_schema.chain_schema(
-            [
-                core_schema.int_schema(),
-                core_schema.no_info_plain_validator_function(from_int),
-            ]
-        )
-
-        return core_schema.json_or_python_schema(
-            json_schema=from_int_schema,
-            python_schema=core_schema.union_schema(
-                [
-                    # check if it's an instance first before doing any further work
-                    core_schema.is_instance_schema(RuralIndicator),
-                    from_int_schema,
-                ]
-            ),
-            serialization=core_schema.plain_serializer_function_ser_schema(to_int),
-        )
-
 
 class ProviderDetail(BaseModel):
     """
     ProviderDetail contains basic information about the provider and/or locality used for pricing.
     Not all fields are returned with every pricing request. For example, the CMS Certification
     Number (CCN) is only returned for facilities which have a CCN such as hospitals.
     """
```

### Comparing `mphapi-0.1.0/mphapi/response.py` & `mphapi-0.2.0/mphapi/response.py`

 * *Files identical despite different names*

