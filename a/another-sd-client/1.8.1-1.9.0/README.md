# Comparing `tmp/another_sd_client-1.8.1.tar.gz` & `tmp/another_sd_client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.8.1.tar", max compression
+gzip compressed data, was "another_sd_client-1.9.0.tar", max compression
```

## Comparing `another_sd_client-1.8.1.tar` & `another_sd_client-1.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6296 2024-02-08 08:24:29.846416 another_sd_client-1.8.1/README.md
--rw-r--r--   0        0        0      950 2024-02-08 08:24:31.324537 another_sd_client-1.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-08 08:24:29.888419 another_sd_client-1.8.1/sdclient/__init__.py
--rw-r--r--   0        0        0     5018 2024-02-08 08:24:29.847416 another_sd_client-1.8.1/sdclient/client.py
--rw-r--r--   0        0        0     1017 2024-02-08 08:24:29.848416 another_sd_client-1.8.1/sdclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-08 08:24:29.888419 another_sd_client-1.8.1/sdclient/py.typed
--rw-r--r--   0        0        0     5281 2024-02-08 08:24:29.848416 another_sd_client-1.8.1/sdclient/requests.py
--rw-r--r--   0        0        0     2975 2024-02-08 08:24:29.848416 another_sd_client-1.8.1/sdclient/responses.py
--rw-r--r--   0        0        0     7033 1970-01-01 00:00:00.000000 another_sd_client-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     6296 2024-03-22 10:58:13.562756 another_sd_client-1.9.0/README.md
+-rw-r--r--   0        0        0      950 2024-03-22 10:58:14.302806 another_sd_client-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 10:58:13.620760 another_sd_client-1.9.0/sdclient/__init__.py
+-rw-r--r--   0        0        0     5517 2024-03-22 10:58:13.563757 another_sd_client-1.9.0/sdclient/client.py
+-rw-r--r--   0        0        0     1017 2024-03-22 10:58:13.563757 another_sd_client-1.9.0/sdclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:58:13.620760 another_sd_client-1.9.0/sdclient/py.typed
+-rw-r--r--   0        0        0     5564 2024-03-22 10:58:13.563757 another_sd_client-1.9.0/sdclient/requests.py
+-rw-r--r--   0        0        0     3206 2024-03-22 10:58:13.564756 another_sd_client-1.9.0/sdclient/responses.py
+-rw-r--r--   0        0        0     7033 1970-01-01 00:00:00.000000 another_sd_client-1.9.0/PKG-INFO
```

### Comparing `another_sd_client-1.8.1/README.md` & `another_sd_client-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.8.1/pyproject.toml` & `another_sd_client-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "another-sd-client"
-version = "1.8.1"
+version = "1.9.0"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
```

### Comparing `another_sd_client-1.8.1/sdclient/client.py` & `another_sd_client-1.9.0/sdclient/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from pyexpat import ExpatError
 from typing import OrderedDict
 from typing import Tuple
 
 import httpx
 import xmltodict
 from httpx import HTTPError
 from httpx import HTTPStatusError
 from httpx import StreamError
 
 from sdclient.exceptions import SDCallError
 from sdclient.exceptions import SDHTTPStatusError
 from sdclient.exceptions import SDParseResponseError
+from sdclient.requests import GetDepartmentParentRequest
 from sdclient.requests import GetDepartmentRequest
 from sdclient.requests import GetEmploymentRequest
 from sdclient.requests import GetOrganizationRequest
 from sdclient.requests import SDRequest
+from sdclient.responses import GetDepartmentParentResponse
 from sdclient.responses import GetDepartmentResponse
 from sdclient.responses import GetEmploymentResponse
 from sdclient.responses import GetOrganizationResponse
 
 
 class SDClient:
     BASE_URL = "https://service.sd.dk/sdws/"
-    ENDPOINT_SUFFIX = "20111201"
 
     def __init__(self, sd_username: str, sd_password: str, timeout: int = 120):
         self.username = sd_username
         self.password = sd_password
         self.timeout = timeout
 
     def _call_sd(
@@ -47,15 +47,15 @@
                 which MUST be lists. This ensures that the SD OrderedDicts
                 are compatible with the SD response Pydantic models
         Returns:
             XML response from SD in the form of an OrderedDict
         """
 
         # Get the endpoint name, e.g. "GetEmployment20111201"
-        endpoint_name = query_params.get_name() + SDClient.ENDPOINT_SUFFIX
+        endpoint_name = query_params.get_name()
 
         try:
             response = httpx.get(
                 SDClient.BASE_URL + endpoint_name,
                 params=query_params.to_query_params(),
                 auth=(self.username, self.password),
                 timeout=self.timeout,
@@ -143,7 +143,23 @@
             XML response from SD converted to Pydantic
         """
 
         root_elem = self._call_sd(
             query_params, xml_force_list=("DepartmentReference", "Organization")
         )
         return GetOrganizationResponse.parse_obj(root_elem)
+
+    def get_department_parent(
+        self, query_params: GetDepartmentParentRequest
+    ) -> GetDepartmentParentResponse:
+        """
+        Call the SD endpoint GetDepartmentParent.
+
+        Args:
+            query_params: The HTTP query parameters to set in the request
+
+        Returns:
+            XML response from SD converted to Pydantic
+        """
+
+        root_elem = self._call_sd(query_params)
+        return GetDepartmentParentResponse.parse_obj(root_elem)
```

### Comparing `another_sd_client-1.8.1/sdclient/exceptions.py` & `another_sd_client-1.9.0/sdclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.8.1/sdclient/requests.py` & `another_sd_client-1.9.0/sdclient/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             raise ValueError(
                 "ProductionUnitIndicator requires PostalAddressIndicator to be true"
             )
 
         return values
 
     def get_name(self):
-        return "GetDepartment"
+        return "GetDepartment20111201"
 
 
 class GetEmploymentRequest(SDRequest):
     """
     Query parameters for SDs GetEmployment20111201 endpoint
     """
 
@@ -102,15 +102,15 @@
     SalaryAgreementIndicator: bool = False
     SalaryCodeGroupIndicator: bool = False
     WorkingTimeIndicator: bool = False
     UUIDIndicator: bool = False
 
     # TODO: add validator (not enough to set StatusActiveIndicator...)
     def get_name(self):
-        return "GetEmployment"
+        return "GetEmployment20111201"
 
 
 class GetOrganizationRequest(SDRequest):
     """
     Query parameters for SDs GetOrganization20111201 endpoint
     """
 
@@ -146,8 +146,20 @@
             raise ValueError(
                 "ActivationDate must be less than or equal to DeactivationDate"
             )
 
         return values
 
     def get_name(self):
-        return "GetOrganization"
+        return "GetOrganization20111201"
+
+
+class GetDepartmentParentRequest(SDRequest):
+    """
+    Query parameters for the GetDepartmentParent20190701 endpoint
+    """
+
+    EffectiveDate: date
+    DepartmentUUIDIdentifier: UUID
+
+    def get_name(self):
+        return "GetDepartmentParent20190701"
```

### Comparing `another_sd_client-1.8.1/sdclient/responses.py` & `another_sd_client-1.9.0/sdclient/responses.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,7 +115,19 @@
     RegionUUIDIdentifier: UUID | None = None
     InstitutionIdentifier: str
     InstitutionUUIDIdentifier: UUID | None = None
     DepartmentStructureName: str
 
     OrganizationStructure: DepartmentLevelReference
     Organization: list[OrganizationModel] = []
+
+
+class DepartmentParent(BaseModel):
+    DepartmentUUIDIdentifier: UUID
+
+
+class GetDepartmentParentResponse(BaseModel):
+    """
+    Response model for SDs GetDepartmentParent20190701
+    """
+
+    DepartmentParent: DepartmentParent
```

### Comparing `another_sd_client-1.8.1/PKG-INFO` & `another_sd_client-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.8.1
+Version: 1.9.0
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

