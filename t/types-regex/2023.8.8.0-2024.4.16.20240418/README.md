# Comparing `tmp/types-regex-2023.8.8.0.tar.gz` & `tmp/types-regex-2024.4.16.20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2023.8.8.0.tar", last modified: Thu Aug 10 01:15:57 2023, max compression
+gzip compressed data, was "types-regex-2024.4.16.20240418.tar", last modified: Thu Apr 18 02:16:43 2024, max compression
```

## Comparing `types-regex-2023.8.8.0.tar` & `types-regex-2024.4.16.20240418.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 01:15:57.324126 types-regex-2023.8.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-10 01:15:56.000000 types-regex-2023.8.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-10 01:15:56.000000 types-regex-2023.8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-10 01:15:57.324126 types-regex-2023.8.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 01:15:57.324126 types-regex-2023.8.8.0/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-10 01:15:56.000000 types-regex-2023.8.8.0/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-10 01:15:39.000000 types-regex-2023.8.8.0/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-10 01:15:39.000000 types-regex-2023.8.8.0/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-10 01:15:39.000000 types-regex-2023.8.8.0/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-08-10 01:15:39.000000 types-regex-2023.8.8.0/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-10 01:15:57.324126 types-regex-2023.8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-10 01:15:56.000000 types-regex-2023.8.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 01:15:57.324126 types-regex-2023.8.8.0/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-10 01:15:57.000000 types-regex-2023.8.8.0/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-10 01:15:57.000000 types-regex-2023.8.8.0/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-10 01:15:57.000000 types-regex-2023.8.8.0/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-10 01:15:57.000000 types-regex-2023.8.8.0/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.086822 types-regex-2024.4.16.20240418/
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-04-18 02:16:27.000000 types-regex-2024.4.16.20240418/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:16:43.086822 types-regex-2024.4.16.20240418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-18 02:16:41.000000 types-regex-2024.4.16.20240418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:16:43.082822 types-regex-2024.4.16.20240418/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 02:16:43.000000 types-regex-2024.4.16.20240418/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2023.8.8.0/CHANGELOG.md` & `types-regex-2024.4.16.20240418/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+## 2024.4.16.20240418 (2024-04-18)
+
+[stubsabot] Bump regex to 2024.4.16 (#11773)
+
+## 2023.12.25.20240311 (2024-03-11)
+
+Use PEP 570 syntax in third party stubs (#11554)
+
+## 2023.12.25.20240106 (2024-01-06)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
+## 2023.12.25.20231225 (2023-12-25)
+
+[stubsabot] Bump regex to 2023.12.25 (#11198)
+
+## 2023.10.3.0 (2023-10-04)
+
+[stubsabot] Bump regex to 2023.10.3 (#10832)
+
 ## 2023.8.8.0 (2023-08-10)
 
 [stubsabot] Bump regex to 2023.8.8 (#10553)
 
 Release: https://pypi.org/pypi/regex/2023.8.8
 Homepage: https://github.com/mrabarnett/mrab-regex
 Repository: https://github.com/mrabarnett/mrab-regex
```

### Comparing `types-regex-2023.8.8.0/PKG-INFO` & `types-regex-2024.4.16.20240418/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.8.8.0
+Version: 2024.4.16.20240418
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for regex
 
-This is a PEP 561 type stub package for the `regex` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`regex`](https://github.com/mrabarnett/mrab-regex) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`regex`. The source for this package can be found at
+`regex`.
+
+This version of `types-regex` aims to provide accurate annotations
+for `regex==2024.4.16`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9647d964d0db817fe34fba4814a05888a6fbfe85` and was tested
-with mypy 1.4.1, pyright 1.1.320, and
-pytype 2023.7.21.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-regex-2023.8.8.0/regex-stubs/_regex.pyi` & `types-regex-2024.4.16.20240418/regex-stubs/_regex.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This is actually a C-extension module.
 # Not all types defined in C are exported to Python.
 # For example: `Pattern` and `Match` are not exported
 # and are redefined in `regex.regex module.
 
-from typing import Any, AnyStr, Generic
-from typing_extensions import Self, final
+from typing import Any, AnyStr, Generic, final
+from typing_extensions import Self
 
 from .regex import Match, Pattern
 
 @final
 class Splitter(Generic[AnyStr]):
     @property
     def pattern(self) -> Pattern[AnyStr]: ...
```

### Comparing `types-regex-2023.8.8.0/regex-stubs/_regex_core.pyi` & `types-regex-2024.4.16.20240418/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.8.8.0/regex-stubs/regex.pyi` & `types-regex-2024.4.16.20240418/regex-stubs/regex.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from _typeshed import ReadableBuffer
 from collections.abc import Callable, Mapping
-from typing import Any, AnyStr, Generic, TypeVar, overload
-from typing_extensions import Literal, Self, final
+from typing import Any, AnyStr, Generic, Literal, TypeVar, final, overload
+from typing_extensions import Self
 
 from . import _regex
 from ._regex_core import *
 
 if sys.version_info >= (3, 9):
     from types import GenericAlias
 
@@ -589,62 +589,62 @@
     @property
     def regs(self) -> tuple[tuple[int, int], ...]: ...
     @property
     def fuzzy_counts(self) -> tuple[int, int, int]: ...
     @property
     def fuzzy_changes(self) -> tuple[list[int], list[int], list[int]]: ...
     @overload
-    def group(self, __group: Literal[0] = 0) -> AnyStr: ...
+    def group(self, group: Literal[0] = 0, /) -> AnyStr: ...
     @overload
-    def group(self, __group: int | str = ...) -> AnyStr | Any: ...
+    def group(self, group: int | str = ..., /) -> AnyStr | Any: ...
     @overload
-    def group(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[AnyStr | Any, ...]: ...
+    def group(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[AnyStr | Any, ...]: ...
     @overload
     def groups(self, default: None = None) -> tuple[AnyStr | Any, ...]: ...
     @overload
     def groups(self, default: _T) -> tuple[AnyStr | _T, ...]: ...
     @overload
     def groupdict(self, default: None = None) -> dict[str, AnyStr | Any]: ...
     @overload
     def groupdict(self, default: _T) -> dict[str, AnyStr | _T]: ...
     @overload
-    def span(self, __group: int | str = ...) -> tuple[int, int]: ...
+    def span(self, group: int | str = ..., /) -> tuple[int, int]: ...
     @overload
-    def span(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[tuple[int, int], ...]: ...
+    def span(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[tuple[int, int], ...]: ...
     @overload
-    def spans(self, __group: int | str = ...) -> list[tuple[int, int]]: ...
+    def spans(self, group: int | str = ..., /) -> list[tuple[int, int]]: ...
     @overload
-    def spans(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[list[tuple[int, int]], ...]: ...
+    def spans(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[list[tuple[int, int]], ...]: ...
     @overload
-    def start(self, __group: int | str = ...) -> int: ...
+    def start(self, group: int | str = ..., /) -> int: ...
     @overload
-    def start(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[int, ...]: ...
+    def start(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[int, ...]: ...
     @overload
-    def starts(self, __group: int | str = ...) -> list[int]: ...
+    def starts(self, group: int | str = ..., /) -> list[int]: ...
     @overload
-    def starts(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[list[int], ...]: ...
+    def starts(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[list[int], ...]: ...
     @overload
-    def end(self, __group: int | str = ...) -> int: ...
+    def end(self, group: int | str = ..., /) -> int: ...
     @overload
-    def end(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[int, ...]: ...
+    def end(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[int, ...]: ...
     @overload
-    def ends(self, __group: int | str = ...) -> list[int]: ...
+    def ends(self, group: int | str = ..., /) -> list[int]: ...
     @overload
-    def ends(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[list[int], ...]: ...
+    def ends(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[list[int], ...]: ...
     def expand(self, template: AnyStr) -> AnyStr: ...
     def expandf(self, format: AnyStr) -> AnyStr: ...
     @overload
-    def captures(self, __group: int | str = ...) -> list[AnyStr]: ...
+    def captures(self, group: int | str = ..., /) -> list[AnyStr]: ...
     @overload
-    def captures(self, __group1: int | str, __group2: int | str, *groups: int | str) -> tuple[list[AnyStr], ...]: ...
+    def captures(self, group1: int | str, group2: int | str, /, *groups: int | str) -> tuple[list[AnyStr], ...]: ...
     def capturesdict(self) -> dict[str, list[AnyStr]]: ...
     def detach_string(self) -> None: ...
     def allcaptures(self) -> tuple[list[AnyStr]]: ...
     def allspans(self) -> tuple[list[tuple[int, int]]]: ...
     @overload
-    def __getitem__(self, __key: Literal[0]) -> AnyStr: ...
+    def __getitem__(self, key: Literal[0], /) -> AnyStr: ...
     @overload
-    def __getitem__(self, __key: int | str) -> AnyStr | Any: ...
+    def __getitem__(self, key: int | str, /) -> AnyStr | Any: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self) -> Self: ...
     if sys.version_info >= (3, 9):
         def __class_getitem__(cls, item: Any) -> GenericAlias: ...
```

### Comparing `types-regex-2023.8.8.0/setup.py` & `types-regex-2024.4.16.20240418/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-regex"
 description = "Typing stubs for regex"
 long_description = '''
 ## Typing stubs for regex
 
-This is a PEP 561 type stub package for the `regex` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`regex`](https://github.com/mrabarnett/mrab-regex) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`regex`. The source for this package can be found at
+`regex`.
+
+This version of `types-regex` aims to provide accurate annotations
+for `regex==2024.4.16`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9647d964d0db817fe34fba4814a05888a6fbfe85` and was tested
-with mypy 1.4.1, pyright 1.1.320, and
-pytype 2023.7.21.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2023.8.8.0",
+      version="2024.4.16.20240418",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['regex-stubs'],
-      package_data={'regex-stubs': ['__init__.pyi', '_regex.pyi', '_regex_core.pyi', 'regex.pyi', 'METADATA.toml']},
+      package_data={'regex-stubs': ['__init__.pyi', '_regex.pyi', '_regex_core.pyi', 'regex.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-regex-2023.8.8.0/types_regex.egg-info/PKG-INFO` & `types-regex-2024.4.16.20240418/types_regex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.8.8.0
+Version: 2024.4.16.20240418
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for regex
 
-This is a PEP 561 type stub package for the `regex` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`regex`](https://github.com/mrabarnett/mrab-regex) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`regex`. The source for this package can be found at
+`regex`.
+
+This version of `types-regex` aims to provide accurate annotations
+for `regex==2024.4.16`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9647d964d0db817fe34fba4814a05888a6fbfe85` and was tested
-with mypy 1.4.1, pyright 1.1.320, and
-pytype 2023.7.21.
+This package was generated from typeshed commit `12b9e48324df292379db3eca4e3c54175e5f374e` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

