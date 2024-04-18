# Comparing `tmp/ng_data_pipelines_sdk-0.1.7.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.7.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.8.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.7.tar` & `ng_data_pipelines_sdk-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-17 16:06:17.632858 ng_data_pipelines_sdk-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-17 16:06:17.658858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-17 16:06:17.632858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-17 16:06:17.632858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24231 2024-04-17 16:06:17.633858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-17 16:06:17.633858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2969 2024-04-17 16:06:17.633858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-17 16:06:17.633858 ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      671 2024-04-17 16:06:17.634858 ng_data_pipelines_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 21:47:43.539633 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4766 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24231 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2878 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      671 2024-04-18 21:47:43.516634 ng_data_pipelines_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.8/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/aws_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-from typing import Dict
+from typing import Dict, Optional
 import boto3
 import json
 
 from ng_data_pipelines_sdk.interfaces import AWSCredentials, Env
 
 
 class AWSServiceClient:
-    def __init__(self, aws_credentials: AWSCredentials, region_name: str):
+    def __init__(
+        self, region_name: str, aws_credentials: Optional[AWSCredentials] = None
+    ):
+        aws_access_key_id = (
+            aws_credentials.aws_access_key_id if aws_credentials else None
+        )
+        aws_secret_access_key = (
+            aws_credentials.aws_secret_access_key if aws_credentials else None
+        )
+
         self.s3_client = boto3.client(
             "s3",
             region_name=region_name,
-            aws_access_key_id=aws_credentials.aws_access_key_id,
-            aws_secret_access_key=aws_credentials.aws_secret_access_key,
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
         )
         self.s3_resource = boto3.resource(
             "s3",
             region_name=region_name,
-            aws_access_key_id=aws_credentials.aws_access_key_id,
-            aws_secret_access_key=aws_credentials.aws_secret_access_key,
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
         )
         self.secrets_manager_client = boto3.client(
             "secretsmanager",
             region_name=region_name,
-            aws_access_key_id=aws_credentials.aws_access_key_id,
-            aws_secret_access_key=aws_credentials.aws_secret_access_key,
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
         )
 
 
 class AWSInterface:
     def __init__(
-        self, region_name: str, aws_credentials_dict: Dict[Env, AWSCredentials]
+        self,
+        region_name: str,
+        aws_credentials_dict: Optional[Dict[Env, Optional[AWSCredentials]]] = None,
     ):
+        if not aws_credentials_dict:
+            aws_credentials_dict = {Env.DEV: None, Env.PRD: None}
+
         self.client_managers = {
-            env: AWSServiceClient(credentials, region_name)
+            env: AWSServiceClient(region_name, credentials)
             for env, credentials in aws_credentials_dict.items()
         }
 
     def get_service_client(self, env: Env) -> AWSServiceClient:
         if env not in self.client_managers:
             raise ValueError(f"No AWS credentials found for environment {env.value}")
         return self.client_managers[env]
```

### Comparing `ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/spark_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 from ng_data_pipelines_sdk.interfaces import AWSCredentials, Env, FileType
 
 
 class SparkManager:
     def __init__(
         self,
         app_name: str,
-        aws_credentials_dict: Dict[Env, AWSCredentials],
+        aws_credentials_dict: Optional[Dict[Env, AWSCredentials]] = None,
     ):
         self.aws_credentials_dict = aws_credentials_dict
         spark_config = self.create_spark_config(app_name)
         self.spark = SparkSession.builder.config(conf=spark_config).getOrCreate()  # type: ignore
         self.spark.sparkContext.setLogLevel("ERROR")
 
     def _set_aws_credentials(self, env: Env):
         if not self.aws_credentials_dict:
-            raise ValueError(
-                "AWS credentials must be provided in order to access S3 resources"
-            )
+            return
 
         aws_credentials = self.aws_credentials_dict[env]
 
         jsc = getattr(self.spark.sparkContext, "_jsc")
         hadoopConfiguration = jsc.hadoopConfiguration()
 
         hadoopConfiguration.set("fs.s3a.access.key", aws_credentials.aws_access_key_id)
```

### Comparing `ng_data_pipelines_sdk-0.1.7/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.7/pyproject.toml` & `ng_data_pipelines_sdk-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.1.7"
+version = "0.1.8"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airlow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `ng_data_pipelines_sdk-0.1.7/PKG-INFO` & `ng_data_pipelines_sdk-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airlow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

