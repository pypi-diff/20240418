# Comparing `tmp/pywayne-1.0.0.6.8.tar.gz` & `tmp/pywayne-1.0.0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.6.8.tar", last modified: Wed Apr 10 13:23:49 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.6.9.tar", last modified: Thu Apr 18 13:49:07 2024, max compression
```

## Comparing `pywayne-1.0.0.6.8.tar` & `pywayne-1.0.0.6.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.708918 pywayne-1.0.0.6.8/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-10 13:23:49.708241 pywayne-1.0.0.6.8/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.691572 pywayne-1.0.0.6.8/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.8/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.8/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.695635 pywayne-1.0.0.6.8/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-10 13:22:10.000000 pywayne-1.0.0.6.8/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.701256 pywayne-1.0.0.6.8/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.8/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.8/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.702513 pywayne-1.0.0.6.8/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.704759 pywayne-1.0.0.6.8/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.8/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.8/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.8/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.8/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.8/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    15331 2024-04-10 13:22:35.000000 pywayne-1.0.0.6.8/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.706117 pywayne-1.0.0.6.8/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.8/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.8/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.706880 pywayne-1.0.0.6.8/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.8/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.8/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-10 13:23:49.707567 pywayne-1.0.0.6.8/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-10 13:23:49.000000 pywayne-1.0.0.6.8/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-10 13:23:49.000000 pywayne-1.0.0.6.8/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-10 13:23:49.000000 pywayne-1.0.0.6.8/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      153 2024-04-10 13:23:49.000000 pywayne-1.0.0.6.8/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-10 13:23:49.000000 pywayne-1.0.0.6.8/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-10 13:23:49.709044 pywayne-1.0.0.6.8/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.8/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.517295 pywayne-1.0.0.6.9/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-18 13:49:07.516979 pywayne-1.0.0.6.9/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.510017 pywayne-1.0.0.6.9/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.6.9/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.6.9/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.512372 pywayne-1.0.0.6.9/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-04-18 13:48:08.000000 pywayne-1.0.0.6.9/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.514040 pywayne-1.0.0.6.9/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.9/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.6.9/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.514540 pywayne-1.0.0.6.9/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.515252 pywayne-1.0.0.6.9/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.6.9/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.6.9/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.6.9/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.6.9/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.6.9/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    15728 2024-04-18 13:48:34.000000 pywayne-1.0.0.6.9/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.515889 pywayne-1.0.0.6.9/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.9/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.6.9/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.516402 pywayne-1.0.0.6.9/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.6.9/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.6.9/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-04-18 13:49:07.516713 pywayne-1.0.0.6.9/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1461 2024-04-18 13:49:07.000000 pywayne-1.0.0.6.9/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-04-18 13:49:07.000000 pywayne-1.0.0.6.9/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-04-18 13:49:07.000000 pywayne-1.0.0.6.9/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      153 2024-04-18 13:49:07.000000 pywayne-1.0.0.6.9/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-04-18 13:49:07.000000 pywayne-1.0.0.6.9/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-04-18 13:49:07.517345 pywayne-1.0.0.6.9/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.6.9/setup.py
```

### Comparing `pywayne-1.0.0.6.8/LICENSE` & `pywayne-1.0.0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/PKG-INFO` & `pywayne-1.0.0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.8
+Version: 1.0.0.6.9
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.8/README.md` & `pywayne-1.0.0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/bin/gettool.py` & `pywayne-1.0.0.6.9/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.6.9/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/ahrs/tools.py` & `pywayne-1.0.0.6.9/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.6.9/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/data_structure.py` & `pywayne-1.0.0.6.9/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/dsp.py` & `pywayne-1.0.0.6.9/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/gui.py` & `pywayne-1.0.0.6.9/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/math.py` & `pywayne-1.0.0.6.9/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/plot.py` & `pywayne-1.0.0.6.9/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/tools.py` & `pywayne-1.0.0.6.9/pywayne/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     color_code = colors.get(color, colors["default"])
     end_code = colors["default"]  # Reset color and style to avoid affecting subsequent prints
     print(f"{color_code}{bold_code}{text}{end_code}")
 
 
 def write_yaml_config(config_yaml_file: str, config: dict, update=False):
     """
-    Writes the given configuration dictionary to a YAML file.
+    Writes the given configuration dictionary to a YAML file with file lock protection.
 
     :param config_yaml_file: The path to the YAML file where the config should be written.
     :param config: A dictionary containing the configuration settings to write.
     :param update: If True, the function will update the existing YAML file with the new config. If False, the function will overwrite the existing YAML file with the new config.
     """
 
     def deep_merge_dicts(original, updater):
@@ -398,36 +398,49 @@
                     deep_merge_dicts(original_value, value)
                 else:
                     original[key] = value
             else:
                 original[key] = value
         return original
 
-    try:
-        if update:
-            existing_config = read_yaml_config(config_yaml_file)
-            config = deep_merge_dicts(existing_config, config)
-        with open(config_yaml_file, 'w', encoding='UTF-8') as f:
-            yaml.dump(config, f, default_flow_style=False)
-    except IOError as e:
-        print(f"Error writing to file {config_yaml_file}: {e}")
-    except yaml.YAMLError as e:
-        print(f"Error dumping config to YAML: {e}")
+    lock_file = config_yaml_file + ".lock"
+    lock = FileLock(lock_file)
+
+    if update and os.path.exists(config_yaml_file):
+        existing_config = read_yaml_config(config_yaml_file)
+    else:
+        existing_config = {}
+
+    with lock:
+        try:
+            if update:
+                config = deep_merge_dicts(existing_config, config)
+            with open(config_yaml_file, 'w', encoding='UTF-8') as f:
+                yaml.dump(config, f, default_flow_style=False)
+        except IOError as e:
+            print(f"Error writing to file {config_yaml_file}: {e}")
+        except yaml.YAMLError as e:
+            print(f"Error dumping config to YAML: {e}")
 
 
 def read_yaml_config(config_yaml_file: str):
     """
-    Reads and returns the configuration from a YAML file.
+    Reads and returns the configuration from a YAML file with file lock protection.
 
     :param config_yaml_file: The path to the YAML file from which to read the config.
     :return: A dictionary containing the configuration settings.
     """
-    try:
-        with open(config_yaml_file, 'r', encoding='UTF-8') as f:
-            data = yaml.safe_load(f)
-        return data
-    except IOError as e:
-        print(f"Error reading file {config_yaml_file}: {e}")
-        return {}
-    except yaml.YAMLError as e:
-        print(f"Error parsing YAML file: {e}")
-        return {}
+
+    lock_file = config_yaml_file + ".lock"
+    lock = FileLock(lock_file)
+
+    with lock:
+        try:
+            with open(config_yaml_file, 'r', encoding='UTF-8') as f:
+                data = yaml.safe_load(f)
+            return data
+        except IOError as e:
+            print(f"Error reading file {config_yaml_file}: {e}")
+            return {}
+        except yaml.YAMLError as e:
+            print(f"Error parsing YAML file: {e}")
+            return {}
```

### Comparing `pywayne-1.0.0.6.8/pywayne/vio/tools.py` & `pywayne-1.0.0.6.9/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.6.9/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.6.9/pywayne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.6.8
+Version: 1.0.0.6.9
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.6.8/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.6.9/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.6.8/setup.py` & `pywayne-1.0.0.6.9/setup.py`

 * *Files identical despite different names*

