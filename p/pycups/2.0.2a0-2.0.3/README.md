# Comparing `tmp/pycups-2.0.2a0.tar.gz` & `tmp/pycups-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycups-2.0.2a0.tar", last modified: Wed Apr 17 14:25:32 2024, max compression
+gzip compressed data, was "pycups-2.0.3.tar", last modified: Wed Apr 17 14:28:43 2024, max compression
```

## Comparing `pycups-2.0.2a0.tar` & `pycups-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.518317 pycups-2.0.2a0/
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    18092 2022-08-31 12:07:01.000000 pycups-2.0.2a0/COPYING
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      256 2022-08-31 12:07:01.000000 pycups-2.0.2a0/MANIFEST.in
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1222 2024-04-17 11:25:39.000000 pycups-2.0.2a0/Makefile
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    11598 2024-04-17 11:30:11.000000 pycups-2.0.2a0/NEWS
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1247 2024-04-17 14:25:32.518317 pycups-2.0.2a0/PKG-INFO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1189 2022-10-25 13:03:09.000000 pycups-2.0.2a0/README
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      214 2022-08-31 12:07:01.000000 pycups-2.0.2a0/TODO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)   172355 2024-04-17 11:30:11.000000 pycups-2.0.2a0/cupsconnection.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2118 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsconnection.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    22247 2024-04-17 11:30:11.000000 pycups-2.0.2a0/cupsipp.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1386 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsipp.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    36411 2022-10-25 13:03:04.000000 pycups-2.0.2a0/cupsmodule.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1660 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsmodule.h
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    46838 2022-10-25 13:03:04.000000 pycups-2.0.2a0/cupsppd.c
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1358 2022-08-31 12:07:01.000000 pycups-2.0.2a0/cupsppd.h
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.517317 pycups-2.0.2a0/examples/
--rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     2114 2023-04-06 06:01:00.000000 pycups-2.0.2a0/examples/cupstree.py
--rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     7754 2022-08-31 12:07:01.000000 pycups-2.0.2a0/postscriptdriver.prov
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      165 2022-08-31 12:07:01.000000 pycups-2.0.2a0/psdriver.attr
-drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:25:32.518317 pycups-2.0.2a0/pycups.egg-info/
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1247 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/PKG-INFO
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      368 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/SOURCES.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        1 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/dependency_links.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       18 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/requires.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        5 2024-04-17 14:25:32.000000 pycups-2.0.2a0/pycups.egg-info/top_level.txt
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       38 2024-04-17 14:25:32.518317 pycups-2.0.2a0/setup.cfg
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2746 2024-04-17 14:22:29.000000 pycups-2.0.2a0/setup.py
--rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1401 2023-04-06 08:19:15.000000 pycups-2.0.2a0/test.py
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:28:43.393506 pycups-2.0.3/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    18092 2022-08-31 12:07:01.000000 pycups-2.0.3/COPYING
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      256 2022-08-31 12:07:01.000000 pycups-2.0.3/MANIFEST.in
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1222 2024-04-17 11:25:39.000000 pycups-2.0.3/Makefile
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    11598 2024-04-17 11:30:11.000000 pycups-2.0.3/NEWS
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1245 2024-04-17 14:28:43.393506 pycups-2.0.3/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1189 2022-10-25 13:03:09.000000 pycups-2.0.3/README
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      214 2022-08-31 12:07:01.000000 pycups-2.0.3/TODO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)   172355 2024-04-17 11:30:11.000000 pycups-2.0.3/cupsconnection.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2118 2022-08-31 12:07:01.000000 pycups-2.0.3/cupsconnection.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    22247 2024-04-17 11:30:11.000000 pycups-2.0.3/cupsipp.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1386 2022-08-31 12:07:01.000000 pycups-2.0.3/cupsipp.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    36411 2022-10-25 13:03:04.000000 pycups-2.0.3/cupsmodule.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1660 2022-08-31 12:07:01.000000 pycups-2.0.3/cupsmodule.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    46838 2022-10-25 13:03:04.000000 pycups-2.0.3/cupsppd.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1358 2022-08-31 12:07:01.000000 pycups-2.0.3/cupsppd.h
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:28:43.392506 pycups-2.0.3/examples/
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     2114 2023-04-06 06:01:00.000000 pycups-2.0.3/examples/cupstree.py
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     7754 2022-08-31 12:07:01.000000 pycups-2.0.3/postscriptdriver.prov
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      165 2022-08-31 12:07:01.000000 pycups-2.0.3/psdriver.attr
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 14:28:43.392506 pycups-2.0.3/pycups.egg-info/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1245 2024-04-17 14:28:43.000000 pycups-2.0.3/pycups.egg-info/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      368 2024-04-17 14:28:43.000000 pycups-2.0.3/pycups.egg-info/SOURCES.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        1 2024-04-17 14:28:43.000000 pycups-2.0.3/pycups.egg-info/dependency_links.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       18 2024-04-17 14:28:43.000000 pycups-2.0.3/pycups.egg-info/requires.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        5 2024-04-17 14:28:43.000000 pycups-2.0.3/pycups.egg-info/top_level.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       38 2024-04-17 14:28:43.393506 pycups-2.0.3/setup.cfg
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2745 2024-04-17 14:27:05.000000 pycups-2.0.3/setup.py
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1401 2023-04-06 08:19:15.000000 pycups-2.0.3/test.py
```

### Comparing `pycups-2.0.2a0/COPYING` & `pycups-2.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/Makefile` & `pycups-2.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/NEWS` & `pycups-2.0.3/NEWS`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/PKG-INFO` & `pycups-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycups
-Version: 2.0.2a0
+Version: 2.0.3
 Summary: Python bindings for libcups
 Home-page: https://github.com/OpenPrinting/pycups
 Download-URL: https://github.com/OpenPrinting/pycups/releases
 Maintainer: Zdenek Dohnal
 Maintainer-email: zdohnal@redhat.com
 License: GPLv2+
 Classifier: Intended Audience :: Developers
```

### Comparing `pycups-2.0.2a0/README` & `pycups-2.0.3/README`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsconnection.c` & `pycups-2.0.3/cupsconnection.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsconnection.h` & `pycups-2.0.3/cupsconnection.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsipp.c` & `pycups-2.0.3/cupsipp.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsipp.h` & `pycups-2.0.3/cupsipp.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsmodule.c` & `pycups-2.0.3/cupsmodule.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsmodule.h` & `pycups-2.0.3/cupsmodule.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsppd.c` & `pycups-2.0.3/cupsppd.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/cupsppd.h` & `pycups-2.0.3/cupsppd.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/examples/cupstree.py` & `pycups-2.0.3/examples/cupstree.py`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/postscriptdriver.prov` & `pycups-2.0.3/postscriptdriver.prov`

 * *Files identical despite different names*

### Comparing `pycups-2.0.2a0/pycups.egg-info/PKG-INFO` & `pycups-2.0.3/pycups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycups
-Version: 2.0.2a0
+Version: 2.0.3
 Summary: Python bindings for libcups
 Home-page: https://github.com/OpenPrinting/pycups
 Download-URL: https://github.com/OpenPrinting/pycups/releases
 Maintainer: Zdenek Dohnal
 Maintainer-email: zdohnal@redhat.com
 License: GPLv2+
 Classifier: Intended Audience :: Developers
```

### Comparing `pycups-2.0.2a0/setup.py` & `pycups-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 duplex ipp://192.168.1.1:631/printers/duplex
 HP-LaserJet-6MP ipp://192.168.1.1:631/printers/HP-LaserJet-6MP
 EPSON-Stylus-D78 usb://EPSON/Stylus%20D78
 """
 
 from distutils.core import setup, Extension
 import sys
-VERSION="2.0.2a"
+VERSION="2.0.3"
 libraries=["cups"]
 
 if sys.platform == "darwin" or sys.platform.startswith("freebsd"):
     libraries.append ("iconv")
 
 setup (name="pycups",
        version=VERSION,
```

### Comparing `pycups-2.0.2a0/test.py` & `pycups-2.0.3/test.py`

 * *Files identical despite different names*

