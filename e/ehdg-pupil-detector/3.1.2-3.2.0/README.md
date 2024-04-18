# Comparing `tmp/ehdg_pupil_detector-3.1.2.tar.gz` & `tmp/ehdg_pupil_detector-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.1.2.tar", last modified: Tue Apr 16 04:43:35 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.2.0.tar", last modified: Wed Apr 17 03:03:09 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.1.2.tar` & `ehdg_pupil_detector-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.868942 ehdg_pupil_detector-3.1.2/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.2/LICENSE
--rw-rw-rw-   0        0        0     4068 2024-04-16 04:43:35.867945 ehdg_pupil_detector-3.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.2/README.md
--rw-rw-rw-   0        0        0     1148 2024-04-16 04:32:50.000000 ehdg_pupil_detector-3.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 04:43:35.868942 ehdg_pupil_detector-3.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.833538 ehdg_pupil_detector-3.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.841500 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    12338 2024-04-16 04:37:00.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opmtrack.py
-drwxrwxrwx   0        0        0        0 2024-04-16 04:43:35.865949 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4068 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-16 04:43:35.000000 ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 03:03:09.113124 ehdg_pupil_detector-3.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-17 03:03:09.112124 ehdg_pupil_detector-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.2.0/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-17 02:48:47.000000 ehdg_pupil_detector-3.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 03:03:09.113124 ehdg_pupil_detector-3.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 03:03:09.086241 ehdg_pupil_detector-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 03:03:09.095169 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    14123 2024-04-17 03:00:59.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-17 03:03:09.111127 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 03:03:09.000000 ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.1.2/LICENSE` & `ehdg_pupil_detector-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.2/PKG-INFO` & `ehdg_pupil_detector-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.2
+Version: 3.2.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
-Requires-Dist: ehdg_tools
+Requires-Dist: ehdg_tools>=4.2.1
 Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
```

### Comparing `ehdg_pupil_detector-3.1.2/README.md` & `ehdg_pupil_detector-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.2/pyproject.toml` & `ehdg_pupil_detector-3.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.1.2"
+version = "3.2.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
-dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
+dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.1", "numpy"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
@@ -18,15 +18,15 @@
 opmtrack = "ehdg_pupil_detector.opmtrack:main"
 
 [project.urls]
 "Homepage" = "https://github.com/jtur044/ehdg_pupil_detector"
 "Bug Tracker" = "https://github.com/jtur044/ehdg_pupil_detector/issues"
 
 [build-system]
-requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
+requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.1", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 import importlib.metadata
 from importlib.resources import files
 import cv2
 import commentjson
 from ehdg_pupil_detector import ehdg_pupil_detector
 from ehdg_tools.ehdg_buffers import TinyFillBuffer
+from ehdg_tools.ehdg_plotter import raw_plot
 import numpy as np
 
 
 # This function is to get built-in config location with new library (from importlib.resources import files)
 def get_config_location(module_name, config_file_name):
     config_dir = files(module_name).joinpath(config_file_name)
     return str(config_dir)
@@ -49,15 +50,15 @@
     temp_dict["ellipse_axis_b"] = ellipse_axis_b
     temp_dict["ellipse_angle"] = ellipse_angle
 
     return temp_dict
 
 
 # This function is to redetect with pupil detector by given detector and tiny fill buffer
-def opm_detect(trial_video, out_folder, config_dict, buffer_length_input, direction_input=None):
+def opm_detect(trial_video, out_folder, config_dict, plot_dict, buffer_length_input, direction_input=None):
     out_csv_dir = os.path.join(out_folder, "result.csv")
     out_video_dir = os.path.join(out_folder, "result.mp4")
 
     detector = ehdg_pupil_detector.Detector()
     buffer = TinyFillBuffer(buffer_length_input)
     detector.update_config(config_dict)
     updated_properties = detector.get_config_info()
@@ -155,37 +156,44 @@
                 destination_file.close()
                 v_writer.release()
                 print(f"Result folder dir: {out_folder}.")
                 print(f"Result csv dir: {out_csv_dir}.")
                 print(f"Result video dir: {out_video_dir}.")
                 break
 
+    raw_plot_info = plot_dict["raw_plot"]
+    out_image_dir = raw_plot(out_csv_dir, raw_plot_info)
+    print(f"Result plot image dir: {out_image_dir}.")
+
 
 def main():
     parser = argparse.ArgumentParser(prog='opmtrack',
                                      description='OKNTRACK package.')
     opmtrack_version = importlib.metadata.version('ehdg_pupil_detector')
     parser.add_argument('--version', action='version', version=opmtrack_version),
-    parser.add_argument("-i", dest="input_video", required=False, default=None,
+    parser.add_argument("-i", dest="input_video", required=True, default=None,
                         metavar="input video")
-    parser.add_argument("-o", dest="output_folder", required=False, default=None,
+    parser.add_argument("-o", dest="output_folder", required=True, default=None,
                         metavar="output folder")
     parser.add_argument("-c", dest="opm_config", required=False, default=None,
                         metavar="opm detector config")
     parser.add_argument("-d", dest="direction_input", required=False, default=None,
                         metavar="direction input")
     parser.add_argument("-bl", dest="buffer_length", required=False, default=None,
                         metavar="buffer length")
+    parser.add_argument("-p", dest="plot_config", required=False, default=None,
+                        metavar="plot config")
 
     args = parser.parse_args()
     input_video = args.input_video
     output_folder = args.output_folder
     opm_config = args.opm_config
     direction_input = args.direction_input
     buffer_length = args.buffer_length
+    plot_config = args.plot_config
 
     default_buffer_length = 7
 
     if not os.path.isfile(input_video):
         print(f"Input video is invalid.")
         print(f"Input video: {input_video} is invalid.")
         return
@@ -214,23 +222,47 @@
                 return
 
     if opm_config is None:
         opm_config = get_config_location("ehdg_pupil_detector", "opm_detector_config.json")
         try:
             with open(opm_config) as opm_config_info:
                 opm_config_dict = commentjson.load(opm_config_info)
+                print("There is no custom opm detector config input.")
+                print("Therefore, built-in opm detector config will be used.")
+                print(f"Location: {opm_config}")
         except FileNotFoundError:
             raise FileNotFoundError(f"Error opening built-in opm config file:{opm_config}!")
     else:
         try:
             with open(opm_config) as opm_config_info:
                 opm_config_dict = commentjson.load(opm_config_info)
+                print("There is custom opm detector config input.")
+                print(f"Location: {opm_config}")
         except FileNotFoundError:
             raise FileNotFoundError(f"Error opening opm config file:{opm_config}!")
 
+    if plot_config is None:
+        plot_config = get_config_location("ehdg_pupil_detector", "opmtrack_plot.json")
+        try:
+            with open(plot_config) as plot_info:
+                plot_info_dict = commentjson.load(plot_info)
+                print("There is no custom plot info input.")
+                print("Therefore, built-in plot info config will be used.")
+                print(f"Location: {plot_config}")
+        except FileNotFoundError:
+            raise FileNotFoundError(f"Error opening built-in opm plot config file:{plot_config}!")
+    else:
+        try:
+            with open(plot_config) as plot_info:
+                plot_info_dict = commentjson.load(plot_info)
+                print("There is custom plot info input.")
+                print(f"Location: {plot_config}")
+        except FileNotFoundError:
+            raise FileNotFoundError(f"Error opening opm plot config file:{plot_config}!")
+
     if direction_input is not None:
         if str(direction_input).lower() == "right":
             direction_to_be_used = 1
         elif str(direction_input).lower() == "left":
             direction_to_be_used = -1
         else:
             try:
@@ -240,14 +272,16 @@
                 else:
                     raise ValueError(f"Invalid direction input {direction_input}.")
             except ValueError:
                 raise ValueError(f"Invalid direction input {direction_input}.")
         print(f"There is direction input {direction_input}.")
         print(f"Therefore, direction: {direction_to_be_used} will be added to csv as a column.")
     else:
+        print(f"There is no direction input.")
+        print(f"Therefore, there will be no direction column in result.csv.")
         direction_to_be_used = None
 
     if buffer_length is not None:
         try:
             buffer_length_to_be_used = int(buffer_length)
             print("There is buffer length input.")
             print(f"OPM detector will be using Tiny Fill Buffer with length:{buffer_length_to_be_used}.")
@@ -256,9 +290,9 @@
             print(f"There is buffer length input but it is invalid: {buffer_length}.")
             print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
     else:
         buffer_length_to_be_used = default_buffer_length
         print("There is no buffer length input.")
         print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
 
-    opm_detect(input_video, output_directory, opm_config_dict,
+    opm_detect(input_video, output_directory, opm_config_dict, plot_info_dict,
                buffer_length_to_be_used, direction_input=direction_to_be_used)
```

### Comparing `ehdg_pupil_detector-3.1.2/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.2.0/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.1.2
+Version: 3.2.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
-Requires-Dist: ehdg_tools
+Requires-Dist: ehdg_tools>=4.2.1
 Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
```

