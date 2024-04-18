# Comparing `tmp/eodc-2024.3.2.tar.gz` & `tmp/eodc-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.3.2.tar", max compression
+gzip compressed data, was "eodc-2024.4.1.tar", max compression
```

## Comparing `eodc-2024.3.2.tar` & `eodc-2024.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      513 2024-04-04 12:19:34.419047 eodc-2024.3.2/README.md
--rw-r--r--   0        0        0      195 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    28345 2024-04-04 12:19:34.419047 eodc-2024.3.2/eodc/workspace.py
--rw-r--r--   0        0        0     1913 2024-04-04 12:19:34.423047 eodc-2024.3.2/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 eodc-2024.3.2/PKG-INFO
+-rw-r--r--   0        0        0      513 2024-04-18 16:19:16.024990 eodc-2024.4.1/README.md
+-rw-r--r--   0        0        0      195 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    28594 2024-04-18 16:19:16.024990 eodc-2024.4.1/eodc/workspace.py
+-rw-r--r--   0        0        0     1913 2024-04-18 16:19:16.028990 eodc-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 eodc-2024.4.1/PKG-INFO
```

### Comparing `eodc-2024.3.2/README.md` & `eodc-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/auth.py` & `eodc-2024.4.1/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/dask.py` & `eodc-2024.4.1/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/faas.py` & `eodc-2024.4.1/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/settings.py` & `eodc-2024.4.1/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/storage.py` & `eodc-2024.4.1/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.4.1/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.4.1/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.4.1/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.4.1/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.3.2/eodc/workspace.py` & `eodc-2024.4.1/eodc/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,50 +362,52 @@
         self.s3_client = boto3.client(
             "s3",
             aws_access_key_id=access_key.get_secret_value(),
             aws_secret_access_key=secret_key.get_secret_value(),
             endpoint_url=url,
         )
 
-        self.s3_session = boto3.Session(
-            aws_access_key_id=access_key.get_secret_value(),
-            aws_secret_access_key=secret_key.get_secret_value(),
-        )
+        handlers = self.s3_client.meta.events._emitter._handlers
 
-        self.iam_client = boto3.client(
-            "iam",
-            aws_access_key_id=access_key.get_secret_value(),
-            aws_secret_access_key=secret_key.get_secret_value(),
-            endpoint_url=url,
-            region_name="default",
+        handlers_to_unregister = handlers.prefix_search("before-parameter-build.s3")
+        handler_to_unregister = handlers_to_unregister[0]
+        self.s3_client.meta.events._emitter.unregister(
+            "before-parameter-build.s3", handler_to_unregister
         )
 
     def get_s3_credentials(self):
         return {
             "url": self.url,
             "access_key": self.access_key.get_secret_value(),
             "secret_key": self.secret_key.get_secret_value(),
         }
 
     def list_workspaces(self) -> list[str]:
         return [bucket["Name"] for bucket in self.s3_client.list_buckets()["Buckets"]]
 
     def create_user_workspace(
-        self, workspace_name: str, user_name: str, cwd: str
+        self, workspace_name: str, user_name: str = "", cwd: str = ""
     ) -> None:
         self.s3_client.create_bucket(Bucket=workspace_name)
 
+    def _workspace_acl_private(self, workspace_name: str):
+        self.s3_client.put_bucket_acl(ACL="private", Bucket=workspace_name)
+
     def delete_user_workspace(self, workspace_name: str):
         self.s3_client.delete_bucket(Bucket=workspace_name)
 
     def workspace_exists(self, workspace_name: str) -> bool:
         return workspace_name in self.list_workspaces()
 
+    def _override_validate_bucket_name(self, x, y):
+        return True
+
     def list_workspace_files(self, workspace_name: str):
-        return self.s3_client.list_objects(Bucket=workspace_name)["Contents"]
+        files = self.s3_client.list_objects(Bucket=workspace_name)
+        return files["Contents"]
 
     def upload_file(
         self, workspace_name: str, file_path: str, path_in_workspace: str = ""
     ):
         path_in_workspace = path_in_workspace.removesuffix("/")
         self.s3_client.put_object_acl()
         self.s3_client.upload_file(
@@ -446,14 +448,17 @@
 
     def download_file(self, workspace_name: str, file_name: str, path: str):
         self.s3_client.download_file(workspace_name, file_name, path)
 
     def download_stream(self, workspace_name: str, file_name: str):
         return self.s3_client.get_object(Bucket=workspace_name, Key=file_name)["Body"]
 
+    def get_workspace(self, workspace_name: str):
+        return self.s3_client.get_bucket(workspace_name)
+
     def get_fsspec(self, workspace_name: str):
         return fsspec.filesystem(
             "s3",
             anon=False,
             key=self.get_s3_credentials()["access_key"],
             secret=self.get_s3_credentials()["secret_key"],
             client_kwargs={
```

### Comparing `eodc-2024.3.2/pyproject.toml` & `eodc-2024.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.3.2"
+version = "2024.4.1"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.3.2/PKG-INFO` & `eodc-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

