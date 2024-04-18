# Comparing `tmp/friendly_sequences-1.0.tar.gz` & `tmp/friendly_sequences-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "friendly_sequences-1.0.tar", last modified: Fri Apr 12 19:14:33 2024, max compression
+gzip compressed data, was "friendly_sequences-1.1.tar", last modified: Wed Apr 17 20:09:41 2024, max compression
```

## Comparing `friendly_sequences-1.0.tar` & `friendly_sequences-1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-12 19:14:12.930929 friendly_sequences-1.0/LICENSE
--rw-r--r--   0        0        0      362 2024-04-12 19:14:12.930929 friendly_sequences-1.0/README.md
--rw-r--r--   0        0        0     2588 2024-04-12 19:14:12.930929 friendly_sequences-1.0/friendly_sequences/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 19:14:12.930929 friendly_sequences-1.0/friendly_sequences/py.typed
--rw-r--r--   0        0        0     2550 2024-04-12 19:14:33.038882 friendly_sequences-1.0/pyproject.toml
--rw-r--r--   0        0        0     1188 2024-04-12 19:14:12.930929 friendly_sequences-1.0/tests/test_friendly_sequences.py
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 friendly_sequences-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 20:09:23.080026 friendly_sequences-1.1/LICENSE
+-rw-r--r--   0        0        0      546 2024-04-17 20:09:23.080026 friendly_sequences-1.1/README.md
+-rw-r--r--   0        0        0     2955 2024-04-17 20:09:23.080026 friendly_sequences-1.1/friendly_sequences/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:09:23.080026 friendly_sequences-1.1/friendly_sequences/py.typed
+-rw-r--r--   0        0        0     2550 2024-04-17 20:09:41.608182 friendly_sequences-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1141 2024-04-17 20:09:23.080026 friendly_sequences-1.1/tests/test_friendly_sequences.py
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 friendly_sequences-1.1/PKG-INFO
```

### Comparing `friendly_sequences-1.0/LICENSE` & `friendly_sequences-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `friendly_sequences-1.0/friendly_sequences/__init__.py` & `friendly_sequences-1.1/friendly_sequences/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 
 IterableType1 = PT.TypeVar("IterableType1")
 IterableType2 = PT.TypeVar("IterableType2")
 ReturnIterableType1 = PT.TypeVar("ReturnIterableType1")
 ReturnIterableType2 = PT.TypeVar("ReturnIterableType2")
 
 
-def to_iterable(el):
-    return iter(el) if hasattr(el, "__iter__") else iter((el,))
-
-
 @attrs.frozen(auto_attribs=True, slots=True)
 class Seq(Iterator, PT.Generic[IterableType1]):
-    some: Iterator[IterableType1] = attrs.field(converter=to_iterable)
+    some: Iterator[IterableType1] = attrs.field(
+        converter=lambda some: iter(some)
+    )
 
     def map(
         self,
         func: Callable[
             [IterableType1],
             ReturnIterableType1,
         ],
@@ -42,20 +40,25 @@
         return Seq(
             map(
                 func,
                 itertools.chain.from_iterable(self),
             )
         )
 
+    def flatten(
+        self,
+    ) -> "Seq[ReturnIterableType1]":
+        return Seq(itertools.chain.from_iterable(self))
+
     def filter(
         self, func: Callable[[IterableType1], bool]
     ) -> "Seq[IterableType1]":
         return Seq(filter(func, self))
 
-    def reduce(
+    def fold(
         self,
         func: Callable[
             [
                 ReturnIterableType1,
                 IterableType1,
             ],
             ReturnIterableType1,
@@ -64,14 +67,29 @@
     ) -> ReturnIterableType1:
         return functools.reduce(
             func,
             self,
             initial,
         )
 
+    def reduce(
+        self,
+        func: Callable[
+            [
+                ReturnIterableType1,
+                IterableType1,
+            ],
+            ReturnIterableType1,
+        ],
+    ) -> ReturnIterableType1:
+        return functools.reduce(
+            func,
+            self,
+        )
+
     def take(self, n: int = 1) -> "Seq[IterableType1]":
         return Seq(itertools.islice(self, n))
 
     def sort(
         self,
         *,
         key: None = None,
```

### Comparing `friendly_sequences-1.0/pyproject.toml` & `friendly_sequences-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 ]
 dependencies = [
     "pytest>=7.3.1",
     "attrs>=23.2.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "1.0"
+version = "1.1"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/friendly-sequences"
 
 [build-system]
 requires = [
     "pdm-backend",
```

