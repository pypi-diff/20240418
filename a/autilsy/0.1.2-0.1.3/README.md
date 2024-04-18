# Comparing `tmp/autilsy-0.1.2.tar.gz` & `tmp/autilsy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autilsy-0.1.2.tar", last modified: Mon Mar 25 13:33:36 2024, max compression
+gzip compressed data, was "autilsy-0.1.3.tar", last modified: Thu Apr 18 13:56:07 2024, max compression
```

## Comparing `autilsy-0.1.2.tar` & `autilsy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-25 13:33:36.655336 autilsy-0.1.2/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      174 2024-03-25 13:33:36.655336 autilsy-0.1.2/PKG-INFO
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-25 13:33:36.651336 autilsy-0.1.2/autilsy/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-17 09:58:08.000000 autilsy-0.1.2/autilsy/__init__.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     2790 2024-03-24 08:13:18.000000 autilsy-0.1.2/autilsy/annots.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)    18851 2024-03-24 11:28:08.000000 autilsy-0.1.2/autilsy/common.py
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     1927 2024-03-24 13:04:08.000000 autilsy-0.1.2/autilsy/ui.py
-drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-25 13:33:36.655336 autilsy-0.1.2/autilsy.egg-info/
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      174 2024-03-25 13:33:35.000000 autilsy-0.1.2/autilsy.egg-info/PKG-INFO
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      232 2024-03-25 13:33:36.000000 autilsy-0.1.2/autilsy.egg-info/SOURCES.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        1 2024-03-25 13:33:35.000000 autilsy-0.1.2/autilsy.egg-info/dependency_links.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       97 2024-03-25 13:33:36.000000 autilsy-0.1.2/autilsy.egg-info/requires.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        8 2024-03-25 13:33:36.000000 autilsy-0.1.2/autilsy.egg-info/top_level.txt
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       38 2024-03-25 13:33:36.655336 autilsy-0.1.2/setup.cfg
--rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      384 2024-03-25 13:32:27.000000 autilsy-0.1.2/setup.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 13:56:07.871737 autilsy-0.1.3/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      174 2024-04-18 13:56:07.871737 autilsy-0.1.3/PKG-INFO
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 13:56:07.867737 autilsy-0.1.3/autilsy/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-03-17 09:58:08.000000 autilsy-0.1.3/autilsy/__init__.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     2790 2024-03-24 08:13:18.000000 autilsy-0.1.3/autilsy/annots.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)    22350 2024-04-18 13:50:17.000000 autilsy-0.1.3/autilsy/common.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 13:56:07.871737 autilsy-0.1.3/autilsy/resource/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-04 13:46:33.000000 autilsy-0.1.3/autilsy/resource/__init__.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)   705306 2024-04-04 13:46:33.000000 autilsy-0.1.3/autilsy/resource/image_bytes.py
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)     9995 2024-04-04 14:04:14.000000 autilsy-0.1.3/autilsy/ui.py
+drwxrwxr-x   0 yinyunjie  (1000) yinyunjie  (1000)        0 2024-04-18 13:56:07.871737 autilsy-0.1.3/autilsy.egg-info/
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      174 2024-04-18 13:56:06.000000 autilsy-0.1.3/autilsy.egg-info/PKG-INFO
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      293 2024-04-18 13:56:07.000000 autilsy-0.1.3/autilsy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        1 2024-04-18 13:56:06.000000 autilsy-0.1.3/autilsy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      119 2024-04-18 13:56:07.000000 autilsy-0.1.3/autilsy.egg-info/requires.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)        8 2024-04-18 13:56:07.000000 autilsy-0.1.3/autilsy.egg-info/top_level.txt
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)       38 2024-04-18 13:56:07.871737 autilsy-0.1.3/setup.cfg
+-rw-rw-r--   0 yinyunjie  (1000) yinyunjie  (1000)      412 2024-04-18 13:54:20.000000 autilsy-0.1.3/setup.py
```

### Comparing `autilsy-0.1.2/autilsy/annots.py` & `autilsy-0.1.3/autilsy/annots.py`

 * *Files identical despite different names*

### Comparing `autilsy-0.1.2/autilsy/common.py` & `autilsy-0.1.3/autilsy/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 import os
 import imutils, imutils.paths
 import json
 import xml.etree.ElementTree as ET
 import uuid
 import cv2
 import numpy as np
+import scipy.interpolate
 import shutil
 from tqdm import tqdm
 import random
 from tabulate import tabulate
 from moviepy.video.io.bindings import mplfig_to_npimage
+from easydict import EasyDict as edict
+import yaml
 
 from shapely.geometry import Point, Polygon, LineString
 from PIL import Image
 from PIL import ImageFont
 from PIL import ImageDraw 
 
 from sklearn.pipeline import make_pipeline
@@ -147,14 +150,34 @@
         """
         if not self.IsFilePath(xml_path): return None
 
         tree = ET.parse(xml_path)
         root_node = tree.getroot()
 
         return root_node
+
+    def ReadYMLFile(self, yml_path:str):
+        """
+        Read yaml file data to dict.
+        args:
+            yml_path: yaml file path
+        """
+        cfg = yaml.load(open(yml_path, 'r').read(), Loader=yaml.FullLoader)
+        cfg = edict(cfg)
+        return cfg
+
+    def WriteYML(self, data:dict, yml_path):
+        """
+        Write dict data to yaml file.
+        args:
+            data: data to write file.
+            yml_path: yaml save path.
+        """
+        with open(yml_path, 'w') as yaml_file:
+            yaml.dump(data, yaml_file, default_flow_style=False, sort_keys=False)
     
     def MkDir(self, dir_path:str)->None:
         """
         args:
             dir_path: directory of want to create
         return:
             None
@@ -188,14 +211,41 @@
         args:
             js_data: json format data
             save_path: json file path
         """
         with open(save_path, "w", encoding='utf-8') as f:
             json.dump(js_data, f, indent=4, ensure_ascii=False)
 
+    def ConcateTxts(self, txt_paths:list[str], dst_path:str, mode="rewrite"):
+        """
+        merge all contents of some txt files to a new txt file.
+        
+        args:
+            txt_paths: list of source txt file paths.
+            dst_path:  path of output txt file.
+            mode: write output file's mode.
+             ('rewrite': create a new file; 'append': append conents to the output file.)
+
+        """
+        assert mode in ["rewrite", "append"]
+
+        src_lines = []
+        for txt_path in txt_paths:
+            assert self.IsFilePath(txt_path), "{} invalid".format(txt_path)
+            with open(txt_path, 'r') as f:
+                src_lines.extend(list(f.readlines()))
+
+        if not self.IsDirPath(os.path.dirname(dst_path)):
+            self.MkDir(os.path.dirname(dst_path))
+            print("Output directory have maked.")
+        
+        open_mode = 'w' if mode == "rewrite" else "a+"
+        with open(dst_path, open_mode) as f:
+            for line in src_lines:
+                f.write(line)
    
     #-----math
     def CalTwoPtsDist(self,p1, p2)->float:
         """
         args:
             p1, p2: two points.
         return:
@@ -325,14 +375,59 @@
         fit_xy = np.poly1d(fit_param)
         pts = []
         for y in range(int(ys[0]),int(ys[-1]) , 1):
             pts.append((fit_xy(y), y))
 
         return pts
 
+    def Inter1dV2(self, xs:list, ys:list, dst_xs:list, dst_ys:list, indep_dim="y", inter_every=True, inter_step=1):
+        """
+        interpolate points among [(x1,y1), (x2,y2),...,(xn,yn)]
+        args:
+            xs: x values of all points.
+            ys: y values of all points.
+            dst_xs: interpolated x values.
+            dst_ys: interpolated y values.
+            indep_dim: value in ["x", "y"].
+            inter_every: interpolate evey two points iteratively.
+            inter_step: interpolate step.
+        """
+        assert indep_dim in ["x", "y"]
+        assert len(xs) >=2 and len(ys) >=2
+        assert isinstance(dst_xs, list) and isinstance(dst_ys, list)
+
+        xs_parts, ys_parts = [],[]
+        if inter_every:
+            for i in range(len(xs)-1):
+                xs_parts.append([xs[i], xs[i+1]])
+                ys_parts.append([ys[i], ys[i+1]])
+        else:
+            xs_parts.append(xs)
+            ys_parts.append(ys)
+
+        for xs_part, ys_part in zip(xs_parts, ys_parts):
+            if indep_dim == "x":
+                indep_var = xs_part
+                dep_var = ys_part
+            else:
+                indep_var = ys_part
+                dep_var = xs_part
+
+            inter_func = scipy.interpolate.interp1d(indep_var, dep_var)
+            step = inter_step if indep_var[0] < indep_var[1] else -1*inter_step
+            for idx in range(indep_var[0], indep_var[-1], step):
+                if indep_dim == "x":
+                    dst_xs.append(idx)
+                    dst_ys.append(float(inter_func(idx)))
+                else:
+                    dst_xs.append(float(inter_func(idx)))
+                    dst_ys.append(idx)
+        dst_xs.append(xs[-1])
+        dst_ys.append(ys[-1])
+
     def RefineLine(self,line, poly_factor, fit_method="RANSAC"):
         """
         args:
             line: a list of points.
             poly_facotr: 1,2,3...
             fit_method: "RANSAC", "HuberRegressor","Theil_Sen","OLS"
         return:
@@ -364,15 +459,15 @@
     def ConvertPILimg2numpy(self, pil_img):
         """
         convert pillow image to opencv image format
         args:
             pil_img: pillow format image.
         """
         opencvImage = cv2.cvtColor(np.array(pil_img), cv2.COLOR_RGB2BGR)
-        
+
         return opencvImage
 
     def convertFigure2numpy(self, figure):
         """
         convert matplot figure to opencv image format.
         args:
             figure: matplot format figure.
@@ -593,8 +688,11 @@
                 cv2.waitKey(0)
             elif key == 113: #"q" (quit):
                 print("exit!")
                 break
             else:
                 print("Invalid key!")
                 continue
+
+if __name__ == "__main__":
+    autil = Autils()
```

