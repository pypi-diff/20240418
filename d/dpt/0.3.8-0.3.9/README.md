# Comparing `tmp/dpt-0.3.8.tar.gz` & `tmp/dpt-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-0.3.8.tar", last modified: Sun Apr 14 15:37:59 2024, max compression
+gzip compressed data, was "dpt-0.3.9.tar", last modified: Thu Apr 18 18:34:46 2024, max compression
```

## Comparing `dpt-0.3.8.tar` & `dpt-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:37:59.155127 dpt-0.3.8/
--rw-rw-rw-   0        0        0      188 2024-04-14 15:37:59.154127 dpt-0.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 15:37:59.109869 dpt-0.3.8/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-0.3.8/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:37:59.148127 dpt-0.3.8/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-0.3.8/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-0.3.8/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-0.3.8/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-0.3.8/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-0.3.8/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:37:59.152129 dpt-0.3.8/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-0.3.8/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-0.3.8/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-0.3.8/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13237 2024-04-12 03:20:41.000000 dpt-0.3.8/dpt/processor.py
--rw-rw-rw-   0        0        0     5729 2024-04-12 03:20:41.000000 dpt-0.3.8/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:37:59.128522 dpt-0.3.8/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-04-14 15:37:59.000000 dpt-0.3.8/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-04-14 15:37:59.000000 dpt-0.3.8/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:37:59.000000 dpt-0.3.8/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-14 15:37:59.000000 dpt-0.3.8/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-14 15:37:59.000000 dpt-0.3.8/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:37:59.155127 dpt-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-14 15:37:06.000000 dpt-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.573165 dpt-0.3.9/
+-rw-rw-rw-   0        0        0      188 2024-04-18 18:34:46.571165 dpt-0.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.502166 dpt-0.3.9/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-0.3.9/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.556172 dpt-0.3.9/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-0.3.9/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-0.3.9/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-0.3.9/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-0.3.9/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-0.3.9/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.567165 dpt-0.3.9/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-0.3.9/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-0.3.9/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-0.3.9/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-0.3.9/dpt/processor.py
+-rw-rw-rw-   0        0        0     5729 2024-04-12 03:20:41.000000 dpt-0.3.9/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.544207 dpt-0.3.9/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:34:46.574185 dpt-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-18 18:34:40.000000 dpt-0.3.9/setup.py
```

### Comparing `dpt-0.3.8/dpt/deployment/deploy.py` & `dpt-0.3.9/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.8/dpt/deployment/extract.py` & `dpt-0.3.9/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.8/dpt/management.py` & `dpt-0.3.9/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.8/dpt/mongo/files.py` & `dpt-0.3.9/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.8/dpt/processor.py` & `dpt-0.3.9/dpt/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         self.modules[module.name] = module
         module.project = self
 
     def get_module(self, info: str | ModuleType):
         if isinstance(info, str):
             name = info
         else:
-            name = info.__name__.rsplit(".", 1)[-1]
+            parts = info.__name__.split('.')
+            name = '.'.join(parts[1:])
         if name not in self.modules:
             raise Exception(f"module '{name}' is not defined")
         return self.modules[name]
 
     def add_modules(self, modules: list[Module]):
         for item in modules:
             self.add_module(item)
```

### Comparing `dpt-0.3.8/dpt/storage.py` & `dpt-0.3.9/dpt/storage.py`

 * *Files identical despite different names*

