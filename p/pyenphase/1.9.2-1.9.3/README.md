# Comparing `tmp/pyenphase-1.9.2.tar.gz` & `tmp/pyenphase-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.9.2.tar", max compression
+gzip compressed data, was "pyenphase-1.9.3.tar", max compression
```

## Comparing `pyenphase-1.9.2.tar` & `pyenphase-1.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1067 2023-09-07 01:02:54.448800 pyenphase-1.9.2/LICENSE
--rw-r--r--   0        0        0     3476 2023-09-07 01:02:54.448800 pyenphase-1.9.2/README.md
--rw-r--r--   0        0        0     2376 2023-09-07 01:02:55.512862 pyenphase-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     1338 2023-09-07 01:02:55.480860 pyenphase-1.9.2/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8363 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/auth.py
--rw-r--r--   0        0        0     1459 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/const.py
--rw-r--r--   0        0        0    12924 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1386 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     3310 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/firmware.py
--rw-r--r--   0        0        0      413 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/json.py
--rw-r--r--   0        0        0        0 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     3407 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     3624 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2000 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1335 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/ssl.py
--rw-r--r--   0        0        0        0 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/__init__.py
--rw-r--r--   0        0        0     1451 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/api_v1_production.py
--rw-r--r--   0        0        0     1777 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/api_v1_production_inverters.py
--rw-r--r--   0        0        0     1583 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/base.py
--rw-r--r--   0        0        0     4917 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/ensemble.py
--rw-r--r--   0        0        0     3216 2023-09-07 01:02:54.452800 pyenphase-1.9.2/src/pyenphase/updaters/production.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-09-07 02:05:02.694677 pyenphase-1.9.3/LICENSE
+-rw-r--r--   0        0        0     3476 2023-09-07 02:05:02.694677 pyenphase-1.9.3/README.md
+-rw-r--r--   0        0        0     2376 2023-09-07 02:05:03.646690 pyenphase-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1338 2023-09-07 02:05:03.606690 pyenphase-1.9.3/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8363 2023-09-07 02:05:02.694677 pyenphase-1.9.3/src/pyenphase/auth.py
+-rw-r--r--   0        0        0     1459 2023-09-07 02:05:02.694677 pyenphase-1.9.3/src/pyenphase/const.py
+-rw-r--r--   0        0        0    12924 2023-09-07 02:05:02.694677 pyenphase-1.9.3/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1386 2023-09-07 02:05:02.694677 pyenphase-1.9.3/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     3310 2023-09-07 02:05:02.694677 pyenphase-1.9.3/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0      413 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/json.py
+-rw-r--r--   0        0        0        0 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     3407 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     3624 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2000 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1335 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0        0 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/__init__.py
+-rw-r--r--   0        0        0     1451 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/api_v1_production.py
+-rw-r--r--   0        0        0     1777 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/api_v1_production_inverters.py
+-rw-r--r--   0        0        0     1583 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/base.py
+-rw-r--r--   0        0        0     4917 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/ensemble.py
+-rw-r--r--   0        0        0     3832 2023-09-07 02:05:02.698677 pyenphase-1.9.3/src/pyenphase/updaters/production.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.9.3/PKG-INFO
```

### Comparing `pyenphase-1.9.2/LICENSE` & `pyenphase-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/README.md` & `pyenphase-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/pyproject.toml` & `pyenphase-1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.9.2"
+version = "1.9.3"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.9.2/src/pyenphase/__init__.py` & `pyenphase-1.9.3/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/auth.py` & `pyenphase-1.9.3/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/const.py` & `pyenphase-1.9.3/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/envoy.py` & `pyenphase-1.9.3/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/exceptions.py` & `pyenphase-1.9.3/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/firmware.py` & `pyenphase-1.9.3/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.9.3/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/encharge.py` & `pyenphase-1.9.3/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/enpower.py` & `pyenphase-1.9.3/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/envoy.py` & `pyenphase-1.9.3/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/inverter.py` & `pyenphase-1.9.3/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/system_consumption.py` & `pyenphase-1.9.3/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/models/system_production.py` & `pyenphase-1.9.3/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/ssl.py` & `pyenphase-1.9.3/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/updaters/api_v1_production.py` & `pyenphase-1.9.3/src/pyenphase/updaters/api_v1_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/updaters/api_v1_production_inverters.py` & `pyenphase-1.9.3/src/pyenphase/updaters/api_v1_production_inverters.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/updaters/base.py` & `pyenphase-1.9.3/src/pyenphase/updaters/base.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/src/pyenphase/updaters/ensemble.py` & `pyenphase-1.9.3/src/pyenphase/updaters/ensemble.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.9.2/PKG-INFO` & `pyenphase-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.9.2
+Version: 1.9.3
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 1.9.2 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.9.3 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

