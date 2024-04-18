# Comparing `tmp/rilaas-0.1.9.tar.gz` & `tmp/rilaas-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rilaas-0.1.9.tar", last modified: Mon Mar 25 09:30:14 2024, max compression
+gzip compressed data, was "rilaas-0.2.1.tar", last modified: Thu Apr 18 13:49:40 2024, max compression
```

## Comparing `rilaas-0.1.9.tar` & `rilaas-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 09:30:14.793810 rilaas-0.1.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-03-08 10:28:21.000000 rilaas-0.1.9/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1709 2024-03-25 09:30:14.793810 rilaas-0.1.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1364 2024-03-08 10:28:21.000000 rilaas-0.1.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 09:30:14.793810 rilaas-0.1.9/rilaas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14885 2024-03-25 09:28:10.000000 rilaas-0.1.9/rilaas/Client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-08 10:28:21.000000 rilaas-0.1.9/rilaas/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 09:30:14.793810 rilaas-0.1.9/rilaas.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1709 2024-03-25 09:30:14.000000 rilaas-0.1.9/rilaas.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      211 2024-03-25 09:30:14.000000 rilaas-0.1.9/rilaas.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-25 09:30:14.000000 rilaas-0.1.9/rilaas.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2024-03-25 09:30:14.000000 rilaas-0.1.9/rilaas.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-03-25 09:30:14.000000 rilaas-0.1.9/rilaas.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-25 09:30:14.793810 rilaas-0.1.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2024-03-25 09:29:53.000000 rilaas-0.1.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-03-08 10:28:21.000000 rilaas-0.2.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-18 13:49:40.102779 rilaas-0.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2024-04-18 13:49:03.000000 rilaas-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/rilaas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16524 2024-04-18 13:44:51.000000 rilaas-0.2.1/rilaas/Client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-08 10:28:21.000000 rilaas-0.2.1/rilaas/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-04-18 13:45:02.000000 rilaas-0.2.1/rilaas/get_file_type.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/rilaas.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2024-04-18 13:49:40.000000 rilaas-0.2.1/rilaas.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-18 13:49:40.102779 rilaas-0.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2024-04-18 13:47:01.000000 rilaas-0.2.1/setup.py
```

### Comparing `rilaas-0.1.9/LICENSE` & `rilaas-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rilaas-0.1.9/PKG-INFO` & `rilaas-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rilaas
-Version: 0.1.9
+Version: 0.2.1
 Summary: This is a package for getting a response from the EC2 server for the models deployed for ServeLine
 Home-page: https://github.com/ahfahad96/rilaas
 Author: Abdul Hafeez Fahad
 Author-email: ah.fahad@redbuffer.net
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 
 ## Usage
 
 ```python
 from rilaas.Client import Client
 
 # Example usage
-client = Client(url='<ip-address>:<port>', model_type='Models Deployed', endpoint='Function you want to execute', Optional_Params="Any other parameters you want to add according to the model")
+client = Client(id='id', api_key='API KEY', Optional_Params="Any other parameters you want to add according to the model")
 ```
 
 ## Configuration
 
 The package utilizes a `config.yaml` file for configuration. Below is an example:
 
 ```yaml
```

### Comparing `rilaas-0.1.9/README.md` & `rilaas-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Usage
 
 ```python
 from rilaas.Client import Client
 
 # Example usage
-client = Client(url='<ip-address>:<port>', model_type='Models Deployed', endpoint='Function you want to execute', Optional_Params="Any other parameters you want to add according to the model")
+client = Client(id='id', api_key='API KEY', Optional_Params="Any other parameters you want to add according to the model")
 ```
 
 ## Configuration
 
 The package utilizes a `config.yaml` file for configuration. Below is an example:
 
 ```yaml
```

### Comparing `rilaas-0.1.9/rilaas/Client.py` & `rilaas-0.2.1/rilaas/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+import sys
+import os
+
+current_dir = os.path.dirname(os.path.abspath(__file__))
+sys.path.append(current_dir)
+
 from requests_toolbelt.multipart.encoder import MultipartEncoder
+from get_file_type import get_mime_type
 import requests
 import json
-import os
 
 class Client:
     def __init__(self, api_key, **kwargs):
         self.ptr_id = kwargs.get('id', None)
         self.model_name = kwargs.get('name', None)
         self.api_key = api_key
         self.api_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/rilaas_client_get_metadata'
@@ -383,8 +389,51 @@
             response = requests.request(
                     method="POST",
                     url=url,
                     headers=headers,
                     data=multipart_encoder.to_string()
                 )
             return response
-        
+        
+class CustomModel_Client():
+    def __init__(self, ptr_id, api_key, selected_endpoint):
+        self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
+        self.ptr_id = ptr_id
+        self.api_key = api_key
+        self.selected_endpoint = selected_endpoint
+    
+    def predict(self, **kwargs):
+        url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
+        fields = {}
+    
+        if 'text' in kwargs:
+            fields['text'] = json.dumps(kwargs['text'])
+        
+        if 'json' in kwargs:
+            fields['json'] = kwargs['json']
+        
+        if 'dataframe' in kwargs:
+            fields['dataframe'] = kwargs['dataframe']
+        
+        if 'numpy' in kwargs:
+            fields['numpy'] = kwargs['numpy']
+        
+        if 'input_img' in kwargs:
+            fields['input_img'] = ('image.jpg', open(kwargs['input_img'], 'rb'), 'image/jpeg')
+        
+        if 'file' in kwargs:
+            fields['file'] = ('file.yml', open(kwargs['file'], 'rb'), get_mime_type('file.yml'))
+        
+        multipart_encoder = MultipartEncoder(fields=fields)
+        headers = {
+            'accept': 'image/jpeg',
+            'Content-Type': multipart_encoder.content_type,
+            'API_KEY': self.api_key
+        }
+        
+        response = requests.request(
+            method="POST",
+            url=url,
+            headers=headers,
+            data=multipart_encoder.to_string()
+        )
+        return response
```

### Comparing `rilaas-0.1.9/rilaas.egg-info/PKG-INFO` & `rilaas-0.2.1/rilaas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rilaas
-Version: 0.1.9
+Version: 0.2.1
 Summary: This is a package for getting a response from the EC2 server for the models deployed for ServeLine
 Home-page: https://github.com/ahfahad96/rilaas
 Author: Abdul Hafeez Fahad
 Author-email: ah.fahad@redbuffer.net
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,15 +25,15 @@
 
 ## Usage
 
 ```python
 from rilaas.Client import Client
 
 # Example usage
-client = Client(url='<ip-address>:<port>', model_type='Models Deployed', endpoint='Function you want to execute', Optional_Params="Any other parameters you want to add according to the model")
+client = Client(id='id', api_key='API KEY', Optional_Params="Any other parameters you want to add according to the model")
 ```
 
 ## Configuration
 
 The package utilizes a `config.yaml` file for configuration. Below is an example:
 
 ```yaml
```

### Comparing `rilaas-0.1.9/setup.py` & `rilaas-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rilaas',
-    version='0.1.9',
+    version='0.2.1',
     packages=find_packages(),
     # package_data={'config': ['*.yaml']},
     install_requires=[
         'requests',
         'pyyaml',
         'requests-toolbelt'
```

