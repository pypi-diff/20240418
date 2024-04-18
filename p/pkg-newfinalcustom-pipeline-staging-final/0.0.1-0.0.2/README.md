# Comparing `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.1.tar.gz` & `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.1.tar", last modified: Tue Apr 16 21:54:58 2024, max compression
+gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.2.tar", last modified: Thu Apr 18 18:51:26 2024, max compression
```

## Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.1.tar` & `pkg_newfinalcustom_pipeline_staging_final-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:54:58.305520 pkg_newfinalcustom_pipeline_staging_final-0.0.1/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-16 21:54:58.305520 pkg_newfinalcustom_pipeline_staging_final-0.0.1/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/README.md
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:54:58.295520 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pipeline_staging_properties_pkg/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pipeline_staging_properties_pkg/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1036 2024-04-16 21:53:43.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pipeline_staging_properties_pkg/pipeline_staging_properties.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:54:58.305520 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-16 21:54:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-16 21:54:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-16 21:54:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-16 21:54:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-16 21:54:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-16 21:54:58.305520 pkg_newfinalcustom_pipeline_staging_final-0.0.1/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-16 21:52:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.1/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 18:51:26.643059 pkg_newfinalcustom_pipeline_staging_final-0.0.2/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-18 18:51:26.643059 pkg_newfinalcustom_pipeline_staging_final-0.0.2/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/README.md
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 18:51:26.633059 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pipeline_staging_properties_pkg/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pipeline_staging_properties_pkg/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1266 2024-04-18 18:50:44.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pipeline_staging_properties_pkg/pipeline_staging_properties.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 18:51:26.643059 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-18 18:51:26.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-18 18:51:26.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-18 18:51:26.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-18 18:51:26.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-18 18:51:26.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-18 18:51:26.643059 pkg_newfinalcustom_pipeline_staging_final-0.0.2/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-18 18:46:11.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.2/setup.py
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.1/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.1/pipeline_staging_properties_pkg/pipeline_staging_properties.py` & `pkg_newfinalcustom_pipeline_staging_final-0.0.2/pipeline_staging_properties_pkg/pipeline_staging_properties.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import boto3
+import os
 from botocore.exceptions import ClientError
 
+os.environ["AWS_ACCESS_KEY_ID"] = "x23203595AccessKeyIDPipelineStaging"
+os.environ["AWS_SECRET_ACCESS_KEY"] = "x23203595AccessKeyPipelineStaging"
+os.environ["AWS_SESSION_TOKEN"] = "x23203595SessionTokenPipelineStaging"
+
 class PipelineStagingManager:
     def __init__(self, bucket_name):
         self.bucket_name = bucket_name
         self.s3_client = boto3.client('s3')
 
     def list_stages(self):
         try:
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.1/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.2/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.1/setup.py` & `pkg_newfinalcustom_pipeline_staging_final-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pkg-newfinalcustom-pipeline-staging-final",
-    version="0.0.1",
+    version="0.0.2",
     author="Vinay Sriram Iyer",
     author_email="x23203595@student.ncirl.ie",
     description="A package where Custom Pipeline Stages can be managed at the behest of the user",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/x23203595/PipelineStagingSalesManagementSystem.git",
     packages=setuptools.find_packages(),
```

