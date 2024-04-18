# Comparing `tmp/omero-scripts-5.8.0.tar.gz` & `tmp/omero-scripts-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-scripts-5.8.0.tar", last modified: Wed Mar 13 13:14:23 2024, max compression
+gzip compressed data, was "omero-scripts-5.8.1.tar", last modified: Thu Apr 18 13:19:00 2024, max compression
```

## Comparing `omero-scripts-5.8.0.tar` & `omero-scripts-5.8.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.698495 omero-scripts-5.8.0/omero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.698495 omero-scripts-5.8.0/omero/analysis_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    18644 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/analysis_scripts/Kymograph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/analysis_scripts/Kymograph_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/analysis_scripts/Plot_Profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/analysis_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.698495 omero-scripts-5.8.0/omero/annotation_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/annotation_scripts/KeyVal_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/annotation_scripts/KeyVal_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/annotation_scripts/Remove_KeyVal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/annotation_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/omero/export_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/export_scripts/Batch_Image_Export.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/export_scripts/Batch_ROI_Export.py
--rw-r--r--   0 runner    (1001) docker     (127)    26575 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/export_scripts/Make_Movie.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/export_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/omero/figure_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    24587 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/Movie_Figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30720 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/Movie_ROI_Figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    35622 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/ROI_Split_Figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31155 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/Split_View_Figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    26133 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/Thumbnail_Figure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/figure_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/omero/import_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/import_scripts/Populate_Metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/import_scripts/Populate_ROI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/import_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/omero/util_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/Channel_Offsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/Combine_Images.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/Dataset_To_Plate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/Images_From_ROIs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/Move_Annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/omero/util_scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/omero_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-13 13:14:23.000000 omero-scripts-5.8.0/omero_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-13 13:14:23.000000 omero-scripts-5.8.0/omero_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:14:23.000000 omero-scripts-5.8.0/omero_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:14:23.000000 omero-scripts-5.8.0/omero_scripts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 13:14:23.000000 omero-scripts-5.8.0/omero_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 13:14:23.702495 omero-scripts-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-13 13:14:21.000000 omero-scripts-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.645709 omero-scripts-5.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-18 13:19:00.645709 omero-scripts-5.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.637709 omero-scripts-5.8.1/omero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/analysis_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/analysis_scripts/Kymograph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/analysis_scripts/Kymograph_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/analysis_scripts/Plot_Profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/analysis_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/annotation_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/annotation_scripts/KeyVal_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/annotation_scripts/KeyVal_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/annotation_scripts/Remove_KeyVal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/annotation_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/export_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    22770 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/export_scripts/Batch_Image_Export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/export_scripts/Batch_ROI_Export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26575 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/export_scripts/Make_Movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/export_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/figure_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    24587 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/Movie_Figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30720 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/Movie_ROI_Figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35622 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/ROI_Split_Figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31155 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/Split_View_Figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26133 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/Thumbnail_Figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/figure_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/import_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/import_scripts/Populate_Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/import_scripts/Populate_ROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/import_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.641709 omero-scripts-5.8.1/omero/util_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/Channel_Offsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/Combine_Images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/Dataset_To_Plate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/Images_From_ROIs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/Move_Annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/omero/util_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:19:00.645709 omero-scripts-5.8.1/omero_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-18 13:19:00.000000 omero-scripts-5.8.1/omero_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-18 13:19:00.000000 omero-scripts-5.8.1/omero_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:19:00.000000 omero-scripts-5.8.1/omero_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:19:00.000000 omero-scripts-5.8.1/omero_scripts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 13:19:00.000000 omero-scripts-5.8.1/omero_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:19:00.645709 omero-scripts-5.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-18 13:18:55.000000 omero-scripts-5.8.1/setup.py
```

### Comparing `omero-scripts-5.8.0/PKG-INFO` & `omero-scripts-5.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-scripts
-Version: 5.8.0
+Version: 5.8.1
 Summary: OMERO scripts
 Home-page: https://github.com/ome/omero-scripts/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
 Download-URL: https://github.com/ome/omero-scripts/
 Platform: UNKNOWN
```

### Comparing `omero-scripts-5.8.0/README.rst` & `omero-scripts-5.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/analysis_scripts/Kymograph.py` & `omero-scripts-5.8.1/omero/analysis_scripts/Kymograph.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 from omero.gateway import BlitzGateway
 import omero
 import omero.util.script_utils as script_utils
 import omero.util.roi_handling_utils as roi_utils
 from omero.rtypes import rlong, rstring, robject, unwrap
 import omero.scripts as scripts
-from numpy import zeros, hstack, vstack, asarray, math
+from numpy import zeros, hstack, vstack, asarray
+import math
 import logging
 from PIL import Image
 from io import BytesIO
 
 logger = logging.getLogger('kymograph')
```

### Comparing `omero-scripts-5.8.0/omero/analysis_scripts/Kymograph_Analysis.py` & `omero-scripts-5.8.1/omero/analysis_scripts/Kymograph_Analysis.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/analysis_scripts/Plot_Profile.py` & `omero-scripts-5.8.1/omero/analysis_scripts/Plot_Profile.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/annotation_scripts/KeyVal_from_csv.py` & `omero-scripts-5.8.1/omero/annotation_scripts/KeyVal_from_csv.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/annotation_scripts/KeyVal_to_csv.py` & `omero-scripts-5.8.1/omero/annotation_scripts/KeyVal_to_csv.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/annotation_scripts/Remove_KeyVal.py` & `omero-scripts-5.8.1/omero/annotation_scripts/Remove_KeyVal.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/export_scripts/Batch_Image_Export.py` & `omero-scripts-5.8.1/omero/export_scripts/Batch_Image_Export.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/export_scripts/Batch_ROI_Export.py` & `omero-scripts-5.8.1/omero/export_scripts/Batch_ROI_Export.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/export_scripts/Make_Movie.py` & `omero-scripts-5.8.1/omero/export_scripts/Make_Movie.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/figure_scripts/Movie_Figure.py` & `omero-scripts-5.8.1/omero/figure_scripts/Movie_Figure.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/figure_scripts/Movie_ROI_Figure.py` & `omero-scripts-5.8.1/omero/figure_scripts/Movie_ROI_Figure.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/figure_scripts/ROI_Split_Figure.py` & `omero-scripts-5.8.1/omero/figure_scripts/ROI_Split_Figure.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/figure_scripts/Split_View_Figure.py` & `omero-scripts-5.8.1/omero/figure_scripts/Split_View_Figure.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/figure_scripts/Thumbnail_Figure.py` & `omero-scripts-5.8.1/omero/figure_scripts/Thumbnail_Figure.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/import_scripts/Populate_Metadata.py` & `omero-scripts-5.8.1/omero/import_scripts/Populate_Metadata.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/import_scripts/Populate_ROI.py` & `omero-scripts-5.8.1/omero/import_scripts/Populate_ROI.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/util_scripts/Channel_Offsets.py` & `omero-scripts-5.8.1/omero/util_scripts/Channel_Offsets.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/util_scripts/Combine_Images.py` & `omero-scripts-5.8.1/omero/util_scripts/Combine_Images.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/util_scripts/Dataset_To_Plate.py` & `omero-scripts-5.8.1/omero/util_scripts/Dataset_To_Plate.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/util_scripts/Images_From_ROIs.py` & `omero-scripts-5.8.1/omero/util_scripts/Images_From_ROIs.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero/util_scripts/Move_Annotations.py` & `omero-scripts-5.8.1/omero/util_scripts/Move_Annotations.py`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/omero_scripts.egg-info/PKG-INFO` & `omero-scripts-5.8.1/omero_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-scripts
-Version: 5.8.0
+Version: 5.8.1
 Summary: OMERO scripts
 Home-page: https://github.com/ome/omero-scripts/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
 Download-URL: https://github.com/ome/omero-scripts/
 Platform: UNKNOWN
```

### Comparing `omero-scripts-5.8.0/omero_scripts.egg-info/SOURCES.txt` & `omero-scripts-5.8.1/omero_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-scripts-5.8.0/setup.py` & `omero-scripts-5.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-version = '5.8.0'
+version = '5.8.1'
 url = "https://github.com/ome/omero-scripts/"
 
 setup(
     version=version,
     name='omero-scripts',
     packages=[
         'omero.analysis_scripts',
```

