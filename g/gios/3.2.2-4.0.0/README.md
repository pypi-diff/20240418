# Comparing `tmp/gios-3.2.2.tar.gz` & `tmp/gios-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gios-3.2.2.tar", last modified: Mon Nov 27 10:28:28 2023, max compression
+gzip compressed data, was "gios-4.0.0.tar", last modified: Thu Apr 18 20:57:55 2024, max compression
```

## Comparing `gios-3.2.2.tar` & `gios-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 10:28:28.284450 gios-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2023-11-27 10:28:16.000000 gios-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-27 10:28:16.000000 gios-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-11-27 10:28:28.280450 gios-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2023-11-27 10:28:16.000000 gios-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 10:28:28.280450 gios-3.2.2/gios/
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-11-27 10:28:16.000000 gios-3.2.2/gios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-27 10:28:16.000000 gios-3.2.2/gios/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-27 10:28:16.000000 gios-3.2.2/gios/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-27 10:28:16.000000 gios-3.2.2/gios/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 10:28:16.000000 gios-3.2.2/gios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 10:28:28.280450 gios-3.2.2/gios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-11-27 10:28:28.000000 gios-3.2.2/gios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-27 10:28:28.000000 gios-3.2.2/gios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 10:28:28.000000 gios-3.2.2/gios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-27 10:28:28.000000 gios-3.2.2/gios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-27 10:28:28.000000 gios-3.2.2/gios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-11-27 10:28:16.000000 gios-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-27 10:28:16.000000 gios-3.2.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-27 10:28:16.000000 gios-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 10:28:28.284450 gios-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-11-27 10:28:16.000000 gios-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 10:28:28.280450 gios-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2023-11-27 10:28:16.000000 gios-3.2.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:57:55.836135 gios-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-18 20:57:47.000000 gios-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 20:57:47.000000 gios-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-18 20:57:55.836135 gios-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 20:57:47.000000 gios-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:57:55.836135 gios-4.0.0/gios/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-18 20:57:47.000000 gios-4.0.0/gios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-18 20:57:47.000000 gios-4.0.0/gios/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-18 20:57:47.000000 gios-4.0.0/gios/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-18 20:57:47.000000 gios-4.0.0/gios/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:57:47.000000 gios-4.0.0/gios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:57:55.836135 gios-4.0.0/gios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-18 20:57:55.000000 gios-4.0.0/gios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-18 20:57:55.000000 gios-4.0.0/gios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:57:55.000000 gios-4.0.0/gios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 20:57:55.000000 gios-4.0.0/gios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 20:57:55.000000 gios-4.0.0/gios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-18 20:57:47.000000 gios-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-18 20:57:47.000000 gios-4.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 20:57:47.000000 gios-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:57:55.836135 gios-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-18 20:57:47.000000 gios-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:57:55.836135 gios-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-04-18 20:57:47.000000 gios-4.0.0/tests/test_init.py
```

### Comparing `gios-3.2.2/LICENSE` & `gios-4.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Maciej Bieniek
+   Copyright 2024 Maciej Bieniek
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gios-3.2.2/PKG-INFO` & `gios-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: gios
-Version: 3.2.2
+Version: 4.0.0
 Summary: Python wrapper for getting air quality data from GIOŚ servers.
 Home-page: https://github.com/bieniu/gios
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: dacite>=1.7.0
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
```

### Comparing `gios-3.2.2/README.md` & `gios-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gios-3.2.2/gios/__init__.py` & `gios-4.0.0/gios/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Python wrapper for getting air quality data from GIOS."""
+
 import logging
 from contextlib import suppress
 from http import HTTPStatus
 from typing import Any, Final
 
 from aiohttp import ClientSession
 from dacite import from_dict
```

### Comparing `gios-3.2.2/gios/const.py` & `gios-4.0.0/gios/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for GIOS library."""
+
 from typing import Final
 
 ATTR_AQI: Final[str] = "AQI"
 ATTR_ID: Final[str] = "id"
 ATTR_INDEX: Final[str] = "index"
 ATTR_INDEX_LEVEL: Final[str] = "{}IndexLevel"
 ATTR_NAME: Final[str] = "name"
```

### Comparing `gios-3.2.2/gios.egg-info/PKG-INFO` & `gios-4.0.0/gios.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: gios
-Version: 3.2.2
+Version: 4.0.0
 Summary: Python wrapper for getting air quality data from GIOŚ servers.
 Home-page: https://github.com/bieniu/gios
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: dacite>=1.7.0
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
```

### Comparing `gios-3.2.2/setup.py` & `gios-4.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Setup module for gios."""
+
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "3.2.2"
+VERSION = "4.0.0"
 
 setup(
     name="gios",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for getting air quality data from GIOŚ servers.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/gios",
     license="Apache-2.0 License",
     packages=["gios"],
     package_data={"gios": ["py.typed"]},
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=["aiohttp>=3.7.0", "dacite>=1.7.0"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Typing :: Typed",
     ],
 )
```

