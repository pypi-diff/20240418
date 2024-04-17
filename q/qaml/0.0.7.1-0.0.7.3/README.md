# Comparing `tmp/qaml-0.0.7.1.tar.gz` & `tmp/qaml-0.0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.1.tar", last modified: Wed Apr 17 15:45:16 2024, max compression
+gzip compressed data, was "qaml-0.0.7.3.tar", last modified: Wed Apr 17 18:36:16 2024, max compression
```

## Comparing `qaml-0.0.7.1.tar` & `qaml-0.0.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.229779 qaml-0.0.7.1/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.1/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 15:45:16.229519 qaml-0.0.7.1/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.1/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 15:45:13.000000 qaml-0.0.7.1/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.228373 qaml-0.0.7.1/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.1/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.1/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    10610 2024-04-17 15:43:09.000000 qaml-0.0.7.1/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 15:45:16.229176 qaml-0.0.7.1/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 15:45:16.000000 qaml-0.0.7.1/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 15:45:16.229830 qaml-0.0.7.1/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.692478 qaml-0.0.7.3/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.3/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 18:36:16.692332 qaml-0.0.7.3/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.3/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-17 18:36:06.000000 qaml-0.0.7.3/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.691480 qaml-0.0.7.3/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.3/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1113 2024-04-11 18:51:32.000000 qaml-0.0.7.3/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    11051 2024-04-17 18:31:00.000000 qaml-0.0.7.3/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-17 18:36:16.692184 qaml-0.0.7.3/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-17 18:36:16.000000 qaml-0.0.7.3/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-17 18:36:16.692509 qaml-0.0.7.3/setup.cfg
```

### Comparing `qaml-0.0.7.1/LICENSE` & `qaml-0.0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.1/PKG-INFO` & `qaml-0.0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.1
+Version: 0.0.7.3
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.1/README.md` & `qaml-0.0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.1/pyproject.toml` & `qaml-0.0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.1"
+version = "0.0.7.3"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.1/qaml/__main__.py` & `qaml-0.0.7.3/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.1/qaml/client.py` & `qaml-0.0.7.3/qaml/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,29 @@
         new_size = (960, int(960 / aspect_ratio)) if PIL_image.size[0] == longer_side else (int(960 * aspect_ratio), 960)
         PIL_image = PIL_image.resize(new_size)
         buffered = BytesIO()
         PIL_image.save(buffered, format="PNG")
         screenshot = base64.b64encode(buffered.getvalue()).decode("utf-8")
         return screenshot
 
+    def _execute_function(self, function_name, **kwargs):
+        available_functions = {
+            "tap": self.tap_coordinates,
+            "drag": self.drag,
+            "swipe": self.swipe,
+            "scroll": self.scroll,
+            "type_text": self.type_text,
+            "sleep": self.sleep,
+            "report_error": self.report_error,
+            "switch_to_app": self.switch_to_app,
+        }
+        function = available_functions.get(function_name)
+        if function:
+            function(**kwargs)
+
     def execute(self, script):
         screenshot = self.get_screenshot()
         payload = {"action": script, "screen_size": self.screen_size, "screenshot": screenshot, "platform": self.platform, "extra_context": self.context}
         response = self.req_session.post("https://api.camelqa.com/v1/execute", json=payload, headers={"Authorization": f"Bearer {self.api_key}"})
         print(f"Action: {script} - Response: {response.text}")
         actions = response.json()
         available_functions = {
@@ -77,17 +92,15 @@
             "scroll": self.scroll,
             "type_text": self.type_text,
             "sleep": self.sleep,
             "report_error": self.report_error,
             "switch_to_app": self.switch_to_app,
         }
         for action in actions:
-            function = available_functions[action["name"]]
-            arguments = json.loads(action["arguments"])
-            function(**arguments)
+            self._execute_function(action["name"], **json.loads(action["arguments"]))
 
     def agent(self, task):
         progress = []
         while True:
             screenshot = self.get_screenshot()
             payload = {"task": task, "progress": progress, "platform": self.platform, "screenshot": screenshot}
             response = self.req_session.post("https://api.camelqa.com/v1/agent", json=payload)
@@ -242,23 +255,23 @@
             devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
             connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
             return connected_devices
         except:
             return []
 
     if driver is not None:
-            platform_name = driver.platform_name.lower()
-            if platform_name == 'android':
-                print("Using the provided Appium driver for Android.")
-                return AndroidClient(api_key, driver=driver)
-            elif platform_name == 'ios':
-                print("Using the provided Appium driver for iOS.")
-                return IOSClient(api_key, driver=driver)
-            else:
-                raise Exception("Unsupported platform specified in the provided driver's capabilities.")
+        platform_name = driver.capabilities.get("platformName").lower()
+        if platform_name == 'android':
+            print("Using the provided Appium driver for Android.")
+            return AndroidClient(api_key, driver=driver)
+        elif platform_name == 'ios':
+            print("Using the provided Appium driver for iOS.")
+            return IOSClient(api_key, driver=driver)
+        else:
+            raise Exception("Unsupported platform specified in the provided driver's capabilities.")
 
     android_devices = get_connected_android_devices()
     if android_devices:
         return AndroidClient(api_key)
 
     ios_udid = get_ios_udid()
     if ios_udid:
```

### Comparing `qaml-0.0.7.1/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.3/qaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.1
+Version: 0.0.7.3
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

