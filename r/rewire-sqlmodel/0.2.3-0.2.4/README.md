# Comparing `tmp/rewire-sqlmodel-0.2.3.tar.gz` & `tmp/rewire_sqlmodel-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.2.3.tar", last modified: Mon Apr  8 20:12:32 2024, max compression
+gzip compressed data, was "rewire_sqlmodel-0.2.4.tar", last modified: Wed Apr 17 17:45:37 2024, max compression
```

## Comparing `rewire-sqlmodel-0.2.3.tar` & `rewire_sqlmodel-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.095971 rewire-sqlmodel-0.2.3/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-04-08 20:12:32.094468 rewire-sqlmodel-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.2.3/README.md
--rw-rw-rw-   0        0        0      812 2024-04-08 20:12:20.000000 rewire-sqlmodel-0.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.079941 rewire-sqlmodel-0.2.3/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    15870 2024-04-08 20:12:06.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.091462 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.091462 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.092467 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2582 2024-04-08 18:06:38.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:12:32.093466 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-04-08 20:12:32.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-08 20:12:32.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:12:32.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 20:12:32.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 20:12:32.000000 rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 20:12:32.096145 rewire-sqlmodel-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.370274 rewire_sqlmodel-0.2.4/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-17 17:45:37.369277 rewire_sqlmodel-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire_sqlmodel-0.2.4/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-17 17:45:25.000000 rewire_sqlmodel-0.2.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.346250 rewire_sqlmodel-0.2.4/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    15870 2024-04-08 20:12:06.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.364764 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.366269 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.366269 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2521 2024-04-17 17:45:21.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:45:37.367274 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 17:45:37.000000 rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 17:45:37.370274 rewire_sqlmodel-0.2.4/setup.cfg
```

### Comparing `rewire-sqlmodel-0.2.3/LICENSE` & `rewire_sqlmodel-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/PKG-INFO` & `rewire_sqlmodel-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.3
+Version: 0.2.4
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.2.3/pyproject.toml` & `rewire_sqlmodel-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.2.3"
+version = "0.2.4"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/__init__.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/ext/fastapi.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel/tests.py` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,17 @@
     data: Sequence[Union[Callable[[], None], SQLModel]]
 
     @asynccontextmanager
     async def use_module(self):
         with TemporaryDirectory() as dir:
             ConfigModule.get().patch(
                 {
-                    "plugins": {
-                        "sql": {
-                            "alembic": {"generate": False},
-                            "url": f"sqlite+aiosqlite:///{dir}/db.sqlite",
-                        }
+                    "rewire_sqlmodel": {
+                        "alembic": {"generate": False},
+                        "url": f"sqlite+aiosqlite:///{dir}/db.sqlite",
                     }
                 }
             )
             yield
 
     @transaction(1)
     async def _init(self):
```

### Comparing `rewire-sqlmodel-0.2.3/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire_sqlmodel-0.2.4/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.2.3
+Version: 0.2.4
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

