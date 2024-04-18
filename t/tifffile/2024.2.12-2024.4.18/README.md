# Comparing `tmp/tifffile-2024.2.12.tar.gz` & `tmp/tifffile-2024.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2024.2.12.tar", last modified: Mon Feb 12 18:53:11 2024, max compression
+gzip compressed data, was "tifffile-2024.4.18.tar", last modified: Thu Apr 18 02:07:18 2024, max compression
```

## Comparing `tifffile-2024.2.12.tar` & `tifffile-2024.4.18.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.682385 tifffile-2024.2.12/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.2.12/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    37742 2024-02-12 18:53:10.000000 tifffile-2024.2.12/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-02-12 18:53:10.000000 tifffile-2024.2.12/LICENSE
--rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.2.12/MANIFEST.in
--rw-rw-rw-   0        0        0    31456 2024-02-12 18:53:11.682385 tifffile-2024.2.12/PKG-INFO
--rw-rw-rw-   0        0        0    30214 2024-02-12 18:53:10.000000 tifffile-2024.2.12/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.672609 tifffile-2024.2.12/docs/
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.672609 tifffile-2024.2.12/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.2.12/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.2.12/docs/conf.py
--rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.2.12/docs/make.py
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.672609 tifffile-2024.2.12/examples/
--rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.2.12/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.2.12/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2024-02-12 18:53:11.682385 tifffile-2024.2.12/setup.cfg
--rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.2.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.672609 tifffile-2024.2.12/tests/
--rw-rw-rw-   0        0        0     1603 2023-08-30 07:20:06.000000 tifffile-2024.2.12/tests/conftest.py
--rw-rw-rw-   0        0        0   740847 2024-02-12 18:24:17.000000 tifffile-2024.2.12/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.672609 tifffile-2024.2.12/tifffile/
--rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.2.12/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.2.12/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11827 2024-01-29 05:07:27.000000 tifffile-2024.2.12/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.2.12/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.2.12/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.2.12/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.2.12/tifffile/py.typed
--rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.2.12/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.2.12/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   886692 2024-02-12 18:45:03.000000 tifffile-2024.2.12/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2024-02-12 18:53:11.682385 tifffile-2024.2.12/tifffile.egg-info/
--rw-rw-rw-   0        0        0    31456 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-12 18:53:11.000000 tifffile-2024.2.12/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.4.18/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    37954 2024-04-18 02:07:16.000000 tifffile-2024.4.18/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-04-18 02:07:16.000000 tifffile-2024.4.18/LICENSE
+-rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.4.18/MANIFEST.in
+-rw-rw-rw-   0        0        0    31748 2024-04-18 02:07:18.260378 tifffile-2024.4.18/PKG-INFO
+-rw-rw-rw-   0        0        0    30506 2024-04-18 02:07:16.000000 tifffile-2024.4.18/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/docs/
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.4.18/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.4.18/docs/conf.py
+-rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.4.18/docs/make.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/examples/
+-rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.4.18/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.4.18/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:07:18.260378 tifffile-2024.4.18/setup.cfg
+-rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.4.18/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tests/
+-rw-rw-rw-   0        0        0     1603 2023-08-30 07:20:06.000000 tifffile-2024.4.18/tests/conftest.py
+-rw-rw-rw-   0        0        0   744257 2024-04-18 01:23:55.000000 tifffile-2024.4.18/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tifffile/
+-rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.4.18/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.4.18/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11827 2024-01-29 05:07:27.000000 tifffile-2024.4.18/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.4.18/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.4.18/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.4.18/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.4.18/tifffile/py.typed
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.4.18/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.4.18/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   888468 2024-04-18 01:45:15.000000 tifffile-2024.4.18/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31748 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-04-18 02:07:18.000000 tifffile-2024.4.18/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2024.2.12/CHANGES.rst` & `tifffile-2024.4.18/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Revisions
 ---------
 
+2024.4.18
+
+- Pass 5077 tests.
+- Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
+- Add option not to quote file names in write_fsspec.
+- Allow compress bilevel images with deflate, LZMA, and Zstd.
+
 2024.2.12
 
-- Pass 5074 tests.
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
 - Add imreadargs parameters passed to FileSequence.imread.
 
 2024.1.30
 
 - Fix compatibility issue with numpy 2 (#238).
 - Enable DeprecationWarning for tuple compression argument.
```

### Comparing `tifffile-2024.2.12/LICENSE` & `tifffile-2024.4.18/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/MANIFEST.in` & `tifffile-2024.4.18/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/PKG-INFO` & `tifffile-2024.4.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.2.12
+Version: 2024.4.18
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.12
+:Version: 2024.4.18
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -95,33 +95,39 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 5.1.0
+- `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.16.1
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.2.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.4.18
+
+- Pass 5077 tests.
+- Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
+- Add option not to quote file names in write_fsspec.
+- Allow compress bilevel images with deflate, LZMA, and Zstd.
+
 2024.2.12
 
-- Pass 5074 tests.
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
 - Add imreadargs parameters passed to FileSequence.imread.
 
 2024.1.30
 
 - Fix compatibility issue with numpy 2 (#238).
 - Enable DeprecationWarning for tuple compression argument.
@@ -317,16 +323,17 @@
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
 - **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
-  attributes of the XML formatted description of the first page. Tifffile can
-  read Philips slides.
+  attributes of the XML formatted description of the first page. Tile offsets
+  and byte counts may be 0 and last rows of tiles may be missing.
+  Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
```

### Comparing `tifffile-2024.2.12/README.rst` & `tifffile-2024.4.18/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.12
+:Version: 2024.4.18
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -62,33 +62,39 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 5.1.0
+- `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.16.1
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.2.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.4.18
+
+- Pass 5077 tests.
+- Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
+- Add option not to quote file names in write_fsspec.
+- Allow compress bilevel images with deflate, LZMA, and Zstd.
+
 2024.2.12
 
-- Pass 5074 tests.
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
 - Add imreadargs parameters passed to FileSequence.imread.
 
 2024.1.30
 
 - Fix compatibility issue with numpy 2 (#238).
 - Enable DeprecationWarning for tuple compression argument.
@@ -284,16 +290,17 @@
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
 - **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
-  attributes of the XML formatted description of the first page. Tifffile can
-  read Philips slides.
+  attributes of the XML formatted description of the first page. Tile offsets
+  and byte counts may be 0 and last rows of tiles may be missing.
+  Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
```

### Comparing `tifffile-2024.2.12/docs/conf.py` & `tifffile-2024.4.18/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/docs/make.py` & `tifffile-2024.4.18/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/examples/earthbigdata.py` & `tifffile-2024.4.18/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/examples/issue125.py` & `tifffile-2024.4.18/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/setup.py` & `tifffile-2024.4.18/setup.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tests/conftest.py` & `tifffile-2024.4.18/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tests/test_tifffile.py` & `tifffile-2024.4.18/tests/test_tifffile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2024.2.12
+:Version: 2024.4.18
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -296,15 +296,15 @@
         SKIP_ZARR = True
 
 if SKIP_DASK:
     dask = None
 else:
     try:
         import dask  # type: ignore
-        import dask.array
+        import dask.array  # type: ignore
     except ImportError:
         dask = None
         SKIP_DASK = True
 
 if SKIP_NDTIFF:
     ndtiff = None
 else:
@@ -2831,14 +2831,83 @@
             compression='zlib',
             **kwargs,
         )
         im = imread(fname, maxworkers=2, buffersize=buffersize)
     assert_array_equal(im, data)
 
 
+@pytest.mark.skipif(
+    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
+)
+def test_issue_philips_fsspec():
+    """Test write_fsspec with Philips slide missing row of tiles."""
+    # https://github.com/cgohlke/tifffile/issues/249
+    fname = private_file('PhilipsDP/patient_080_node_2.tif')
+    with TiffFile(fname) as tif:
+        assert len(tif.series) == 2
+        assert len(tif.pages) == 11
+        assert tif.is_philips
+        assert tif.philips_metadata.endswith('</DataObject>')
+        page = tif.pages.first
+        assert page.compression == JPEG
+        assert page.photometric == YCBCR
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 155136
+        assert page.tags['ImageLength'].value == 78336
+        assert page.imagewidth == 155136
+        assert page.imagelength == 78336
+        assert page.bitspersample == 8
+        assert page.samplesperpixel == 3
+        assert page.tags['Software'].value == 'Philips DP v1.0'
+        series = tif.series[1]
+        assert series.kind == 'philips'
+        assert series.shape == (801, 1756, 3)
+        assert len(series.levels) == 1
+        assert not series.is_pyramidal
+        series = tif.series[0]
+        assert series.kind == 'philips'
+        assert series.shape == (78336, 155136, 3)
+        assert len(series.levels) == 10
+        assert series.is_pyramidal
+        page = series.levels[3].pages[0]
+        assert page.compression == JPEG
+        assert page.photometric == YCBCR
+        assert page.planarconfig == CONTIG
+        assert page.tags['ImageWidth'].value == 19456
+        assert page.tags['ImageLength'].value == 9728
+        assert page.imagewidth == 19392
+        assert page.imagelength == 9792
+        # assert data
+        image = tif.asarray(series=0, level=3)
+        assert image.shape == (9792, 19392, 3)
+        assert image[300, 400, 1] == 226
+        assert image[9791, 0, 1] == 0
+        assert_aszarr_method(series, image, level=3)
+        assert__str__(tif)
+
+        if SKIP_ZARR:
+            return
+
+        # write fsspec
+        from imagecodecs.numcodecs import register_codecs
+
+        register_codecs('imagecodecs_jpeg', verbose=False)
+        url = os.path.dirname(fname).replace('\\', '/')
+        with TempFileName('issue_philips_fsspec', ext='.json') as jsonfile:
+            page.aszarr().write_fsspec(jsonfile, url, version=0)
+            mapper = fsspec.get_mapper(
+                'reference://',
+                fo=jsonfile,
+                target_protocol='file',
+                remote_protocol='file',
+            )
+            zobj = zarr.open(mapper, mode='r')
+            assert_array_equal(zobj[:], image)
+
+
 class TestExceptions:
     """Test various Exceptions and Warnings."""
 
     data = random_data(numpy.uint16, (5, 13, 17))
 
     @pytest.fixture(scope='class')
     def fname(self):
@@ -3061,15 +3130,15 @@
                 compression=7,
                 subsampling=(3, 3),
             )
 
     def test_compress_bilevel(self, fname):
         # cannot compress bilevel image
         with pytest.raises(NotImplementedError):
-            imwrite(fname, self.data.astype('?'), compression=8)
+            imwrite(fname, self.data.astype('?'), compression='jpeg')
 
     def test_description_unicode(self, fname):
         # strings must be 7-bit ASCII
         with pytest.raises(ValueError):
             imwrite(fname, self.data, description='mu: \u03BC')
 
     def test_compression_contiguous(self, fname):
@@ -3632,15 +3701,15 @@
             assert 'None' not in tags
             assert None not in tags
             assert 'TiffTags' in repr(tags)
 
 
 def test_class_tifftagregistry():
     """Test TiffTagRegistry."""
-    numtags = 656
+    numtags = 657
     tags = TIFF.TAGS
     assert len(tags) == numtags
     assert tags[11] == 'ProcessingSoftware'
     assert tags['ProcessingSoftware'] == 11
     assert tags.getall(11) == ['ProcessingSoftware']
     assert tags.getall('ProcessingSoftware') == [11]
     tags.add(11, 'ProcessingSoftware')
@@ -12248,15 +12317,15 @@
         assert page.tags['ImageLength'].value == 89600
         assert page.imagewidth == 85654
         assert page.imagelength == 89225
         assert page.bitspersample == 8
         assert page.samplesperpixel == 3
         assert page.tags['Software'].value == 'Philips DP v1.0'
         series = tif.series[0]
-        assert series.kind == 'generic'
+        assert series.kind == 'philips'
         assert series.shape == (89225, 85654, 3)
         assert len(series.levels) == 9
         assert series.is_pyramidal
         # assert data
         image = tif.asarray(series=0, level=5)
         assert image.shape == (2789, 2677, 3)
         assert image[300, 400, 1] == 206
@@ -13501,29 +13570,34 @@
         (5, 219, 301),
         (4, 3, 219, 301),
         (4, 219, 301, 3),
         (3, 4, 219, 301),
         (3, 4, 219, 301, 1),
     ],
 )
+@pytest.mark.parametrize(
+    'compression', [None]  # , 'zlib', 'lzw', 'lzma', 'zstd', 'packbits']
+)
 @pytest.mark.parametrize('dtype', list('?bhiqefdBHIQFD'))
 @pytest.mark.parametrize('byteorder', ['>', '<'])
 @pytest.mark.parametrize('bigtiff', ['plaintiff', 'bigtiff'])
 @pytest.mark.parametrize('tile', [None, (64, 64)])
 @pytest.mark.parametrize('data', ['random', None])
-def test_write(data, byteorder, bigtiff, dtype, shape, tile):
+def test_write(data, byteorder, bigtiff, compression, dtype, shape, tile):
     """Test TiffWriter with various options."""
-    # TODO: test compression ?
-    fname = 'write_{}_{}_{}_{}{}{}'.format(
+    if compression is not None and (data is None or SKIP_CODECS):
+        pytest.xfail(REASON)
+    fname = 'write_{}_{}_{}_{}{}{}{}'.format(
         bigtiff,
         {'<': 'le', '>': 'be'}[byteorder],
         numpy.dtype(dtype).name,
         str(shape).replace(' ', ''),
         '_tiled' if tile is not None else '',
         '_empty' if data is None else '',
+        f'_{compression}' if compression is not None else '',
     )
     bigtiff = bigtiff == 'bigtiff'
     if (3 in shape or 4 in shape) and shape[-1] != 1 and dtype != '?':
         photometric = 'rgb'
     else:
         photometric = None
 
@@ -13557,14 +13631,15 @@
             imwrite(
                 fname,
                 data,
                 byteorder=byteorder,
                 bigtiff=bigtiff,
                 tile=tile,
                 photometric=photometric,
+                compression=compression,
             )
             image = imread(fname)
             assert image.flags['C_CONTIGUOUS']
             assert_array_equal(data.squeeze(), image.squeeze())
             if not SKIP_ZARR:
                 with imread(fname, aszarr=True) as store:
                     data = zarr.open(store, mode='r')
@@ -14963,18 +15038,20 @@
             assert page.samplesperpixel == 3
             image = tif.asarray()
             assert_allclose(data, image, atol=atol)
             assert_aszarr_method(tif, image)
             assert__str__(tif)
 
 
-def test_write_compression_deflate():
+@pytest.mark.parametrize('dtype', [numpy.uint8, bool])
+def test_write_compression_deflate(dtype):
     """Test write ZLIB compression."""
-    data = WRITE_DATA
-    with TempFileName('write_compression_deflate') as fname:
+    dtype = numpy.dtype(dtype)
+    data = WRITE_DATA.astype(dtype)
+    with TempFileName(f'write_compression_deflate_{dtype}') as fname:
         imwrite(
             fname,
             data,
             compression=DEFLATE,
             compressionargs={'level': 6},
             photometric=RGB,
             rowsperstrip=108,
@@ -15022,18 +15099,20 @@
             assert page.samplesperpixel == 3
             image = tif.asarray()
             assert_array_equal(data, image)
             assert_aszarr_method(tif, image)
             assert__str__(tif)
 
 
-def test_write_compression_lzma():
+@pytest.mark.parametrize('dtype', [numpy.uint8, bool])
+def test_write_compression_lzma(dtype):
     """Test write LZMA compression."""
-    data = WRITE_DATA
-    with TempFileName('write_compression_lzma') as fname:
+    dtype = numpy.dtype(dtype)
+    data = WRITE_DATA.astype(dtype)
+    with TempFileName(f'write_compression_lzma_{dtype}') as fname:
         imwrite(
             fname, data, compression=LZMA, photometric=RGB, rowsperstrip=108
         )
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
@@ -15049,18 +15128,20 @@
             image = tif.asarray()
             assert_array_equal(data, image)
             assert_aszarr_method(tif, image)
             assert__str__(tif)
 
 
 @pytest.mark.skipif(SKIP_CODECS or not imagecodecs.ZSTD, reason=REASON)
-def test_write_compression_zstd():
+@pytest.mark.parametrize('dtype', [numpy.uint8, bool])
+def test_write_compression_zstd(dtype):
     """Test write ZSTD compression."""
-    data = WRITE_DATA
-    with TempFileName('write_compression_zstd') as fname:
+    dtype = numpy.dtype(dtype)
+    data = WRITE_DATA.astype(dtype)
+    with TempFileName(f'write_compression_zstd_{dtype}') as fname:
         imwrite(
             fname, data, compression=ZSTD, photometric=RGB, rowsperstrip=108
         )
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
@@ -15258,15 +15339,15 @@
             assert 0.5 > numpy.mean(
                 image.astype(numpy.float32) - data.astype(numpy.float32)
             )
             assert__str__(tif)
 
 
 @pytest.mark.skipif(SKIP_CODECS, reason=REASON)
-@pytest.mark.parametrize('dtype', [numpy.int8, numpy.uint8, numpy.bool_])
+@pytest.mark.parametrize('dtype', [numpy.int8, numpy.uint8, bool])
 @pytest.mark.parametrize('tile', [None, (16, 16)])
 def test_write_compression_packbits(dtype, tile):
     """Test write PackBits compression."""
     dtype = numpy.dtype(dtype)
     uncompressed = numpy.frombuffer(
         b'\xaa\xaa\xaa\x80\x00\x2a\xaa\xaa\xaa\xaa\x80\x00'
         b'\x2a\x22\xaa\xaa\xaa\xaa\xaa\xaa\xaa\xaa\xaa\xaa',
```

### Comparing `tifffile-2024.2.12/tifffile/_imagecodecs.py` & `tifffile-2024.4.18/tifffile/_imagecodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/geodb.py` & `tifffile-2024.4.18/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/lsm2bin.py` & `tifffile-2024.4.18/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/numcodecs.py` & `tifffile-2024.4.18/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/tiff2fsspec.py` & `tifffile-2024.4.18/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/tiffcomment.py` & `tifffile-2024.4.18/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.2.12/tifffile/tifffile.py` & `tifffile-2024.4.18/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.12
+:Version: 2024.4.18
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -92,33 +92,39 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 5.1.0
+- `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.16.1
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.2.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.4.18
+
+- Pass 5077 tests.
+- Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
+- Add option not to quote file names in write_fsspec.
+- Allow compress bilevel images with deflate, LZMA, and Zstd.
+
 2024.2.12
 
-- Pass 5074 tests.
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
 - Add imreadargs parameters passed to FileSequence.imread.
 
 2024.1.30
 
 - Fix compatibility issue with numpy 2 (#238).
 - Enable DeprecationWarning for tuple compression argument.
@@ -314,16 +320,17 @@
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
 - **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
-  attributes of the XML formatted description of the first page. Tifffile can
-  read Philips slides.
+  attributes of the XML formatted description of the first page. Tile offsets
+  and byte counts may be 0 and last rows of tiles may be missing.
+  Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
@@ -821,15 +828,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.2.12'
+__version__ = '2024.4.18'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -2961,33 +2968,36 @@
             else:
                 subifds = int(subifds)  # type: ignore
             self._subifds = subifds
             addtag(
                 tags, 330, 18 if offsetsize > 4 else 13, subifds, [0] * subifds
             )
         if not bilevel and not datadtype.kind == 'u':
+            # SampleFormat
             sampleformat = {'u': 1, 'i': 2, 'f': 3, 'c': 6}[datadtype.kind]
             addtag(
                 tags,
                 339,
                 3,
                 storedshape.samples,
                 (sampleformat,) * storedshape.samples,
             )
         if colormap is not None:
             addtag(tags, 320, 3, colormap.size, colormap)
         addtag(tags, 277, 3, 1, storedshape.samples)
         if bilevel:
-            pass
+            # PlanarConfiguration
+            if storedshape.samples > 1:
+                addtag(tags, 284, 3, 1, storedshape.planarconfig)
         elif storedshape.samples > 1:
+            # PlanarConfiguration
+            addtag(tags, 284, 3, 1, storedshape.planarconfig)
+            # BitsPerSample
             addtag(
-                tags, 284, 3, 1, storedshape.planarconfig
-            )  # PlanarConfiguration
-            addtag(
-                tags,  # BitsPerSample
+                tags,
                 258,
                 3,
                 storedshape.samples,
                 (bitspersample,) * storedshape.samples,
             )
         else:
             addtag(tags, 258, 3, 1, bitspersample)
@@ -3284,16 +3294,16 @@
             if compressiontag == 1:
 
                 def compressionfunc1(data, axis=compressionaxis) -> bytes:
                     return numpy.packbits(data, axis=axis).tobytes()
 
                 compressionfunc = compressionfunc1
 
-            elif compressiontag in {5, 32773}:
-                # LZW, PackBits
+            elif compressiontag in {5, 32773, 8, 32946, 50013, 34925, 50000}:
+                # LZW, PackBits, deflate, LZMA, ZSTD
                 def compressionfunc2(
                     data,
                     compressor=TIFF.COMPRESSORS[compressiontag],
                     axis=compressionaxis,
                     kwargs=compressionargs,
                 ) -> bytes:
                     data = numpy.packbits(data, axis=axis).tobytes()
@@ -4632,14 +4642,15 @@
             'stk',
             'sis',
             'svs',
             'scn',
             'qpi',
             'ndpi',
             'bif',
+            'philips',
             'scanimage',
             # 'indica',  # TODO: rewrite _series_indica()
             'nih',
             'mdgel',  # adds second page to cache
             'uniform',
         ):
             if getattr(self, 'is_' + kind, False):
@@ -5232,14 +5243,34 @@
                     # s.kind += '_macro'
                 elif mag == -2.0:
                     s.name = 'Map'
                     # s.kind += '_map'
         self.is_uniform = False
         return series
 
+    def _series_philips(self) -> list[TiffPageSeries] | None:
+        """Return pyramidal image series in Philips DP file."""
+        series = self._series_generic()
+        if series is None:
+            return None
+        for s in series:
+            s.kind = 'philips'
+            if s.is_pyramidal:
+                # TODO: read name from XML
+                s.name = 'Baseline'
+                # if s.dtype.itemsize == 1:
+                #     for level in s.levels:
+                #         level.keyframe.nodata = 255
+            elif s.keyframe.description.startswith('Macro'):
+                s.name = 'Macro'
+            elif s.keyframe.description.startswith('Label'):
+                s.name = 'Label'
+        self.is_uniform = False
+        return series
+
     def _series_indica(self) -> list[TiffPageSeries] | None:
         """Return pyramidal image series in IndicaLabs file."""
         # TODO: need more IndicaLabs sample files
         # TODO: parse indica series from XML
         # TODO: alpha channels in SubIFDs or main IFDs
 
         from xml.etree import ElementTree as etree
@@ -13337,16 +13368,18 @@
         else:
             with self._filecache.lock:
                 page = series[pageindex]
             if page is None or page.keyframe is None:
                 return keyframe, None, chunkindex, 0, 0
             try:
                 offset = page.dataoffsets[chunkindex]
-            except IndexError as exc:
-                raise KeyError(key) from exc
+            except IndexError:
+                # raise KeyError(key) from exc
+                # issue #249: Philips may be missing last row of tiles
+                return page.keyframe, page, chunkindex, 0, 0
         try:
             bytecount = page.databytecounts[chunkindex]
         except IndexError as exc:
             raise KeyError(key) from exc
         return page.keyframe, page, chunkindex, offset, bytecount
 
     def _indices(self, key: str, series: TiffPageSeries, /) -> tuple[int, int]:
@@ -13611,28 +13644,32 @@
 
     def write_fsspec(
         self,
         jsonfile: str | os.PathLike[Any] | TextIO,
         /,
         url: str,
         *,
+        quote: bool | None = None,
         groupname: str | None = None,
         templatename: str | None = None,
         codec_id: str | None = None,
         version: int | None = None,
         _append: bool = False,
         _close: bool = True,
     ) -> None:
         """Write fsspec ReferenceFileSystem as JSON to file.
 
         Parameters:
             jsonfile:
                 Name or open file handle of output JSON file.
             url:
                 Remote location of TIFF file(s) without file name(s).
+            quote:
+                Quote file names, that is, replace ' ' with '%20'.
+                The default is True.
             groupname:
                 Zarr group name.
             templatename:
                 Version 1 URL template name. The default is 'u'.
             codec_id:
                 Name of Numcodecs codec to decode files or chunks.
             version:
@@ -13641,15 +13678,15 @@
                 Experimental API.
 
         References:
             - `fsspec ReferenceFileSystem format
               <https://github.com/fsspec/kerchunk>`_
 
         """
-        from urllib.parse import quote
+        from urllib.parse import quote as quote_
 
         kwargs = self._kwargs.copy()
 
         if codec_id is not None:
             pass
         elif self._imread == imread:
             codec_id = 'tifffile'
@@ -13745,15 +13782,17 @@
 
         for key, value in self._store.items():
             if '.zarray' in key:
                 value = json.loads(value)
                 for index, filename in sorted(
                     self._lookup.items(), key=lambda x: x[0]
                 ):
-                    filename = quote(filename[prefix:].replace('\\', '/'))
+                    filename = filename[prefix:].replace('\\', '/')
+                    if quote is None or quote:
+                        filename = quote_(filename)
                     if filename[0] == '/':
                         filename = filename[1:]
                     indexstr = '.'.join(str(i) for i in index)
                     fh.write(
                         f',\n{indent}"{groupname}{indexstr}": '
                         f'["{url}{filename}"]'
                     )
@@ -17144,14 +17183,15 @@
                 (532, 'ReferenceBlackWhite'),
                 (559, 'StripRowCounts'),
                 (700, 'XMP'),  # XMLPacket
                 (769, 'GDIGamma'),  # GDI+
                 (770, 'ICCProfileDescriptor'),  # GDI+
                 (771, 'SRGBRenderingIntent'),  # GDI+
                 (800, 'ImageTitle'),  # GDI+
+                (907, 'SiffCompress'),  # https://github.com/MaimonLab/SiffPy
                 (999, 'USPTO_Miscellaneous'),
                 (4864, 'AndorId'),  # TODO, Andor Technology 4864 - 5030
                 (4869, 'AndorTemperature'),
                 (4876, 'AndorExposureTime'),
                 (4878, 'AndorKineticCycleTime'),
                 (4879, 'AndorAccumulations'),
                 (4881, 'AndorAcquisitionCycleTime'),
```

### Comparing `tifffile-2024.2.12/tifffile.egg-info/PKG-INFO` & `tifffile-2024.4.18/tifffile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.2.12
+Version: 2024.4.18
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.2.12
+:Version: 2024.4.18
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -95,33 +95,39 @@
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.8, 3.12.2, 64-bit
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.3
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.9, 3.12.3, 64-bit
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 5.1.0
+- `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.16.1
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
-- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.2.0
+- `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
+2024.4.18
+
+- Pass 5077 tests.
+- Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
+- Add option not to quote file names in write_fsspec.
+- Allow compress bilevel images with deflate, LZMA, and Zstd.
+
 2024.2.12
 
-- Pass 5074 tests.
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
 - Add imreadargs parameters passed to FileSequence.imread.
 
 2024.1.30
 
 - Fix compatibility issue with numpy 2 (#238).
 - Enable DeprecationWarning for tuple compression argument.
@@ -317,16 +323,17 @@
   cannot be decoded with common JPEG libraries. Tifffile works around this
   limitation by separately decoding the MCUs between restart markers, which
   performs poorly. BitsPerSample, SamplesPerPixel, and
   PhotometricInterpretation tags may contain wrong values, which can be
   corrected using the value of tag 65441.
 - **Philips TIFF** slides store wrong ImageWidth and ImageLength tag values
   for tiled pages. The values can be corrected using the DICOM_PIXEL_SPACING
-  attributes of the XML formatted description of the first page. Tifffile can
-  read Philips slides.
+  attributes of the XML formatted description of the first page. Tile offsets
+  and byte counts may be 0 and last rows of tiles may be missing.
+  Tifffile can read Philips slides.
 - **Ventana/Roche BIF** slides store tiles and metadata in a BigTIFF container.
   Tiles may overlap and require stitching based on the TileJointInfo elements
   in the XMP tag. Volumetric scans are stored using the ImageDepth extension.
   Tifffile can read BIF and decode individual tiles but does not perform
   stitching.
 - **ScanImage** optionally allows corrupted non-BigTIFF files > 2 GB.
   The values of StripOffsets and StripByteCounts can be recovered using the
```

### Comparing `tifffile-2024.2.12/tifffile.egg-info/SOURCES.txt` & `tifffile-2024.4.18/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

