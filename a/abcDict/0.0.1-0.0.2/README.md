# Comparing `tmp/abcDict-0.0.1.tar.gz` & `tmp/abcdict-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcDict-0.0.1.tar", last modified: Tue Feb  6 05:49:19 2024, max compression
+gzip compressed data, was "abcdict-0.0.2.tar", last modified: Thu Apr 18 12:19:16 2024, max compression
```

## Comparing `abcDict-0.0.1.tar` & `abcdict-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 05:49:19.934381 abcDict-0.0.1/
--rw-rw-rw-   0        0        0     1083 2024-02-06 05:45:24.000000 abcDict-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      464 2024-02-06 05:49:19.933380 abcDict-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2024-02-06 05:48:47.000000 abcDict-0.0.1/README.md
--rw-rw-rw-   0        0        0      570 2024-02-06 05:48:00.000000 abcDict-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 05:49:19.934381 abcDict-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-06 05:49:19.928379 abcDict-0.0.1/src/
--rw-rw-rw-   0        0        0       30 2024-02-06 05:46:23.000000 abcDict-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 05:49:19.932380 abcDict-0.0.1/src/abcDict.egg-info/
--rw-rw-rw-   0        0        0      464 2024-02-06 05:49:19.000000 abcDict-0.0.1/src/abcDict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-02-06 05:49:19.000000 abcDict-0.0.1/src/abcDict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 05:49:19.000000 abcDict-0.0.1/src/abcDict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-02-06 05:49:19.000000 abcDict-0.0.1/src/abcDict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2428 2024-02-06 05:46:50.000000 abcDict-0.0.1/src/abcdict.py
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.590995 abcdict-0.0.2/
+-rw-r--r--   0 tudou      (501) staff       (20)     1062 2024-04-18 12:15:37.000000 abcdict-0.0.2/LICENSE
+-rw-r--r--   0 tudou      (501) staff       (20)      450 2024-04-18 12:19:16.590774 abcdict-0.0.2/PKG-INFO
+-rw-r--r--   0 tudou      (501) staff       (20)       10 2024-04-18 12:15:37.000000 abcdict-0.0.2/README.md
+-rw-r--r--   0 tudou      (501) staff       (20)      547 2024-04-18 12:15:37.000000 abcdict-0.0.2/pyproject.toml
+-rw-r--r--   0 tudou      (501) staff       (20)       38 2024-04-18 12:19:16.591037 abcdict-0.0.2/setup.cfg
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.589866 abcdict-0.0.2/src/
+-rw-r--r--   0 tudou      (501) staff       (20)       28 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/__init__.py
+drwxr-xr-x   0 tudou      (501) staff       (20)        0 2024-04-18 12:19:16.590565 abcdict-0.0.2/src/abcDict.egg-info/
+-rw-r--r--   0 tudou      (501) staff       (20)      450 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/PKG-INFO
+-rw-r--r--   0 tudou      (501) staff       (20)      215 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/SOURCES.txt
+-rw-r--r--   0 tudou      (501) staff       (20)        1 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/dependency_links.txt
+-rw-r--r--   0 tudou      (501) staff       (20)       22 2024-04-18 12:19:16.000000 abcdict-0.0.2/src/abcDict.egg-info/top_level.txt
+-rw-r--r--   0 tudou      (501) staff       (20)     3305 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/abcdict.py
+-rw-r--r--   0 tudou      (501) staff       (20)       75 2024-04-18 12:15:37.000000 abcdict-0.0.2/src/util.py
```

### Comparing `abcDict-0.0.1/pyproject.toml` & `abcdict-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = [
-    "setuptools>=61.0",
-    "PyYAML>=5.4.1"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "abcDict"
-version = "0.0.1"
-authors = [
-    { name="msbrm", email="cuihaniss@gmail.com" },
-]
-description = "use yaml config easy"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/msbrm/abcDict/tree/main"
+[build-system]
+requires = [
+    "setuptools>=61.0",
+    "PyYAML>=5.4.1"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "abcDict"
+version = "0.0.2"
+authors = [
+    { name="msbrm", email="cuihaniss@gmail.com" },
+]
+description = "use yaml config easy"
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/msbrm/abcDict/tree/main"
 "Bug Tracker" = "https://github.com/msbrm/abcDict/issues"
```

