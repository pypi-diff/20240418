# Comparing `tmp/sqlmodel_react_admin-0.0.4.tar.gz` & `tmp/sqlmodel_react_admin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_react_admin-0.0.4.tar", max compression
+gzip compressed data, was "sqlmodel_react_admin-0.0.5.tar", max compression
```

## Comparing `sqlmodel_react_admin-0.0.4.tar` & `sqlmodel_react_admin-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.4/LICENSE
--rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.4/README.md
--rw-r--r--   0        0        0      506 2024-04-17 08:51:03.875606 sqlmodel_react_admin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-17 08:16:39.104617 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/client.py
--rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/models.py
--rw-r--r--   0        0        0    17683 2024-04-17 09:03:01.788016 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/routers.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.5/LICENSE
+-rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.5/README.md
+-rw-r--r--   0        0        0      506 2024-04-17 15:18:20.251058 sqlmodel_react_admin-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-17 08:16:39.104617 sqlmodel_react_admin-0.0.5/sqlmodel_react_admin/client.py
+-rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.5/sqlmodel_react_admin/models.py
+-rw-r--r--   0        0        0    17688 2024-04-17 15:18:00.443680 sqlmodel_react_admin-0.0.5/sqlmodel_react_admin/routers.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.5/PKG-INFO
```

### Comparing `sqlmodel_react_admin-0.0.4/LICENSE` & `sqlmodel_react_admin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/routers.py` & `sqlmodel_react_admin-0.0.5/sqlmodel_react_admin/routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,15 @@
         self,
         id: UUID,
         request: Request,
         client: httpx.AsyncClient = Depends(get_async_client),
     ) -> Any:
 
         try:
-            URL = f"{self.base_url}/{self.name_plural}/{id}"
+            URL = f"{self.base_url}/{self.machine_name}/{id}"
             req = client.build_request(
                 "PUT",
                 URL,
                 headers=request.headers.raw,
                 content=request.stream(),
             )
             r = await client.send(req, stream=True)
@@ -422,15 +422,15 @@
     async def delete(
         self,
         id: UUID,
         request: Request,
         client: httpx.AsyncClient = Depends(get_async_client),
     ) -> None:
         try:
-            URL = f"{self.base_url}/{self.name_plural}/{id}"
+            URL = f"{self.base_url}/{self.machine_name}/{id}"
             req = client.build_request(
                 "DELETE",
                 URL,
                 headers=request.headers.raw,
                 content=request.stream(),
             )
             r = await client.send(req, stream=True)
@@ -450,15 +450,15 @@
     async def create(
         self,
         request: Request,
         client: httpx.AsyncClient = Depends(get_async_client),
     ) -> Any:
 
         try:
-            URL = f"{self.base_url}/{self.name_plural}"
+            URL = f"{self.base_url}/{self.machine_name}"
             req = client.build_request(
                 "POST",
                 URL,
                 headers=request.headers.raw,
                 content=request.stream(),
             )
             r = await client.send(req, stream=True)
@@ -479,15 +479,15 @@
         self,
         id: UUID,
         request: Request,
         client: httpx.AsyncClient = Depends(get_async_client),
     ) -> Any:
 
         try:
-            URL = f"{self.base_url}/{self.name_plural}/{id}"
+            URL = f"{self.base_url}/{self.machine_name}/{id}"
             req = client.build_request(
                 "GET",
                 URL,
                 headers=request.headers.raw,
                 content=request.stream(),
             )
             r = await client.send(req, stream=True)
@@ -507,15 +507,15 @@
     async def get_many(
         self,
         request: Request,
         client: httpx.AsyncClient = Depends(get_async_client),
     ) -> Any:
 
         try:
-            URL = f"{self.base_url}/{self.name_plural}"
+            URL = f"{self.base_url}/{self.machine_name}"
             req = client.build_request(
                 "GET",
                 URL,
                 headers=request.headers.raw,
                 content=request.stream(),
             )
             r = await client.send(req, stream=True)
```

### Comparing `sqlmodel_react_admin-0.0.4/PKG-INFO` & `sqlmodel_react_admin-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-react-admin
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create fast SQLModel/FastAPI APIs/BFFs for React Admin
 License: MIT
 Author: Evan Thomas
 Author-email: evan@evanjt.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

