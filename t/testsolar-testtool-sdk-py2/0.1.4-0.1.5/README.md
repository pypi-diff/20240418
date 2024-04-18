# Comparing `tmp/testsolar-testtool-sdk-py2-0.1.4.tar.gz` & `tmp/testsolar-testtool-sdk-py2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.4.tar", last modified: Wed Apr 17 02:27:49 2024, max compression
+gzip compressed data, was "dist/testsolar-testtool-sdk-py2-0.1.5.tar", last modified: Thu Apr 18 10:58:02 2024, max compression
```

## Comparing `testsolar-testtool-sdk-py2-0.1.4.tar` & `testsolar-testtool-sdk-py2-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2327 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/
--rw-r--r--   0 root         (0) root         (0)      443 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2894 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/tests/test_testresult.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/tests/test_param.py
--rw-r--r--   0 root         (0) root         (0)     5965 2024-04-17 02:27:42.000000 testsolar-testtool-sdk-py2-0.1.4/tests/test_report.py
--rw-r--r--   0 root         (0) root         (0)      581 2024-04-17 02:27:49.000000 testsolar-testtool-sdk-py2-0.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/
+-rw-r--r--   0 root         (0) root         (0)     2327 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/reporter.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/pipe_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 root         (0) root         (0)      443 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/decoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/tests/test_param.py
+-rw-r--r--   0 root         (0) root         (0)      219 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/tests/test_decoder.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5965 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-04-18 10:57:56.000000 testsolar-testtool-sdk-py2-0.1.5/tests/test_testresult.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      714 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-18 10:58:02.000000 testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/requires.txt
```

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 setup.py
 tests/__init__.py
+tests/test_decoder.py
 tests/test_param.py
 tests/test_report.py
 tests/test_testresult.py
 testsolar_testtool_sdk/__init__.py
+testsolar_testtool_sdk/decoder.py
 testsolar_testtool_sdk/pipe_reader.py
 testsolar_testtool_sdk/reporter.py
 testsolar_testtool_sdk/model/__init__.py
 testsolar_testtool_sdk/model/encoder.py
 testsolar_testtool_sdk/model/load.py
 testsolar_testtool_sdk/model/param.py
 testsolar_testtool_sdk/model/testresult.py
```

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk_py2.egg-info/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

### Comparing `testsolar-testtool-sdk-py2-0.1.4/setup.py` & `testsolar-testtool-sdk-py2-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(req_file, 'r') as f:
         install_requires = [str(req) for req in parse_requirements(f)]
         return install_requires
 
 
 setup(
     name='testsolar-testtool-sdk-py2',
-    version='0.1.4',
+    version='0.1.5',
     author='asiazhang',
     author_email='asiazhang2002@gmail.com',
     description='Python2 SDK for TestSolar testtool',
     url='https://github.com/OpenTestSolar/testtool-sdk-python-py2',
     packages=find_packages(),
     python_requires='>=2.7, <3',
     classifiers=[
```

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/param.py` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/param.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/testsolar_testtool_sdk/model/encoder.py` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk/model/encoder.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/tests/test_testresult.py` & `testsolar-testtool-sdk-py2-0.1.5/tests/test_testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/tests/test_report.py` & `testsolar-testtool-sdk-py2-0.1.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-py2-0.1.4/PKG-INFO` & `testsolar-testtool-sdk-py2-0.1.5/testsolar_testtool_sdk_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: testsolar-testtool-sdk-py2
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python2 SDK for TestSolar testtool
 Home-page: https://github.com/OpenTestSolar/testtool-sdk-python-py2
 Author: asiazhang
 Author-email: asiazhang2002@gmail.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: testsolar
```

