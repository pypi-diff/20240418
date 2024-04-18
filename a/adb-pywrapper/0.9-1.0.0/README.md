# Comparing `tmp/adb-pywrapper-0.9.tar.gz` & `tmp/adb_pywrapper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb-pywrapper-0.9.tar", last modified: Wed Apr 10 09:18:48 2024, max compression
+gzip compressed data, was "adb_pywrapper-1.0.0.tar", last modified: Thu Apr 18 07:26:28 2024, max compression
```

## Comparing `adb-pywrapper-0.9.tar` & `adb_pywrapper-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:18:48.547591 adb-pywrapper-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-04-10 09:18:44.000000 adb-pywrapper-0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-10 09:18:48.543591 adb-pywrapper-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-10 09:18:44.000000 adb-pywrapper-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-10 09:18:44.000000 adb-pywrapper-0.9/adb_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:18:48.543591 adb-pywrapper-0.9/adb_pywrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-10 09:18:48.000000 adb-pywrapper-0.9/adb_pywrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 09:18:48.000000 adb-pywrapper-0.9/adb_pywrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:18:48.000000 adb-pywrapper-0.9/adb_pywrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 09:18:48.000000 adb-pywrapper-0.9/adb_pywrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:18:48.547591 adb-pywrapper-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-10 09:18:44.000000 adb-pywrapper-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:26:28.644799 adb_pywrapper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-04-18 07:26:25.000000 adb_pywrapper-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-18 07:26:28.644799 adb_pywrapper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-18 07:26:25.000000 adb_pywrapper-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-18 07:26:25.000000 adb_pywrapper-1.0.0/adb_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:26:28.644799 adb_pywrapper-1.0.0/adb_pywrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-18 07:26:28.000000 adb_pywrapper-1.0.0/adb_pywrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-18 07:26:28.000000 adb_pywrapper-1.0.0/adb_pywrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:26:28.000000 adb_pywrapper-1.0.0/adb_pywrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 07:26:28.000000 adb_pywrapper-1.0.0/adb_pywrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:26:28.644799 adb_pywrapper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 07:26:25.000000 adb_pywrapper-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:26:28.644799 adb_pywrapper-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    20148 2024-04-18 07:26:25.000000 adb_pywrapper-1.0.0/test/test_adb_pywrapper.py
```

### Comparing `adb-pywrapper-0.9/LICENSE.txt` & `adb_pywrapper-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adb-pywrapper-0.9/PKG-INFO` & `adb_pywrapper-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-pywrapper
-Version: 0.9
+Version: 1.0.0
 Summary: adb-pywrapper facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) directly within Python scripts.
 Home-page: https://github.com/NetherlandsForensicInstitute/adb-pywrapper
 Author: Netherlands Forensic Institute
 Author-email: netherlandsforensicinstitute@users.noreply.github.com
 License: EUPL-1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 ## AdbDevice: Interacting with Android Devices using ADB in Python
 
 The `AdbDevice` class in the `adb-pywrapper` Python package facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) directly within Python scripts.
 
 Installation
 ------------
 
-To install the `adb-pywrapper` package from the internal nexus pipy server, you can use `pip`:
+To install the `adb-pywrapper` package from the internal Nexus PyPI server, you can use `pip`:
 
 ```bash
 pip install adb-pywrapper
 ```
 
 Before using `adb-pywrapper`, ensure that ADB is installed on your machine and added to PATH. You can download and install the Android SDK, which includes ADB, from the official Android developer website.
 
@@ -203,8 +203,8 @@
 * snapshot_save(snapshot_name)  
 * snapshot_delete(delete=None)  
 
 ## Error Handling
 Be sure to handle errors gracefully in your code, as various operations may fail, adb-pywrapper tries to provide information where possible on success or failure in the `AdbResult` and `PullResult` objects.
 
 ## Contributing
-Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR.
+Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR. Find our contribution guidelines [here](CONTRIBUTING.md).
```

### Comparing `adb-pywrapper-0.9/README.md` & `adb_pywrapper-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## AdbDevice: Interacting with Android Devices using ADB in Python
 
 The `AdbDevice` class in the `adb-pywrapper` Python package facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) directly within Python scripts.
 
 Installation
 ------------
 
-To install the `adb-pywrapper` package from the internal nexus pipy server, you can use `pip`:
+To install the `adb-pywrapper` package from the internal Nexus PyPI server, you can use `pip`:
 
 ```bash
 pip install adb-pywrapper
 ```
 
 Before using `adb-pywrapper`, ensure that ADB is installed on your machine and added to PATH. You can download and install the Android SDK, which includes ADB, from the official Android developer website.
 
@@ -192,8 +192,8 @@
 * snapshot_save(snapshot_name)  
 * snapshot_delete(delete=None)  
 
 ## Error Handling
 Be sure to handle errors gracefully in your code, as various operations may fail, adb-pywrapper tries to provide information where possible on success or failure in the `AdbResult` and `PullResult` objects.
 
 ## Contributing
-Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR.
+Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR. Find our contribution guidelines [here](CONTRIBUTING.md).
```

### Comparing `adb-pywrapper-0.9/adb_init.py` & `adb_pywrapper-1.0.0/adb_init.py`

 * *Files identical despite different names*

### Comparing `adb-pywrapper-0.9/adb_pywrapper.egg-info/PKG-INFO` & `adb_pywrapper-1.0.0/adb_pywrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-pywrapper
-Version: 0.9
+Version: 1.0.0
 Summary: adb-pywrapper facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) directly within Python scripts.
 Home-page: https://github.com/NetherlandsForensicInstitute/adb-pywrapper
 Author: Netherlands Forensic Institute
 Author-email: netherlandsforensicinstitute@users.noreply.github.com
 License: EUPL-1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 ## AdbDevice: Interacting with Android Devices using ADB in Python
 
 The `AdbDevice` class in the `adb-pywrapper` Python package facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) directly within Python scripts.
 
 Installation
 ------------
 
-To install the `adb-pywrapper` package from the internal nexus pipy server, you can use `pip`:
+To install the `adb-pywrapper` package from the internal Nexus PyPI server, you can use `pip`:
 
 ```bash
 pip install adb-pywrapper
 ```
 
 Before using `adb-pywrapper`, ensure that ADB is installed on your machine and added to PATH. You can download and install the Android SDK, which includes ADB, from the official Android developer website.
 
@@ -203,8 +203,8 @@
 * snapshot_save(snapshot_name)  
 * snapshot_delete(delete=None)  
 
 ## Error Handling
 Be sure to handle errors gracefully in your code, as various operations may fail, adb-pywrapper tries to provide information where possible on success or failure in the `AdbResult` and `PullResult` objects.
 
 ## Contributing
-Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR.
+Contributions to the adb-pywrapper package are welcome. If you encounter any issues, have suggestions, or want to contribute, feel free to open an issue or PR. Find our contribution guidelines [here](CONTRIBUTING.md).
```

### Comparing `adb-pywrapper-0.9/setup.py` & `adb_pywrapper-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="adb-pywrapper",
-    version="0.9",
+    version="1.0.0",
     description="adb-pywrapper facilitates seamless interaction with Android devices using the Android Debug Bridge (ADB) "
                 "directly within Python scripts.",
     long_description=f"{open('README.md').read()}",
     long_description_content_type="text/markdown",
     author="Netherlands Forensic Institute",
     author_email="netherlandsforensicinstitute@users.noreply.github.com",
     url="https://github.com/NetherlandsForensicInstitute/adb-pywrapper",
```

