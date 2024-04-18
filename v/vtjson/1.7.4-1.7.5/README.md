# Comparing `tmp/vtjson-1.7.4.tar.gz` & `tmp/vtjson-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.7.4.tar", last modified: Mon Apr 15 02:22:40 2024, max compression
+gzip compressed data, was "vtjson-1.7.5.tar", last modified: Thu Apr 18 03:17:02 2024, max compression
```

## Comparing `vtjson-1.7.4.tar` & `vtjson-1.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:40.542594 vtjson-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 02:22:36.000000 vtjson-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19323 2024-04-15 02:22:40.542594 vtjson-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-04-15 02:22:36.000000 vtjson-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 02:22:36.000000 vtjson-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:22:40.542594 vtjson-1.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:40.542594 vtjson-1.7.4/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19323 2024-04-15 02:22:40.000000 vtjson-1.7.4/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 02:22:40.000000 vtjson-1.7.4/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:22:40.000000 vtjson-1.7.4/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 02:22:40.000000 vtjson-1.7.4/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 02:22:40.000000 vtjson-1.7.4/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28578 2024-04-15 02:22:36.000000 vtjson-1.7.4/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:17:02.303800 vtjson-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 03:16:58.000000 vtjson-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-18 03:17:02.303800 vtjson-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-18 03:16:58.000000 vtjson-1.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-18 03:16:58.000000 vtjson-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:17:02.303800 vtjson-1.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:17:02.303800 vtjson-1.7.5/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-18 03:17:02.000000 vtjson-1.7.5/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 03:17:02.000000 vtjson-1.7.5/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:17:02.000000 vtjson-1.7.5/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 03:17:02.000000 vtjson-1.7.5/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 03:17:02.000000 vtjson-1.7.5/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-04-18 03:16:58.000000 vtjson-1.7.5/vtjson.py
```

### Comparing `vtjson-1.7.4/LICENSE` & `vtjson-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.4/PKG-INFO` & `vtjson-1.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.4
+Version: 1.7.5
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -243,14 +243,15 @@
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
```

### Comparing `vtjson-1.7.4/README.md` & `vtjson-1.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
```

### Comparing `vtjson-1.7.4/pyproject.toml` & `vtjson-1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.7.4/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.5/vtjson.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.7.4
+Version: 1.7.5
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -243,14 +243,15 @@
 - `one_of(key1, ..., keyN)`. This represents a dictionary with exactly one key among `key1, ..., keyN`.
 - `at_least_one_of(key1, ..., keyN)`. This represents a dictionary with a least one key among `key1, ..., keyN`.
 - `at_most_one_of(key1, ..., keyN)`. This represents an dictionary with at most one key among `key1, ..., keyN`.
 - `keys(key1, ..., keyN)`. This represents a dictionary containing all the keys in `key1, ..., keyN`.
 - `interval(lowerbound, upperbound)`. This checks if `lowerbound <= object <= upperbound`, provided the comparisons make sense. An upper/lowerbound `...` (ellipsis) means that the
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
+- `fields({field1: schema1, field2: schema2, ..., fieldN: schemaN})`. Matches Python objects with attributes `field1, field2, ..., fieldN` whose corresponding values should validate against `schema1, schema2, ..., schemaN` respectively.
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
 ## Pre-compiling a schema
 An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles a schema before performing a validation against it, so pre-compiling is not necessary but it gains a bit of performance as it needs to be done only once. Compiling is an idempotent operation. It does nothing for an already compiled schema.
```

### Comparing `vtjson-1.7.4/vtjson.py` & `vtjson-1.7.5/vtjson.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.7.4"
+__version__ = "1.7.5"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -759,14 +759,41 @@
                 raise SchemaError(f"{repr(c)} is not a tuple of length two")
         self.args = args
 
     def __compile__(self, _deferred_compiles=None):
         return _cond(self.args, _deferred_compiles=_deferred_compiles)
 
 
+class _fields:
+    def __init__(self, d, _deferred_compiles=None):
+        self.d = {}
+        for k, v in d.items():
+            self.d[k] = compile(v, _deferred_compiles=_deferred_compiles)
+
+    def __validate__(self, object, name, strict):
+        for k, v in self.d.items():
+            name_ = f"{name}.{k}"
+            if not hasattr(object, k):
+                return f"{name_} is missing"
+            ret = self.d[k].__validate__(getattr(object, k), name=name_, strict=strict)
+            if ret != "":
+                return ret
+        return ""
+
+
+class fields:
+    def __init__(self, d):
+        if not isinstance(d, dict):
+            raise SchemaError(f"{repr(d)} is not a dictionary")
+        self.d = d
+
+    def __compile__(self, _deferred_compiles=None):
+        return _fields(self.d, _deferred_compiles=_deferred_compiles)
+
+
 class _dict:
     def __init__(self, schema, _deferred_compiles=None):
         self.schema = collections.OrderedDict()
         for k, v in schema.items():
             self.schema[k] = compile(v, _deferred_compiles=_deferred_compiles)
         self.keys = _keys(self.schema)
         self.keys2 = _keys2(self.schema)
```

