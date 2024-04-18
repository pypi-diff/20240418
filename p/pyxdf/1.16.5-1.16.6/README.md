# Comparing `tmp/pyxdf-1.16.5.tar.gz` & `tmp/pyxdf-1.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxdf-1.16.5.tar", last modified: Fri Jan 12 07:33:17 2024, max compression
+gzip compressed data, was "pyxdf-1.16.6.tar", last modified: Thu Apr 18 07:42:04 2024, max compression
```

## Comparing `pyxdf-1.16.5.tar` & `pyxdf-1.16.6.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-01-12 07:33:17.492525 pyxdf-1.16.5/
--rw-r--r--   0 clemens    (501) staff       (20)     1275 2023-05-25 10:10:46.000000 pyxdf-1.16.5/.gitignore
--rw-r--r--   0 clemens    (501) staff       (20)     5173 2024-01-12 07:28:17.000000 pyxdf-1.16.5/CHANGELOG.md
--rw-r--r--   0 clemens    (501) staff       (20)     1433 2023-05-25 10:10:46.000000 pyxdf-1.16.5/LICENSE
--rw-r--r--   0 clemens    (501) staff       (20)     2332 2024-01-12 07:33:17.492453 pyxdf-1.16.5/PKG-INFO
--rw-r--r--   0 clemens    (501) staff       (20)     1508 2023-05-25 10:10:46.000000 pyxdf-1.16.5/README.md
--rw-r--r--   0 clemens    (501) staff       (20)     1339 2023-05-25 10:10:46.000000 pyxdf-1.16.5/azure-pipelines.yml
-drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-01-12 07:33:17.491007 pyxdf-1.16.5/pyxdf/
--rw-r--r--   0 clemens    (501) staff       (20)      563 2024-01-12 07:28:17.000000 pyxdf-1.16.5/pyxdf/__init__.py
--rw-r--r--   0 clemens    (501) staff       (20)     1087 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/example.py
--rw-r--r--   0 clemens    (501) staff       (20)     1000 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/pyxdf.pxd
--rw-r--r--   0 clemens    (501) staff       (20)    33497 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/pyxdf.py
-drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-01-12 07:33:17.492077 pyxdf-1.16.5/pyxdf/test/
--rw-r--r--   0 clemens    (501) staff       (20)        0 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/test/__init__.py
--rw-r--r--   0 clemens    (501) staff       (20)     2691 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/test/test_data.py
--rw-r--r--   0 clemens    (501) staff       (20)      973 2023-05-25 10:10:46.000000 pyxdf-1.16.5/pyxdf/test/test_library_basic.py
-drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-01-12 07:33:17.492253 pyxdf-1.16.5/pyxdf.egg-info/
--rw-r--r--   0 clemens    (501) staff       (20)     2332 2024-01-12 07:33:17.000000 pyxdf-1.16.5/pyxdf.egg-info/PKG-INFO
--rw-r--r--   0 clemens    (501) staff       (20)      370 2024-01-12 07:33:17.000000 pyxdf-1.16.5/pyxdf.egg-info/SOURCES.txt
--rw-r--r--   0 clemens    (501) staff       (20)        1 2024-01-12 07:33:17.000000 pyxdf-1.16.5/pyxdf.egg-info/dependency_links.txt
--rw-r--r--   0 clemens    (501) staff       (20)        6 2024-01-12 07:33:17.000000 pyxdf-1.16.5/pyxdf.egg-info/requires.txt
--rw-r--r--   0 clemens    (501) staff       (20)        6 2024-01-12 07:33:17.000000 pyxdf-1.16.5/pyxdf.egg-info/top_level.txt
--rw-r--r--   0 clemens    (501) staff       (20)      102 2024-01-12 07:33:17.492718 pyxdf-1.16.5/setup.cfg
--rw-r--r--   0 clemens    (501) staff       (20)     3802 2023-05-25 10:10:46.000000 pyxdf-1.16.5/setup.py
+drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-04-18 07:42:04.195046 pyxdf-1.16.6/
+-rw-r--r--   0 clemens    (501) staff       (20)     1275 2023-05-25 10:10:46.000000 pyxdf-1.16.6/.gitignore
+-rw-r--r--   0 clemens    (501) staff       (20)     5364 2024-04-18 07:30:39.000000 pyxdf-1.16.6/CHANGELOG.md
+-rw-r--r--   0 clemens    (501) staff       (20)     1433 2024-04-18 07:20:56.000000 pyxdf-1.16.6/LICENSE
+-rw-r--r--   0 clemens    (501) staff       (20)     3070 2024-04-18 07:42:04.194988 pyxdf-1.16.6/PKG-INFO
+-rw-r--r--   0 clemens    (501) staff       (20)     2043 2024-04-18 07:20:56.000000 pyxdf-1.16.6/README.md
+-rw-r--r--   0 clemens    (501) staff       (20)     1339 2024-04-18 07:20:56.000000 pyxdf-1.16.6/azure-pipelines.yml
+drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-04-18 07:42:04.192892 pyxdf-1.16.6/pyxdf/
+-rw-r--r--   0 clemens    (501) staff       (20)      386 2024-04-18 07:20:56.000000 pyxdf-1.16.6/pyxdf/__init__.py
+drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-04-18 07:42:04.193958 pyxdf-1.16.6/pyxdf/examples/
+-rw-r--r--   0 clemens    (501) staff       (20)        0 2024-04-10 05:39:02.000000 pyxdf-1.16.6/pyxdf/examples/__init__.py
+-rw-r--r--   0 clemens    (501) staff       (20)     8587 2024-04-10 05:39:02.000000 pyxdf-1.16.6/pyxdf/examples/playback_lsl.py
+-rw-r--r--   0 clemens    (501) staff       (20)     1424 2024-04-10 05:39:02.000000 pyxdf-1.16.6/pyxdf/examples/print_metadata.py
+-rw-r--r--   0 clemens    (501) staff       (20)     1000 2023-05-25 10:10:46.000000 pyxdf-1.16.6/pyxdf/pyxdf.pxd
+-rw-r--r--   0 clemens    (501) staff       (20)    33766 2024-04-10 05:39:02.000000 pyxdf-1.16.6/pyxdf/pyxdf.py
+drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-04-18 07:42:04.194296 pyxdf-1.16.6/pyxdf/test/
+-rw-r--r--   0 clemens    (501) staff       (20)        0 2023-05-25 10:10:46.000000 pyxdf-1.16.6/pyxdf/test/__init__.py
+-rw-r--r--   0 clemens    (501) staff       (20)     2691 2023-05-25 10:10:46.000000 pyxdf-1.16.6/pyxdf/test/test_data.py
+-rw-r--r--   0 clemens    (501) staff       (20)      973 2023-05-25 10:10:46.000000 pyxdf-1.16.6/pyxdf/test/test_library_basic.py
+drwxr-xr-x   0 clemens    (501) staff       (20)        0 2024-04-18 07:42:04.194715 pyxdf-1.16.6/pyxdf.egg-info/
+-rw-r--r--   0 clemens    (501) staff       (20)     3070 2024-04-18 07:42:04.000000 pyxdf-1.16.6/pyxdf.egg-info/PKG-INFO
+-rw-r--r--   0 clemens    (501) staff       (20)      444 2024-04-18 07:42:04.000000 pyxdf-1.16.6/pyxdf.egg-info/SOURCES.txt
+-rw-r--r--   0 clemens    (501) staff       (20)        1 2024-04-18 07:42:04.000000 pyxdf-1.16.6/pyxdf.egg-info/dependency_links.txt
+-rw-r--r--   0 clemens    (501) staff       (20)        6 2024-04-18 07:42:04.000000 pyxdf-1.16.6/pyxdf.egg-info/requires.txt
+-rw-r--r--   0 clemens    (501) staff       (20)        6 2024-04-18 07:42:04.000000 pyxdf-1.16.6/pyxdf.egg-info/top_level.txt
+-rw-r--r--   0 clemens    (501) staff       (20)      102 2024-04-18 07:42:04.195296 pyxdf-1.16.6/setup.cfg
+-rw-r--r--   0 clemens    (501) staff       (20)     1867 2024-04-18 07:20:56.000000 pyxdf-1.16.6/setup.py
```

### Comparing `pyxdf-1.16.5/.gitignore` & `pyxdf-1.16.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyxdf-1.16.5/CHANGELOG.md` & `pyxdf-1.16.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## [1.16.6] - 2024-04-18
+### Changed
+- Minimum required Python version is now 3.9 ([#100](https://github.com/xdf-modules/xdf-Python/pull/100) by [Clemens Brunner](https://github.com/cbrnr))
+
 ## [1.16.5] - 2024-01-12
 ### Added
 - Added compatibility with Python 3.12 ([#96](https://github.com/xdf-modules/xdf-Python/pull/96) by [Clemens Brunner](https://github.com/cbrnr))
 
 ## [1.16.4] - 2023-01-09
 ### Fixed
 - Fix invalid `np.object` type ([#87](https://github.com/xdf-modules/xdf-Python/pull/87) by [Clemens Brunner](https://github.com/cbrnr))
```

### Comparing `pyxdf-1.16.5/LICENSE` & `pyxdf-1.16.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 BSD 2-Clause License
 
-Copyright (c) 2015-2023, Syntrogi Inc. dba Intheon
-Copyright (c) 2018-2023, Chad Boulay
-Copyright (c) 2018-2023, Tristan Stenner
-Copyright (c) 2018-2023, Clemens Brunner
+Copyright (c) 2015-2024, Syntrogi Inc. dba Intheon
+Copyright (c) 2018-2024, Chad Boulay
+Copyright (c) 2018-2024, Tristan Stenner
+Copyright (c) 2018-2024, Clemens Brunner
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pyxdf-1.16.5/PKG-INFO` & `pyxdf-1.16.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: pyxdf
-Version: 1.16.5
+Version: 1.16.6
 Summary: Python library for importing XDF (Extensible Data Format)
 Home-page: https://github.com/xdf-modules/xdf-Python
 Author: Christian Kothe
 Author-email: christian.kothe@intheon.io
 License: BSD
-Keywords: XDF,pyxdf,LSL,Lab Streaming Layer,File Format,biosignals,stream
+Keywords: XDF,pyxdf,LSL,Lab Streaming Layer,file format,biosignals,stream
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 [![Latest PyPI Release](https://img.shields.io/pypi/v/pyxdf)](https://pypi.org/project/pyxdf/)
 [![Latest Conda Release](https://img.shields.io/conda/vn/conda-forge/pyxdf)](https://anaconda.org/conda-forge/pyxdf)
-![Python 3.5+](https://img.shields.io/badge/python-3.5+-green.svg)
+![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 ![License](https://img.shields.io/github/license/xdf-modules/xdf-python)
 
 pyXDF
 =====
 
 pyXDF is a Python importer for [XDF](https://github.com/sccn/xdf) files.
 
@@ -52,14 +56,23 @@
         plt.plot(stream['time_stamps'], y)
     else:
         raise RuntimeError('Unknown stream format')
 
 plt.show()
 ```
 
+## CLI examples
+
+`pyxdf` has an `examples` module. These can be run from the command line for basic functionality.
+
+* `print_metadata` will enable a DEBUG logger to log read messages, then it will print basic metadata about each found stream.
+    * `python -m pyxdf.examples.print_metadata -f=/path/to/my.xdf`
+* `playback_lsl` will open an XDF file then replay its data in an infinite loop, but using current timestamps. This is useful for prototyping online processing.
+    * `python -m pyxdf.examples.playback_lsl /path/to/my.xdf` 
+
 ## Installation
 
 The latest stable version can be installed with `pip install pyxdf`.
 
 For the latest development version, use `pip install git+https://github.com/xdf-modules/pyxdf.git`.
 
 ## For maintainers
```

### Comparing `pyxdf-1.16.5/azure-pipelines.yml` & `pyxdf-1.16.6/azure-pipelines.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     include:
     - main
 
 pool:
   vmImage: 'ubuntu-latest'
 strategy:
   matrix:
-    Python37:
-      python.version: '3.7'
+    Python39:
+      python.version: '3.9'
 
 steps:
 - task: UsePythonVersion@0
   inputs:
     versionSpec: '$(python.version)'
   displayName: 'Use Python $(python.version)'
```

### Comparing `pyxdf-1.16.5/pyxdf/pyxdf.pxd` & `pyxdf-1.16.6/pyxdf/pyxdf.pxd`

 * *Files identical despite different names*

### Comparing `pyxdf-1.16.5/pyxdf/pyxdf.py` & `pyxdf-1.16.6/pyxdf/pyxdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 This function is closely following the load_xdf reference implementation.
 """
 import io
 import struct
 import itertools
 import gzip
-from xml.etree.ElementTree import fromstring
+from xml.etree.ElementTree import fromstring, ParseError
 from collections import OrderedDict, defaultdict
 import logging
 from pathlib import Path
 
 import numpy as np
 
 
@@ -324,15 +324,21 @@
                         "found likely XDF file corruption (%s), "
                         "scanning forward to next boundary chunk." % e
                     )
                     _scan_forward(f)
             elif tag == 6:
                 # read [StreamFooter] chunk
                 xml_string = f.read(chunklen - 6)
-                streams[StreamId]["footer"] = _xml2dict(fromstring(xml_string))
+                try:
+                    streams[StreamId]["footer"] = _xml2dict(fromstring(xml_string))
+                except ParseError as e:
+                    logger.error(
+                        f"found likely XDF file corruption ({e}), "
+                        "ignoring corrupted XML element in footer."
+                    )
             elif tag == 4:
                 # read [ClockOffset] chunk
                 temp[StreamId].clock_times.append(
                     struct.unpack("<d", f.read(8))[0]
                 )
                 temp[StreamId].clock_values.append(
                     struct.unpack("<d", f.read(8))[0]
```

### Comparing `pyxdf-1.16.5/pyxdf/test/test_data.py` & `pyxdf-1.16.6/pyxdf/test/test_data.py`

 * *Files identical despite different names*

### Comparing `pyxdf-1.16.5/pyxdf/test/test_library_basic.py` & `pyxdf-1.16.6/pyxdf/test/test_library_basic.py`

 * *Files identical despite different names*

### Comparing `pyxdf-1.16.5/pyxdf.egg-info/PKG-INFO` & `pyxdf-1.16.6/pyxdf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: pyxdf
-Version: 1.16.5
+Version: 1.16.6
 Summary: Python library for importing XDF (Extensible Data Format)
 Home-page: https://github.com/xdf-modules/xdf-Python
 Author: Christian Kothe
 Author-email: christian.kothe@intheon.io
 License: BSD
-Keywords: XDF,pyxdf,LSL,Lab Streaming Layer,File Format,biosignals,stream
+Keywords: XDF,pyxdf,LSL,Lab Streaming Layer,file format,biosignals,stream
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 [![Latest PyPI Release](https://img.shields.io/pypi/v/pyxdf)](https://pypi.org/project/pyxdf/)
 [![Latest Conda Release](https://img.shields.io/conda/vn/conda-forge/pyxdf)](https://anaconda.org/conda-forge/pyxdf)
-![Python 3.5+](https://img.shields.io/badge/python-3.5+-green.svg)
+![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
 ![License](https://img.shields.io/github/license/xdf-modules/xdf-python)
 
 pyXDF
 =====
 
 pyXDF is a Python importer for [XDF](https://github.com/sccn/xdf) files.
 
@@ -52,14 +56,23 @@
         plt.plot(stream['time_stamps'], y)
     else:
         raise RuntimeError('Unknown stream format')
 
 plt.show()
 ```
 
+## CLI examples
+
+`pyxdf` has an `examples` module. These can be run from the command line for basic functionality.
+
+* `print_metadata` will enable a DEBUG logger to log read messages, then it will print basic metadata about each found stream.
+    * `python -m pyxdf.examples.print_metadata -f=/path/to/my.xdf`
+* `playback_lsl` will open an XDF file then replay its data in an infinite loop, but using current timestamps. This is useful for prototyping online processing.
+    * `python -m pyxdf.examples.playback_lsl /path/to/my.xdf` 
+
 ## Installation
 
 The latest stable version can be installed with `pip install pyxdf`.
 
 For the latest development version, use `pip install git+https://github.com/xdf-modules/pyxdf.git`.
 
 ## For maintainers
```

