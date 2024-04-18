# Comparing `tmp/myria3d-3.8.1.tar.gz` & `tmp/myria3d-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myria3d-3.8.1.tar", last modified: Thu Apr 18 12:58:49 2024, max compression
+gzip compressed data, was "myria3d-3.8.2.tar", last modified: Thu Apr 18 13:05:20 2024, max compression
```

## Comparing `myria3d-3.8.1.tar` & `myria3d-3.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 12:58:49.718924 myria3d-3.8.1/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1571 2022-12-07 10:34:45.000000 myria3d-3.8.1/LICENSE
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 12:58:49.718924 myria3d-3.8.1/PKG-INFO
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     3396 2023-04-04 08:22:07.000000 myria3d-3.8.1/README.md
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 12:58:49.710924 myria3d-3.8.1/myria3d/
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)      266 2022-12-07 10:34:45.000000 myria3d-3.8.1/myria3d/__init__.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       74 2024-04-18 12:55:41.000000 myria3d-3.8.1/myria3d/_version.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2713 2024-03-13 09:13:29.000000 myria3d-3.8.1/myria3d/predict.py
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     6751 2024-03-13 09:13:29.000000 myria3d-3.8.1/myria3d/train.py
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 12:58:49.714924 myria3d-3.8.1/myria3d.egg-info/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 12:58:49.000000 myria3d-3.8.1/myria3d.egg-info/PKG-INFO
--rw-r--r--   0 LVauchier (24820) usernis  (10000)      232 2024-04-18 12:58:49.000000 myria3d-3.8.1/myria3d.egg-info/SOURCES.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)        1 2024-04-18 12:58:49.000000 myria3d-3.8.1/myria3d.egg-info/dependency_links.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)        8 2024-04-18 12:58:49.000000 myria3d-3.8.1/myria3d.egg-info/top_level.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1958 2024-04-18 12:55:41.000000 myria3d-3.8.1/pyproject.toml
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       38 2024-04-18 12:58:49.718924 myria3d-3.8.1/setup.cfg
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.222821 myria3d-3.8.2/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     1571 2022-12-07 10:34:45.000000 myria3d-3.8.2/LICENSE
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 13:05:20.222821 myria3d-3.8.2/PKG-INFO
+-rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     3396 2023-04-04 08:22:07.000000 myria3d-3.8.2/README.md
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.218821 myria3d-3.8.2/myria3d/
+-rwxr-xr-x   0 LVauchier (24820) usernis  (10000)      266 2022-12-07 10:34:45.000000 myria3d-3.8.2/myria3d/__init__.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)       74 2024-04-18 13:00:25.000000 myria3d-3.8.2/myria3d/_version.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2713 2024-03-13 09:13:29.000000 myria3d-3.8.2/myria3d/predict.py
+-rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     6751 2024-03-13 09:13:29.000000 myria3d-3.8.2/myria3d/train.py
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.222821 myria3d-3.8.2/myria3d.egg-info/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/PKG-INFO
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)      232 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/SOURCES.txt
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)        1 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/dependency_links.txt
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)        8 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/top_level.txt
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     1958 2024-04-18 12:55:41.000000 myria3d-3.8.2/pyproject.toml
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)       38 2024-04-18 13:05:20.222821 myria3d-3.8.2/setup.cfg
```

### Comparing `myria3d-3.8.1/LICENSE` & `myria3d-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.1/PKG-INFO` & `myria3d-3.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myria3d
-Version: 3.8.1
+Version: 3.8.2
 Summary: Deep Learning for the Semantic Segmentation of Aerial Lidar Point Clouds
 Author-email: Charles GAYDON <charles.gaydon@gmail.com>
 Maintainer: Michel DAAB
 Maintainer-email: Charles GAYDON <charles.gaydon@gmail.com>, Léa VAUCHIER <lea.vauchier@ign.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Institut National de l'Information Géographique et Forestière
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: myria3d Version: 3.8.1 Summary: Deep Learning for
+Metadata-Version: 2.1 Name: myria3d Version: 3.8.2 Summary: Deep Learning for
 the Semantic Segmentation of Aerial Lidar Point Clouds Author-email: Charles
 GAYDON
 gmail.com> Maintainer: Michel DAAB Maintainer-email: Charles GAYDON
 gmail.com>, LÃ©a VAUCHIER
 ign.fr> License: BSD 3-Clause License Copyright (c) 2021, Institut National de
 l'Information GÃ©ographique et ForestiÃ¨re All rights reserved. Redistribution
 and use in source and binary forms, with or without modification, are permitted
```

### Comparing `myria3d-3.8.1/README.md` & `myria3d-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.1/myria3d/predict.py` & `myria3d-3.8.2/myria3d/predict.py`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.1/myria3d/train.py` & `myria3d-3.8.2/myria3d/train.py`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.1/myria3d.egg-info/PKG-INFO` & `myria3d-3.8.2/myria3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myria3d
-Version: 3.8.1
+Version: 3.8.2
 Summary: Deep Learning for the Semantic Segmentation of Aerial Lidar Point Clouds
 Author-email: Charles GAYDON <charles.gaydon@gmail.com>
 Maintainer: Michel DAAB
 Maintainer-email: Charles GAYDON <charles.gaydon@gmail.com>, Léa VAUCHIER <lea.vauchier@ign.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Institut National de l'Information Géographique et Forestière
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: myria3d Version: 3.8.1 Summary: Deep Learning for
+Metadata-Version: 2.1 Name: myria3d Version: 3.8.2 Summary: Deep Learning for
 the Semantic Segmentation of Aerial Lidar Point Clouds Author-email: Charles
 GAYDON
 gmail.com> Maintainer: Michel DAAB Maintainer-email: Charles GAYDON
 gmail.com>, LÃ©a VAUCHIER
 ign.fr> License: BSD 3-Clause License Copyright (c) 2021, Institut National de
 l'Information GÃ©ographique et ForestiÃ¨re All rights reserved. Redistribution
 and use in source and binary forms, with or without modification, are permitted
```

### Comparing `myria3d-3.8.1/pyproject.toml` & `myria3d-3.8.2/pyproject.toml`

 * *Files identical despite different names*

