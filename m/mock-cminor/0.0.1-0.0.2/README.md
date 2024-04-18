# Comparing `tmp/mock_cminor-0.0.1.tar.gz` & `tmp/mock_cminor-0.0.2.tar.gz`

## Comparing `mock_cminor-0.0.1.tar` & `mock_cminor-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/setup.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/__version__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/adaptor.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/analyzers.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/generator.py
--rw-r--r--   0        0        0  1828815 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/src/mock_cminor/src/get_results.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/LICENCE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/README.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 mock_cminor-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/__version__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/adaptor.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/analyzers.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/generator.py
+-rw-r--r--   0        0        0  1828815 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/src/mock_cminor/get_results.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/LICENCE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/README.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 mock_cminor-0.0.2/PKG-INFO
```

### Comparing `mock_cminor-0.0.1/src/mock_cminor/src/analyzers.py` & `mock_cminor-0.0.2/src/mock_cminor/analyzers.py`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.1/src/mock_cminor/src/generator.py` & `mock_cminor-0.0.2/src/mock_cminor/generator.py`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.1/src/mock_cminor/src/get_results.py` & `mock_cminor-0.0.2/src/mock_cminor/get_results.py`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.1/LICENCE` & `mock_cminor-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.1/README.md` & `mock_cminor-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mock_cminor-0.0.1/pyproject.toml` & `mock_cminor-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mock-cminor"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Cathoven A.I", email="contact@cathoven.com" },
 ]
 description = "Mocking library for Cminor"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mock_cminor-0.0.1/PKG-INFO` & `mock_cminor-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mock-cminor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mocking library for Cminor
 Project-URL: Homepage, https://github.com/yunusarli/cminor
 Project-URL: Issues, https://github.com/yunusarli/cminor/issues
 Author-email: "Cathoven A.I" <contact@cathoven.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

