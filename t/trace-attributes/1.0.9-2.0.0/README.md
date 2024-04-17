# Comparing `tmp/trace-attributes-1.0.9.tar.gz` & `tmp/trace-attributes-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace-attributes-1.0.9.tar", last modified: Thu Feb 15 18:38:48 2024, max compression
+gzip compressed data, was "trace-attributes-2.0.0.tar", last modified: Wed Apr 17 22:21:04 2024, max compression
```

## Comparing `trace-attributes-1.0.9.tar` & `trace-attributes-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.225161 trace-attributes-1.0.9/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1068 2024-02-15 00:23:08.000000 trace-attributes-1.0.9/LICENSE
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 18:38:48.225045 trace-attributes-1.0.9/PKG-INFO
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     6591 2024-02-15 01:50:48.000000 trace-attributes-1.0.9/README.md
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       38 2024-02-15 18:38:48.225211 trace-attributes-1.0.9/setup.cfg
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      960 2024-02-15 18:38:36.000000 trace-attributes-1.0.9/setup.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.222703 trace-attributes-1.0.9/src/
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.222947 trace-attributes-1.0.9/src/python/
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.223592 trace-attributes-1.0.9/src/python/langtrace/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:26.000000 trace-attributes-1.0.9/src/python/langtrace/__init__.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.223921 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      293 2024-02-15 07:33:15.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.224294 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       13 2024-02-15 01:53:13.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      305 2024-02-14 23:14:51.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/langtrace_span_attributes.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)     1251 2024-02-15 07:27:58.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/openai_span_attributes.py
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      442 2024-02-15 00:23:08.000000 trace-attributes-1.0.9/src/python/langtrace/trace_attributes/module.py
-drwxr-xr-x   0 karthikkalyanaraman   (501) staff       (20)        0 2024-02-15 18:38:48.224881 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      494 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)      613 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)        1 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       21 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 karthikkalyanaraman   (501) staff       (20)       10 2024-02-15 18:38:48.000000 trace-attributes-1.0.9/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.533699 trace-attributes-2.0.0/
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)    11357 2024-04-04 15:20:34.000000 trace-attributes-2.0.0/LICENSE
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)      545 2024-04-17 22:21:04.533460 trace-attributes-2.0.0/PKG-INFO
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)     2825 2024-04-12 19:12:01.000000 trace-attributes-2.0.0/README.md
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)       38 2024-04-17 22:21:04.533737 trace-attributes-2.0.0/setup.cfg
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)      960 2024-04-17 22:20:44.000000 trace-attributes-2.0.0/setup.py
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.529916 trace-attributes-2.0.0/src/
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.530185 trace-attributes-2.0.0/src/python/
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.531228 trace-attributes-2.0.0/src/python/langtrace/
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)       13 2024-03-04 16:20:38.000000 trace-attributes-2.0.0/src/python/langtrace/__init__.py
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.531373 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)     1311 2024-04-04 15:20:34.000000 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.532110 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)       13 2024-03-04 16:20:38.000000 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)     1529 2024-04-12 19:12:01.000000 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)     1418 2024-04-12 19:12:01.000000 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)     3683 2024-04-17 20:36:57.000000 trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-17 22:21:04.533187 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)      545 2024-04-17 22:21:04.000000 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)      635 2024-04-17 22:21:04.000000 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)        1 2024-04-17 22:21:04.000000 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)       21 2024-04-17 22:21:04.000000 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 rohitkadhe   (501) staff       (20)       10 2024-04-17 22:21:04.000000 trace-attributes-2.0.0/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace-attributes-1.0.9/setup.py` & `trace-attributes-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='1.0.9',
+    version='2.0.0',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace-attributes-1.0.9/src/python/langtrace/trace_attributes/models/openai_span_attributes.py` & `trace-attributes-2.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # generated by datamodel-codegen:
-#   filename:  openai_span_attributes.json
-#   timestamp: 2024-02-15T07:27:58+00:00
+#   filename:  database_span_attributes.json
+#   timestamp: 2024-04-10T15:00:03+00:00
 
 from __future__ import annotations
 
 from typing import Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Extra, Field
 
 
-class OpenAISpanAttributes(BaseModel):
-    url_full: str = Field(..., alias='url.full')
-    llm_api: str = Field(..., alias='llm.api')
-    llm_model: str = Field(..., alias='llm.model')
-    llm_temperature: Optional[float] = Field(None, alias='llm.temperature')
-    llm_top_p: Optional[float] = Field(None, alias='llm.top_p')
-    llm_user: Optional[str] = Field(None, alias='llm.user')
-    llm_system_fingerprint: Optional[str] = Field(None, alias='llm.system.fingerprint')
-    http_max_retries: Optional[int] = Field(None, alias='http.max.retries')
-    http_timeout: Optional[int] = Field(None, alias='http.timeout')
-    llm_prompts: str = Field(..., alias='llm.prompts')
-    llm_responses: str = Field(..., alias='llm.responses')
-    llm_token_counts: Optional[str] = Field(None, alias='llm.token.counts')
-    llm_stream: Optional[bool] = Field(None, alias='llm.stream')
-    llm_encoding_format: Optional[str] = Field(None, alias='llm.encoding.format')
-    llm_dimensions: Optional[str] = Field(None, alias='llm.dimensions')
+class DatabaseSpanAttributes(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    langtrace_service_name: str = Field(..., alias='langtrace.service.name')
+    langtrace_service_type: str = Field(..., alias='langtrace.service.type')
+    langtrace_service_version: Optional[str] = Field(
+        None, alias='langtrace.service.version'
+    )
+    langtrace_sdk_name: str = Field(..., alias='langtrace.sdk.name')
+    langtrace_version: str = Field(..., alias='langtrace.version')
+    server_address: Optional[str] = Field(None, alias='server.address')
+    db_operation: Optional[str] = Field(None, alias='db.operation')
+    db_system: str = Field(..., alias='db.system')
+    db_namespace: Optional[str] = Field(None, alias='db.namespace')
+    db_index: Optional[str] = Field(None, alias='db.index')
+    db_collection_name: Optional[str] = Field(None, alias='db.collection.name')
+    db_pinecone_top_k: Optional[float] = Field(None, alias='db.pinecone.top_k')
+    db_chromadb_embedding_model: Optional[str] = Field(
+        None, alias='db.chromadb.embedding_model'
+    )
+    user_id: Optional[str] = Field(None, alias='user.id')
+    user_feedback_rating: Optional[int] = Field(None, alias='user.feedback.rating')
+    langtrace_testId: Optional[str] = Field(None, alias='langtrace.testId')
```

