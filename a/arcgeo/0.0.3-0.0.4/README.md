# Comparing `tmp/arcgeo-0.0.3.tar.gz` & `tmp/arcgeo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcgeo-0.0.3.tar", last modified: Thu Feb 29 05:57:57 2024, max compression
+gzip compressed data, was "arcgeo-0.0.4.tar", last modified: Thu Apr 18 04:18:07 2024, max compression
```

## Comparing `arcgeo-0.0.3.tar` & `arcgeo-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.654254 arcgeo-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.654254 arcgeo-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.658254 arcgeo-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-29 05:57:43.000000 arcgeo-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 05:57:43.000000 arcgeo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-29 05:57:43.000000 arcgeo-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-29 05:57:57.662254 arcgeo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-29 05:57:43.000000 arcgeo-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.658254 arcgeo-0.0.3/arcgeo/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-29 05:57:43.000000 arcgeo-0.0.3/arcgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-29 05:57:43.000000 arcgeo-0.0.3/arcgeo/arcgeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-29 05:57:43.000000 arcgeo-0.0.3/arcgeo/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/arcgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 05:57:57.000000 arcgeo-0.0.3/arcgeo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.658254 arcgeo-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/docs/Lab4/
--rw-r--r--   0 runner    (1001) docker     (127)    27573 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/Lab4/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/arcgeo.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-29 05:57:43.000000 arcgeo-0.0.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-29 05:57:43.000000 arcgeo-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-29 05:57:43.000000 arcgeo-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 05:57:43.000000 arcgeo-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-29 05:57:43.000000 arcgeo-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 05:57:57.662254 arcgeo-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 05:57:57.662254 arcgeo-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-29 05:57:43.000000 arcgeo-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-29 05:57:43.000000 arcgeo-0.0.3/tests/test_arcgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.654445 arcgeo-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.658445 arcgeo-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.658445 arcgeo-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 04:17:57.000000 arcgeo-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 04:17:57.000000 arcgeo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 04:17:57.000000 arcgeo-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 04:18:07.662445 arcgeo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 04:17:57.000000 arcgeo-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.658445 arcgeo-0.0.4/arcgeo/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 04:17:57.000000 arcgeo-0.0.4/arcgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-18 04:17:57.000000 arcgeo-0.0.4/arcgeo/arcgeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 04:17:57.000000 arcgeo-0.0.4/arcgeo/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/arcgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 04:18:07.000000 arcgeo-0.0.4/arcgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 04:17:57.000000 arcgeo-0.0.4/cats.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/arcgeo.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/examples/lab9.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/examples/practice.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 04:17:57.000000 arcgeo-0.0.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-18 04:17:57.000000 arcgeo-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-18 04:17:57.000000 arcgeo-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 04:17:57.000000 arcgeo-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-18 04:17:57.000000 arcgeo-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 04:18:07.662445 arcgeo-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:18:07.662445 arcgeo-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 04:17:57.000000 arcgeo-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 04:17:57.000000 arcgeo-0.0.4/tests/test_arcgeo.py
```

### Comparing `arcgeo-0.0.3/.github/workflows/docs-build.yml` & `arcgeo-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/docs.yml` & `arcgeo-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/installation.yml` & `arcgeo-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/macos.yml` & `arcgeo-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/pypi.yml` & `arcgeo-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/ubuntu.yml` & `arcgeo-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.github/workflows/windows.yml` & `arcgeo-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/.gitignore` & `arcgeo-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/PKG-INFO` & `arcgeo-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcgeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Just a practice repo
 Author-email: Shabiha Hossain <sabihahossain4105@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Omiimo05/arcgeo
 Keywords: arcgeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipyleaflet
 Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyshp
+Requires-Dist: geopandas
+Requires-Dist: localtileserver
 Provides-Extra: all
 Requires-Dist: arcgeo[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # arcgeo
```

### Comparing `arcgeo-0.0.3/arcgeo.egg-info/PKG-INFO` & `arcgeo-0.0.4/arcgeo.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcgeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Just a practice repo
 Author-email: Shabiha Hossain <sabihahossain4105@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Omiimo05/arcgeo
 Keywords: arcgeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipyleaflet
 Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyshp
+Requires-Dist: geopandas
+Requires-Dist: localtileserver
 Provides-Extra: all
 Requires-Dist: arcgeo[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # arcgeo
```

### Comparing `arcgeo-0.0.3/arcgeo.egg-info/SOURCES.txt` & `arcgeo-0.0.4/arcgeo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .editorconfig
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
+cats.txt
 mkdocs.yml
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
@@ -30,12 +31,13 @@
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/usage.md
-docs/Lab4/lab4.ipynb
 docs/examples/intro.ipynb
+docs/examples/lab9.ipynb
+docs/examples/practice.ipynb
 docs/overrides/main.html
 tests/__init__.py
 tests/test_arcgeo.py
```

### Comparing `arcgeo-0.0.3/docs/contributing.md` & `arcgeo-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/docs/installation.md` & `arcgeo-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `arcgeo-0.0.3/mkdocs.yml` & `arcgeo-0.0.4/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -43,18 +43,18 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: True
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["*ignore.ipynb"]
+          execute_ignore: ["*ignore.ipynb", "lab9.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -77,10 +77,14 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Omiimo05/arcgeo/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/lab9.ipynb
+    - Labs:
+        - Labs/lab4.ipynb
+        - Labs/lab5.ipynb
     - API Reference:
           - arcgeo module: arcgeo.md
           - common module: common.md
```

### Comparing `arcgeo-0.0.3/pyproject.toml` & `arcgeo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arcgeo"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "Just a practice repo"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

