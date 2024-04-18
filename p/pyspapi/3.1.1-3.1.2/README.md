# Comparing `tmp/pyspapi-3.1.1.tar.gz` & `tmp/pyspapi-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspapi-3.1.1.tar", last modified: Thu Apr 18 17:40:06 2024, max compression
+gzip compressed data, was "pyspapi-3.1.2.tar", last modified: Thu Apr 18 18:12:59 2024, max compression
```

## Comparing `pyspapi-3.1.1.tar` & `pyspapi-3.1.2.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:06.042276 pyspapi-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 17:39:56.000000 pyspapi-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 17:39:56.000000 pyspapi-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 17:40:06.042276 pyspapi-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 17:39:56.000000 pyspapi-3.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:06.038276 pyspapi-3.1.1/pyspapi/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 17:39:56.000000 pyspapi-3.1.1/pyspapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:39:56.000000 pyspapi-3.1.1/pyspapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-18 17:39:56.000000 pyspapi-3.1.1/pyspapi/spworlds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:40:06.042276 pyspapi-3.1.1/pyspapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 17:40:05.000000 pyspapi-3.1.1/pyspapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 17:40:06.000000 pyspapi-3.1.1/pyspapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:40:05.000000 pyspapi-3.1.1/pyspapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 17:40:05.000000 pyspapi-3.1.1/pyspapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 17:40:05.000000 pyspapi-3.1.1/pyspapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 17:39:56.000000 pyspapi-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:40:06.042276 pyspapi-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 17:39:56.000000 pyspapi-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:59.085726 pyspapi-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 18:12:46.000000 pyspapi-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 18:12:46.000000 pyspapi-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 18:12:59.085726 pyspapi-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 18:12:46.000000 pyspapi-3.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:59.081726 pyspapi-3.1.2/pyspapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:59.085726 pyspapi-3.1.2/pyspapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/spworlds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:59.085726 pyspapi-3.1.2/pyspapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/types/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/types/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 18:12:46.000000 pyspapi-3.1.2/pyspapi/types/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:59.085726 pyspapi-3.1.2/pyspapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 18:12:59.000000 pyspapi-3.1.2/pyspapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-18 18:12:59.000000 pyspapi-3.1.2/pyspapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:12:59.000000 pyspapi-3.1.2/pyspapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 18:12:59.000000 pyspapi-3.1.2/pyspapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 18:12:59.000000 pyspapi-3.1.2/pyspapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 18:12:46.000000 pyspapi-3.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:12:59.085726 pyspapi-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-18 18:12:46.000000 pyspapi-3.1.2/setup.py
```

### Comparing `pyspapi-3.1.1/LICENSE` & `pyspapi-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspapi-3.1.1/PKG-INFO` & `pyspapi-3.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspapi
-Version: 3.1.1
+Version: 3.1.2
 Summary: API wrapper for SP servers written in Python
 Home-page: https://github.com/deesiigneer/pyspapi
 Author: deesiigneer
 License: MIT
 Project-URL: Documentation, https://pyspapi.readthedocs.io/ru/latest/
 Project-URL: GitHub, https://github.com/deesiigneer/pyspapi
 Project-URL: Discord, https://discord.com/invite/VbyHaKRAaN
```

### Comparing `pyspapi-3.1.1/README.rst` & `pyspapi-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyspapi-3.1.1/pyspapi/spworlds.py` & `pyspapi-3.1.2/pyspapi/spworlds.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     async def me(self):
         """
         Получает информацию об аккаунте текущего пользователя.
 
         :return: Объект Account, представляющий аккаунт текущего пользователя.
         :rtype: Account
         """
-        me = await self.__get('account/me')
+        me = await self.__get('accounts/me')
         return Account(
                 account_id=me['id'],
                 username=me['username'],
                 status=me['status'],
                 roles=me['roles'],
                 city=me['city'],
                 cards=me['cards'],
```

### Comparing `pyspapi-3.1.1/pyspapi.egg-info/PKG-INFO` & `pyspapi-3.1.2/pyspapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspapi
-Version: 3.1.1
+Version: 3.1.2
 Summary: API wrapper for SP servers written in Python
 Home-page: https://github.com/deesiigneer/pyspapi
 Author: deesiigneer
 License: MIT
 Project-URL: Documentation, https://pyspapi.readthedocs.io/ru/latest/
 Project-URL: GitHub, https://github.com/deesiigneer/pyspapi
 Project-URL: Discord, https://discord.com/invite/VbyHaKRAaN
```

### Comparing `pyspapi-3.1.1/setup.py` & `pyspapi-3.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 requirements = []
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 version = ""
 with open("pyspapi/__init__.py") as f:
@@ -17,30 +17,27 @@
 if not version:
     raise RuntimeError("Version is not set")
 
 readme = ""
 with open("README.rst") as f:
     readme = f.read()
 
-packages = [
-    "pyspapi"
-]
-
 setup(
     name='pyspapi',
     license='MIT',
     author='deesiigneer',
     version=version,
     url='https://github.com/deesiigneer/pyspapi',
     project_urls={
         "Documentation": "https://pyspapi.readthedocs.io/ru/latest/",
         "GitHub": "https://github.com/deesiigneer/pyspapi",
         "Discord": "https://discord.com/invite/VbyHaKRAaN"
     },
     description='API wrapper for SP servers written in Python',
     long_description=readme,
     long_description_content_type='text/x-rst',
-    packages=packages,
+    packages=find_packages(),
+    package_data={'pyspapi': ['types/*', 'api/*']},  # Включаем дополнительные файлы и папки
     include_package_data=True,
     install_requires=requirements,
     python_requires='>=3.8.0',
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

