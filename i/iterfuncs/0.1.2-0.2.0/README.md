# Comparing `tmp/iterfuncs-0.1.2.tar.gz` & `tmp/iterfuncs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterfuncs-0.1.2.tar", last modified: Mon Mar 25 15:29:51 2024, max compression
+gzip compressed data, was "iterfuncs-0.2.0.tar", last modified: Thu Apr 18 06:01:01 2024, max compression
```

## Comparing `iterfuncs-0.1.2.tar` & `iterfuncs-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-03-25 15:29:51.192983 iterfuncs-0.1.2/
--rw-r--r--   0 liava    (60327) liava    (60327)     1070 2024-03-13 13:40:00.000000 iterfuncs-0.1.2/LICENSE
--rw-r--r--   0 liava    (60327) liava    (60327)       25 2024-03-13 13:40:00.000000 iterfuncs-0.1.2/MANIFEST.in
--rw-r--r--   0 liava    (60327) liava    (60327)     1095 2024-03-25 15:29:51.191983 iterfuncs-0.1.2/PKG-INFO
--rw-r--r--   0 liava    (60327) liava    (60327)      696 2024-03-25 14:39:51.000000 iterfuncs-0.1.2/README.md
-drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-03-25 15:29:51.191983 iterfuncs-0.1.2/iterfuncs/
--rw-r--r--   0 liava    (60327) liava    (60327)        0 2024-03-13 13:40:00.000000 iterfuncs-0.1.2/iterfuncs/__init__.py
--rw-r--r--   0 liava    (60327) liava    (60327)     1650 2024-03-25 14:33:38.000000 iterfuncs-0.1.2/iterfuncs/asyncio.py
--rw-r--r--   0 liava    (60327) liava    (60327)     4940 2024-03-25 15:29:17.000000 iterfuncs-0.1.2/iterfuncs/cache.py
--rw-r--r--   0 liava    (60327) liava    (60327)     4478 2024-03-25 14:30:03.000000 iterfuncs-0.1.2/iterfuncs/itertools.py
--rw-r--r--   0 liava    (60327) liava    (60327)      187 2024-03-25 14:33:37.000000 iterfuncs-0.1.2/iterfuncs/typing.py
-drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-03-25 15:29:51.191983 iterfuncs-0.1.2/iterfuncs.egg-info/
--rw-r--r--   0 liava    (60327) liava    (60327)     1095 2024-03-25 15:29:51.000000 iterfuncs-0.1.2/iterfuncs.egg-info/PKG-INFO
--rw-r--r--   0 liava    (60327) liava    (60327)      307 2024-03-25 15:29:51.000000 iterfuncs-0.1.2/iterfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 liava    (60327) liava    (60327)        1 2024-03-25 15:29:51.000000 iterfuncs-0.1.2/iterfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 liava    (60327) liava    (60327)       10 2024-03-25 15:29:51.000000 iterfuncs-0.1.2/iterfuncs.egg-info/top_level.txt
--rw-r--r--   0 liava    (60327) liava    (60327)       87 2024-03-13 13:40:00.000000 iterfuncs-0.1.2/pyproject.toml
--rw-r--r--   0 liava    (60327) liava    (60327)        0 2024-03-13 13:42:32.000000 iterfuncs-0.1.2/requirements.txt
--rw-r--r--   0 liava    (60327) liava    (60327)       38 2024-03-25 15:29:51.192983 iterfuncs-0.1.2/setup.cfg
--rw-r--r--   0 liava    (60327) liava    (60327)      930 2024-03-25 15:29:33.000000 iterfuncs-0.1.2/setup.py
+drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-04-18 06:01:01.979403 iterfuncs-0.2.0/
+-rw-r--r--   0 liava    (60327) liava    (60327)     1070 2024-03-13 13:40:00.000000 iterfuncs-0.2.0/LICENSE
+-rw-r--r--   0 liava    (60327) liava    (60327)       25 2024-03-13 13:40:00.000000 iterfuncs-0.2.0/MANIFEST.in
+-rw-r--r--   0 liava    (60327) liava    (60327)     1095 2024-04-18 06:01:01.978403 iterfuncs-0.2.0/PKG-INFO
+-rw-r--r--   0 liava    (60327) liava    (60327)      696 2024-03-25 14:39:51.000000 iterfuncs-0.2.0/README.md
+drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-04-18 06:01:01.976403 iterfuncs-0.2.0/iterfuncs/
+-rw-r--r--   0 liava    (60327) liava    (60327)        0 2024-03-13 13:40:00.000000 iterfuncs-0.2.0/iterfuncs/__init__.py
+-rw-r--r--   0 liava    (60327) liava    (60327)     1650 2024-03-25 14:33:38.000000 iterfuncs-0.2.0/iterfuncs/asyncio.py
+-rw-r--r--   0 liava    (60327) liava    (60327)     6329 2024-04-18 05:58:43.000000 iterfuncs-0.2.0/iterfuncs/cache.py
+-rw-r--r--   0 liava    (60327) liava    (60327)     4478 2024-03-25 14:30:03.000000 iterfuncs-0.2.0/iterfuncs/itertools.py
+-rw-r--r--   0 liava    (60327) liava    (60327)      225 2024-04-18 05:46:08.000000 iterfuncs-0.2.0/iterfuncs/typing.py
+drwxr-xr-x   0 liava    (60327) liava    (60327)        0 2024-04-18 06:01:01.977403 iterfuncs-0.2.0/iterfuncs.egg-info/
+-rw-r--r--   0 liava    (60327) liava    (60327)     1095 2024-04-18 06:01:01.000000 iterfuncs-0.2.0/iterfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 liava    (60327) liava    (60327)      307 2024-04-18 06:01:01.000000 iterfuncs-0.2.0/iterfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 liava    (60327) liava    (60327)        1 2024-04-18 06:01:01.000000 iterfuncs-0.2.0/iterfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 liava    (60327) liava    (60327)       10 2024-04-18 06:01:01.000000 iterfuncs-0.2.0/iterfuncs.egg-info/top_level.txt
+-rw-r--r--   0 liava    (60327) liava    (60327)       87 2024-03-13 13:40:00.000000 iterfuncs-0.2.0/pyproject.toml
+-rw-r--r--   0 liava    (60327) liava    (60327)        0 2024-03-13 13:42:32.000000 iterfuncs-0.2.0/requirements.txt
+-rw-r--r--   0 liava    (60327) liava    (60327)       38 2024-04-18 06:01:01.979403 iterfuncs-0.2.0/setup.cfg
+-rw-r--r--   0 liava    (60327) liava    (60327)      930 2024-04-18 05:58:35.000000 iterfuncs-0.2.0/setup.py
```

### Comparing `iterfuncs-0.1.2/LICENSE` & `iterfuncs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iterfuncs-0.1.2/PKG-INFO` & `iterfuncs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterfuncs
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of iteration, caching and async tools
 Home-page: https://github.com/Quartz-Vision/python-iterfuncs
 Author: liava
 Author-email: liava@tuta.io
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `iterfuncs-0.1.2/README.md` & `iterfuncs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `iterfuncs-0.1.2/iterfuncs/asyncio.py` & `iterfuncs-0.2.0/iterfuncs/asyncio.py`

 * *Files identical despite different names*

### Comparing `iterfuncs-0.1.2/iterfuncs/cache.py` & `iterfuncs-0.2.0/iterfuncs/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import weakref
-from collections.abc import Awaitable
-from functools import lru_cache as _lru_cache
 from functools import wraps
 from time import time
 from typing import Any, Callable
 
-from iterfuncs.typing import DecoratorFactoryT, IdT, MethodT
+from iterfuncs.typing import AbsDecoratorFT, IdT
 
 
 def make_hash(*args, **kwargs):
     """
     Generates hash from args and kwargs.
     """
     return hash(
@@ -55,69 +53,78 @@
                 del cache[item]
 
             tmp = func(*args, **kwargs)
             cache[cache_key] = tmp
 
             return tmp
 
+        def delete(*args: P.args, **kwargs: P.kwargs):
+            cache_key = key(*args, **kwargs)
+            if cache_key in cache:
+                del cache[cache_key]
+
+        setattr(wrapper, "delete", delete)
+
         return wrapper
 
     return ttl_decorator
 
 
+def copy_cache_methods(source, target):
+    cache_methods = ["delete"]
+    for method_name in cache_methods:
+        setattr(target, method_name, getattr(source, method_name, lambda *_, **__: None))
+
+
 def async_cache_adapter[
-    **P, **DP, DT
-](
-    cache_decorator_factory: DecoratorFactoryT[
-        P, Callable[DP, Callable[[], Awaitable[DT]]]
-    ]
-) -> DecoratorFactoryT[P, Callable[DP, Awaitable[DT]]]:
+    **P
+](cache_decorator_factory: AbsDecoratorFT[P]) -> AbsDecoratorFT[P]:
     """
     Should be used only for async functions. Every time it will return a !new! coroutine that returns cached value,
         so it should not be used inside other adapters that provide additional cache capabilities.
 
     Example:
         ```
         @async_cache_adapter(ttl_cache)(ttl=3600)
         async def f(x):
             return x
         ```
     """
     nothing = object()
 
     def transformed_decorator_factory(*d_args: P.args, **d_kwargs: P.kwargs):
-        def decorator(func: Callable[DP, Awaitable]):
+        def decorator(func):
             @cache_decorator_factory(*d_args, **d_kwargs)
             def update_coro(*args, **kwargs):
                 data: Any = nothing
 
-                async def get_coro() -> DT:
+                async def get_coro():
                     nonlocal data
                     if data is nothing:
                         data = await func(*args, **kwargs)
                     return data
 
                 return get_coro
 
             @wraps(func)
-            async def wrapped_func(*args: DP.args, **kwargs: DP.kwargs):
+            async def wrapped_func(*args, **kwargs):
                 return await update_coro(*args, **kwargs)()
 
+            copy_cache_methods(update_coro, wrapped_func)
+
             return wrapped_func
 
         return decorator
 
     return transformed_decorator_factory
 
 
 def method_cache_adapter[
-    **P, **DP, DT
-](cache_decorator_factory: DecoratorFactoryT[P, MethodT[DP, DT]]) -> DecoratorFactoryT[
-    P, MethodT[DP, DT]
-]:
+    **P
+](cache_decorator_factory: AbsDecoratorFT[P]) -> AbsDecoratorFT[P]:
     """
     Should be used only for instance methods and be the top level adapter (wrap all other adapters),
     so it can prevent them from handling `self`
 
     Example:
         ```
         class A:
@@ -129,37 +136,79 @@
             @method_cache_adapter(async_cache_adapter(ttl_cache))(ttl=3600)
             async def f(self, x):
                 return x
         ```
     """
 
     def transformed_decorator_factory(*d_args: P.args, **d_kwargs: P.kwargs):
-        def decorator(func: MethodT[DP, DT]):
+        def decorator(func):
             @wraps(func)
-            def wrapped_method(self, *args: DP.args, **kwargs: DP.kwargs) -> DT:
+            def wrapped_method(self, *args, **kwargs):
                 # If we had a strong reference to self the instance would never die
                 self_weak = weakref.ref(self)
 
-                @wraps(func)
                 @cache_decorator_factory(*d_args, **d_kwargs)
-                def cached_method(_, *args, **kwargs):
+                def cached_method(*args, **kwargs):
                     return func(self_weak(), *args, **kwargs)
 
+                wrapped_cached_method = wraps(func)(cached_method)
+                copy_cache_methods(cached_method, wrapped_cached_method)
+
                 # Replace the method with the cached one, so it
                 # will be called next time without cache initialization
-                setattr(self, func.__name__, cached_method)
+                setattr(self, func.__name__, wrapped_cached_method)
+
+                return wrapped_cached_method(*args, **kwargs)
 
-                return cached_method(None, *args, **kwargs)
+            copy_cache_methods(None, wrapped_method)
 
             return wrapped_method
 
         return decorator
 
     return transformed_decorator_factory
 
 
-def amethod_cache_adapter(cache_decorator_factory):
+def amethod_cache_adapter[
+    **P
+](cache_decorator_factory: AbsDecoratorFT[P]) -> AbsDecoratorFT[P]:
     return method_cache_adapter(async_cache_adapter(cache_decorator_factory))
 
 
-def lru_cache(maxsize: int) -> IdT:
-    return _lru_cache(maxsize)
+def lru_cache[**P, T](size: int = -1, key: Callable[..., int] = make_hash) -> IdT:
+    """
+    Creates a function with size-limited cache.
+
+    :param key: function that generates cache key. By default, it uses make_hash
+    :param size: maximum number of items in cache. If -1, cache is unlimited
+    """
+
+    def ttl_decorator(func: Callable[P, T]) -> Callable[P, T]:
+        cache = {}
+
+        @wraps(func)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+            nonlocal cache
+
+            cache_key = key(*args, **kwargs)
+            if cache_key in cache:
+                return cache[cache_key]
+
+            if size > 0 and len(cache) >= size:
+                item = next(iter(cache))
+                del cache[item]
+
+            tmp = func(*args, **kwargs)
+            cache[cache_key] = tmp
+
+            return tmp
+
+        def delete(*args: P.args, **kwargs: P.kwargs):
+            cache_key = key(*args, **kwargs)
+            if cache_key in cache:
+                del cache[cache_key]
+
+        setattr(wrapper, "delete", delete)
+
+        return wrapper
+
+    return ttl_decorator
```

### Comparing `iterfuncs-0.1.2/iterfuncs/itertools.py` & `iterfuncs-0.2.0/iterfuncs/itertools.py`

 * *Files identical despite different names*

### Comparing `iterfuncs-0.1.2/iterfuncs.egg-info/PKG-INFO` & `iterfuncs-0.2.0/iterfuncs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterfuncs
-Version: 0.1.2
+Version: 0.2.0
 Summary: Collection of iteration, caching and async tools
 Home-page: https://github.com/Quartz-Vision/python-iterfuncs
 Author: liava
 Author-email: liava@tuta.io
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `iterfuncs-0.1.2/setup.py` & `iterfuncs-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open(ROOT / "requirements.txt") as fr:
     reqs = fr.read().strip().split("\n")
 
 
 setuptools.setup(
     name="iterfuncs",
-    version="0.1.2",
+    version="0.2.0",
     author="liava",
     author_email="liava@tuta.io",
     description="Collection of iteration, caching and async tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Quartz-Vision/python-iterfuncs",
     packages=setuptools.find_packages(),
```

