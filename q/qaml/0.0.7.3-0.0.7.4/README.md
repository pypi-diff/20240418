# Comparing `tmp/qaml-0.0.7.3.tar.gz` & `tmp/qaml-0.0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.3.tar", last modified: Wed Apr 17 18:36:16 2024, max compression
+gzip compressed data, was "qaml-0.0.7.4.tar", last modified: Wed Apr 17 23:41:45 2024, max compression
```

## Comparing `qaml-0.0.7.3.tar` & `qaml-0.0.7.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.692478 qaml-0.0.7.3/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.3/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 18:36:16.692332 qaml-0.0.7.3/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.3/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 18:36:06.000000 qaml-0.0.7.3/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.691480 qaml-0.0.7.3/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.3/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.3/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    11051 2024-04-17 18:31:00.000000 qaml-0.0.7.3/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.692184 qaml-0.0.7.3/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 18:36:16.692509 qaml-0.0.7.3/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.474450 qaml-0.0.7.4/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.4/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:41:45.474307 qaml-0.0.7.4/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.4/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 23:39:59.000000 qaml-0.0.7.4/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.473456 qaml-0.0.7.4/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.4/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.4/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13559 2024-04-17 23:39:26.000000 qaml-0.0.7.4/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 23:41:45.474156 qaml-0.0.7.4/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 23:41:45.000000 qaml-0.0.7.4/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 23:41:45.474481 qaml-0.0.7.4/setup.cfg
```

### Comparing `qaml-0.0.7.3/LICENSE` & `qaml-0.0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.3/PKG-INFO` & `qaml-0.0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.3/README.md` & `qaml-0.0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.3/pyproject.toml` & `qaml-0.0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.3"
+version = "0.0.7.4"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.3/qaml/__main__.py` & `qaml-0.0.7.4/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.3/qaml/client.py` & `qaml-0.0.7.4/qaml/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -170,18 +170,19 @@
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
         subprocess.run(["adb", "shell", "input", "text", f"'{text}'"])
 
 class IOSClient(BaseClient):
-    def __init__(self, api_key, driver=None, ios_udid=None, use_mjpeg=True):
+    def __init__(self, api_key, driver=None, ios_udid=None, use_mjpeg=True, use_hid_typing=False):
         super().__init__(api_key)
         self.platform = "iOS"
         self.use_mjpeg = use_mjpeg
+        self.use_hid_typing = use_hid_typing
         if driver:
             self.driver = driver
         else:
             # try 3 times to setup the driver
             for _ in range(3):
                 try:
                     self.setup_driver(ios_udid)
@@ -230,20 +231,71 @@
         self.driver.execute_script("mobile: swipe", {"direction": direction})
 
     def scroll(self, direction):
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.driver.execute_script("mobile: swipe", {"direction": direction_map[direction]})
 
     def type_text(self, text):
-        self.driver.find_element(AppiumBy.IOS_PREDICATE, "type == 'XCUIElementTypeApplication'").send_keys(text)
+        if self.use_hid_typing:
+            self.type_text_hid(text)
+        else:
+            try:
+                self.driver.find_element(AppiumBy.IOS_PREDICATE, "type == 'XCUIElementTypeApplication'").send_keys(text)
+            except:
+                self.type_text_hid(text)
+
+    def type_text_hid(self, text):
+        # HID usage mappings for special characters and numbers
+        special_chars = {
+                ' ': 0x2C, '!': 0x1E, '@': 0x1F, '#': 0x20, '$': 0x21, '%': 0x22,
+                '^': 0x23, '&': 0x24, '*': 0x25, '(': 0x26, ')': 0x27, '-': 0x2D,
+                '_': 0x2D, '=': 0x2E, '+': 0x2E, '[': 0x2F, '{': 0x2F, ']': 0x30,
+                '}': 0x30, '\\': 0x31, '|': 0x31, ';': 0x33, ':': 0x33, '\'': 0x34,
+                '"': 0x34, '`': 0x35, '~': 0x35, ',': 0x36, '<': 0x36, '.': 0x37,
+                '>': 0x37, '/': 0x38, '?': 0x38
+                }
+
+        # Base HID usage codes
+        hid_base_lower = 0x04  # HID usage for 'a'
+        hid_base_upper = 0x04  # HID usage for 'A'
+        hid_base_number = 0x1E  # HID usage for '1'
+
+        for char in text:
+            usage = None
+            shift = False
+
+            if 'a' <= char <= 'z':
+                usage = hid_base_lower + (ord(char) - ord('a'))
+            elif 'A' <= char <= 'Z':
+                usage = hid_base_upper + (ord(char) - ord('A'))
+                shift = True
+            elif '1' <= char <= '9':
+                usage = hid_base_number + (ord(char) - ord('1'))
+            elif char == '0':
+                usage = 0x27
+            elif char in special_chars:
+                usage = special_chars[char]
+                # Determine if shift needs to be pressed for special characters
+                shift = char in '~!@#$%^&*()_+{}|:"<>?'
+
+            if usage is None:
+                continue  # Skip unsupported characters
+
+            # Press and release the shift key if necessary
+            if shift:
+                self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0xE1, "durationSeconds": 0.1})  # Shift down
+            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.1})  # Key down
+            self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.1})  # Key up
+            if shift:
+                self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0xE1, "durationSeconds": 0.1})  # Shift up
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
-def Client(api_key, driver=None, use_mjpeg=True):
+def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
     def get_ios_udid():
         system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
         serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
 
         if serial_numbers:
             first_serial_number = serial_numbers[0][1].strip()
             modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
@@ -271,11 +323,11 @@
 
     android_devices = get_connected_android_devices()
     if android_devices:
         return AndroidClient(api_key)
 
     ios_udid = get_ios_udid()
     if ios_udid:
-        return IOSClient(api_key, ios_udid=ios_udid, use_mjpeg=use_mjpeg)
+        return IOSClient(api_key, ios_udid=ios_udid, use_mjpeg=use_mjpeg, use_hid_typing=use_hid_typing)
 
     raise Exception("No connected devices found or driver provided.")
```

### Comparing `qaml-0.0.7.3/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.4/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.3
+Version: 0.0.7.4
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

