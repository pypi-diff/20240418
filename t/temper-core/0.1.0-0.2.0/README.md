# Comparing `tmp/temper_core-0.1.0.tar.gz` & `tmp/temper_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_core-0.1.0.tar", max compression
+gzip compressed data, was "temper_core-0.2.0.tar", max compression
```

## Comparing `temper_core-0.1.0.tar` & `temper_core-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      428 2024-02-08 21:05:30.832979 temper_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    35617 2024-02-08 21:05:30.835947 temper_core-0.1.0/temper_core/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 21:05:30.833989 temper_core-0.1.0/temper_core/py.typed
--rw-r--r--   0        0        0     1555 2024-02-08 21:05:30.836872 temper_core-0.1.0/temper_core/regex.py
--rw-r--r--   0        0        0     3552 2024-02-08 21:05:30.839361 temper_core-0.1.0/temper_core/testing.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      428 2024-04-18 16:39:36.792472 temper_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    36160 2024-04-18 16:39:36.792472 temper_core-0.2.0/temper_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 16:39:36.792472 temper_core-0.2.0/temper_core/py.typed
+-rw-r--r--   0        0        0     1555 2024-04-18 16:39:36.792472 temper_core-0.2.0/temper_core/regex.py
+-rw-r--r--   0        0        0     3552 2024-04-18 16:39:36.792472 temper_core-0.2.0/temper_core/testing.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 temper_core-0.2.0/setup.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.2.0/PKG-INFO
```

### Comparing `temper_core-0.1.0/temper_core/__init__.py` & `temper_core-0.2.0/temper_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Implementation of many of the connected methods in temper.
 """
 
+import sys
+import logging
 from abc import abstractmethod
-from json import loads
 from logging import getLogger, INFO
 from math import copysign, inf, isclose, isinf, isnan, nan
 from typing import (
     Union,
     Any,
     Callable,
     Iterable,
@@ -74,14 +75,23 @@
     "Temper semantics for printing."
     if isinstance(value, str):
         print(value)
     else:
         print(repr(value))
 
 
+def init_simple_logging():
+    "Log all at INFO or higher to stdout without decoration."
+    logging.basicConfig(
+        handlers=[logging.StreamHandler(stream=sys.stdout)],
+        level=INFO,
+        format="%(message)s",
+    )
+
+
 class LoggingConsole(TemperObject):
     """One class per file to log data to the console."""
 
     __slots__ = ("logger",)
 
     def __init__(self, name: str):
         self.logger = getLogger(name)
@@ -258,39 +268,47 @@
 def cast_by_test(val: T, predicate: Callable[[T], bool]) -> Any:
     "This cast validates that a temper function meets some predicate, e.g. callable."
     if not predicate(val):
         raise ValueError()
     return val
 
 
-class Nexter(object):
+def adapt_generator(generator):
     """
-    Construct a consumer function that calls next on an iterator
-    mimics the javascript generator interface.
+    May be applied as a decorator to turn a Generator into a turn function.
+    """
+    # TODO: need type info for generator and result.
+    return lambda *args: GeneratorToStepFunctionAdapter(generator(*args))
+
+
+class GeneratorToStepFunctionAdapter(object):
+    """
+    Construct a callable function that calls next on an iterator.
     """
 
     __slots__ = ("_iterator", "value", "done")
 
+    # TODO: need a type on iterable and _iterator.
     def __init__(self, iterable):
-        self._iterator = iter(iterable())
+        self._iterator = iter(iterable)
         self.value = None
         self.done = False
 
     def __call__(self):
         if not self.done:
             try:
                 self.value = next(self._iterator)
             except StopIteration as exc:
                 self.done = True
                 # TODO Retain original StopIteration? In what contexts used?
                 raise RuntimeError() from exc
             except Exception as exc:
                 self.done = True
                 raise exc
-        return self
+        return None
 
 
 class Label(BaseException):
     "A label enables labled breaks with reasonably readable python."
     __slots__ = ()
 
     def __enter__(self) -> "Label":
@@ -1088,53 +1106,62 @@
 def map_builder_remove(builder: dict[Key, Value], key: Key) -> Value:
     "Implements MapBuilder's remove, which deletes an entry in a MapBuilder."
     # TODO Inline?
     return builder.pop(key)
 
 
 def map_builder_set(builder: dict[Key, Value], key: Key, value: Value) -> None:
-    "Set's entry on a MapBuilder."
+    "Sets entry on a MapBuilder."
     builder[key] = value
 
 
 def mapped_has(mapped: Mapping[Key, Value], key: Key) -> bool:
     "Checks if a Mapped object has a Key key"
-    # This can't be inlined well because order (mapped -> key) is swapped for (key -> mapped).
-    # Which would be an issue if mapped and key were expressions with SideEffects.
+    # This can't be inlined well because order (mapped -> key) is swapped for
+    # (key -> mapped). Which would be an issue if mapped and key were
+    # expressions with SideEffects.
     return key in mapped
 
 
 def mapped_to_map(mapped: Mapping[Key, Value]) -> MappingProxyType[Key, Value]:
     "Converts a Mapped to a Map."
     return MappingProxyType(dict(mapped))
 
 
 def mapped_to_list(mapped: Mapping[Key, Value]) -> Sequence[Pair[Key, Value]]:
     "Implements .toList() for Mapping objects."
     return tuple(Pair(key, mapped[key]) for key in mapped.keys())
 
 
-def mapped_to_list_builder(mapped: Mapping[Key, Value]) -> MutableSequence[Pair[Key, Value]]:
+def mapped_to_list_builder(
+    mapped: Mapping[Key, Value]
+) -> MutableSequence[Pair[Key, Value]]:
     "Implements .toListBuilder() for Mapping objects."
     return list(Pair(key, mapped[key]) for key in mapped.keys())
 
 
-def mapped_to_list_with(mapped: Mapping[Key, Value], func: Callable[[Key, Value], T]) -> Sequence[T]:
+def mapped_to_list_with(
+    mapped: Mapping[Key, Value], func: Callable[[Key, Value], T]
+) -> Sequence[T]:
     "Implements .toListWith{...} for Mapping objects."
     return tuple(func(key, mapped[key]) for key in mapped.keys())
 
 
-def mapped_to_list_builder_with(mapped: Mapping[Key, Value], func: Callable[[Key, Value], T]) -> MutableSequence[T]:
+def mapped_to_list_builder_with(
+    mapped: Mapping[Key, Value], func: Callable[[Key, Value], T]
+) -> MutableSequence[T]:
     "Implements .toListBuilderWith{...} for Mapping objects."
     return list(func(key, mapped[key]) for key in mapped.keys())
 
 
-def mapped_for_each(mapped: Mapping[Key, Value], func: Callable[[Key, Value], None]) -> None:
+def mapped_for_each(
+    mapped: Mapping[Key, Value], func: Callable[[Key, Value], None]
+) -> None:
     "Implements .forEach {...} for Mapping objects."
-    for (key, value) in mapped.items():
+    for key, value in mapped.items():
         func(key, value)
 
 
 # Utility functions
 
 
 def _utf8_size(code_point: int) -> int:
```

### Comparing `temper_core-0.1.0/temper_core/regex.py` & `temper_core-0.2.0/temper_core/regex.py`

 * *Files identical despite different names*

### Comparing `temper_core-0.1.0/temper_core/testing.py` & `temper_core-0.2.0/temper_core/testing.py`

 * *Files identical despite different names*

