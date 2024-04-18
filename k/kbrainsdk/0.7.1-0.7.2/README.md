# Comparing `tmp/kbrainsdk-0.7.1.tar.gz` & `tmp/kbrainsdk-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsdk-0.7.1.tar", max compression
+gzip compressed data, was "kbrainsdk-0.7.2.tar", max compression
```

## Comparing `kbrainsdk-0.7.1.tar` & `kbrainsdk-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3092 2024-02-19 01:30:07.417447 kbrainsdk-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-11-25 18:26:16.692533 kbrainsdk-0.7.1/kbrainsdk/__init__.py
--rw-r--r--   0        0        0      368 2024-03-19 02:51:34.092206 kbrainsdk-0.7.1/kbrainsdk/admin.py
--rw-r--r--   0        0        0     1166 2024-02-19 01:30:07.417447 kbrainsdk-0.7.1/kbrainsdk/ai.py
--rw-r--r--   0        0        0     1528 2023-12-04 00:25:40.514991 kbrainsdk-0.7.1/kbrainsdk/api.py
--rw-r--r--   0        0        0       86 2023-11-26 20:37:51.991218 kbrainsdk-0.7.1/kbrainsdk/apibase.py
--rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.1/kbrainsdk/azure_models/__init__.py
--rw-r--r--   0        0        0     1829 2024-02-19 01:30:07.417447 kbrainsdk-0.7.1/kbrainsdk/azure_models/model.py
--rw-r--r--   0        0        0     4123 2024-03-19 03:40:34.047444 kbrainsdk-0.7.1/kbrainsdk/datasets.py
--rw-r--r--   0        0        0     8317 2024-03-19 03:40:47.897433 kbrainsdk-0.7.1/kbrainsdk/ingest.py
--rw-r--r--   0        0        0     3763 2024-03-19 03:40:34.047444 kbrainsdk-0.7.1/kbrainsdk/llms.py
--rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.1/kbrainsdk/security/__init__.py
--rw-r--r--   0        0        0     1496 2024-02-22 07:29:13.145949 kbrainsdk-0.7.1/kbrainsdk/security/azure_authentication.py
--rw-r--r--   0        0        0     1336 2024-02-22 07:29:13.145949 kbrainsdk-0.7.1/kbrainsdk/security/bearer.py
--rw-r--r--   0        0        0      662 2024-04-18 18:54:58.567378 kbrainsdk-0.7.1/kbrainsdk/users.py
--rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.1/kbrainsdk/validation/__init__.py
--rw-r--r--   0        0        0      748 2023-11-26 20:37:51.991218 kbrainsdk-0.7.1/kbrainsdk/validation/admin.py
--rw-r--r--   0        0        0     2083 2024-02-19 01:30:07.427447 kbrainsdk-0.7.1/kbrainsdk/validation/ai.py
--rw-r--r--   0        0        0      838 2023-11-26 20:37:51.991218 kbrainsdk-0.7.1/kbrainsdk/validation/common.py
--rw-r--r--   0        0        0     5285 2024-03-19 03:40:47.897433 kbrainsdk-0.7.1/kbrainsdk/validation/datasets.py
--rw-r--r--   0        0        0     2843 2024-03-19 03:40:34.047444 kbrainsdk-0.7.1/kbrainsdk/validation/ingest.py
--rw-r--r--   0        0        0     1881 2024-03-19 03:40:34.047444 kbrainsdk-0.7.1/kbrainsdk/validation/llms.py
--rw-r--r--   0        0        0      681 2024-04-18 18:49:59.776803 kbrainsdk-0.7.1/kbrainsdk/validation/users.py
--rw-r--r--   0        0        0      586 2024-04-18 19:05:28.947771 kbrainsdk-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 kbrainsdk-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3092 2024-02-19 01:30:07.417447 kbrainsdk-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-11-25 18:26:16.692533 kbrainsdk-0.7.2/kbrainsdk/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-19 02:51:34.092206 kbrainsdk-0.7.2/kbrainsdk/admin.py
+-rw-r--r--   0        0        0     1166 2024-02-19 01:30:07.417447 kbrainsdk-0.7.2/kbrainsdk/ai.py
+-rw-r--r--   0        0        0     1528 2023-12-04 00:25:40.514991 kbrainsdk-0.7.2/kbrainsdk/api.py
+-rw-r--r--   0        0        0       86 2023-11-26 20:37:51.991218 kbrainsdk-0.7.2/kbrainsdk/apibase.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.2/kbrainsdk/azure_models/__init__.py
+-rw-r--r--   0        0        0     1829 2024-02-19 01:30:07.417447 kbrainsdk-0.7.2/kbrainsdk/azure_models/model.py
+-rw-r--r--   0        0        0     4123 2024-03-19 03:40:34.047444 kbrainsdk-0.7.2/kbrainsdk/datasets.py
+-rw-r--r--   0        0        0     8317 2024-03-19 03:40:47.897433 kbrainsdk-0.7.2/kbrainsdk/ingest.py
+-rw-r--r--   0        0        0     3763 2024-03-19 03:40:34.047444 kbrainsdk-0.7.2/kbrainsdk/llms.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.2/kbrainsdk/security/__init__.py
+-rw-r--r--   0        0        0     1496 2024-02-22 07:29:13.145949 kbrainsdk-0.7.2/kbrainsdk/security/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2024-02-22 07:29:13.145949 kbrainsdk-0.7.2/kbrainsdk/security/bearer.py
+-rw-r--r--   0        0        0      662 2024-04-18 18:54:58.567378 kbrainsdk-0.7.2/kbrainsdk/users.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.2/kbrainsdk/validation/__init__.py
+-rw-r--r--   0        0        0      748 2023-11-26 20:37:51.991218 kbrainsdk-0.7.2/kbrainsdk/validation/admin.py
+-rw-r--r--   0        0        0     2083 2024-02-19 01:30:07.427447 kbrainsdk-0.7.2/kbrainsdk/validation/ai.py
+-rw-r--r--   0        0        0      838 2023-11-26 20:37:51.991218 kbrainsdk-0.7.2/kbrainsdk/validation/common.py
+-rw-r--r--   0        0        0     5285 2024-03-19 03:40:47.897433 kbrainsdk-0.7.2/kbrainsdk/validation/datasets.py
+-rw-r--r--   0        0        0     2843 2024-03-19 03:40:34.047444 kbrainsdk-0.7.2/kbrainsdk/validation/ingest.py
+-rw-r--r--   0        0        0     1881 2024-03-19 03:40:34.047444 kbrainsdk-0.7.2/kbrainsdk/validation/llms.py
+-rw-r--r--   0        0        0      691 2024-04-18 19:14:04.512858 kbrainsdk-0.7.2/kbrainsdk/validation/users.py
+-rw-r--r--   0        0        0      586 2024-04-18 19:14:19.330598 kbrainsdk-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 kbrainsdk-0.7.2/PKG-INFO
```

### Comparing `kbrainsdk-0.7.1/README.md` & `kbrainsdk-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/ai.py` & `kbrainsdk-0.7.2/kbrainsdk/ai.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/api.py` & `kbrainsdk-0.7.2/kbrainsdk/api.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/azure_models/model.py` & `kbrainsdk-0.7.2/kbrainsdk/azure_models/model.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/datasets.py` & `kbrainsdk-0.7.2/kbrainsdk/datasets.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/ingest.py` & `kbrainsdk-0.7.2/kbrainsdk/ingest.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/llms.py` & `kbrainsdk-0.7.2/kbrainsdk/llms.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/security/azure_authentication.py` & `kbrainsdk-0.7.2/kbrainsdk/security/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/security/bearer.py` & `kbrainsdk-0.7.2/kbrainsdk/security/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/users.py` & `kbrainsdk-0.7.2/kbrainsdk/users.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/admin.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/admin.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/ai.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/ai.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/common.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/common.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/datasets.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/datasets.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/ingest.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/ingest.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/llms.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/llms.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.7.1/kbrainsdk/validation/users.py` & `kbrainsdk-0.7.2/kbrainsdk/validation/users.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from validation.common import get_payload, validate_email
+from kbrainsdk.validation.common import get_payload, validate_email
 
 
 def validate_user_entra_groups(req):
     body = get_payload(req)
     email = body.get('email')
     token = body.get('token')
     client_id = body.get('client_id')
```

### Comparing `kbrainsdk-0.7.1/pyproject.toml` & `kbrainsdk-0.7.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsdk"
-version = "0.7.1"
+version = "0.7.2"
 description = "SDK for using KBRaiN tools"
 authors = ["Daniel E Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "unlicensed"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kbrainsdk-0.7.1/PKG-INFO` & `kbrainsdk-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsdk
-Version: 0.7.1
+Version: 0.7.2
 Summary: SDK for using KBRaiN tools
 License: unlicensed
 Author: Daniel E Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

