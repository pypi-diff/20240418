# Comparing `tmp/sebchw_example_package-0.2.2.tar.gz` & `tmp/sebchw_example_package-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sebchw_example_package-0.2.2.tar", last modified: Thu Apr 18 06:46:13 2024, max compression
+gzip compressed data, was "sebchw_example_package-0.3.2.tar", last modified: Thu Apr 18 07:10:00 2024, max compression
```

## Comparing `sebchw_example_package-0.2.2.tar` & `sebchw_example_package-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:46:13.607823 sebchw_example_package-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-18 06:46:09.000000 sebchw_example_package-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 06:46:13.607823 sebchw_example_package-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 06:46:09.000000 sebchw_example_package-0.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     2039 2024-04-18 06:46:10.000000 sebchw_example_package-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 06:46:13.607823 sebchw_example_package-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:46:13.603823 sebchw_example_package-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:46:13.603823 sebchw_example_package-0.2.2/src/sebchw_example_package/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 06:46:09.000000 sebchw_example_package-0.2.2/src/sebchw_example_package/__init__.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-18 06:46:09.000000 sebchw_example_package-0.2.2/src/sebchw_example_package/example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:46:13.607823 sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 06:46:13.000000 sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      309 2024-04-18 06:46:13.000000 sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 06:46:13.000000 sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 06:46:13.000000 sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:10:00.334854 sebchw_example_package-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-18 07:09:56.000000 sebchw_example_package-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 07:10:00.334854 sebchw_example_package-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 07:09:56.000000 sebchw_example_package-0.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2039 2024-04-18 07:09:57.000000 sebchw_example_package-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 07:10:00.334854 sebchw_example_package-0.3.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:10:00.330854 sebchw_example_package-0.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:10:00.330854 sebchw_example_package-0.3.2/src/sebchw_example_package/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 07:09:56.000000 sebchw_example_package-0.3.2/src/sebchw_example_package/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-18 07:09:56.000000 sebchw_example_package-0.3.2/src/sebchw_example_package/example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:10:00.334854 sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-04-18 07:10:00.000000 sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      309 2024-04-18 07:10:00.000000 sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 07:10:00.000000 sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 07:10:00.000000 sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/top_level.txt
```

### Comparing `sebchw_example_package-0.2.2/LICENSE` & `sebchw_example_package-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sebchw_example_package-0.2.2/PKG-INFO` & `sebchw_example_package-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sebchw_example_package
-Version: 0.2.2
+Version: 0.3.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sebchw_example_package-0.2.2/pyproject.toml` & `sebchw_example_package-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sebchw_example_package"
-version = "0.2.2"
+version = "0.3.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sebchw_example_package-0.2.2/src/sebchw_example_package.egg-info/PKG-INFO` & `sebchw_example_package-0.3.2/src/sebchw_example_package.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sebchw_example_package
-Version: 0.2.2
+Version: 0.3.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

