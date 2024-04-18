# Comparing `tmp/kbraincortex-0.7.0.tar.gz` & `tmp/kbraincortex-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbraincortex-0.7.0.tar", max compression
+gzip compressed data, was "kbraincortex-0.7.1.tar", max compression
```

## Comparing `kbraincortex-0.7.0.tar` & `kbraincortex-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3552 2024-03-19 03:40:47.887433 kbraincortex-0.7.0/kbraincortex/ai/reasoning.py
--rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.0/kbraincortex/api/__init__.py
--rw-r--r--   0        0        0      494 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/api/accounts.py
--rw-r--r--   0        0        0     3950 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/api/keys.py
--rw-r--r--   0        0        0     1498 2023-11-26 14:38:31.036676 kbraincortex-0.7.0/kbraincortex/api/telemetry.py
--rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.0/kbraincortex/azure/__init__.py
--rw-r--r--   0        0        0     2286 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/azure/cosmos.py
--rw-r--r--   0        0        0     1517 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/azure/datafactory.py
--rw-r--r--   0        0        0     1927 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/azure/search.py
--rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.0/kbraincortex/common/__init__.py
--rw-r--r--   0        0        0     1146 2024-03-19 03:40:34.037444 kbraincortex-0.7.0/kbraincortex/common/configuration.py
--rw-r--r--   0        0        0     1419 2023-12-04 00:25:40.504991 kbraincortex-0.7.0/kbraincortex/guidance/azure.py
--rw-r--r--   0        0        0     1037 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/ingest/onedrive.py
--rw-r--r--   0        0        0      968 2024-03-19 03:40:34.037444 kbraincortex-0.7.0/kbraincortex/ingest/rfp_responses.py
--rw-r--r--   0        0        0     1000 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/ingest/sharepoint.py
--rw-r--r--   0        0        0      732 2024-02-19 01:30:07.407447 kbraincortex-0.7.0/kbraincortex/ingest/status.py
--rw-r--r--   0        0        0      160 2023-12-04 00:25:40.514991 kbraincortex-0.7.0/kbraincortex/llms/encodings.py
--rw-r--r--   0        0        0     1296 2024-02-19 01:30:07.417447 kbraincortex-0.7.0/kbraincortex/llms/generation.py
--rw-r--r--   0        0        0     3385 2024-03-19 03:40:34.037444 kbraincortex-0.7.0/kbraincortex/llms/meta.py
--rw-r--r--   0        0        0     1391 2024-03-19 03:40:34.037444 kbraincortex-0.7.0/kbraincortex/llms/mistral.py
--rw-r--r--   0        0        0     7342 2024-03-19 03:40:34.037444 kbraincortex-0.7.0/kbraincortex/llms/models.py
--rw-r--r--   0        0        0     2758 2024-04-18 18:00:31.769043 kbraincortex-0.7.0/kbraincortex/microsoft/graph.py
--rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.0/kbraincortex/rag/__init__.py
--rw-r--r--   0        0        0    10252 2024-04-16 21:42:06.011956 kbraincortex-0.7.0/kbraincortex/rag/datasets.py
--rw-r--r--   0        0        0     1936 2024-03-19 03:40:47.887433 kbraincortex-0.7.0/kbraincortex/rag/retrieval.py
--rw-r--r--   0        0        0     4946 2024-02-19 01:30:07.417447 kbraincortex-0.7.0/kbraincortex/taxonomy/categories.py
--rw-r--r--   0        0        0     3058 2024-02-19 01:30:07.417447 kbraincortex-0.7.0/kbraincortex/taxonomy/tagging.py
--rw-r--r--   0        0        0      949 2024-04-18 18:56:10.187370 kbraincortex-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 kbraincortex-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3552 2024-03-19 03:40:47.887433 kbraincortex-0.7.1/kbraincortex/ai/reasoning.py
+-rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.1/kbraincortex/api/__init__.py
+-rw-r--r--   0        0        0      494 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/api/accounts.py
+-rw-r--r--   0        0        0     3950 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/api/keys.py
+-rw-r--r--   0        0        0     1498 2023-11-26 14:38:31.036676 kbraincortex-0.7.1/kbraincortex/api/telemetry.py
+-rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.1/kbraincortex/azure/__init__.py
+-rw-r--r--   0        0        0     2286 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/azure/cosmos.py
+-rw-r--r--   0        0        0     1517 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/azure/datafactory.py
+-rw-r--r--   0        0        0     1927 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/azure/search.py
+-rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.1/kbraincortex/common/__init__.py
+-rw-r--r--   0        0        0     1146 2024-03-19 03:40:34.037444 kbraincortex-0.7.1/kbraincortex/common/configuration.py
+-rw-r--r--   0        0        0     1419 2023-12-04 00:25:40.504991 kbraincortex-0.7.1/kbraincortex/guidance/azure.py
+-rw-r--r--   0        0        0     1037 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/ingest/onedrive.py
+-rw-r--r--   0        0        0      968 2024-03-19 03:40:34.037444 kbraincortex-0.7.1/kbraincortex/ingest/rfp_responses.py
+-rw-r--r--   0        0        0     1000 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/ingest/sharepoint.py
+-rw-r--r--   0        0        0      732 2024-02-19 01:30:07.407447 kbraincortex-0.7.1/kbraincortex/ingest/status.py
+-rw-r--r--   0        0        0      160 2023-12-04 00:25:40.514991 kbraincortex-0.7.1/kbraincortex/llms/encodings.py
+-rw-r--r--   0        0        0     1296 2024-02-19 01:30:07.417447 kbraincortex-0.7.1/kbraincortex/llms/generation.py
+-rw-r--r--   0        0        0     3385 2024-03-19 03:40:34.037444 kbraincortex-0.7.1/kbraincortex/llms/meta.py
+-rw-r--r--   0        0        0     1391 2024-03-19 03:40:34.037444 kbraincortex-0.7.1/kbraincortex/llms/mistral.py
+-rw-r--r--   0        0        0     7342 2024-03-19 03:40:34.037444 kbraincortex-0.7.1/kbraincortex/llms/models.py
+-rw-r--r--   0        0        0     2758 2024-04-18 18:00:31.769043 kbraincortex-0.7.1/kbraincortex/microsoft/graph.py
+-rw-r--r--   0        0        0        0 2023-11-26 14:38:31.036676 kbraincortex-0.7.1/kbraincortex/rag/__init__.py
+-rw-r--r--   0        0        0    10252 2024-04-16 21:42:06.011956 kbraincortex-0.7.1/kbraincortex/rag/datasets.py
+-rw-r--r--   0        0        0     1936 2024-03-19 03:40:47.887433 kbraincortex-0.7.1/kbraincortex/rag/retrieval.py
+-rw-r--r--   0        0        0     4946 2024-02-19 01:30:07.417447 kbraincortex-0.7.1/kbraincortex/taxonomy/categories.py
+-rw-r--r--   0        0        0     3058 2024-02-19 01:30:07.417447 kbraincortex-0.7.1/kbraincortex/taxonomy/tagging.py
+-rw-r--r--   0        0        0      949 2024-04-18 19:08:37.800960 kbraincortex-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 kbraincortex-0.7.1/PKG-INFO
```

### Comparing `kbraincortex-0.7.0/kbraincortex/ai/reasoning.py` & `kbraincortex-0.7.1/kbraincortex/ai/reasoning.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/api/keys.py` & `kbraincortex-0.7.1/kbraincortex/api/keys.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/api/telemetry.py` & `kbraincortex-0.7.1/kbraincortex/api/telemetry.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/azure/cosmos.py` & `kbraincortex-0.7.1/kbraincortex/azure/cosmos.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/azure/datafactory.py` & `kbraincortex-0.7.1/kbraincortex/azure/datafactory.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/azure/search.py` & `kbraincortex-0.7.1/kbraincortex/azure/search.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/common/configuration.py` & `kbraincortex-0.7.1/kbraincortex/common/configuration.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/guidance/azure.py` & `kbraincortex-0.7.1/kbraincortex/guidance/azure.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/ingest/onedrive.py` & `kbraincortex-0.7.1/kbraincortex/ingest/onedrive.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/ingest/rfp_responses.py` & `kbraincortex-0.7.1/kbraincortex/ingest/rfp_responses.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/ingest/sharepoint.py` & `kbraincortex-0.7.1/kbraincortex/ingest/sharepoint.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/ingest/status.py` & `kbraincortex-0.7.1/kbraincortex/ingest/status.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/llms/generation.py` & `kbraincortex-0.7.1/kbraincortex/llms/generation.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/llms/meta.py` & `kbraincortex-0.7.1/kbraincortex/llms/meta.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/llms/mistral.py` & `kbraincortex-0.7.1/kbraincortex/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/llms/models.py` & `kbraincortex-0.7.1/kbraincortex/llms/models.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/microsoft/graph.py` & `kbraincortex-0.7.1/kbraincortex/microsoft/graph.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/rag/datasets.py` & `kbraincortex-0.7.1/kbraincortex/rag/datasets.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/rag/retrieval.py` & `kbraincortex-0.7.1/kbraincortex/rag/retrieval.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/taxonomy/categories.py` & `kbraincortex-0.7.1/kbraincortex/taxonomy/categories.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/kbraincortex/taxonomy/tagging.py` & `kbraincortex-0.7.1/kbraincortex/taxonomy/tagging.py`

 * *Files identical despite different names*

### Comparing `kbraincortex-0.7.0/pyproject.toml` & `kbraincortex-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kbraincortex"
-version = "0.7.0"
+version = "0.7.1"
 description = "Common KBRaiN Functions"
 authors = ["Daniel Eric Fredriksen <daniel.fredriksen@us.kbr.com>"]
 license = "unlicensed"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 azure-core = "^1.29.5"
@@ -18,15 +18,15 @@
 azure-mgmt-datafactory = "^4.0.0"
 azure-identity = "^1.15.0"
 nest-asyncio = "^1.5.8"
 numpy = "^1.26.2"
 guidance = "^0.1.10"
 azure-search = "^1.0.0b2"
 azure-search-documents = "11.4.0b6"
-kbrainsdk = "0.7.0"
+kbrainsdk = "0.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `kbraincortex-0.7.0/PKG-INFO` & `kbraincortex-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbraincortex
-Version: 0.7.0
+Version: 0.7.1
 Summary: Common KBRaiN Functions
 License: unlicensed
 Author: Daniel Eric Fredriksen
 Author-email: daniel.fredriksen@us.kbr.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -16,13 +16,13 @@
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: azure-mgmt-datafactory (>=4.0.0,<5.0.0)
 Requires-Dist: azure-search (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-search-documents (==11.4.0b6)
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
 Requires-Dist: datetime (>=5.3,<6.0)
 Requires-Dist: guidance (>=0.1.10,<0.2.0)
-Requires-Dist: kbrainsdk (==0.7.0)
+Requires-Dist: kbrainsdk (==0.7.1)
 Requires-Dist: nest-asyncio (>=1.5.8,<2.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: openai (>=1.3.3,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

