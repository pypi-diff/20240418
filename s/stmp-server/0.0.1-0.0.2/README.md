# Comparing `tmp/stmp_server-0.0.1.tar.gz` & `tmp/stmp_server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmp_server-0.0.1.tar", last modified: Thu Apr 18 09:53:55 2024, max compression
+gzip compressed data, was "stmp_server-0.0.2.tar", last modified: Thu Apr 18 16:34:32 2024, max compression
```

## Comparing `stmp_server-0.0.1.tar` & `stmp_server-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:55.637170 stmp_server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:55.637170 stmp_server-0.0.1/.assets/
--rw-r--r--   0 runner    (1001) docker     (127)    96470 2024-04-18 09:53:41.000000 stmp_server-0.0.1/.assets/stmp.excalidraw.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 09:53:41.000000 stmp_server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-18 09:53:41.000000 stmp_server-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 09:53:55.637170 stmp_server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-18 09:53:41.000000 stmp_server-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-18 09:53:41.000000 stmp_server-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 09:53:41.000000 stmp_server-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:53:55.637170 stmp_server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:55.637170 stmp_server-0.0.1/stmp/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 09:53:41.000000 stmp_server-0.0.1/stmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 09:53:41.000000 stmp_server-0.0.1/stmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 09:53:41.000000 stmp_server-0.0.1/stmp/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-18 09:53:41.000000 stmp_server-0.0.1/stmp/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-18 09:53:41.000000 stmp_server-0.0.1/stmp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:55.637170 stmp_server-0.0.1/stmp_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 09:53:55.000000 stmp_server-0.0.1/stmp_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 09:53:55.000000 stmp_server-0.0.1/stmp_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:53:55.000000 stmp_server-0.0.1/stmp_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 09:53:55.000000 stmp_server-0.0.1/stmp_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 09:53:55.000000 stmp_server-0.0.1/stmp_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:53:55.637170 stmp_server-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 09:53:41.000000 stmp_server-0.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.124820 stmp_server-0.0.2/.assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    96470 2024-04-18 16:34:19.000000 stmp_server-0.0.2/.assets/stmp.excalidraw.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 16:34:19.000000 stmp_server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 16:34:19.000000 stmp_server-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 16:34:32.128820 stmp_server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-18 16:34:19.000000 stmp_server-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-18 16:34:19.000000 stmp_server-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 16:34:19.000000 stmp_server-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:34:32.128820 stmp_server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp/stmp_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/stmp_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp/stmp_server/transilation/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transilation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp/stmp_server/transilation/enc/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transilation/enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transilation/enc/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transilation/transilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp/stmp_server/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transport/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-18 16:34:19.000000 stmp_server-0.0.2/stmp/stmp_server/transport/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/stmp_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 16:34:32.000000 stmp_server-0.0.2/stmp_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 16:34:32.000000 stmp_server-0.0.2/stmp_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:34:32.000000 stmp_server-0.0.2/stmp_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 16:34:32.000000 stmp_server-0.0.2/stmp_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 16:34:32.000000 stmp_server-0.0.2/stmp_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:34:32.128820 stmp_server-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 16:34:19.000000 stmp_server-0.0.2/test/test.py
```

### Comparing `stmp_server-0.0.1/.assets/stmp.excalidraw.svg` & `stmp_server-0.0.2/.assets/stmp.excalidraw.svg`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/LICENSE` & `stmp_server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/PKG-INFO` & `stmp_server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmp-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: A primitive zero-configuration local network protocol purely written in python, originally intended for tinkering with your office mates over LAN!
 Author-email: "@bRuttaZz" <agrajpdasprivate@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Agraj P Das
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stmp_server-0.0.1/README.md` & `stmp_server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/pyproject.toml` & `stmp_server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/stmp/interfaces.py` & `stmp_server-0.0.2/stmp/interfaces.py`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/stmp/server.py` & `stmp_server-0.0.2/stmp/server.py`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/stmp/settings.py` & `stmp_server-0.0.2/stmp/settings.py`

 * *Files identical despite different names*

### Comparing `stmp_server-0.0.1/stmp_server.egg-info/PKG-INFO` & `stmp_server-0.0.2/stmp_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmp-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: A primitive zero-configuration local network protocol purely written in python, originally intended for tinkering with your office mates over LAN!
 Author-email: "@bRuttaZz" <agrajpdasprivate@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Agraj P Das
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stmp_server-0.0.1/test/test.py` & `stmp_server-0.0.2/test/test.py`

 * *Files identical despite different names*

