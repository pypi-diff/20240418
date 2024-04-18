# Comparing `tmp/pyfunvice-0.1.4.tar.gz` & `tmp/pyfunvice-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunvice-0.1.4.tar", max compression
+gzip compressed data, was "pyfunvice-0.1.5.tar", max compression
```

## Comparing `pyfunvice-0.1.4.tar` & `pyfunvice-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.4/README.md
--rw-r--r--   0        0        0     5570 2024-04-02 01:41:13.443528 pyfunvice-0.1.4/pyfunvice/__init__.py
--rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.4/pyfunvice/cli.py
--rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.4/pyfunvice/common_func.py
--rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.4/pyfunvice/docker_cli.py
--rw-r--r--   0        0        0      577 2024-03-26 09:15:00.081774 pyfunvice-0.1.4/pyfunvice/struct.py
--rw-r--r--   0        0        0      454 2024-04-07 07:09:38.597243 pyfunvice-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.5/README.md
+-rw-r--r--   0        0        0     5628 2024-04-12 09:27:28.208125 pyfunvice-0.1.5/pyfunvice/__init__.py
+-rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.5/pyfunvice/cli.py
+-rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.5/pyfunvice/common_func.py
+-rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.5/pyfunvice/docker_cli.py
+-rw-r--r--   0        0        0      577 2024-03-26 09:15:00.081774 pyfunvice-0.1.5/pyfunvice/struct.py
+-rw-r--r--   0        0        0      454 2024-04-18 02:22:16.165161 pyfunvice-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.5/PKG-INFO
```

### Comparing `pyfunvice-0.1.4/README.md` & `pyfunvice-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.4/pyfunvice/__init__.py` & `pyfunvice-0.1.5/pyfunvice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from fastapi.params import Form
 from gunicorn.app.base import BaseApplication
+from gunicorn.arbiter import Arbiter
+from gunicorn.workers.base import Worker
 from fastapi import APIRouter, FastAPI, File, Request, UploadFile
+from fastapi.params import Form
 from functools import wraps
 import inspect
-import subprocess
 import aiofiles
 
 from pyfunvice.common_func import delete_file, get_uuid
 from pyfunvice.struct import ResponseModel
 
 app = FastAPI()
 faas_router = APIRouter()
 
 
-def faas(path="/", body_type="raw", inparam_type="dict"):
+def app_service(path="/", body_type="raw", inparam_type="dict"):
     """
     path : str = "/",                       # http path
     body_type : str = "raw", "form-data"    # http body type
     inparam_type : str = "dict", "flat"     # faas inparam type
     """
 
     def decorator(func):
@@ -43,15 +44,14 @@
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
 
-                return func
             elif inparam_type == "flat":
 
                 @wraps(func)
                 async def wrapper(*args, **kwargs):
                     return await func(*args, **kwargs)
 
                 signature = inspect.signature(func)
@@ -74,14 +74,15 @@
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
             else:
                 pass
+            return func
         elif body_type == "form-data":
 
             @wraps(func)
             async def wrapper(file_name: str, file: UploadFile = File(...)):
                 async with aiofiles.open(file_name, "wb") as out_file:
                     content = await file.read()
                     await out_file.write(content)
@@ -136,29 +137,31 @@
         for key, value in config.items():
             self.cfg.set(key.lower(), value)
 
     def load(self):
         return self.application
 
 
-def start_faas(port: int = 8000, workers: int = 1):
+def start_app(port: int = 8000, workers: int = 1, post_fork_func: callable = None):
     app.include_router(faas_router)
+
+    def post_fork(server: Arbiter, worker: Worker):
+        if post_fork_func is not None:
+            post_fork_func()
+        else:
+            pass
+
     options = {
         "bind": f"0.0.0.0:{port}",
         "timeout": 7200,
         "workers": workers,
         "worker_class": "uvicorn.workers.UvicornWorker",
+        "post_fork": post_fork,
     }
     StandaloneApplication(app, options).run()
 
 
-def start_fass_with_cmd(port: int = 8000, workers: int = 1):
-    gunicorn_cmd = (
-        f"poetry run gunicorn "
-        "pyfunvice:app "
-        f"--timeout 7200 "
-        f"--workers {workers} "
-        "--worker-class uvicorn.workers.UvicornWorker "
-        f"--bind 0.0.0.0:{port}"
-    )
-    result = subprocess.run(gunicorn_cmd, shell=True, check=True, text=True)
-    print(result)
+def get_app_instance(post_fork_func: callable = None):
+    if post_fork_func is not None:
+        post_fork_func()
+    app.include_router(faas_router)
+    return app
```

### Comparing `pyfunvice-0.1.4/pyfunvice/cli.py` & `pyfunvice-0.1.5/pyfunvice/cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.4/pyfunvice/docker_cli.py` & `pyfunvice-0.1.5/pyfunvice/docker_cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.4/pyfunvice/struct.py` & `pyfunvice-0.1.5/pyfunvice/struct.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.4/PKG-INFO` & `pyfunvice-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfunvice
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: 遥奕
 Author-email: jibing.yjb@alibaba-inc.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

