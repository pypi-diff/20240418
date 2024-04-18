# Comparing `tmp/geodynamic-0.0.6.tar.gz` & `tmp/geodynamic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodynamic-0.0.6.tar", last modified: Wed Apr 17 10:50:39 2024, max compression
+gzip compressed data, was "geodynamic-0.0.7.tar", last modified: Thu Apr 18 15:04:55 2024, max compression
```

## Comparing `geodynamic-0.0.6.tar` & `geodynamic-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.565636 geodynamic-0.0.6/
--rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.6/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-17 10:50:39.565562 geodynamic-0.0.6/PKG-INFO
--rw-------   0 mac        (501) staff       (20)      415 2024-04-09 12:57:37.000000 geodynamic-0.0.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.559301 geodynamic-0.0.6/geodynamic/
--rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.6/geodynamic/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.562104 geodynamic-0.0.6/geodynamic/geo/
--rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.6/geodynamic/geo/__init__.py
--rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.6/geodynamic/geo/construction.py
--rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.6/geodynamic/geo/lib_commands.py
--rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.6/geodynamic/geo/lib_elements.py
--rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.6/geodynamic/geo/lib_vars.py
--rw-------   0 mac        (501) staff       (20)    31572 2024-04-17 10:49:55.000000 geodynamic-0.0.6/geodynamic/manim_dynamic.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.564345 geodynamic-0.0.6/geodynamic/parsers/
--rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.6/geodynamic/parsers/__init__.py
--rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.6/geodynamic/parsers/ggb_generator.py
--rw-------   0 mac        (501) staff       (20)     7314 2024-04-15 15:20:08.000000 geodynamic-0.0.6/geodynamic/parsers/ggb_parser.py
--rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.6/geodynamic/parsers/short_parser.py
--rw-rw-r--   0 mac        (501) staff       (20)     6043 2024-04-09 12:06:03.000000 geodynamic-0.0.6/geodynamic/parsers/svg_parser.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-17 10:50:39.565091 geodynamic-0.0.6/geodynamic.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1086 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-17 10:50:39.000000 geodynamic-0.0.6/geodynamic.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-17 10:50:39.566226 geodynamic-0.0.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-17 10:50:27.000000 geodynamic-0.0.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839944 geodynamic-0.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)       18 2024-04-05 12:40:59.000000 geodynamic-0.0.7/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-18 15:04:55.839872 geodynamic-0.0.7/PKG-INFO
+-rw-------   0 mac        (501) staff       (20)      428 2024-04-18 12:05:16.000000 geodynamic-0.0.7/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.834292 geodynamic-0.0.7/geodynamic/
+-rw-------   0 mac        (501) staff       (20)        0 2024-04-05 11:31:09.000000 geodynamic-0.0.7/geodynamic/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.837290 geodynamic-0.0.7/geodynamic/geo/
+-rw-------   0 mac        (501) staff       (20)        0 2023-12-28 13:25:09.000000 geodynamic-0.0.7/geodynamic/geo/__init__.py
+-rw-------   0 mac        (501) staff       (20)    10547 2024-04-13 15:38:56.000000 geodynamic-0.0.7/geodynamic/geo/construction.py
+-rw-------   0 mac        (501) staff       (20)    24312 2024-04-15 15:34:01.000000 geodynamic-0.0.7/geodynamic/geo/lib_commands.py
+-rw-------   0 mac        (501) staff       (20)    12974 2024-04-13 14:52:57.000000 geodynamic-0.0.7/geodynamic/geo/lib_elements.py
+-rw-------   0 mac        (501) staff       (20)     1752 2024-01-22 09:44:40.000000 geodynamic-0.0.7/geodynamic/geo/lib_vars.py
+-rw-------   0 mac        (501) staff       (20)    31503 2024-04-18 14:56:31.000000 geodynamic-0.0.7/geodynamic/manim_dynamic.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839166 geodynamic-0.0.7/geodynamic/parsers/
+-rw-rw-r--   0 mac        (501) staff       (20)      411 2024-04-08 16:07:59.000000 geodynamic-0.0.7/geodynamic/parsers/__init__.py
+-rw-------   0 mac        (501) staff       (20)    13622 2024-04-05 11:51:36.000000 geodynamic-0.0.7/geodynamic/parsers/ggb_generator.py
+-rw-------   0 mac        (501) staff       (20)     7380 2024-04-18 13:47:34.000000 geodynamic-0.0.7/geodynamic/parsers/ggb_parser.py
+-rw-------   0 mac        (501) staff       (20)     3344 2024-04-05 11:52:04.000000 geodynamic-0.0.7/geodynamic/parsers/short_parser.py
+-rw-rw-r--   0 mac        (501) staff       (20)     6514 2024-04-18 14:55:48.000000 geodynamic-0.0.7/geodynamic/parsers/svg_parser.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-18 15:04:55.839601 geodynamic-0.0.7/geodynamic.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1099 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      575 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       60 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2024-04-18 15:04:55.000000 geodynamic-0.0.7/geodynamic.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-18 15:04:55.840234 geodynamic-0.0.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      951 2024-04-18 12:05:38.000000 geodynamic-0.0.7/setup.py
```

### Comparing `geodynamic-0.0.6/PKG-INFO` & `geodynamic-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,16 @@
 1. Preparing code `test.py`:
 
 ```python
 from geodynamic.manim_dynamic import *
 
 class TestScene(GeoDynamic):
     def construct(self):       
-        self.loadGeoGebra('test.ggb', scheme = 'pandora', px_size = [400, 300])    
-        self.exportSVG('test_ggb.svg')
+        self.loadGeoGebra('test.ggb', style_json_file = 'pandora.json', px_size = [400, 'auto'])    
+        self.exportSVG('test.svg')
 ```
 
 2. Run compilation:
 
 ```bash
 manim 'test.py' TestScene
 ```
```

### Comparing `geodynamic-0.0.6/geodynamic/geo/construction.py` & `geodynamic-0.0.7/geodynamic/geo/construction.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/geo/lib_commands.py` & `geodynamic-0.0.7/geodynamic/geo/lib_commands.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/geo/lib_elements.py` & `geodynamic-0.0.7/geodynamic/geo/lib_elements.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/geo/lib_vars.py` & `geodynamic-0.0.7/geodynamic/geo/lib_vars.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/manim_dynamic.py` & `geodynamic-0.0.7/geodynamic/manim_dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,195 +7,184 @@
 from .parsers.svg_parser import *
 from .parsers import short_parser, ggb_parser
 
 import xml.etree.ElementTree as ET
 
 #--------------------------------------------------------------------------
 
-#стилевик от Пандоры
-style_pandora = {}
-
-style_pandora['dot'] = {}
-style_pandora['line'] = {}
-style_pandora['angle'] = {}
-style_pandora['strich'] = {}
-style_pandora['color'] = {}
-
-style_pandora['dot']['main'] = 7
-style_pandora['dot']['bold'] = 9
-style_pandora['dot']['aux'] = 5
-
-style_pandora['line']['main'] = 2
-style_pandora['line']['bold'] = 2.5
-style_pandora['line']['aux'] = 1.5
-
-style_pandora['angle']['line'] = 1
-style_pandora['angle']['r_default'] = 12.5
-style_pandora['angle']['r_shift'] = 1.5
-style_pandora['angle']['r_right'] = 10
-
-style_pandora['strich']['width'] = 2
-style_pandora['strich']['len'] = 12
-style_pandora['strich']['shift'] = 4
-
-style_pandora['color']['black'] = '#000000'
-style_pandora['color']['main'] = '#2581b5'
-style_pandora['color']['light'] = '#bef3fc'
-style_pandora['color']['aux'] = '#000000'
-style_pandora['color']['acc'] = '#ef60ab'
-style_pandora['color']['acc_light'] = '#ffd2ee'
-
 def isnan(x):
-    if isinstance(x, str):
+    if isinstance(x, (int, float)): return False
+    else:
         try:
             y = float(x)
             return False
         except:
             return True
-    else:
-        return not isinstance(x, (int, float))
 
 def CorrectSVG(svg_path):
     #tree = ET.parse(svg_path)
 
     #for elem in tree.findall(f'.//{xmlns}text'):
     #    elem.set('font-style', 'italic')
 
     #tree.write(svg_path, encoding = "UTF-8", xml_declaration = False)
     return
 
 class GeoStyle:
-    def __init__(self, style_json_file = None, scheme = None, color = 'blue', theme = 'light', px_size = [1920, 1080], crop_padding = None):
+    def __init__(self, style_json_file = None, px_size = [1920, 1080]):
         self.dot_size = 0.17   
         self.line_width = 6   
         self.ang_width = 0.75 * self.line_width
         self.strich_rshift = 0.14
         self.ang_rshift = 0.75 * self.strich_rshift
         self.strich_len = 0.45
         self.strich_width = 6
         self.ang_rdefault = 0.8
         self.ang_right = 0.65
         
         self.background = WHITE
         self.strong = BLACK
+        self.col_gray = '#eeeeee'
+
+        self.col = '#6688c2'
+        self.col_light = '#dee7f5'
+        self.col_accent = '#d05456'
+        self.col_accent_light = '#f6e0db'
+        
+        self.technic = {}
         
         if style_json_file is not None:
             style_json = json.loads(open(style_json_file, 'r').read())
-            scheme = style_json['name']
-            
-            if scheme == 'pandora':
-                global style_pandora
-                style_pandora = style_json['style']
-                #print(style_pandora)
-
-        if scheme == 'pandora':            
-            self.convert_pandora_to_manim()
-            
-        else:
-            if theme == 'dark':
-                self.background = BLACK
-                self.strong = WHITE
-                self.col_gray = '#282828'
-
-                if color == 'white':
-                    self.col = '#ffffff'
-                    self.col_light = '#333333'
-                    self.col_accent = '#db4251'
-                    self.col_accent_light = '#68383f'
-                elif color == 'purple':
-                    self.background = '#151324'
-                    self.col = '#9f9fdd'
-                    self.col_light = '#3c3766'
-                    self.col_accent = '#db4251'
-                    self.col_accent_light = '#542f36'
-                    self.col_gray = '#211f2f'
-
-            else:
-                self.background = WHITE
-                self.strong = BLACK
-
-                if color == 'green':
-                    self.col = '#80be8c'
-                    self.col_light = '#e3efdb'
-                    self.col_accent = '#d05456'
-                    self.col_accent_light = '#f6e0db'
-                elif color == 'orange':
-                    self.col = '#d97c2c'
-                    self.col_light = '#fae7ca'
-                    self.col_accent = '#72a6d9'
-                    self.col_accent_light = '#d8edfb'
-                elif color == 'purple':
-                    self.col = '#8670ac'
-                    self.col_light = '#e8e3f0'
-                    self.col_accent = '#d05456'
-                    self.col_accent_light = '#f6e0db'
-                else: #blue
-                    self.col = '#6688c2'
-                    self.col_light = '#dee7f5'
-                    self.col_accent = '#d05456'
-                    self.col_accent_light = '#f6e0db'
-
-                self.col_gray = '#eeeeee'
+             
+            if style_json['name'] == 'pandora':
+                self.convert_from_pandora(style_json)                
         
         #параметры окна отображения 
         # размеры width и height в px
         # положение начала координат xZero и yZero
         # масштаб scale в px для 0.5 unit
         self.view = {}
         if px_size is not None:
-            self.view['width'], self.view['height'] = px_size[0], px_size[1]
+            q = self.technic['scale_export'] if 'scale_export' in self.technic else 1
+            self.view['width'] = float(px_size[0]) * q if not isnan(px_size[0]) else None
+            self.view['height'] = float(px_size[1]) * q if not isnan(px_size[1]) else None
 
-    def convert_pandora_to_manim(self):
-        self.dot_size = 0.02 * style_pandora['dot']['main']
-        self.line_width = 2 * style_pandora['line']['main']
-        self.ang_width = 2 * style_pandora['angle']['line']
-        self.ang_rshift = 2 * style_pandora['angle']['r_shift']
-        self.ang_rdefault = 0.02 * style_pandora['angle']['r_default']
-        self.ang_right = 0.02 * style_pandora['angle']['r_right']
-        self.strich_width = 2 * style_pandora['strich']['width']
-        self.strich_len = 0.02 * style_pandora['strich']['len']
-        self.strich_rshift = 0.02 * style_pandora['strich']['shift']
+    def convert_from_pandora(self, style_map):
+        style = style_map['style']
+        
+        self.dot_size = 0.02 * style['dot']['main']
+        self.line_width = 2 * style['line']['main']
+        self.ang_width = 2 * style['angle']['line']
+        self.ang_rshift = 2 * style['angle']['r_shift']
+        self.ang_rdefault = 0.02 * style['angle']['r_default']
+        self.ang_right = 0.02 * style['angle']['r_right']
+        self.strich_width = 2 * style['strich']['width']
+        self.strich_len = 0.02 * style['strich']['len']
+        self.strich_rshift = 0.02 * style['strich']['shift']
         
         self.background = '#ffffff'
-        self.col = style_pandora['color']['main']
-        self.col_light = style_pandora['color']['light']
-        self.col_accent = style_pandora['color']['acc']
-        self.col_accent_light = style_pandora['color']['acc_light']
+        self.col = style['color']['main']
+        self.col_light = style['color']['light']
+        self.col_accent = style['color']['acc']
+        self.col_accent_light = style['color']['acc_light']
         self.col_gray = '#eeeeee'
+        
+        self.technic = style_map['technic']
 
     def setViewByGeo(self, geoView):
         w0, h0 = self.view['width'], self.view['height']
         w, h = geoView['width'], geoView['height']
         if isnan(w0) & isnan(h0): 
             print("ERROR: width and heigth haven't been set")
+            return
         elif isnan(w0):
             #print(w0, h0, w, h)
             w0 = float(h0) * w / h
             self.view['width'] = w0
         elif isnan(h0):
             #print(w0, h0, w, h)
             h0 = float(w0) * h / w
             self.view['height'] = h0
             
         q = min(w0/w, h0/h)
         
         self.view['scale'] = geoView['scale'] * q
         self.view['xZero'] = geoView['xZero'] * q + (w0 - q * w) / 2
         self.view['yZero'] = geoView['yZero'] * q + (h0 - q * h) / 2
+        
+        
+def MakeGeoStyle(color = "blue", theme = "light", px_size = [1920, 1080]):
+    style = GeoStyle(px_size = px_size)
+    
+    if theme == 'dark':
+        style.background = BLACK
+        style.strong = WHITE
+        style.col_gray = '#282828'
+
+        if color == 'white':
+            style.col = '#ffffff'
+            style.col_light = '#333333'
+            style.col_accent = '#db4251'
+            style.col_accent_light = '#68383f'
+        elif color == 'purple':
+            style.background = '#151324'
+            style.col = '#9f9fdd'
+            style.col_light = '#3c3766'
+            style.col_accent = '#db4251'
+            style.col_accent_light = '#542f36'
+            style.col_gray = '#211f2f'
+
+    else:
+        style.background = WHITE
+        style.strong = BLACK
+        style.col_gray = '#eeeeee'
+
+        if color == 'green':
+            style.col = '#80be8c'
+            style.col_light = '#e3efdb'
+            style.col_accent = '#d05456'
+            style.col_accent_light = '#f6e0db'
+        elif color == 'orange':
+            style.col = '#d97c2c'
+            style.col_light = '#fae7ca'
+            style.col_accent = '#72a6d9'
+            style.col_accent_light = '#d8edfb'
+        elif color == 'purple':
+            style.col = '#8670ac'
+            style.col_light = '#e8e3f0'
+            style.col_accent = '#d05456'
+            style.col_accent_light = '#f6e0db'
+        else: #blue
+            style.col = '#6688c2'
+            style.col_light = '#dee7f5'
+            style.col_accent = '#d05456'
+            style.col_accent_light = '#f6e0db'
+            
+    return style
+
+def updateMin(minX, x):
+    if isnan(minX): return x
+    if isnan(x): return minX
+    return min(minX, x)
+      
+def updateMax(maxX, x):
+    if isnan(maxX): return x
+    if isnan(x): return maxX
+    return max(maxX, x)
 
 #--------------------------------------------------------------------------
 
 class GeoDynamic(MovingCameraScene):
-    style_default = GeoStyle(color = 'blue', theme = 'light')
+    style_default = MakeGeoStyle(color = 'blue', theme = 'light')
 
     def __init__(self):
         super().__init__()
         self.obj = {}                       #хранение объектов сцены mobjects obj[name] = MObject
         self.geo = geo.Construction()
-        self.style = GeoStyle(color = 'blue')
+        self.style = GeoStyle()
 
         self._styles_back = {}
         self._gray_mobjects = {}
 
         self.cuts = 0
 
     def mobject(self, name):
@@ -225,23 +214,28 @@
             [geo.Point]
         ]
 
         for el_types in element_types:
             for el in self.geo.elements: 
                 if type(el.data) in el_types: self.addGeoElement(el, show) 
  
-    def getAllGeometryBounds(self):
+    def getAllGeometryBounds(self, scale = 1):
         bounds = [None,None,None,None]
         for elem in self.geo.elements: 
             if elem.visible:
                 mobj = CreateMObject(elem, z_auto = True)
                 if mobj is not None:
-                    #!здесь нужно проверить границы элемента и расширить bounds по необходимости
-                    x = 0
+                    bounds[0] = updateMin(bounds[0], mobj.get_left()[0])
+                    bounds[1] = updateMin(bounds[1], mobj.get_bottom()[1])
+                    bounds[2] = updateMax(bounds[2], mobj.get_right()[0])
+                    bounds[3] = updateMax(bounds[3], mobj.get_top()[1])
+        
+        for i in range(4): bounds[i] *= scale
                     
+        return bounds
 
     #пауза для обрезки видео + отображение ярлыка слева
     def waitCut(self, msg = None, **kwargs):
         self.cuts += 1
 
         rect = Rectangle(color = RED, fill_opacity = 1, height = self.camera.frame_height, width = self.camera.frame_width/4).move_to(self.camera.frame_center).shift( (3/8) * self.camera.frame_width * LEFT)
         txt = Text(str(msg) if msg is not None else str(self.cuts)).set_color(BLACK).scale(3).move_to(rect)
@@ -284,32 +278,41 @@
             if not el.visible: 
                 mobj.set_opacity(0)
 
     def loadGeometry(self, filepath, update = False, debug = False):
         short_parser.loadCode(self.geo, filepath, update = update, debug = debug)
         self.geo.rebuild(debug = debug)
 
-    def loadGeoGebra(self, filepath, style_json_file = None, scheme = 'pandora', px_size = None, crop_padding = None, debug = False):
+    def loadGeoGebra(self, filepath, style_json_file = None, px_size = None, debug = False):
         self.geo = ggb_parser.load(filepath, debug = debug) 
         self.geo.rebuild(debug = debug)
         
-        style = GeoStyle(style_json_file = style_json_file, scheme = scheme, px_size = px_size, crop_padding = crop_padding)
+        style = GeoStyle(style_json_file = style_json_file, px_size = px_size)
+        
+        bounds = self.getAllGeometryBounds(self.geo.style['view']['scale'])
+        padding = style.technic['crop_padding'] if 'crop_padding' in style.technic else 10
+        
+        print('BOUNDS:', bounds)
         
-        if crop_padding is not None:
-            print('This method is going to be realized soon.')    
+        self.geo.style['view']['width'] = bounds[2] - bounds[0] + 2 * padding
+        self.geo.style['view']['height'] = bounds[3] - bounds[1] + 2 * padding
+        self.geo.style['view']['xZero'] = -bounds[0] + padding
+        self.geo.style['view']['yZero'] = bounds[3] + padding
         
         if px_size is not None:
             style.setViewByGeo(self.geo.style['view'])
         else:
             style.view = self.geo.style['view']
 
         view = style.view
         scale = view['scale']
+        scale_export = style.technic['scale_export'] if 'scale_export' in style.technic else 1
+        q = 50 * scale_export / scale
         for key in ['dot_size', 'line_width', 'ang_width', 'ang_rdefault', 'ang_right', 'ang_rshift', 'strich_rshift', 'strich_len']:
-            style.__setattr__(key, getattr(style, key) * 50 / scale)
+            setattr(style, key, getattr(style, key) * q)
 
         self.camera.frame.set(width = view['width'] / scale)
         dx = self.camera.frame.width / 2 - view['xZero'] / scale
         dy = view['height'] / (2 * scale) - view['yZero'] / scale      
         self.camera.frame.shift(dx * RIGHT + dy * DOWN)
 
         self.setStyle(style)
@@ -349,15 +352,15 @@
     def exportSVG(self, filepath):
         #config.frame_height = self.camera.frame.get_height()
         #config.frame_width = self.camera.frame.get_width()
         #scale = 2 * self.style['view']['scale']
         #config.frame_width, config.frame_height = self.style['view']['width'] / scale, self.style['view']['height'] / scale
         #config.__setattr__('frame_center', self.camera.frame.get_center())
         config.__setattr__('ggb_view', self.style.view)
-        VGroup(*self.mobjects).to_svg(filepath)
+        VGroup(*self.mobjects).to_svg(filepath, self.style.technic)
     
     def addGrid(self, x_range=(-10, 10, 1), y_range=(-10, 10, 1)):
         grid = NumberPlane(
             x_range = x_range,
             y_range = y_range,
             x_length = x_range[1] - x_range[0],
             y_length = y_range[1] - y_range[0],
```

### Comparing `geodynamic-0.0.6/geodynamic/parsers/ggb_generator.py` & `geodynamic-0.0.7/geodynamic/parsers/ggb_generator.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/parsers/ggb_parser.py` & `geodynamic-0.0.7/geodynamic/parsers/ggb_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,16 @@
                 if elem is not None:
                     r, g, b, a = int(elem.attrib['r']), int(elem.attrib['g']), int(elem.attrib['b']), float(elem.attrib['alpha'])
                     if xelem.attrib['type'] in ['angle', 'polygon', 'arc', 'conic']:
                         style[name]['fill'] = rgb_to_hex(r, g, b)
                         style[name]['fill_opacity'] = a
                     lineStyle = xelem.find("lineStyle")
                     if lineStyle is not None:
-                        thick, tt, op = lineStyle.attrib['thickness'], lineStyle.attrib['type'], float(lineStyle.attrib['opacity'])
+                        thick, tt = lineStyle.attrib['thickness'], lineStyle.attrib['type']
+                        op = float(lineStyle.attrib['opacity']) if 'opacity' in lineStyle.attrib else 255
                         if xelem.attrib['type'] in ['angle', 'segment', 'arc', 'conic']:
                             style[name]['stroke'] = rgb_to_hex(r, g, b)
                             #style[name]['stroke_opacity'] = op / 255
                             #style[name]['stroke_width'] = thick
                             if int(tt) > 0: style[name]['stroke_dash'] = 0.65
                         
         if xelems_left_to_pass:
```

### Comparing `geodynamic-0.0.6/geodynamic/parsers/short_parser.py` & `geodynamic-0.0.7/geodynamic/parsers/short_parser.py`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/geodynamic/parsers/svg_parser.py` & `geodynamic-0.0.7/geodynamic/parsers/svg_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         pat = cairo.LinearGradient(*it.chain(*(point[:2] for point in points)))
         step = 1.0 / (len(rgbas) - 1)
         offsets = np.arange(0, 1 + step, step)
         for rgba, offset in zip(rgbas, offsets):
             pat.add_color_stop_rgba(offset, *rgba)
         ctx.set_source(pat)
 
-def _apply_stroke(ctx: cairo.Context, vmobject: VMobject, background: bool = False):
+def _apply_stroke(ctx: cairo.Context, vmobject: VMobject, background: bool = False, technic = None):
     from manim import config
 
     width = vmobject.get_stroke_width(background)
     if width == 0:
         return
     _set_cairo_context_color(
         ctx,
@@ -89,19 +89,28 @@
     )
     ctx.set_line_width(
         width
         * CAIRO_LINE_WIDTH_MULTIPLE
         # This ensures lines have constant width as you zoom in on them.
         * (config.frame_width / config.frame_width),
     )
+    if technic is not None:
+        linecap = {
+            "auto": cairo.LINE_CAP_BUTT,
+            "butt": cairo.LINE_CAP_BUTT,
+            "round": cairo.LINE_CAP_ROUND,
+            "square": cairo.LINE_CAP_SQUARE
+        }
+        ctx.set_line_cap(linecap[technic['line_caps']])
+    
     # if vmobject.joint_type != LineJointType.AUTO:
     #     ctx.set_line_join(LINE_JOIN_MAP[vmobject.joint_type])
     ctx.stroke_preserve()
 
-def _apply_fill(ctx: cairo.Context, vmobject: VMobject):
+def _apply_fill(ctx: cairo.Context, vmobject: VMobject, technic = None):
     """Fills the cairo context
     Parameters
     ----------
     ctx
         The cairo context
     vmobject
         The VMobject
@@ -114,15 +123,15 @@
         ctx,
         vmobject.get_fill_rgbas(),
         vmobject,
     )
     ctx.fill_preserve()
     return
 
-def _create_svg_from_vmobject_internal(vmobject: VMobject, ctx: cairo.Content):
+def _create_svg_from_vmobject_internal(vmobject: VMobject, ctx: cairo.Content, technic = None):
     # check if points are valid
     points = vmobject.points
     points = _transform_points_pre_display(points)
     if len(points) == 0:
         return
     ctx.new_path()
     subpaths = vmobject.gen_subpaths_from_points_2d(points)
@@ -132,21 +141,22 @@
         start = subpath[0]
         ctx.move_to(*start[:2])
         for _p0, p1, p2, p3 in quads:
             ctx.curve_to(*p1[:2], *p2[:2], *p3[:2])
         if vmobject.consider_points_equals_2d(subpath[0], subpath[-1]):
             ctx.close_path()
 
-    _apply_stroke(ctx, vmobject, background=True)
-    _apply_fill(ctx, vmobject)
-    _apply_stroke(ctx, vmobject)
+    _apply_stroke(ctx, vmobject, background=True, technic = technic)
+    _apply_fill(ctx, vmobject, technic = technic)
+    _apply_stroke(ctx, vmobject, technic = technic)
 
 def create_svg_from_vmobject(
     vmobject: VMobject,
-    file_name: str | Path = None
+    file_name: str | Path = None,
+    technic = None
 ) -> Path:
     """create_svg_from_vmobject creates an svg from a VMobject.
 
     Parameters
     ----------
     vmobject : VMobject
         The VMobject to create an svg from.
@@ -165,20 +175,21 @@
     """
 
     if file_name is None:
         file_name = tempfile.mktemp(suffix=".svg")
     file_name = Path(file_name).absolute()
     with _get_cairo_context(file_name) as ctx:
         for _vmobject in extract_mobject_family_members([vmobject], True, True):
-            _create_svg_from_vmobject_internal(_vmobject, ctx)
+            _create_svg_from_vmobject_internal(_vmobject, ctx, technic = technic)
     return file_name
 
 def create_svg_from_vgroup(
     vgroup: VGroup,
-    file_name: str | Path = None
+    file_name: str | Path = None,
+    technic = None
 ) -> Path:
     """create_svg_from_vgroup creates an svg from a VGroup.
 
     Parameters
     ----------
     vgroup : VGroup
         The VGroup to create the svg from.
@@ -199,9 +210,9 @@
         file_name = tempfile.mktemp(suffix=".svg")
     file_name = Path(file_name).absolute()
     with _get_cairo_context(file_name) as ctx:
         # a vgroup is a list of VMobjects which may contain other VGroups
         # flatten the vgroup to get a list of VMobjects
         vgroup = extract_mobject_family_members(vgroup, True, True)
         for vmobject in vgroup:
-            _create_svg_from_vmobject_internal(vmobject, ctx)
+            _create_svg_from_vmobject_internal(vmobject, ctx, technic = technic)
     return file_name
```

### Comparing `geodynamic-0.0.6/geodynamic.egg-info/PKG-INFO` & `geodynamic-0.0.7/geodynamic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodynamic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG
 Home-page: https://gitlab.mathem.ru/
 Author: ivaleo
 Author-email: ivaleotion@gmail.com
 Keywords: geometry dynamic geogebra manim animation svg python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,16 @@
 1. Preparing code `test.py`:
 
 ```python
 from geodynamic.manim_dynamic import *
 
 class TestScene(GeoDynamic):
     def construct(self):       
-        self.loadGeoGebra('test.ggb', scheme = 'pandora', px_size = [400, 300])    
-        self.exportSVG('test_ggb.svg')
+        self.loadGeoGebra('test.ggb', style_json_file = 'pandora.json', px_size = [400, 'auto'])    
+        self.exportSVG('test.svg')
 ```
 
 2. Run compilation:
 
 ```bash
 manim 'test.py' TestScene
 ```
```

### Comparing `geodynamic-0.0.6/geodynamic.egg-info/SOURCES.txt` & `geodynamic-0.0.7/geodynamic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geodynamic-0.0.6/setup.py` & `geodynamic-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='geodynamic',
-  version='0.0.6',
+  version='0.0.7',
   author='ivaleo',
   author_email='ivaleotion@gmail.com',
   description='Geometric tools for parsing GeoGebra construction, proccess with manim animation and export to SVG',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://gitlab.mathem.ru/',
   packages=find_packages(),
```

