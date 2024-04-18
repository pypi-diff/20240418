# Comparing `tmp/bagelML-0.0.12.tar.gz` & `tmp/bagelML-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagelML-0.0.12.tar", last modified: Tue Apr  2 18:35:11 2024, max compression
+gzip compressed data, was "bagelML-0.0.13.tar", last modified: Thu Apr 18 08:29:17 2024, max compression
```

## Comparing `bagelML-0.0.12.tar` & `bagelML-0.0.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.275547 bagelML-0.0.12/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-02 18:35:11.275245 bagelML-0.0.12/PKG-INFO
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5638 2024-04-02 18:31:43.000000 bagelML-0.0.12/README.md
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.271122 bagelML-0.0.12/bagel/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      376 2024-04-02 18:31:43.000000 bagelML-0.0.12/bagel/__init__.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.273113 bagelML-0.0.12/bagel/api/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    15205 2024-04-02 18:31:43.000000 bagelML-0.0.12/bagel/api/Cluster.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    12895 2024-04-02 18:31:43.000000 bagelML-0.0.12/bagel/api/__init__.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    19375 2024-04-02 18:31:43.000000 bagelML-0.0.12/bagel/api/fastapi.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    11570 2024-02-22 02:33:19.000000 bagelML-0.0.12/bagel/api/types.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5965 2024-02-22 02:33:19.000000 bagelML-0.0.12/bagel/config.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      683 2024-02-22 02:33:19.000000 bagelML-0.0.12/bagel/errors.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.273472 bagelML-0.0.12/bagel/utils/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.12/bagel/utils/__init__.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.274280 bagelML-0.0.12/bagelML.egg-info/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-02 18:35:11.000000 bagelML-0.0.12/bagelML.egg-info/PKG-INFO
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      383 2024-04-02 18:35:11.000000 bagelML-0.0.12/bagelML.egg-info/SOURCES.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        1 2024-04-02 18:35:11.000000 bagelML-0.0.12/bagelML.egg-info/dependency_links.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      267 2024-04-02 18:35:11.000000 bagelML-0.0.12/bagelML.egg-info/requires.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       11 2024-04-02 18:35:11.000000 bagelML-0.0.12/bagelML.egg-info/top_level.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       38 2024-04-02 18:35:11.275603 bagelML-0.0.12/setup.cfg
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     1217 2024-04-02 18:34:31.000000 bagelML-0.0.12/setup.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-02 18:35:11.274772 bagelML-0.0.12/test/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.12/test/__init__.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2717 2024-04-02 18:31:43.000000 bagelML-0.0.12/test/client_test.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2332 2024-02-22 02:33:19.000000 bagelML-0.0.12/test/opt_test.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.081661 bagelML-0.0.13/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-18 08:29:17.081434 bagelML-0.0.13/PKG-INFO
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5638 2024-04-02 18:31:43.000000 bagelML-0.0.13/README.md
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.078238 bagelML-0.0.13/bagel/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      376 2024-04-18 08:27:45.000000 bagelML-0.0.13/bagel/__init__.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.079555 bagelML-0.0.13/bagel/api/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    15205 2024-04-02 18:31:43.000000 bagelML-0.0.13/bagel/api/Cluster.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    13969 2024-04-18 08:27:54.000000 bagelML-0.0.13/bagel/api/__init__.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    22393 2024-04-18 08:27:54.000000 bagelML-0.0.13/bagel/api/fastapi.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    11570 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/api/types.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5965 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/config.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      683 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/errors.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.079881 bagelML-0.0.13/bagel/utils/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/utils/__init__.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.080533 bagelML-0.0.13/bagelML.egg-info/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/PKG-INFO
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      383 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/SOURCES.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        1 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/dependency_links.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      267 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/requires.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       11 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/top_level.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       38 2024-04-18 08:29:17.081712 bagelML-0.0.13/setup.cfg
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     1217 2024-04-18 08:27:54.000000 bagelML-0.0.13/setup.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.081042 bagelML-0.0.13/test/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.13/test/__init__.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2717 2024-04-02 18:31:43.000000 bagelML-0.0.13/test/client_test.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2332 2024-02-22 02:33:19.000000 bagelML-0.0.13/test/opt_test.py
```

### Comparing `bagelML-0.0.12/PKG-INFO` & `bagelML-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.12
+Version: 0.0.13
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.12/README.md` & `bagelML-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/bagel/api/Cluster.py` & `bagelML-0.0.13/bagel/api/Cluster.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/bagel/api/__init__.py` & `bagelML-0.0.13/bagel/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -410,7 +410,51 @@
             HTTPException: If there is an error in the HTTP request.
 
         """
         pass
 
     def share_cluster(self, cluster_id: str, usernames: List[str]):
         pass
+    
+    @abstractmethod
+    def create_dataset(
+            self,
+            dataset_id: UUID,
+            name: str,
+            description: str,
+            user_id: str = DEFAULT_TENANT,
+            api_key: Optional[str] = None
+    ) -> str:
+        """Create a dataset"""
+        pass
+    
+    @abstractmethod
+    def get_dataset_info(
+            self, 
+            dataset_id: str,
+            api_key: Optional[str] = None
+    ) -> str:
+        """Get information about a dataset."""
+        pass
+
+    @abstractmethod
+    def upload_dataset(
+            self,
+            dataset_id: str, 
+            chunk_number: int = 1,
+            file_name: str = "",
+            file_content: bytes = None,
+            api_key: Optional[str] = None
+    ) -> str:
+        """Upload a dataset file to Bagel."""
+        pass
+
+    @abstractmethod
+    def download_dataset(
+            self,
+            dataset_id: str,
+            file_path: Optional[str] = "",
+            api_key: Optional[str] = None
+    ) -> str:  
+        """Download the full dataset."""
+        pass
+
```

### Comparing `bagelML-0.0.12/bagel/api/fastapi.py` & `bagelML-0.0.13/bagel/api/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, cast, Any, List
+from typing import Optional, cast, Any, List, Tuple
 from bagel.api import API
 from bagel.config import System
 from bagel.api.types import (
     Document,
     Documents,
     Embeddings,
     IDs,
@@ -26,14 +26,16 @@
 from overrides import override
 import base64
 from io import BytesIO
 import os
 import uuid
 import time
 
+import tempfile, zipfile
+
 BAGEL_USER_ID = "BAGEL_USER_ID"
 BAGEL_API_KEY = "BAGEL_API_KEY"
 
 X_API_KEY = 'x-api-key'
 
 DEFAULT_TENANT = "default_tenant"
 DEFAULT_DATABASE = "default_database"
@@ -552,14 +554,109 @@
 
     def _extract_user_id_and_api_key(self, api_key, user_id):
         if os.environ.get(BAGEL_USER_ID) is not None and user_id == DEFAULT_TENANT:
             user_id = os.environ.get(BAGEL_USER_ID)
         if os.environ.get(BAGEL_API_KEY) is not None and api_key is None:
             api_key = os.environ.get(BAGEL_API_KEY)
         return api_key, user_id
+    
+    @override
+    def create_dataset(
+            self,
+            dataset_id: UUID,
+            name: str,
+            description: str,
+            user_id: str = DEFAULT_TENANT,
+            api_key: Optional[str] = None
+    ) -> str:
+        """Create a dataset"""
+        headers, user_id = self._extract_headers_with_key_and_user_id(api_key, user_id)
+        url = f"{self._api_url}/dataset-git"
+
+        data = {
+            "dataset_id": str(dataset_id),
+            "dataset_type": "Tabular",
+            "title": name,
+            "tags": [
+                "Dataset"
+            ],
+            "category": "AI",
+            "details": description,
+            "user_id": user_id
+        }
+        
+        resp = requests.post(url, headers=headers, data=json.dumps(data))
+        raise_bagel_error(resp)
+        
+        resp_text = resp.text
+        uuid_clean = resp_text.strip('"')
+
+        return uuid_clean
+
+    @override
+    def get_dataset_info(
+            self,
+            dataset_id: str,
+            path: Optional[str] = "",
+            api_key: Optional[str] = None
+    ) -> str:
+        """Get information about a dataset."""
+        headers = self._popuate_headers_with_api_key(api_key)
+        url = f"{self._api_url}/dataset-git"
+        
+        data = {'dataset_id': dataset_id, 'path': path}
+        
+        resp = requests.get(url, headers=headers, params=data)
+
+        resp_json = resp.json()
+        
+        return resp_json
+    
+    @override
+    def upload_dataset(
+            self,
+            dataset_id: str,
+            chunk_number: int = 1,
+            file_name: str = "",
+            file_content: bytes = None,
+            api_key: Optional[str] = None
+    ) -> str:
+        """Upload a dataset file to Bagel."""
+        headers = self._popuate_headers_with_api_key(api_key)
+        url = f"{self._api_url}/datasets/{dataset_id}/upload-dataset-git"
+
+        params = {'dataset_id': dataset_id, 'chunk_number': chunk_number, 'file_name': file_name}
+
+        files = {'data_file': (file_name, file_content)}
+        
+        resp = requests.post(url, headers=headers, files=files, params=params)
+        
+        return resp.text
+    
+    @override
+    def download_dataset(
+            self,
+            dataset_id: str,
+            file_path: Optional[str] = "",
+            api_key: Optional[str] = None
+    ) -> str:
+        """Download a specific file from dataset."""
+        headers = self._popuate_headers_with_api_key(api_key)
+        url = f"{self._api_url}/download-dataset-git"
+        
+        params = {'dataset_id': dataset_id, 'file_path': file_path}
+        
+        resp = requests.get(url, headers=headers, params=params)
+        # raise_bagel_error(resp)
+        
+        file_content = resp.content
+        file_name = resp.headers.get('Content-Disposition', '').split('filename=')[1].strip('"')
+        file_type = resp.headers.get('Content-Type', '')
+        
+        return file_content, file_name, file_type
 
 
 def raise_bagel_error(resp: requests.Response) -> None:
     """Raises an error if the response is not ok, using a BagelError if possible"""
     if resp.ok:
         return
```

### Comparing `bagelML-0.0.12/bagel/api/types.py` & `bagelML-0.0.13/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/bagel/config.py` & `bagelML-0.0.13/bagel/config.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/bagel/errors.py` & `bagelML-0.0.13/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/bagelML.egg-info/PKG-INFO` & `bagelML-0.0.13/bagelML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.12
+Version: 0.0.13
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.12/setup.py` & `bagelML-0.0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bagelML",
-    version="0.0.12",
+    version="0.0.13",
     description="BagelML is a Python library for interacting with the Bagel inference and vector embedding API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bagel.net",
     url="https://github.com/BagelNetwork/Client",
     packages=find_packages(),
```

### Comparing `bagelML-0.0.12/test/client_test.py` & `bagelML-0.0.13/test/client_test.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.12/test/opt_test.py` & `bagelML-0.0.13/test/opt_test.py`

 * *Files identical despite different names*

