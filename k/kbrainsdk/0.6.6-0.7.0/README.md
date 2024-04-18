# Comparing `tmp/kbrainsdk-0.6.6.tar.gz` & `tmp/kbrainsdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbrainsdk-0.6.6.tar", max compression
+gzip compressed data, was "kbrainsdk-0.7.0.tar", max compression
```

## Comparing `kbrainsdk-0.6.6.tar` & `kbrainsdk-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     3092 2024-02-19 01:30:07.417447 kbrainsdk-0.6.6/README.md
--rw-r--r--   0        0        0        0 2023-11-25 18:26:16.692533 kbrainsdk-0.6.6/kbrainsdk/__init__.py
--rw-r--r--   0        0        0      368 2024-03-19 02:51:34.092206 kbrainsdk-0.6.6/kbrainsdk/admin.py
--rw-r--r--   0        0        0     1166 2024-02-19 01:30:07.417447 kbrainsdk-0.6.6/kbrainsdk/ai.py
--rw-r--r--   0        0        0     1528 2023-12-04 00:25:40.514991 kbrainsdk-0.6.6/kbrainsdk/api.py
--rw-r--r--   0        0        0       86 2023-11-26 20:37:51.991218 kbrainsdk-0.6.6/kbrainsdk/apibase.py
--rw-r--r--   0        0        0        0 2024-03-18 23:42:59.455373 kbrainsdk-0.6.6/kbrainsdk/azure_models/__init__.py
--rw-r--r--   0        0        0     1829 2024-02-19 01:30:07.417447 kbrainsdk-0.6.6/kbrainsdk/azure_models/model.py
--rw-r--r--   0        0        0     4123 2024-03-19 00:25:14.893078 kbrainsdk-0.6.6/kbrainsdk/datasets.py
--rw-r--r--   0        0        0     8317 2024-03-19 02:41:56.245761 kbrainsdk-0.6.6/kbrainsdk/ingest.py
--rw-r--r--   0        0        0     3763 2024-03-19 02:47:55.832257 kbrainsdk-0.6.6/kbrainsdk/llms.py
--rw-r--r--   0        0        0        0 2024-03-18 23:42:56.765374 kbrainsdk-0.6.6/kbrainsdk/security/__init__.py
--rw-r--r--   0        0        0     1496 2024-02-22 07:29:13.145949 kbrainsdk-0.6.6/kbrainsdk/security/azure_authentication.py
--rw-r--r--   0        0        0     1336 2024-02-22 07:29:13.145949 kbrainsdk-0.6.6/kbrainsdk/security/bearer.py
--rw-r--r--   0        0        0        0 2024-03-18 23:42:43.265379 kbrainsdk-0.6.6/kbrainsdk/validation/__init__.py
--rw-r--r--   0        0        0      748 2023-11-26 20:37:51.991218 kbrainsdk-0.6.6/kbrainsdk/validation/admin.py
--rw-r--r--   0        0        0     2083 2024-02-19 01:30:07.427447 kbrainsdk-0.6.6/kbrainsdk/validation/ai.py
--rw-r--r--   0        0        0      838 2023-11-26 20:37:51.991218 kbrainsdk-0.6.6/kbrainsdk/validation/common.py
--rw-r--r--   0        0        0     5285 2024-03-19 03:37:46.356322 kbrainsdk-0.6.6/kbrainsdk/validation/datasets.py
--rw-r--r--   0        0        0     2843 2024-03-01 00:52:30.956689 kbrainsdk-0.6.6/kbrainsdk/validation/ingest.py
--rw-r--r--   0        0        0     1881 2024-03-11 11:30:32.509968 kbrainsdk-0.6.6/kbrainsdk/validation/llms.py
--rw-r--r--   0        0        0      586 2024-03-19 03:39:40.927452 kbrainsdk-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 kbrainsdk-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     3092 2024-02-19 01:30:07.417447 kbrainsdk-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-11-25 18:26:16.692533 kbrainsdk-0.7.0/kbrainsdk/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-19 02:51:34.092206 kbrainsdk-0.7.0/kbrainsdk/admin.py
+-rw-r--r--   0        0        0     1166 2024-02-19 01:30:07.417447 kbrainsdk-0.7.0/kbrainsdk/ai.py
+-rw-r--r--   0        0        0     1528 2023-12-04 00:25:40.514991 kbrainsdk-0.7.0/kbrainsdk/api.py
+-rw-r--r--   0        0        0       86 2023-11-26 20:37:51.991218 kbrainsdk-0.7.0/kbrainsdk/apibase.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.0/kbrainsdk/azure_models/__init__.py
+-rw-r--r--   0        0        0     1829 2024-02-19 01:30:07.417447 kbrainsdk-0.7.0/kbrainsdk/azure_models/model.py
+-rw-r--r--   0        0        0     4123 2024-03-19 03:40:34.047444 kbrainsdk-0.7.0/kbrainsdk/datasets.py
+-rw-r--r--   0        0        0     8317 2024-03-19 03:40:47.897433 kbrainsdk-0.7.0/kbrainsdk/ingest.py
+-rw-r--r--   0        0        0     3763 2024-03-19 03:40:34.047444 kbrainsdk-0.7.0/kbrainsdk/llms.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.0/kbrainsdk/security/__init__.py
+-rw-r--r--   0        0        0     1496 2024-02-22 07:29:13.145949 kbrainsdk-0.7.0/kbrainsdk/security/azure_authentication.py
+-rw-r--r--   0        0        0     1336 2024-02-22 07:29:13.145949 kbrainsdk-0.7.0/kbrainsdk/security/bearer.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:34.464588 kbrainsdk-0.7.0/kbrainsdk/users.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:40:47.897433 kbrainsdk-0.7.0/kbrainsdk/validation/__init__.py
+-rw-r--r--   0        0        0      748 2023-11-26 20:37:51.991218 kbrainsdk-0.7.0/kbrainsdk/validation/admin.py
+-rw-r--r--   0        0        0     2083 2024-02-19 01:30:07.427447 kbrainsdk-0.7.0/kbrainsdk/validation/ai.py
+-rw-r--r--   0        0        0      838 2023-11-26 20:37:51.991218 kbrainsdk-0.7.0/kbrainsdk/validation/common.py
+-rw-r--r--   0        0        0     5285 2024-03-19 03:40:47.897433 kbrainsdk-0.7.0/kbrainsdk/validation/datasets.py
+-rw-r--r--   0        0        0     2843 2024-03-19 03:40:34.047444 kbrainsdk-0.7.0/kbrainsdk/validation/ingest.py
+-rw-r--r--   0        0        0     1881 2024-03-19 03:40:34.047444 kbrainsdk-0.7.0/kbrainsdk/validation/llms.py
+-rw-r--r--   0        0        0      681 2024-04-18 18:49:59.776803 kbrainsdk-0.7.0/kbrainsdk/validation/users.py
+-rw-r--r--   0        0        0      586 2024-04-18 18:54:13.087395 kbrainsdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 kbrainsdk-0.7.0/PKG-INFO
```

### Comparing `kbrainsdk-0.6.6/README.md` & `kbrainsdk-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/ai.py` & `kbrainsdk-0.7.0/kbrainsdk/ai.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/api.py` & `kbrainsdk-0.7.0/kbrainsdk/api.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/azure_models/model.py` & `kbrainsdk-0.7.0/kbrainsdk/azure_models/model.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/datasets.py` & `kbrainsdk-0.7.0/kbrainsdk/datasets.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/ingest.py` & `kbrainsdk-0.7.0/kbrainsdk/ingest.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/llms.py` & `kbrainsdk-0.7.0/kbrainsdk/llms.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/security/azure_authentication.py` & `kbrainsdk-0.7.0/kbrainsdk/security/azure_authentication.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/security/bearer.py` & `kbrainsdk-0.7.0/kbrainsdk/security/bearer.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/admin.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/admin.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/ai.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/ai.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/common.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/common.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/datasets.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/datasets.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/ingest.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/ingest.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/kbrainsdk/validation/llms.py` & `kbrainsdk-0.7.0/kbrainsdk/validation/llms.py`

 * *Files identical despite different names*

### Comparing `kbrainsdk-0.6.6/pyproject.toml` & `kbrainsdk-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbrainsdk"
-version = "0.6.6"
+version = "0.7.0"
 description = "SDK for using KBRaiN tools"
 authors = ["Daniel E Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "unlicensed"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kbrainsdk-0.6.6/PKG-INFO` & `kbrainsdk-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbrainsdk
-Version: 0.6.6
+Version: 0.7.0
 Summary: SDK for using KBRaiN tools
 License: unlicensed
 Author: Daniel E Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

