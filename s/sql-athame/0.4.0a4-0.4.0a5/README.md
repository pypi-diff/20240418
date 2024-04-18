# Comparing `tmp/sql_athame-0.4.0a4.tar.gz` & `tmp/sql_athame-0.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a4.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a5.tar", max compression
```

## Comparing `sql_athame-0.4.0a4.tar` & `sql_athame-0.4.0a5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/LICENSE
--rw-r--r--   0        0        0    12086 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/README.md
--rw-r--r--   0        0        0      751 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/__init__.py
--rw-r--r--   0        0        0    10350 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/base.py
--rw-r--r--   0        0        0    19787 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      743 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/py.typed
--rw-r--r--   0        0        0     1305 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      412 2024-04-15 00:02:17.474692 sql_athame-0.4.0a4/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-18 14:38:46.803742 sql_athame-0.4.0a5/LICENSE
+-rw-r--r--   0        0        0    12086 2024-04-18 14:38:46.803742 sql_athame-0.4.0a5/README.md
+-rw-r--r--   0        0        0      751 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10350 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/base.py
+-rw-r--r--   0        0        0    20442 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      743 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/py.typed
+-rw-r--r--   0        0        0     1305 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      412 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a5/PKG-INFO
```

### Comparing `sql_athame-0.4.0a4/LICENSE` & `sql_athame-0.4.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a4/README.md` & `sql_athame-0.4.0a5/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a4/pyproject.toml` & `sql_athame-0.4.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-4"
+version = "0.4.0-alpha-5"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a4/sql_athame/base.py` & `sql_athame-0.4.0a5/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a4/sql_athame/dataclasses.py` & `sql_athame-0.4.0a5/sql_athame/dataclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -454,39 +454,54 @@
         if cls.array_safe_insert:
             return await cls.insert_multiple_array_safe(connection_or_pool, rows)
         else:
             return await cls.insert_multiple_unnest(connection_or_pool, rows)
 
     @classmethod
     async def upsert_multiple_unnest(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: Type[T],
+        connection_or_pool: Union[Connection, Pool],
+        rows: Iterable[T],
+        insert_only: FieldNamesSet = (),
     ) -> str:
         return await connection_or_pool.execute(
-            *cls.upsert_sql(cls.insert_multiple_sql(rows))
+            *cls.upsert_sql(cls.insert_multiple_sql(rows), exclude=insert_only)
         )
 
     @classmethod
     async def upsert_multiple_array_safe(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: Type[T],
+        connection_or_pool: Union[Connection, Pool],
+        rows: Iterable[T],
+        insert_only: FieldNamesSet = (),
     ) -> str:
         last = ""
         for chunk in chunked(rows, 100):
             last = await connection_or_pool.execute(
-                *cls.upsert_sql(cls.insert_multiple_array_safe_sql(chunk))
+                *cls.upsert_sql(
+                    cls.insert_multiple_array_safe_sql(chunk), exclude=insert_only
+                )
             )
         return last
 
     @classmethod
     async def upsert_multiple(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: Type[T],
+        connection_or_pool: Union[Connection, Pool],
+        rows: Iterable[T],
+        insert_only: FieldNamesSet = (),
     ) -> str:
         if cls.array_safe_insert:
-            return await cls.upsert_multiple_array_safe(connection_or_pool, rows)
+            return await cls.upsert_multiple_array_safe(
+                connection_or_pool, rows, insert_only=insert_only
+            )
         else:
-            return await cls.upsert_multiple_unnest(connection_or_pool, rows)
+            return await cls.upsert_multiple_unnest(
+                connection_or_pool, rows, insert_only=insert_only
+            )
 
     @classmethod
     def _get_equal_ignoring_fn(
         cls: Type[T], ignore: FieldNamesSet = ()
     ) -> Callable[[T, T], bool]:
         env: Dict[str, Any] = dict()
         func = ["def equal_ignoring(a, b):"]
@@ -501,17 +516,19 @@
     async def replace_multiple(
         cls: Type[T],
         connection: Connection,
         rows: Union[Iterable[T], Iterable[Mapping[str, Any]]],
         *,
         where: Where,
         ignore: FieldNamesSet = (),
+        insert_only: FieldNamesSet = (),
     ) -> Tuple[List[T], List[T], List[T]]:
+        ignore = sorted(set(ignore) | set(insert_only))
         equal_ignoring = cls._cached(
-            ("equal_ignoring", tuple(sorted(ignore))),
+            ("equal_ignoring", tuple(ignore)),
             lambda: cls._get_equal_ignoring_fn(ignore),
         )
         pending = {row.primary_key(): row for row in map(cls.ensure_model, rows)}
 
         updated = []
         deleted = []
 
@@ -525,15 +542,17 @@
                 if not equal_ignoring(old, pending[pk]):
                     updated.append(pending[pk])
                 del pending[pk]
 
         created = list(pending.values())
 
         if created or updated:
-            await cls.upsert_multiple(connection, (*created, *updated))
+            await cls.upsert_multiple(
+                connection, (*created, *updated), insert_only=insert_only
+            )
         if deleted:
             await cls.delete_multiple(connection, deleted)
 
         return created, updated, deleted
 
     @classmethod
     def _get_differences_ignoring_fn(
@@ -557,17 +576,19 @@
     async def replace_multiple_reporting_differences(
         cls: Type[T],
         connection: Connection,
         rows: Union[Iterable[T], Iterable[Mapping[str, Any]]],
         *,
         where: Where,
         ignore: FieldNamesSet = (),
+        insert_only: FieldNamesSet = (),
     ) -> Tuple[List[T], List[Tuple[T, T, List[str]]], List[T]]:
+        ignore = sorted(set(ignore) | set(insert_only))
         differences_ignoring = cls._cached(
-            ("differences_ignoring", tuple(sorted(ignore))),
+            ("differences_ignoring", tuple(ignore)),
             lambda: cls._get_differences_ignoring_fn(ignore),
         )
 
         pending = {row.primary_key(): row for row in map(cls.ensure_model, rows)}
 
         updated_triples = []
         deleted = []
@@ -584,15 +605,17 @@
                     updated_triples.append((old, pending[pk], diffs))
                 del pending[pk]
 
         created = list(pending.values())
 
         if created or updated_triples:
             await cls.upsert_multiple(
-                connection, (*created, *(t[1] for t in updated_triples))
+                connection,
+                (*created, *(t[1] for t in updated_triples)),
+                insert_only=insert_only,
             )
         if deleted:
             await cls.delete_multiple(connection, deleted)
 
         return created, updated_triples, deleted
```

### Comparing `sql_athame-0.4.0a4/sql_athame/escape.py` & `sql_athame-0.4.0a5/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a4/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a5/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a4/PKG-INFO` & `sql_athame-0.4.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a4
+Version: 0.4.0a5
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

