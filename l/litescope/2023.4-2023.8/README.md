# Comparing `tmp/litescope-2023.4.tar.gz` & `tmp/litescope-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litescope-2023.4.tar", last modified: Thu Apr 18 20:10:59 2024, max compression
+gzip compressed data, was "litescope-2023.8.tar", last modified: Thu Apr 18 20:11:27 2024, max compression
```

## Comparing `litescope-2023.4.tar` & `litescope-2023.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.368275 litescope-2023.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1684 2024-04-18 20:09:07.000000 litescope-2023.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)     4408 2024-04-18 20:10:59.367988 litescope-2023.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4021 2024-04-18 20:09:07.000000 litescope-2023.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.363045 litescope-2023.4/litescope/
--rw-r--r--   0 timkpaine   (501) staff       (20)      188 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10671 2024-04-18 20:09:26.000000 litescope-2023.4/litescope/core.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.364214 litescope-2023.4/litescope/software/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.364811 litescope-2023.4/litescope/software/driver/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/driver/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7575 2024-04-18 20:10:39.000000 litescope-2023.4/litescope/software/driver/analyzer.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      540 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/driver/io.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.366732 litescope-2023.4/litescope/software/dump/
--rw-r--r--   0 timkpaine   (501) staff       (20)      326 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3012 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/common.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1424 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/csv.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      678 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/json.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      847 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/python.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4486 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/sigrok.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4104 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/dump/vcd.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8268 2024-04-18 20:09:07.000000 litescope-2023.4/litescope/software/litescope_cli.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.367681 litescope-2023.4/litescope.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4408 2024-04-18 20:10:59.000000 litescope-2023.4/litescope.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      703 2024-04-18 20:10:59.000000 litescope-2023.4/litescope.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:10:59.000000 litescope-2023.4/litescope.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       72 2024-04-18 20:10:59.000000 litescope-2023.4/litescope.egg-info/entry_points.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       10 2024-04-18 20:10:59.000000 litescope-2023.4/litescope.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:10:59.368332 litescope-2023.4/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)      912 2024-04-18 20:10:56.000000 litescope-2023.4/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:10:59.367419 litescope-2023.4/test/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1784 2024-04-18 20:09:07.000000 litescope-2023.4/test/test_analyzer.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1191 2024-04-18 20:09:07.000000 litescope-2023.4/test/test_dump.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      579 2024-04-18 20:09:07.000000 litescope-2023.4/test/test_examples.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.403901 litescope-2023.8/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1684 2024-04-18 20:09:07.000000 litescope-2023.8/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4408 2024-04-18 20:11:27.403668 litescope-2023.8/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4021 2024-04-18 20:09:07.000000 litescope-2023.8/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.399640 litescope-2023.8/litescope/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      188 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10675 2024-04-18 20:11:17.000000 litescope-2023.8/litescope/core.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.400655 litescope-2023.8/litescope/software/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.401364 litescope-2023.8/litescope/software/driver/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/driver/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7575 2024-04-18 20:10:39.000000 litescope-2023.8/litescope/software/driver/analyzer.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      540 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/driver/io.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.402672 litescope-2023.8/litescope/software/dump/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      326 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3012 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1424 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/csv.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      678 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/json.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      847 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/python.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4486 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/sigrok.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4104 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/dump/vcd.py
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)     8268 2024-04-18 20:09:07.000000 litescope-2023.8/litescope/software/litescope_cli.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.403429 litescope-2023.8/litescope.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4408 2024-04-18 20:11:27.000000 litescope-2023.8/litescope.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      703 2024-04-18 20:11:27.000000 litescope-2023.8/litescope.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:11:27.000000 litescope-2023.8/litescope.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       72 2024-04-18 20:11:27.000000 litescope-2023.8/litescope.egg-info/entry_points.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       10 2024-04-18 20:11:27.000000 litescope-2023.8/litescope.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:11:27.403951 litescope-2023.8/setup.cfg
+-rwxr-xr-x   0 timkpaine   (501) staff       (20)      912 2024-04-18 20:11:25.000000 litescope-2023.8/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:11:27.403201 litescope-2023.8/test/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1784 2024-04-18 20:09:07.000000 litescope-2023.8/test/test_analyzer.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1191 2024-04-18 20:09:07.000000 litescope-2023.8/test/test_dump.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      579 2024-04-18 20:09:07.000000 litescope-2023.8/test/test_examples.py
```

### Comparing `litescope-2023.4/LICENSE` & `litescope-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/PKG-INFO` & `litescope-2023.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litescope
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable embedded FPGA logic analyzer core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litescope
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litescope-2023.4/README.md` & `litescope-2023.8/README.md`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/core.py` & `litescope-2023.8/litescope/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #
 # Copyright (c) 2016-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2018 bunnie <bunnie@kosagi.com>
 # Copyright (c) 2016 Tim 'mithro' Ansell <mithro@mithis.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.misc import WaitTimer
 from migen.genlib.cdc import MultiReg, PulseSynchronizer
 
+from litex.gen.genlib.misc import WaitTimer
 from litex.build.tools import write_to_file
 
 from litex.soc.interconnect.csr import *
 from litex.soc.cores.gpio import GPIOInOut
 from litex.soc.interconnect import stream
 
 # LiteScope IO -------------------------------------------------------------------------------------
```

### Comparing `litescope-2023.4/litescope/software/driver/analyzer.py` & `litescope-2023.8/litescope/software/driver/analyzer.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/driver/io.py` & `litescope-2023.8/litescope/software/driver/io.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/common.py` & `litescope-2023.8/litescope/software/dump/common.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/csv.py` & `litescope-2023.8/litescope/software/dump/csv.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/json.py` & `litescope-2023.8/litescope/software/dump/json.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/python.py` & `litescope-2023.8/litescope/software/dump/python.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/sigrok.py` & `litescope-2023.8/litescope/software/dump/sigrok.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/dump/vcd.py` & `litescope-2023.8/litescope/software/dump/vcd.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope/software/litescope_cli.py` & `litescope-2023.8/litescope/software/litescope_cli.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/litescope.egg-info/PKG-INFO` & `litescope-2023.8/litescope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litescope
-Version: 2023.4
+Version: 2023.8
 Summary: Small footprint and configurable embedded FPGA logic analyzer core
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/enjoy-digital/litescope
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
 Requires-Python: ~=3.6
```

### Comparing `litescope-2023.4/litescope.egg-info/SOURCES.txt` & `litescope-2023.8/litescope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/setup.py` & `litescope-2023.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = fp.read()
 
 setup(
     name="litescope",
     description="Small footprint and configurable embedded FPGA logic analyzer core",
     long_description              = long_description,
     long_description_content_type = "text/markdown",
-    version="2023.04",
+    version="2023.08",
     author="Florent Kermarrec",
     author_email="florent@enjoy-digital.fr",
     url="http://enjoy-digital.fr",
     download_url="https://github.com/enjoy-digital/litescope",
     test_suite="test",
     license="BSD",
     python_requires="~=3.6",
```

### Comparing `litescope-2023.4/test/test_analyzer.py` & `litescope-2023.8/test/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/test/test_dump.py` & `litescope-2023.8/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `litescope-2023.4/test/test_examples.py` & `litescope-2023.8/test/test_examples.py`

 * *Files identical despite different names*

