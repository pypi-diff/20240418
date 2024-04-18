# Comparing `tmp/windmill_artifact-1.0.0.8-py3-none-any.whl.zip` & `tmp/windmill_artifact-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6847 bytes, number of entries: 9
--rw-r--r--  2.0 unx      235 b- defN 24-Mar-15 13:49 windmillartifactv1/__init__.py
--rw-r--r--  2.0 unx      235 b- defN 24-Mar-15 13:16 windmillartifactv1/client/__init__.py
--rw-r--r--  2.0 unx     3647 b- defN 24-Mar-15 13:16 windmillartifactv1/client/artifact_api_artifact.py
--rw-r--r--  2.0 unx    10411 b- defN 24-Mar-15 13:47 windmillartifactv1/client/artifact_client.py
--rw-r--r--  2.0 unx     1717 b- defN 24-Mar-15 13:16 windmillartifactv1/client/paging.py
--rw-r--r--  2.0 unx      629 b- defN 24-Mar-15 13:49 windmill_artifact-1.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-15 13:49 windmill_artifact-1.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Mar-15 13:49 windmill_artifact-1.0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      825 b- defN 24-Mar-15 13:49 windmill_artifact-1.0.0.8.dist-info/RECORD
-9 files, 17810 bytes uncompressed, 5397 bytes compressed:  69.7%
+Zip file size: 6936 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      235 b- defN 24-Mar-19 15:31 windmillartifactv1/__init__.py
+-rw-r--r--  2.0 unx      235 b- defN 24-Mar-19 15:31 windmillartifactv1/client/__init__.py
+-rw-r--r--  2.0 unx     3900 b- defN 24-Mar-19 15:31 windmillartifactv1/client/artifact_api_artifact.py
+-rw-r--r--  2.0 unx    10568 b- defN 24-Mar-19 15:31 windmillartifactv1/client/artifact_client.py
+-rw-r--r--  2.0 unx     1717 b- defN 24-Mar-19 15:31 windmillartifactv1/client/paging.py
+-rw-r--r--  2.0 unx      629 b- defN 24-Mar-19 15:31 windmill_artifact-1.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-19 15:31 windmill_artifact-1.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Mar-19 15:31 windmill_artifact-1.0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      825 b- defN 24-Mar-19 15:31 windmill_artifact-1.0.0.9.dist-info/RECORD
+9 files, 18220 bytes uncompressed, 5486 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: windmillartifactv1/client/artifact_client.py
 Comment: 
 
 Filename: windmillartifactv1/client/paging.py
 Comment: 
 
-Filename: windmill_artifact-1.0.0.8.dist-info/METADATA
+Filename: windmill_artifact-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: windmill_artifact-1.0.0.8.dist-info/WHEEL
+Filename: windmill_artifact-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: windmill_artifact-1.0.0.8.dist-info/top_level.txt
+Filename: windmill_artifact-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: windmill_artifact-1.0.0.8.dist-info/RECORD
+Filename: windmill_artifact-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## windmillartifactv1/client/artifact_api_artifact.py

```diff
@@ -21,14 +21,24 @@
     """
     LocationStyle
     """
     DEFAULT = "Default"
     TRITON = "Triton"
 
 
+def get_location_path(base_path: str, location_style: str, version: str):
+    """
+    get location path
+    """
+    if location_style == LocationStyle.TRITON.value:
+        return f"{base_path}/{version}"
+
+    return f"{base_path}/versions/{version}"
+
+
 class ArtifactContent:
     """
     artifact content class
     """
 
     def __init__(self, uri: Optional[str] = "",
                  description: Optional[str] = "",
```

## windmillartifactv1/client/artifact_client.py

```diff
@@ -109,31 +109,34 @@
                   "orderBy": page_request.orderby}
 
         return self._send_request(http_method=http_methods.GET,
                                   path=bytes("/v1/versions", encoding="utf-8"),
                                   params=params)
 
     def update_artifact(self, object_name: Optional[str] = "", version: Optional[str] = "", alias: Optional[list] = "",
-                        tags: Optional[dict] = None, description: Optional[str] = ""):
+                        tags: Optional[dict] = None, metadata: Optional[Any] = None,
+                        description: Optional[str] = ""):
         """
         Update details of an artifact.
 
         Args:
             object_name (str): 数据完整名称, example:"workspaces/ws1/modelstores/ms1/models/model1"
             version (str): 版本 example:"1"
             alias (Optional[List]):  版本别名，如default, latest.
             tags (Optional[Dict]): 版本标签 [key:value]
+            metadata (Optional[Any]): 版本基本信息
             description (str): 版本描述, example:"artifact description"
 
         Returns:
             dict: The response containing information about the updated artifact.
         """
         body = {"alias": alias,
                 "tags": tags,
                 "description": description,
+                "metadata": metadata,
                 "objectName": object_name,
                 "version": version}
         return self._send_request(http_method=http_methods.PUT,
                                   path=bytes("/v1/versions/" + version, encoding="utf-8"),
                                   params={"objectName": object_name},
                                   headers={b"Content-Type": http_content_types.JSON},
                                   body=json.dumps(body))
@@ -193,19 +196,19 @@
 
     @staticmethod
     def is_upload_required(uri, filesystem):
         """
         is_upload_required
         reference: artifact-go/command/artifact.go:CheckUri
         """
-        if uri.startswith(filesystem.kind):
+        if uri.startswith(filesystem["kind"]):
             return False
 
         # need enum filesystem.kind
-        if filesystem.kind == "file" and uri.startswith("s3"):
+        if filesystem["kind"] == "file" and uri.startswith("s3"):
             return False
 
         return True
 
     def create_location(self,
                         object_name: Optional[str] = "",
                         style: Optional[str] = LocationStyle.DEFAULT.value):
```

## Comparing `windmill_artifact-1.0.0.8.dist-info/METADATA` & `windmill_artifact-1.0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-artifact
-Version: 1.0.0.8
+Version: 1.0.0.9
 Summary: sdk in python for windmill artifact
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/artifact-go/tree/master/sdk/python
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `windmill_artifact-1.0.0.8.dist-info/RECORD` & `windmill_artifact-1.0.0.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 windmillartifactv1/__init__.py,sha256=lKPSTTL-s2LATDTCNAsIXlKPfw__8BreM8HrYsX9UHU,235
 windmillartifactv1/client/__init__.py,sha256=lKPSTTL-s2LATDTCNAsIXlKPfw__8BreM8HrYsX9UHU,235
-windmillartifactv1/client/artifact_api_artifact.py,sha256=ZSaQGPpZ5moWiH4i2dCndFiyA0dk_mvVxxMREHpcTVE,3647
-windmillartifactv1/client/artifact_client.py,sha256=CS9X1L8Mh75ndmtAUUqS4hZtG9rgqJt7e8P6HwFXgv8,10411
+windmillartifactv1/client/artifact_api_artifact.py,sha256=hQMjwHhT4Zn5vBwBa_6bZHcJZRUjbtTlhO00PVVcSnc,3900
+windmillartifactv1/client/artifact_client.py,sha256=o2zxAmgGgWKq0WufzjZNIQUzJYEE1-Jn8RMwpXrn1pA,10568
 windmillartifactv1/client/paging.py,sha256=Z9urwSGeNWgonqJyfTWyVdL77OI51aLm33TBnSV-OcU,1717
-windmill_artifact-1.0.0.8.dist-info/METADATA,sha256=LADbu-naAsDsxzSCXkawZxhhVx1XrmvUgY0MsQEA0wA,629
-windmill_artifact-1.0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-windmill_artifact-1.0.0.8.dist-info/top_level.txt,sha256=RBKeC1FcJSfcSsFKcqlKQi_Ajit-qQ96OO1TvJ5HAEg,19
-windmill_artifact-1.0.0.8.dist-info/RECORD,,
+windmill_artifact-1.0.0.9.dist-info/METADATA,sha256=JjbVAXhGuq1OXTYd2H42IWwY7JsywQV5-jzCXVll2oE,629
+windmill_artifact-1.0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+windmill_artifact-1.0.0.9.dist-info/top_level.txt,sha256=RBKeC1FcJSfcSsFKcqlKQi_Ajit-qQ96OO1TvJ5HAEg,19
+windmill_artifact-1.0.0.9.dist-info/RECORD,,
```

