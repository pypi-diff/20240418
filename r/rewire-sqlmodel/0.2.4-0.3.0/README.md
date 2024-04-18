# Comparing `tmp/rewire_sqlmodel-0.2.4.tar.gz` & `tmp/rewire_sqlmodel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire_sqlmodel-0.2.4.tar", last modified: Wed Apr 17 17:45:37 2024, max compression
+gzip compressed data, was "rewire_sqlmodel-0.3.0.tar", last modified: Thu Apr 18 11:48:55 2024, max compression
```

## Comparing `rewire_sqlmodel-0.2.4.tar` & `rewire_sqlmodel-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.370274 rewire_sqlmodel-0.2.4/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-17 17:45:37.369277 rewire_sqlmodel-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.2.4/README.md
--rw-rw-rw-   0        0        0      812 2024-04-17 17:45:25.000000 rewire_sqlmodel-0.2.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.346250 rewire_sqlmodel-0.2.4/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    15870 2024-04-08 20:12:06.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.364764 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.366269 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.366269 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2521 2024-04-17 17:45:21.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.367274 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 17:45:37.370274 rewire_sqlmodel-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.636870 rewire_sqlmodel-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-18 11:48:55.635869 rewire_sqlmodel-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.3.0/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-18 11:48:40.000000 rewire_sqlmodel-0.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.617920 rewire_sqlmodel-0.3.0/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15242 2024-04-18 10:44:34.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.632870 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.632870 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.633871 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2521 2024-04-17 17:45:21.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:48:55.634869 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-18 11:48:55.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-18 11:48:55.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:48:55.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-18 11:48:55.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 11:48:55.000000 rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:48:55.636870 rewire_sqlmodel-0.3.0/setup.cfg
```

### Comparing `rewire_sqlmodel-0.2.4/LICENSE` & `rewire_sqlmodel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/PKG-INFO` & `rewire_sqlmodel-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.4
+Version: 0.3.0
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire_sqlmodel-0.2.4/pyproject.toml` & `rewire_sqlmodel-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.2.4"
+version = "0.3.0"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/__init__.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,18 +221,21 @@
 
 session_context = Context[AsyncSession]()
 
 
 class ContextSession:
     ctx = CTX()
     session: AsyncSession | None = None
+    lock: anyio.Lock | None = None
     commit_hooks: list[Callable[[], Awaitable]]
     rollback_hooks: list[Callable[[], Awaitable]]
 
     async def __aenter__(self):
+        if PluginConfig.parallel is not False:
+            self.lock = await tx_lock.__aenter__()
         if (root := self.ctx.get(None)) is not None:
             self.context = None
             return root
         if self.session is not None:
             self.context = session_context.use(self.session)
             self.context.__enter__()
             self.self_context = self.ctx.use()
@@ -253,14 +256,17 @@
 
     async def start(self):
         self.session = Dependencies.ctx.get().resolve(AsyncSessionmaker)()
         self.commit_hooks = []
         self.rollback_hooks = []
 
     async def __aexit__(self, exc_type, exc_value, trace):
+        if self.lock is not None:
+            await self.lock.__aexit__(exc_type, exc_value, trace)
+
         if not self.context:
             return
         self.self_context.__exit__(exc_type, exc_value, trace)
         self.context.__exit__(exc_type, exc_value, trace)
         if self.session is None:
             return
         if not exc_type:
@@ -366,48 +372,27 @@
     def wrapper[**P, T](cb: Callable[P, Awaitable[T]]):  # type:ignore
         @asynccontextmanager
         async def run(*args: P.args, **kwargs: P.kwargs):
             session_provider = LazySession.ctx.get(None)
 
             if session_provider and not standalone:
                 session = await session_provider.start()
-                with use_context_value(session_context, session):
+                assert session.session is not None
+                with use_context_value(session_context, session.session):
                     yield await cb(*args, **kwargs)
                 return
 
             if (session_context.get(None) is not None) and not standalone:
                 yield await cb(*args, **kwargs)
                 return
 
             async with ContextSession():
                 yield await cb(*args, **kwargs)
 
-        if PluginConfig.parallel is not False:
-            return run
-
-        @asynccontextmanager
-        async def run_locked(*args: P.args, **kwargs: P.kwargs):
-            if session_context.get(None) is not None and not standalone:
-                logger.trace(
-                    "running nested transaction {}(*{}, **{})", cb, args, kwargs
-                )
-                yield await cb(*args, **kwargs)
-                return
-
-            logger.trace("waiting transaction {}(*{}, **{})", cb, args, kwargs)
-            async with tx_lock:
-                logger.trace("running transaction {}(*{}, **{})", cb, args, kwargs)
-                try:
-                    async with run(*args, **kwargs) as result:
-                        yield result
-                        return
-                finally:
-                    logger.trace("transaction ended {}(*{}, **{})", cb, args, kwargs)
-
-        return run_locked
+        return run
 
     return wrapper
 
 
 def transaction(tries: int = 3, standalone: bool = False):  # /NOSONAR
     tx = context_transaction(standalone)
     delays = [0] + [max(i**1.5, 60) for i in range(tries)]
```

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/fastapi.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel/tests.py` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel/tests.py`

 * *Files identical despite different names*

### Comparing `rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire_sqlmodel-0.3.0/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.4
+Version: 0.3.0
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

