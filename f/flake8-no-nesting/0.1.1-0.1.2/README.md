# Comparing `tmp/flake8_no_nesting-0.1.1.tar.gz` & `tmp/flake8_no_nesting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_no_nesting-0.1.1.tar", last modified: Wed Apr 17 05:32:27 2024, max compression
+gzip compressed data, was "flake8_no_nesting-0.1.2.tar", last modified: Thu Apr 18 05:40:47 2024, max compression
```

## Comparing `flake8_no_nesting-0.1.1.tar` & `flake8_no_nesting-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-17 05:32:27.367109 flake8_no_nesting-0.1.1/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1030 2024-04-17 05:32:27.367109 flake8_no_nesting-0.1.1/PKG-INFO
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      101 2024-04-17 05:30:52.000000 flake8_no_nesting-0.1.1/README.md
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-17 05:32:27.367109 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1030 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/PKG-INFO
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      329 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/SOURCES.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)        1 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/dependency_links.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       50 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/entry_points.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       63 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/requires.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       18 2024-04-17 05:32:27.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.egg-info/top_level.txt
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2521 2024-04-17 05:22:40.000000 flake8_no_nesting-0.1.1/flake8_no_nesting.py
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1080 2024-04-17 05:32:27.367109 flake8_no_nesting-0.1.1/setup.cfg
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       39 2024-04-16 05:04:25.000000 flake8_no_nesting-0.1.1/setup.py
-drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-17 05:32:27.367109 flake8_no_nesting-0.1.1/tests/
--rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2529 2024-04-17 05:21:52.000000 flake8_no_nesting-0.1.1/tests/test_flake8_no_nesting.py
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-18 05:40:46.996897 flake8_no_nesting-0.1.2/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     3161 2024-04-18 05:40:46.996897 flake8_no_nesting-0.1.2/PKG-INFO
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2232 2024-04-18 05:36:49.000000 flake8_no_nesting-0.1.2/README.md
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-18 05:40:46.996897 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     3161 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/PKG-INFO
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)      329 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/SOURCES.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)        1 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/dependency_links.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       50 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/entry_points.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       63 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/requires.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       18 2024-04-18 05:40:46.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.egg-info/top_level.txt
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2521 2024-04-18 05:30:53.000000 flake8_no_nesting-0.1.2/flake8_no_nesting.py
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     1080 2024-04-18 05:40:46.996897 flake8_no_nesting-0.1.2/setup.cfg
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)       39 2024-04-16 05:04:25.000000 flake8_no_nesting-0.1.2/setup.py
+drwxr-xr-x   0 nocyphr   (1000) nocyphr   (1000)        0 2024-04-18 05:40:46.996897 flake8_no_nesting-0.1.2/tests/
+-rw-r--r--   0 nocyphr   (1000) nocyphr   (1000)     2529 2024-04-18 05:29:42.000000 flake8_no_nesting-0.1.2/tests/test_flake8_no_nesting.py
```

### Comparing `flake8_no_nesting-0.1.1/flake8_no_nesting.py` & `flake8_no_nesting-0.1.2/flake8_no_nesting.py`

 * *Files identical despite different names*

### Comparing `flake8_no_nesting-0.1.1/setup.cfg` & `flake8_no_nesting-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8_no_nesting
-version = 0.1.1
+version = 0.1.2
 description = A flake8 plugin to enforce object calisthenics rule "ONE level of indentation"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sebastian Guckes
 author_email = nocyphr@outlook.com
 url = https://git.nocyphr.com/flake8-plugins/flake8-no-nesting
 license = MIT
```

### Comparing `flake8_no_nesting-0.1.1/tests/test_flake8_no_nesting.py` & `flake8_no_nesting-0.1.2/tests/test_flake8_no_nesting.py`

 * *Files identical despite different names*

