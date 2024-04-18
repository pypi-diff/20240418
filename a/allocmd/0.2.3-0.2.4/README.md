# Comparing `tmp/allocmd-0.2.3.tar.gz` & `tmp/allocmd-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocmd-0.2.3.tar", last modified: Fri Mar 22 14:39:45 2024, max compression
+gzip compressed data, was "allocmd-0.2.4.tar", last modified: Thu Apr 18 09:54:25 2024, max compression
```

## Comparing `allocmd-0.2.3.tar` & `allocmd-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-03-22 14:39:45.738506 allocmd-0.2.3/
--rw-r--r--   0 okedeji    (501) staff       (20)    11357 2024-03-15 12:58:44.000000 allocmd-0.2.3/LICENSE
--rw-r--r--   0 okedeji    (501) staff       (20)     5734 2024-03-22 14:39:45.738255 allocmd-0.2.3/PKG-INFO
--rw-r--r--   0 okedeji    (501) staff       (20)     4741 2024-03-14 16:23:54.000000 allocmd-0.2.3/README.md
-drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-03-22 14:39:45.734281 allocmd-0.2.3/allocmd/
--rw-r--r--   0 okedeji    (501) staff       (20)        0 2024-02-05 15:29:39.000000 allocmd-0.2.3/allocmd/__init__.py
--rw-r--r--   0 okedeji    (501) staff       (20)     7224 2024-03-22 13:49:33.000000 allocmd-0.2.3/allocmd/cli.py
-drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-03-22 14:39:45.737800 allocmd-0.2.3/allocmd/utilities/
--rw-r--r--   0 okedeji    (501) staff       (20)        0 2024-02-14 17:17:13.000000 allocmd-0.2.3/allocmd/utilities/__init__.py
--rw-r--r--   0 okedeji    (501) staff       (20)       22 2024-03-22 14:39:31.000000 allocmd-0.2.3/allocmd/utilities/constants.py
--rw-r--r--   0 okedeji    (501) staff       (20)       88 2024-02-14 17:20:33.000000 allocmd-0.2.3/allocmd/utilities/typings.py
--rw-r--r--   0 okedeji    (501) staff       (20)    20019 2024-03-22 14:31:11.000000 allocmd-0.2.3/allocmd/utilities/utils.py
-drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-03-22 14:39:45.736529 allocmd-0.2.3/allocmd.egg-info/
--rw-r--r--   0 okedeji    (501) staff       (20)     5734 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/PKG-INFO
--rw-r--r--   0 okedeji    (501) staff       (20)      366 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/SOURCES.txt
--rw-r--r--   0 okedeji    (501) staff       (20)        1 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/dependency_links.txt
--rw-r--r--   0 okedeji    (501) staff       (20)       63 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/entry_points.txt
--rw-r--r--   0 okedeji    (501) staff       (20)       44 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/requires.txt
--rw-r--r--   0 okedeji    (501) staff       (20)        8 2024-03-22 14:39:45.000000 allocmd-0.2.3/allocmd.egg-info/top_level.txt
--rw-r--r--   0 okedeji    (501) staff       (20)       38 2024-03-22 14:39:45.738602 allocmd-0.2.3/setup.cfg
--rw-r--r--   0 okedeji    (501) staff       (20)      987 2024-03-15 13:03:27.000000 allocmd-0.2.3/setup.py
+drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-04-18 09:54:25.381286 allocmd-0.2.4/
+-rw-r--r--   0 okedeji    (501) staff       (20)    11357 2024-03-15 12:58:44.000000 allocmd-0.2.4/LICENSE
+-rw-r--r--   0 okedeji    (501) staff       (20)     5734 2024-04-18 09:54:25.380886 allocmd-0.2.4/PKG-INFO
+-rw-r--r--   0 okedeji    (501) staff       (20)     4741 2024-03-14 16:23:54.000000 allocmd-0.2.4/README.md
+drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-04-18 09:54:25.374792 allocmd-0.2.4/allocmd/
+-rw-r--r--   0 okedeji    (501) staff       (20)        0 2024-02-05 15:29:39.000000 allocmd-0.2.4/allocmd/__init__.py
+-rw-r--r--   0 okedeji    (501) staff       (20)     7224 2024-03-22 13:49:33.000000 allocmd-0.2.4/allocmd/cli.py
+drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-04-18 09:54:25.379452 allocmd-0.2.4/allocmd/utilities/
+-rw-r--r--   0 okedeji    (501) staff       (20)        0 2024-02-14 17:17:13.000000 allocmd-0.2.4/allocmd/utilities/__init__.py
+-rw-r--r--   0 okedeji    (501) staff       (20)       22 2024-04-18 09:51:04.000000 allocmd-0.2.4/allocmd/utilities/constants.py
+-rw-r--r--   0 okedeji    (501) staff       (20)       88 2024-02-14 17:20:33.000000 allocmd-0.2.4/allocmd/utilities/typings.py
+-rw-r--r--   0 okedeji    (501) staff       (20)    20019 2024-03-22 14:31:11.000000 allocmd-0.2.4/allocmd/utilities/utils.py
+drwxr-xr-x   0 okedeji    (501) staff       (20)        0 2024-04-18 09:54:25.377746 allocmd-0.2.4/allocmd.egg-info/
+-rw-r--r--   0 okedeji    (501) staff       (20)     5734 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/PKG-INFO
+-rw-r--r--   0 okedeji    (501) staff       (20)      366 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/SOURCES.txt
+-rw-r--r--   0 okedeji    (501) staff       (20)        1 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/dependency_links.txt
+-rw-r--r--   0 okedeji    (501) staff       (20)       63 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/entry_points.txt
+-rw-r--r--   0 okedeji    (501) staff       (20)       44 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/requires.txt
+-rw-r--r--   0 okedeji    (501) staff       (20)        8 2024-04-18 09:54:25.000000 allocmd-0.2.4/allocmd.egg-info/top_level.txt
+-rw-r--r--   0 okedeji    (501) staff       (20)       38 2024-04-18 09:54:25.381466 allocmd-0.2.4/setup.cfg
+-rw-r--r--   0 okedeji    (501) staff       (20)      987 2024-03-15 13:03:27.000000 allocmd-0.2.4/setup.py
```

### Comparing `allocmd-0.2.3/LICENSE` & `allocmd-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `allocmd-0.2.3/PKG-INFO` & `allocmd-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
```

### Comparing `allocmd-0.2.3/README.md` & `allocmd-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `allocmd-0.2.3/allocmd/cli.py` & `allocmd-0.2.4/allocmd/cli.py`

 * *Files identical despite different names*

### Comparing `allocmd-0.2.3/allocmd/utilities/utils.py` & `allocmd-0.2.4/allocmd/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `allocmd-0.2.3/allocmd.egg-info/PKG-INFO` & `allocmd-0.2.4/allocmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
```

### Comparing `allocmd-0.2.3/setup.py` & `allocmd-0.2.4/setup.py`

 * *Files identical despite different names*

