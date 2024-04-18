# Comparing `tmp/strawberry_persisted_queries-1.0.3.tar.gz` & `tmp/strawberry_persisted_queries-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_persisted_queries-1.0.3.tar", max compression
+gzip compressed data, was "strawberry_persisted_queries-1.1.0.tar", max compression
```

## Comparing `strawberry_persisted_queries-1.0.3.tar` & `strawberry_persisted_queries-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/LICENSE
--rw-r--r--   0        0        0     1120 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/README.md
--rw-r--r--   0        0        0      729 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      162 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/__init__.py
--rw-r--r--   0        0        0      216 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/cache.py
--rw-r--r--   0        0        0       84 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/django_cache/__init__.py
--rw-r--r--   0        0        0      354 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/django_cache/cache.py
--rw-r--r--   0        0        0     3244 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/extension.py
--rw-r--r--   0        0        0       64 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/safelisting/__init__.py
--rw-r--r--   0        0        0      298 2024-03-04 17:14:48.164866 strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/safelisting/dict.py
--rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 strawberry_persisted_queries-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1873 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/README.md
+-rw-r--r--   0        0        0      714 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/cache.py
+-rw-r--r--   0        0        0       84 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/django_cache/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/django_cache/cache.py
+-rw-r--r--   0        0        0     3244 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/extension.py
+-rw-r--r--   0        0        0       64 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/safelisting/__init__.py
+-rw-r--r--   0        0        0      298 2024-04-18 06:11:08.991186 strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/safelisting/dict.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 strawberry_persisted_queries-1.1.0/PKG-INFO
```

### Comparing `strawberry_persisted_queries-1.0.3/LICENSE` & `strawberry_persisted_queries-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_persisted_queries-1.0.3/README.md` & `strawberry_persisted_queries-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # 🍓Strawberry Persisted Queries
 
 [![PyPI](https://img.shields.io/pypi/v/strawberry_persisted_queries?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/strawberry_persisted_queries/)
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/catgirlinspace?style=for-the-badge&logo=githubsponsors)](https://github.com/sponsors/catgirlinspace)
 
 Apollo-compatible persisted queries for Strawberry. 
 
 ## Usage
 
-Add `PersistedQueriesExtension` to your extensions.
+Add `PersistedQueriesExtension()` to your extensions.
 
 ```python
 import strawberry
 from strawberry_persisted_queries import PersistedQueriesExtension
 
 schema = strawberry.Schema(
     query=Query,
@@ -18,26 +19,44 @@
         PersistedQueriesExtension(),
     ],
 )
 ```
 
 ### Django
 
-For Django, a Django cache backend is available.
+For Django users, a Django cache backend is available. This uses the default cache set in Django. 
 ```python
 from strawberry_persisted_queries.django_cache import DjangoPersistedQueryCache
 
 PersistedQueriesExtension(cache_backend=DjangoPersistedQueryCache())
 ```
 
 ### Safelisted Queries
 
 `DictSafelist` can be used to require persisted queries to already be saved.
-This can be used with a build tool to ensure only queries used by your app are available.
+This can be used with a build tool to ensure only queries used within an app are available.
 
 ```python
 from strawberry_persisted_queries.safelisting import DictSafelist
 
 PersistedQueriesExtension(safelist=DictSafelist({
     'sha256Hash': 'query {...}',
 }))
-```
+```
+
+## Custom Cache Backends
+
+Custom cache backends allow using another cache for persisted queries, such as memcached or a database.
+Custom cache backends can inherit from `strawberry_persisted_queries.PersistedQueryCache`. 
+
+```python
+from strawberry_persisted_queries.cache import PersistedQueryCache
+
+class MyCache(PersistedQueryCache):
+    def get(self, query_hash):
+        return cache.get(query_hash)
+
+    def set(self, query_hash, value):
+        cache.set(query_hash, value)
+
+PersistedQueriesExtension(cache_backend=MyCache())
+```
```

### Comparing `strawberry_persisted_queries-1.0.3/strawberry_persisted_queries/extension.py` & `strawberry_persisted_queries-1.1.0/strawberry_persisted_queries/extension.py`

 * *Files identical despite different names*

### Comparing `strawberry_persisted_queries-1.0.3/PKG-INFO` & `strawberry_persisted_queries-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: strawberry_persisted_queries
-Version: 1.0.3
+Version: 1.1.0
 Summary: Apollo-compatible persisted queries for Strawberry
 Home-page: https://github.com/catgirlinspace/strawberry_persisted_queries.git
 License: MIT
 Author: Rosalina
 Author-email: catgirl@catgirlin.space
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: django
 Requires-Dist: django (>=5.0.3,<6.0.0) ; extra == "django"
-Requires-Dist: strawberry-graphql (==0.220.0.dev.1709543239)
+Requires-Dist: strawberry-graphql (>=0.226)
 Project-URL: Repository, https://github.com/catgirlinspace/strawberry_persisted_queries.git
 Description-Content-Type: text/markdown
 
 # 🍓Strawberry Persisted Queries
 
 [![PyPI](https://img.shields.io/pypi/v/strawberry_persisted_queries?logo=pypi&logoColor=white&style=for-the-badge)](https://pypi.org/project/strawberry_persisted_queries/)
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/catgirlinspace?style=for-the-badge&logo=githubsponsors)](https://github.com/sponsors/catgirlinspace)
 
 Apollo-compatible persisted queries for Strawberry. 
 
 ## Usage
 
-Add `PersistedQueriesExtension` to your extensions.
+Add `PersistedQueriesExtension()` to your extensions.
 
 ```python
 import strawberry
 from strawberry_persisted_queries import PersistedQueriesExtension
 
 schema = strawberry.Schema(
     query=Query,
@@ -39,26 +40,45 @@
         PersistedQueriesExtension(),
     ],
 )
 ```
 
 ### Django
 
-For Django, a Django cache backend is available.
+For Django users, a Django cache backend is available. This uses the default cache set in Django. 
 ```python
 from strawberry_persisted_queries.django_cache import DjangoPersistedQueryCache
 
 PersistedQueriesExtension(cache_backend=DjangoPersistedQueryCache())
 ```
 
 ### Safelisted Queries
 
 `DictSafelist` can be used to require persisted queries to already be saved.
-This can be used with a build tool to ensure only queries used by your app are available.
+This can be used with a build tool to ensure only queries used within an app are available.
 
 ```python
 from strawberry_persisted_queries.safelisting import DictSafelist
 
 PersistedQueriesExtension(safelist=DictSafelist({
     'sha256Hash': 'query {...}',
 }))
 ```
+
+## Custom Cache Backends
+
+Custom cache backends allow using another cache for persisted queries, such as memcached or a database.
+Custom cache backends can inherit from `strawberry_persisted_queries.PersistedQueryCache`. 
+
+```python
+from strawberry_persisted_queries.cache import PersistedQueryCache
+
+class MyCache(PersistedQueryCache):
+    def get(self, query_hash):
+        return cache.get(query_hash)
+
+    def set(self, query_hash, value):
+        cache.set(query_hash, value)
+
+PersistedQueriesExtension(cache_backend=MyCache())
+```
+
```

