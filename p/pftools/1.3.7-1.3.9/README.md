# Comparing `tmp/pftools-1.3.7.tar.gz` & `tmp/pftools-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pftools-1.3.7.tar", last modified: Wed Feb 15 23:19:24 2023, max compression
+gzip compressed data, was "dist/pftools-1.3.9.tar", last modified: Fri Mar  3 21:28:24 2023, max compression
```

## Comparing `pftools-1.3.7.tar` & `pftools-1.3.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.703226 pftools-1.3.7/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     3922 2023-02-15 23:16:31.000000 pftools-1.3.7/CHANGELOG.md
--rw-rw----   0 smithsg   (5319) smithsg   (5319)       48 2023-02-15 23:16:31.000000 pftools-1.3.7/MANIFEST.in
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     7068 2023-02-15 23:19:24.704218 pftools-1.3.7/PKG-INFO
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     5519 2023-02-15 23:16:31.000000 pftools-1.3.7/README.md
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.532033 pftools-1.3.7/parflow/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      281 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/__init__.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.544336 pftools-1.3.7/parflow/cli/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/cli/__init__.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1094 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/cli/pfdist_sort.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     3931 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/cli/tcl2py.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.598298 pftools-1.3.7/parflow/tools/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      300 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/__init__.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    54981 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/builders.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    17617 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/core.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.623010 pftools-1.3.7/parflow/tools/database/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/database/__init__.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    30436 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/database/core.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    19937 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/database/domains.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)   307539 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/database/generated.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     7564 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/database/handlers.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    22288 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/export.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     2730 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/fs.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     5094 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/helper.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    19650 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/hydrology.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    66816 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/io.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)    25846 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/pf_backend.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.656337 pftools-1.3.7/parflow/tools/ref/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      384 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/default_vegp_values.json
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1652 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/subsurface_conus_1.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      971 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/subsurface_freeze_cherry.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1417 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/subsurface_washita.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     7023 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/table_keys.yaml
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1128 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/vegp_header.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     4431 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/vegp_igbp.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     2685 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/ref/vegp_keys.yaml
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1733 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/settings.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      675 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/terminal.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.667334 pftools-1.3.7/parflow/tools/tests/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/tests/__init__.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.673225 pftools-1.3.7/parflow/tools/tests/data/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:16:31.000000 pftools-1.3.7/parflow/tools/tests/data/__init__.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     5344 2023-02-15 23:16:32.000000 pftools-1.3.7/parflow/tools/tests/pfb_summary.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     6149 2023-02-15 23:16:32.000000 pftools-1.3.7/parflow/tools/tests/test_pf_xarray.py
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1754 2023-02-15 23:16:32.000000 pftools-1.3.7/parflow/tools/util.py
-drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-02-15 23:19:24.697321 pftools-1.3.7/pftools.egg-info/
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     7068 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/PKG-INFO
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1243 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/SOURCES.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        1 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/dependency_links.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)       79 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/entry_points.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      122 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/requires.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)        8 2023-02-15 23:19:24.000000 pftools-1.3.7/pftools.egg-info/top_level.txt
--rw-rw----   0 smithsg   (5319) smithsg   (5319)      307 2023-02-15 23:19:24.707227 pftools-1.3.7/setup.cfg
--rw-rw----   0 smithsg   (5319) smithsg   (5319)     1333 2023-02-15 23:16:32.000000 pftools-1.3.7/setup.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.696481 pftools-1.3.9/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     3922 2023-03-03 21:28:03.000000 pftools-1.3.9/CHANGELOG.md
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)       48 2023-03-03 21:28:03.000000 pftools-1.3.9/MANIFEST.in
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     7068 2023-03-03 21:28:24.697494 pftools-1.3.9/PKG-INFO
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     5519 2023-03-03 21:28:03.000000 pftools-1.3.9/README.md
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.537512 pftools-1.3.9/parflow/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      281 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/__init__.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.548524 pftools-1.3.9/parflow/cli/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/cli/__init__.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1094 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/cli/pfdist_sort.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     3931 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/cli/tcl2py.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.599518 pftools-1.3.9/parflow/tools/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      300 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/__init__.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    54981 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/builders.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    17617 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/core.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.625473 pftools-1.3.9/parflow/tools/database/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/database/__init__.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    30436 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/database/core.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    19937 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/database/domains.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)   308847 2023-03-03 21:28:02.000000 pftools-1.3.9/parflow/tools/database/generated.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     7564 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/database/handlers.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    22288 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/export.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     2730 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/fs.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     5094 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/helper.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    19801 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/hydrology.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    66816 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/io.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)    25846 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/pf_backend.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.661368 pftools-1.3.9/parflow/tools/ref/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      384 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/default_vegp_values.json
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1652 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/subsurface_conus_1.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      971 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/subsurface_freeze_cherry.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1417 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/subsurface_washita.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     7023 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/table_keys.yaml
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1128 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/vegp_header.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     4431 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/vegp_igbp.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     2685 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/ref/vegp_keys.yaml
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1733 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/settings.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      675 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/terminal.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.668302 pftools-1.3.9/parflow/tools/tests/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/tests/__init__.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.673507 pftools-1.3.9/parflow/tools/tests/data/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/tests/data/__init__.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     5344 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/tests/pfb_summary.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     6149 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/tests/test_pf_xarray.py
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1754 2023-03-03 21:28:03.000000 pftools-1.3.9/parflow/tools/util.py
+drwxrws---   0 smithsg   (5319) smithsg   (5319)        0 2023-03-03 21:28:24.696368 pftools-1.3.9/pftools.egg-info/
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     7068 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/PKG-INFO
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1243 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/SOURCES.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        1 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/dependency_links.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)       79 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/entry_points.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      122 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/requires.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)        8 2023-03-03 21:28:24.000000 pftools-1.3.9/pftools.egg-info/top_level.txt
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)      307 2023-03-03 21:28:24.701475 pftools-1.3.9/setup.cfg
+-rw-rw----   0 smithsg   (5319) smithsg   (5319)     1333 2023-03-03 21:28:03.000000 pftools-1.3.9/setup.py
```

### Comparing `pftools-1.3.7/CHANGELOG.md` & `pftools-1.3.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/PKG-INFO` & `pftools-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pftools
-Version: 1.3.7
+Version: 1.3.9
 Summary: A Python package creating an interface with the ParFlow hydrologic model.
 Home-page: https://github.com/parflow/parflow/tree/master/pftools/python
 Author: HydroFrame
 Author-email: parflow@parflow.org
 License: BSD
 Description: # pftools
```

### Comparing `pftools-1.3.7/README.md` & `pftools-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/cli/pfdist_sort.py` & `pftools-1.3.9/parflow/cli/pfdist_sort.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/cli/tcl2py.py` & `pftools-1.3.9/parflow/cli/tcl2py.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/builders.py` & `pftools-1.3.9/parflow/tools/builders.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/core.py` & `pftools-1.3.9/parflow/tools/core.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/database/core.py` & `pftools-1.3.9/parflow/tools/database/core.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/database/domains.py` & `pftools-1.3.9/parflow/tools/database/domains.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/database/generated.py` & `pftools-1.3.9/parflow/tools/database/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r'''
 --- DO NOT EDIT ---
 File automatically generated - any manual change will be lost
-Generated on 2023/02/15 - 15:16:30
-Created 179 classes
+Generated on 2023/03/03 - 13:28:01
+Created 180 classes
  => No class name duplication found
-Defined 542 fields were found
+Defined 545 fields were found
 '''
 from .core import PFDBObj, PFDBObjListNumber
 
 
 # ------------------------------------------------------------------------------
 
 class Process(PFDBObj):
@@ -2208,14 +2208,15 @@
     '''
     def __init__(self, parent=None):
         super().__init__(parent)
         self._value_ = 'Impes'
         self.CLM = CLM(self)
         self.EvapTrans = EvapTrans(self)
         self.ResetSurfacePressure = ResetSurfacePressure(self)
+        self.SurfacePredictor = SurfacePredictor(self)
         self.OverlandDiffusive = OverlandDiffusive(self)
         self.OverlandKinematic = OverlandKinematic(self)
         self.TerrainFollowingGrid = TerrainFollowingGrid(self)
         self.Linear = Linear(self)
         self.Nonlinear = Nonlinear(self)
         self.AbsTol = 1e-09
         self.AdvectOrder = 2
@@ -4583,14 +4584,50 @@
             }
           }
         }
 
 
 # ------------------------------------------------------------------------------
 
+class SurfacePredictor(PFDBObj):
+    '''
+    [Type: logical] Try to calculate if a surface cell will pond / switch from sub surface to surface flow and set pressure to a positive value.
+    '''
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self._value_ = False
+        self.PressureValue = 1e-05
+        self.PrintValues = False
+        self._details_ = {
+          "_value_": {
+            "help": "[Type: boolean/string] Try to calculate if a surface cell will pond / switch from sub surface to surface flow and set pressure to a positive value.\n",
+            "default": False,
+            "domains": {
+              "BoolDomain": None
+            }
+          },
+          "PressureValue": {
+            "help": "[Type: double] Surface pressure value set if flux into cell exceeds capacity.\n",
+            "default": 1e-05,
+            "domains": {
+              "DoubleValue": None
+            }
+          },
+          "PrintValues": {
+            "help": "[Type: logical] Surface predictor print flag.\n",
+            "default": False,
+            "domains": {
+              "BoolDomain": None
+            }
+          }
+        }
+
+
+# ------------------------------------------------------------------------------
+
 class OverlandDiffusive(PFDBObj):
     '''
     Setting epsilon value for the diffusive overland flow formulation.
     '''
     def __init__(self, parent=None):
         super().__init__(parent)
         self.Epsilon = 1e-05
```

### Comparing `pftools-1.3.7/parflow/tools/database/handlers.py` & `pftools-1.3.9/parflow/tools/database/handlers.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/export.py` & `pftools-1.3.9/parflow/tools/export.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/fs.py` & `pftools-1.3.9/parflow/tools/fs.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/helper.py` & `pftools-1.3.9/parflow/tools/helper.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/hydrology.py` & `pftools-1.3.9/parflow/tools/hydrology.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,26 +195,28 @@
     ##### --- ######
     #     qx       #
     ##### --- ######
 
     # We will be tweaking the slope values for this algorithm, so we make a copy
     slopex = np.copy(slopex)
     slopey = np.copy(slopey)
+    mannings = np.copy(mannings)
 
     # We're only interested in the surface mask, as an ny-by-nx array
     mask = mask[-1, ...]
 
     # Find all patterns of the form
     #  -------
     # | 0 | 1 |
     #  -------
-    # and copy the slopex values from the '1' cells to the corresponding '0' cells
+    # and copy the slopex, slopey and mannings values from the '1' cells to the corresponding '0' cells
     _x, _y = np.where(np.diff(mask, axis=1, append=0) == 1)
     slopex[(_x, _y)] = slopex[(_x, _y + 1)]
     slopey[(_x, _y)] = slopey[(_x, _y + 1)] 
+    mannings[(_x, _y)] = mannings[(_x, _y + 1)] 
     
     slope = np.maximum(epsilon, np.hypot(slopex, slopey))
     
     # Upwind pressure - this is for the north and east face of all cells
     # The slopes are calculated across these boundaries so the upper x boundaries are included in these
     # calculations. The lower x boundaries are added further down as q_x0
     pressure_top_padded = np.pad(pressure_top[:, 1:], ((0, 0,), (0, 1)))  # pad right
@@ -239,14 +241,15 @@
     #  ---
     # | 0 |
     # | 1 |
     #  ---
     _x, _y = np.where(np.diff(mask, axis=0, append=0) == 1)
     slopey[(_x, _y)] = slopey[(_x + 1, _y)]
     slopex[(_x, _y)] = slopex[(_x + 1, _y)]
+    mannings[(_x, _y)] = mannings[(_x + 1, _y)]
     
     slope = np.maximum(epsilon, np.hypot(slopex, slopey))
     
 
     # Upwind pressure - this is for the north and east face of all cells
     # The slopes are calculated across these boundaries so the upper y boundaries are included in these
     # calculations. The lower y boundaries are added further down as q_y0
```

### Comparing `pftools-1.3.7/parflow/tools/io.py` & `pftools-1.3.9/parflow/tools/io.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/pf_backend.py` & `pftools-1.3.9/parflow/tools/pf_backend.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/subsurface_conus_1.txt` & `pftools-1.3.9/parflow/tools/ref/subsurface_conus_1.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/subsurface_freeze_cherry.txt` & `pftools-1.3.9/parflow/tools/ref/subsurface_freeze_cherry.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/subsurface_washita.txt` & `pftools-1.3.9/parflow/tools/ref/subsurface_washita.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/table_keys.yaml` & `pftools-1.3.9/parflow/tools/ref/table_keys.yaml`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/vegp_header.txt` & `pftools-1.3.9/parflow/tools/ref/vegp_header.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/vegp_igbp.txt` & `pftools-1.3.9/parflow/tools/ref/vegp_igbp.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/ref/vegp_keys.yaml` & `pftools-1.3.9/parflow/tools/ref/vegp_keys.yaml`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/settings.py` & `pftools-1.3.9/parflow/tools/settings.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/terminal.py` & `pftools-1.3.9/parflow/tools/terminal.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/tests/pfb_summary.py` & `pftools-1.3.9/parflow/tools/tests/pfb_summary.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/tests/test_pf_xarray.py` & `pftools-1.3.9/parflow/tools/tests/test_pf_xarray.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/parflow/tools/util.py` & `pftools-1.3.9/parflow/tools/util.py`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/pftools.egg-info/PKG-INFO` & `pftools-1.3.9/pftools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pftools
-Version: 1.3.7
+Version: 1.3.9
 Summary: A Python package creating an interface with the ParFlow hydrologic model.
 Home-page: https://github.com/parflow/parflow/tree/master/pftools/python
 Author: HydroFrame
 Author-email: parflow@parflow.org
 License: BSD
 Description: # pftools
```

### Comparing `pftools-1.3.7/pftools.egg-info/SOURCES.txt` & `pftools-1.3.9/pftools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pftools-1.3.7/setup.py` & `pftools-1.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # reading the README file
 HERE = Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='pftools',
-    version="1.3.7",
+    version="1.3.9",
     description=('A Python package creating an interface with the ParFlow '
                  'hydrologic model.'),
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/parflow/parflow/tree/master/pftools/python',
     author='HydroFrame',
     author_email='parflow@parflow.org',
```

