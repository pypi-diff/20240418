# Comparing `tmp/types-hdbcli-2.20.0.20240331.tar.gz` & `tmp/types-hdbcli-2.20.0.20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hdbcli-2.20.0.20240331.tar", last modified: Sun Mar 31 02:18:22 2024, max compression
+gzip compressed data, was "types-hdbcli-2.20.0.20240418.tar", last modified: Thu Apr 18 02:16:49 2024, max compression
```

## Comparing `types-hdbcli-2.20.0.20240331.tar` & `types-hdbcli-2.20.0.20240418.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:22.447443 types-hdbcli-2.20.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-31 02:18:21.000000 types-hdbcli-2.20.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:21.000000 types-hdbcli-2.20.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-31 02:18:22.447443 types-hdbcli-2.20.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:22.447443 types-hdbcli-2.20.0.20240331/hdbcli-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-31 02:18:21.000000 types-hdbcli-2.20.0.20240331/hdbcli-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-31 02:17:27.000000 types-hdbcli-2.20.0.20240331/hdbcli-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-03-31 02:17:27.000000 types-hdbcli-2.20.0.20240331/hdbcli-stubs/dbapi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:21.000000 types-hdbcli-2.20.0.20240331/hdbcli-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 02:17:27.000000 types-hdbcli-2.20.0.20240331/hdbcli-stubs/resultrow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:22.447443 types-hdbcli-2.20.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-31 02:18:21.000000 types-hdbcli-2.20.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:22.447443 types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-31 02:18:22.000000 types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-31 02:18:22.000000 types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:22.000000 types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 02:18:22.000000 types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:49.626788 types-hdbcli-2.20.0.20240418/
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-18 02:16:49.626788 types-hdbcli-2.20.0.20240418/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:49.626788 types-hdbcli-2.20.0.20240418/hdbcli-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/hdbcli-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 02:16:27.000000 types-hdbcli-2.20.0.20240418/hdbcli-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-18 02:16:27.000000 types-hdbcli-2.20.0.20240418/hdbcli-stubs/dbapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/hdbcli-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 02:16:27.000000 types-hdbcli-2.20.0.20240418/hdbcli-stubs/resultrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:16:49.626788 types-hdbcli-2.20.0.20240418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:49.626788 types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 02:16:49.000000 types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/top_level.txt
```

### Comparing `types-hdbcli-2.20.0.20240331/CHANGELOG.md` & `types-hdbcli-2.20.0.20240418/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.20.0.20240418 (2024-04-18)
+
+Update Ruff and enable F821 in stubs (#11771)
+
 ## 2.20.0.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
 
 ## 2.20.0.20240321 (2024-03-21)
 
 [stubsabot] Bump hdbcli to 2.20.* (#11628)
```

### Comparing `types-hdbcli-2.20.0.20240331/PKG-INFO` & `types-hdbcli-2.20.0.20240418/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.20.0.20240331
+Version: 2.20.0.20240418
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-hdbcli` aims to provide accurate annotations
 for `hdbcli==2.20.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-hdbcli-2.20.0.20240331/hdbcli-stubs/dbapi.pyi` & `types-hdbcli-2.20.0.20240418/hdbcli-stubs/dbapi.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing_extensions import Self, TypeAlias
 
 from .resultrow import ResultRow
 
 apilevel: str
 threadsafety: int
 paramstyle: tuple[str, ...]  # hdbcli defines it as a tuple which does not follow PEP 249
-connect = Connection
 
 class Connection:
     def __init__(
         self,
         address: str,
         port: int,
         user: str,
@@ -36,14 +35,16 @@
     def getclientinfo(self, key: str = ...) -> str | dict[str, str]: ...
     def getproperty(self, *args, **kwargs): ...
     def isconnected(self) -> bool: ...
     def rollback(self) -> None: ...
     def setautocommit(self, auto: bool = ...) -> None: ...
     def setclientinfo(self, key: str, value: str | None = ...) -> None: ...
 
+connect = Connection
+
 class LOB:
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def close(self) -> bool: ...
     def find(self, object: str, length: int, position: int = ...) -> int: ...
     def read(self, size: int = ..., position: int = ...) -> str | bytes: ...
     def write(self, object: str | bytes) -> int: ...
```

### Comparing `types-hdbcli-2.20.0.20240331/hdbcli-stubs/resultrow.pyi` & `types-hdbcli-2.20.0.20240418/hdbcli-stubs/resultrow.pyi`

 * *Files identical despite different names*

### Comparing `types-hdbcli-2.20.0.20240331/setup.py` & `types-hdbcli-2.20.0.20240418/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-hdbcli` aims to provide accurate annotations
 for `hdbcli==2.20.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.20.0.20240331",
+      version="2.20.0.20240418",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md",
```

### Comparing `types-hdbcli-2.20.0.20240331/types_hdbcli.egg-info/PKG-INFO` & `types-hdbcli-2.20.0.20240418/types_hdbcli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hdbcli
-Version: 2.20.0.20240331
+Version: 2.20.0.20240418
 Summary: Typing stubs for hdbcli
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hdbcli.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-hdbcli` aims to provide accurate annotations
 for `hdbcli==2.20.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hdbcli. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

