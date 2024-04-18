# Comparing `tmp/finite_state_sdk-0.1.6.tar.gz` & `tmp/finite_state_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finite_state_sdk-0.1.6.tar", max compression
+gzip compressed data, was "finite_state_sdk-0.1.7.tar", max compression
```

## Comparing `finite_state_sdk-0.1.6.tar` & `finite_state_sdk-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2024-03-29 20:05:40.406290 finite_state_sdk-0.1.6/LICENSE
--rw-r--r--   0        0        0     2053 2024-03-29 20:05:40.406388 finite_state_sdk-0.1.6/README.md
--rw-r--r--   0        0        0    95617 2024-04-10 18:42:22.531582 finite_state_sdk-0.1.6/finite_state_sdk/__init__.py
--rw-r--r--   0        0        0    24623 2024-04-10 18:42:22.532040 finite_state_sdk-0.1.6/finite_state_sdk/queries.py
--rw-r--r--   0        0        0     2634 2024-04-10 18:42:22.532375 finite_state_sdk-0.1.6/finite_state_sdk/token_cache.py
--rw-r--r--   0        0        0     3051 2024-04-10 19:16:33.477428 finite_state_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-03-29 20:05:40.406290 finite_state_sdk-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2053 2024-03-29 20:05:40.406388 finite_state_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0    97777 2024-04-17 18:34:29.708646 finite_state_sdk-0.1.7/finite_state_sdk/__init__.py
+-rw-r--r--   0        0        0    24623 2024-04-10 18:42:22.532040 finite_state_sdk-0.1.7/finite_state_sdk/queries.py
+-rw-r--r--   0        0        0     2634 2024-04-10 18:42:22.532375 finite_state_sdk-0.1.7/finite_state_sdk/token_cache.py
+-rw-r--r--   0        0        0     3016 2024-04-18 14:43:32.571041 finite_state_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.7/PKG-INFO
```

### Comparing `finite_state_sdk-0.1.6/LICENSE` & `finite_state_sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.6/README.md` & `finite_state_sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.6/finite_state_sdk/__init__.py` & `finite_state_sdk-0.1.7/finite_state_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,18 @@
 
     Raises:
         ValueError: Raised if business_unit_id, created_by_user_id, asset_id, or asset_version_name are not provided.
         Exception: Raised if the query fails.
 
     Returns:
         dict: createAssetVersion Object
+
+    deprecated:: 0.1.7. Use create_asset_version_on_asset instead.
     """
+    warn('`create_asset_version` is deprecated. Use: `create_asset_version_on_asset instead`', DeprecationWarning, stacklevel=2)
     if not business_unit_id:
         raise ValueError("Business unit ID is required")
     if not created_by_user_id:
         raise ValueError("Created by user ID is required")
     if not asset_id:
         raise ValueError("Asset ID is required")
     if not asset_version_name:
@@ -282,14 +285,69 @@
     if product_id is not None:
         variables["input"]["ctx"]["products"] = product_id
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
     return response['data']
 
 
+def create_asset_version_on_asset(
+    token,
+    organization_context,
+    created_by_user_id=None,
+    asset_id=None,
+    asset_version_name=None,
+):
+    """
+    Create a new Asset Version.
+
+    Args:
+        token (str):
+            Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
+        organization_context (str):
+            Organization context. This is provided by the Finite State API management. It looks like "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx".
+        created_by_user_id (str, optional):
+            User ID of the user creating the asset version.
+        asset_id (str, required):
+            Asset ID to associate the asset version with.
+        asset_version_name (str, required):
+            The name of the Asset Version being created.
+
+    Raises:
+        ValueError: Raised if business_unit_id, created_by_user_id, asset_id, or asset_version_name are not provided.
+        Exception: Raised if the query fails.
+
+    Returns:
+        dict: createAssetVersion Object
+    """
+    if not asset_id:
+        raise ValueError("Asset ID is required")
+    if not asset_version_name:
+        raise ValueError("Asset version name is required")
+
+    graphql_query = '''
+        mutation BapiCreateAssetVersion($assetVersionName: String!, $assetId: ID!, $createdByUserId: ID!) {
+            createNewAssetVersionOnAsset(assetVersionName: $assetVersionName, assetId: $assetId, createdByUserId: $createdByUserId) {
+                id
+                assetVersion {
+                    id
+                }
+            }
+        }
+    '''
+
+    # Asset name, business unit context, and creating user are required
+    variables = {"assetVersionName": asset_version_name, "assetId": asset_id}
+
+    if created_by_user_id:
+        variables["createdByUserId"] = created_by_user_id
+
+    response = send_graphql_query(token, organization_context, graphql_query, variables)
+    return response['data']
+
+
 def create_new_asset_version_artifact_and_test_for_upload(
     token,
     organization_context,
     business_unit_id=None,
     created_by_user_id=None,
     asset_id=None,
     version=None,
@@ -359,17 +417,17 @@
 
         if not business_unit_id:
             raise ValueError("Business Unit ID is required and could not be retrieved from the existing asset")
         if not created_by_user_id:
             raise ValueError("Created By User ID is required and could not be retrieved from the existing asset")
 
     # create the asset version
-    response = create_asset_version(token, organization_context, business_unit_id=business_unit_id,
-                                    created_by_user_id=created_by_user_id, asset_id=asset_id,
-                                    asset_version_name=version)
+    response = create_asset_version_on_asset(
+        token, organization_context, created_by_user_id=created_by_user_id, asset_id=asset_id, asset_version_name=version
+    )
     # get the asset version ID
     asset_version_id = response['createAssetVersion']['id']
 
     # create the test
     if test_type == "finite_state_binary_analysis":
         # create the artifact
         if not artifact_description:
@@ -642,16 +700,27 @@
         }
 
     response = send_graphql_query(token, organization_context, graphql_query, variables)
 
     return response['data']
 
 
-def create_test(token, organization_context, business_unit_id=None, created_by_user_id=None, asset_id=None,
-                artifact_id=None, test_name=None, product_id=None, test_type=None, tools=[], upload_method: UploadMethod = UploadMethod.API):
+def create_test(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_id=None,
+    artifact_id=None,
+    test_name=None,
+    product_id=None,
+    test_type=None,
+    tools=[],
+    upload_method: UploadMethod = UploadMethod.API,
+):
     """
     Create a new Test object for uploading files.
     This is an advanced method - you are probably looking for create_new_asset_version_and_upload_test_results or create_new_asset_version_and_upload_binary.
     Please see the examples in the Github repository for more information:
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/upload_test_results.py
     - https://github.com/FiniteStateInc/finite-state-sdk-python/blob/main/examples/uploading_a_binary.py
 
@@ -798,16 +867,25 @@
     ]
     return create_test(token, organization_context, business_unit_id=business_unit_id,
                        created_by_user_id=created_by_user_id, asset_id=asset_id, artifact_id=artifact_id,
                        test_name=test_name, product_id=product_id, test_type="finite_state_binary_analysis",
                        tools=tools, upload_method=upload_method)
 
 
-def create_test_as_cyclone_dx(token, organization_context, business_unit_id=None, created_by_user_id=None,
-                              asset_id=None, artifact_id=None, test_name=None, product_id=None, upload_method: UploadMethod = UploadMethod.API):
+def create_test_as_cyclone_dx(
+    token,
+    organization_context,
+    business_unit_id=None,
+    created_by_user_id=None,
+    asset_id=None,
+    artifact_id=None,
+    test_name=None,
+    product_id=None,
+    upload_method: UploadMethod = UploadMethod.API,
+):
     """
     Create a new Test object for uploading CycloneDX files.
 
     Args:
         token (str):
             Auth token. This is the token returned by get_auth_token(). Just the token, do not include "Bearer" in this string, that is handled inside the method.
         organization_context (str):
```

### Comparing `finite_state_sdk-0.1.6/finite_state_sdk/queries.py` & `finite_state_sdk-0.1.7/finite_state_sdk/queries.py`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.6/finite_state_sdk/token_cache.py` & `finite_state_sdk-0.1.7/finite_state_sdk/token_cache.py`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.6/pyproject.toml` & `finite_state_sdk-0.1.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "finite-state-sdk"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     "Finite State, Inc. <developer-tools@finitestate.io>"
 ]
 maintainers = [
     "Finite State, Inc. <developer-tools@finitestate.io>"
 ]
 repository = "https://www.github.com/FiniteStateInc/finite-state-sdk-python"
@@ -28,51 +28,50 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-bleach = "==6.0.0"
-build = "==0.10.0"
-certifi = "==2023.5.7"
-charset-normalizer = "==3.2.0"
-cyclonedx-bom = "==3.11.2"
+bleach = "^6.1.0"
+build = "^1.2.1"
+certifi = "^2024.2.2"
+charset-normalizer = "^3.2.0"
+cyclonedx-bom = "==3.11.7"
 cyclonedx-python-lib = "==3.1.5"
-docutils = "==0.20.1"
-idna = "==3.4"
-importlib-metadata = "==6.8.0"
-jaraco-classes = "==3.3.0"
-Jinja2 = "==3.1.2"
-keyring = "==24.2.0"
-markdown-it-py = "==3.0.0"
-MarkupSafe = "==2.1.3"
-mdurl = "==0.1.2"
-more-itertools = "==9.1.0"
-packageurl-python = "==0.11.1"
-packaging = "==23.1"
-pdoc = "==14.0.0"
-pip-requirements-parser = "==32.0.1"
-pkginfo = "==1.9.6"
-Pygments = "==2.15.1"
-pyparsing = "==3.1.0"
-pyproject_hooks = "==1.0.0"
-readme-renderer = "==40.0"
-requests = "==2.31.0"
-requests-toolbelt = "==1.0.0"
-rfc3986 = "==2.0.0"
-six = "==1.16.0"
-sortedcontainers = "==2.4.0"
-toml = "==0.10.2"
-tomli = "==2.0.1"
-twine = "==4.0.2"
-urllib3 = "==2.0.3"
-webencodings = "==0.5.1"
-zipp = "==3.16.2"
-
+docutils = "^0.21.1"
+idna = "^3.4"
+importlib-metadata = "^7.1.0"
+jaraco-classes = "^3.3.0"
+Jinja2 = "^3.1.2"
+keyring = "^25.1.0"
+markdown-it-py = "^3.0.0"
+MarkupSafe = "^2.1.3"
+mdurl = "^0.1.2"
+more-itertools = "^10.2.0"
+packageurl-python = "^0.15.0"
+packaging = "^24.0"
+pdoc = "^14.0.0"
+pip-requirements-parser = "^32.0.1"
+pkginfo = "^1.9.6"
+Pygments = "^2.15.1"
+pyparsing = "^3.1.0"
+pyproject_hooks = "^1.0.0"
+readme-renderer = "^43.0"
+requests = "^2.31.0"
+requests-toolbelt = "^1.0.0"
+rfc3986 = "^2.0.0"
+six = "^1.16.0"
+sortedcontainers = "^2.4.0"
+toml = "^0.10.2"
+tomli = "^2.0.1"
+twine = "^5.0.0"
+urllib3 = "^2.0.3"
+webencodings = "^0.5.1"
+zipp = "^3.16.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
 libcst = "^1.0.1"
 rich = "^13.5.2"
```

### Comparing `finite_state_sdk-0.1.6/PKG-INFO` & `finite_state_sdk-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finite-state-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: The official Finite State Python SDK.
 Home-page: https://github.com/FiniteStateInc/finite-state-sdk-python
 License: MIT
 Author: Finite State, Inc.
 Author-email: developer-tools@finitestate.io
 Maintainer: Finite State, Inc.
 Maintainer-email: developer-tools@finitestate.io
@@ -17,50 +17,50 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Jinja2 (==3.1.2)
-Requires-Dist: MarkupSafe (==2.1.3)
-Requires-Dist: Pygments (==2.15.1)
-Requires-Dist: bleach (==6.0.0)
-Requires-Dist: build (==0.10.0)
-Requires-Dist: certifi (==2023.5.7)
-Requires-Dist: charset-normalizer (==3.2.0)
-Requires-Dist: cyclonedx-bom (==3.11.2)
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: MarkupSafe (>=2.1.3,<3.0.0)
+Requires-Dist: Pygments (>=2.15.1,<3.0.0)
+Requires-Dist: bleach (>=6.1.0,<7.0.0)
+Requires-Dist: build (>=1.2.1,<2.0.0)
+Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
+Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
+Requires-Dist: cyclonedx-bom (==3.11.7)
 Requires-Dist: cyclonedx-python-lib (==3.1.5)
-Requires-Dist: docutils (==0.20.1)
-Requires-Dist: idna (==3.4)
-Requires-Dist: importlib-metadata (==6.8.0)
-Requires-Dist: jaraco-classes (==3.3.0)
-Requires-Dist: keyring (==24.2.0)
-Requires-Dist: markdown-it-py (==3.0.0)
-Requires-Dist: mdurl (==0.1.2)
-Requires-Dist: more-itertools (==9.1.0)
-Requires-Dist: packageurl-python (==0.11.1)
-Requires-Dist: packaging (==23.1)
-Requires-Dist: pdoc (==14.0.0)
-Requires-Dist: pip-requirements-parser (==32.0.1)
-Requires-Dist: pkginfo (==1.9.6)
-Requires-Dist: pyparsing (==3.1.0)
-Requires-Dist: pyproject_hooks (==1.0.0)
-Requires-Dist: readme-renderer (==40.0)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: requests-toolbelt (==1.0.0)
-Requires-Dist: rfc3986 (==2.0.0)
-Requires-Dist: six (==1.16.0)
-Requires-Dist: sortedcontainers (==2.4.0)
-Requires-Dist: toml (==0.10.2)
-Requires-Dist: tomli (==2.0.1)
-Requires-Dist: twine (==4.0.2)
-Requires-Dist: urllib3 (==2.0.3)
-Requires-Dist: webencodings (==0.5.1)
-Requires-Dist: zipp (==3.16.2)
+Requires-Dist: docutils (>=0.21.1,<0.22.0)
+Requires-Dist: idna (>=3.4,<4.0)
+Requires-Dist: importlib-metadata (>=7.1.0,<8.0.0)
+Requires-Dist: jaraco-classes (>=3.3.0,<4.0.0)
+Requires-Dist: keyring (>=25.1.0,<26.0.0)
+Requires-Dist: markdown-it-py (>=3.0.0,<4.0.0)
+Requires-Dist: mdurl (>=0.1.2,<0.2.0)
+Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
+Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: pdoc (>=14.0.0,<15.0.0)
+Requires-Dist: pip-requirements-parser (>=32.0.1,<33.0.0)
+Requires-Dist: pkginfo (>=1.9.6,<2.0.0)
+Requires-Dist: pyparsing (>=3.1.0,<4.0.0)
+Requires-Dist: pyproject_hooks (>=1.0.0,<2.0.0)
+Requires-Dist: readme-renderer (>=43.0,<44.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: rfc3986 (>=2.0.0,<3.0.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: twine (>=5.0.0,<6.0.0)
+Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
+Requires-Dist: webencodings (>=0.5.1,<0.6.0)
+Requires-Dist: zipp (>=3.16.2,<4.0.0)
 Project-URL: Repository, https://www.github.com/FiniteStateInc/finite-state-sdk-python
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://finitestate.io/hs-fs/hubfs/FS-Logo-Final-01.png" />
 </p>
```

