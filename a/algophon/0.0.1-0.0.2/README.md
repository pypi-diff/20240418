# Comparing `tmp/algophon-0.0.1.tar.gz` & `tmp/algophon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.0.1.tar", last modified: Thu Apr 18 14:54:04 2024, max compression
+gzip compressed data, was "algophon-0.0.2.tar", last modified: Thu Apr 18 16:47:35 2024, max compression
```

## Comparing `algophon-0.0.1.tar` & `algophon-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 14:54:04.349256 algophon-0.0.1/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.1/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)      843 2024-04-18 14:54:04.348220 algophon-0.0.1/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      238 2024-04-18 14:19:46.000000 algophon-0.0.1/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 14:54:04.338407 algophon-0.0.1/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-04-18 14:24:25.000000 algophon-0.0.1/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 14:54:04.347098 algophon-0.0.1/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)      843 2024-04-18 14:54:04.000000 algophon-0.0.1/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      181 2024-04-18 14:54:04.000000 algophon-0.0.1/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 14:54:04.000000 algophon-0.0.1/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 14:54:04.000000 algophon-0.0.1/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      734 2024-04-18 14:53:56.000000 algophon-0.0.1/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 14:54:04.349367 algophon-0.0.1/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.692990 algophon-0.0.2/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.0.2/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)     1147 2024-04-18 16:47:35.692376 algophon-0.0.2/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      542 2024-04-18 15:22:58.000000 algophon-0.0.2/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.687142 algophon-0.0.2/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      129 2024-04-18 16:17:39.000000 algophon-0.0.2/algophon/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350526 2024-04-18 15:23:33.000000 algophon-0.0.2/algophon/ipa.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)     1167 2024-04-18 15:56:55.000000 algophon-0.0.2/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3485 2024-04-18 16:31:03.000000 algophon-0.0.2/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      202 2024-04-18 15:16:06.000000 algophon-0.0.2/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      203 2024-04-18 15:37:08.000000 algophon-0.0.2/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-04-18 16:47:35.691532 algophon-0.0.2/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)     1147 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      272 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-04-18 16:47:35.000000 algophon-0.0.2/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      788 2024-04-18 16:46:20.000000 algophon-0.0.2/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-04-18 16:47:35.693068 algophon-0.0.2/setup.cfg
```

### Comparing `algophon-0.0.1/LICENSE` & `algophon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.0.1/pyproject.toml` & `algophon-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
@@ -20,9 +20,12 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
+[tool.setuptools.package-data]
+algophon = ["ipa.txt"]
+
 [project.urls]
-Homepage = "https://github.com/cbelth/algophon"
+Homepage = "https://github.com/cbelth/algophon"
```

