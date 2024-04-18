# Comparing `tmp/myarg-1.0.0.tar.gz` & `tmp/myarg-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myarg-1.0.0.tar", last modified: Thu Apr 18 02:08:18 2024, max compression
+gzip compressed data, was "myarg-2.0.0.tar", last modified: Thu Apr 18 02:08:03 2024, max compression
```

## Comparing `myarg-1.0.0.tar` & `myarg-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:18.390878 myarg-1.0.0/
--rw-rw-rw-   0        0        0     1138 2024-04-18 02:08:18.390878 myarg-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:18.390383 myarg-1.0.0/myarg.egg-info/
--rw-rw-rw-   0        0        0     1138 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:08:18.000000 myarg-1.0.0/myarg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 02:08:18.391378 myarg-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     8688 2024-04-18 02:08:16.000000 myarg-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:08:03.937714 myarg-2.0.0/
+-rw-rw-rw-   0        0        0     1138 2024-04-18 02:08:03.937205 myarg-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 02:08:03.936194 myarg-2.0.0/myarg.egg-info/
+-rw-rw-rw-   0        0        0     1138 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:08:03.000000 myarg-2.0.0/myarg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:08:03.937714 myarg-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     8688 2024-04-18 02:08:02.000000 myarg-2.0.0/setup.py
```

### Comparing `myarg-1.0.0/PKG-INFO` & `myarg-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myarg
-Version: 1.0.0
+Version: 2.0.0
 Summary: A sample Python project
 Home-page: https://github.com/pypa/myarg
 Author: A. Random Developer
 Author-email: 15732692001@163.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/pypa/myarg/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `myarg-1.0.0/myarg.egg-info/PKG-INFO` & `myarg-2.0.0/myarg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myarg
-Version: 1.0.0
+Version: 2.0.0
 Summary: A sample Python project
 Home-page: https://github.com/pypa/myarg
 Author: A. Random Developer
 Author-email: 15732692001@163.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/pypa/myarg/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `myarg-1.0.0/setup.py` & `myarg-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="myarg",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.0",  # Required
+    version="2.0.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A sample Python project",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

