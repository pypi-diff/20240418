# Comparing `tmp/hfutils-0.0.6.tar.gz` & `tmp/hfutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.0.6.tar", last modified: Tue Jan  9 09:21:48 2024, max compression
+gzip compressed data, was "hfutils-0.1.0.tar", last modified: Thu Apr 18 13:40:57 2024, max compression
```

## Comparing `hfutils-0.0.6.tar` & `hfutils-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.893394 hfutils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-09 09:21:24.000000 hfutils-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-09 09:21:24.000000 hfutils-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-01-09 09:21:48.893394 hfutils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-01-09 09:21:24.000000 hfutils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.885394 hfutils-0.0.6/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/entry/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/operate/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-09 09:21:24.000000 hfutils-0.0.6/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 09:21:48.889394 hfutils-0.0.6/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 09:21:48.000000 hfutils-0.0.6/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-09 09:21:24.000000 hfutils-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 09:21:48.893394 hfutils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-01-09 09:21:24.000000 hfutils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.140425 hfutils-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 13:40:35.000000 hfutils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 13:40:35.000000 hfutils-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-18 13:40:57.140425 hfutils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-18 13:40:35.000000 hfutils-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/entry/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.132424 hfutils-0.1.0/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.136424 hfutils-0.1.0/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-18 13:40:35.000000 hfutils-0.1.0/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:40:57.136424 hfutils-0.1.0/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 13:40:57.000000 hfutils-0.1.0/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 13:40:35.000000 hfutils-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:40:57.140425 hfutils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 13:40:35.000000 hfutils-0.1.0/setup.py
```

### Comparing `hfutils-0.0.6/LICENSE` & `hfutils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/PKG-INFO` & `hfutils-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.0.6
+Version: 0.1.0
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,24 +12,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.17
+Requires-Dist: huggingface_hub>=0.20
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
-Provides-Extra: 7z
-Requires-Dist: py7zr; extra == "7z"
+Provides-Extra: rar
+Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
@@ -59,20 +60,20 @@
 Requires-Dist: nbsphinx>=0.8.8; extra == "doc"
 Requires-Dist: ipython>=7.16.3; extra == "doc"
 Requires-Dist: psutil>=5.8.0; extra == "doc"
 Requires-Dist: ipykernel>=6.15; extra == "doc"
 Requires-Dist: py-cpuinfo>=8.0.0; extra == "doc"
 Requires-Dist: click>=7.0.0; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
-Provides-Extra: rar
-Requires-Dist: rarfile; extra == "rar"
-Provides-Extra: transfer
-Requires-Dist: hf-transfer; extra == "transfer"
 Provides-Extra: build
 Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
+Provides-Extra: 7z
+Requires-Dist: py7zr; extra == "7z"
+Provides-Extra: transfer
+Requires-Dist: hf-transfer; extra == "transfer"
 
 # hfutils
 
 [![PyPI](https://img.shields.io/pypi/v/hfutils)](https://pypi.org/project/hfutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/comments.json)
```

### Comparing `hfutils-0.0.6/README.md` & `hfutils-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/archive/__init__.py` & `hfutils-0.1.0/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/archive/base.py` & `hfutils-0.1.0/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/archive/sevenz.py` & `hfutils-0.1.0/hfutils/archive/zip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-import os
+import os.path
+import zipfile
 from typing import Optional
 
 from .base import register_archive_type
 from ..utils import tqdm, walk_files
 
 try:
-    import py7zr
-except ImportError:  # pragma: no cover
-    py7zr = None
+    import zlib
 
+    del zlib
+    _ZLIB_SUPPORTED = True
+except ImportError:
+    _ZLIB_SUPPORTED = False
 
-def _7z_pack(directory, sz_file, silent: bool = False, clear: bool = False):
-    with py7zr.SevenZipFile(sz_file, 'w') as zf:
+
+def _zip_pack(directory, zip_file, silent: bool = False, clear: bool = False):
+    with zipfile.ZipFile(zip_file, "w", compression=zipfile.ZIP_DEFLATED) as zf:
         progress = tqdm(walk_files(directory), silent=silent, desc=f'Packing {directory!r} ...')
         for file in progress:
             progress.set_description(file)
             zf.write(os.path.join(directory, file), file)
             if clear:
                 os.remove(os.path.join(directory, file))
 
 
-def _7z_unpack(sz_file, directory, silent: bool = False, password: Optional[str] = None):
+def _zip_unpack(zip_file, directory, silent: bool = False, password: Optional[str] = None):
     directory = os.fspath(directory)
     os.makedirs(directory, exist_ok=True)
-    with py7zr.SevenZipFile(sz_file, 'r', password=password) as zf:
-        progress = tqdm(zf.getnames(), silent=silent, desc=f'Unpacking {directory!r} ...')
-        for name in progress:
-            progress.set_description(name)
-            zf.extract(path=directory, targets=[name])
-            zf.reset()
+    with zipfile.ZipFile(zip_file, 'r') as zf:
+        if password is not None:
+            zf.setpassword(password.encode(encoding='utf-8'))
+        progress = tqdm(zf.namelist(), silent=silent, desc=f'Unpacking {directory!r} ...')
+        for zipinfo in progress:
+            progress.set_description(zipinfo)
+            zf.extract(zipinfo, directory)
 
 
-if py7zr is not None:
-    register_archive_type('7z', ['.7z'], _7z_pack, _7z_unpack)
+if _ZLIB_SUPPORTED:
+    register_archive_type('zip', ['.zip'], _zip_pack, _zip_unpack)
```

### Comparing `hfutils-0.0.6/hfutils/archive/tar.py` & `hfutils-0.1.0/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/archive/zip.py` & `hfutils-0.1.0/hfutils/archive/rar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-import os.path
-import zipfile
+import os
 from typing import Optional
 
 from .base import register_archive_type
-from ..utils import tqdm, walk_files
 
 try:
-    import zlib
+    import rarfile
+except ImportError:  # pragma: no cover
+    rarfile = None
 
-    del zlib
-    _ZLIB_SUPPORTED = True
-except ImportError:
-    _ZLIB_SUPPORTED = False
 
+def _rar_pack(directory, zip_file, silent: bool = False, clear: bool = False):
+    _ = directory, zip_file, silent, clear
+    raise RuntimeError('RAR format packing is not supported.')
 
-def _zip_pack(directory, zip_file, silent: bool = False, clear: bool = False):
-    with zipfile.ZipFile(zip_file, "w", compression=zipfile.ZIP_DEFLATED) as zf:
-        progress = tqdm(walk_files(directory), silent=silent, desc=f'Packing {directory!r} ...')
-        for file in progress:
-            progress.set_description(file)
-            zf.write(os.path.join(directory, file), file)
-            if clear:
-                os.remove(os.path.join(directory, file))
 
-
-def _zip_unpack(zip_file, directory, silent: bool = False, password: Optional[str] = None):
+def _rar_unpack(rar_file, directory, silent: bool = False, password: Optional[str] = None):
+    _ = silent
     directory = os.fspath(directory)
     os.makedirs(directory, exist_ok=True)
-    with zipfile.ZipFile(zip_file, 'r') as zf:
+    with rarfile.RarFile(rar_file, 'r') as zf:
         if password is not None:
-            zf.setpassword(password.encode(encoding='utf-8'))
-        progress = tqdm(zf.namelist(), silent=silent, desc=f'Unpacking {directory!r} ...')
-        for zipinfo in progress:
-            progress.set_description(zipinfo)
-            zf.extract(zipinfo, directory)
+            zf.setpassword(password)
+        zf.extractall(directory)
 
 
-if _ZLIB_SUPPORTED:
-    register_archive_type('zip', ['.zip'], _zip_pack, _zip_unpack)
+if rarfile is not None:
+    register_archive_type('rar', ['.rar'], _rar_pack, _rar_unpack)
```

### Comparing `hfutils-0.0.6/hfutils/entry/base.py` & `hfutils-0.1.0/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/entry/dispatch.py` & `hfutils-0.1.0/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/entry/download.py` & `hfutils-0.1.0/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/entry/upload.py` & `hfutils-0.1.0/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/operate/base.py` & `hfutils-0.1.0/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/operate/download.py` & `hfutils-0.1.0/hfutils/operate/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import logging
 import os.path
 import shutil
 from concurrent.futures import ThreadPoolExecutor
 from typing import List, Optional
 
 from .base import RepoTypeTyping, list_files_in_repository, _IGNORE_PATTERN_UNSET, get_hf_client
+from .validate import is_local_file_ready
 from ..archive import archive_unpack
 from ..utils import tqdm, TemporaryDirectory
 
 
 def download_file_to_file(local_file: str, repo_id: str, file_in_repo: str,
                           repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
                           resume_download: bool = True, hf_token: Optional[str] = None):
@@ -107,22 +109,33 @@
     :param hf_token: Huggingface token for API client, use ``HF_TOKEN`` variable if not assigned.
     :type hf_token: str, optional
     """
     files = list_files_in_repository(repo_id, repo_type, dir_in_repo, revision, ignore_patterns)
     progress = tqdm(files, silent=silent, desc=f'Downloading {dir_in_repo!r} ...')
 
     def _download_one_file(rel_file):
-        download_file_to_file(
-            local_file=os.path.join(local_directory, rel_file),
-            repo_id=repo_id,
-            file_in_repo=f'{dir_in_repo}/{rel_file}',
-            repo_type=repo_type,
-            revision=revision,
-            resume_download=resume_download,
-            hf_token=hf_token,
-        )
+        dst_file = os.path.join(local_directory, rel_file)
+        if os.path.exists(dst_file) and is_local_file_ready(
+                repo_id=repo_id,
+                repo_type=repo_type,
+                local_file=dst_file,
+                file_in_repo=f'{dir_in_repo}/{rel_file}',
+                revision=revision,
+                hf_token=hf_token,
+        ):
+            logging.info(f'Local file {rel_file} is ready, download skipped.')
+        else:
+            download_file_to_file(
+                local_file=dst_file,
+                repo_id=repo_id,
+                file_in_repo=f'{dir_in_repo}/{rel_file}',
+                repo_type=repo_type,
+                revision=revision,
+                resume_download=resume_download,
+                hf_token=hf_token,
+            )
         progress.update()
 
     tp = ThreadPoolExecutor(max_workers=max_workers)
     for file in files:
         tp.submit(_download_one_file, file)
     tp.shutdown(wait=True)
```

### Comparing `hfutils-0.0.6/hfutils/operate/upload.py` & `hfutils-0.1.0/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/utils/binary.py` & `hfutils-0.1.0/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/utils/download.py` & `hfutils-0.1.0/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/utils/temp.py` & `hfutils-0.1.0/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/utils/tqdm_.py` & `hfutils-0.1.0/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils/utils/walk.py` & `hfutils-0.1.0/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.0.6/hfutils.egg-info/PKG-INFO` & `hfutils-0.1.0/hfutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.0.6
+Version: 0.1.0
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,24 +12,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hbutils>=0.9.0
-Requires-Dist: huggingface_hub>=0.17
+Requires-Dist: huggingface_hub>=0.20
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: click>=7
-Provides-Extra: 7z
-Requires-Dist: py7zr; extra == "7z"
+Provides-Extra: rar
+Requires-Dist: rarfile; extra == "rar"
 Provides-Extra: test
 Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: mock>=4.0.3; extra == "test"
 Requires-Dist: flake8~=3.5; extra == "test"
 Requires-Dist: testfixtures>=6.18.5; extra == "test"
 Requires-Dist: pytest~=6.2.5; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
@@ -59,20 +60,20 @@
 Requires-Dist: nbsphinx>=0.8.8; extra == "doc"
 Requires-Dist: ipython>=7.16.3; extra == "doc"
 Requires-Dist: psutil>=5.8.0; extra == "doc"
 Requires-Dist: ipykernel>=6.15; extra == "doc"
 Requires-Dist: py-cpuinfo>=8.0.0; extra == "doc"
 Requires-Dist: click>=7.0.0; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
-Provides-Extra: rar
-Requires-Dist: rarfile; extra == "rar"
-Provides-Extra: transfer
-Requires-Dist: hf-transfer; extra == "transfer"
 Provides-Extra: build
 Requires-Dist: pyinstaller<5,>=4.7; extra == "build"
+Provides-Extra: 7z
+Requires-Dist: py7zr; extra == "7z"
+Provides-Extra: transfer
+Requires-Dist: hf-transfer; extra == "transfer"
 
 # hfutils
 
 [![PyPI](https://img.shields.io/pypi/v/hfutils)](https://pypi.org/project/hfutils/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hfutils)
 ![Loc](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/loc.json)
 ![Comments](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/narugo1992/b98a0fd1468c4858abf2a355bc9b4039/raw/comments.json)
```

### Comparing `hfutils-0.0.6/hfutils.egg-info/SOURCES.txt` & `hfutils-0.1.0/hfutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,13 +30,14 @@
 hfutils/entry/dispatch.py
 hfutils/entry/download.py
 hfutils/entry/upload.py
 hfutils/operate/__init__.py
 hfutils/operate/base.py
 hfutils/operate/download.py
 hfutils/operate/upload.py
+hfutils/operate/validate.py
 hfutils/utils/__init__.py
 hfutils/utils/binary.py
 hfutils/utils/download.py
 hfutils/utils/temp.py
 hfutils/utils/tqdm_.py
 hfutils/utils/walk.py
```

### Comparing `hfutils-0.0.6/hfutils.egg-info/requires.txt` & `hfutils-0.1.0/hfutils.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 hbutils>=0.9.0
-huggingface_hub>=0.17
+huggingface_hub>=0.20
 tqdm
 requests
 click>=7
 
 [7z]
 py7zr
```

### Comparing `hfutils-0.0.6/setup.py` & `hfutils-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     entry_points={
         'console_scripts': [
             'hfutils=hfutils.entry:hfutilscli'
         ]
     },
 )
```

