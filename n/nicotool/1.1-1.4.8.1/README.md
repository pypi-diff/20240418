# Comparing `tmp/nicotool-1.1.tar.gz` & `tmp/nicotool-1.4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicotool-1.1.tar", last modified: Sat Mar  9 19:46:13 2024, max compression
+gzip compressed data, was "nicotool-1.4.8.1.tar", last modified: Thu Apr 18 08:07:46 2024, max compression
```

## Comparing `nicotool-1.1.tar` & `nicotool-1.4.8.1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 19:46:13.504732 nicotool-1.1/
--rw-rw-rw-   0        0        0      303 2024-03-09 19:46:13.503735 nicotool-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-03-05 16:57:58.000000 nicotool-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 19:46:13.492765 nicotool-1.1/nico/
--rw-rw-rw-   0        0        0      798 2024-03-09 11:14:29.000000 nicotool-1.1/nico/__init__.py
--rw-rw-rw-   0        0        0     8342 2024-03-09 11:14:20.000000 nicotool-1.1/nico/additional_functions.py
--rw-rw-rw-   0        0        0    13965 2024-03-08 16:09:17.000000 nicotool-1.1/nico/ascii.py
--rw-rw-rw-   0        0        0     1499 2024-03-07 12:31:49.000000 nicotool-1.1/nico/id.py
--rw-rw-rw-   0        0        0    12434 2024-03-07 13:21:49.000000 nicotool-1.1/nico/jsonify.py
--rw-rw-rw-   0        0        0     3467 2024-03-06 11:56:27.000000 nicotool-1.1/nico/print_additions.py
-drwxrwxrwx   0        0        0        0 2024-03-09 19:46:13.501740 nicotool-1.1/nicotool.egg-info/
--rw-rw-rw-   0        0        0      303 2024-03-09 19:46:13.000000 nicotool-1.1/nicotool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-03-09 19:46:13.000000 nicotool-1.1/nicotool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 19:46:13.000000 nicotool-1.1/nicotool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-09 19:46:13.000000 nicotool-1.1/nicotool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 19:46:13.504732 nicotool-1.1/setup.cfg
--rw-rw-rw-   0        0        0      285 2024-03-09 19:45:57.000000 nicotool-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.333716 nicotool-1.4.8.1/
+-rw-rw-rw-   0        0        0      307 2024-04-18 08:07:46.332711 nicotool-1.4.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-03-13 13:16:47.000000 nicotool-1.4.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.314765 nicotool-1.4.8.1/nicotool/
+-rw-rw-rw-   0        0        0     3885 2024-04-17 08:25:07.000000 nicotool-1.4.8.1/nicotool/__init__.py
+-rw-rw-rw-   0        0        0     9448 2024-04-08 07:07:28.000000 nicotool-1.4.8.1/nicotool/additional_functions.py
+-rw-rw-rw-   0        0        0    13965 2024-04-08 07:07:29.000000 nicotool-1.4.8.1/nicotool/ascii.py
+-rw-rw-rw-   0        0        0      812 2024-04-08 07:07:41.000000 nicotool-1.4.8.1/nicotool/data_manipulation.py
+-rw-rw-rw-   0        0        0    38183 2024-04-17 13:12:42.000000 nicotool-1.4.8.1/nicotool/database.py
+-rw-rw-rw-   0        0        0     9440 2024-04-08 07:07:43.000000 nicotool-1.4.8.1/nicotool/files.py
+-rw-rw-rw-   0        0        0     1499 2024-04-08 07:07:42.000000 nicotool-1.4.8.1/nicotool/id.py
+-rw-rw-rw-   0        0        0    12338 2024-03-21 08:42:28.000000 nicotool-1.4.8.1/nicotool/jsonify.py
+-rw-rw-rw-   0        0        0     5435 2024-04-08 07:12:58.000000 nicotool-1.4.8.1/nicotool/keyboard.py
+-rw-rw-rw-   0        0        0     3797 2024-04-08 07:12:59.000000 nicotool-1.4.8.1/nicotool/print_additions.py
+-rw-rw-rw-   0        0        0     3704 2024-04-08 07:13:01.000000 nicotool-1.4.8.1/nicotool/profanities.py
+-rw-rw-rw-   0        0        0    17309 2024-04-08 07:12:51.000000 nicotool-1.4.8.1/nicotool/youtube.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:07:46.330716 nicotool-1.4.8.1/nicotool.egg-info/
+-rw-rw-rw-   0        0        0      307 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 08:07:46.000000 nicotool-1.4.8.1/nicotool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 08:07:46.334706 nicotool-1.4.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-04-18 08:07:39.000000 nicotool-1.4.8.1/setup.py
```

### Comparing `nicotool-1.1/nico/additional_functions.py` & `nicotool-1.4.8.1/nicotool/additional_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 import datetime
 import copy
 import csv
 import math
 import logging
 import time
-import warnings
 
 
 def remove_whitespace(text:str):
     """
     Removes every whitespace from a string.
 
     Args:
@@ -324,7 +323,38 @@
     Args:
         - lst (list): The input list.
 
     Returns:
         - list: A list containing unique elements.
     """
     return list(set(lst))
+def validateHex(hex_color):
+    """
+    Validates a hexadecimal color code and returns its RGB representation if valid.
+    
+    Args:
+        hex_color (str): The hexadecimal color code to validate.
+        
+    Returns:
+        tuple or None: A tuple containing the RGB representation (as integers between 0 and 255) 
+                       if the hex color is valid. Returns None if the hex color is invalid.
+    """
+    hex_color = hex_color.lstrip('#')
+    
+    # Check if the length of the string is valid for hex color (either 3 or 6 characters)
+    if len(hex_color) != 3 and len(hex_color) != 6:
+        return None
+    
+    # Check if all characters are valid hexadecimal digits
+    if not all(c in '0123456789ABCDEFabcdef' for c in hex_color):
+        return None
+    
+    # If the length is 3, expand the shorthand notation to 6 characters
+    if len(hex_color) == 3:
+        hex_color = ''.join(c * 2 for c in hex_color)
+    
+    # Convert hexadecimal to RGB
+    r = int(hex_color[0:2], 16)
+    g = int(hex_color[2:4], 16)
+    b = int(hex_color[4:6], 16)
+    
+    return (r, g, b)
```

### Comparing `nicotool-1.1/nico/ascii.py` & `nicotool-1.4.8.1/nicotool/ascii.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.1/nico/id.py` & `nicotool-1.4.8.1/nicotool/id.py`

 * *Files identical despite different names*

### Comparing `nicotool-1.1/nico/jsonify.py` & `nicotool-1.4.8.1/nicotool/jsonify.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             json.load(file)
         return True
     except (json.JSONDecodeError, IOError):
         return False
 
 
 
-def loadJson(filepath):
+def readJson(filepath):
     """
     Read JSON data from a file.
 
     Args:
     - filepath (str): The path of the file to read.
 
     Returns:
@@ -57,15 +57,14 @@
     - allow_overwrite (bool): Whether to allow overwriting an existing file (default False).
 
     Returns:
     - True if the file was successfully created, False otherwise.
     """
     filepath = os.path.join(path, filename)
     if os.path.exists(filepath) and not allow_overwrite:
-        print(f"Error: File '{filename}' already exists and allow_overwrite is set to False.")
         return False
     
     try:
         with open(filepath, 'w') as file:
             json.dump(data, file)
         return True
     except Exception as e:
```

