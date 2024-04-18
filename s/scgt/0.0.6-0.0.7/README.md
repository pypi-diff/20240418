# Comparing `tmp/scgt-0.0.6.tar.gz` & `tmp/scgt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgt-0.0.6.tar", last modified: Tue Mar 19 04:18:44 2024, max compression
+gzip compressed data, was "scgt-0.0.7.tar", last modified: Thu Apr 18 20:00:40 2024, max compression
```

## Comparing `scgt-0.0.6.tar` & `scgt-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 04:18:44.788051 scgt-0.0.6/
--rw-rw-rw-   0        0        0     1314 2023-09-24 05:16:05.000000 scgt-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     3128 2024-03-19 04:18:44.780192 scgt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-09-24 05:16:05.000000 scgt-0.0.6/README.md
--rw-rw-rw-   0        0        0     1144 2024-03-19 04:14:37.000000 scgt-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       79 2023-09-24 05:16:05.000000 scgt-0.0.6/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 04:18:44.713116 scgt-0.0.6/scgt/
--rw-rw-rw-   0        0        0       41 2023-09-24 05:16:05.000000 scgt-0.0.6/scgt/__init__.py
--rw-rw-rw-   0        0        0    29369 2024-03-19 03:21:07.000000 scgt-0.0.6/scgt/scgt.py
-drwxrwxrwx   0        0        0        0 2024-03-19 04:18:44.780192 scgt-0.0.6/scgt.egg-info/
--rw-rw-rw-   0        0        0     3128 2024-03-19 04:18:44.000000 scgt-0.0.6/scgt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-03-19 04:18:44.000000 scgt-0.0.6/scgt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 04:18:44.000000 scgt-0.0.6/scgt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-03-19 04:18:44.000000 scgt-0.0.6/scgt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-19 04:18:44.000000 scgt-0.0.6/scgt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 04:18:44.788051 scgt-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.488186 scgt-0.0.7/
+-rw-rw-rw-   0        0        0     1314 2023-09-24 05:16:05.000000 scgt-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0     3128 2024-04-18 20:00:40.433415 scgt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-09-24 05:16:05.000000 scgt-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1107 2024-04-18 19:45:15.000000 scgt-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-09-24 05:16:05.000000 scgt-0.0.7/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.242657 scgt-0.0.7/scgt/
+-rw-rw-rw-   0        0        0       41 2023-09-24 05:16:05.000000 scgt-0.0.7/scgt/__init__.py
+-rw-rw-rw-   0        0        0    31983 2024-04-18 19:59:25.000000 scgt-0.0.7/scgt/scgt.py
+drwxrwxrwx   0        0        0        0 2024-04-18 20:00:40.429412 scgt-0.0.7/scgt.egg-info/
+-rw-rw-rw-   0        0        0     3128 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-18 20:00:40.000000 scgt-0.0.7/scgt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 20:00:39.000000 scgt-0.0.7/scgt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 20:00:40.490187 scgt-0.0.7/setup.cfg
```

### Comparing `scgt-0.0.6/LICENSE.md` & `scgt-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scgt-0.0.6/PKG-INFO` & `scgt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgt
-Version: 0.0.6
+Version: 0.0.7
 Summary: UC Santa Cruz Geographical Toolkit
 Author-email: Jasmine Tai <jctai@ucsc.edu>, Natalie Valett <nvalett@ucsc.edu>, Luca de Alfaro <luca@dealfaro.com>
 License: Copyright 2023, The Regents of the University of California. 
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

### Comparing `scgt-0.0.6/README.md` & `scgt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `scgt-0.0.6/pyproject.toml` & `scgt-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "scgt"
-version = "0.0.6"
-authors = [
-        {name="Jasmine Tai", email="jctai@ucsc.edu"},
-        {name="Natalie Valett", email="nvalett@ucsc.edu"},
-        {name="Luca de Alfaro", email="luca@dealfaro.com"}]
-description = "UC Santa Cruz Geographical Toolkit"
-readme = "README.md"
-requires-python = ">=3.7"
-license = {file="LICENSE.md"}
-classifiers = [
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-]
-dynamic = ["dependencies"]
-
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-
-[tool.setuptools]
-packages = ["scgt"]
-
-[project.urls]
-"Homepage" = "https://github.com/ecoscape-earth/scgt"
-"Bug Tracker" = "https://github.com/ecoscape-earth/scgt/issues"
-
-
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "scgt"
+version = "0.0.7"
+authors = [
+        {name="Jasmine Tai", email="jctai@ucsc.edu"},
+        {name="Natalie Valett", email="nvalett@ucsc.edu"},
+        {name="Luca de Alfaro", email="luca@dealfaro.com"}]
+description = "UC Santa Cruz Geographical Toolkit"
+readme = "README.md"
+requires-python = ">=3.7"
+license = {file="LICENSE.md"}
+classifiers = [
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
+[tool.setuptools]
+packages = ["scgt"]
+
+[project.urls]
+"Homepage" = "https://github.com/ecoscape-earth/scgt"
+"Bug Tracker" = "https://github.com/ecoscape-earth/scgt/issues"
+
+
```

### Comparing `scgt-0.0.6/scgt/scgt.py` & `scgt-0.0.7/scgt/scgt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import rasterio
 import rasterio.plot
 import shutil
 from rasterio.windows import Window, from_bounds
 from rasterio.warp import calculate_default_transform, reproject, Resampling
+from rasterio.io import MemoryFile
 import sys
 import numpy as np
 import matplotlib.pyplot as plt
 import math
 from osgeo import gdal
 import scipy.ndimage as nd
 
 class GeoTiff(object):
     """A GeoTiff object provides an interface to reading/writing geotiffs in
     a tiled fashion, and to many other additional operations."""
     
-    def __init__(self, file=None):
+    def __init__(self, file=None, memory_file=None):
         """
         Initializes a GeoTiff object.
         :param file: A file object for the geotiff.
+        :param memory_file: The corresponding opened MemoryFile object if the geotiff is stored in memory.
 
         Properties:
         dataset : open geotiff file
-        size : touple -> raster width, height
+        size : tuple -> raster width, height
         bands : int -> number of bands in geotiff
         transform : the dataset's geospatial transform - an affine transformation matrix that maps pixel
                     locations in (row, col) coordinates to (x, y) spatial positions
         corners : array of lat/long of corners, in order top left, top right, bottom right, bottom left
         block_shapes : array with the shape of blocks for all bands
                         i.e [(1, (3, 791)), (2, (3, 791))]
         profile : Geotiff profile - used for writing metadata to new file
+        memory_file : the associated memory file object if geotiff is stored in memory
         """
         if file:
             self.dataset = file
             self.filepath = file.name
             self.size = (self.dataset.width, self.dataset.height)
             self.width, self.height = self.dataset.width, self.dataset.height
             self.bands = self.dataset.count
@@ -41,26 +44,30 @@
                             self.transform * (0, self.dataset.height),                  # top right
                             self.transform * (self.dataset.width, self.dataset.height), #bottom right
                             self.transform * (self.dataset.width, 0)]                   #bottom left
             self.block_shapes = self.dataset.block_shapes
             self.data_types = self.dataset.dtypes
             self.profile = self.dataset.profile
             self.crs = self.dataset.crs
+            self.memory_file = memory_file
 
 
     def __enter__(self):
         """Context manager entry for use in with statements."""
         # essentially returns what to use for the variable in a with statement
         return self
 
     def __exit__(self, type, value, traceback):
         """Context manager exit."""
         # closes the dataset at the conclusion of a with statement
-        self.getAttributeTable()
-        self.dataset.close()
+        if self.memory_file is not None:
+            self.close_memory_file()
+        else:
+            self.getAttributeTable()
+            self.dataset.close()
 
     @classmethod
     def from_file(cls, filename):
         """
         Creates a GeoTiff object from a filename.
         :param filename: filename to open in read mode.
         :return: the GeoTiff object.
@@ -82,27 +89,51 @@
             (note that if geotiff is of unsigned type, like uint8, the no_data value must be  a positive int in the data
             range, which could result in data obstruction. If datatype is signed, we suggest using a negative value)
         :return: the GeoTiff object for the new file.
         """
         # create file with write mode, then open with rw to have full read/write access
         f = rasterio.open(filename, 'w', **profile)
         f.close()
+
         # sets no_data (transparent value)
         if no_data_value is not None:
             with rasterio.open(filename, "r+") as dataset:
                 dataset.nodata = no_data_value
                 nodata_mask = np.ones((dataset.width, dataset.height)) * no_data_value
                 dataset.write(nodata_mask.astype(profile['dtype']), 1)
 
         open_file = rasterio.open(filename, 'r+', **profile)
         if not open_file:
             sys.exit("GeoTiff Error: copy_to_new_file() being called with invalid Geotiff data or filepath")
+        
         # return GeoTiff obj with open file
         return cls(open_file)
 
+    @classmethod
+    def create_memory_file(cls, profile, no_data_value=None):
+        """ creates a temporary file in memory in which to store a GeoTiff obj.
+        :param profile: profile for writing the geotiff.
+        :param no_data_value (dtype of raster): value to be used as transparent 'nodata' value, otherwise fills 0's
+            (note that if geotiff is of unsigned type, like uint8, the no_data value must be  a positive int in the data range, which could result in data obstruction. If datatype is signed, we suggest using a negative value)
+        :return: the GeoTiff object for the new file.
+        """
+        # create file in memory
+        f = MemoryFile()
+
+        # open file for read/write
+        dataset = rasterio.open(f, mode="w+", **profile)
+
+        # set no_data (transparent value) if given
+        if no_data_value is not None:
+            dataset.nodata = no_data_value
+            nodata_mask = np.ones((dataset.width, dataset.height)) * no_data_value
+            dataset.write(nodata_mask.astype(profile['dtype']), 1)
+        
+        # return GeoTiff obj with open file
+        return cls(dataset, memory_file=f)
 
     def clone_shape(self, filename, no_data_value=None, dtype=None):
         """Creates a new geotiff with the indicated filename, cloning the shape of the current one.
         :param filename: filename where to create the new clone.
         :param no_data_value (dtype of raster): value to be used as transparent 'nodata' value, otherwise fills 0's
             (note that if geotiff is of unsigned type, like uint8, the no_data value must be  a positive int in the data
             range, which could result in data obstruction. If datatype is signed, we suggest using a negative value)
@@ -119,14 +150,15 @@
         if no_data_value is not None:
             assert rasterio.dtypes.can_cast_dtype(no_data_value, profile['dtype']), \
                 f"The chosen no_data value {no_data_value} cannot be cast to type {profile['dtype']} without loss of information"
 
         # copies src tif file to destination
         shutil.copy(src=self.filepath, dst=filename)
         tiff = GeoTiff.copy_to_new_file(filename, profile=profile, no_data_value=no_data_value)
+        
         return tiff
 
     def scale_tiff(self, reference_tif=None, scale_x=1, scale_y=1):
         """
         Scales a tiff.
         :param reference_tif: Tiff to be scaled.
         :param scale_x: x scale.
@@ -404,20 +436,21 @@
         """
         plt.figure(figsize=(width, height))
         fig, ax = plt.subplots(figsize = (width, height))
         fig.colorbar(ax.imshow(self.get_rectangle((0, self.width), (0, self.height), band),
                                                   cmap="inferno"))
         plt.show()
 
-    def crop_to_new_file(self, output_path, bounds, padding=0):
+    def crop_to_new_file(self, bounds, padding=0, filename=None, in_memory=False):
         """
         Create a new geotiff by cropping the current one and writing to a new file.
-        :param output_path: path where to write result.
         :param bounds: bounding box (xmin, ymin, xmax, ymax) for the output (in the same coordinate system)
         :param padding: amount of padding in meters to add around the shape bounds.
+        :param filename: path where to write result.
+        :param in_memory: whether to create the file in memory only. filename is ignored if True.
         :return: the GeoTiff object for the new file.
         """
         # add padding to the bounds
         bounds = (bounds[0] - padding, bounds[1] - padding, bounds[2] + padding, bounds[3] + padding)
 
         # keep window within bounds of self, and round lengths and offsets to keep windows aligned
         src_window = from_bounds(*self.dataset.bounds, transform=self.dataset.transform)
@@ -431,16 +464,22 @@
             'height': cropped_window.height,
             'transform': self.dataset.window_transform(cropped_window),
             'nodata': None,
             'compress': 'LZW',
             'bigtiff': 'YES'
         })
 
+        # create new file
+        if in_memory:
+            output = GeoTiff.create_memory_file(profile)
+        else:
+            assert filename is not None, "filename must be provided if not creating file in memory"
+            output = GeoTiff.copy_to_new_file(filename, profile)
+
         # copy data within the cropping window over to new file
-        output = GeoTiff.copy_to_new_file(output_path, profile)
         reader = output.get_reader(b=0, w=10000, h=10000)
         for tile in reader:
             tile.fit_to_bounds(width=output.width, height=output.height)
             window = Window(tile.x, tile.y, tile.w, tile.h)
             src_window = Window(tile.x + x_offset, tile.y + y_offset, tile.w, tile.h)
             output.dataset.write(self.dataset.read(window=src_window), window=window)
 
@@ -544,14 +583,28 @@
             j = asize // 2
             k[j, j] = 1
             return nd.gaussian_filter(k, sigma=asize / 4)
         window = rasterio.windows.Window(x - (size/2), y - (size/2), size, size)
         arr = np.squeeze(self.dataset.read(window=window))
         return np.average(arr, weights=gaussian_kernel(arr.shape[0]))
 
+    def close_memory_file(self):
+        """
+        Closes the memory file if the GeoTiff object is created in memory only.
+        This is called automatically if the object is used in a with statement.
+        Otherwise, it should be called when the GeoTiff object is not needed anymore
+        so that the memory file is deleted.
+        """
+        if self.memory_file is not None and not self.memory_file.closed:
+            self.dataset.close()
+            self.memory_file._env.close()
+            self.memory_file.close()
+        elif self.memory_file is None:
+            print(f'The current GeoTiff object ("{self.filepath}") is not stored in memory.')
+
 class Reader(object):
     """
     A reader iterates through the tiles of a geotiff.
     """
     def __init__(self, geo, b=0, w=None, h=None):
         """
         Initializes a reader.
```

### Comparing `scgt-0.0.6/scgt.egg-info/PKG-INFO` & `scgt-0.0.7/scgt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgt
-Version: 0.0.6
+Version: 0.0.7
 Summary: UC Santa Cruz Geographical Toolkit
 Author-email: Jasmine Tai <jctai@ucsc.edu>, Natalie Valett <nvalett@ucsc.edu>, Luca de Alfaro <luca@dealfaro.com>
 License: Copyright 2023, The Regents of the University of California. 
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
```

