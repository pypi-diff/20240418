# Comparing `tmp/file_iter-0.1.0.tar.gz` & `tmp/file_iter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_iter-0.1.0.tar", max compression
+gzip compressed data, was "file_iter-0.1.1.tar", max compression
```

## Comparing `file_iter-0.1.0.tar` & `file_iter-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.0/LICENSE
--rw-r--r--   0        0        0     1888 2024-04-06 14:54:46.000216 file_iter-0.1.0/README.md
--rw-r--r--   0        0        0      106 2024-04-06 16:59:35.449657 file_iter-0.1.0/file_iter/__init__.py
--rw-r--r--   0        0        0     9520 2024-04-06 14:54:46.000216 file_iter-0.1.0/file_iter/file_iter.py
--rw-r--r--   0        0        0      914 2024-04-06 17:25:44.295575 file_iter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 file_iter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-05 19:06:27.300345 file_iter-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1894 2024-04-12 14:11:20.845268 file_iter-0.1.1/README.md
+-rw-r--r--   0        0        0      106 2024-04-06 16:59:35.449657 file_iter-0.1.1/file_iter/__init__.py
+-rw-r--r--   0        0        0     9552 2024-04-12 14:17:04.345030 file_iter-0.1.1/file_iter/file_iter.py
+-rw-r--r--   0        0        0      915 2024-04-11 21:42:53.651502 file_iter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 file_iter-0.1.1/PKG-INFO
```

### Comparing `file_iter-0.1.0/LICENSE` & `file_iter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `file_iter-0.1.0/README.md` & `file_iter-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Peek at the next line: `peek()`
 - Jump ahead `n` lines `jump(n)`
 - Check if empty: `isempty()`
 - Filter out unimportant lines:
     - Always filter: `FileIter(f, filter_func=is_data)`
     - Filter only single next(): `filter_next(filter_func)`
 
-```
+```python
 >>> def is_data(line: str) -> bool:
 ...    return len(line) > 0 and (line[0] != "#")
 >>> my_iter = FileIter(
 ...     ["Hello", "", "# comment", "World", "How", "are", "you?"],
 ...     filter_func=is_data
 ... )
 >>> next(my_iter)
```

### Comparing `file_iter-0.1.0/file_iter/file_iter.py` & `file_iter-0.1.1/file_iter/file_iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import itertools
 from collections import deque
 from pathlib import Path
-from typing import Any, Callable, Iterable, Iterator, Literal, TypeVar, overload
+from typing import Any, Callable, Iterable, Iterator, Literal, overload
 
-T = TypeVar("T")
-D = TypeVar("D", bound=Any)
 _marker: Any = object()
 
 
 class FileIter(Iterator[str]):
     """
     A Swiss Army knife iterator for files (or any iterator of strings)
 
@@ -100,24 +98,28 @@
         """
         line = self._cache.popleft() if self._cache else next(self._it)
         self._current_line = line.strip()
         self._position += 1
         return self._current_line
 
     @overload
-    def filtered_next(self, filter_func: Callable[[str], bool]) -> str: ...
+    def filtered_next(self, filter_func: Callable[[str], bool]) -> str:
+        ...
 
     @overload
-    def filtered_next(self, filter_func: Callable[[str], bool], default: T) -> str | T: ...
+    def filtered_next(
+        self, filter_func: Callable[[str], bool], default: object
+    ) -> str | object:
+        ...
 
     def filtered_next(
         self,
         filter_func: Callable[[str], bool],
-        default: str | T = _marker,
-    ) -> str | T:
+        default: str | object = _marker,
+    ) -> str | object:
         """
         Get the next element in the iterator that passes the filter function
 
         :param filter_func: a function that checks if the line is valid
 
         >>> my_iter = FileIter(["", "# comment", "hello"])
         >>> my_iter.filtered_next(is_data)
@@ -202,20 +204,22 @@
 
         for _ in itertools.islice(self, num - 1):
             pass
 
         return next(self)
 
     @overload
-    def peek(self) -> str: ...
+    def peek(self) -> str:
+        ...
 
     @overload
-    def peek(self, default: D) -> D | str: ...
+    def peek(self, default: object) -> object | str:
+        ...
 
-    def peek(self, default: D = _marker) -> D | str:
+    def peek(self, default: object = _marker) -> object | str:
         """
         Get the next element in the iterator without consuming it
 
         Note: peek does not respect the filter function
 
         :param default: the value to return if the iterator is empty
         :return: the next element in the iterator
```

### Comparing `file_iter-0.1.0/pyproject.toml` & `file_iter-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "file_iter"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Swiss Army knife iterator for files (or any iterator of strings)"
 authors = ["Jonathon Vandezande"]
 keywords = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jevandezande/file_iter"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = ">=3.12"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "*"
 pre-commit = "*"
 ruff = ">=0.3.0"
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `file_iter-0.1.0/PKG-INFO` & `file_iter-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: file-iter
-Version: 0.1.0
+Name: file_iter
+Version: 0.1.1
 Summary: A Swiss Army knife iterator for files (or any iterator of strings)
 Home-page: https://github.com/jevandezande/file_iter
 License: MIT
 Author: Jonathon Vandezande
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/jevandezande/file_iter
 Description-Content-Type: text/markdown
 
 # File Iter
 
 [![License](https://img.shields.io/github/license/jevandezande/file_iter)](https://github.com/jevandezande/file_iter/blob/master/LICENSE)
 [![Code style: ruff](https://img.shields.io/badge/code%20style-ruff-000000.svg)](https://github.com/astral-sh/ruff)
@@ -27,15 +28,15 @@
 - Peek at the next line: `peek()`
 - Jump ahead `n` lines `jump(n)`
 - Check if empty: `isempty()`
 - Filter out unimportant lines:
     - Always filter: `FileIter(f, filter_func=is_data)`
     - Filter only single next(): `filter_next(filter_func)`
 
-```
+```python
 >>> def is_data(line: str) -> bool:
 ...    return len(line) > 0 and (line[0] != "#")
 >>> my_iter = FileIter(
 ...     ["Hello", "", "# comment", "World", "How", "are", "you?"],
 ...     filter_func=is_data
 ... )
 >>> next(my_iter)
```

