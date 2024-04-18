# Comparing `tmp/pytesseract-api-1.0.1.tar.gz` & `tmp/pytesseract_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesseract-api-1.0.1.tar", last modified: Sun Oct 15 06:37:10 2023, max compression
+gzip compressed data, was "pytesseract_api-1.0.2.tar", last modified: Thu Apr 18 09:44:53 2024, max compression
```

## Comparing `pytesseract-api-1.0.1.tar` & `pytesseract_api-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 06:37:10.119467 pytesseract-api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-10-15 06:37:10.119467 pytesseract-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 06:37:10.119467 pytesseract-api-1.0.1/pytesseract_api/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pytesseract_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pytesseract_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pytesseract_api/capi_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pytesseract_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/pytesseract_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 06:37:10.119467 pytesseract-api-1.0.1/pytesseract_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-10-15 06:37:10.000000 pytesseract-api-1.0.1/pytesseract_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-10-15 06:37:10.000000 pytesseract-api-1.0.1/pytesseract_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 06:37:10.000000 pytesseract-api-1.0.1/pytesseract_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-15 06:37:10.000000 pytesseract-api-1.0.1/pytesseract_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 06:37:10.119467 pytesseract-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-10-15 06:37:00.000000 pytesseract-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:53.349659 pytesseract_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 09:44:53.349659 pytesseract_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:53.349659 pytesseract_api-1.0.2/pytesseract_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pytesseract_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pytesseract_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pytesseract_api/capi_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pytesseract_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/pytesseract_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:53.349659 pytesseract_api-1.0.2/pytesseract_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 09:44:53.000000 pytesseract_api-1.0.2/pytesseract_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 09:44:53.000000 pytesseract_api-1.0.2/pytesseract_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:44:53.000000 pytesseract_api-1.0.2/pytesseract_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:44:53.000000 pytesseract_api-1.0.2/pytesseract_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:44:53.349659 pytesseract_api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-18 09:44:49.000000 pytesseract_api-1.0.2/setup.py
```

### Comparing `pytesseract-api-1.0.1/LICENSE` & `pytesseract_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytesseract-api-1.0.1/PKG-INFO` & `pytesseract_api-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesseract-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tesseract C-API in python, a faster alternative to pytesseract
 Home-page: https://github.com/sandbox-pokhara/pytesseract-api
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/pytesseract-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytesseract-api-1.0.1/README.md` & `pytesseract_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytesseract-api-1.0.1/pytesseract_api/api.py` & `pytesseract_api-1.0.2/pytesseract_api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import atexit
 import os
 from ctypes import CDLL
 from ctypes import POINTER
+from ctypes import c_bool
 from ctypes import c_char_p
 from ctypes import c_int
 from ctypes import c_void_p
 from ctypes import cdll
 from functools import lru_cache
 from typing import Any
+from typing import Dict
 from typing import Optional
 
 from cv2.typing import MatLike
 
 from pytesseract_api.capi_types import TessBaseAPI
 from pytesseract_api.capi_types import TessPageSegMode
 from pytesseract_api.exceptions import TesseractError
@@ -52,14 +54,20 @@
         c_int,
         c_int,
         c_int,
         c_int,
     ]
     lib.TessBaseAPIGetUTF8Text.restype = c_char_p
     lib.TessBaseAPIGetUTF8Text.argtypes = [POINTER(TessBaseAPI)]
+    lib.TessBaseAPISetVariable.restype = c_bool
+    lib.TessBaseAPISetVariable.argtypes = [
+        POINTER(TessBaseAPI),
+        c_char_p,
+        c_char_p,
+    ]
     return lib
 
 
 @lru_cache()
 def get_tess_api(
     lib: CDLL,
     tessdata_path: Optional[str] = None,
@@ -87,19 +95,22 @@
 
 def image_to_string(
     img: MatLike,
     lib_path: Optional[str] = None,
     tessdata_path: Optional[str] = None,
     lang: str = "eng",
     psm: TessPageSegMode = TessPageSegMode.PSM_SINGLE_BLOCK,
+    variables: Dict[str, str] = {},
 ) -> str:
     # NOTE: ocr bugs on sliced image without this
     img = img.copy()
     data = get_image_data(img)
 
     lib = get_tess_lib(lib_path)
     api = get_tess_api(lib, tessdata_path=tessdata_path, lang=lang)
+    for k, v in variables.items():
+        lib.TessBaseAPISetVariable(api, k.encode(), v.encode())
     lib.TessBaseAPISetPageSegMode(api, psm.value)
     lib.TessBaseAPISetImage(api, *data)
     res: bytes = lib.TessBaseAPIGetUTF8Text(api)
     text = res.decode().strip()
     return text
```

### Comparing `pytesseract-api-1.0.1/pytesseract_api.egg-info/PKG-INFO` & `pytesseract_api-1.0.2/pytesseract_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesseract-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tesseract C-API in python, a faster alternative to pytesseract
 Home-page: https://github.com/sandbox-pokhara/pytesseract-api
 Author: Pradish Bijukchhe
 Author-email: pradishbijukchhe@gmail.com
 Project-URL: Bug Tracker, https://github.com/sandbox-pokhara/pytesseract-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytesseract-api-1.0.1/setup.py` & `pytesseract_api-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytesseract-api",
-    version="1.0.1",
+    version="1.0.2",
     author="Pradish Bijukchhe",
     author_email="pradishbijukchhe@gmail.com",
     description=(
         "Tesseract C-API in python, a faster alternative to pytesseract"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

