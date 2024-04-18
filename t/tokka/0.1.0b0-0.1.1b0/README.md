# Comparing `tmp/tokka-0.1.0b0.tar.gz` & `tmp/tokka-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokka-0.1.0b0.tar", last modified: Sun Apr 14 23:02:17 2024, max compression
+gzip compressed data, was "tokka-0.1.1b0.tar", last modified: Thu Apr 18 01:51:47 2024, max compression
```

## Comparing `tokka-0.1.0b0.tar` & `tokka-0.1.1b0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1077 2024-04-14 22:56:22.919410 tokka-0.1.0b0/LICENSE
--rw-r--r--   0        0        0     2337 2024-04-14 23:00:47.339365 tokka-0.1.0b0/README.md
--rw-r--r--   0        0        0     2279 2024-04-14 23:02:17.529351 tokka-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0    10034 2024-04-14 22:25:35.389706 tokka-0.1.0b0/src/tokka/__init__.py
--rw-r--r--   0        0        0     1539 2024-04-14 22:25:35.389706 tokka-0.1.0b0/src/tokka/kwargs.py
--rw-r--r--   0        0        0        0 2024-04-12 18:12:04.269756 tokka-0.1.0b0/tests/__init__.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 tokka-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-14 22:56:22.919410 tokka-0.1.1b0/LICENSE
+-rw-r--r--   0        0        0     4058 2024-04-18 01:43:03.815019 tokka-0.1.1b0/README.md
+-rw-r--r--   0        0        0     2330 2024-04-18 01:51:47.331303 tokka-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0    20243 2024-04-18 01:43:03.825019 tokka-0.1.1b0/src/tokka/__init__.py
+-rw-r--r--   0        0        0     1746 2024-04-18 01:43:03.815019 tokka-0.1.1b0/src/tokka/kwargs.py
+-rw-r--r--   0        0        0        0 2024-04-12 18:12:04.269756 tokka-0.1.1b0/tests/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-18 01:43:03.815019 tokka-0.1.1b0/tests/conftest.py
+-rw-r--r--   0        0        0      233 2024-04-18 01:43:03.815019 tokka-0.1.1b0/tests/test_connection.py
+-rw-r--r--   0        0        0     4619 2024-04-18 01:43:03.825019 tokka-0.1.1b0/tests/test_queries.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 tokka-0.1.1b0/PKG-INFO
```

### Comparing `tokka-0.1.0b0/LICENSE` & `tokka-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokka-0.1.0b0/pyproject.toml` & `tokka-0.1.1b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tokka"
-version = "0.1.0b"
+version = "0.1.1b"
 description = "A thin async layer between Pydantic and MongoDB"
 authors = [
     { name = "ericmiguel", email = "eric.mrib@gmail.com" },
 ]
 dependencies = [
     "motor>=3.4.0",
     "pydantic>=2.7.0",
@@ -130,8 +130,10 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff>=0.3.7",
     "icecream>=2.1.3",
+    "pytest>=8.1.1",
+    "pytest-asyncio>=0.23.6",
 ]
```

### Comparing `tokka-0.1.0b0/src/tokka/kwargs.py` & `tokka-0.1.1b0/src/tokka/kwargs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""Type aliases and TypedDicts for the kwargs of the methods in the tokka module."""
+
 from typing import Any
 from typing import Literal
 from typing import Mapping
 from typing import Sequence
 from typing import Tuple
 from typing import TypeAlias
 from typing import TypedDict
 
-from motor.motor_asyncio import AsyncIOMotorClient
+from motor.motor_asyncio import AsyncIOMotorClientSession
 from pydantic.main import IncEx
 from pymongo.typings import _CollationIn
 
 
 Sort: TypeAlias = tuple[
     str | Sequence[str | Tuple[str, int | str | Mapping[str, Any]]] | Mapping[str, Any],
     int | str,
@@ -22,14 +24,16 @@
 
 Hint: TypeAlias = (
     str | Sequence[str | Tuple[str, int | str | Mapping[str, Any]]] | Mapping[str, Any]
 )
 
 
 class FindKwargs(TypedDict, total=False):
+    """MongoDB find method keyword arguments."""
+
     projection: dict[str, Any]
     skip: int
     limit: int
     no_cursor_timeout: bool
     cursor_type: Literal[0, 1]
 
     # see cursor.html#pymongo.cursor.Cursor.sort
@@ -44,19 +48,21 @@
     max_time_ms: int
     max: MinMax
     min: MinMax
     return_key: bool
     show_record_id: bool
     snapshot: bool
     comment: Any
-    session: AsyncIOMotorClient
+    session: AsyncIOMotorClientSession
     allow_disk_use: bool
 
 
 class ModelDumpKwargs(TypedDict, total=False):
+    """Pydantic model dump method keyword arguments."""
+
     mode: Literal["json", "python"]
     include: IncEx
     exclude: IncEx
     by_alias: bool
     exclude_unset: bool
     exclude_defaults: bool
     exclude_none: bool
```

