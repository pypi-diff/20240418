# Comparing `tmp/a9x_webstatistics_package-0.1.1.tar.gz` & `tmp/a9x_webstatistics_package-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics_package-0.1.1.tar", last modified: Tue Apr 16 19:48:30 2024, max compression
+gzip compressed data, was "a9x_webstatistics_package-0.1.2.tar", last modified: Thu Apr 18 15:01:36 2024, max compression
```

## Comparing `a9x_webstatistics_package-0.1.1.tar` & `a9x_webstatistics_package-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 19:48:30.051869 a9x_webstatistics_package-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 19:48:30.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.323001 a9x_webstatistics_package-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.323001 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 15:01:36.000000 a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:01:36.327001 a9x_webstatistics_package-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 15:01:25.000000 a9x_webstatistics_package-0.1.2/tests/test_module1.py
```

### Comparing `a9x_webstatistics_package-0.1.1/LICENSE` & `a9x_webstatistics_package-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.1/PKG-INFO` & `a9x_webstatistics_package-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics_package
-Version: 0.1.1
+Version: 0.1.2
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
 Keywords: webstats,statistics,analytics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
@@ -287,9 +286,7 @@
 
 - [Python Packaging Authority (PyPA)'s sample project](https://github.com/pypa/sampleproject)
 - [PyPA's Python Packaging User Guide](https://packaging.python.org/tutorials/packaging-projects/)
 - [Stackoverflow questions and answers](https://stackoverflow.com/questions/41093648/how-to-test-that-pypi-install-will-work-before-pushing-to-pypi-python)
 - [GitHub Actions Guides: Building and testing Python](https://docs.github.com/en/free-pro-team@latest/actions/guides/building-and-testing-python)
 
 Btw, if you want to publish TypeScript (JavaScript) package to the npm registry, go to [Example TypeScript Package ready to be published on npm for 2021](https://github.com/tomchen/example-typescript-package).
-
-
```

### Comparing `a9x_webstatistics_package-0.1.1/README.md` & `a9x_webstatistics_package-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.1/setup.py` & `a9x_webstatistics_package-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/PKG-INFO` & `a9x_webstatistics_package-0.1.2/src/a9x_webstatistics_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
-Name: a9x-webstatistics-package
-Version: 0.1.1
+Name: a9x_webstatistics_package
+Version: 0.1.2
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
 Keywords: webstats,statistics,analytics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
@@ -287,9 +286,7 @@
 
 - [Python Packaging Authority (PyPA)'s sample project](https://github.com/pypa/sampleproject)
 - [PyPA's Python Packaging User Guide](https://packaging.python.org/tutorials/packaging-projects/)
 - [Stackoverflow questions and answers](https://stackoverflow.com/questions/41093648/how-to-test-that-pypi-install-will-work-before-pushing-to-pypi-python)
 - [GitHub Actions Guides: Building and testing Python](https://docs.github.com/en/free-pro-team@latest/actions/guides/building-and-testing-python)
 
 Btw, if you want to publish TypeScript (JavaScript) package to the npm registry, go to [Example TypeScript Package ready to be published on npm for 2021](https://github.com/tomchen/example-typescript-package).
-
-
```

