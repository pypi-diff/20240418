# Comparing `tmp/pyspapi-3.0.0a0.tar.gz` & `tmp/pyspapi-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspapi-3.0.0a0.tar", last modified: Mon Aug 15 20:31:23 2022, max compression
+gzip compressed data, was "pyspapi-3.1.0.tar", last modified: Thu Apr 18 16:53:00 2024, max compression
```

## Comparing `pyspapi-3.0.0a0.tar` & `pyspapi-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:31:23.060896 pyspapi-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-08-15 20:31:23.060896 pyspapi-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:31:23.056896 pyspapi-3.0.0a0/pyspapi/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/pyspapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8732 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/pyspapi/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/pyspapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/pyspapi/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/pyspapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 20:31:23.060896 pyspapi-3.0.0a0/pyspapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-08-15 20:31:23.000000 pyspapi-3.0.0a0/pyspapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-08-15 20:31:23.000000 pyspapi-3.0.0a0/pyspapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 20:31:23.000000 pyspapi-3.0.0a0/pyspapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-15 20:31:23.000000 pyspapi-3.0.0a0/pyspapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-15 20:31:23.000000 pyspapi-3.0.0a0/pyspapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-15 20:31:23.060896 pyspapi-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-08-15 20:31:15.000000 pyspapi-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:53:00.619758 pyspapi-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 16:52:49.000000 pyspapi-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 16:52:49.000000 pyspapi-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 16:53:00.619758 pyspapi-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 16:52:49.000000 pyspapi-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:53:00.619758 pyspapi-3.1.0/pyspapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 16:52:49.000000 pyspapi-3.1.0/pyspapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:52:49.000000 pyspapi-3.1.0/pyspapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-18 16:52:49.000000 pyspapi-3.1.0/pyspapi/spworlds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:53:00.619758 pyspapi-3.1.0/pyspapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 16:53:00.000000 pyspapi-3.1.0/pyspapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 16:53:00.000000 pyspapi-3.1.0/pyspapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:53:00.000000 pyspapi-3.1.0/pyspapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 16:53:00.000000 pyspapi-3.1.0/pyspapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 16:53:00.000000 pyspapi-3.1.0/pyspapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 16:52:49.000000 pyspapi-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:53:00.619758 pyspapi-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 16:52:49.000000 pyspapi-3.1.0/setup.py
```

### Comparing `pyspapi-3.0.0a0/LICENSE` & `pyspapi-3.1.0/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Aleksey
+Copyright (c) 2022 deesiigneer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyspapi-3.0.0a0/PKG-INFO` & `pyspapi-3.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyspapi
-Version: 3.0.0a0
+Version: 3.1.0
 Summary: API wrapper for SP servers written in Python
 Home-page: https://github.com/deesiigneer/pyspapi
 Author: deesiigneer
 License: MIT
-Project-URL: pyspapi documentation, https://pyspapi.readthedocs.io/
-Project-URL: api documentation, https://spworlds.readthedocs.io/
+Project-URL: Documentation, https://pyspapi.readthedocs.io/ru/latest/
 Project-URL: GitHub, https://github.com/deesiigneer/pyspapi
 Project-URL: Discord, https://discord.com/invite/VbyHaKRAaN
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -49,32 +48,39 @@
 
     pip install pyspapi
 
 *Linux/macOS*
 
 .. code:: sh
 
-    sudo apt pip3 install pyspapi
+    pip3 install pyspapi
 
 Quick example
 --------------
 
 Checking the balance
 ~~~~~~~~~~~~~~~~~~~~~
 .. code:: py
 
-  import pyspapi
+    from pyspapi import SPAPI
+    from asyncio import get_event_loop
 
-  print(await pyspapi.API(card_id='card_id', token='token').balance)
+    spapi = SPAPI(card_id='CARD_ID', token='TOKEN')
+
+
+    async def main():
+        print(await spapi.balance)
+
+    loop = get_event_loop()
+    loop.run_until_complete(main())
 
 More examples can be found in the `examples <https://github.com/deesiigneer/pyspapi/tree/main/examples>`_
 
 Links
 ------
 
 - `Discord server <https://discord.gg/VbyHaKRAaN>`_
 - `pyspapi documentation <https://pyspapi.readthedocs.io/>`_
-- `API documentation <https://spworlds.readthedocs.io>`_
 - `PyPi <https://pypi.org/project/pyspapi/>`_
 - `API documentation for SP sites <https://github.com/sp-worlds/api-docs>`_
```

### Comparing `pyspapi-3.0.0a0/README.rst` & `pyspapi-3.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -33,30 +33,37 @@
 
     pip install pyspapi
 
 *Linux/macOS*
 
 .. code:: sh
 
-    sudo apt pip3 install pyspapi
+    pip3 install pyspapi
 
 Quick example
 --------------
 
 Checking the balance
 ~~~~~~~~~~~~~~~~~~~~~
 .. code:: py
 
-  import pyspapi
+    from pyspapi import SPAPI
+    from asyncio import get_event_loop
 
-  print(await pyspapi.API(card_id='card_id', token='token').balance)
+    spapi = SPAPI(card_id='CARD_ID', token='TOKEN')
+
+
+    async def main():
+        print(await spapi.balance)
+
+    loop = get_event_loop()
+    loop.run_until_complete(main())
 
 More examples can be found in the `examples <https://github.com/deesiigneer/pyspapi/tree/main/examples>`_
 
 Links
 ------
 
 - `Discord server <https://discord.gg/VbyHaKRAaN>`_
 - `pyspapi documentation <https://pyspapi.readthedocs.io/>`_
-- `API documentation <https://spworlds.readthedocs.io>`_
 - `PyPi <https://pypi.org/project/pyspapi/>`_
 - `API documentation for SP sites <https://github.com/sp-worlds/api-docs>`_
```

### Comparing `pyspapi-3.0.0a0/pyspapi.egg-info/PKG-INFO` & `pyspapi-3.1.0/pyspapi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyspapi
-Version: 3.0.0a0
+Version: 3.1.0
 Summary: API wrapper for SP servers written in Python
 Home-page: https://github.com/deesiigneer/pyspapi
 Author: deesiigneer
 License: MIT
-Project-URL: pyspapi documentation, https://pyspapi.readthedocs.io/
-Project-URL: api documentation, https://spworlds.readthedocs.io/
+Project-URL: Documentation, https://pyspapi.readthedocs.io/ru/latest/
 Project-URL: GitHub, https://github.com/deesiigneer/pyspapi
 Project-URL: Discord, https://discord.com/invite/VbyHaKRAaN
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -49,32 +48,39 @@
 
     pip install pyspapi
 
 *Linux/macOS*
 
 .. code:: sh
 
-    sudo apt pip3 install pyspapi
+    pip3 install pyspapi
 
 Quick example
 --------------
 
 Checking the balance
 ~~~~~~~~~~~~~~~~~~~~~
 .. code:: py
 
-  import pyspapi
+    from pyspapi import SPAPI
+    from asyncio import get_event_loop
 
-  print(await pyspapi.API(card_id='card_id', token='token').balance)
+    spapi = SPAPI(card_id='CARD_ID', token='TOKEN')
+
+
+    async def main():
+        print(await spapi.balance)
+
+    loop = get_event_loop()
+    loop.run_until_complete(main())
 
 More examples can be found in the `examples <https://github.com/deesiigneer/pyspapi/tree/main/examples>`_
 
 Links
 ------
 
 - `Discord server <https://discord.gg/VbyHaKRAaN>`_
 - `pyspapi documentation <https://pyspapi.readthedocs.io/>`_
-- `API documentation <https://spworlds.readthedocs.io>`_
 - `PyPi <https://pypi.org/project/pyspapi/>`_
 - `API documentation for SP sites <https://github.com/sp-worlds/api-docs>`_
```

### Comparing `pyspapi-3.0.0a0/setup.py` & `pyspapi-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 setup(
     name='pyspapi',
     license='MIT',
     author='deesiigneer',
     version=version,
     url='https://github.com/deesiigneer/pyspapi',
     project_urls={
-        "pyspapi documentation": "https://pyspapi.readthedocs.io/",
-        "api documentation": "https://spworlds.readthedocs.io/",
+        "Documentation": "https://pyspapi.readthedocs.io/ru/latest/",
         "GitHub": "https://github.com/deesiigneer/pyspapi",
         "Discord": "https://discord.com/invite/VbyHaKRAaN"
     },
     description='API wrapper for SP servers written in Python',
     long_description=readme,
     long_description_content_type='text/x-rst',
     packages=packages,
```

