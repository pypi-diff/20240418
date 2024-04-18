# Comparing `tmp/qaml-0.0.7.4.tar.gz` & `tmp/qaml-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.4.tar", last modified: Wed Apr 17 23:41:45 2024, max compression
+gzip compressed data, was "qaml-0.0.7.5.tar", last modified: Wed Apr 17 23:48:34 2024, max compression
```

## Comparing `qaml-0.0.7.4.tar` & `qaml-0.0.7.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.474450 qaml-0.0.7.4/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.4/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:41:45.474307 qaml-0.0.7.4/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.4/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 23:39:59.000000 qaml-0.0.7.4/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.473456 qaml-0.0.7.4/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.4/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.4/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13559 2024-04-17 23:39:26.000000 qaml-0.0.7.4/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.474156 qaml-0.0.7.4/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 23:41:45.474481 qaml-0.0.7.4/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.220499 qaml-0.0.7.5/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.5/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:48:34.220336 qaml-0.0.7.5/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.5/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 23:48:31.000000 qaml-0.0.7.5/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.219390 qaml-0.0.7.5/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.5/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.5/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13590 2024-04-17 23:47:00.000000 qaml-0.0.7.5/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.220182 qaml-0.0.7.5/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 23:48:34.220529 qaml-0.0.7.5/setup.cfg
```

### Comparing `qaml-0.0.7.4/LICENSE` & `qaml-0.0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.4/PKG-INFO` & `qaml-0.0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.4/README.md` & `qaml-0.0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.4/pyproject.toml` & `qaml-0.0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.4"
+version = "0.0.7.5"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.4/qaml/__main__.py` & `qaml-0.0.7.5/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.4/qaml/client.py` & `qaml-0.0.7.5/qaml/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
     if driver is not None:
         platform_name = driver.capabilities.get("platformName").lower()
         if platform_name == 'android':
             print("Using the provided Appium driver for Android.")
             return AndroidClient(api_key, driver=driver)
         elif platform_name == 'ios':
             print("Using the provided Appium driver for iOS.")
-            return IOSClient(api_key, driver=driver)
+            return IOSClient(api_key, driver=driver, use_hid_typing=use_hid_typing)
         else:
             raise Exception("Unsupported platform specified in the provided driver's capabilities.")
 
     android_devices = get_connected_android_devices()
     if android_devices:
         return AndroidClient(api_key)
```

### Comparing `qaml-0.0.7.4/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.5/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

