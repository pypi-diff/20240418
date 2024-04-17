# Comparing `tmp/setuptools-ext-0.5.tar.gz` & `tmp/setuptools_ext-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-ext-0.5.tar", last modified: Thu Oct 27 06:57:36 2022, max compression
+gzip compressed data, was "setuptools_ext-0.6.tar", last modified: Wed Apr 17 22:01:50 2024, max compression
```

## Comparing `setuptools-ext-0.5.tar` & `setuptools_ext-0.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2022-10-27 06:57:36.472481 setuptools-ext-0.5/
--rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools-ext-0.5/LICENSE
--rw-r--r--   0 wim        (501) staff       (20)     9127 2022-10-27 06:57:36.472276 setuptools-ext-0.5/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)     8753 2022-04-22 04:08:11.000000 setuptools-ext-0.5/README.rst
--rw-r--r--   0 wim        (501) staff       (20)      708 2022-10-27 06:55:42.000000 setuptools-ext-0.5/pyproject.toml
--rw-r--r--   0 wim        (501) staff       (20)       38 2022-10-27 06:57:36.472520 setuptools-ext-0.5/setup.cfg
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2022-10-27 06:57:36.472085 setuptools-ext-0.5/setuptools_ext.egg-info/
--rw-r--r--   0 wim        (501) staff       (20)     9127 2022-10-27 06:57:36.000000 setuptools-ext-0.5/setuptools_ext.egg-info/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)      240 2022-10-27 06:57:36.000000 setuptools-ext-0.5/setuptools_ext.egg-info/SOURCES.txt
--rw-r--r--   0 wim        (501) staff       (20)        1 2022-10-27 06:57:36.000000 setuptools-ext-0.5/setuptools_ext.egg-info/dependency_links.txt
--rw-r--r--   0 wim        (501) staff       (20)      159 2022-10-27 06:57:36.000000 setuptools-ext-0.5/setuptools_ext.egg-info/requires.txt
--rw-r--r--   0 wim        (501) staff       (20)       15 2022-10-27 06:57:36.000000 setuptools-ext-0.5/setuptools_ext.egg-info/top_level.txt
--rw-r--r--   0 wim        (501) staff       (20)     4377 2022-10-27 06:55:42.000000 setuptools-ext-0.5/setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.788884 setuptools_ext-0.6/
+-rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools_ext-0.6/LICENSE
+-rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-17 22:01:50.788585 setuptools_ext-0.6/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)     8751 2022-10-27 07:06:15.000000 setuptools_ext-0.6/README.rst
+-rw-r--r--   0 wim        (501) staff       (20)      564 2024-04-17 22:01:11.000000 setuptools_ext-0.6/pyproject.toml
+-rw-r--r--   0 wim        (501) staff       (20)       38 2024-04-17 22:01:50.789125 setuptools_ext-0.6/setup.cfg
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.788323 setuptools_ext-0.6/setuptools_ext.egg-info/
+-rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)      269 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 wim        (501) staff       (20)        1 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 wim        (501) staff       (20)       53 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/requires.txt
+-rw-r--r--   0 wim        (501) staff       (20)       15 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/top_level.txt
+-rw-r--r--   0 wim        (501) staff       (20)     4246 2024-04-17 22:01:11.000000 setuptools_ext-0.6/setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.787951 setuptools_ext-0.6/tests/
+-rw-r--r--   0 wim        (501) staff       (20)     3316 2024-04-17 22:01:11.000000 setuptools_ext-0.6/tests/test_setuptools_ext.py
```

### Comparing `setuptools-ext-0.5/LICENSE` & `setuptools_ext-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-ext-0.5/PKG-INFO` & `setuptools_ext-0.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: setuptools-ext
-Version: 0.5
-Summary: Extension of setuptools to support all core metadata fields
-Author: Wim Glenn
-Author-email: hey@wimglenn.com
-License: MIT
-Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
-Keywords: setuptools,packaging,metadata
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-License-File: LICENSE
-
 |pypi|_ |actions|_ |codecov|_ |womm|_
 
 .. |pypi| image:: https://img.shields.io/pypi/v/setuptools-ext.svg
 .. _pypi: https://pypi.org/project/setuptools-ext
 
 .. |actions| image:: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/badge.svg
 .. _actions: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/
 
-.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/master/graph/badge.svg
+.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/main/graph/badge.svg
 .. _codecov: https://codecov.io/gh/wimglenn/setuptools-ext
 
 .. |womm| image:: https://cdn.rawgit.com/nikku/works-on-my-machine/v0.2.0/badge.svg
 .. _womm: https://github.com/nikku/works-on-my-machine
 
 setuptools-ext
 ==============
```

### Comparing `setuptools-ext-0.5/README.rst` & `setuptools_ext-0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+Metadata-Version: 2.1
+Name: setuptools-ext
+Version: 0.6
+Summary: Extension of setuptools to support all core metadata fields
+Author: Wim Glenn
+Author-email: hey@wimglenn.com
+License: MIT
+Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
+Keywords: setuptools,packaging,metadata
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: setuptools>=61.0.0
+Requires-Dist: tomli; python_version < "3.11"
+
 |pypi|_ |actions|_ |codecov|_ |womm|_
 
 .. |pypi| image:: https://img.shields.io/pypi/v/setuptools-ext.svg
 .. _pypi: https://pypi.org/project/setuptools-ext
 
 .. |actions| image:: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/badge.svg
 .. _actions: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/
 
-.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/master/graph/badge.svg
+.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/main/graph/badge.svg
 .. _codecov: https://codecov.io/gh/wimglenn/setuptools-ext
 
 .. |womm| image:: https://cdn.rawgit.com/nikku/works-on-my-machine/v0.2.0/badge.svg
 .. _womm: https://github.com/nikku/works-on-my-machine
 
 setuptools-ext
 ==============
```

### Comparing `setuptools-ext-0.5/pyproject.toml` & `setuptools_ext-0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "setuptools-ext"
-version = "0.5"
+version = "0.6"
+requires-python = ">= 3.7"
 description = "Extension of setuptools to support all core metadata fields"
 authors = [
     {name = "Wim Glenn"},
     {email = "hey@wimglenn.com"},
 ]
 readme = "README.rst"
 keywords = ["setuptools", "packaging", "metadata"]
 license = {text = "MIT"}
 dependencies = [
-    "setuptools >= 61.0.0; python_version >= '3.7'",
-    "setuptools",
-    "toml; python_version < '3.11'",
-    "pathlib2; python_version < '3.5'",
-]
-
-[project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "wheel",
+    "setuptools >= 61.0.0",
+    "tomli; python_version < '3.11'",
 ]
 
 [project.urls]
 Homepage = "https://github.com/wimglenn/setuptools-ext"
```

### Comparing `setuptools-ext-0.5/setuptools_ext.egg-info/PKG-INFO` & `setuptools_ext-0.6/setuptools_ext.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: setuptools-ext
-Version: 0.5
+Version: 0.6
 Summary: Extension of setuptools to support all core metadata fields
 Author: Wim Glenn
 Author-email: hey@wimglenn.com
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
 Keywords: setuptools,packaging,metadata
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0.0
+Requires-Dist: tomli; python_version < "3.11"
 
 |pypi|_ |actions|_ |codecov|_ |womm|_
 
 .. |pypi| image:: https://img.shields.io/pypi/v/setuptools-ext.svg
 .. _pypi: https://pypi.org/project/setuptools-ext
 
 .. |actions| image:: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/badge.svg
 .. _actions: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/
 
-.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/master/graph/badge.svg
+.. |codecov| image:: https://codecov.io/gh/wimglenn/setuptools-ext/branch/main/graph/badge.svg
 .. _codecov: https://codecov.io/gh/wimglenn/setuptools-ext
 
 .. |womm| image:: https://cdn.rawgit.com/nikku/works-on-my-machine/v0.2.0/badge.svg
 .. _womm: https://github.com/nikku/works-on-my-machine
 
 setuptools-ext
 ==============
```

### Comparing `setuptools-ext-0.5/setuptools_ext.py` & `setuptools_ext-0.6/setuptools_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 """Extension of setuptools to support all core metadata fields"""
-from __future__ import unicode_literals
-
 import base64
-import email
+import email.policy
 import hashlib
-import sys
+from pathlib import Path
 from zipfile import ZipFile
-from setuptools.build_meta import build_wheel as orig_build_wheel
-from setuptools.build_meta import *
 
-try:
-    from pathlib import Path
-except ImportError:
-    from pathlib2 import Path
+from setuptools.build_meta import *
+from setuptools.build_meta import build_wheel as orig_build_wheel
 try:
     # stdlib Python 3.11+
     import tomllib as toml
 except ImportError:
-    import toml
-
-
-PY2 = sys.version_info < (3,)
+    import tomli as toml
 
 
 allowed_fields = {
     x.lower(): x
     for x in [
         "Platform",
         "Supported-Platform",
@@ -61,22 +52,21 @@
     pkginfo = email.message_from_string(data.decode())
     # delete some annoying kv that distutils seems to put in there for no reason
     for key in dict(pkginfo):
         if pkginfo.get_all(key) == ["UNKNOWN"]:
             if key.lower() not in ["metadata-version", "name", "version"]:
                 del pkginfo[key]
     new_headers = extra_metadata.items()
-    if PY2:
-        new_headers.sort()
     for key, vals in new_headers:
         already_present = pkginfo.get_all(key, [])
         for val in vals:
             if val not in already_present:
                 pkginfo.add_header(key, val)
-    result = pkginfo.as_string() if PY2 else pkginfo.as_bytes()
+    policy = email.policy.Compat32(max_line_length=0)
+    result = pkginfo.as_bytes(policy=policy)
     return result
 
 
 def rewrite_record(data, new_line):
     lines = []
     for line in data.decode().splitlines():
         fname = line.split(",")[0]
```

