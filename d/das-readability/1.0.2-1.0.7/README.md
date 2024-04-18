# Comparing `tmp/das_readability-1.0.2.tar.gz` & `tmp/das_readability-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "das_readability-1.0.2.tar", max compression
+gzip compressed data, was "das_readability-1.0.7.tar", max compression
```

## Comparing `das_readability-1.0.2.tar` & `das_readability-1.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       35 2024-04-17 11:49:15.852161 das_readability-1.0.2/LICENSE
--rw-r--r--   0        0        0       17 2024-04-17 09:54:26.916751 das_readability-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-17 11:33:43.740872 das_readability-1.0.2/das_readability/__init__.py
--rw-r--r--   0        0        0       87 2024-04-18 08:01:24.044671 das_readability-1.0.2/das_readability/__main__.py
--rw-r--r--   0        0        0     6884 2024-04-18 08:01:21.768655 das_readability-1.0.2/das_readability/readability.py
--rw-r--r--   0        0        0      769 2024-04-18 08:22:08.997154 das_readability-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 das_readability-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-04-17 11:49:15.852161 das_readability-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1821 2024-04-18 10:02:08.774946 das_readability-1.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 11:33:43.740872 das_readability-1.0.7/das_readability/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-18 08:01:24.044671 das_readability-1.0.7/das_readability/__main__.py
+-rw-r--r--   0        0        0     6876 2024-04-18 09:51:07.179652 das_readability-1.0.7/das_readability/readability.py
+-rw-r--r--   0        0        0     1060 2024-04-18 11:09:01.469219 das_readability-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 das_readability-1.0.7/PKG-INFO
```

### Comparing `das_readability-1.0.2/das_readability/readability.py` & `das_readability-1.0.7/das_readability/readability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-name: DAS Readability Checker
+name: DAS Readability
 license: Copyright (C) 2024 Novo Nordisk A/S
 author: LZVB <lzvb@novonordisk.com>
 file: readability.py
 
 Checks the readability of markdown files in a directory and its subdirectories.
 It uses the textstat library to calculate the SMOG Index and Flesch Reading Ease score.
 The SMOG Index is chosen due to its general application in the healthcare industry.
```

### Comparing `das_readability-1.0.2/pyproject.toml` & `das_readability-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [tool.poetry]
 name = "das-readability"
-version = "1.0.2"
+version = "1.0.7"
 description = "Checks the readability of markdown files in a directory and its subdirectories."
 authors = ["lzvb <lzvb@novonordisk.com>"]
 license = "Copyright (C) 2024 Novo Nordisk A/S"
 readme = "README.md"
 packages = [{include = "das_readability"}]
+repository = "https://github.com/innersource-nn/das-readability"
+documentation = "https://github.com/innersource-nn/das-readability"
+homepage = "https://github.com/innersource-nn/das-readability"
+keywords = ["readability", "markdown", "textstat", "cli", "smog", "reading", "ease", "flesch"]
 
 [tool.poetry.scripts]
 readability = "das_readability.readability:main"
 das-readability = "das_readability.readability:main"
 
 [tool.poetry.dependencies]
 python = "^3.9.7"
```

