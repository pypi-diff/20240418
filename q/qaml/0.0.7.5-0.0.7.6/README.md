# Comparing `tmp/qaml-0.0.7.5.tar.gz` & `tmp/qaml-0.0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.5.tar", last modified: Wed Apr 17 23:48:34 2024, max compression
+gzip compressed data, was "qaml-0.0.7.6.tar", last modified: Thu Apr 18 00:06:43 2024, max compression
```

## Comparing `qaml-0.0.7.5.tar` & `qaml-0.0.7.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.220499 qaml-0.0.7.5/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.5/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:48:34.220336 qaml-0.0.7.5/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.5/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 23:48:31.000000 qaml-0.0.7.5/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.219390 qaml-0.0.7.5/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.5/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.5/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13590 2024-04-17 23:47:00.000000 qaml-0.0.7.5/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:48:34.220182 qaml-0.0.7.5/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 23:48:34.000000 qaml-0.0.7.5/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 23:48:34.220529 qaml-0.0.7.5/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.371058 qaml-0.0.7.6/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.6/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 00:06:43.370918 qaml-0.0.7.6/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.6/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 00:06:40.000000 qaml-0.0.7.6/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.370067 qaml-0.0.7.6/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.6/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.6/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13116 2024-04-18 00:06:01.000000 qaml-0.0.7.6/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.370767 qaml-0.0.7.6/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 00:06:43.371088 qaml-0.0.7.6/setup.cfg
```

### Comparing `qaml-0.0.7.5/LICENSE` & `qaml-0.0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.5/PKG-INFO` & `qaml-0.0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.5
+Version: 0.0.7.6
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.5/README.md` & `qaml-0.0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.5/pyproject.toml` & `qaml-0.0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.5"
+version = "0.0.7.6"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.5/qaml/__main__.py` & `qaml-0.0.7.6/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.5/qaml/client.py` & `qaml-0.0.7.6/qaml/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,15 +240,14 @@
         else:
             try:
                 self.driver.find_element(AppiumBy.IOS_PREDICATE, "type == 'XCUIElementTypeApplication'").send_keys(text)
             except:
                 self.type_text_hid(text)
 
     def type_text_hid(self, text):
-        # HID usage mappings for special characters and numbers
         special_chars = {
                 ' ': 0x2C, '!': 0x1E, '@': 0x1F, '#': 0x20, '$': 0x21, '%': 0x22,
                 '^': 0x23, '&': 0x24, '*': 0x25, '(': 0x26, ')': 0x27, '-': 0x2D,
                 '_': 0x2D, '=': 0x2E, '+': 0x2E, '[': 0x2F, '{': 0x2F, ']': 0x30,
                 '}': 0x30, '\\': 0x31, '|': 0x31, ';': 0x33, ':': 0x33, '\'': 0x34,
                 '"': 0x34, '`': 0x35, '~': 0x35, ',': 0x36, '<': 0x36, '.': 0x37,
                 '>': 0x37, '/': 0x38, '?': 0x38
@@ -274,23 +273,18 @@
                 usage = 0x27
             elif char in special_chars:
                 usage = special_chars[char]
                 # Determine if shift needs to be pressed for special characters
                 shift = char in '~!@#$%^&*()_+{}|:"<>?'
 
             if usage is None:
-                continue  # Skip unsupported characters
+                continue
 
-            # Press and release the shift key if necessary
-            if shift:
-                self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0xE1, "durationSeconds": 0.1})  # Shift down
-            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.1})  # Key down
-            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.1})  # Key up
-            if shift:
-                self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0xE1, "durationSeconds": 0.1})  # Shift up
+            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.005})  # Key down
+            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.005})  # Key up
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
 def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
     def get_ios_udid():
         system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
```

### Comparing `qaml-0.0.7.5/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.6/qaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.5
+Version: 0.0.7.6
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

