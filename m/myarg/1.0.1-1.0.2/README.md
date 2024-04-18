# Comparing `tmp/myarg-1.0.1.tar.gz` & `tmp/myarg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myarg-1.0.1.tar", last modified: Thu Apr 18 03:21:48 2024, max compression
+gzip compressed data, was "myarg-1.0.2.tar", last modified: Thu Apr 18 03:27:40 2024, max compression
```

## Comparing `myarg-1.0.1.tar` & `myarg-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:21:48.780027 myarg-1.0.1/
--rw-rw-rw-   0        0        0     1138 2024-04-18 03:21:48.779565 myarg-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:21:48.779064 myarg-1.0.1/myarg.egg-info/
--rw-rw-rw-   0        0        0     1138 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:21:48.000000 myarg-1.0.1/myarg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 03:21:48.780027 myarg-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     8688 2024-04-18 03:21:40.000000 myarg-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 03:27:40.782010 myarg-1.0.2/
+-rw-rw-rw-   0        0        0     1138 2024-04-18 03:27:40.782010 myarg-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-18 02:02:21.000000 myarg-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 03:27:40.781511 myarg-1.0.2/myarg.egg-info/
+-rw-rw-rw-   0        0        0     1138 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 03:27:40.000000 myarg-1.0.2/myarg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 03:27:40.782010 myarg-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     8690 2024-04-18 03:27:36.000000 myarg-1.0.2/setup.py
```

### Comparing `myarg-1.0.1/PKG-INFO` & `myarg-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myarg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A sample Python project
 Home-page: https://github.com/pypa/myarg
 Author: A. Random Developer
 Author-email: 15732692001@163.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/pypa/myarg/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `myarg-1.0.1/myarg.egg-info/PKG-INFO` & `myarg-1.0.2/myarg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myarg
-Version: 1.0.1
+Version: 1.0.2
 Summary: A sample Python project
 Home-page: https://github.com/pypa/myarg
 Author: A. Random Developer
 Author-email: 15732692001@163.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/pypa/myarg/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `myarg-1.0.1/setup.py` & `myarg-1.0.2/setup.py`

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
-    version="1.0.1",  # Required
+    version="1.0.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A sample Python project",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -146,15 +146,15 @@
         "sample": ["package_data.dat"],
     },
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    data_files=[("my_data", ["data/data_file"])],  # Optional
+    # data_files=[("my_data", ["data/data_file"])],  # Optional
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
```

