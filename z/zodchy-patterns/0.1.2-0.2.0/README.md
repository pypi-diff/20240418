# Comparing `tmp/zodchy_patterns-0.1.2.tar.gz` & `tmp/zodchy_patterns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_patterns-0.1.2.tar", max compression
+gzip compressed data, was "zodchy_patterns-0.2.0.tar", max compression
```

## Comparing `zodchy_patterns-0.1.2.tar` & `zodchy_patterns-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.1.2/README.md
--rw-r--r--   0        0        0      435 2024-04-15 10:23:42.273056 zodchy_patterns-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      205 2024-04-11 07:57:07.720094 zodchy_patterns-0.1.2/zodchy_patterns/__init__.py
--rw-r--r--   0        0        0      172 2024-04-11 07:57:07.720291 zodchy_patterns-0.1.2/zodchy_patterns/events/__init__.py
--rw-r--r--   0        0        0     1470 2024-04-13 13:25:25.515788 zodchy_patterns-0.1.2/zodchy_patterns/events/http.py
--rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.1.2/zodchy_patterns/mapping.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.2.0/README.md
+-rw-r--r--   0        0        0      435 2024-04-18 15:44:02.099131 zodchy_patterns-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-18 15:44:02.094165 zodchy_patterns-0.2.0/zodchy_patterns/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-18 15:44:02.102702 zodchy_patterns-0.2.0/zodchy_patterns/events/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:27:46.945461 zodchy_patterns-0.2.0/zodchy_patterns/events/io/__init__.py
+-rw-r--r--   0        0        0     1771 2024-04-18 15:44:02.106121 zodchy_patterns-0.2.0/zodchy_patterns/events/io/error.py
+-rw-r--r--   0        0        0      314 2024-04-18 15:44:02.089184 zodchy_patterns-0.2.0/zodchy_patterns/events/io/generic.py
+-rw-r--r--   0        0        0     1095 2024-04-18 15:44:02.083540 zodchy_patterns-0.2.0/zodchy_patterns/events/io/info.py
+-rw-r--r--   0        0        0      499 2024-04-11 07:57:07.720475 zodchy_patterns-0.2.0/zodchy_patterns/mapping.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.2.0/PKG-INFO
```

### Comparing `zodchy_patterns-0.1.2/zodchy_patterns/events/http.py` & `zodchy_patterns-0.2.0/zodchy_patterns/events/io/error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,78 @@
-import collections.abc
+import re
 import dataclasses
 from zodchy import codex
 
+from . import generic
+
 
 @dataclasses.dataclass
-class HTTPResponseEvent(codex.ResponseEvent):
+class HttpError(generic.HttpEvent, codex.Error):
+    code: int = 500
+    message: str | None = None
+    details: dict | None = None
+
     def get_content(self) -> dict:
-        data = dataclasses.asdict(self)
+        details = self.details or {}
+        for field in dataclasses.fields(self):
+            if field.name not in ('code', 'message', 'details'):
+                details[field.name] = getattr(self, field.name)
         return {
-            'data': data or None
+            'data': {
+                'code': self.code,
+                'message': self._get_message(),
+                'details': details or None
+            }
         }
 
     def get_status_code(self) -> int:
-        return 200
+        return self.code
+
+    def _get_message(self):
+        if self.message is None:
+            matches = re.finditer(
+                '.+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)',
+                type(self).__name__
+            )
+            return " ".join((_[0] for _ in matches))
+        return self.message
 
 
 @dataclasses.dataclass
-class ErrorResponseEvent(HTTPResponseEvent):
+class HttpClientError(HttpError):
+    code: int = 400
+
     def get_status_code(self) -> int:
-        return 500
+        return self.code
 
 
 @dataclasses.dataclass
-class CreatedResponseEvent(HTTPResponseEvent):
-    def get_content(self) -> dict:
-        data = dataclasses.asdict(self)
-        return {'data': data} if data else None
-
-    def get_status_code(self):
-        return 200 if self.get_content() else 201
+class HttpAuthError(HttpClientError):
+    code: int = 403
 
 
 @dataclasses.dataclass
-class ItemResponseEvent(HTTPResponseEvent):
-    data: collections.abc.Mapping
+class HttpRateLimitError(HttpClientError):
+    code: int = 429
 
-    def get_content(self):
-        return {'data': self.data} if self.data else None
 
-    def get_status_code(self):
-        return 200 if self.data else 404
+@dataclasses.dataclass
+class HttpValidationError(HttpClientError):
+    code: int = 422
 
 
 @dataclasses.dataclass
-class ListResponseEvent(HTTPResponseEvent):
-    data: collections.abc.Iterable[collections.abc.Mapping]
+class HttpNotFoundError(HttpClientError):
+    code: int = 404
 
-    def get_content(self):
-        return {
-            'data': self.data or []
-        }
+
+@dataclasses.dataclass
+class HttpDuplicationError(HttpClientError):
+    code: int = 409
 
 
 @dataclasses.dataclass
-class PaginatedListResponseEvent(ListResponseEvent):
-    total: int
+class HttpEmptyRosterError(HttpClientError):
+    code: int = 200
 
-    def get_content(self):
-        return super().get_content() | {
-            'pagination': {
-                'quantity': self.total
-            }
-        }
+    def get_content(self) -> dict:
+        return {'data': []}
```

### Comparing `zodchy_patterns-0.1.2/PKG-INFO` & `zodchy_patterns-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodchy-patterns
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of patterns to use in CQRS applications
 Home-page: https://github.com/smairon/zodchy-patterns
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

