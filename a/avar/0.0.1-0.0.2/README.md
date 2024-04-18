# Comparing `tmp/avar-0.0.1.tar.gz` & `tmp/avar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avar-0.0.1.tar", last modified: Thu Apr 18 11:30:18 2024, max compression
+gzip compressed data, was "avar-0.0.2.tar", last modified: Thu Apr 18 11:42:24 2024, max compression
```

## Comparing `avar-0.0.1.tar` & `avar-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:30:18.854611 avar-0.0.1/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.1/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:30:18.854559 avar-0.0.1/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       45 2024-04-18 11:27:04.000000 avar-0.0.1/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.1/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-04-18 11:30:18.854828 avar-0.0.1/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:30:18.852831 avar-0.0.1/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:30:18.853629 avar-0.0.1/src/avar/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.1/src/avar/__init__.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)     8541 2024-04-16 21:22:35.000000 avar-0.0.1/src/avar/allan.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)      770 2024-04-16 22:40:50.000000 avar-0.0.1/src/avar/test_allan.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:30:18.854390 avar-0.0.1/src/avar.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:30:18.000000 avar-0.0.1/src/avar.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      267 2024-04-18 11:30:18.000000 avar-0.0.1/src/avar.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-18 11:30:18.000000 avar-0.0.1/src/avar.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-04-18 11:30:18.000000 avar-0.0.1/src/avar.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-04-18 11:30:18.000000 avar-0.0.1/src/avar.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:42:24.391291 avar-0.0.2/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.2/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:42:24.391242 avar-0.0.2/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       45 2024-04-18 11:27:04.000000 avar-0.0.2/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.2/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-04-18 11:42:24.391513 avar-0.0.2/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:42:24.389493 avar-0.0.2/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:42:24.390267 avar-0.0.2/src/avar/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.2/src/avar/__init__.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)     8541 2024-04-16 21:22:35.000000 avar-0.0.2/src/avar/avar.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)      770 2024-04-16 22:40:50.000000 avar-0.0.2/src/avar/test_avar.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-18 11:42:24.391061 avar-0.0.2/src/avar.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      513 2024-04-18 11:42:24.000000 avar-0.0.2/src/avar.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-04-18 11:42:24.000000 avar-0.0.2/src/avar.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-18 11:42:24.000000 avar-0.0.2/src/avar.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-04-18 11:42:24.000000 avar-0.0.2/src/avar.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-04-18 11:42:24.000000 avar-0.0.2/src/avar.egg-info/top_level.txt
```

### Comparing `avar-0.0.1/LICENSE.txt` & `avar-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avar-0.0.1/setup.cfg` & `avar-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = avar
-version = 0.0.1
+version = 0.0.2
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Allan variance tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/avar
 classifiers =
```

### Comparing `avar-0.0.1/src/avar/allan.py` & `avar-0.0.2/src/avar/avar.py`

 * *Files identical despite different names*

### Comparing `avar-0.0.1/src/avar/test_allan.py` & `avar-0.0.2/src/avar/test_avar.py`

 * *Files identical despite different names*

