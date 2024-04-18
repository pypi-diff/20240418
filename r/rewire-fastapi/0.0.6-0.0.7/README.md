# Comparing `tmp/rewire_fastapi-0.0.6.tar.gz` & `tmp/rewire_fastapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire_fastapi-0.0.6.tar", last modified: Wed Apr 17 06:41:50 2024, max compression
+gzip compressed data, was "rewire_fastapi-0.0.7.tar", last modified: Thu Apr 18 09:32:32 2024, max compression
```

## Comparing `rewire_fastapi-0.0.6.tar` & `rewire_fastapi-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.320377 rewire_fastapi-0.0.6/
--rw-rw-rw-   0        0        0     1086 2024-02-01 21:35:51.000000 rewire_fastapi-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3403 2024-04-17 06:41:50.319377 rewire_fastapi-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1498 2024-02-01 22:53:53.000000 rewire_fastapi-0.0.6/README.md
--rw-rw-rw-   0        0        0      734 2024-04-17 06:41:39.000000 rewire_fastapi-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.303847 rewire_fastapi-0.0.6/rewire_fastapi/
--rw-rw-rw-   0        0        0     6299 2024-04-17 06:41:30.000000 rewire_fastapi-0.0.6/rewire_fastapi/__init__.py
--rw-rw-rw-   0        0        0     1646 2024-01-24 06:53:30.000000 rewire_fastapi-0.0.6/rewire_fastapi/dependable.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:41:50.319377 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/
--rw-rw-rw-   0        0        0     3403 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 06:41:50.000000 rewire_fastapi-0.0.6/rewire_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:41:50.321377 rewire_fastapi-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:32.796410 rewire_fastapi-0.0.7/
+-rw-rw-rw-   0        0        0     1086 2024-02-01 21:35:51.000000 rewire_fastapi-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3403 2024-04-18 09:32:32.794906 rewire_fastapi-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2024-02-01 22:53:53.000000 rewire_fastapi-0.0.7/README.md
+-rw-rw-rw-   0        0        0      734 2024-04-18 09:32:19.000000 rewire_fastapi-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:32.777903 rewire_fastapi-0.0.7/rewire_fastapi/
+-rw-rw-rw-   0        0        0     6299 2024-04-17 06:41:30.000000 rewire_fastapi-0.0.7/rewire_fastapi/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-04-18 09:32:14.000000 rewire_fastapi-0.0.7/rewire_fastapi/dependable.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:32:32.793906 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/
+-rw-rw-rw-   0        0        0     3403 2024-04-18 09:32:32.000000 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-18 09:32:32.000000 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:32:32.000000 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-18 09:32:32.000000 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-18 09:32:32.000000 rewire_fastapi-0.0.7/rewire_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 09:32:32.796410 rewire_fastapi-0.0.7/setup.cfg
```

### Comparing `rewire_fastapi-0.0.6/LICENSE` & `rewire_fastapi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.6/PKG-INFO` & `rewire_fastapi-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire_fastapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fastapi integration for rewire
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire_fastapi-0.0.6/README.md` & `rewire_fastapi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.6/pyproject.toml` & `rewire_fastapi-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire_fastapi"
-version = "0.0.6"
+version = "0.0.7"
 description = "Fastapi integration for rewire"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire_fastapi-0.0.6/rewire_fastapi/__init__.py` & `rewire_fastapi-0.0.7/rewire_fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rewire_fastapi-0.0.6/rewire_fastapi/dependable.py` & `rewire_fastapi-0.0.7/rewire_fastapi/dependable.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         update_wrapper(self, callable)
         super().__init__(callable)
 
     def _return_type(self) -> Type[T]:
         ...
 
     @property
-    def Result(self):
+    def Result(self) -> Type[T]:
         type_ = self._return_type()
         return Annotated[type_, Depends(self.dependency)]
 
     def __call__(self, *args: P.args, **kwds: P.kwargs) -> R:
         assert self.dependency
         return self.dependency(*args, **kwds)
```

### Comparing `rewire_fastapi-0.0.6/rewire_fastapi.egg-info/PKG-INFO` & `rewire_fastapi-0.0.7/rewire_fastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire_fastapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fastapi integration for rewire
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

