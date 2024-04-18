# Comparing `tmp/ragdoll-0.3.0.tar.gz` & `tmp/ragdoll-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragdoll-0.3.0.tar", max compression
+gzip compressed data, was "ragdoll-0.4.0.tar", max compression
```

## Comparing `ragdoll-0.3.0.tar` & `ragdoll-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-08-28 04:54:56.732922 ragdoll-0.3.0/LICENSE.md
--rw-r--r--   0        0        0      562 2024-03-15 15:33:10.496101 ragdoll-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      168 2024-03-15 15:33:10.496373 ragdoll-0.3.0/ragdoll/__init__.py
--rw-r--r--   0        0        0     3147 2024-03-15 15:31:51.590550 ragdoll-0.3.0/ragdoll/base.py
--rw-r--r--   0        0        0      414 2024-02-21 23:40:32.949687 ragdoll-0.3.0/ragdoll/django.py
--rw-r--r--   0        0        0     1725 2024-03-15 15:31:51.591296 ragdoll-0.3.0/ragdoll/env.py
--rw-r--r--   0        0        0      162 2023-08-28 04:54:56.734598 ragdoll-0.3.0/ragdoll/errors.py
--rw-r--r--   0        0        0      147 2023-08-28 04:54:56.734736 ragdoll-0.3.0/ragdoll/utils.py
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 ragdoll-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-28 04:54:56.732922 ragdoll-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0      562 2024-04-18 11:44:34.905107 ragdoll-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2024-04-18 11:44:34.905364 ragdoll-0.4.0/ragdoll/__init__.py
+-rw-r--r--   0        0        0     3259 2024-04-18 11:44:26.558869 ragdoll-0.4.0/ragdoll/base.py
+-rw-r--r--   0        0        0      414 2024-02-21 23:40:32.949687 ragdoll-0.4.0/ragdoll/django.py
+-rw-r--r--   0        0        0     1725 2024-03-15 15:31:51.591296 ragdoll-0.4.0/ragdoll/env.py
+-rw-r--r--   0        0        0      162 2023-08-28 04:54:56.734598 ragdoll-0.4.0/ragdoll/errors.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 ragdoll-0.4.0/PKG-INFO
```

### Comparing `ragdoll-0.3.0/LICENSE.md` & `ragdoll-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragdoll-0.3.0/pyproject.toml` & `ragdoll-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragdoll"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Aaron Zhang <rabbit.aaron@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/rabbit-aaron/ragdoll"
 repository = "https://github.com/rabbit-aaron/ragdoll.git"
 
 [tool.poetry.dependencies]
```

### Comparing `ragdoll-0.3.0/ragdoll/base.py` & `ragdoll-0.4.0/ragdoll/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,23 @@
             ), f"`default_value` must be one of {choices!r}"
 
         self._choices = choices
         self.extra_kwargs = kwargs
 
     @property
     def _default(self) -> Any:
+        if callable(self._default_value):
+            value = self._default_value()
+        else:
+            value = self._default_value
+
         if self._process_default_value:
-            return self.to_python(self._default_value)
-        return self._default_value
+            return self.to_python(value)
+
+        return value
 
     @property
     def name(self):
         return self._name
 
     @abc.abstractmethod
     def to_python(self, value: Any) -> Any:  # pragma: no cover
```

### Comparing `ragdoll-0.3.0/ragdoll/env.py` & `ragdoll-0.4.0/ragdoll/env.py`

 * *Files identical despite different names*

### Comparing `ragdoll-0.3.0/PKG-INFO` & `ragdoll-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragdoll
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/rabbit-aaron/ragdoll
 License: MIT
 Author: Aaron Zhang
 Author-email: rabbit.aaron@gmail.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

