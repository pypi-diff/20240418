# Comparing `tmp/compute_horde_facilitator_sdk-0.0.1a1.tar.gz` & `tmp/compute_horde_facilitator_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compute_horde_facilitator_sdk-0.0.1a1.tar", last modified: Wed Apr 10 08:41:47 2024, max compression
+gzip compressed data, was "compute_horde_facilitator_sdk-0.0.2.tar", last modified: Thu Apr 18 07:18:45 2024, max compression
```

## Comparing `compute_horde_facilitator_sdk-0.0.1a1.tar` & `compute_horde_facilitator_sdk-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0     1079 2024-04-10 08:41:40.333642 compute_horde_facilitator_sdk-0.0.1a1/LICENSE
--rw-r--r--   0        0        0       32 2024-04-10 08:41:40.333642 compute_horde_facilitator_sdk-0.0.1a1/README.md
--rw-r--r--   0        0        0      429 2024-04-10 08:41:47.129653 compute_horde_facilitator_sdk-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-10 08:41:40.333642 compute_horde_facilitator_sdk-0.0.1a1/src/compute_horde_facilitator_sdk/__init__.py
--rw-r--r--   0        0        0     3850 2024-04-10 08:41:40.333642 compute_horde_facilitator_sdk-0.0.1a1/src/compute_horde_facilitator_sdk/sdk.py
--rw-r--r--   0        0        0        0 2024-04-10 08:41:40.333642 compute_horde_facilitator_sdk-0.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 compute_horde_facilitator_sdk-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0       32 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0     1074 2024-04-18 07:18:45.300788 compute_horde_facilitator_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0     3418 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/sdk.py
+-rw-r--r--   0        0        0      139 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/v1.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     4137 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     3465 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/test_sdk.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/apiver/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-18 07:18:38.892714 compute_horde_facilitator_sdk-0.0.2/tests/v1/apiver/apiver_deps.py
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 compute_horde_facilitator_sdk-0.0.2/PKG-INFO
```

### Comparing `compute_horde_facilitator_sdk-0.0.1a1/LICENSE` & `compute_horde_facilitator_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `compute_horde_facilitator_sdk-0.0.1a1/src/compute_horde_facilitator_sdk/sdk.py` & `compute_horde_facilitator_sdk-0.0.2/src/compute_horde_facilitator_sdk/_internal/sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,12 @@
 from typing import Any
 
 import httpx
 
 
-def acquire_token(base_url: str, username: str, password: str) -> str:
-    with httpx.Client() as client:
-        response = client.post(f"{base_url}/api-token-auth/", data={"username": username, "password": password})
-    response.raise_for_status()
-    return response.json()["token"]
-
-
-async def async_acquire_token(base_url: str, username: str, password: str) -> str:
-    async with httpx.AsyncClient() as client:
-        response = await client.post(f"{base_url}/api-token-auth/", data={"username": username, "password": password})
-    response.raise_for_status()
-    return response.json()["token"]
-
-
 class FacilitatorClient:
     def __init__(self, base_url: str, token: str):
         self.base_url = base_url
         self.token = token
         self.client = httpx.Client(base_url=base_url, headers={"Authorization": f"Token {token}"})
 
     def __enter__(self):
@@ -42,15 +28,20 @@
     def create_raw_job(self, raw_script: str, input_url: str = "") -> dict[str, Any]:
         data = {"raw_script": raw_script, "input_url": input_url}
         response = self.client.post("/job-raw/", json=data)
         response.raise_for_status()
         return response.json()
 
     def create_docker_job(
-        self, docker_image: str, args: str = "", env: dict[str, str] = {}, use_gpu: bool = False, input_url: str = ""
+        self,
+        docker_image: str,
+        args: str = "",
+        env: dict[str, str] = {},
+        use_gpu: bool = False,
+        input_url: str = "",
     ) -> dict[str, Any]:
         data = {
             "docker_image": docker_image,
             "args": args,
             "env": env,
             "use_gpu": use_gpu,
             "input_url": input_url,
@@ -63,15 +54,17 @@
         self.client.close()
 
 
 class AsyncFacilitatorClient:
     def __init__(self, base_url: str, token: str):
         self.base_url = base_url
         self.token = token
-        self.client = httpx.AsyncClient(base_url=base_url, headers={"Authorization": f"Token {token}"})
+        self.client = httpx.AsyncClient(
+            base_url=base_url, headers={"Authorization": f"Token {token}"}
+        )
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
@@ -88,16 +81,27 @@
     async def create_raw_job(self, raw_script: str, input_url: str = "") -> dict[str, Any]:
         data = {"raw_script": raw_script, "input_url": input_url}
         response = await self.client.post("/job-raw/", json=data)
         response.raise_for_status()
         return response.json()
 
     async def create_docker_job(
-        self, docker_image: str, args: str = "", env: dict[str, str] = {}, use_gpu: bool = False, input_url: str = ""
+        self,
+        docker_image: str,
+        args: str = "",
+        env: dict[str, str] = {},
+        use_gpu: bool = False,
+        input_url: str = "",
     ) -> dict[str, Any]:
-        data = {"docker_image": docker_image, "args": args, "env": env, "use_gpu": use_gpu, "input_url": input_url}
+        data = {
+            "docker_image": docker_image,
+            "args": args,
+            "env": env,
+            "use_gpu": use_gpu,
+            "input_url": input_url,
+        }
         response = await self.client.post("/job-docker/", json=data)
         response.raise_for_status()
         return response.json()
 
     async def close(self):
         await self.client.aclose()
```

