# Comparing `tmp/qaml-0.0.7.6.tar.gz` & `tmp/qaml-0.0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.6.tar", last modified: Thu Apr 18 00:06:43 2024, max compression
+gzip compressed data, was "qaml-0.0.7.7.tar", last modified: Thu Apr 18 20:03:09 2024, max compression
```

## Comparing `qaml-0.0.7.6.tar` & `qaml-0.0.7.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.371058 qaml-0.0.7.6/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.6/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 00:06:43.370918 qaml-0.0.7.6/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.6/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 00:06:40.000000 qaml-0.0.7.6/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.370067 qaml-0.0.7.6/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.6/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.6/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13116 2024-04-18 00:06:01.000000 qaml-0.0.7.6/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 00:06:43.370767 qaml-0.0.7.6/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 00:06:43.000000 qaml-0.0.7.6/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 00:06:43.371088 qaml-0.0.7.6/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.340035 qaml-0.0.7.7/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.7/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:03:09.339895 qaml-0.0.7.7/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.7/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 20:02:31.000000 qaml-0.0.7.7/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.339026 qaml-0.0.7.7/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.7/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.7/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13174 2024-04-18 19:52:37.000000 qaml-0.0.7.7/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.339724 qaml-0.0.7.7/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 20:03:09.340064 qaml-0.0.7.7/setup.cfg
```

### Comparing `qaml-0.0.7.6/LICENSE` & `qaml-0.0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.6/PKG-INFO` & `qaml-0.0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.6
+Version: 0.0.7.7
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.6/README.md` & `qaml-0.0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.6/pyproject.toml` & `qaml-0.0.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.6"
+version = "0.0.7.7"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.6/qaml/__main__.py` & `qaml-0.0.7.7/qaml/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,14 @@
     api_key = os.environ.get("QAML_API_KEY")
     use_mjpeg = os.environ.get("QAML_USE_MJPEG", "true").lower() == "true"
     if api_key is None:
         print("Please set the QAML_API_KEY environment variable")
         sys.exit(1)
     print("Initializing device driver...")
     client = qaml.Client(api_key=api_key, use_mjpeg=use_mjpeg)
-    print(dir(qaml))
-    print(qaml.__file__)
-    print(qaml.__name__)
-    print(qaml.__package__)
-    print(qaml.__path__)
-    print(qaml.__spec__)
-    print(qaml)
     # if no args, start repl
     if len(sys.argv) == 1:
         while True:
             try:
                 command = input("Enter a command: ")
                 client.execute(command)
             except EOFError:
```

### Comparing `qaml-0.0.7.6/qaml/client.py` & `qaml-0.0.7.7/qaml/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,36 +170,46 @@
         direction_map = {"up": "down", "down": "up", "left": "right", "right": "left"}
         self.swipe(direction_map[direction])
 
     def type_text(self, text):
         subprocess.run(["adb", "shell", "input", "text", f"'{text}'"])
 
 class IOSClient(BaseClient):
-    def __init__(self, api_key, driver=None, ios_udid=None, use_mjpeg=True, use_hid_typing=False):
+    def __init__(self, api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
         super().__init__(api_key)
         self.platform = "iOS"
         self.use_mjpeg = use_mjpeg
         self.use_hid_typing = use_hid_typing
         if driver:
             self.driver = driver
         else:
+            def get_ios_udid():
+                system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
+                serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
+
+                if serial_numbers:
+                    first_serial_number = serial_numbers[0][1].strip()
+                    modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
+                    return modified_serial_number
+            ios_udid = get_ios_udid()
             # try 3 times to setup the driver
             for _ in range(3):
                 try:
                     self.setup_driver(ios_udid)
                     break
                 except:
                     pass
             else:
                 raise Exception("Failed to setup the driver.")
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self, udid):
         options = XCUITestOptions()
-        options.udid = udid
+        if udid:
+            options.udid = udid
         options.new_command_timeout = 60 * 5 # 5 minutes
         if self.use_mjpeg:
             custom_caps = {"mjpegScreenshotUrl": "http://localhost:9100"}
             options.load_capabilities(custom_caps)
 
         def create_driver(options):
             try:
@@ -282,22 +292,14 @@
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": usage, "durationSeconds": 0.005})  # Key down
             self.driver.execute_script("mobile: performIoHidEvent", {"page": 0x07, "usage": 0x00, "durationSeconds": 0.005})  # Key up
 
     def switch_to_app(self, bundle_id):
         self.driver.activate_app(bundle_id)
 
 def Client(api_key, driver=None, use_mjpeg=True, use_hid_typing=False):
-    def get_ios_udid():
-        system_profiler_output = subprocess.run(["system_profiler", "SPUSBDataType"], capture_output=True, text=True).stdout
-        serial_numbers = re.findall(r'(iPhone|iPad).*?Serial Number: *([^\n]+)', system_profiler_output, re.DOTALL)
-
-        if serial_numbers:
-            first_serial_number = serial_numbers[0][1].strip()
-            modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
-            return modified_serial_number
 
     def get_connected_android_devices():
         try:
             result = subprocess.run(["adb", "devices"], capture_output=True, text=True)
             devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
             connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
             return connected_devices
@@ -315,13 +317,12 @@
         else:
             raise Exception("Unsupported platform specified in the provided driver's capabilities.")
 
     android_devices = get_connected_android_devices()
     if android_devices:
         return AndroidClient(api_key)
 
-    ios_udid = get_ios_udid()
-    if ios_udid:
-        return IOSClient(api_key, ios_udid=ios_udid, use_mjpeg=use_mjpeg, use_hid_typing=use_hid_typing)
-
-    raise Exception("No connected devices found or driver provided.")
+    try:
+        return IOSClient(api_key, use_mjpeg=use_mjpeg, use_hid_typing=use_hid_typing)
+    except:
+        raise Exception("No connected devices found or driver provided.")
```

### Comparing `qaml-0.0.7.6/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.7/qaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.6
+Version: 0.0.7.7
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

