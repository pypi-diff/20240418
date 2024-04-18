# Comparing `tmp/steelpy-1.0.1.tar.gz` & `tmp/steelpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelpy-1.0.1.tar", max compression
+gzip compressed data, was "steelpy-1.0.2.tar", max compression
```

## Comparing `steelpy-1.0.1.tar` & `steelpy-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-1.0.1/license.txt
--rw-r--r--   0        0        0      488 2024-04-16 23:54:26.912611 steelpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-1.0.1/README.md
--rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-1.0.1/steelpy/__init__.py
--rw-r--r--   0        0        0    11358 2024-04-15 00:44:17.980620 steelpy-1.0.1/steelpy/LICENSE.md
--rw-r--r--   0        0        0       10 2024-04-15 00:44:17.980620 steelpy-1.0.1/steelpy/README.md
--rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-1.0.1/steelpy/shape files/.DS_Store
--rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-1.0.1/steelpy/shape files/C_shapes.xlsx
--rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-1.0.1/steelpy/shape files/DBL_L_shapes.xlsx
--rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-1.0.1/steelpy/shape files/HP_shapes.xlsx
--rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-1.0.1/steelpy/shape files/HSS_R_shapes.xlsx
--rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-1.0.1/steelpy/shape files/HSS_shapes.xlsx
--rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-1.0.1/steelpy/shape files/L_shapes.xlsx
--rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-1.0.1/steelpy/shape files/M_shapes.xlsx
--rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-1.0.1/steelpy/shape files/MC_shapes.xlsx
--rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-1.0.1/steelpy/shape files/MT_shapes.xlsx
--rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-1.0.1/steelpy/shape files/PIPE_shapes.xlsx
--rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-1.0.1/steelpy/shape files/S_shapes.xlsx
--rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-1.0.1/steelpy/shape files/ST_shapes.xlsx
--rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-1.0.1/steelpy/shape files/W_shapes.xlsx
--rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-1.0.1/steelpy/shape files/WT_shapes.xlsx
--rw-r--r--   0        0        0     1829 2024-04-16 23:47:01.477340 steelpy-1.0.1/steelpy/steelpy.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 steelpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-15 00:15:35.250711 steelpy-1.0.2/license.txt
+-rw-r--r--   0        0        0      488 2024-04-18 00:21:27.687556 steelpy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1491 2024-04-14 19:17:05.548477 steelpy-1.0.2/README.md
+-rw-r--r--   0        0        0       25 2024-04-15 00:07:30.681181 steelpy-1.0.2/steelpy/__init__.py
+-rw-r--r--   0        0        0    11358 2024-04-17 23:35:29.126753 steelpy-1.0.2/steelpy/LICENSE.md
+-rw-r--r--   0        0        0       10 2024-04-17 23:35:29.126753 steelpy-1.0.2/steelpy/README.md
+-rw-r--r--   0        0        0     6148 2024-04-13 14:24:11.525081 steelpy-1.0.2/steelpy/shape files/.DS_Store
+-rw-r--r--   0        0        0    11454 2024-04-13 14:22:22.387676 steelpy-1.0.2/steelpy/shape files/C_shapes.xlsx
+-rw-r--r--   0        0        0    55958 2024-04-13 14:22:22.517421 steelpy-1.0.2/steelpy/shape files/DBL_L_shapes.xlsx
+-rw-r--r--   0        0        0     8761 2024-04-13 14:22:22.531852 steelpy-1.0.2/steelpy/shape files/HP_shapes.xlsx
+-rw-r--r--   0        0        0    19577 2024-04-13 14:22:22.685953 steelpy-1.0.2/steelpy/shape files/HSS_R_shapes.xlsx
+-rw-r--r--   0        0        0    53674 2024-04-13 14:22:22.648944 steelpy-1.0.2/steelpy/shape files/HSS_shapes.xlsx
+-rw-r--r--   0        0        0    32880 2024-04-13 14:22:22.749414 steelpy-1.0.2/steelpy/shape files/L_shapes.xlsx
+-rw-r--r--   0        0        0     7785 2024-04-13 14:22:22.761931 steelpy-1.0.2/steelpy/shape files/M_shapes.xlsx
+-rw-r--r--   0        0        0    12974 2024-04-13 14:22:22.783967 steelpy-1.0.2/steelpy/shape files/MC_shapes.xlsx
+-rw-r--r--   0        0        0     6841 2024-04-13 14:22:22.794757 steelpy-1.0.2/steelpy/shape files/MT_shapes.xlsx
+-rw-r--r--   0        0        0     9052 2024-04-13 14:22:22.809959 steelpy-1.0.2/steelpy/shape files/PIPE_shapes.xlsx
+-rw-r--r--   0        0        0     9556 2024-04-13 14:22:22.825993 steelpy-1.0.2/steelpy/shape files/S_shapes.xlsx
+-rw-r--r--   0        0        0     8516 2024-04-13 14:22:22.839824 steelpy-1.0.2/steelpy/shape files/ST_shapes.xlsx
+-rw-r--r--   0        0        0    51977 2024-04-13 14:22:22.946043 steelpy-1.0.2/steelpy/shape files/W_shapes.xlsx
+-rw-r--r--   0        0        0    46395 2024-04-13 14:22:23.030673 steelpy-1.0.2/steelpy/shape files/WT_shapes.xlsx
+-rw-r--r--   0        0        0     1885 2024-04-18 00:05:46.187099 steelpy-1.0.2/steelpy/steelpy.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 steelpy-1.0.2/PKG-INFO
```

### Comparing `steelpy-1.0.1/license.txt` & `steelpy-1.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/README.md` & `steelpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/LICENSE.md` & `steelpy-1.0.2/steelpy/LICENSE.md`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/.DS_Store` & `steelpy-1.0.2/steelpy/shape files/.DS_Store`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/C_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/C_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/DBL_L_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/DBL_L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/HP_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/HP_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/HSS_R_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/HSS_R_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/HSS_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/HSS_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/L_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/L_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/M_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/M_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/MC_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/MC_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/MT_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/MT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/PIPE_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/PIPE_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/S_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/S_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/ST_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/ST_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/W_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/W_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/shape files/WT_shapes.xlsx` & `steelpy-1.0.2/steelpy/shape files/WT_shapes.xlsx`

 * *Files identical despite different names*

### Comparing `steelpy-1.0.1/steelpy/steelpy.py` & `steelpy-1.0.2/steelpy/steelpy.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import pandas as pd
-from collections import namedtuple
-import os
-import glob
-
-class Steel:
-    def __init__(self):
-        self.variables = {}
-
-    def add_variable(self, name, value):
-        self.variables[name] = value
-
-    def __getattr__(self, name):
-        if name in self.variables:
-            return self.variables[name]
-        raise AttributeError(f"'DynamicVariables' object has no attribute '{name}'")
-    
-aisc = Steel()
-
-# Get the directory of the currently executing module
-module_dir = os.path.dirname(__file__)
-# Construct the relative path to shape files folder.
-directory_path = os.path.join(module_dir, 'shape files')
-
-# Get a list of all .xlsx files in the directory
-shape_files = glob.glob(os.path.join(directory_path, "*.xlsx"))
-
-# Iterate over each .xlsx file
-for file in shape_files: 
-    # Get current shape being considered e.g. 'W_shapes'
-    curFileName = os.path.basename(file)[:-5]
-
-    # Read Excel file into a pandas DataFrame
-    df = pd.read_excel(file)
-
-    # Define a named tuple class for the shape section properties dynamically
-    ShapeProperties = namedtuple('ShapeProperties', df.columns[1:])
-
-    # Create a dictionary to store shape section properties
-    props_dict = {}
-
-    # Populate the dictionary with shape section properties
-    for row in df.itertuples(index=False):
-        key = row[0]  # Key is taken from the first column
-        properties = ShapeProperties(*row[1:])  # Create a namedtuple for properties
-        props_dict[key] = properties
-
-    # Define a named tuple class for the steel shapes
-    SteelShapes = namedtuple('SteelShapes', props_dict.keys())
-
-    # Create dictionary for 
-
-    # Create a named tuple instance for steel shapes
-    steel_shapes = SteelShapes(**props_dict)
-
-    #add shape to aisc class
+import pandas as pd
+from collections import namedtuple
+import os
+import glob
+
+class Steel:
+    def __init__(self):
+        self.variables = {}
+
+    def add_variable(self, name, value):
+        self.variables[name] = value
+
+    def __getattr__(self, name):
+        if name in self.variables:
+            return self.variables[name]
+        raise AttributeError(f"'DynamicVariables' object has no attribute '{name}'")
+    
+aisc = Steel()
+
+# Get the directory of the currently executing module
+module_dir = os.path.dirname(__file__)
+# Construct the relative path to shape files folder.
+directory_path = os.path.join(module_dir, 'shape files')
+
+# Get a list of all .xlsx files in the directory
+shape_files = glob.glob(os.path.join(directory_path, "*.xlsx"))
+
+# Iterate over each .xlsx file
+for file in shape_files: 
+    # Get current shape being considered e.g. 'W_shapes'
+    curFileName = os.path.basename(file)[:-5]
+
+    # Read Excel file into a pandas DataFrame
+    df = pd.read_excel(file)
+
+    # Define a named tuple class for the shape section properties dynamically
+    ShapeProperties = namedtuple('ShapeProperties', df.columns[1:])
+
+    # Create a dictionary to store shape section properties
+    props_dict = {}
+
+    # Populate the dictionary with shape section properties
+    for row in df.itertuples(index=False):
+        key = row[0]  # Key is taken from the first column
+        properties = ShapeProperties(*row[1:])  # Create a namedtuple for properties
+        props_dict[key] = properties
+
+    # Define a named tuple class for the steel shapes
+    SteelShapes = namedtuple('SteelShapes', props_dict.keys())
+
+    # Create dictionary for 
+
+    # Create a named tuple instance for steel shapes
+    steel_shapes = SteelShapes(**props_dict)
+
+    #add shape to aisc class
     aisc.add_variable(curFileName, steel_shapes)
```

### Comparing `steelpy-1.0.1/PKG-INFO` & `steelpy-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steelpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple library for section properties of AISC steel shapes
 License: Apache-2.0
 Keywords: steel,AISC,engineering,shapes_AISC,AISC Shapes Database v16.0
 Author: evanfaler
 Author-email: emfaler@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

