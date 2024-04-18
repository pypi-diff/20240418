# Comparing `tmp/eidolon_ai_usage_client-0.1.0.tar.gz` & `tmp/eidolon_ai_usage_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_usage_client-0.1.0.tar", max compression
+gzip compressed data, was "eidolon_ai_usage_client-0.1.1.tar", max compression
```

## Comparing `eidolon_ai_usage_client-0.1.0.tar` & `eidolon_ai_usage_client-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-19 16:13:23.010729 eidolon_ai_usage_client-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 16:13:23.015427 eidolon_ai_usage_client-0.1.0/eidolon_ai_usage_client/__init__.py
--rw-r--r--   0        0        0     1672 2024-03-21 14:54:46.807950 eidolon_ai_usage_client-0.1.0/eidolon_ai_usage_client/client.py
--rw-r--r--   0        0        0      460 2024-03-19 16:13:23.017639 eidolon_ai_usage_client-0.1.0/eidolon_ai_usage_client/models.py
--rw-r--r--   0        0        0      420 2024-03-21 14:54:46.804193 eidolon_ai_usage_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-19 16:13:23.010729 eidolon_ai_usage_client-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 23:17:38.645326 eidolon_ai_usage_client-0.1.1/eidolon_ai_usage_client/__init__.py
+-rw-r--r--   0        0        0     1724 2024-04-17 21:35:51.486615 eidolon_ai_usage_client-0.1.1/eidolon_ai_usage_client/client.py
+-rw-r--r--   0        0        0      460 2024-03-21 23:17:38.647427 eidolon_ai_usage_client-0.1.1/eidolon_ai_usage_client/models.py
+-rw-r--r--   0        0        0      420 2024-04-18 04:24:57.302762 eidolon_ai_usage_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.1/PKG-INFO
```

### Comparing `eidolon_ai_usage_client-0.1.0/eidolon_ai_usage_client/client.py` & `eidolon_ai_usage_client-0.1.1/eidolon_ai_usage_client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import os
+
 from httpx import AsyncClient
 
 from eidolon_ai_usage_client.models import UsageSummary, UsageReset, UsageDelta
 
 
 class UsageClient:
     kwargs: dict
 
-    def __init__(self, location: str = "http://localhost:8527", **kwargs):
+    def __init__(self, location: str = os.environ.get('USAGE_SERVICE_LOC', "http://localhost:8527"), **kwargs):
         self.kwargs = dict(base_url=location, **kwargs)
 
     @property
     def client(self) -> AsyncClient:
         return AsyncClient(**self.kwargs)
 
     async def get_summary(self, subject: str) -> UsageSummary:
@@ -19,15 +21,15 @@
             response.raise_for_status()
             summary = UsageSummary(**response.json())
             if summary.used >= summary.allowed:
                 raise UsageLimitExceeded(summary)
             return summary
 
     async def record_transaction(
-        self, subject: str, transaction: UsageDelta | UsageReset
+            self, subject: str, transaction: UsageDelta | UsageReset
     ):
         transaction_dict = transaction.model_dump(exclude_defaults=True)
         transaction_dict["type"] = transaction.type
         async with self.client as client:
             response = await client.post(
                 f"/subjects/{subject}/transactions", json=transaction_dict
             )
```

