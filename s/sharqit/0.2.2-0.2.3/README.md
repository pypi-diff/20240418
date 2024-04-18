# Comparing `tmp/sharqit-0.2.2.tar.gz` & `tmp/sharqit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharqit-0.2.2.tar", last modified: Fri Apr  5 13:15:59 2024, max compression
+gzip compressed data, was "sharqit-0.2.3.tar", last modified: Thu Apr 18 13:19:52 2024, max compression
```

## Comparing `sharqit-0.2.2.tar` & `sharqit-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1572 2024-03-27 12:57:53.000000 sharqit-0.2.2/CMakeLists.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1067 2024-02-17 09:27:38.000000 sharqit-0.2.2/LICENSE
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       79 2024-03-14 14:57:12.000000 sharqit-0.2.2/MANIFEST.in
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-05 13:15:59.769859 sharqit-0.2.2/PKG-INFO
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4981 2024-04-05 12:58:50.000000 sharqit-0.2.2/README.md
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       38 2024-04-05 13:15:59.769859 sharqit-0.2.2/setup.cfg
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1910 2024-04-05 12:58:50.000000 sharqit-0.2.2/setup.py
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       92 2024-03-26 14:24:02.000000 sharqit-0.2.2/sharqit/__init__.py
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit/cpp/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1506 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/CMakeLists.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)   112731 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/Doxyfile
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2114 2024-03-17 23:24:30.000000 sharqit-0.2.2/sharqit/cpp/Makefile
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    26788 2024-03-31 23:29:48.000000 sharqit-0.2.2/sharqit/cpp/TAGS
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2430 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/binary_matrix.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5970 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/binary_matrix.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14930 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dag.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    20976 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      406 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagedge.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      317 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/dagnode.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    11949 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/extract_qcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      357 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/fraction.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8343 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/fraction.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4047 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/linear_map.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4528 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/linear_map.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8745 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/merge_rotation.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10169 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/nb_sharqit.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5118 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/optimizer.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     3792 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/optimizer.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2487 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/phase.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4239 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/phase.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2342 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/propagate_pauli_x.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28756 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qcirc.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    27013 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qcirc.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14516 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qgate.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10490 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/qgate.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     7660 2024-03-14 23:07:51.000000 sharqit-0.2.2/sharqit/cpp/sharqit.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      385 2024-04-05 12:58:50.000000 sharqit-0.2.2/sharqit/cpp/sharqit.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28969 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/simplify.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2168 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/util.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28058 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zx.h
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    17166 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zxdiagram.cpp
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      539 2024-03-14 14:57:12.000000 sharqit-0.2.2/sharqit/cpp/zxnode.cpp
-drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-05 13:15:59.769859 sharqit-0.2.2/sharqit.egg-info/
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/PKG-INFO
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1015 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/SOURCES.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)        1 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/dependency_links.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       16 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/requires.txt
--rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       25 2024-04-05 13:15:59.000000 sharqit-0.2.2/sharqit.egg-info/top_level.txt
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-18 13:19:52.361111 sharqit-0.2.3/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1572 2024-03-27 12:57:53.000000 sharqit-0.2.3/CMakeLists.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1067 2024-02-17 09:27:38.000000 sharqit-0.2.3/LICENSE
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       79 2024-03-14 14:57:12.000000 sharqit-0.2.3/MANIFEST.in
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-18 13:19:52.361111 sharqit-0.2.3/PKG-INFO
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4981 2024-04-05 13:26:28.000000 sharqit-0.2.3/README.md
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       38 2024-04-18 13:19:52.361111 sharqit-0.2.3/setup.cfg
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1910 2024-04-18 13:06:12.000000 sharqit-0.2.3/setup.py
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-18 13:19:52.361111 sharqit-0.2.3/sharqit/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       92 2024-03-26 14:24:02.000000 sharqit-0.2.3/sharqit/__init__.py
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-18 13:19:52.361111 sharqit-0.2.3/sharqit/cpp/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1506 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/CMakeLists.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)   112731 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/Doxyfile
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2114 2024-03-17 23:24:30.000000 sharqit-0.2.3/sharqit/cpp/Makefile
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    29297 2024-04-13 02:14:16.000000 sharqit-0.2.3/sharqit/cpp/TAGS
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2430 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/binary_matrix.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5970 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/binary_matrix.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    14976 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/dag.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    21035 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/dagcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      406 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/dagedge.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      317 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/dagnode.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    11949 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/extract_qcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      357 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/fraction.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8343 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/fraction.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4047 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/linear_map.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4528 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/linear_map.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     8921 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/merge_rotation.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    12887 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/nb_sharqit.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     5161 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/optimizer.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     3792 2024-04-16 00:12:03.000000 sharqit-0.2.3/sharqit/cpp/optimizer.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2487 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/phase.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     4239 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/phase.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2342 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/propagate_pauli_x.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    35195 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/qcirc.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28947 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/qcirc.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    15884 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/qgate.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    10845 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/qgate.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     7660 2024-04-10 12:28:22.000000 sharqit-0.2.3/sharqit/cpp/sharqit.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      385 2024-04-18 13:06:12.000000 sharqit-0.2.3/sharqit/cpp/sharqit.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28969 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/simplify.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     2168 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/util.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    28058 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/zx.h
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)    17166 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/zxdiagram.cpp
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      539 2024-03-14 14:57:12.000000 sharqit-0.2.3/sharqit/cpp/zxnode.cpp
+drwxr-xr-x   0 nakagawa  (1000) nakagawa  (1000)        0 2024-04-18 13:19:52.361111 sharqit-0.2.3/sharqit.egg-info/
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)      437 2024-04-18 13:19:52.000000 sharqit-0.2.3/sharqit.egg-info/PKG-INFO
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)     1015 2024-04-18 13:19:52.000000 sharqit-0.2.3/sharqit.egg-info/SOURCES.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)        1 2024-04-18 13:19:52.000000 sharqit-0.2.3/sharqit.egg-info/dependency_links.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       16 2024-04-18 13:19:52.000000 sharqit-0.2.3/sharqit.egg-info/requires.txt
+-rw-r--r--   0 nakagawa  (1000) nakagawa  (1000)       25 2024-04-18 13:19:52.000000 sharqit-0.2.3/sharqit.egg-info/top_level.txt
```

### Comparing `sharqit-0.2.2/CMakeLists.txt` & `sharqit-0.2.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/LICENSE` & `sharqit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/README.md` & `sharqit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/setup.py` & `sharqit-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 import pathlib
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext as build_ext_orig
 
-_VERSION = '0.2.2'
+_VERSION = '0.2.3'
 
 class CMakeExtension(Extension):
 
     def __init__(self, name):
         super().__init__(name, sources=[])
 
 class build_ext(build_ext_orig):
```

### Comparing `sharqit-0.2.2/sharqit/cpp/CMakeLists.txt` & `sharqit-0.2.3/sharqit/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/Doxyfile` & `sharqit-0.2.3/sharqit/cpp/Doxyfile`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/Makefile` & `sharqit-0.2.3/sharqit/cpp/Makefile`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/TAGS` & `sharqit-0.2.3/sharqit/cpp/TAGS`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 0c0a 7072 6f70 6167 6174 655f 7061 756c  ..propagate_paul
 00000010: 695f 782e 6370 702c 3634 0a76 6f69 6420  i_x.cpp,64.void 
 00000020: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
 00000030: 7072 6f70 6167 6174 655f 7061 756c 695f  propagate_pauli_
 00000040: 7828 7f70 726f 7061 6761 7465 5f70 6175  x(.propagate_pau
 00000050: 6c69 5f78 0139 2c31 3938 0a0c 0a6e 625f  li_x.9,198...nb_
 00000060: 7368 6172 7169 742e 6370 702c 3138 0a4e  sharqit.cpp,18.N
-00000070: 425f 4d4f 4455 4c45 287f 3230 2c34 3139  B_MODULE(.20,419
+00000070: 425f 4d4f 4455 4c45 287f 3232 2c34 3932  B_MODULE(.22,492
 00000080: 0a0c 0a6c 696e 6561 725f 6d61 702e 682c  ...linear_map.h,
 00000090: 3638 370a 2364 6566 696e 6520 4c49 4e45  687.#define LINE
 000000a0: 4152 5f4d 4150 5f48 7f37 2c39 340a 6e61  AR_MAP_H.7,94.na
 000000b0: 6d65 7370 6163 6520 5368 6172 7169 7420  mespace Sharqit 
 000000c0: 7f31 362c 3231 340a 2020 636c 6173 7320  .16,214.  class 
 000000d0: 4c69 6e65 6172 4d61 7020 7f32 342c 3337  LinearMap .24,37
 000000e0: 300a 2020 2020 4c69 6e65 6172 4d61 7028  0.    LinearMap(
@@ -273,1403 +273,1560 @@
 00001100: 7369 626c 6501 3534 2c31 3237 370a 7374  sible.54,1277.st
 00001110: 643a 3a76 6563 746f 723c 7374 643a 3a70  d::vector<std::p
 00001120: 6169 723c 7569 6e74 3332 5f74 2c20 7569  air<uint32_t, ui
 00001130: 6e74 3332 5f74 3e3e 2053 6861 7271 3a3a  nt32_t>> Sharq::
 00001140: 4269 6e61 7279 4d61 7472 6978 3a3a 6761  BinaryMatrix::ga
 00001150: 7573 735f 7265 6475 6365 287f 6761 7573  uss_reduce(.gaus
 00001160: 735f 7265 6475 6365 0137 312c 3135 3433  s_reduce.71,1543
-00001170: 0a0c 0a71 6369 7263 2e63 7070 2c31 3932  ...qcirc.cpp,192
-00001180: 310a 766f 6964 2053 6861 7271 6974 3a3a  1.void Sharqit::
-00001190: 5143 6972 633a 3a73 6176 6528 7f73 6176  QCirc::save(.sav
-000011a0: 6501 382c 3939 0a76 6f69 6420 5368 6172  e.8,99.void Shar
-000011b0: 7169 743a 3a51 4369 7263 3a3a 6c6f 6164  qit::QCirc::load
-000011c0: 287f 6c6f 6164 0132 302c 3331 360a 7374  (.load.20,316.st
-000011d0: 643a 3a6d 6170 3c73 7464 3a3a 7374 7269  d::map<std::stri
-000011e0: 6e67 2c20 7569 6e74 3332 5f74 3e20 5368  ng, uint32_t> Sh
-000011f0: 6172 7169 743a 3a51 4369 7263 3a3a 7374  arqit::QCirc::st
-00001200: 6174 7328 7f73 7461 7473 0136 372c 3135  ats(.stats.67,15
-00001210: 3832 0a76 6f69 6420 5368 6172 7169 743a  82.void Sharqit:
-00001220: 3a51 4369 7263 3a3a 7072 696e 745f 7374  :QCirc::print_st
-00001230: 6174 7328 7f70 7269 6e74 5f73 7461 7473  ats(.print_stats
-00001240: 0138 352c 3230 3738 0a75 696e 7433 325f  .85,2078.uint32_
-00001250: 7420 5368 6172 7169 743a 3a51 4369 7263  t Sharqit::QCirc
-00001260: 3a3a 6964 5f63 6f75 6e74 287f 6964 5f63  ::id_count(.id_c
-00001270: 6f75 6e74 0131 3031 2c32 3837 320a 7569  ount.101,2872.ui
-00001280: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
-00001290: 5143 6972 633a 3a78 5f63 6f75 6e74 287f  QCirc::x_count(.
-000012a0: 785f 636f 756e 7401 3130 382c 3330 3132  x_count.108,3012
-000012b0: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
-000012c0: 743a 3a51 4369 7263 3a3a 7a5f 636f 756e  t::QCirc::z_coun
-000012d0: 7428 7f7a 5f63 6f75 6e74 0131 3135 2c33  t(.z_count.115,3
-000012e0: 3135 300a 7569 6e74 3332 5f74 2053 6861  150.uint32_t Sha
-000012f0: 7271 6974 3a3a 5143 6972 633a 3a68 5f63  rqit::QCirc::h_c
-00001300: 6f75 6e74 287f 685f 636f 756e 7401 3132  ount(.h_count.12
-00001310: 322c 3332 3838 0a75 696e 7433 325f 7420  2,3288.uint32_t 
-00001320: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
-00001330: 735f 636f 756e 7428 7f73 5f63 6f75 6e74  s_count(.s_count
-00001340: 0131 3239 2c33 3432 360a 7569 6e74 3332  .129,3426.uint32
-00001350: 5f74 2053 6861 7271 6974 3a3a 5143 6972  _t Sharqit::QCir
-00001360: 633a 3a74 5f63 6f75 6e74 287f 745f 636f  c::t_count(.t_co
-00001370: 756e 7401 3133 362c 3335 3634 0a75 696e  unt.136,3564.uin
-00001380: 7433 325f 7420 5368 6172 7169 743a 3a51  t32_t Sharqit::Q
-00001390: 4369 7263 3a3a 727a 5f63 6f75 6e74 287f  Circ::rz_count(.
-000013a0: 727a 5f63 6f75 6e74 0131 3433 2c33 3730  rz_count.143,370
-000013b0: 320a 7569 6e74 3332 5f74 2053 6861 7271  2.uint32_t Sharq
-000013c0: 6974 3a3a 5143 6972 633a 3a63 785f 636f  it::QCirc::cx_co
-000013d0: 756e 7428 7f63 785f 636f 756e 7401 3135  unt(.cx_count.15
-000013e0: 302c 3338 3432 0a75 696e 7433 325f 7420  0,3842.uint32_t 
-000013f0: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
-00001400: 637a 5f63 6f75 6e74 287f 637a 5f63 6f75  cz_count(.cz_cou
-00001410: 6e74 0131 3537 2c33 3938 320a 7569 6e74  nt.157,3982.uint
-00001420: 3332 5f74 2053 6861 7271 6974 3a3a 5143  32_t Sharqit::QC
-00001430: 6972 633a 3a64 6570 7468 287f 6465 7074  irc::depth(.dept
-00001440: 6801 3136 342c 3431 3232 0a73 7464 3a3a  h.164,4122.std::
-00001450: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
-00001460: 5143 6972 633a 3a74 6f5f 7374 7269 6e67  QCirc::to_string
-00001470: 287f 746f 5f73 7472 696e 6701 3138 382c  (.to_string.188,
-00001480: 3436 3334 0a53 6861 7271 6974 3a3a 5143  4634.Sharqit::QC
-00001490: 6972 6326 2053 6861 7271 6974 3a3a 5143  irc& Sharqit::QC
-000014a0: 6972 633a 3a61 6464 5f71 6761 7465 287f  irc::add_qgate(.
-000014b0: 6164 645f 7167 6174 6501 3337 342c 3130  add_qgate.374,10
-000014c0: 3531 360a 5368 6172 7169 743a 3a51 4369  516.Sharqit::QCi
-000014d0: 7263 2620 5368 6172 7169 743a 3a51 4369  rc& Sharqit::QCi
-000014e0: 7263 3a3a 6164 645f 7167 6174 6528 7f61  rc::add_qgate(.a
-000014f0: 6464 5f71 6761 7465 0133 3834 2c31 3037  dd_qgate.384,107
-00001500: 3239 0a53 6861 7271 6974 3a3a 5143 6972  29.Sharqit::QCir
+00001170: 0a0c 0a71 6369 7263 2e63 7070 2c32 3137  ...qcirc.cpp,217
+00001180: 360a 2364 6566 696e 6520 4445 4255 477f  6.#define DEBUG.
+00001190: 382c 3939 0a76 6f69 6420 5368 6172 7169  8,99.void Sharqi
+000011a0: 743a 3a51 4369 7263 3a3a 7361 7665 287f  t::QCirc::save(.
+000011b0: 7361 7665 0131 302c 3131 340a 766f 6964  save.10,114.void
+000011c0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+000011d0: 3a6c 6f61 6428 7f6c 6f61 6401 3232 2c33  :load(.load.22,3
+000011e0: 3331 0a73 7464 3a3a 6d61 703c 7374 643a  31.std::map<std:
+000011f0: 3a73 7472 696e 672c 2075 696e 7433 325f  :string, uint32_
+00001200: 743e 2053 6861 7271 6974 3a3a 5143 6972  t> Sharqit::QCir
+00001210: 633a 3a73 7461 7473 287f 7374 6174 7301  c::stats(.stats.
+00001220: 3432 2c37 3536 0a76 6f69 6420 5368 6172  42,756.void Shar
+00001230: 7169 743a 3a51 4369 7263 3a3a 7072 696e  qit::QCirc::prin
+00001240: 745f 7374 6174 7328 7f70 7269 6e74 5f73  t_stats(.print_s
+00001250: 7461 7473 0136 322c 3133 3336 0a75 696e  tats.62,1336.uin
+00001260: 7433 325f 7420 5368 6172 7169 743a 3a51  t32_t Sharqit::Q
+00001270: 4369 7263 3a3a 6964 5f63 6f75 6e74 287f  Circ::id_count(.
+00001280: 6964 5f63 6f75 6e74 0137 382c 3231 3330  id_count.78,2130
+00001290: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+000012a0: 743a 3a51 4369 7263 3a3a 785f 636f 756e  t::QCirc::x_coun
+000012b0: 7428 7f78 5f63 6f75 6e74 0138 352c 3232  t(.x_count.85,22
+000012c0: 3730 0a75 696e 7433 325f 7420 5368 6172  70.uint32_t Shar
+000012d0: 7169 743a 3a51 4369 7263 3a3a 7a5f 636f  qit::QCirc::z_co
+000012e0: 756e 7428 7f7a 5f63 6f75 6e74 0139 322c  unt(.z_count.92,
+000012f0: 3234 3038 0a75 696e 7433 325f 7420 5368  2408.uint32_t Sh
+00001300: 6172 7169 743a 3a51 4369 7263 3a3a 685f  arqit::QCirc::h_
+00001310: 636f 756e 7428 7f68 5f63 6f75 6e74 0139  count(.h_count.9
+00001320: 392c 3235 3436 0a75 696e 7433 325f 7420  9,2546.uint32_t 
+00001330: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00001340: 735f 636f 756e 7428 7f73 5f63 6f75 6e74  s_count(.s_count
+00001350: 0131 3036 2c32 3638 340a 7569 6e74 3332  .106,2684.uint32
+00001360: 5f74 2053 6861 7271 6974 3a3a 5143 6972  _t Sharqit::QCir
+00001370: 633a 3a74 5f63 6f75 6e74 287f 745f 636f  c::t_count(.t_co
+00001380: 756e 7401 3131 332c 3238 3232 0a75 696e  unt.113,2822.uin
+00001390: 7433 325f 7420 5368 6172 7169 743a 3a51  t32_t Sharqit::Q
+000013a0: 4369 7263 3a3a 727a 5f63 6f75 6e74 287f  Circ::rz_count(.
+000013b0: 727a 5f63 6f75 6e74 0131 3230 2c32 3936  rz_count.120,296
+000013c0: 300a 7569 6e74 3332 5f74 2053 6861 7271  0.uint32_t Sharq
+000013d0: 6974 3a3a 5143 6972 633a 3a63 785f 636f  it::QCirc::cx_co
+000013e0: 756e 7428 7f63 785f 636f 756e 7401 3132  unt(.cx_count.12
+000013f0: 372c 3331 3030 0a75 696e 7433 325f 7420  7,3100.uint32_t 
+00001400: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00001410: 637a 5f63 6f75 6e74 287f 637a 5f63 6f75  cz_count(.cz_cou
+00001420: 6e74 0131 3334 2c33 3234 300a 7569 6e74  nt.134,3240.uint
+00001430: 3332 5f74 2053 6861 7271 6974 3a3a 5143  32_t Sharqit::QC
+00001440: 6972 633a 3a63 6378 5f63 6f75 6e74 287f  irc::ccx_count(.
+00001450: 6363 785f 636f 756e 7401 3134 312c 3333  ccx_count.141,33
+00001460: 3830 0a75 696e 7433 325f 7420 5368 6172  80.uint32_t Shar
+00001470: 7169 743a 3a51 4369 7263 3a3a 6363 7a5f  qit::QCirc::ccz_
+00001480: 636f 756e 7428 7f63 637a 5f63 6f75 6e74  count(.ccz_count
+00001490: 0131 3438 2c33 3532 320a 7569 6e74 3332  .148,3522.uint32
+000014a0: 5f74 2053 6861 7271 6974 3a3a 5143 6972  _t Sharqit::QCir
+000014b0: 633a 3a64 6570 7468 287f 6465 7074 6801  c::depth(.depth.
+000014c0: 3135 352c 3336 3634 0a73 7464 3a3a 7374  155,3664.std::st
+000014d0: 7269 6e67 2053 6861 7271 6974 3a3a 5143  ring Sharqit::QC
+000014e0: 6972 633a 3a74 6f5f 7374 7269 6e67 287f  irc::to_string(.
+000014f0: 746f 5f73 7472 696e 6701 3137 392c 3431  to_string.179,41
+00001500: 3736 0a53 6861 7271 6974 3a3a 5143 6972  76.Sharqit::QCir
 00001510: 6326 2053 6861 7271 6974 3a3a 5143 6972  c& Sharqit::QCir
-00001520: 633a 3a61 6464 5f71 6369 7263 287f 6164  c::add_qcirc(.ad
-00001530: 645f 7163 6972 6301 3339 362c 3131 3033  d_qcirc.396,1103
-00001540: 380a 5368 6172 7169 743a 3a51 4369 7263  8.Sharqit::QCirc
-00001550: 2620 5368 6172 7169 743a 3a51 4369 7263  & Sharqit::QCirc
-00001560: 3a3a 6164 645f 7261 6e64 6f6d 287f 6164  ::add_random(.ad
-00001570: 645f 7261 6e64 6f6d 0134 3034 2c31 3131  d_random.404,111
-00001580: 3834 0a53 6861 7271 6974 3a3a 5143 6972  84.Sharqit::QCir
-00001590: 6326 2053 6861 7271 6974 3a3a 5143 6972  c& Sharqit::QCir
-000015a0: 633a 3a61 6464 5f72 616e 646f 6d5f 7374  c::add_random_st
-000015b0: 7228 7f61 6464 5f72 616e 646f 6d5f 7374  r(.add_random_st
-000015c0: 7201 3437 362c 3133 3631 390a 5368 6172  r.476,13619.Shar
-000015d0: 7169 743a 3a51 4369 7263 2053 6861 7271  qit::QCirc Sharq
-000015e0: 6974 3a3a 5143 6972 633a 3a72 6576 6572  it::QCirc::rever
-000015f0: 7365 287f 7265 7665 7273 6501 3439 302c  se(.reverse.490,
-00001600: 3134 3136 310a 5368 6172 7169 743a 3a51  14161.Sharqit::Q
-00001610: 4369 7263 2053 6861 7271 6974 3a3a 5143  Circ Sharqit::QC
-00001620: 6972 633a 3a69 6e76 6572 7365 287f 696e  irc::inverse(.in
-00001630: 7665 7273 6501 3530 302c 3134 3338 310a  verse.500,14381.
-00001640: 626f 6f6c 2053 6861 7271 6974 3a3a 5143  bool Sharqit::QC
-00001650: 6972 633a 3a69 735f 6964 656e 7469 6361  irc::is_identica
-00001660: 6c28 7f69 735f 6964 656e 7469 6361 6c01  l(.is_identical.
-00001670: 3531 302c 3134 3631 310a 626f 6f6c 2053  510,14611.bool S
-00001680: 6861 7271 6974 3a3a 5143 6972 633a 3a69  harqit::QCirc::i
-00001690: 735f 6571 7561 6c28 7f69 735f 6571 7561  s_equal(.is_equa
-000016a0: 6c01 3531 392c 3134 3835 340a 766f 6964  l.519,14854.void
-000016b0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
-000016c0: 3a74 6f5f 646f 745f 6669 6c65 287f 746f  :to_dot_file(.to
-000016d0: 5f64 6f74 5f66 696c 6501 3536 322c 3136  _dot_file.562,16
-000016e0: 3231 350a 766f 6964 2053 6861 7271 6974  215.void Sharqit
-000016f0: 3a3a 5143 6972 633a 3a74 6f5f 7376 675f  ::QCirc::to_svg_
-00001700: 6669 6c65 287f 746f 5f73 7667 5f66 696c  file(.to_svg_fil
-00001710: 6501 3736 392c 3233 3233 390a 5368 6172  e.769,23239.Shar
-00001720: 7169 743a 3a5a 5844 6961 6772 616d 2053  qit::ZXDiagram S
-00001730: 6861 7271 6974 3a3a 5143 6972 633a 3a74  harqit::QCirc::t
-00001740: 6f5f 7a78 6469 6167 7261 6d28 7f74 6f5f  o_zxdiagram(.to_
-00001750: 7a78 6469 6167 7261 6d01 3738 312c 3233  zxdiagram.781,23
-00001760: 3730 350a 5368 6172 7169 743a 3a4c 696e  705.Sharqit::Lin
-00001770: 6561 724d 6170 2053 6861 7271 6974 3a3a  earMap Sharqit::
-00001780: 5143 6972 633a 3a74 6f5f 6c69 6e65 6172  QCirc::to_linear
-00001790: 6d61 7028 7f74 6f5f 6c69 6e65 6172 6d61  map(.to_linearma
-000017a0: 7001 3739 392c 3234 3138 350a 5368 6172  p.799,24185.Shar
-000017b0: 7169 743a 3a44 4147 4369 7263 2053 6861  qit::DAGCirc Sha
-000017c0: 7271 6974 3a3a 5143 6972 633a 3a74 6f5f  rqit::QCirc::to_
-000017d0: 6461 6763 6972 6328 7f74 6f5f 6461 6763  dagcirc(.to_dagc
-000017e0: 6972 6301 3830 382c 3234 3338 320a 766f  irc.808,24382.vo
-000017f0: 6964 2053 6861 7271 6974 3a3a 5143 6972  id Sharqit::QCir
-00001800: 633a 3a63 7a5f 746f 5f63 7828 7f63 7a5f  c::cz_to_cx(.cz_
-00001810: 746f 5f63 7801 3831 352c 3234 3534 340a  to_cx.815,24544.
-00001820: 766f 6964 2053 6861 7271 6974 3a3a 5143  void Sharqit::QC
-00001830: 6972 633a 3a64 6563 6f6d 705f 746f 6628  irc::decomp_tof(
-00001840: 7f64 6563 6f6d 705f 746f 6601 3833 332c  .decomp_tof.833,
-00001850: 3235 3131 390a 626f 6f6c 2053 6861 7271  25119.bool Sharq
-00001860: 6974 3a3a 5143 6972 633a 3a69 6e63 6c75  it::QCirc::inclu
-00001870: 6465 5f74 6f66 287f 696e 636c 7564 655f  de_tof(.include_
-00001880: 746f 6601 3837 332c 3236 3031 380a 766f  tof.873,26018.vo
-00001890: 6964 2053 6861 7271 6974 3a3a 5143 6972  id Sharqit::QCir
-000018a0: 633a 3a72 656d 6f76 655f 6964 287f 7265  c::remove_id(.re
-000018b0: 6d6f 7665 5f69 6401 3838 322c 3236 3230  move_id.882,2620
-000018c0: 340a 766f 6964 2020 5368 6172 7169 743a  4.void  Sharqit:
-000018d0: 3a51 4369 7263 3a3a 7265 706c 6163 655f  :QCirc::replace_
-000018e0: 7769 7468 5f72 7a28 7f72 6570 6c61 6365  with_rz(.replace
-000018f0: 5f77 6974 685f 727a 0138 3936 2c32 3637  _with_rz.896,267
-00001900: 3531 0a0c 0a70 6861 7365 2e63 7070 2c39  51...phase.cpp,9
-00001910: 300a 5368 6172 7169 743a 3a50 6861 7365  0.Sharqit::Phase
-00001920: 3a3a 5068 6173 6528 7f50 6861 7365 0138  ::Phase(.Phase.8
-00001930: 2c39 300a 7374 643a 3a73 7472 696e 6720  ,90.std::string 
-00001940: 5368 6172 7169 743a 3a50 6861 7365 3a3a  Sharqit::Phase::
-00001950: 746f 5f73 7472 696e 6728 7f74 6f5f 7374  to_string(.to_st
-00001960: 7269 6e67 0133 312c 3734 340a 0c0a 6d65  ring.31,744...me
-00001970: 7267 655f 726f 7461 7469 6f6e 2e63 7070  rge_rotation.cpp
-00001980: 2c32 3039 0a62 6f6f 6c20 5368 6172 7169  ,209.bool Sharqi
-00001990: 743a 3a51 4369 7263 3a3a 6973 5f74 6572  t::QCirc::is_ter
-000019a0: 6d69 6e61 7469 6f6e 5f62 6f72 6465 7228  mination_border(
-000019b0: 7f69 735f 7465 726d 696e 6174 696f 6e5f  .is_termination_
-000019c0: 626f 7264 6572 0138 2c31 3438 0a76 6f69  border.8,148.voi
-000019d0: 6420 5368 6172 7169 743a 3a51 4369 7263  d Sharqit::QCirc
-000019e0: 3a3a 6d65 7267 655f 726f 7461 7469 6f6e  ::merge_rotation
-000019f0: 5f6f 6e65 5f74 696d 6528 7f6d 6572 6765  _one_time(.merge
-00001a00: 5f72 6f74 6174 696f 6e5f 6f6e 655f 7469  _rotation_one_ti
-00001a10: 6d65 0131 382c 3431 320a 766f 6964 2053  me.18,412.void S
-00001a20: 6861 7271 6974 3a3a 5143 6972 633a 3a6d  harqit::QCirc::m
-00001a30: 6572 6765 5f72 6f74 6174 696f 6e28 7f6d  erge_rotation(.m
-00001a40: 6572 6765 5f72 6f74 6174 696f 6e01 3832  erge_rotation.82
-00001a50: 2c32 3630 310a 0c0a 6269 6e61 7279 5f6d  ,2601...binary_m
-00001a60: 6174 7269 782e 682c 3833 370a 2364 6566  atrix.h,837.#def
-00001a70: 696e 6520 4249 4e41 5259 5f4d 4154 5249  ine BINARY_MATRI
-00001a80: 585f 487f 372c 3130 330a 2020 636c 6173  X_H.7,103.  clas
-00001a90: 7320 4269 6e61 7279 4d61 7472 6978 7f32  s BinaryMatrix.2
-00001aa0: 302c 3238 370a 2020 2020 7569 6e74 3332  0,287.    uint32
-00001ab0: 5f74 2072 6f77 5f6e 756d 5f3b 7f32 332c  _t row_num_;.23,
-00001ac0: 3332 330a 2020 2020 7569 6e74 3332 5f74  323.    uint32_t
-00001ad0: 2063 6f6c 5f6e 756d 5f3b 7f32 342c 3337   col_num_;.24,37
-00001ae0: 360a 2020 2020 7374 643a 3a76 6563 746f  6.    std::vecto
-00001af0: 723c 7374 643a 3a76 6563 746f 723c 7569  r<std::vector<ui
-00001b00: 6e74 385f 743e 3e20 656c 656d 656e 7473  nt8_t>> elements
-00001b10: 5f3b 7f32 352c 3433 320a 2020 2020 7374  _;.25,432.    st
-00001b20: 643a 3a76 6563 746f 723c 7569 6e74 3332  d::vector<uint32
-00001b30: 5f74 3e20 726f 775f 696e 6465 7865 735f  _t> row_indexes_
-00001b40: 3b7f 3236 2c35 3333 0a20 2020 2042 696e  ;.26,533.    Bin
-00001b50: 6172 794d 6174 7269 7828 7f33 342c 3836  aryMatrix(.34,86
-00001b60: 310a 2020 2020 4269 6e61 7279 4d61 7472  1.    BinaryMatr
-00001b70: 6978 287f 3433 2c31 3235 360a 2020 2020  ix(.43,1256.    
-00001b80: 4269 6e61 7279 4d61 7472 6978 287f 3534  BinaryMatrix(.54
-00001b90: 2c31 3631 350a 2020 2020 7569 6e74 3332  ,1615.    uint32
-00001ba0: 5f74 2072 6f77 5f6e 756d 287f 3537 2c31  _t row_num(.57,1
-00001bb0: 3739 390a 2020 2020 7569 6e74 3332 5f74  799.    uint32_t
-00001bc0: 2063 6f6c 5f6e 756d 287f 3539 2c31 3838   col_num(.59,188
-00001bd0: 300a 2020 2020 7374 643a 3a76 6563 746f  0.    std::vecto
-00001be0: 723c 7374 643a 3a76 6563 746f 723c 7569  r<std::vector<ui
-00001bf0: 6e74 385f 743e 3e20 656c 656d 656e 7473  nt8_t>> elements
-00001c00: 287f 3631 2c31 3936 320a 2020 2020 7374  (.61,1962.    st
-00001c10: 643a 3a76 6563 746f 723c 7569 6e74 3332  d::vector<uint32
-00001c20: 5f74 3e20 726f 775f 696e 6465 7865 7328  _t> row_indexes(
-00001c30: 7f36 332c 3230 3735 0a20 2020 2076 6f69  .63,2075.    voi
-00001c40: 6420 726f 775f 6e75 6d28 7f36 352c 3231  d row_num(.65,21
-00001c50: 3738 0a20 2020 2076 6f69 6420 636f 6c5f  78.    void col_
-00001c60: 6e75 6d28 7f36 372c 3232 3734 0a20 2020  num(.67,2274.   
-00001c70: 2076 6f69 6420 656c 656d 656e 7473 287f   void elements(.
-00001c80: 3639 2c32 3337 310a 2020 2020 766f 6964  69,2371.    void
-00001c90: 2072 6f77 5f69 6e64 6578 6573 287f 3731   row_indexes(.71
-00001ca0: 2c32 3530 310a 2020 2020 766f 6964 2073  ,2501.    void s
-00001cb0: 6574 5f69 6465 6e74 6974 7928 7f38 322c  et_identity(.82,
-00001cc0: 3239 3534 0a20 2020 2076 6f69 6420 7265  2954.    void re
-00001cd0: 7665 7273 655f 656c 656d 656e 7428 7f39  verse_element(.9
-00001ce0: 362c 3333 3536 0a20 2020 2075 696e 7433  6,3356.    uint3
-00001cf0: 325f 7420 786f 725f 726f 7773 287f 3130  2_t xor_rows(.10
-00001d00: 382c 3338 3339 0a20 2020 2076 6f69 6420  8,3839.    void 
-00001d10: 7377 6170 5f72 6f77 7328 7f31 3235 2c34  swap_rows(.125,4
-00001d20: 3334 310a 2020 2020 766f 6964 2073 7761  341.    void swa
-00001d30: 705f 636f 6c73 287f 3134 302c 3437 3930  p_cols(.140,4790
-00001d40: 0a20 2020 2062 6f6f 6c20 6665 6173 6962  .    bool feasib
-00001d50: 6c65 287f 3135 332c 3531 3833 0a20 2020  le(.153,5183.   
-00001d60: 2073 7464 3a3a 7665 6374 6f72 3c7f 7374   std::vector<.st
-00001d70: 643a 3a76 6563 746f 7201 3137 342c 3537  d::vector.174,57
-00001d80: 3430 0a20 2020 2066 7269 656e 6420 7374  40.    friend st
-00001d90: 643a 3a6f 7374 7265 616d 2620 6f70 6572  d::ostream& oper
-00001da0: 6174 6f72 3c3c 287f 3137 352c 3538 3333  ator<<(.175,5833
-00001db0: 0a0c 0a75 7469 6c2e 682c 3436 0a23 6465  ...util.h,46.#de
-00001dc0: 6669 6e65 2055 5449 4c5f 487f 372c 3834  fine UTIL_H.7,84
-00001dd0: 0a6e 616d 6573 7061 6365 2053 6861 7271  .namespace Sharq
-00001de0: 6974 207f 3133 2c31 3536 0a0c 0a71 6761  it .13,156...qga
-00001df0: 7465 2e63 7070 2c36 3738 0a53 6861 7271  te.cpp,678.Sharq
-00001e00: 6974 3a3a 5147 6174 653a 3a51 4761 7465  it::QGate::QGate
-00001e10: 287f 5147 6174 6501 382c 3930 0a53 6861  (.QGate.8,90.Sha
-00001e20: 7271 6974 3a3a 5147 6174 653a 3a51 4761  rqit::QGate::QGa
-00001e30: 7465 287f 5147 6174 6501 3634 2c31 3631  te(.QGate.64,161
-00001e40: 350a 7374 643a 3a76 6563 746f 723c 7374  5.std::vector<st
-00001e50: 643a 3a76 6563 746f 723c 7374 643a 3a63  d::vector<std::c
-00001e60: 6f6d 706c 6578 3c64 6f75 626c 653e 3e3e  omplex<double>>>
-00001e70: 2053 6861 7271 6974 3a3a 5147 6174 653a   Sharqit::QGate:
-00001e80: 3a6b 696e 645f 746f 5f6f 7028 7f6b 696e  :kind_to_op(.kin
-00001e90: 645f 746f 5f6f 7001 3832 2c32 3134 350a  d_to_op.82,2145.
-00001ea0: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
-00001eb0: 7169 743a 3a51 4761 7465 3a3a 6e61 6d65  qit::QGate::name
-00001ec0: 287f 6e61 6d65 0131 3638 2c34 3631 380a  (.name.168,4618.
-00001ed0: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
-00001ee0: 7169 743a 3a51 4761 7465 3a3a 746f 5f73  qit::QGate::to_s
-00001ef0: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
-00001f00: 0131 3737 2c34 3933 340a 7374 643a 3a74  .177,4934.std::t
-00001f10: 7570 6c65 3c53 6861 7271 6974 3a3a 5147  uple<Sharqit::QG
-00001f20: 6174 654b 696e 642c 2053 6861 7271 6974  ateKind, Sharqit
-00001f30: 3a3a 5068 6173 653e 2053 6861 7271 6974  ::Phase> Sharqit
-00001f40: 3a3a 5147 6174 653a 3a6b 696e 645f 7068  ::QGate::kind_ph
-00001f50: 6173 6528 7f6b 696e 645f 7068 6173 6501  ase(.kind_phase.
-00001f60: 3139 362c 3532 3335 0a53 6861 7271 6974  196,5235.Sharqit
-00001f70: 3a3a 5147 6174 6520 5368 6172 7169 743a  ::QGate Sharqit:
-00001f80: 3a51 4761 7465 3a3a 696e 7665 7273 6528  :QGate::inverse(
-00001f90: 7f69 6e76 6572 7365 0132 3733 2c37 3039  .inverse.273,709
-00001fa0: 390a 626f 6f6c 2053 6861 7271 6974 3a3a  9.bool Sharqit::
-00001fb0: 5147 6174 653a 3a69 735f 6964 656e 7469  QGate::is_identi
-00001fc0: 6361 6c28 7f69 735f 6964 656e 7469 6361  cal(.is_identica
-00001fd0: 6c01 3335 342c 3936 3334 0a62 6f6f 6c20  l.354,9634.bool 
-00001fe0: 5368 6172 7169 743a 3a51 4761 7465 3a3a  Sharqit::QGate::
-00001ff0: 6f76 6572 6c61 7028 7f6f 7665 726c 6170  overlap(.overlap
-00002000: 0133 3639 2c31 3031 3933 0a62 6f6f 6c20  .369,10193.bool 
-00002010: 5368 6172 7169 743a 3a51 4761 7465 3a3a  Sharqit::QGate::
-00002020: 6d65 7267 6561 626c 6528 7f6d 6572 6765  mergeable(.merge
-00002030: 6162 6c65 0133 3833 2c31 3034 3434 0a62  able.383,10444.b
-00002040: 6f6f 6c20 5368 6172 7169 743a 3a51 4761  ool Sharqit::QGa
-00002050: 7465 3a3a 636f 6d6d 7574 6162 6c65 287f  te::commutable(.
-00002060: 636f 6d6d 7574 6162 6c65 0134 3030 2c31  commutable.400,1
-00002070: 3131 3831 0a76 6f69 6420 5368 6172 7169  1181.void Sharqi
-00002080: 743a 3a51 4761 7465 3a3a 6d65 7267 6528  t::QGate::merge(
-00002090: 7f6d 6572 6765 0134 3434 2c31 3330 3836  .merge.444,13086
-000020a0: 0a0c 0a65 7874 7261 6374 5f71 6369 7263  ...extract_qcirc
-000020b0: 2e63 7070 2c34 3635 0a76 6f69 6420 5368  .cpp,465.void Sh
-000020c0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-000020d0: 3a3a 7065 726d 7574 6174 696f 6e5f 6173  ::permutation_as
-000020e0: 5f73 7761 7028 7f70 6572 6d75 7461 7469  _swap(.permutati
-000020f0: 6f6e 5f61 735f 7377 6170 0138 2c31 3531  on_as_swap.8,151
-00002100: 0a73 7464 3a3a 7665 6374 6f72 3c73 7464  .std::vector<std
-00002110: 3a3a 7061 6972 3c75 696e 7433 325f 742c  ::pair<uint32_t,
-00002120: 2075 696e 7433 325f 743e 3e20 5368 6172   uint32_t>> Shar
-00002130: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
-00002140: 6578 7472 6163 745f 3271 5f63 6f6e 6e65  extract_2q_conne
-00002150: 6374 7328 7f65 7874 7261 6374 5f32 715f  cts(.extract_2q_
-00002160: 636f 6e6e 6563 7473 0132 382c 3632 370a  connects.28,627.
-00002170: 626f 6f6c 2053 6861 7271 6974 3a3a 5a58  bool Sharqit::ZX
-00002180: 4469 6167 7261 6d3a 3a75 7064 6174 655f  Diagram::update_
-00002190: 6672 6f6e 7469 6572 287f 7570 6461 7465  frontier(.update
-000021a0: 5f66 726f 6e74 6965 7201 3836 2c32 3238  _frontier.86,228
-000021b0: 310a 626f 6f6c 2053 6861 7271 6974 3a3a  1.bool Sharqit::
-000021c0: 5a58 4469 6167 7261 6d3a 3a75 7064 6174  ZXDiagram::updat
-000021d0: 655f 6672 6f6e 7469 6572 5f70 6728 7f75  e_frontier_pg(.u
-000021e0: 7064 6174 655f 6672 6f6e 7469 6572 5f70  pdate_frontier_p
-000021f0: 6701 3232 352c 3634 3038 0a76 6f69 6420  g.225,6408.void 
-00002200: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00002210: 616d 3a3a 7072 6f63 6573 735f 6672 6f6e  am::process_fron
-00002220: 7469 6572 287f 7072 6f63 6573 735f 6672  tier(.process_fr
-00002230: 6f6e 7469 6572 0133 3035 2c39 3030 380a  ontier.305,9008.
-00002240: 5368 6172 7169 743a 3a51 4369 7263 2053  Sharqit::QCirc S
-00002250: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-00002260: 6d3a 3a65 7874 7261 6374 5f71 6369 7263  m::extract_qcirc
-00002270: 287f 6578 7472 6163 745f 7163 6972 6301  (.extract_qcirc.
-00002280: 3335 332c 3130 3539 350a 0c0a 6461 672e  353,10595...dag.
-00002290: 682c 3138 3933 0a23 6465 6669 6e65 2044  h,1893.#define D
-000022a0: 4147 5f48 7f37 2c31 3337 0a20 2065 6e75  AG_H.7,137.  enu
-000022b0: 6d20 4441 474e 6f64 654b 696e 6420 7f32  m DAGNodeKind .2
-000022c0: 322c 3332 390a 0909 2020 2020 4f70 4e6f  2,329...    OpNo
-000022d0: 6465 2c7f 3233 2c33 3530 0a09 0920 2020  de,.23,350...   
-000022e0: 2049 6e4e 6f64 652c 7f32 342c 3430 310a   InNode,.24,401.
-000022f0: 0909 2020 2020 4f75 744e 6f64 6520 7f32  ..    OutNode .2
-00002300: 352c 3433 310a 2020 656e 756d 2044 4147  5,431.  enum DAG
-00002310: 4564 6765 4b69 6e64 207f 3238 2c34 3933  EdgeKind .28,493
-00002320: 0a09 0920 2020 2046 6f72 7761 7264 2c7f  ...    Forward,.
-00002330: 3239 2c35 3134 0a09 0920 2020 2042 6163  29,514...    Bac
-00002340: 6b77 6172 6420 7f33 302c 3535 320a 2020  kward .30,552.  
-00002350: 636c 6173 7320 4441 474e 6f64 657f 3339  class DAGNode.39
-00002360: 2c37 3133 0a20 2020 2044 4147 4e6f 6465  ,713.    DAGNode
-00002370: 4b69 6e64 206b 696e 645f 3b7f 3432 2c37  Kind kind_;.42,7
-00002380: 3434 0a20 2020 2051 4761 7465 2071 6761  44.    QGate qga
-00002390: 7465 5f3b 7f34 332c 3738 390a 2020 2020  te_;.43,789.    
-000023a0: 4441 474e 6f64 6528 7f35 302c 3130 3031  DAGNode(.50,1001
-000023b0: 0a20 2020 2044 4147 4e6f 6465 287f 3536  .    DAGNode(.56
-000023c0: 2c31 3232 360a 2020 2020 4441 474e 6f64  ,1226.    DAGNod
-000023d0: 654b 696e 6420 6b69 6e64 287f 3538 2c31  eKind kind(.58,1
-000023e0: 3333 310a 2020 2020 5147 6174 6520 7167  331.    QGate qg
-000023f0: 6174 6528 7f36 302c 3134 3037 0a20 2020  ate(.60,1407.   
-00002400: 2076 6f69 6420 6b69 6e64 287f 3632 2c31   void kind(.62,1
-00002410: 3437 380a 2020 2020 766f 6964 2071 6761  478.    void qga
-00002420: 7465 287f 3634 2c31 3536 330a 2020 2020  te(.64,1563.    
-00002430: 7569 6e74 3332 5f74 2071 7562 6974 5f6e  uint32_t qubit_n
-00002440: 756d 287f 3734 2c31 3839 340a 2020 2020  um(.74,1894.    
-00002450: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
-00002460: 3332 5f74 3e20 7169 6428 7f37 392c 3231  32_t> qid(.79,21
-00002470: 3038 0a20 2020 2062 6f6f 6c20 6973 5f69  08.    bool is_i
-00002480: 6e6e 6f64 6528 7f38 342c 3233 3032 0a20  nnode(.84,2302. 
-00002490: 2020 2062 6f6f 6c20 6973 5f6f 7574 6e6f     bool is_outno
-000024a0: 6465 287f 3839 2c32 3531 380a 2020 2020  de(.89,2518.    
-000024b0: 626f 6f6c 2069 735f 6f70 6e6f 6465 287f  bool is_opnode(.
-000024c0: 3934 2c32 3737 320a 2020 2020 626f 6f6c  94,2772.    bool
-000024d0: 2069 735f 6964 656e 7469 7479 287f 3939   is_identity(.99
-000024e0: 2c33 3030 380a 2020 2020 626f 6f6c 2069  ,3008.    bool i
-000024f0: 735f 6861 6461 6d61 7264 287f 3130 352c  s_hadamard(.105,
-00002500: 3332 3832 0a20 2020 2062 6f6f 6c20 6973  3282.    bool is
-00002510: 5f72 6f74 6174 696f 6e28 7f31 3130 2c33  _rotation(.110,3
-00002520: 3438 330a 2020 2020 626f 6f6c 2069 735f  483.    bool is_
-00002530: 636e 6f74 287f 3131 352c 3336 3737 0a20  cnot(.115,3677. 
-00002540: 2020 2062 6f6f 6c20 6973 5f69 6e63 6c75     bool is_inclu
-00002550: 6465 6428 7f31 3231 2c33 3935 320a 2020  ded(.121,3952.  
-00002560: 2020 626f 6f6c 206d 6572 6765 6162 6c65    bool mergeable
-00002570: 287f 3133 312c 3432 3938 0a20 2020 2062  (.131,4298.    b
-00002580: 6f6f 6c20 636f 6d6d 7574 6162 6c65 287f  ool commutable(.
-00002590: 3133 372c 3436 3036 0a20 2020 2076 6f69  137,4606.    voi
-000025a0: 6420 6d65 7267 6528 7f31 3432 2c34 3832  d merge(.142,482
-000025b0: 340a 2020 636c 6173 7320 4441 4745 6467  4.  class DAGEdg
-000025c0: 657f 3135 302c 3439 3938 0a20 2020 2044  e.150,4998.    D
-000025d0: 4147 4564 6765 4b69 6e64 206b 696e 645f  AGEdgeKind kind_
-000025e0: 3b7f 3135 332c 3530 3239 0a20 2020 2075  ;.153,5029.    u
-000025f0: 696e 7433 325f 7420 715f 3b7f 3135 342c  int32_t q_;.154,
-00002600: 3531 3032 0a20 2020 2075 696e 7433 325f  5102.    uint32_
-00002610: 7420 746f 5f3b 7f31 3535 2c35 3135 330a  t to_;.155,5153.
-00002620: 2020 2020 4441 4745 6467 6528 7f31 3633      DAGEdge(.163
-00002630: 2c35 3431 340a 2020 2020 4441 4745 6467  ,5414.    DAGEdg
-00002640: 6528 7f31 3639 2c35 3636 360a 2020 2020  e(.169,5666.    
-00002650: 4441 4745 6467 654b 696e 6420 6b69 6e64  DAGEdgeKind kind
-00002660: 287f 3137 312c 3537 3738 0a20 2020 2075  (.171,5778.    u
-00002670: 696e 7433 325f 7420 7128 7f31 3733 2c35  int32_t q(.173,5
-00002680: 3835 300a 2020 2020 7569 6e74 3332 5f74  850.    uint32_t
-00002690: 2074 6f28 7f31 3735 2c35 3931 340a 2020   to(.175,5914.  
-000026a0: 2020 766f 6964 206b 696e 6428 7f31 3737    void kind(.177
-000026b0: 2c35 3938 320a 2020 2020 766f 6964 2071  ,5982.    void q
-000026c0: 287f 3137 392c 3630 3537 0a20 2020 2076  (.179,6057.    v
-000026d0: 6f69 6420 746f 287f 3138 312c 3631 3138  oid to(.181,6118
-000026e0: 0a20 2020 2062 6f6f 6c20 6973 5f66 6f72  .    bool is_for
-000026f0: 7761 7264 287f 3139 312c 3634 3039 0a20  ward(.191,6409. 
-00002700: 2020 2062 6f6f 6c20 6973 5f62 6163 6b77     bool is_backw
-00002710: 6172 6428 7f31 3936 2c36 3632 370a 2020  ard(.196,6627.  
-00002720: 636c 6173 7320 4441 4743 6972 637f 3230  class DAGCirc.20
-00002730: 352c 3638 3434 0a20 2020 2075 696e 7433  5,6844.    uint3
-00002740: 325f 7420 7175 6269 745f 6e75 6d5f 3b7f  2_t qubit_num_;.
-00002750: 3230 382c 3638 3735 0a20 2020 2073 7464  208,6875.    std
-00002760: 3a3a 7665 6374 6f72 3c44 4147 4e6f 6465  ::vector<DAGNode
-00002770: 3e20 6e6f 6465 735f 3b7f 3230 392c 3639  > nodes_;.209,69
-00002780: 3232 0a20 2020 2073 7464 3a3a 7665 6374  22.    std::vect
-00002790: 6f72 3c75 696e 7433 325f 743e 2069 6e70  or<uint32_t> inp
-000027a0: 7574 735f 3b7f 3231 302c 3639 3930 0a20  uts_;.210,6990. 
-000027b0: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
-000027c0: 696e 7433 325f 743e 206f 7574 7075 7473  int32_t> outputs
-000027d0: 5f3b 7f32 3131 2c37 3036 330a 2020 2020  _;.211,7063.    
-000027e0: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
-000027f0: 3a76 6563 746f 723c 4441 4745 6467 653e  :vector<DAGEdge>
-00002800: 3e20 6164 6a5f 6d61 745f 3b7f 3231 322c  > adj_mat_;.212,
-00002810: 3731 3338 0a20 2020 2044 4147 4369 7263  7138.    DAGCirc
-00002820: 287f 3236 362c 3935 3435 0a20 2020 2075  (.266,9545.    u
-00002830: 696e 7433 325f 7420 7175 6269 745f 6e75  int32_t qubit_nu
-00002840: 6d28 7f32 3730 2c39 3733 370a 2020 2020  m(.270,9737.    
-00002850: 7374 643a 3a76 6563 746f 723c 4441 474e  std::vector<DAGN
-00002860: 6f64 653e 206e 6f64 6573 287f 3237 322c  ode> nodes(.272,
-00002870: 3938 3230 0a20 2020 2073 7464 3a3a 7665  9820.    std::ve
-00002880: 6374 6f72 3c75 696e 7433 325f 743e 2069  ctor<uint32_t> i
-00002890: 6e70 7574 7328 7f32 3734 2c39 3930 380a  nputs(.274,9908.
-000028a0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-000028b0: 7569 6e74 3332 5f74 3e20 6f75 7470 7574  uint32_t> output
-000028c0: 7328 7f32 3736 2c31 3030 3030 0a20 2020  s(.276,10000.   
-000028d0: 2073 7464 3a3a 7665 6374 6f72 3c73 7464   std::vector<std
-000028e0: 3a3a 7665 6374 6f72 3c44 4147 4564 6765  ::vector<DAGEdge
-000028f0: 3e3e 2061 646a 5f6d 6174 287f 3237 382c  >> adj_mat(.278,
-00002900: 3130 3039 340a 2020 2020 766f 6964 2071  10094.    void q
-00002910: 7562 6974 5f6e 756d 287f 3238 302c 3130  ubit_num(.280,10
-00002920: 3230 320a 2020 2020 766f 6964 206e 6f64  202.    void nod
-00002930: 6573 287f 3238 322c 3130 3330 340a 2020  es(.282,10304.  
-00002940: 2020 766f 6964 2069 6e70 7574 7328 7f32    void inputs(.2
-00002950: 3834 2c31 3034 3034 0a20 2020 2076 6f69  84,10404.    voi
-00002960: 6420 6f75 7470 7574 7328 7f32 3836 2c31  d outputs(.286,1
-00002970: 3035 3130 0a20 2020 2076 6f69 6420 6164  0510.    void ad
-00002980: 6a5f 6d61 7428 7f32 3838 2c31 3036 3230  j_mat(.288,10620
-00002990: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
-000029a0: 3239 372c 3130 3931 390a 2020 2020 7569  297,10919.    ui
-000029b0: 6e74 3332 5f74 2067 6174 655f 636f 756e  nt32_t gate_coun
-000029c0: 7428 7f33 3031 2c31 3130 3138 0a20 2020  t(.301,11018.   
-000029d0: 2066 7269 656e 6420 7374 643a 3a6f 7374   friend std::ost
-000029e0: 7265 616d 2620 6f70 6572 6174 6f72 3c3c  ream& operator<<
-000029f0: 287f 3339 332c 3134 3830 320a 0c0a 7163  (.393,14802...qc
-00002a00: 6972 632e 682c 3138 3033 0a23 6465 6669  irc.h,1803.#defi
-00002a10: 6e65 2051 4349 5243 5f48 7f37 2c38 300a  ne QCIRC_H.7,80.
-00002a20: 2020 636c 6173 7320 5143 6972 637f 3334    class QCirc.34
-00002a30: 2c34 3932 0a20 2020 2075 696e 7433 325f  ,492.    uint32_
-00002a40: 7420 7175 6269 745f 6e75 6d5f 3b7f 3337  t qubit_num_;.37
-00002a50: 2c35 3231 0a20 2020 2073 7464 3a3a 7665  ,521.    std::ve
-00002a60: 6374 6f72 3c51 4761 7465 3e20 7167 6174  ctor<QGate> qgat
-00002a70: 6573 5f3b 7f33 382c 3536 380a 2020 2020  es_;.38,568.    
-00002a80: 5143 6972 6328 7f35 392c 3135 3530 0a20  QCirc(.59,1550. 
-00002a90: 2020 2051 4369 7263 287f 3634 2c31 3731     QCirc(.64,171
-00002aa0: 390a 2020 2020 5143 6972 6328 7f36 392c  9.    QCirc(.69,
-00002ab0: 3139 3037 0a20 2020 2075 696e 7433 325f  1907.    uint32_
-00002ac0: 7420 7175 6269 745f 6e75 6d28 7f37 312c  t qubit_num(.71,
-00002ad0: 3230 3331 0a20 2020 2075 696e 7433 325f  2031.    uint32_
-00002ae0: 7420 6765 745f 7175 6269 745f 6e75 6d28  t get_qubit_num(
-00002af0: 7f37 332c 3231 3138 0a20 2020 2073 7464  .73,2118.    std
-00002b00: 3a3a 7665 6374 6f72 3c51 4761 7465 3e20  ::vector<QGate> 
-00002b10: 7167 6174 6573 287f 3735 2c32 3230 360a  qgates(.75,2206.
-00002b20: 2020 2020 766f 6964 2071 7562 6974 5f6e      void qubit_n
-00002b30: 756d 287f 3737 2c32 3239 370a 2020 2020  um(.77,2297.    
-00002b40: 766f 6964 2071 6761 7465 7328 7f37 392c  void qgates(.79,
-00002b50: 3234 3030 0a20 2020 2075 696e 7433 325f  2400.    uint32_
-00002b60: 7420 7167 6174 655f 6e75 6d28 7f38 342c  t qgate_num(.84,
-00002b70: 3235 3735 0a20 2020 2076 6f69 6420 636c  2575.    void cl
-00002b80: 6561 7228 7f39 382c 3330 3238 0a20 2020  ear(.98,3028.   
-00002b90: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
-00002ba0: 6d61 7001 3130 332c 3331 3930 0a20 2020  map.103,3190.   
-00002bb0: 2075 696e 7433 325f 7420 6761 7465 5f63   uint32_t gate_c
-00002bc0: 6f75 6e74 287f 3130 382c 3333 3934 0a20  ount(.108,3394. 
-00002bd0: 2020 2075 696e 7433 325f 7420 7477 6f71     uint32_t twoq
-00002be0: 5f63 6f75 6e74 287f 3135 382c 3439 3636  _count(.158,4966
-00002bf0: 0a20 2020 2076 6f69 6420 7368 6f77 287f  .    void show(.
-00002c00: 3137 332c 3535 3031 0a20 2020 2076 6f69  173,5501.    voi
-00002c10: 6420 7072 696e 745f 7163 6972 6328 7f31  d print_qcirc(.1
-00002c20: 3737 2c35 3635 370a 2020 2020 5143 6972  77,5657.    QCir
-00002c30: 6326 2061 6464 5f71 6761 7465 287f 3230  c& add_qgate(.20
-00002c40: 312c 3637 3633 0a20 2020 2053 6861 7271  1,6763.    Sharq
-00002c50: 6974 3a3a 5147 6174 6520 6765 745f 7167  it::QGate get_qg
-00002c60: 6174 6528 7f32 3333 2c38 3533 310a 2020  ate(.233,8531.  
-00002c70: 2020 7374 643a 3a76 6563 746f 723c 5368    std::vector<Sh
-00002c80: 6172 7169 743a 3a51 4761 7465 3e20 6765  arqit::QGate> ge
-00002c90: 745f 7167 6174 6573 287f 3233 382c 3837  t_qgates(.238,87
-00002ca0: 3038 0a20 2020 2051 4369 7263 2620 6964  08.    QCirc& id
-00002cb0: 287f 3333 302c 3131 3938 300a 2020 2020  (.330,11980.    
-00002cc0: 5143 6972 6326 2078 287f 3333 362c 3132  QCirc& x(.336,12
-00002cd0: 3233 380a 2020 2020 5143 6972 6326 207a  238.    QCirc& z
-00002ce0: 287f 3334 322c 3132 3439 340a 2020 2020  (.342,12494.    
-00002cf0: 5143 6972 6326 2073 287f 3334 382c 3132  QCirc& s(.348,12
-00002d00: 3734 340a 2020 2020 5143 6972 6326 2073  744.    QCirc& s
-00002d10: 6467 287f 3335 342c 3133 3032 320a 2020  dg(.354,13022.  
-00002d20: 2020 5143 6972 6326 2074 287f 3336 302c    QCirc& t(.360,
-00002d30: 3133 3237 360a 2020 2020 5143 6972 6326  13276.    QCirc&
-00002d40: 2074 6467 287f 3336 362c 3133 3535 340a   tdg(.366,13554.
-00002d50: 2020 2020 5143 6972 6326 2068 287f 3337      QCirc& h(.37
-00002d60: 322c 3133 3832 300a 2020 2020 5143 6972  2,13820.    QCir
-00002d70: 6326 2072 7a28 7f33 3739 2c31 3431 3138  c& rz(.379,14118
-00002d80: 0a20 2020 2051 4369 7263 2620 6964 3228  .    QCirc& id2(
-00002d90: 7f33 3836 2c31 3434 3737 0a20 2020 2051  .386,14477.    Q
-00002da0: 4369 7263 2620 6378 287f 3339 332c 3134  Circ& cx(.393,14
-00002db0: 3832 330a 2020 2020 5143 6972 6326 2063  823.    QCirc& c
-00002dc0: 7a28 7f34 3030 2c31 3531 3630 0a20 2020  z(.400,15160.   
-00002dd0: 2051 4369 7263 2620 7278 287f 3430 372c   QCirc& rx(.407,
-00002de0: 3135 3438 310a 2020 2020 5143 6972 6326  15481.    QCirc&
-00002df0: 2063 6378 287f 3431 352c 3135 3837 370a   ccx(.415,15877.
-00002e00: 2020 2020 5143 6972 6326 2063 637a 287f      QCirc& ccz(.
-00002e10: 3432 332c 3136 3330 340a 2020 2020 5143  423,16304.    QC
-00002e20: 6972 6326 2079 287f 3432 392c 3136 3631  irc& y(.429,1661
-00002e30: 340a 2020 2020 5143 6972 6326 2073 7828  4.    QCirc& sx(
-00002e40: 7f34 3335 2c31 3638 3832 0a20 2020 2051  .435,16882.    Q
-00002e50: 4369 7263 2620 7378 6467 287f 3434 312c  Circ& sxdg(.441,
-00002e60: 3137 3138 340a 2020 2020 5143 6972 6326  17184.    QCirc&
-00002e70: 2072 7928 7f34 3438 2c31 3734 3739 0a20   ry(.448,17479. 
-00002e80: 2020 2051 4369 7263 2620 7028 7f34 3536     QCirc& p(.456
-00002e90: 2c31 3738 3435 0a20 2020 2051 4369 7263  ,17845.    QCirc
-00002ea0: 2620 6379 287f 3436 332c 3138 3138 380a  & cy(.463,18188.
-00002eb0: 2020 2020 5143 6972 6326 2063 7378 287f      QCirc& csx(.
-00002ec0: 3437 302c 3138 3535 350a 2020 2020 5143  470,18555.    QC
-00002ed0: 6972 6326 2063 7378 6467 287f 3437 372c  irc& csxdg(.477,
-00002ee0: 3138 3934 350a 2020 2020 5143 6972 6326  18945.    QCirc&
-00002ef0: 2063 6828 7f34 3834 2c31 3933 3234 0a20   ch(.484,19324. 
-00002f00: 2020 2051 4369 7263 2620 6373 287f 3439     QCirc& cs(.49
-00002f10: 322c 3139 3734 340a 2020 2020 5143 6972  2,19744.    QCir
-00002f20: 6326 2063 7364 6728 7f35 3030 2c32 3031  c& csdg(.500,201
-00002f30: 3338 0a20 2020 2051 4369 7263 2620 6374  38.    QCirc& ct
-00002f40: 287f 3530 382c 3230 3531 330a 2020 2020  (.508,20513.    
-00002f50: 5143 6972 6326 2063 7464 6728 7f35 3136  QCirc& ctdg(.516
-00002f60: 2c32 3039 3139 0a20 2020 2051 4369 7263  ,20919.    QCirc
-00002f70: 2620 6372 7828 7f35 3235 2c32 3133 3438  & crx(.525,21348
-00002f80: 0a20 2020 2051 4369 7263 2620 6372 7928  .    QCirc& cry(
-00002f90: 7f35 3334 2c32 3137 3835 0a20 2020 2051  .534,21785.    Q
-00002fa0: 4369 7263 2620 6372 7a28 7f35 3433 2c32  Circ& crz(.543,2
-00002fb0: 3232 3437 0a20 2020 2051 4369 7263 2620  2247.    QCirc& 
-00002fc0: 6370 287f 3535 322c 3232 3730 380a 2020  cp(.552,22708.  
-00002fd0: 2020 5143 6972 6326 2072 7878 287f 3536    QCirc& rxx(.56
-00002fe0: 312c 3233 3134 320a 2020 2020 5143 6972  1,23142.    QCir
-00002ff0: 6326 2072 7979 287f 3537 352c 3233 3633  c& ryy(.575,2363
-00003000: 300a 2020 2020 5143 6972 6326 2072 7a7a  0.    QCirc& rzz
-00003010: 287f 3538 392c 3234 3136 380a 2020 2020  (.589,24168.    
-00003020: 5143 6972 6326 2073 7728 7f35 3937 2c32  QCirc& sw(.597,2
-00003030: 3435 3236 0a20 2020 2051 4369 7263 2620  4526.    QCirc& 
-00003040: 6373 7728 7f36 3036 2c32 3439 3337 0a20  csw(.606,24937. 
-00003050: 2020 2051 4369 7263 2620 6363 785f 6465     QCirc& ccx_de
-00003060: 636f 6d70 5f41 287f 3631 352c 3235 3430  comp_A(.615,2540
-00003070: 300a 2020 2020 5143 6972 6326 2063 637a  0.    QCirc& ccz
-00003080: 5f64 6563 6f6d 705f 4128 7f36 3237 2c32  _decomp_A(.627,2
-00003090: 3539 3637 0a20 2020 2051 4369 7263 2620  5967.    QCirc& 
-000030a0: 6f70 6572 6174 6f72 2b3d 287f 6f70 6572  operator+=(.oper
-000030b0: 6174 6f72 2b3d 0136 3332 2c32 3632 3136  ator+=.632,26216
-000030c0: 0a20 2020 2066 7269 656e 6420 5143 6972  .    friend QCir
-000030d0: 6320 6f70 6572 6174 6f72 2b28 7f36 3333  c operator+(.633
-000030e0: 2c32 3632 3833 0a20 2020 2066 7269 656e  ,26283.    frien
-000030f0: 6420 7374 643a 3a6f 7374 7265 616d 2620  d std::ostream& 
-00003100: 6f70 6572 6174 6f72 3c3c 287f 3633 342c  operator<<(.634,
-00003110: 3236 3339 320a 0c0a 6461 6763 6972 632e  26392...dagcirc.
-00003120: 6370 702c 3136 3235 0a53 6861 7271 6974  cpp,1625.Sharqit
-00003130: 3a3a 4441 4743 6972 633a 3a44 4147 4369  ::DAGCirc::DAGCi
-00003140: 7263 287f 4441 4743 6972 6301 382c 3932  rc(.DAGCirc.8,92
-00003150: 0a53 6861 7271 6974 3a3a 4441 4743 6972  .Sharqit::DAGCir
-00003160: 633a 3a44 4147 4369 7263 287f 4441 4743  c::DAGCirc(.DAGC
-00003170: 6972 6301 3239 2c36 3939 0a73 7464 3a3a  irc.29,699.std::
-00003180: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
-00003190: 4441 4743 6972 633a 3a74 6f5f 7374 7269  DAGCirc::to_stri
-000031a0: 6e67 287f 746f 5f73 7472 696e 6701 3533  ng(.to_string.53
-000031b0: 2c31 3339 330a 7569 6e74 3332 5f74 2053  ,1393.uint32_t S
-000031c0: 6861 7271 6974 3a3a 4441 4743 6972 633a  harqit::DAGCirc:
-000031d0: 3a61 7070 656e 645f 6e6f 6465 287f 6170  :append_node(.ap
-000031e0: 7065 6e64 5f6e 6f64 6501 3732 2c31 3836  pend_node.72,186
-000031f0: 320a 7569 6e74 3332 5f74 2053 6861 7271  2.uint32_t Sharq
-00003200: 6974 3a3a 4441 4743 6972 633a 3a70 7265  it::DAGCirc::pre
-00003210: 765f 6e6f 6465 287f 7072 6576 5f6e 6f64  v_node(.prev_nod
-00003220: 6501 3830 2c32 3035 350a 7569 6e74 3332  e.80,2055.uint32
-00003230: 5f74 2053 6861 7271 6974 3a3a 4441 4743  _t Sharqit::DAGC
-00003240: 6972 633a 3a6e 6578 745f 6e6f 6465 287f  irc::next_node(.
-00003250: 6e65 7874 5f6e 6f64 6501 3939 2c32 3532  next_node.99,252
-00003260: 330a 766f 6964 2053 6861 7271 6974 3a3a  3.void Sharqit::
-00003270: 4441 4743 6972 633a 3a63 6f6e 6e65 6374  DAGCirc::connect
-00003280: 5f6e 6f64 6573 287f 636f 6e6e 6563 745f  _nodes(.connect_
-00003290: 6e6f 6465 7301 3131 382c 3239 3838 0a76  nodes.118,2988.v
-000032a0: 6f69 6420 5368 6172 7169 743a 3a44 4147  oid Sharqit::DAG
-000032b0: 4369 7263 3a3a 7265 6d6f 7665 5f6e 6f64  Circ::remove_nod
-000032c0: 6528 7f72 656d 6f76 655f 6e6f 6465 0131  e(.remove_node.1
-000032d0: 3239 2c33 3437 330a 766f 6964 2053 6861  29,3473.void Sha
-000032e0: 7271 6974 3a3a 4441 4743 6972 633a 3a72  rqit::DAGCirc::r
-000032f0: 656d 6f76 655f 6564 6765 287f 7265 6d6f  emove_edge(.remo
-00003300: 7665 5f65 6467 6501 3136 312c 3431 3233  ve_edge.161,4123
-00003310: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
-00003320: 4147 4369 7263 3a3a 7265 6d6f 7665 5f65  AGCirc::remove_e
-00003330: 6467 6528 7f72 656d 6f76 655f 6564 6765  dge(.remove_edge
-00003340: 0131 3739 2c34 3532 380a 766f 6964 2053  .179,4528.void S
-00003350: 6861 7271 6974 3a3a 4441 4743 6972 633a  harqit::DAGCirc:
-00003360: 3a72 656d 6f76 655f 6564 6765 735f 6f66  :remove_edges_of
-00003370: 5f6e 6f64 6528 7f72 656d 6f76 655f 6564  _node(.remove_ed
-00003380: 6765 735f 6f66 5f6e 6f64 6501 3139 372c  ges_of_node.197,
-00003390: 3439 3833 0a76 6f69 6420 5368 6172 7169  4983.void Sharqi
-000033a0: 743a 3a44 4147 4369 7263 3a3a 7265 6d6f  t::DAGCirc::remo
-000033b0: 7665 5f69 736f 6c61 7465 645f 6e6f 6465  ve_isolated_node
-000033c0: 7328 7f72 656d 6f76 655f 6973 6f6c 6174  s(.remove_isolat
-000033d0: 6564 5f6e 6f64 6573 0132 3131 2c35 3331  ed_nodes.211,531
-000033e0: 320a 5368 6172 7169 743a 3a44 4147 4369  2.Sharqit::DAGCi
-000033f0: 7263 2620 5368 6172 7169 743a 3a44 4147  rc& Sharqit::DAG
-00003400: 4369 7263 3a3a 6164 645f 7167 6174 6528  Circ::add_qgate(
-00003410: 7f61 6464 5f71 6761 7465 0132 3237 2c35  .add_qgate.227,5
-00003420: 3633 310a 5368 6172 7169 743a 3a51 4369  631.Sharqit::QCi
-00003430: 7263 2053 6861 7271 6974 3a3a 4441 4743  rc Sharqit::DAGC
-00003440: 6972 633a 3a74 6f5f 7163 6972 6328 7f74  irc::to_qcirc(.t
-00003450: 6f5f 7163 6972 6301 3236 342c 3637 3137  o_qcirc.264,6717
-00003460: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
-00003470: 4147 4369 7263 3a3a 6964 5f72 656d 6f76  AGCirc::id_remov
-00003480: 616c 287f 6964 5f72 656d 6f76 616c 0133  al(.id_removal.3
-00003490: 3036 2c37 3736 390a 766f 6964 2053 6861  06,7769.void Sha
-000034a0: 7271 6974 3a3a 4441 4743 6972 633a 3a63  rqit::DAGCirc::c
-000034b0: 785f 746f 5f63 7a5f 6761 7465 287f 6378  x_to_cz_gate(.cx
-000034c0: 5f74 6f5f 637a 5f67 6174 6501 3332 392c  _to_cz_gate.329,
-000034d0: 3834 3834 0a76 6f69 6420 5368 6172 7169  8484.void Sharqi
-000034e0: 743a 3a44 4147 4369 7263 3a3a 637a 5f74  t::DAGCirc::cz_t
-000034f0: 6f5f 6378 5f67 6174 6528 7f63 7a5f 746f  o_cx_gate(.cz_to
-00003500: 5f63 785f 6761 7465 0133 3539 2c39 3330  _cx_gate.359,930
-00003510: 370a 766f 6964 2053 6861 7271 6974 3a3a  7.void Sharqit::
-00003520: 4441 4743 6972 633a 3a68 6164 616d 6172  DAGCirc::hadamar
-00003530: 645f 6761 7465 5f72 6564 7563 7469 6f6e  d_gate_reduction
-00003540: 5f31 287f 6861 6461 6d61 7264 5f67 6174  _1(.hadamard_gat
-00003550: 655f 7265 6475 6374 696f 6e5f 3101 3339  e_reduction_1.39
-00003560: 342c 3130 3534 360a 766f 6964 2053 6861  4,10546.void Sha
-00003570: 7271 6974 3a3a 4441 4743 6972 633a 3a68  rqit::DAGCirc::h
-00003580: 6164 616d 6172 645f 6761 7465 5f72 6564  adamard_gate_red
-00003590: 7563 7469 6f6e 5f32 287f 6861 6461 6d61  uction_2(.hadama
-000035a0: 7264 5f67 6174 655f 7265 6475 6374 696f  rd_gate_reductio
-000035b0: 6e5f 3201 3433 342c 3131 3830 360a 766f  n_2.434,11806.vo
-000035c0: 6964 2053 6861 7271 6974 3a3a 4441 4743  id Sharqit::DAGC
-000035d0: 6972 633a 3a68 6164 616d 6172 645f 6761  irc::hadamard_ga
-000035e0: 7465 5f72 6564 7563 7469 6f6e 5f33 287f  te_reduction_3(.
-000035f0: 6861 6461 6d61 7264 5f67 6174 655f 7265  hadamard_gate_re
-00003600: 6475 6374 696f 6e5f 3301 3437 352c 3133  duction_3.475,13
-00003610: 3038 370a 7569 6e74 3332 5f74 2053 6861  087.uint32_t Sha
-00003620: 7271 6974 3a3a 4441 4743 6972 633a 3a68  rqit::DAGCirc::h
-00003630: 6164 616d 6172 645f 6761 7465 5f72 6564  adamard_gate_red
-00003640: 7563 7469 6f6e 287f 6861 6461 6d61 7264  uction(.hadamard
-00003650: 5f67 6174 655f 7265 6475 6374 696f 6e01  _gate_reduction.
-00003660: 3533 332c 3135 3036 320a 7569 6e74 3332  533,15062.uint32
-00003670: 5f74 2053 6861 7271 6974 3a3a 4441 4743  _t Sharqit::DAGC
-00003680: 6972 633a 3a73 696e 676c 655f 7175 6269  irc::single_qubi
-00003690: 745f 6761 7465 5f63 616e 6365 6c6c 6174  t_gate_cancellat
-000036a0: 696f 6e28 7f73 696e 676c 655f 7175 6269  ion(.single_qubi
-000036b0: 745f 6761 7465 5f63 616e 6365 6c6c 6174  t_gate_cancellat
-000036c0: 696f 6e01 3534 342c 3135 3237 350a 7569  ion.544,15275.ui
-000036d0: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
-000036e0: 4441 4743 6972 633a 3a74 776f 5f71 7562  DAGCirc::two_qub
-000036f0: 6974 5f67 6174 655f 6361 6e63 656c 6c61  it_gate_cancella
-00003700: 7469 6f6e 287f 7477 6f5f 7175 6269 745f  tion(.two_qubit_
-00003710: 6761 7465 5f63 616e 6365 6c6c 6174 696f  gate_cancellatio
-00003720: 6e01 3634 322c 3137 3939 340a 766f 6964  n.642,17994.void
-00003730: 2053 6861 7271 6974 3a3a 4441 4743 6972   Sharqit::DAGCir
-00003740: 633a 3a72 756c 655f 6261 7365 645f 6761  c::rule_based_ga
-00003750: 7465 5f72 6564 7563 7469 6f6e 287f 7275  te_reduction(.ru
-00003760: 6c65 5f62 6173 6564 5f67 6174 655f 7265  le_based_gate_re
-00003770: 6475 6374 696f 6e01 3733 322c 3230 3732  duction.732,2072
-00003780: 350a 0c0a 6c69 6e65 6172 5f6d 6170 2e63  5...linear_map.c
-00003790: 7070 2c34 3431 0a62 6f6f 6c20 5368 6172  pp,441.bool Shar
-000037a0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
-000037b0: 6973 5f7a 6572 6f28 7f69 735f 7a65 726f  is_zero(.is_zero
-000037c0: 0138 2c31 3034 0a62 6f6f 6c20 5368 6172  .8,104.bool Shar
-000037d0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
-000037e0: 6973 5f69 6465 6e74 6974 7928 7f69 735f  is_identity(.is_
-000037f0: 6964 656e 7469 7479 0132 312c 3434 340a  identity.21,444.
-00003800: 626f 6f6c 2053 6861 7271 6974 3a3a 4c69  bool Sharqit::Li
-00003810: 6e65 6172 4d61 703a 3a69 735f 6469 6167  nearMap::is_diag
-00003820: 6f6e 616c 287f 6973 5f64 6961 676f 6e61  onal(.is_diagona
-00003830: 6c01 3333 2c37 3432 0a62 6f6f 6c20 5368  l.33,742.bool Sh
-00003840: 6172 7169 743a 3a4c 696e 6561 724d 6170  arqit::LinearMap
-00003850: 3a3a 6973 5f69 6465 6e74 6974 795f 6d75  ::is_identity_mu
-00003860: 6c74 6970 6c65 5f63 6f6e 7374 616e 7428  ltiple_constant(
-00003870: 7f69 735f 6964 656e 7469 7479 5f6d 756c  .is_identity_mul
-00003880: 7469 706c 655f 636f 6e73 7461 6e74 0134  tiple_constant.4
-00003890: 352c 3130 3336 0a62 6f6f 6c20 5368 6172  5,1036.bool Shar
-000038a0: 7169 743a 3a4c 696e 6561 724d 6170 3a3a  qit::LinearMap::
-000038b0: 6973 5f75 6e69 7461 7279 287f 6973 5f75  is_unitary(.is_u
-000038c0: 6e69 7461 7279 0135 392c 3134 3239 0a62  nitary.59,1429.b
-000038d0: 6f6f 6c20 5368 6172 7169 743a 3a4c 696e  ool Sharqit::Lin
-000038e0: 6561 724d 6170 3a3a 6973 5f65 7175 616c  earMap::is_equal
-000038f0: 287f 6973 5f65 7175 616c 0137 302c 3136  (.is_equal.70,16
-00003900: 3930 0a53 6861 7271 6974 3a3a 4c69 6e65  90.Sharqit::Line
-00003910: 6172 4d61 7026 2053 6861 7271 6974 3a3a  arMap& Sharqit::
-00003920: 4c69 6e65 6172 4d61 703a 3a6f 7065 7261  LinearMap::opera
-00003930: 7465 5f71 6761 7465 287f 6f70 6572 6174  te_qgate(.operat
-00003940: 655f 7167 6174 6501 3831 2c31 3934 330a  e_qgate.81,1943.
-00003950: 0c0a 7368 6172 7169 742e 682c 3439 0a23  ..sharqit.h,49.#
-00003960: 6465 6669 6e65 2053 4841 5251 4954 5f48  define SHARQIT_H
-00003970: 7f37 2c38 380a 6e61 6d65 7370 6163 6520  .7,88.namespace 
-00003980: 5368 6172 7169 7420 7f31 392c 3239 340a  Sharqit .19,294.
-00003990: 0c0a 7368 6172 7169 742e 6370 702c 3137  ..sharqit.cpp,17
-000039a0: 360a 766f 6964 2070 7269 6e74 5f68 656c  6.void print_hel
-000039b0: 7028 7f31 312c 3133 300a 766f 6964 206f  p(.11,130.void o
-000039c0: 7074 696d 697a 6528 7f35 372c 3236 3332  ptimize(.57,2632
-000039d0: 0a76 6f69 6420 7665 7269 6679 5f65 7175  .void verify_equ
-000039e0: 616c 6974 7928 7f37 372c 3331 3439 0a76  ality(.77,3149.v
-000039f0: 6f69 6420 7261 6e64 6f6d 5f71 6369 7263  oid random_qcirc
-00003a00: 287f 3938 2c33 3731 340a 766f 6964 2070  (.98,3714.void p
-00003a10: 7269 6e74 5f73 7461 7473 287f 3132 362c  rint_stats(.126,
-00003a20: 3435 3031 0a76 6f69 6420 7368 6f77 5f71  4501.void show_q
-00003a30: 6369 7263 287f 3134 322c 3438 3230 0a69  circ(.142,4820.i
-00003a40: 6e74 206d 6169 6e28 7f31 3539 2c35 3135  nt main(.159,515
-00003a50: 370a 0c0a 7369 6d70 6c69 6679 2e63 7070  7...simplify.cpp
-00003a60: 2c31 3135 360a 766f 6964 2053 6861 7271  ,1156.void Sharq
-00003a70: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a66  it::ZXDiagram::f
-00003a80: 7573 655f 7370 6964 6572 7328 7f66 7573  use_spiders(.fus
-00003a90: 655f 7370 6964 6572 7301 382c 3134 320a  e_spiders.8,142.
-00003aa0: 766f 6964 2053 6861 7271 6974 3a3a 5a58  void Sharqit::ZX
-00003ab0: 4469 6167 7261 6d3a 3a63 6f6e 765f 785f  Diagram::conv_x_
-00003ac0: 746f 5f7a 287f 636f 6e76 5f78 5f74 6f5f  to_z(.conv_x_to_
-00003ad0: 7a01 3638 2c31 3639 360a 766f 6964 2053  z.68,1696.void S
-00003ae0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-00003af0: 6d3a 3a72 656d 6f76 655f 7061 7261 6c6c  m::remove_parall
-00003b00: 656c 5f73 656c 666c 6f6f 7073 5f68 6164  el_selfloops_had
-00003b10: 616d 6172 645f 6564 6765 7328 7f72 656d  amard_edges(.rem
-00003b20: 6f76 655f 7061 7261 6c6c 656c 5f73 656c  ove_parallel_sel
-00003b30: 666c 6f6f 7073 5f68 6164 616d 6172 645f  floops_hadamard_
-00003b40: 6564 6765 7301 3837 2c32 3234 360a 766f  edges.87,2246.vo
-00003b50: 6964 2053 6861 7271 6974 3a3a 5a58 4469  id Sharqit::ZXDi
-00003b60: 6167 7261 6d3a 3a75 7064 6174 655f 6e6f  agram::update_no
-00003b70: 6465 5f70 6c61 6365 7328 7f75 7064 6174  de_places(.updat
-00003b80: 655f 6e6f 6465 5f70 6c61 6365 7301 3131  e_node_places.11
-00003b90: 382c 3333 3434 0a76 6f69 6420 5368 6172  8,3344.void Shar
-00003ba0: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
-00003bb0: 7570 6461 7465 5f70 6861 7365 5f67 6164  update_phase_gad
-00003bc0: 6765 7428 7f75 7064 6174 655f 7068 6173  get(.update_phas
-00003bd0: 655f 6761 6467 6574 0131 3432 2c34 3130  e_gadget.142,410
-00003be0: 360a 766f 6964 2053 6861 7271 6974 3a3a  6.void Sharqit::
-00003bf0: 5a58 4469 6167 7261 6d3a 3a67 7261 7068  ZXDiagram::graph
-00003c00: 5f6c 696b 6528 7f67 7261 7068 5f6c 696b  _like(.graph_lik
-00003c10: 6501 3136 352c 3437 3830 0a76 6f69 6420  e.165,4780.void 
-00003c20: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00003c30: 616d 3a3a 6c63 6f6d 705f 6f6e 655f 7469  am::lcomp_one_ti
-00003c40: 6d65 287f 6c63 6f6d 705f 6f6e 655f 7469  me(.lcomp_one_ti
-00003c50: 6d65 0132 3238 2c36 3530 300a 7569 6e74  me.228,6500.uint
-00003c60: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
-00003c70: 4469 6167 7261 6d3a 3a6c 636f 6d70 287f  Diagram::lcomp(.
-00003c80: 6c63 6f6d 7001 3234 332c 3639 3830 0a76  lcomp.243,6980.v
-00003c90: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
-00003ca0: 6961 6772 616d 3a3a 7069 766f 7431 5f6f  iagram::pivot1_o
-00003cb0: 6e65 5f74 696d 6528 7f70 6976 6f74 315f  ne_time(.pivot1_
-00003cc0: 6f6e 655f 7469 6d65 0132 3935 2c38 3334  one_time.295,834
-00003cd0: 360a 7569 6e74 3332 5f74 2053 6861 7271  6.uint32_t Sharq
-00003ce0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a70  it::ZXDiagram::p
-00003cf0: 6976 6f74 3128 7f70 6976 6f74 3101 3335  ivot1(.pivot1.35
-00003d00: 312c 3130 3237 300a 766f 6964 2053 6861  1,10270.void Sha
-00003d10: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
-00003d20: 3a70 6976 6f74 325f 6f6e 655f 7469 6d65  :pivot2_one_time
-00003d30: 287f 7069 766f 7432 5f6f 6e65 5f74 696d  (.pivot2_one_tim
-00003d40: 6501 3433 312c 3132 3238 300a 7569 6e74  e.431,12280.uint
-00003d50: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
-00003d60: 4469 6167 7261 6d3a 3a70 6976 6f74 3228  Diagram::pivot2(
-00003d70: 7f70 6976 6f74 3201 3531 312c 3134 3937  .pivot2.511,1497
-00003d80: 360a 766f 6964 2053 6861 7271 6974 3a3a  6.void Sharqit::
-00003d90: 5a58 4469 6167 7261 6d3a 3a70 6976 6f74  ZXDiagram::pivot
-00003da0: 335f 6f6e 655f 7469 6d65 287f 7069 766f  3_one_time(.pivo
-00003db0: 7433 5f6f 6e65 5f74 696d 6501 3539 322c  t3_one_time.592,
-00003dc0: 3137 3033 380a 7569 6e74 3332 5f74 2053  17038.uint32_t S
-00003dd0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
-00003de0: 6d3a 3a70 6976 6f74 3328 7f70 6976 6f74  m::pivot3(.pivot
-00003df0: 3301 3639 322c 3230 3336 330a 766f 6964  3.692,20363.void
-00003e00: 2053 6861 7271 6974 3a3a 5a58 4469 6167   Sharqit::ZXDiag
-00003e10: 7261 6d3a 3a69 645f 7265 6d6f 7661 6c28  ram::id_removal(
-00003e20: 7f69 645f 7265 6d6f 7661 6c01 3738 332c  .id_removal.783,
-00003e30: 3232 3639 300a 766f 6964 2053 6861 7271  22690.void Sharq
-00003e40: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a67  it::ZXDiagram::g
-00003e50: 6675 7369 6f6e 5f6f 6e65 5f74 696d 6528  fusion_one_time(
-00003e60: 7f67 6675 7369 6f6e 5f6f 6e65 5f74 696d  .gfusion_one_tim
-00003e70: 6501 3833 382c 3234 3332 390a 7569 6e74  e.838,24329.uint
-00003e80: 3332 5f74 2053 6861 7271 6974 3a3a 5a58  32_t Sharqit::ZX
-00003e90: 4469 6167 7261 6d3a 3a67 6675 7369 6f6e  Diagram::gfusion
-00003ea0: 287f 6766 7573 696f 6e01 3834 362c 3234  (.gfusion.846,24
-00003eb0: 3634 380a 766f 6964 2053 6861 7271 6974  648.void Sharqit
-00003ec0: 3a3a 5a58 4469 6167 7261 6d3a 3a73 696d  ::ZXDiagram::sim
-00003ed0: 706c 6966 7928 7f73 696d 706c 6966 7901  plify(.simplify.
-00003ee0: 3937 392c 3238 3434 370a 0c0a 7068 6173  979,28447...phas
-00003ef0: 652e 682c 3931 340a 2364 6566 696e 6520  e.h,914.#define 
-00003f00: 5048 4153 455f 487f 372c 3830 0a20 2063  PHASE_H.7,80.  c
-00003f10: 6c61 7373 2050 6861 7365 7f32 332c 3239  lass Phase.23,29
-00003f20: 360a 2020 2020 4672 6163 7469 6f6e 2066  6.    Fraction f
-00003f30: 7261 635f 3b7f 3236 2c33 3235 0a20 2020  rac_;.26,325.   
-00003f40: 2050 6861 7365 287f 3333 2c36 3238 0a20   Phase(.33,628. 
-00003f50: 2020 2050 6861 7365 287f 3338 2c38 3437     Phase(.38,847
-00003f60: 0a20 2020 2050 6861 7365 287f 3433 2c31  .    Phase(.43,1
-00003f70: 3034 310a 2020 2020 5068 6173 6528 7f34  041.    Phase(.4
-00003f80: 382c 3131 3637 0a20 2020 2046 7261 6374  8,1167.    Fract
-00003f90: 696f 6e20 6672 6163 287f 3530 2c31 3234  ion frac(.50,124
-00003fa0: 390a 2020 2020 766f 6964 2066 7261 6328  9.    void frac(
-00003fb0: 7f35 322c 3133 3231 0a20 2020 2064 6f75  .52,1321.    dou
-00003fc0: 626c 6520 7661 6c75 6528 7f36 322c 3136  ble value(.62,16
-00003fd0: 3038 0a20 2020 2062 6f6f 6c20 6973 5f7a  08.    bool is_z
-00003fe0: 6572 6f28 7f36 372c 3138 3035 0a20 2020  ero(.67,1805.   
-00003ff0: 2062 6f6f 6c20 6973 5f70 6f73 6974 6976   bool is_positiv
-00004000: 6528 7f37 322c 3139 3833 0a20 2020 2062  e(.72,1983.    b
-00004010: 6f6f 6c20 6973 5f6e 6567 6174 6976 6528  ool is_negative(
-00004020: 7f37 372c 3231 3635 0a20 2020 2076 6f69  .77,2165.    voi
-00004030: 6420 7265 6475 6365 287f 3831 2c32 3330  d reduce(.81,230
-00004040: 320a 2020 2020 766f 6964 206d 6f64 5f32  2.    void mod_2
-00004050: 7069 287f 3835 2c32 3339 310a 2020 2020  pi(.85,2391.    
-00004060: 5068 6173 6520 6f70 6572 6174 6f72 2b28  Phase operator+(
-00004070: 7f39 392c 3238 3932 0a20 2020 2050 6861  .99,2892.    Pha
-00004080: 7365 206f 7065 7261 746f 722d 287f 3130  se operator-(.10
-00004090: 302c 3239 3338 0a20 2020 2050 6861 7365  0,2938.    Phase
-000040a0: 2620 6f70 6572 6174 6f72 2b3d 287f 6f70  & operator+=(.op
-000040b0: 6572 6174 6f72 2b3d 0131 3031 2c32 3939  erator+=.101,299
-000040c0: 320a 2020 2020 5068 6173 6526 206f 7065  2.    Phase& ope
-000040d0: 7261 746f 722d 3d28 7f6f 7065 7261 746f  rator-=(.operato
-000040e0: 722d 3d01 3130 322c 3330 3731 0a20 2020  r-=.102,3071.   
-000040f0: 2050 6861 7365 2620 6f70 6572 6174 6f72   Phase& operator
-00004100: 2a3d 287f 6f70 6572 6174 6f72 2a3d 0131  *=(.operator*=.1
-00004110: 3033 2c33 3135 300a 2020 2020 5068 6173  03,3150.    Phas
-00004120: 6526 206f 7065 7261 746f 722f 3d28 7f6f  e& operator/=(.o
-00004130: 7065 7261 746f 722f 3d01 3130 342c 3332  perator/=.104,32
-00004140: 3233 0a20 2020 2066 7269 656e 6420 626f  23.    friend bo
-00004150: 6f6c 206f 7065 7261 746f 723d 3d28 7f6f  ol operator==(.o
-00004160: 7065 7261 746f 723d 3d01 3130 352c 3332  perator==.105,32
-00004170: 3936 0a20 2020 2066 7269 656e 6420 626f  96.    friend bo
-00004180: 6f6c 206f 7065 7261 746f 7221 3d28 7f6f  ol operator!=(.o
-00004190: 7065 7261 746f 7221 3d01 3131 302c 3335  perator!=.110,35
-000041a0: 3036 0a20 2020 2066 7269 656e 6420 5068  06.    friend Ph
-000041b0: 6173 6520 6f70 6572 6174 6f72 2b28 7f31  ase operator+(.1
-000041c0: 3131 2c33 3539 350a 2020 2020 6672 6965  11,3595.    frie
-000041d0: 6e64 2050 6861 7365 206f 7065 7261 746f  nd Phase operato
-000041e0: 722d 287f 3131 322c 3337 3031 0a20 2020  r-(.112,3701.   
-000041f0: 2066 7269 656e 6420 5068 6173 6520 6f70   friend Phase op
-00004200: 6572 6174 6f72 2a28 7f31 3133 2c33 3830  erator*(.113,380
-00004210: 370a 2020 2020 6672 6965 6e64 2050 6861  7.    friend Pha
-00004220: 7365 206f 7065 7261 746f 722a 287f 3131  se operator*(.11
-00004230: 342c 3339 3037 0a20 2020 2066 7269 656e  4,3907.    frien
-00004240: 6420 5068 6173 6520 6f70 6572 6174 6f72  d Phase operator
-00004250: 2f28 7f31 3135 2c34 3030 370a 2020 2020  /(.115,4007.    
-00004260: 6672 6965 6e64 2073 7464 3a3a 6f73 7472  friend std::ostr
-00004270: 6561 6d26 206f 7065 7261 746f 723c 3c28  eam& operator<<(
-00004280: 7f31 3136 2c34 3130 370a 0c0a 6672 6163  .116,4107...frac
-00004290: 7469 6f6e 2e68 2c31 3731 320a 2364 6566  tion.h,1712.#def
-000042a0: 696e 6520 4652 4143 5449 4f4e 5f48 7f37  ine FRACTION_H.7
-000042b0: 2c38 390a 2020 636c 6173 7320 4672 6163  ,89.  class Frac
-000042c0: 7469 6f6e 7f31 382c 3234 320a 2020 2020  tion.18,242.    
-000042d0: 696e 7433 325f 7420 6e75 6d65 7261 746f  int32_t numerato
-000042e0: 725f 3b7f 3231 2c32 3734 0a20 2020 2069  r_;.21,274.    i
-000042f0: 6e74 3332 5f74 2064 656e 6f6d 696e 6174  nt32_t denominat
-00004300: 6f72 5f3b 7f32 322c 3332 390a 2020 2020  or_;.22,329.    
-00004310: 4672 6163 7469 6f6e 287f 3237 2c34 3536  Fraction(.27,456
-00004320: 0a20 2020 2046 7261 6374 696f 6e28 7f33  .    Fraction(.3
-00004330: 332c 3637 390a 2020 2020 4672 6163 7469  3,679.    Fracti
-00004340: 6f6e 287f 3339 2c39 3139 0a20 2020 2069  on(.39,919.    i
-00004350: 6e74 3332 5f74 206e 756d 6572 6174 6f72  nt32_t numerator
-00004360: 287f 3431 2c31 3035 330a 2020 2020 696e  (.41,1053.    in
-00004370: 7433 325f 7420 6465 6e6f 6d69 6e61 746f  t32_t denominato
-00004380: 7228 7f34 332c 3131 3431 0a20 2020 2076  r(.43,1141.    v
-00004390: 6f69 6420 6e75 6d65 7261 746f 7228 7f34  oid numerator(.4
-000043a0: 352c 3132 3331 0a20 2020 2076 6f69 6420  5,1231.    void 
-000043b0: 6465 6e6f 6d69 6e61 746f 7228 7f34 372c  denominator(.47,
-000043c0: 3133 3438 0a20 2020 2046 7261 6374 696f  1348.    Fractio
-000043d0: 6e20 6164 6428 7f35 382c 3137 3039 0a20  n add(.58,1709. 
-000043e0: 2020 2046 7261 6374 696f 6e20 6164 6428     Fraction add(
-000043f0: 7f36 392c 3231 3330 0a20 2020 2046 7261  .69,2130.    Fra
-00004400: 6374 696f 6e20 7375 6228 7f37 352c 3233  ction sub(.75,23
-00004410: 3439 0a20 2020 2046 7261 6374 696f 6e20  49.    Fraction 
-00004420: 7375 6228 7f38 362c 3237 3732 0a20 2020  sub(.86,2772.   
-00004430: 2046 7261 6374 696f 6e20 6d75 6c28 7f39   Fraction mul(.9
-00004440: 322c 3239 3931 0a20 2020 2046 7261 6374  2,2991.    Fract
-00004450: 696f 6e20 6d75 6c28 7f31 3033 2c33 3337  ion mul(.103,337
-00004460: 370a 2020 2020 4672 6163 7469 6f6e 2064  7.    Fraction d
-00004470: 6976 287f 3130 392c 3335 3931 0a20 2020  iv(.109,3591.   
-00004480: 2046 7261 6374 696f 6e20 6469 7628 7f31   Fraction div(.1
-00004490: 3230 2c33 3937 360a 2020 2020 626f 6f6c  20,3976.    bool
-000044a0: 2069 735f 7a65 726f 287f 3132 352c 3431   is_zero(.125,41
-000044b0: 3732 0a20 2020 2062 6f6f 6c20 6973 5f70  72.    bool is_p
-000044c0: 6f73 6974 6976 6528 7f31 3330 2c34 3335  ositive(.130,435
-000044d0: 320a 2020 2020 626f 6f6c 2069 735f 6e65  2.    bool is_ne
-000044e0: 6761 7469 7665 287f 3133 352c 3435 3530  gative(.135,4550
-000044f0: 0a20 2020 2076 6f69 6420 7265 6475 6365  .    void reduce
-00004500: 287f 3133 392c 3436 3731 0a20 2020 2073  (.139,4671.    s
-00004510: 7461 7469 6320 696e 7433 325f 7420 6763  tatic int32_t gc
-00004520: 6428 7f31 3630 2c35 3237 390a 2020 2020  d(.160,5279.    
-00004530: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
-00004540: 722b 287f 3137 322c 3535 3335 0a20 2020  r+(.172,5535.   
-00004550: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-00004560: 6f72 2d28 7f31 3733 2c35 3538 340a 2020  or-(.173,5584.  
-00004570: 2020 4672 6163 7469 6f6e 2620 6f70 6572    Fraction& oper
-00004580: 6174 6f72 2b3d 287f 6f70 6572 6174 6f72  ator+=(.operator
-00004590: 2b3d 0131 3734 2c35 3633 350a 2020 2020  +=.174,5635.    
-000045a0: 4672 6163 7469 6f6e 2620 6f70 6572 6174  Fraction& operat
-000045b0: 6f72 2b3d 287f 6f70 6572 6174 6f72 2b3d  or+=(.operator+=
-000045c0: 0131 3831 2c35 3832 330a 2020 2020 4672  .181,5823.    Fr
-000045d0: 6163 7469 6f6e 2620 6f70 6572 6174 6f72  action& operator
-000045e0: 2d3d 287f 6f70 6572 6174 6f72 2d3d 0131  -=(.operator-=.1
-000045f0: 3832 2c35 3930 350a 2020 2020 4672 6163  82,5905.    Frac
-00004600: 7469 6f6e 2620 6f70 6572 6174 6f72 2d3d  tion& operator-=
-00004610: 287f 6f70 6572 6174 6f72 2d3d 0131 3839  (.operator-=.189
-00004620: 2c36 3039 330a 2020 2020 4672 6163 7469  ,6093.    Fracti
-00004630: 6f6e 2620 6f70 6572 6174 6f72 2a3d 287f  on& operator*=(.
-00004640: 6f70 6572 6174 6f72 2a3d 0131 3930 2c36  operator*=.190,6
-00004650: 3137 350a 2020 2020 4672 6163 7469 6f6e  175.    Fraction
-00004660: 2620 6f70 6572 6174 6f72 2a3d 287f 6f70  & operator*=(.op
-00004670: 6572 6174 6f72 2a3d 0131 3937 2c36 3336  erator*=.197,636
-00004680: 330a 2020 2020 4672 6163 7469 6f6e 2620  3.    Fraction& 
-00004690: 6f70 6572 6174 6f72 2f3d 287f 6f70 6572  operator/=(.oper
-000046a0: 6174 6f72 2f3d 0131 3938 2c36 3434 350a  ator/=.198,6445.
-000046b0: 2020 2020 4672 6163 7469 6f6e 2620 6f70      Fraction& op
-000046c0: 6572 6174 6f72 2f3d 287f 6f70 6572 6174  erator/=(.operat
-000046d0: 6f72 2f3d 0132 3035 2c36 3633 330a 2020  or/=.205,6633.  
-000046e0: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
-000046f0: 6572 6174 6f72 3d3d 287f 6f70 6572 6174  erator==(.operat
-00004700: 6f72 3d3d 0132 3036 2c36 3731 350a 2020  or==.206,6715.  
-00004710: 2020 6672 6965 6e64 2062 6f6f 6c20 6f70    friend bool op
-00004720: 6572 6174 6f72 213d 287f 6f70 6572 6174  erator!=(.operat
-00004730: 6f72 213d 0132 3130 2c36 3838 370a 2020  or!=.210,6887.  
-00004740: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-00004750: 6e20 6f70 6572 6174 6f72 2b28 7f32 3131  n operator+(.211
-00004760: 2c36 3938 320a 2020 2020 6672 6965 6e64  ,6982.    friend
-00004770: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-00004780: 6f72 2b28 7f32 3132 2c37 3037 390a 2020  or+(.212,7079.  
-00004790: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-000047a0: 6e20 6f70 6572 6174 6f72 2b28 7f32 3133  n operator+(.213
-000047b0: 2c37 3138 340a 2020 2020 6672 6965 6e64  ,7184.    friend
-000047c0: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-000047d0: 6f72 2d28 7f32 3134 2c37 3238 390a 2020  or-(.214,7289.  
-000047e0: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-000047f0: 6e20 6f70 6572 6174 6f72 2d28 7f32 3135  n operator-(.215
-00004800: 2c37 3338 360a 2020 2020 6672 6965 6e64  ,7386.    friend
-00004810: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-00004820: 6f72 2d28 7f32 3136 2c37 3439 310a 2020  or-(.216,7491.  
-00004830: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-00004840: 6e20 6f70 6572 6174 6f72 2a28 7f32 3137  n operator*(.217
-00004850: 2c37 3539 360a 2020 2020 6672 6965 6e64  ,7596.    friend
-00004860: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-00004870: 6f72 2a28 7f32 3138 2c37 3639 330a 2020  or*(.218,7693.  
-00004880: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-00004890: 6e20 6f70 6572 6174 6f72 2a28 7f32 3139  n operator*(.219
-000048a0: 2c37 3739 380a 2020 2020 6672 6965 6e64  ,7798.    friend
-000048b0: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-000048c0: 6f72 2f28 7f32 3230 2c37 3930 330a 2020  or/(.220,7903.  
-000048d0: 2020 6672 6965 6e64 2046 7261 6374 696f    friend Fractio
-000048e0: 6e20 6f70 6572 6174 6f72 2f28 7f32 3231  n operator/(.221
-000048f0: 2c38 3030 300a 2020 2020 6672 6965 6e64  ,8000.    friend
-00004900: 2046 7261 6374 696f 6e20 6f70 6572 6174   Fraction operat
-00004910: 6f72 2f28 7f32 3232 2c38 3130 350a 2020  or/(.222,8105.  
-00004920: 2020 6672 6965 6e64 2073 7464 3a3a 6f73    friend std::os
-00004930: 7472 6561 6d26 206f 7065 7261 746f 723c  tream& operator<
-00004940: 3c28 7f32 3233 2c38 3231 300a 0c0a 7a78  <(.223,8210...zx
-00004950: 6e6f 6465 2e63 7070 2c34 350a 7374 643a  node.cpp,45.std:
-00004960: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
-00004970: 3a5a 584e 6f64 653a 3a6e 616d 6528 7f6e  :ZXNode::name(.n
-00004980: 616d 6501 382c 3839 0a0c 0a7a 7864 6961  ame.8,89...zxdia
-00004990: 6772 616d 2e63 7070 2c31 3230 360a 5368  gram.cpp,1206.Sh
-000049a0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-000049b0: 3a3a 5a58 4469 6167 7261 6d28 7f5a 5844  ::ZXDiagram(.ZXD
-000049c0: 6961 6772 616d 0138 2c39 350a 7374 643a  iagram.8,95.std:
-000049d0: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
-000049e0: 3a5a 5844 6961 6772 616d 3a3a 746f 5f73  :ZXDiagram::to_s
-000049f0: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
-00004a00: 0133 342c 3839 350a 7374 643a 3a6d 6170  .34,895.std::map
-00004a10: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
-00004a20: 6e74 3332 5f74 3e20 5368 6172 7169 743a  nt32_t> Sharqit:
-00004a30: 3a5a 5844 6961 6772 616d 3a3a 7374 6174  :ZXDiagram::stat
-00004a40: 7328 7f73 7461 7473 0135 342c 3134 3034  s(.stats.54,1404
-00004a50: 0a76 6f69 6420 5368 6172 7169 743a 3a5a  .void Sharqit::Z
-00004a60: 5844 6961 6772 616d 3a3a 746f 5f64 6f74  XDiagram::to_dot
-00004a70: 5f66 696c 6528 7f74 6f5f 646f 745f 6669  _file(.to_dot_fi
-00004a80: 6c65 0138 302c 3233 3738 0a76 6f69 6420  le.80,2378.void 
-00004a90: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
-00004aa0: 616d 3a3a 746f 5f73 7667 5f66 696c 6528  am::to_svg_file(
-00004ab0: 7f74 6f5f 7376 675f 6669 6c65 0132 3234  .to_svg_file.224
-00004ac0: 2c36 3930 390a 766f 6964 2053 6861 7271  ,6909.void Sharq
-00004ad0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a61  it::ZXDiagram::a
-00004ae0: 6464 5f71 6761 7465 287f 6164 645f 7167  dd_qgate(.add_qg
-00004af0: 6174 6501 3233 372c 3733 3834 0a62 6f6f  ate.237,7384.boo
-00004b00: 6c20 5368 6172 7169 743a 3a5a 5844 6961  l Sharqit::ZXDia
-00004b10: 6772 616d 3a3a 6368 6563 6b5f 636f 6e6e  gram::check_conn
-00004b20: 6563 7428 7f63 6865 636b 5f63 6f6e 6e65  ect(.check_conne
-00004b30: 6374 0133 3738 2c31 3230 3235 0a76 6f69  ct.378,12025.voi
-00004b40: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
-00004b50: 6772 616d 3a3a 786f 725f 6861 6461 6d61  gram::xor_hadama
-00004b60: 7264 5f65 6467 6528 7f78 6f72 5f68 6164  rd_edge(.xor_had
-00004b70: 616d 6172 645f 6564 6765 0134 3031 2c31  amard_edge.401,1
-00004b80: 3234 3333 0a76 6f69 6420 5368 6172 7169  2433.void Sharqi
-00004b90: 743a 3a5a 5844 6961 6772 616d 3a3a 786f  t::ZXDiagram::xo
-00004ba0: 725f 6861 6461 6d61 7264 5f65 6467 6573  r_hadamard_edges
-00004bb0: 287f 786f 725f 6861 6461 6d61 7264 5f65  (.xor_hadamard_e
-00004bc0: 6467 6573 0134 3334 2c31 3334 3337 0a53  dges.434,13437.S
-00004bd0: 6861 7271 6974 3a3a 5a58 4e6f 6465 4b69  harqit::ZXNodeKi
-00004be0: 6e64 2053 6861 7271 6974 3a3a 5a58 4469  nd Sharqit::ZXDi
-00004bf0: 6167 7261 6d3a 3a72 656d 6f76 655f 6e6f  agram::remove_no
-00004c00: 6465 287f 7265 6d6f 7665 5f6e 6f64 6501  de(.remove_node.
-00004c10: 3434 362c 3133 3830 370a 5368 6172 7169  446,13807.Sharqi
-00004c20: 743a 3a5a 5845 6467 654b 696e 6420 5368  t::ZXEdgeKind Sh
-00004c30: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-00004c40: 3a3a 7265 6d6f 7665 5f65 6467 6528 7f72  ::remove_edge(.r
-00004c50: 656d 6f76 655f 6564 6765 0134 3830 2c31  emove_edge.480,1
-00004c60: 3435 3036 0a75 696e 7433 325f 7420 5368  4506.uint32_t Sh
-00004c70: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-00004c80: 3a3a 6170 7065 6e64 5f6e 6f64 6528 7f61  ::append_node(.a
-00004c90: 7070 656e 645f 6e6f 6465 0135 3034 2c31  ppend_node.504,1
-00004ca0: 3530 3437 0a75 696e 7433 325f 7420 5368  5047.uint32_t Sh
-00004cb0: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
-00004cc0: 3a3a 6170 7065 6e64 5f6e 6f64 6528 7f61  ::append_node(.a
-00004cd0: 7070 656e 645f 6e6f 6465 0135 3132 2c31  ppend_node.512,1
-00004ce0: 3532 3431 0a76 6f69 6420 5368 6172 7169  5241.void Sharqi
-00004cf0: 743a 3a5a 5844 6961 6772 616d 3a3a 636f  t::ZXDiagram::co
-00004d00: 6e6e 6563 745f 6e6f 6465 7328 7f63 6f6e  nnect_nodes(.con
-00004d10: 6e65 6374 5f6e 6f64 6573 0135 3235 2c31  nect_nodes.525,1
-00004d20: 3535 3833 0a76 6f69 6420 5368 6172 7169  5583.void Sharqi
-00004d30: 743a 3a5a 5844 6961 6772 616d 3a3a 7377  t::ZXDiagram::sw
-00004d40: 6170 5f6e 6f64 6573 287f 7377 6170 5f6e  ap_nodes(.swap_n
-00004d50: 6f64 6573 0135 3333 2c31 3538 3339 0a76  odes.533,15839.v
-00004d60: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
-00004d70: 6961 6772 616d 3a3a 7265 6d6f 7665 5f69  iagram::remove_i
-00004d80: 736f 6c61 7465 645f 7370 6964 6572 7328  solated_spiders(
-00004d90: 7f72 656d 6f76 655f 6973 6f6c 6174 6564  .remove_isolated
-00004da0: 5f73 7069 6465 7273 0135 3438 2c31 3632  _spiders.548,162
-00004db0: 3235 0a76 6f69 6420 5368 6172 7169 743a  25.void Sharqit:
-00004dc0: 3a5a 5844 6961 6772 616d 3a3a 726f 775f  :ZXDiagram::row_
-00004dd0: 6f70 6572 6174 696f 6e28 7f72 6f77 5f6f  operation(.row_o
-00004de0: 7065 7261 7469 6f6e 0135 3634 2c31 3635  peration.564,165
-00004df0: 3438 0a73 7464 3a3a 7665 6374 6f72 3c75  48.std::vector<u
-00004e00: 696e 7433 325f 743e 2053 6861 7271 6974  int32_t> Sharqit
-00004e10: 3a3a 5a58 4469 6167 7261 6d3a 3a61 646a  ::ZXDiagram::adj
-00004e20: 6163 656e 745f 6e6f 6465 5f69 6e64 6578  acent_node_index
-00004e30: 6573 287f 6164 6a61 6365 6e74 5f6e 6f64  es(.adjacent_nod
-00004e40: 655f 696e 6465 7865 7301 3537 332c 3136  e_indexes.573,16
-00004e50: 3736 360a 0c0a 6269 6e61 7279 5f6d 6174  766...binary_mat
-00004e60: 7269 782e 6370 702c 3136 320a 7374 643a  rix.cpp,162.std:
-00004e70: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
-00004e80: 3a42 696e 6172 794d 6174 7269 783a 3a74  :BinaryMatrix::t
-00004e90: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
-00004ea0: 696e 6701 382c 3131 330a 7374 643a 3a76  ing.8,113.std::v
-00004eb0: 6563 746f 723c 7374 643a 3a70 6169 723c  ector<std::pair<
-00004ec0: 7569 6e74 3332 5f74 2c20 7569 6e74 3332  uint32_t, uint32
-00004ed0: 5f74 3e3e 2053 6861 7271 6974 3a3a 4269  _t>> Sharqit::Bi
-00004ee0: 6e61 7279 4d61 7472 6978 3a3a 6761 7573  naryMatrix::gaus
-00004ef0: 735f 7265 6475 6365 287f 6761 7573 735f  s_reduce(.gauss_
-00004f00: 7265 6475 6365 0132 382c 3439 300a 0c0a  reduce.28,490...
-00004f10: 7a78 2e68 2c33 3139 320a 2364 6566 696e  zx.h,3192.#defin
-00004f20: 6520 5a58 5f48 7f31 312c 3839 330a 2020  e ZX_H.11,893.  
-00004f30: 656e 756d 205a 584e 6f64 654b 696e 6420  enum ZXNodeKind 
-00004f40: 7f32 352c 3130 3832 0a09 0920 2020 5853  .25,1082...   XS
-00004f50: 7069 6465 722c 7f32 362c 3131 3032 0a09  pider,.26,1102..
-00004f60: 0920 2020 5a53 7069 6465 722c 7f32 372c  .   ZSpider,.27,
-00004f70: 3131 3330 0a09 0920 2020 496e 7075 742c  1130...   Input,
-00004f80: 7f32 382c 3131 3538 0a09 0920 2020 4f75  .28,1158...   Ou
-00004f90: 7470 7574 207f 3239 2c31 3138 360a 2020  tput .29,1186.  
-00004fa0: 656e 756d 205a 5845 6467 654b 696e 6420  enum ZXEdgeKind 
-00004fb0: 7f33 322c 3132 3534 0a09 0920 2020 4e6f  .32,1254...   No
-00004fc0: 6e65 2c7f 3333 2c31 3237 340a 0909 2020  ne,.33,1274...  
-00004fd0: 2050 6c61 696e 2c7f 3334 2c31 3331 320a   Plain,.34,1312.
-00004fe0: 0909 2020 2048 6164 616d 6172 6420 7f33  ..   Hadamard .3
-00004ff0: 352c 3133 3738 0a20 2065 6e75 6d20 5a58  5,1378.  enum ZX
-00005000: 4469 6167 7261 6d4b 696e 6420 7f33 382c  DiagramKind .38,
-00005010: 3134 3631 0a09 0920 2020 2020 2047 656e  1461...      Gen
-00005020: 6572 616c 2c7f 3339 2c31 3438 340a 0909  eral,.39,1484...
-00005030: 2020 2020 2020 4772 6170 684c 696b 6520        GraphLike 
-00005040: 7f34 302c 3135 3235 0a20 2065 6e75 6d20  .40,1525.  enum 
-00005050: 5a58 4e6f 6465 506c 6163 6520 7f34 332c  ZXNodePlace .43,
-00005060: 3136 3030 0a09 0920 2020 2054 6572 6d69  1600...    Termi
-00005070: 6e61 6c2c 7f34 342c 3136 3231 0a09 0920  nal,.44,1621... 
-00005080: 2020 2042 6f75 6e64 6172 792c 7f34 352c     Boundary,.45,
-00005090: 3136 3636 0a09 0920 2020 2049 6e74 6572  1666...    Inter
-000050a0: 6e61 6c20 7f34 362c 3137 3436 0a20 2063  nal .46,1746.  c
-000050b0: 6c61 7373 205a 584e 6f64 657f 3539 2c32  lass ZXNode.59,2
-000050c0: 3233 320a 2020 2020 5a58 4e6f 6465 4b69  232.    ZXNodeKi
-000050d0: 6e64 206b 696e 645f 3b7f 3632 2c32 3236  nd kind_;.62,226
-000050e0: 320a 2020 2020 5068 6173 6520 7068 6173  2.    Phase phas
-000050f0: 655f 3b7f 3633 2c32 3332 300a 2020 2020  e_;.63,2320.    
-00005100: 7569 6e74 3332 5f74 2071 5f3b 7f36 342c  uint32_t q_;.64,
-00005110: 3233 3735 0a20 2020 2062 6f6f 6c20 7067  2375.    bool pg
-00005120: 5f70 6861 7365 5f3b 7f36 352c 3234 3430  _phase_;.65,2440
-00005130: 0a20 2020 2062 6f6f 6c20 7067 5f72 6f6f  .    bool pg_roo
-00005140: 745f 3b7f 3636 2c32 3532 350a 2020 2020  t_;.66,2525.    
-00005150: 626f 6f6c 2070 675f 6c65 6166 5f3b 7f36  bool pg_leaf_;.6
-00005160: 372c 3236 3038 0a20 2020 205a 584e 6f64  7,2608.    ZXNod
-00005170: 6528 7f37 382c 3331 3237 0a20 2020 205a  e(.78,3127.    Z
-00005180: 584e 6f64 6528 7f38 352c 3335 3232 0a20  XNode(.85,3522. 
-00005190: 2020 205a 584e 6f64 654b 696e 6420 6b69     ZXNodeKind ki
-000051a0: 6e64 287f 3838 2c33 3732 300a 2020 2020  nd(.88,3720.    
-000051b0: 5068 6173 6520 7068 6173 6528 7f39 302c  Phase phase(.90,
-000051c0: 3337 3935 0a20 2020 2075 696e 7433 325f  3795.    uint32_
-000051d0: 7420 7128 7f39 322c 3338 3633 0a20 2020  t q(.92,3863.   
-000051e0: 2062 6f6f 6c20 7067 5f70 6861 7365 287f   bool pg_phase(.
-000051f0: 3934 2c33 3933 330a 2020 2020 626f 6f6c  94,3933.    bool
-00005200: 2070 675f 726f 6f74 287f 3936 2c34 3031   pg_root(.96,401
-00005210: 320a 2020 2020 626f 6f6c 2070 675f 6c65  2.    bool pg_le
-00005220: 6166 287f 3938 2c34 3038 390a 2020 2020  af(.98,4089.    
-00005230: 766f 6964 206b 696e 6428 7f31 3030 2c34  void kind(.100,4
-00005240: 3136 330a 2020 2020 766f 6964 2070 6861  163.    void pha
-00005250: 7365 287f 3130 322c 3432 3437 0a20 2020  se(.102,4247.   
-00005260: 2076 6f69 6420 7128 7f31 3034 2c34 3332   void q(.104,432
-00005270: 360a 2020 2020 766f 6964 2070 675f 7068  6.    void pg_ph
-00005280: 6173 6528 7f31 3036 2c34 3339 390a 2020  ase(.106,4399.  
-00005290: 2020 766f 6964 2070 675f 726f 6f74 287f    void pg_root(.
-000052a0: 3130 382c 3434 3935 0a20 2020 2076 6f69  108,4495.    voi
-000052b0: 6420 7067 5f6c 6561 6628 7f31 3130 2c34  d pg_leaf(.110,4
-000052c0: 3538 370a 2020 2020 7374 643a 3a73 7472  587.    std::str
-000052d0: 696e 6720 6b69 6e64 5f73 7472 287f 3131  ing kind_str(.11
-000052e0: 352c 3437 3537 0a20 2063 6c61 7373 205a  5,4757.  class Z
-000052f0: 5845 6467 657f 3133 322c 3531 3430 0a20  XEdge.132,5140. 
-00005300: 2020 205a 5845 6467 654b 696e 6420 6b69     ZXEdgeKind ki
-00005310: 6e64 5f3b 7f31 3335 2c35 3137 300a 2020  nd_;.135,5170.  
-00005320: 2020 7569 6e74 3332 5f74 2074 6f5f 3b7f    uint32_t to_;.
-00005330: 3133 362c 3532 3238 0a20 2020 205a 5845  136,5228.    ZXE
-00005340: 6467 6528 7f31 3433 2c35 3438 390a 2020  dge(.143,5489.  
-00005350: 2020 5a58 4564 6765 287f 3134 382c 3536    ZXEdge(.148,56
-00005360: 3838 0a20 2020 205a 5845 6467 654b 696e  88.    ZXEdgeKin
-00005370: 6420 6b69 6e64 287f 3135 302c 3537 3835  d kind(.150,5785
-00005380: 0a20 2020 2075 696e 7433 325f 7420 746f  .    uint32_t to
-00005390: 287f 3135 322c 3538 3537 0a20 2020 2076  (.152,5857.    v
-000053a0: 6f69 6420 6b69 6e64 287f 3135 342c 3539  oid kind(.154,59
-000053b0: 3235 0a20 2020 2076 6f69 6420 746f 287f  25.    void to(.
-000053c0: 3135 362c 3630 3036 0a20 2020 2073 7464  156,6006.    std
-000053d0: 3a3a 7374 7269 6e67 206b 696e 645f 7374  ::string kind_st
-000053e0: 7228 7f31 3631 2c36 3136 300a 2020 2020  r(.161,6160.    
-000053f0: 7374 643a 3a73 7472 696e 6720 6e61 6d65  std::string name
-00005400: 287f 3136 392c 3633 3837 0a20 2020 2076  (.169,6387.    v
-00005410: 6f69 6420 7265 7665 7273 655f 6b69 6e64  oid reverse_kind
-00005420: 287f 3138 312c 3637 3236 0a20 2063 6c61  (.181,6726.  cla
-00005430: 7373 205a 5844 6961 6772 616d 7f31 3938  ss ZXDiagram.198
-00005440: 2c37 3731 340a 2020 2020 5a58 4469 6167  ,7714.    ZXDiag
-00005450: 7261 6d4b 696e 6420 6b69 6e64 5f3b 7f32  ramKind kind_;.2
-00005460: 3031 2c37 3734 370a 2020 2020 7569 6e74  01,7747.    uint
-00005470: 3332 5f74 2071 7562 6974 5f6e 756d 5f3b  32_t qubit_num_;
-00005480: 7f32 3032 2c37 3830 300a 2020 2020 7374  .202,7800.    st
-00005490: 643a 3a76 6563 746f 723c 5a58 4e6f 6465  d::vector<ZXNode
-000054a0: 3e20 6e6f 6465 735f 3b7f 3230 332c 3738  > nodes_;.203,78
-000054b0: 3437 0a20 2020 2073 7464 3a3a 7665 6374  47.    std::vect
-000054c0: 6f72 3c75 696e 7433 325f 743e 2069 6e70  or<uint32_t> inp
-000054d0: 7574 735f 3b7f 3230 342c 3739 3133 0a20  uts_;.204,7913. 
-000054e0: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
-000054f0: 696e 7433 325f 743e 206f 7574 7075 7473  int32_t> outputs
-00005500: 5f3b 7f32 3035 2c37 3938 360a 2020 2020  _;.205,7986.    
-00005510: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
-00005520: 3a76 6563 746f 723c 5a58 4564 6765 3e3e  :vector<ZXEdge>>
-00005530: 2061 646a 5f6d 6174 5f3b 7f32 3036 2c38   adj_mat_;.206,8
-00005540: 3036 310a 2020 2020 7374 643a 3a76 6563  061.    std::vec
-00005550: 746f 723c 5a58 4e6f 6465 506c 6163 653e  tor<ZXNodePlace>
-00005560: 206e 6f64 655f 706c 6163 6573 5f3b 7f32   node_places_;.2
-00005570: 3037 2c38 3134 370a 2020 2020 7569 6e74  07,8147.    uint
-00005580: 3332 5f74 206d 6178 5f61 646a 5f6e 756d  32_t max_adj_num
-00005590: 287f 3231 312c 3833 3237 0a20 2020 2062  (.211,8327.    b
-000055a0: 6f6f 6c20 6368 6563 6b5f 785f 7370 6964  ool check_x_spid
-000055b0: 6572 287f 3232 342c 3837 3430 0a20 2020  er(.224,8740.   
-000055c0: 2062 6f6f 6c20 6368 6563 6b5f 7a5f 7370   bool check_z_sp
-000055d0: 6964 6572 287f 3233 302c 3930 3837 0a20  ider(.230,9087. 
-000055e0: 2020 2062 6f6f 6c20 6368 6563 6b5f 7a65     bool check_ze
-000055f0: 726f 5f70 6861 7365 5f73 7069 6465 7228  ro_phase_spider(
-00005600: 7f32 3336 2c39 3435 320a 2020 2020 626f  .236,9452.    bo
-00005610: 6f6c 2063 6865 636b 5f70 6175 6c69 5f73  ol check_pauli_s
-00005620: 7069 6465 7228 7f32 3437 2c39 3935 370a  pider(.247,9957.
-00005630: 2020 2020 626f 6f6c 2063 6865 636b 5f70      bool check_p
-00005640: 726f 7065 725f 636c 6966 666f 7264 5f73  roper_clifford_s
-00005650: 7069 6465 7228 7f32 3538 2c31 3035 3139  pider(.258,10519
-00005660: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-00005670: 636c 6966 666f 7264 5f73 7069 6465 7228  clifford_spider(
-00005680: 7f32 3639 2c31 3130 3831 0a20 2020 2062  .269,11081.    b
-00005690: 6f6f 6c20 6368 6563 6b5f 6e6f 6e5f 636c  ool check_non_cl
-000056a0: 6966 666f 7264 5f73 7069 6465 7228 7f32  ifford_spider(.2
-000056b0: 3738 2c31 3134 3930 0a20 2020 2062 6f6f  78,11490.    boo
-000056c0: 6c20 6368 6563 6b5f 696e 7465 726e 616c  l check_internal
-000056d0: 5f6e 6f64 6528 7f32 3834 2c31 3138 3335  _node(.284,11835
-000056e0: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-000056f0: 626f 756e 6461 7279 5f6e 6f64 6528 7f32  boundary_node(.2
-00005700: 3930 2c31 3231 3839 0a20 2020 2062 6f6f  90,12189.    boo
-00005710: 6c20 6368 6563 6b5f 7067 5f70 6861 7365  l check_pg_phase
-00005720: 5f6e 6f64 6528 7f32 3936 2c31 3235 3733  _node(.296,12573
-00005730: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-00005740: 7067 5f72 6f6f 745f 6e6f 6465 287f 3330  pg_root_node(.30
-00005750: 322c 3132 3933 350a 2020 2020 626f 6f6c  2,12935.    bool
-00005760: 2063 6865 636b 5f70 675f 6c65 6166 5f6e   check_pg_leaf_n
-00005770: 6f64 6528 7f33 3038 2c31 3332 3935 0a20  ode(.308,13295. 
-00005780: 2020 2062 6f6f 6c20 6368 6563 6b5f 7068     bool check_ph
-00005790: 6173 655f 6761 6467 6574 5f6e 6f64 6528  ase_gadget_node(
-000057a0: 7f33 3134 2c31 3336 3737 0a20 2020 2062  .314,13677.    b
-000057b0: 6f6f 6c20 6368 6563 6b5f 696e 7075 745f  ool check_input_
-000057c0: 6e6f 6465 287f 3332 312c 3134 3034 370a  node(.321,14047.
-000057d0: 2020 2020 626f 6f6c 2063 6865 636b 5f6f      bool check_o
-000057e0: 7574 7075 745f 6e6f 6465 287f 3332 372c  utput_node(.327,
-000057f0: 3134 3430 320a 2020 2020 626f 6f6c 2063  14402.    bool c
-00005800: 6865 636b 5f63 6f6e 6e65 6374 5f69 6e70  heck_connect_inp
-00005810: 7574 5f6e 6f64 6528 7f33 3333 2c31 3437  ut_node(.333,147
-00005820: 3639 0a20 2020 2062 6f6f 6c20 6368 6563  69.    bool chec
-00005830: 6b5f 636f 6e6e 6563 745f 6f75 7470 7574  k_connect_output
-00005840: 5f6e 6f64 6528 7f33 3435 2c31 3532 3232  _node(.345,15222
-00005850: 0a20 2020 2062 6f6f 6c20 6368 6563 6b5f  .    bool check_
-00005860: 636f 6e6e 6563 745f 7068 6173 655f 6761  connect_phase_ga
-00005870: 6467 6574 287f 3335 372c 3135 3731 310a  dget(.357,15711.
-00005880: 2020 2020 766f 6964 2072 656d 6f76 655f      void remove_
-00005890: 6564 6765 735f 6f66 5f6e 6f64 6528 7f33  edges_of_node(.3
-000058a0: 3932 2c31 3730 3537 0a20 2020 2075 696e  92,17057.    uin
-000058b0: 7433 325f 7420 6465 6772 6565 5f6f 665f  t32_t degree_of_
-000058c0: 6e6f 6465 287f 3430 392c 3137 3536 310a  node(.409,17561.
-000058d0: 2020 2020 5a58 4e6f 6465 4b69 6e64 206b      ZXNodeKind k
-000058e0: 696e 645f 6f66 5f6e 6f64 6528 7f34 3135  ind_of_node(.415
-000058f0: 2c31 3738 3035 0a20 2020 2073 7464 3a3a  ,17805.    std::
-00005900: 7665 6374 6f72 3c7f 7374 643a 3a76 6563  vector<.std::vec
-00005910: 746f 7201 3532 322c 3232 3430 390a 2020  tor.522,22409.  
-00005920: 2020 5a58 4469 6167 7261 6d28 7f35 3333    ZXDiagram(.533
-00005930: 2c32 3237 3739 0a20 2020 205a 5844 6961  ,22779.    ZXDia
-00005940: 6772 616d 4b69 6e64 206b 696e 6428 7f35  gramKind kind(.5
-00005950: 3338 2c32 3330 3233 0a20 2020 2075 696e  38,23023.    uin
-00005960: 7433 325f 7420 7175 6269 745f 6e75 6d28  t32_t qubit_num(
-00005970: 7f35 3430 2c32 3331 3035 0a20 2020 2073  .540,23105.    s
-00005980: 7464 3a3a 7665 6374 6f72 3c5a 584e 6f64  td::vector<ZXNod
-00005990: 653e 206e 6f64 6573 287f 3534 322c 3233  e> nodes(.542,23
-000059a0: 3138 380a 2020 2020 7374 643a 3a76 6563  188.    std::vec
-000059b0: 746f 723c 7569 6e74 3332 5f74 3e20 696e  tor<uint32_t> in
-000059c0: 7075 7473 287f 3534 342c 3233 3237 350a  puts(.544,23275.
-000059d0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
-000059e0: 7569 6e74 3332 5f74 3e20 6f75 7470 7574  uint32_t> output
-000059f0: 7328 7f35 3436 2c32 3333 3637 0a20 2020  s(.546,23367.   
-00005a00: 2073 7464 3a3a 7665 6374 6f72 3c73 7464   std::vector<std
-00005a10: 3a3a 7665 6374 6f72 3c5a 5845 6467 653e  ::vector<ZXEdge>
-00005a20: 3e20 6164 6a5f 6d61 7428 7f35 3438 2c32  > adj_mat(.548,2
-00005a30: 3334 3631 0a20 2020 2076 6f69 6420 6b69  3461.    void ki
-00005a40: 6e64 287f 3535 302c 3233 3536 330a 2020  nd(.550,23563.  
-00005a50: 2020 766f 6964 2071 7562 6974 5f6e 756d    void qubit_num
-00005a60: 287f 3535 322c 3233 3635 340a 2020 2020  (.552,23654.    
-00005a70: 766f 6964 206e 6f64 6573 287f 3535 342c  void nodes(.554,
-00005a80: 3233 3735 360a 2020 2020 766f 6964 2069  23756.    void i
-00005a90: 6e70 7574 7328 7f35 3536 2c32 3338 3535  nputs(.556,23855
-00005aa0: 0a20 2020 2076 6f69 6420 6f75 7470 7574  .    void output
-00005ab0: 7328 7f35 3538 2c32 3339 3631 0a20 2020  s(.558,23961.   
-00005ac0: 2076 6f69 6420 6164 6a5f 6d61 7428 7f35   void adj_mat(.5
-00005ad0: 3630 2c32 3430 3731 0a20 2020 2076 6f69  60,24071.    voi
-00005ae0: 6420 7368 6f77 287f 3537 302c 3234 3337  d show(.570,2437
-00005af0: 340a 2020 2020 7374 643a 3a6d 6170 3c7f  4.    std::map<.
-00005b00: 7374 643a 3a6d 6170 0135 3735 2c32 3435  std::map.575,245
-00005b10: 3336 0a20 2020 2075 696e 7433 325f 7420  36.    uint32_t 
-00005b20: 7370 6964 6572 5f63 6f75 6e74 287f 3538  spider_count(.58
-00005b30: 392c 3234 3933 360a 2020 2020 7569 6e74  9,24936.    uint
-00005b40: 3332 5f74 206e 6f6e 5f63 6c69 6666 6f72  32_t non_cliffor
-00005b50: 645f 636f 756e 7428 7f35 3933 2c32 3530  d_count(.593,250
-00005b60: 3838 0a20 2020 2066 7269 656e 6420 7374  88.    friend st
-00005b70: 643a 3a6f 7374 7265 616d 2620 6f70 6572  d::ostream& oper
-00005b80: 6174 6f72 3c3c 287f 3638 332c 3237 3932  ator<<(.683,2792
-00005b90: 380a 0c0a 6f70 7469 6d69 7a65 722e 682c  8...optimizer.h,
-00005ba0: 3132 3234 0a23 6465 6669 6e65 204f 5054  1224.#define OPT
-00005bb0: 494d 495a 4552 5f48 7f37 2c39 320a 2020  IMIZER_H.7,92.  
-00005bc0: 656e 756d 204f 7074 696d 697a 6572 4b69  enum OptimizerKi
-00005bd0: 6e64 207f 3139 2c32 3531 0a09 0920 2020  nd .19,251...   
-00005be0: 2020 205a 5843 616c 6375 6c75 732c 7f32     ZXCalculus,.2
-00005bf0: 302c 3237 340a 0909 2020 2020 2020 5068  0,274...      Ph
-00005c00: 6173 6550 6f6c 796e 6f6d 6961 6c20 7f32  asePolynomial .2
-00005c10: 312c 3331 370a 2020 636c 6173 7320 4f70  1,317.  class Op
-00005c20: 7469 6d69 7a65 727f 3238 2c34 3435 0a20  timizer.28,445. 
-00005c30: 2020 204f 7074 696d 697a 6572 4b69 6e64     OptimizerKind
-00005c40: 206b 696e 645f 3b7f 3331 2c34 3738 0a20   kind_;.31,478. 
-00005c50: 2020 2064 6f75 626c 6520 7072 6f63 5f74     double proc_t
-00005c60: 696d 655f 3b7f 3332 2c35 3336 0a20 2020  ime_;.32,536.   
-00005c70: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
-00005c80: 6d61 7001 3333 2c35 3830 0a20 2020 2073  map.33,580.    s
-00005c90: 7464 3a3a 6d61 703c 7374 643a 3a73 7472  td::map<std::str
-00005ca0: 696e 672c 2075 696e 7433 325f 743e 2073  ing, uint32_t> s
-00005cb0: 7461 7473 5f69 6e5f 3b7f 3333 2c35 3830  tats_in_;.33,580
-00005cc0: 0a20 2020 2073 7464 3a3a 6d61 703c 7f73  .    std::map<.s
-00005cd0: 7464 3a3a 6d61 7001 3334 2c36 3733 0a20  td::map.34,673. 
-00005ce0: 2020 2073 7464 3a3a 6d61 703c 7374 643a     std::map<std:
-00005cf0: 3a73 7472 696e 672c 2075 696e 7433 325f  :string, uint32_
-00005d00: 743e 2073 7461 7473 5f6f 7574 5f3b 7f33  t> stats_out_;.3
-00005d10: 342c 3637 330a 2020 2020 7374 643a 3a6d  4,673.    std::m
-00005d20: 6170 3c7f 7374 643a 3a6d 6170 0133 352c  ap<.std::map.35,
-00005d30: 3736 360a 2020 2020 7374 643a 3a6d 6170  766.    std::map
-00005d40: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
-00005d50: 6e74 3332 5f74 3e20 7a78 5f73 7461 7473  nt32_t> zx_stats
-00005d60: 5f69 6e5f 3b7f 3335 2c37 3636 0a20 2020  _in_;.35,766.   
-00005d70: 2073 7464 3a3a 6d61 703c 7f73 7464 3a3a   std::map<.std::
-00005d80: 6d61 7001 3336 2c38 3637 0a20 2020 2073  map.36,867.    s
-00005d90: 7464 3a3a 6d61 703c 7374 643a 3a73 7472  td::map<std::str
-00005da0: 696e 672c 2075 696e 7433 325f 743e 207a  ing, uint32_t> z
-00005db0: 785f 7374 6174 735f 6f75 745f 3b7f 3336  x_stats_out_;.36
-00005dc0: 2c38 3637 0a20 2020 204f 7074 696d 697a  ,867.    Optimiz
-00005dd0: 6572 4b69 6e64 206b 696e 6428 7f33 392c  erKind kind(.39,
-00005de0: 3130 3036 0a20 2020 2064 6f75 626c 6520  1006.    double 
-00005df0: 7072 6f63 5f74 696d 6528 7f34 312c 3130  proc_time(.41,10
-00005e00: 3838 0a20 2020 2064 6f75 626c 6520 6765  88.    double ge
-00005e10: 745f 7072 6f63 5f74 696d 6528 7f34 332c  t_proc_time(.43,
-00005e20: 3131 3733 0a20 2020 2073 7464 3a3a 6d61  1173.    std::ma
-00005e30: 703c 7f73 7464 3a3a 6d61 7001 3435 2c31  p<.std::map.45,1
-00005e40: 3236 310a 2020 2020 7374 643a 3a6d 6170  261.    std::map
-00005e50: 3c73 7464 3a3a 7374 7269 6e67 2c20 7569  <std::string, ui
-00005e60: 6e74 3332 5f74 3e20 7374 6174 735f 696e  nt32_t> stats_in
-00005e70: 287f 3435 2c31 3236 310a 2020 2020 7374  (.45,1261.    st
-00005e80: 643a 3a6d 6170 3c7f 7374 643a 3a6d 6170  d::map<.std::map
-00005e90: 0134 372c 3133 3733 0a20 2020 2073 7464  .47,1373.    std
-00005ea0: 3a3a 6d61 703c 7374 643a 3a73 7472 696e  ::map<std::strin
-00005eb0: 672c 2075 696e 7433 325f 743e 2073 7461  g, uint32_t> sta
-00005ec0: 7473 5f6f 7574 287f 3437 2c31 3337 330a  ts_out(.47,1373.
-00005ed0: 2020 2020 7374 643a 3a6d 6170 3c7f 7374      std::map<.st
-00005ee0: 643a 3a6d 6170 0134 392c 3134 3839 0a20  d::map.49,1489. 
-00005ef0: 2020 2073 7464 3a3a 6d61 703c 7374 643a     std::map<std:
-00005f00: 3a73 7472 696e 672c 2075 696e 7433 325f  :string, uint32_
-00005f10: 743e 207a 785f 7374 6174 735f 696e 287f  t> zx_stats_in(.
-00005f20: 3439 2c31 3438 390a 2020 2020 7374 643a  49,1489.    std:
-00005f30: 3a6d 6170 3c7f 7374 643a 3a6d 6170 0135  :map<.std::map.5
-00005f40: 312c 3136 3130 0a20 2020 2073 7464 3a3a  1,1610.    std::
-00005f50: 6d61 703c 7374 643a 3a73 7472 696e 672c  map<std::string,
-00005f60: 2075 696e 7433 325f 743e 207a 785f 7374   uint32_t> zx_st
-00005f70: 6174 735f 6f75 7428 7f35 312c 3136 3130  ats_out(.51,1610
-00005f80: 0a20 2020 2076 6f69 6420 6b69 6e64 287f  .    void kind(.
-00005f90: 3533 2c31 3732 350a 2020 2020 766f 6964  53,1725.    void
-00005fa0: 2070 726f 635f 7469 6d65 287f 3535 2c31   proc_time(.55,1
-00005fb0: 3831 360a 2020 2020 766f 6964 2073 7461  816.    void sta
-00005fc0: 7473 5f69 6e28 7f35 372c 3139 3139 0a20  ts_in(.57,1919. 
-00005fd0: 2020 2076 6f69 6420 7374 6174 735f 6f75     void stats_ou
-00005fe0: 7428 7f35 392c 3230 3435 0a20 2020 2076  t(.59,2045.    v
-00005ff0: 6f69 6420 7a78 5f73 7461 7473 5f69 6e28  oid zx_stats_in(
-00006000: 7f36 312c 3231 3736 0a20 2020 2076 6f69  .61,2176.    voi
-00006010: 6420 7a78 5f73 7461 7473 5f6f 7574 287f  d zx_stats_out(.
-00006020: 3633 2c32 3331 370a 2020 2020 766f 6964  63,2317.    void
-00006030: 2073 686f 7728 7f37 372c 3237 3734 0a20   show(.77,2774. 
-00006040: 2020 2066 7269 656e 6420 7374 643a 3a6f     friend std::o
-00006050: 7374 7265 616d 2620 6f70 6572 6174 6f72  stream& operator
-00006060: 3c3c 287f 3130 352c 3430 3639 0a0c 0a64  <<(.105,4069...d
-00006070: 6167 6564 6765 2e63 7070 2c34 360a 7374  agedge.cpp,46.st
-00006080: 643a 3a73 7472 696e 6720 5368 6172 7169  d::string Sharqi
-00006090: 743a 3a44 4147 4564 6765 3a3a 6e61 6d65  t::DAGEdge::name
-000060a0: 287f 6e61 6d65 0138 2c39 320a 0c0a 6461  (.name.8,92...da
-000060b0: 676e 6f64 652e 6370 702c 3436 0a73 7464  gnode.cpp,46.std
-000060c0: 3a3a 7374 7269 6e67 2053 6861 7271 6974  ::string Sharqit
-000060d0: 3a3a 4441 474e 6f64 653a 3a6e 616d 6528  ::DAGNode::name(
-000060e0: 7f6e 616d 6501 382c 3932 0a0c 0a6f 7074  .name.8,92...opt
-000060f0: 696d 697a 6572 2e63 7070 2c33 3537 0a73  imizer.cpp,357.s
-00006100: 7464 3a3a 7374 7269 6e67 2053 6861 7271  td::string Sharq
-00006110: 6974 3a3a 4f70 7469 6d69 7a65 723a 3a74  it::Optimizer::t
-00006120: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
-00006130: 696e 6701 382c 3130 320a 7374 643a 3a73  ing.8,102.std::s
-00006140: 7472 696e 6720 5368 6172 7169 743a 3a4f  tring Sharqit::O
-00006150: 7074 696d 697a 6572 3a3a 6e61 6d65 287f  ptimizer::name(.
-00006160: 6e61 6d65 0135 312c 3234 3930 0a53 6861  name.51,2490.Sha
-00006170: 7271 6974 3a3a 5143 6972 6320 5368 6172  rqit::QCirc Shar
-00006180: 7169 743a 3a4f 7074 696d 697a 6572 3a3a  qit::Optimizer::
-00006190: 7265 6475 6365 5f67 6174 6573 5f75 7369  reduce_gates_usi
-000061a0: 6e67 5f7a 7828 7f72 6564 7563 655f 6761  ng_zx(.reduce_ga
-000061b0: 7465 735f 7573 696e 675f 7a78 0136 322c  tes_using_zx.62,
-000061c0: 3238 3235 0a53 6861 7271 6974 3a3a 5143  2825.Sharqit::QC
-000061d0: 6972 6320 5368 6172 7169 743a 3a4f 7074  irc Sharqit::Opt
-000061e0: 696d 697a 6572 3a3a 7265 6475 6365 5f67  imizer::reduce_g
-000061f0: 6174 6573 5f75 7369 6e67 5f70 7028 7f72  ates_using_pp(.r
-00006200: 6564 7563 655f 6761 7465 735f 7573 696e  educe_gates_usin
-00006210: 675f 7070 0139 302c 3334 3830 0a53 6861  g_pp.90,3480.Sha
-00006220: 7271 6974 3a3a 5143 6972 6320 5368 6172  rqit::QCirc Shar
-00006230: 7169 743a 3a4f 7074 696d 697a 6572 3a3a  qit::Optimizer::
-00006240: 7265 6475 6365 5f67 6174 6573 287f 7265  reduce_gates(.re
-00006250: 6475 6365 5f67 6174 6573 0131 3132 2c34  duce_gates.112,4
-00006260: 3032 350a 0c0a 7167 6174 652e 682c 3135  025...qgate.h,15
-00006270: 3130 0a23 6465 6669 6e65 2051 4741 5445  10.#define QGATE
-00006280: 5f48 7f37 2c38 300a 2020 656e 756d 2051  _H.7,80.  enum Q
-00006290: 4761 7465 4b69 6e64 207f 3139 2c32 3431  GateKind .19,241
-000062a0: 0a09 0920 2058 2c7f 3230 2c32 3630 0a09  ...  X,.20,260..
-000062b0: 0920 205a 2c7f 3231 2c32 3835 0a09 0920  .  Z,.21,285... 
-000062c0: 2053 2c7f 3232 2c33 3130 0a09 0920 2053   S,.22,310...  S
-000062d0: 6467 2c7f 3233 2c33 3239 0a09 0920 2054  dg,.23,329...  T
-000062e0: 2c7f 3234 2c33 3834 0a09 0920 2054 6467  ,.24,384...  Tdg
-000062f0: 2c7f 3235 2c34 3033 0a09 0920 2048 2c7f  ,.25,403...  H,.
-00006300: 3236 2c34 3538 0a09 0920 2052 5a2c 7f32  26,458...  RZ,.2
-00006310: 372c 3438 380a 0909 2020 4358 2c7f 3238  7,488...  CX,.28
-00006320: 2c35 3039 0a09 0920 2043 5a2c 7f32 392c  ,509...  CZ,.29,
-00006330: 3533 320a 0909 2020 4343 582c 7f33 302c  532...  CCX,.30,
-00006340: 3535 330a 0909 2020 4343 5a2c 7f33 312c  553...  CCZ,.31,
-00006350: 3537 360a 0909 2020 4964 2c7f 3332 2c35  576...  Id,.32,5
-00006360: 3939 0a09 0920 2049 6432 2c7f 3333 2c36  99...  Id2,.33,6
-00006370: 3339 0a20 2063 6c61 7373 2051 4761 7465  39.  class QGate
-00006380: 7f34 302c 3733 370a 2020 2020 5147 6174  .40,737.    QGat
-00006390: 654b 696e 6420 6b69 6e64 5f3b 7f34 332c  eKind kind_;.43,
-000063a0: 3736 360a 2020 2020 7374 643a 3a76 6563  766.    std::vec
-000063b0: 746f 723c 7569 6e74 3332 5f74 3e20 7169  tor<uint32_t> qi
-000063c0: 645f 3b7f 3434 2c38 3133 0a20 2020 2050  d_;.44,813.    P
-000063d0: 6861 7365 2070 6861 7365 5f3b 7f34 352c  hase phase_;.45,
-000063e0: 3837 340a 2020 2020 7374 643a 3a76 6563  874.    std::vec
-000063f0: 746f 723c 7374 643a 3a76 6563 746f 723c  tor<std::vector<
-00006400: 7374 643a 3a63 6f6d 706c 6578 3c64 6f75  std::complex<dou
-00006410: 626c 653e 3e3e 206f 705f 3b7f 3436 2c39  ble>>> op_;.46,9
-00006420: 3230 0a20 2020 2051 4761 7465 287f 3732  20.    QGate(.72
-00006430: 2c32 3035 380a 2020 2020 5147 6174 654b  ,2058.    QGateK
-00006440: 696e 6420 6b69 6e64 287f 3734 2c32 3139  ind kind(.74,219
-00006450: 360a 2020 2020 7374 643a 3a76 6563 746f  6.    std::vecto
-00006460: 723c 7569 6e74 3332 5f74 3e20 7169 6428  r<uint32_t> qid(
-00006470: 7f37 362c 3232 3638 0a20 2020 2050 6861  .76,2268.    Pha
-00006480: 7365 2070 6861 7365 287f 3738 2c32 3335  se phase(.78,235
-00006490: 320a 2020 2020 5068 6173 6520 6765 745f  2.    Phase get_
-000064a0: 7068 6173 6528 7f38 302c 3234 3234 0a20  phase(.80,2424. 
-000064b0: 2020 2073 7464 3a3a 7665 6374 6f72 3c73     std::vector<s
-000064c0: 7464 3a3a 7665 6374 6f72 3c73 7464 3a3a  td::vector<std::
-000064d0: 636f 6d70 6c65 783c 646f 7562 6c65 3e3e  complex<double>>
-000064e0: 3e20 6f70 287f 3832 2c32 3439 370a 2020  > op(.82,2497.  
-000064f0: 2020 766f 6964 206b 696e 6428 7f38 342c    void kind(.84,
-00006500: 3236 3033 0a20 2020 2076 6f69 6420 7169  2603.    void qi
-00006510: 6428 7f38 362c 3236 3834 0a20 2020 2076  d(.86,2684.    v
-00006520: 6f69 6420 7068 6173 6528 7f38 382c 3237  oid phase(.88,27
-00006530: 3736 0a20 2020 2076 6f69 6420 6f70 287f  76.    void op(.
-00006540: 3930 2c32 3835 370a 2020 2020 7569 6e74  90,2857.    uint
-00006550: 3332 5f74 2071 7562 6974 5f6e 756d 287f  32_t qubit_num(.
-00006560: 3130 372c 3334 3836 0a20 2020 2062 6f6f  107,3486.    boo
-00006570: 6c20 6973 5f49 645f 6761 7465 287f 3131  l is_Id_gate(.11
-00006580: 322c 3336 3830 0a20 2020 2062 6f6f 6c20  2,3680.    bool 
-00006590: 6973 5f49 6432 5f67 6174 6528 7f31 3137  is_Id2_gate(.117
-000065a0: 2c33 3837 380a 2020 2020 626f 6f6c 2069  ,3878.    bool i
-000065b0: 735f 585f 6761 7465 287f 3132 322c 3430  s_X_gate(.122,40
-000065c0: 3535 0a20 2020 2062 6f6f 6c20 6973 5f5a  55.    bool is_Z
-000065d0: 5f67 6174 6528 7f31 3237 2c34 3235 350a  _gate(.127,4255.
-000065e0: 2020 2020 626f 6f6c 2069 735f 485f 6761      bool is_H_ga
-000065f0: 7465 287f 3133 372c 3435 3433 0a20 2020  te(.137,4543.   
-00006600: 2062 6f6f 6c20 6973 5f53 5f67 6174 6528   bool is_S_gate(
-00006610: 7f31 3432 2c34 3735 300a 2020 2020 626f  .142,4750.    bo
-00006620: 6f6c 2069 735f 5331 5f67 6174 6528 7f31  ol is_S1_gate(.1
-00006630: 3535 2c35 3134 370a 2020 2020 626f 6f6c  55,5147.    bool
-00006640: 2069 735f 5333 5f67 6174 6528 7f31 3636   is_S3_gate(.166
-00006650: 2c35 3438 300a 2020 2020 626f 6f6c 2069  ,5480.    bool i
-00006660: 735f 545f 6761 7465 287f 3137 372c 3538  s_T_gate(.177,58
-00006670: 3238 0a20 2020 2062 6f6f 6c20 6973 5f54  28.    bool is_T
-00006680: 315f 6761 7465 287f 3139 302c 3632 3235  1_gate(.190,6225
-00006690: 0a20 2020 2062 6f6f 6c20 6973 5f54 375f  .    bool is_T7_
-000066a0: 6761 7465 287f 3230 332c 3635 3735 0a20  gate(.203,6575. 
-000066b0: 2020 2062 6f6f 6c20 6973 5f43 585f 6761     bool is_CX_ga
-000066c0: 7465 287f 3231 362c 3639 3033 0a20 2020  te(.216,6903.   
-000066d0: 2062 6f6f 6c20 6973 5f43 5a5f 6761 7465   bool is_CZ_gate
-000066e0: 287f 3232 312c 3730 3638 0a20 2020 2062  (.221,7068.    b
-000066f0: 6f6f 6c20 6973 5f43 4358 5f67 6174 6528  ool is_CCX_gate(
-00006700: 7f32 3236 2c37 3233 350a 2020 2020 626f  .226,7235.    bo
-00006710: 6f6c 2069 735f 4343 5a5f 6761 7465 287f  ol is_CCZ_gate(.
-00006720: 3233 312c 3734 3034 0a20 2020 2062 6f6f  231,7404.    boo
-00006730: 6c20 6973 5f52 5a5f 6761 7465 287f 3233  l is_RZ_gate(.23
-00006740: 362c 3735 3731 0a20 2020 2062 6f6f 6c20  6,7571.    bool 
-00006750: 6973 5f70 6175 6c69 5f67 6174 6528 7f32  is_pauli_gate(.2
-00006760: 3433 2c37 3931 370a 2020 2020 626f 6f6c  43,7917.    bool
-00006770: 2069 735f 7072 6f70 6572 5f63 6c69 6666   is_proper_cliff
-00006780: 6f72 645f 6761 7465 287f 3234 382c 3831  ord_gate(.248,81
-00006790: 3331 0a20 2020 2062 6f6f 6c20 6973 5f63  31.    bool is_c
-000067a0: 6c69 6666 6f72 645f 6761 7465 287f 3235  lifford_gate(.25
-000067b0: 332c 3833 3038 0a20 2020 2062 6f6f 6c20  3,8308.    bool 
-000067c0: 6973 5f6e 6f6e 5f63 6c69 6666 6f72 645f  is_non_clifford_
-000067d0: 6761 7465 287f 3235 382c 3835 3337 0a20  gate(.258,8537. 
-000067e0: 2020 2062 6f6f 6c20 6973 5f69 6e63 6c75     bool is_inclu
-000067f0: 6465 6428 7f32 3634 2c38 3736 320a 2020  ded(.264,8762.  
-00006800: 2020 7374 6174 6963 2073 7464 3a3a 7475    static std::tu
-00006810: 706c 653c 7f73 7464 3a3a 7475 706c 6501  ple<.std::tuple.
-00006820: 3330 382c 3130 3238 320a 2020 2020 6672  308,10282.    fr
-00006830: 6965 6e64 2073 7464 3a3a 6f73 7472 6561  iend std::ostrea
-00006840: 6d26 206f 7065 7261 746f 723c 3c28 7f33  m& operator<<(.3
-00006850: 3039 2c31 3033 3538 0a0c 0a66 7261 6374  09,10358...fract
-00006860: 696f 6e2e 6370 702c 3537 0a73 7464 3a3a  ion.cpp,57.std::
-00006870: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
-00006880: 4672 6163 7469 6f6e 3a3a 746f 5f73 7472  Fraction::to_str
-00006890: 696e 6728 7f74 6f5f 7374 7269 6e67 0138  ing(.to_string.8
-000068a0: 2c39 390a                                ,99.
+00001520: 633a 3a61 6464 5f71 6761 7465 287f 6164  c::add_qgate(.ad
+00001530: 645f 7167 6174 6501 3239 302c 3830 3430  d_qgate.290,8040
+00001540: 0a53 6861 7271 6974 3a3a 5143 6972 6326  .Sharqit::QCirc&
+00001550: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+00001560: 3a61 6464 5f71 6761 7465 287f 6164 645f  :add_qgate(.add_
+00001570: 7167 6174 6501 3330 332c 3834 3039 0a53  qgate.303,8409.S
+00001580: 6861 7271 6974 3a3a 5143 6972 6326 2053  harqit::QCirc& S
+00001590: 6861 7271 6974 3a3a 5143 6972 633a 3a61  harqit::QCirc::a
+000015a0: 6464 5f71 6369 7263 287f 6164 645f 7163  dd_qcirc(.add_qc
+000015b0: 6972 6301 3332 302c 3930 3338 0a53 6861  irc.320,9038.Sha
+000015c0: 7271 6974 3a3a 5143 6972 6326 2053 6861  rqit::QCirc& Sha
+000015d0: 7271 6974 3a3a 5143 6972 633a 3a61 6464  rqit::QCirc::add
+000015e0: 5f72 616e 646f 6d28 7f61 6464 5f72 616e  _random(.add_ran
+000015f0: 646f 6d01 3332 382c 3931 3834 0a53 6861  dom.328,9184.Sha
+00001600: 7271 6974 3a3a 5143 6972 6326 2053 6861  rqit::QCirc& Sha
+00001610: 7271 6974 3a3a 5143 6972 633a 3a61 6464  rqit::QCirc::add
+00001620: 5f72 616e 646f 6d5f 7374 7228 7f61 6464  _random_str(.add
+00001630: 5f72 616e 646f 6d5f 7374 7201 3431 392c  _random_str.419,
+00001640: 3132 3534 310a 5368 6172 7169 743a 3a51  12541.Sharqit::Q
+00001650: 4369 7263 2053 6861 7271 6974 3a3a 5143  Circ Sharqit::QC
+00001660: 6972 633a 3a72 6576 6572 7365 287f 7265  irc::reverse(.re
+00001670: 7665 7273 6501 3433 332c 3133 3038 330a  verse.433,13083.
+00001680: 5368 6172 7169 743a 3a51 4369 7263 2053  Sharqit::QCirc S
+00001690: 6861 7271 6974 3a3a 5143 6972 633a 3a69  harqit::QCirc::i
+000016a0: 6e76 6572 7365 287f 696e 7665 7273 6501  nverse(.inverse.
+000016b0: 3434 332c 3133 3330 330a 626f 6f6c 2053  443,13303.bool S
+000016c0: 6861 7271 6974 3a3a 5143 6972 633a 3a69  harqit::QCirc::i
+000016d0: 735f 6964 656e 7469 6361 6c28 7f69 735f  s_identical(.is_
+000016e0: 6964 656e 7469 6361 6c01 3435 332c 3133  identical.453,13
+000016f0: 3533 330a 626f 6f6c 2053 6861 7271 6974  533.bool Sharqit
+00001700: 3a3a 5143 6972 633a 3a69 735f 6571 7561  ::QCirc::is_equa
+00001710: 6c28 7f69 735f 6571 7561 6c01 3436 322c  l(.is_equal.462,
+00001720: 3133 3737 360a 766f 6964 2053 6861 7271  13776.void Sharq
+00001730: 6974 3a3a 5143 6972 633a 3a74 6f5f 646f  it::QCirc::to_do
+00001740: 745f 6669 6c65 287f 746f 5f64 6f74 5f66  t_file(.to_dot_f
+00001750: 696c 6501 3439 392c 3134 3935 310a 766f  ile.499,14951.vo
+00001760: 6964 2053 6861 7271 6974 3a3a 5143 6972  id Sharqit::QCir
+00001770: 633a 3a74 6f5f 7376 675f 6669 6c65 287f  c::to_svg_file(.
+00001780: 746f 5f73 7667 5f66 696c 6501 3831 382c  to_svg_file.818,
+00001790: 3237 3037 360a 5368 6172 7169 743a 3a5a  27076.Sharqit::Z
+000017a0: 5844 6961 6772 616d 2053 6861 7271 6974  XDiagram Sharqit
+000017b0: 3a3a 5143 6972 633a 3a74 6f5f 7a78 6469  ::QCirc::to_zxdi
+000017c0: 6167 7261 6d28 7f74 6f5f 7a78 6469 6167  agram(.to_zxdiag
+000017d0: 7261 6d01 3833 302c 3237 3534 320a 5368  ram.830,27542.Sh
+000017e0: 6172 7169 743a 3a4c 696e 6561 724d 6170  arqit::LinearMap
+000017f0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+00001800: 3a74 6f5f 6c69 6e65 6172 6d61 7028 7f74  :to_linearmap(.t
+00001810: 6f5f 6c69 6e65 6172 6d61 7001 3836 382c  o_linearmap.868,
+00001820: 3238 3436 370a 5368 6172 7169 743a 3a44  28467.Sharqit::D
+00001830: 4147 4369 7263 2053 6861 7271 6974 3a3a  AGCirc Sharqit::
+00001840: 5143 6972 633a 3a74 6f5f 6461 6763 6972  QCirc::to_dagcir
+00001850: 6328 7f74 6f5f 6461 6763 6972 6301 3838  c(.to_dagcirc.88
+00001860: 382c 3238 3834 330a 766f 6964 2053 6861  8,28843.void Sha
+00001870: 7271 6974 3a3a 5143 6972 633a 3a63 7a5f  rqit::QCirc::cz_
+00001880: 746f 5f63 7828 7f63 7a5f 746f 5f63 7801  to_cx(.cz_to_cx.
+00001890: 3839 392c 3239 3037 390a 5368 6172 7169  899,29079.Sharqi
+000018a0: 743a 3a51 4369 7263 2620 5368 6172 7169  t::QCirc& Sharqi
+000018b0: 743a 3a51 4369 7263 3a3a 6363 785f 6465  t::QCirc::ccx_de
+000018c0: 636f 6d70 287f 6363 785f 6465 636f 6d70  comp(.ccx_decomp
+000018d0: 0139 3137 2c32 3936 3534 0a53 6861 7271  .917,29654.Sharq
+000018e0: 6974 3a3a 5143 6972 6326 2053 6861 7271  it::QCirc& Sharq
+000018f0: 6974 3a3a 5143 6972 633a 3a63 637a 5f64  it::QCirc::ccz_d
+00001900: 6563 6f6d 7028 7f63 637a 5f64 6563 6f6d  ecomp(.ccz_decom
+00001910: 7001 3935 362c 3330 3931 340a 766f 6964  p.956,30914.void
+00001920: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+00001930: 3a64 6563 6f6d 705f 746f 6628 7f64 6563  :decomp_tof(.dec
+00001940: 6f6d 705f 746f 6601 3938 372c 3332 3037  omp_tof.987,3207
+00001950: 380a 626f 6f6c 2053 6861 7271 6974 3a3a  8.bool Sharqit::
+00001960: 5143 6972 633a 3a69 6e63 6c75 6465 5f74  QCirc::include_t
+00001970: 6f66 287f 696e 636c 7564 655f 746f 6601  of(.include_tof.
+00001980: 3130 3135 2c33 3237 3737 0a76 6f69 6420  1015,32777.void 
+00001990: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+000019a0: 7265 6d6f 7665 5f69 6428 7f72 656d 6f76  remove_id(.remov
+000019b0: 655f 6964 0131 3032 362c 3333 3132 310a  e_id.1026,33121.
+000019c0: 766f 6964 2020 5368 6172 7169 743a 3a51  void  Sharqit::Q
+000019d0: 4369 7263 3a3a 7265 706c 6163 655f 7769  Circ::replace_wi
+000019e0: 7468 5f72 7a28 7f72 6570 6c61 6365 5f77  th_rz(.replace_w
+000019f0: 6974 685f 727a 0131 3034 302c 3333 3636  ith_rz.1040,3366
+00001a00: 380a 0c0a 7068 6173 652e 6370 702c 3930  8...phase.cpp,90
+00001a10: 0a53 6861 7271 6974 3a3a 5068 6173 653a  .Sharqit::Phase:
+00001a20: 3a50 6861 7365 287f 5068 6173 6501 382c  :Phase(.Phase.8,
+00001a30: 3930 0a73 7464 3a3a 7374 7269 6e67 2053  90.std::string S
+00001a40: 6861 7271 6974 3a3a 5068 6173 653a 3a74  harqit::Phase::t
+00001a50: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
+00001a60: 696e 6701 3331 2c37 3434 0a0c 0a6d 6572  ing.31,744...mer
+00001a70: 6765 5f72 6f74 6174 696f 6e2e 6370 702c  ge_rotation.cpp,
+00001a80: 3230 390a 626f 6f6c 2053 6861 7271 6974  209.bool Sharqit
+00001a90: 3a3a 5143 6972 633a 3a69 735f 7465 726d  ::QCirc::is_term
+00001aa0: 696e 6174 696f 6e5f 626f 7264 6572 287f  ination_border(.
+00001ab0: 6973 5f74 6572 6d69 6e61 7469 6f6e 5f62  is_termination_b
+00001ac0: 6f72 6465 7201 382c 3134 380a 766f 6964  order.8,148.void
+00001ad0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+00001ae0: 3a6d 6572 6765 5f72 6f74 6174 696f 6e5f  :merge_rotation_
+00001af0: 6f6e 655f 7469 6d65 287f 6d65 7267 655f  one_time(.merge_
+00001b00: 726f 7461 7469 6f6e 5f6f 6e65 5f74 696d  rotation_one_tim
+00001b10: 6501 3138 2c34 3132 0a76 6f69 6420 5368  e.18,412.void Sh
+00001b20: 6172 7169 743a 3a51 4369 7263 3a3a 6d65  arqit::QCirc::me
+00001b30: 7267 655f 726f 7461 7469 6f6e 287f 6d65  rge_rotation(.me
+00001b40: 7267 655f 726f 7461 7469 6f6e 0138 322c  rge_rotation.82,
+00001b50: 3236 3031 0a0c 0a62 6163 6b75 702f 7163  2601...backup/qc
+00001b60: 6972 635f 626b 3230 3234 3034 3031 2e63  irc_bk20240401.c
+00001b70: 7070 2c32 3033 320a 766f 6964 2053 6861  pp,2032.void Sha
+00001b80: 7271 6974 3a3a 5143 6972 633a 3a73 6176  rqit::QCirc::sav
+00001b90: 6528 7f73 6176 6501 382c 3939 0a76 6f69  e(.save.8,99.voi
+00001ba0: 6420 5368 6172 7169 743a 3a51 4369 7263  d Sharqit::QCirc
+00001bb0: 3a3a 6c6f 6164 287f 6c6f 6164 0132 302c  ::load(.load.20,
+00001bc0: 3331 360a 7374 643a 3a6d 6170 3c73 7464  316.std::map<std
+00001bd0: 3a3a 7374 7269 6e67 2c20 7569 6e74 3332  ::string, uint32
+00001be0: 5f74 3e20 5368 6172 7169 743a 3a51 4369  _t> Sharqit::QCi
+00001bf0: 7263 3a3a 7374 6174 7328 7f73 7461 7473  rc::stats(.stats
+00001c00: 0136 372c 3135 3832 0a76 6f69 6420 5368  .67,1582.void Sh
+00001c10: 6172 7169 743a 3a51 4369 7263 3a3a 7072  arqit::QCirc::pr
+00001c20: 696e 745f 7374 6174 7328 7f70 7269 6e74  int_stats(.print
+00001c30: 5f73 7461 7473 0131 3035 2c32 3639 320a  _stats.105,2692.
+00001c40: 7569 6e74 3332 5f74 2053 6861 7271 6974  uint32_t Sharqit
+00001c50: 3a3a 5143 6972 633a 3a69 645f 636f 756e  ::QCirc::id_coun
+00001c60: 7428 7f69 645f 636f 756e 7401 3132 312c  t(.id_count.121,
+00001c70: 3334 3836 0a75 696e 7433 325f 7420 5368  3486.uint32_t Sh
+00001c80: 6172 7169 743a 3a51 4369 7263 3a3a 785f  arqit::QCirc::x_
+00001c90: 636f 756e 7428 7f78 5f63 6f75 6e74 0131  count(.x_count.1
+00001ca0: 3238 2c33 3632 360a 7569 6e74 3332 5f74  28,3626.uint32_t
+00001cb0: 2053 6861 7271 6974 3a3a 5143 6972 633a   Sharqit::QCirc:
+00001cc0: 3a7a 5f63 6f75 6e74 287f 7a5f 636f 756e  :z_count(.z_coun
+00001cd0: 7401 3133 352c 3337 3634 0a75 696e 7433  t.135,3764.uint3
+00001ce0: 325f 7420 5368 6172 7169 743a 3a51 4369  2_t Sharqit::QCi
+00001cf0: 7263 3a3a 685f 636f 756e 7428 7f68 5f63  rc::h_count(.h_c
+00001d00: 6f75 6e74 0131 3432 2c33 3930 320a 7569  ount.142,3902.ui
+00001d10: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
+00001d20: 5143 6972 633a 3a73 5f63 6f75 6e74 287f  QCirc::s_count(.
+00001d30: 735f 636f 756e 7401 3134 392c 3430 3430  s_count.149,4040
+00001d40: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+00001d50: 743a 3a51 4369 7263 3a3a 745f 636f 756e  t::QCirc::t_coun
+00001d60: 7428 7f74 5f63 6f75 6e74 0131 3536 2c34  t(.t_count.156,4
+00001d70: 3137 380a 7569 6e74 3332 5f74 2053 6861  178.uint32_t Sha
+00001d80: 7271 6974 3a3a 5143 6972 633a 3a72 7a5f  rqit::QCirc::rz_
+00001d90: 636f 756e 7428 7f72 7a5f 636f 756e 7401  count(.rz_count.
+00001da0: 3136 332c 3433 3136 0a75 696e 7433 325f  163,4316.uint32_
+00001db0: 7420 5368 6172 7169 743a 3a51 4369 7263  t Sharqit::QCirc
+00001dc0: 3a3a 6378 5f63 6f75 6e74 287f 6378 5f63  ::cx_count(.cx_c
+00001dd0: 6f75 6e74 0131 3730 2c34 3435 360a 7569  ount.170,4456.ui
+00001de0: 6e74 3332 5f74 2053 6861 7271 6974 3a3a  nt32_t Sharqit::
+00001df0: 5143 6972 633a 3a63 7a5f 636f 756e 7428  QCirc::cz_count(
+00001e00: 7f63 7a5f 636f 756e 7401 3137 372c 3435  .cz_count.177,45
+00001e10: 3936 0a75 696e 7433 325f 7420 5368 6172  96.uint32_t Shar
+00001e20: 7169 743a 3a51 4369 7263 3a3a 6363 785f  qit::QCirc::ccx_
+00001e30: 636f 756e 7428 7f63 6378 5f63 6f75 6e74  count(.ccx_count
+00001e40: 0131 3834 2c34 3733 360a 7569 6e74 3332  .184,4736.uint32
+00001e50: 5f74 2053 6861 7271 6974 3a3a 5143 6972  _t Sharqit::QCir
+00001e60: 633a 3a63 637a 5f63 6f75 6e74 287f 6363  c::ccz_count(.cc
+00001e70: 7a5f 636f 756e 7401 3139 312c 3438 3738  z_count.191,4878
+00001e80: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+00001e90: 743a 3a51 4369 7263 3a3a 6465 7074 6828  t::QCirc::depth(
+00001ea0: 7f64 6570 7468 0131 3938 2c35 3032 300a  .depth.198,5020.
+00001eb0: 7374 643a 3a73 7472 696e 6720 5368 6172  std::string Shar
+00001ec0: 7169 743a 3a51 4369 7263 3a3a 746f 5f73  qit::QCirc::to_s
+00001ed0: 7472 696e 6728 7f74 6f5f 7374 7269 6e67  tring(.to_string
+00001ee0: 0132 3232 2c35 3533 320a 5368 6172 7169  .222,5532.Sharqi
+00001ef0: 743a 3a51 4369 7263 2620 5368 6172 7169  t::QCirc& Sharqi
+00001f00: 743a 3a51 4369 7263 3a3a 6164 645f 7167  t::QCirc::add_qg
+00001f10: 6174 6528 7f61 6464 5f71 6761 7465 0134  ate(.add_qgate.4
+00001f20: 3038 2c31 3134 3134 0a53 6861 7271 6974  08,11414.Sharqit
+00001f30: 3a3a 5143 6972 6326 2053 6861 7271 6974  ::QCirc& Sharqit
+00001f40: 3a3a 5143 6972 633a 3a61 6464 5f71 6761  ::QCirc::add_qga
+00001f50: 7465 287f 6164 645f 7167 6174 6501 3431  te(.add_qgate.41
+00001f60: 382c 3131 3632 370a 5368 6172 7169 743a  8,11627.Sharqit:
+00001f70: 3a51 4369 7263 2620 5368 6172 7169 743a  :QCirc& Sharqit:
+00001f80: 3a51 4369 7263 3a3a 6164 645f 7163 6972  :QCirc::add_qcir
+00001f90: 6328 7f61 6464 5f71 6369 7263 0134 3330  c(.add_qcirc.430
+00001fa0: 2c31 3139 3336 0a53 6861 7271 6974 3a3a  ,11936.Sharqit::
+00001fb0: 5143 6972 6326 2053 6861 7271 6974 3a3a  QCirc& Sharqit::
+00001fc0: 5143 6972 633a 3a61 6464 5f72 616e 646f  QCirc::add_rando
+00001fd0: 6d28 7f61 6464 5f72 616e 646f 6d01 3433  m(.add_random.43
+00001fe0: 382c 3132 3038 320a 5368 6172 7169 743a  8,12082.Sharqit:
+00001ff0: 3a51 4369 7263 2620 5368 6172 7169 743a  :QCirc& Sharqit:
+00002000: 3a51 4369 7263 3a3a 6164 645f 7261 6e64  :QCirc::add_rand
+00002010: 6f6d 5f73 7472 287f 6164 645f 7261 6e64  om_str(.add_rand
+00002020: 6f6d 5f73 7472 0135 3130 2c31 3435 3137  om_str.510,14517
+00002030: 0a53 6861 7271 6974 3a3a 5143 6972 6320  .Sharqit::QCirc 
+00002040: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+00002050: 7265 7665 7273 6528 7f72 6576 6572 7365  reverse(.reverse
+00002060: 0135 3234 2c31 3530 3539 0a53 6861 7271  .524,15059.Sharq
+00002070: 6974 3a3a 5143 6972 6320 5368 6172 7169  it::QCirc Sharqi
+00002080: 743a 3a51 4369 7263 3a3a 696e 7665 7273  t::QCirc::invers
+00002090: 6528 7f69 6e76 6572 7365 0135 3334 2c31  e(.inverse.534,1
+000020a0: 3532 3739 0a62 6f6f 6c20 5368 6172 7169  5279.bool Sharqi
+000020b0: 743a 3a51 4369 7263 3a3a 6973 5f69 6465  t::QCirc::is_ide
+000020c0: 6e74 6963 616c 287f 6973 5f69 6465 6e74  ntical(.is_ident
+000020d0: 6963 616c 0135 3434 2c31 3535 3039 0a62  ical.544,15509.b
+000020e0: 6f6f 6c20 5368 6172 7169 743a 3a51 4369  ool Sharqit::QCi
+000020f0: 7263 3a3a 6973 5f65 7175 616c 287f 6973  rc::is_equal(.is
+00002100: 5f65 7175 616c 0135 3836 2c31 3637 3938  _equal.586,16798
+00002110: 0a76 6f69 6420 5368 6172 7169 743a 3a51  .void Sharqit::Q
+00002120: 4369 7263 3a3a 746f 5f64 6f74 5f66 696c  Circ::to_dot_fil
+00002130: 6528 7f74 6f5f 646f 745f 6669 6c65 0135  e(.to_dot_file.5
+00002140: 3936 2c31 3731 3233 0a76 6f69 6420 5368  96,17123.void Sh
+00002150: 6172 7169 743a 3a51 4369 7263 3a3a 746f  arqit::QCirc::to
+00002160: 5f73 7667 5f66 696c 6528 7f74 6f5f 7376  _svg_file(.to_sv
+00002170: 675f 6669 6c65 0138 3033 2c32 3431 3437  g_file.803,24147
+00002180: 0a53 6861 7271 6974 3a3a 5a58 4469 6167  .Sharqit::ZXDiag
+00002190: 7261 6d20 5368 6172 7169 743a 3a51 4369  ram Sharqit::QCi
+000021a0: 7263 3a3a 746f 5f7a 7864 6961 6772 616d  rc::to_zxdiagram
+000021b0: 287f 746f 5f7a 7864 6961 6772 616d 0138  (.to_zxdiagram.8
+000021c0: 3135 2c32 3436 3133 0a53 6861 7271 6974  15,24613.Sharqit
+000021d0: 3a3a 4c69 6e65 6172 4d61 7020 5368 6172  ::LinearMap Shar
+000021e0: 7169 743a 3a51 4369 7263 3a3a 746f 5f6c  qit::QCirc::to_l
+000021f0: 696e 6561 726d 6170 287f 746f 5f6c 696e  inearmap(.to_lin
+00002200: 6561 726d 6170 0138 3731 2c32 3630 3532  earmap.871,26052
+00002210: 0a53 6861 7271 6974 3a3a 4441 4743 6972  .Sharqit::DAGCir
+00002220: 6320 5368 6172 7169 743a 3a51 4369 7263  c Sharqit::QCirc
+00002230: 3a3a 746f 5f64 6167 6369 7263 287f 746f  ::to_dagcirc(.to
+00002240: 5f64 6167 6369 7263 0139 3030 2c32 3636  _dagcirc.900,266
+00002250: 3431 0a76 6f69 6420 5368 6172 7169 743a  41.void Sharqit:
+00002260: 3a51 4369 7263 3a3a 637a 5f74 6f5f 6378  :QCirc::cz_to_cx
+00002270: 287f 637a 5f74 6f5f 6378 0139 3137 2c32  (.cz_to_cx.917,2
+00002280: 3639 3837 0a76 6f69 6420 5368 6172 7169  6987.void Sharqi
+00002290: 743a 3a51 4369 7263 3a3a 6465 636f 6d70  t::QCirc::decomp
+000022a0: 5f74 6f66 287f 6465 636f 6d70 5f74 6f66  _tof(.decomp_tof
+000022b0: 0139 3335 2c32 3735 3632 0a62 6f6f 6c20  .935,27562.bool 
+000022c0: 5368 6172 7169 743a 3a51 4369 7263 3a3a  Sharqit::QCirc::
+000022d0: 696e 636c 7564 655f 746f 6628 7f69 6e63  include_tof(.inc
+000022e0: 6c75 6465 5f74 6f66 0139 3735 2c32 3834  lude_tof.975,284
+000022f0: 3631 0a76 6f69 6420 5368 6172 7169 743a  61.void Sharqit:
+00002300: 3a51 4369 7263 3a3a 7265 6d6f 7665 5f69  :QCirc::remove_i
+00002310: 6428 7f72 656d 6f76 655f 6964 0139 3834  d(.remove_id.984
+00002320: 2c32 3836 3437 0a76 6f69 6420 2053 6861  ,28647.void  Sha
+00002330: 7271 6974 3a3a 5143 6972 633a 3a72 6570  rqit::QCirc::rep
+00002340: 6c61 6365 5f77 6974 685f 727a 287f 7265  lace_with_rz(.re
+00002350: 706c 6163 655f 7769 7468 5f72 7a01 3939  place_with_rz.99
+00002360: 382c 3239 3139 340a 0c0a 6269 6e61 7279  8,29194...binary
+00002370: 5f6d 6174 7269 782e 682c 3833 370a 2364  _matrix.h,837.#d
+00002380: 6566 696e 6520 4249 4e41 5259 5f4d 4154  efine BINARY_MAT
+00002390: 5249 585f 487f 372c 3130 330a 2020 636c  RIX_H.7,103.  cl
+000023a0: 6173 7320 4269 6e61 7279 4d61 7472 6978  ass BinaryMatrix
+000023b0: 7f32 302c 3238 370a 2020 2020 7569 6e74  .20,287.    uint
+000023c0: 3332 5f74 2072 6f77 5f6e 756d 5f3b 7f32  32_t row_num_;.2
+000023d0: 332c 3332 330a 2020 2020 7569 6e74 3332  3,323.    uint32
+000023e0: 5f74 2063 6f6c 5f6e 756d 5f3b 7f32 342c  _t col_num_;.24,
+000023f0: 3337 360a 2020 2020 7374 643a 3a76 6563  376.    std::vec
+00002400: 746f 723c 7374 643a 3a76 6563 746f 723c  tor<std::vector<
+00002410: 7569 6e74 385f 743e 3e20 656c 656d 656e  uint8_t>> elemen
+00002420: 7473 5f3b 7f32 352c 3433 320a 2020 2020  ts_;.25,432.    
+00002430: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
+00002440: 3332 5f74 3e20 726f 775f 696e 6465 7865  32_t> row_indexe
+00002450: 735f 3b7f 3236 2c35 3333 0a20 2020 2042  s_;.26,533.    B
+00002460: 696e 6172 794d 6174 7269 7828 7f33 342c  inaryMatrix(.34,
+00002470: 3836 310a 2020 2020 4269 6e61 7279 4d61  861.    BinaryMa
+00002480: 7472 6978 287f 3433 2c31 3235 360a 2020  trix(.43,1256.  
+00002490: 2020 4269 6e61 7279 4d61 7472 6978 287f    BinaryMatrix(.
+000024a0: 3534 2c31 3631 350a 2020 2020 7569 6e74  54,1615.    uint
+000024b0: 3332 5f74 2072 6f77 5f6e 756d 287f 3537  32_t row_num(.57
+000024c0: 2c31 3739 390a 2020 2020 7569 6e74 3332  ,1799.    uint32
+000024d0: 5f74 2063 6f6c 5f6e 756d 287f 3539 2c31  _t col_num(.59,1
+000024e0: 3838 300a 2020 2020 7374 643a 3a76 6563  880.    std::vec
+000024f0: 746f 723c 7374 643a 3a76 6563 746f 723c  tor<std::vector<
+00002500: 7569 6e74 385f 743e 3e20 656c 656d 656e  uint8_t>> elemen
+00002510: 7473 287f 3631 2c31 3936 320a 2020 2020  ts(.61,1962.    
+00002520: 7374 643a 3a76 6563 746f 723c 7569 6e74  std::vector<uint
+00002530: 3332 5f74 3e20 726f 775f 696e 6465 7865  32_t> row_indexe
+00002540: 7328 7f36 332c 3230 3735 0a20 2020 2076  s(.63,2075.    v
+00002550: 6f69 6420 726f 775f 6e75 6d28 7f36 352c  oid row_num(.65,
+00002560: 3231 3738 0a20 2020 2076 6f69 6420 636f  2178.    void co
+00002570: 6c5f 6e75 6d28 7f36 372c 3232 3734 0a20  l_num(.67,2274. 
+00002580: 2020 2076 6f69 6420 656c 656d 656e 7473     void elements
+00002590: 287f 3639 2c32 3337 310a 2020 2020 766f  (.69,2371.    vo
+000025a0: 6964 2072 6f77 5f69 6e64 6578 6573 287f  id row_indexes(.
+000025b0: 3731 2c32 3530 310a 2020 2020 766f 6964  71,2501.    void
+000025c0: 2073 6574 5f69 6465 6e74 6974 7928 7f38   set_identity(.8
+000025d0: 322c 3239 3534 0a20 2020 2076 6f69 6420  2,2954.    void 
+000025e0: 7265 7665 7273 655f 656c 656d 656e 7428  reverse_element(
+000025f0: 7f39 362c 3333 3536 0a20 2020 2075 696e  .96,3356.    uin
+00002600: 7433 325f 7420 786f 725f 726f 7773 287f  t32_t xor_rows(.
+00002610: 3130 382c 3338 3339 0a20 2020 2076 6f69  108,3839.    voi
+00002620: 6420 7377 6170 5f72 6f77 7328 7f31 3235  d swap_rows(.125
+00002630: 2c34 3334 310a 2020 2020 766f 6964 2073  ,4341.    void s
+00002640: 7761 705f 636f 6c73 287f 3134 302c 3437  wap_cols(.140,47
+00002650: 3930 0a20 2020 2062 6f6f 6c20 6665 6173  90.    bool feas
+00002660: 6962 6c65 287f 3135 332c 3531 3833 0a20  ible(.153,5183. 
+00002670: 2020 2073 7464 3a3a 7665 6374 6f72 3c7f     std::vector<.
+00002680: 7374 643a 3a76 6563 746f 7201 3137 342c  std::vector.174,
+00002690: 3537 3430 0a20 2020 2066 7269 656e 6420  5740.    friend 
+000026a0: 7374 643a 3a6f 7374 7265 616d 2620 6f70  std::ostream& op
+000026b0: 6572 6174 6f72 3c3c 287f 3137 352c 3538  erator<<(.175,58
+000026c0: 3333 0a0c 0a75 7469 6c2e 682c 3436 0a23  33...util.h,46.#
+000026d0: 6465 6669 6e65 2055 5449 4c5f 487f 372c  define UTIL_H.7,
+000026e0: 3834 0a6e 616d 6573 7061 6365 2053 6861  84.namespace Sha
+000026f0: 7271 6974 207f 3133 2c31 3536 0a0c 0a71  rqit .13,156...q
+00002700: 6761 7465 2e63 7070 2c36 3830 0a53 6861  gate.cpp,680.Sha
+00002710: 7271 6974 3a3a 5147 6174 653a 3a51 4761  rqit::QGate::QGa
+00002720: 7465 287f 5147 6174 6501 382c 3930 0a53  te(.QGate.8,90.S
+00002730: 6861 7271 6974 3a3a 5147 6174 653a 3a51  harqit::QGate::Q
+00002740: 4761 7465 287f 5147 6174 6501 3831 2c32  Gate(.QGate.81,2
+00002750: 3433 330a 7374 643a 3a76 6563 746f 723c  433.std::vector<
+00002760: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+00002770: 3a63 6f6d 706c 6578 3c64 6f75 626c 653e  :complex<double>
+00002780: 3e3e 2053 6861 7271 6974 3a3a 5147 6174  >> Sharqit::QGat
+00002790: 653a 3a6b 696e 645f 746f 5f6f 7028 7f6b  e::kind_to_op(.k
+000027a0: 696e 645f 746f 5f6f 7001 3132 352c 3337  ind_to_op.125,37
+000027b0: 3131 0a73 7464 3a3a 7374 7269 6e67 2053  11.std::string S
+000027c0: 6861 7271 6974 3a3a 5147 6174 653a 3a6e  harqit::QGate::n
+000027d0: 616d 6528 7f6e 616d 6501 3231 312c 3631  ame(.name.211,61
+000027e0: 3834 0a73 7464 3a3a 7374 7269 6e67 2053  84.std::string S
+000027f0: 6861 7271 6974 3a3a 5147 6174 653a 3a74  harqit::QGate::t
+00002800: 6f5f 7374 7269 6e67 287f 746f 5f73 7472  o_string(.to_str
+00002810: 696e 6701 3232 302c 3635 3030 0a73 7464  ing.220,6500.std
+00002820: 3a3a 7475 706c 653c 5368 6172 7169 743a  ::tuple<Sharqit:
+00002830: 3a51 4761 7465 4b69 6e64 2c20 5368 6172  :QGateKind, Shar
+00002840: 7169 743a 3a50 6861 7365 3e20 5368 6172  qit::Phase> Shar
+00002850: 7169 743a 3a51 4761 7465 3a3a 6b69 6e64  qit::QGate::kind
+00002860: 5f70 6861 7365 287f 6b69 6e64 5f70 6861  _phase(.kind_pha
+00002870: 7365 0132 3337 2c36 3938 310a 5368 6172  se.237,6981.Shar
+00002880: 7169 743a 3a51 4761 7465 2053 6861 7271  qit::QGate Sharq
+00002890: 6974 3a3a 5147 6174 653a 3a69 6e76 6572  it::QGate::inver
+000028a0: 7365 287f 696e 7665 7273 6501 3331 342c  se(.inverse.314,
+000028b0: 3838 3435 0a62 6f6f 6c20 5368 6172 7169  8845.bool Sharqi
+000028c0: 743a 3a51 4761 7465 3a3a 6973 5f69 6465  t::QGate::is_ide
+000028d0: 6e74 6963 616c 287f 6973 5f69 6465 6e74  ntical(.is_ident
+000028e0: 6963 616c 0133 3936 2c31 3134 3237 0a62  ical.396,11427.b
+000028f0: 6f6f 6c20 5368 6172 7169 743a 3a51 4761  ool Sharqit::QGa
+00002900: 7465 3a3a 6f76 6572 6c61 7028 7f6f 7665  te::overlap(.ove
+00002910: 726c 6170 0134 3131 2c31 3139 3836 0a62  rlap.411,11986.b
+00002920: 6f6f 6c20 5368 6172 7169 743a 3a51 4761  ool Sharqit::QGa
+00002930: 7465 3a3a 6d65 7267 6561 626c 6528 7f6d  te::mergeable(.m
+00002940: 6572 6765 6162 6c65 0134 3235 2c31 3232  ergeable.425,122
+00002950: 3337 0a62 6f6f 6c20 5368 6172 7169 743a  37.bool Sharqit:
+00002960: 3a51 4761 7465 3a3a 636f 6d6d 7574 6162  :QGate::commutab
+00002970: 6c65 287f 636f 6d6d 7574 6162 6c65 0134  le(.commutable.4
+00002980: 3432 2c31 3239 3734 0a76 6f69 6420 5368  42,12974.void Sh
+00002990: 6172 7169 743a 3a51 4761 7465 3a3a 6d65  arqit::QGate::me
+000029a0: 7267 6528 7f6d 6572 6765 0134 3836 2c31  rge(.merge.486,1
+000029b0: 3438 3739 0a0c 0a65 7874 7261 6374 5f71  4879...extract_q
+000029c0: 6369 7263 2e63 7070 2c34 3635 0a76 6f69  circ.cpp,465.voi
+000029d0: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
+000029e0: 6772 616d 3a3a 7065 726d 7574 6174 696f  gram::permutatio
+000029f0: 6e5f 6173 5f73 7761 7028 7f70 6572 6d75  n_as_swap(.permu
+00002a00: 7461 7469 6f6e 5f61 735f 7377 6170 0138  tation_as_swap.8
+00002a10: 2c31 3531 0a73 7464 3a3a 7665 6374 6f72  ,151.std::vector
+00002a20: 3c73 7464 3a3a 7061 6972 3c75 696e 7433  <std::pair<uint3
+00002a30: 325f 742c 2075 696e 7433 325f 743e 3e20  2_t, uint32_t>> 
+00002a40: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
+00002a50: 616d 3a3a 6578 7472 6163 745f 3271 5f63  am::extract_2q_c
+00002a60: 6f6e 6e65 6374 7328 7f65 7874 7261 6374  onnects(.extract
+00002a70: 5f32 715f 636f 6e6e 6563 7473 0132 382c  _2q_connects.28,
+00002a80: 3632 370a 626f 6f6c 2053 6861 7271 6974  627.bool Sharqit
+00002a90: 3a3a 5a58 4469 6167 7261 6d3a 3a75 7064  ::ZXDiagram::upd
+00002aa0: 6174 655f 6672 6f6e 7469 6572 287f 7570  ate_frontier(.up
+00002ab0: 6461 7465 5f66 726f 6e74 6965 7201 3836  date_frontier.86
+00002ac0: 2c32 3238 310a 626f 6f6c 2053 6861 7271  ,2281.bool Sharq
+00002ad0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a75  it::ZXDiagram::u
+00002ae0: 7064 6174 655f 6672 6f6e 7469 6572 5f70  pdate_frontier_p
+00002af0: 6728 7f75 7064 6174 655f 6672 6f6e 7469  g(.update_fronti
+00002b00: 6572 5f70 6701 3232 352c 3634 3038 0a76  er_pg.225,6408.v
+00002b10: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
+00002b20: 6961 6772 616d 3a3a 7072 6f63 6573 735f  iagram::process_
+00002b30: 6672 6f6e 7469 6572 287f 7072 6f63 6573  frontier(.proces
+00002b40: 735f 6672 6f6e 7469 6572 0133 3035 2c39  s_frontier.305,9
+00002b50: 3030 380a 5368 6172 7169 743a 3a51 4369  008.Sharqit::QCi
+00002b60: 7263 2053 6861 7271 6974 3a3a 5a58 4469  rc Sharqit::ZXDi
+00002b70: 6167 7261 6d3a 3a65 7874 7261 6374 5f71  agram::extract_q
+00002b80: 6369 7263 287f 6578 7472 6163 745f 7163  circ(.extract_qc
+00002b90: 6972 6301 3335 332c 3130 3539 350a 0c0a  irc.353,10595...
+00002ba0: 6461 672e 682c 3138 3933 0a23 6465 6669  dag.h,1893.#defi
+00002bb0: 6e65 2044 4147 5f48 7f37 2c31 3337 0a20  ne DAG_H.7,137. 
+00002bc0: 2065 6e75 6d20 4441 474e 6f64 654b 696e   enum DAGNodeKin
+00002bd0: 6420 7f32 322c 3332 390a 0909 2020 2020  d .22,329...    
+00002be0: 4f70 4e6f 6465 2c7f 3233 2c33 3530 0a09  OpNode,.23,350..
+00002bf0: 0920 2020 2049 6e4e 6f64 652c 7f32 342c  .    InNode,.24,
+00002c00: 3430 310a 0909 2020 2020 4f75 744e 6f64  401...    OutNod
+00002c10: 6520 7f32 352c 3433 310a 2020 656e 756d  e .25,431.  enum
+00002c20: 2044 4147 4564 6765 4b69 6e64 207f 3238   DAGEdgeKind .28
+00002c30: 2c34 3933 0a09 0920 2020 2046 6f72 7761  ,493...    Forwa
+00002c40: 7264 2c7f 3239 2c35 3134 0a09 0920 2020  rd,.29,514...   
+00002c50: 2042 6163 6b77 6172 6420 7f33 302c 3535   Backward .30,55
+00002c60: 320a 2020 636c 6173 7320 4441 474e 6f64  2.  class DAGNod
+00002c70: 657f 3339 2c37 3133 0a20 2020 2044 4147  e.39,713.    DAG
+00002c80: 4e6f 6465 4b69 6e64 206b 696e 645f 3b7f  NodeKind kind_;.
+00002c90: 3432 2c37 3434 0a20 2020 2051 4761 7465  42,744.    QGate
+00002ca0: 2071 6761 7465 5f3b 7f34 332c 3738 390a   qgate_;.43,789.
+00002cb0: 2020 2020 4441 474e 6f64 6528 7f35 302c      DAGNode(.50,
+00002cc0: 3130 3031 0a20 2020 2044 4147 4e6f 6465  1001.    DAGNode
+00002cd0: 287f 3536 2c31 3232 360a 2020 2020 4441  (.56,1226.    DA
+00002ce0: 474e 6f64 654b 696e 6420 6b69 6e64 287f  GNodeKind kind(.
+00002cf0: 3538 2c31 3333 310a 2020 2020 5147 6174  58,1331.    QGat
+00002d00: 6520 7167 6174 6528 7f36 302c 3134 3037  e qgate(.60,1407
+00002d10: 0a20 2020 2076 6f69 6420 6b69 6e64 287f  .    void kind(.
+00002d20: 3632 2c31 3437 380a 2020 2020 766f 6964  62,1478.    void
+00002d30: 2071 6761 7465 287f 3634 2c31 3536 330a   qgate(.64,1563.
+00002d40: 2020 2020 7569 6e74 3332 5f74 2071 7562      uint32_t qub
+00002d50: 6974 5f6e 756d 287f 3734 2c31 3839 340a  it_num(.74,1894.
+00002d60: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
+00002d70: 7569 6e74 3332 5f74 3e20 7169 6428 7f37  uint32_t> qid(.7
+00002d80: 392c 3231 3038 0a20 2020 2062 6f6f 6c20  9,2108.    bool 
+00002d90: 6973 5f69 6e6e 6f64 6528 7f38 342c 3233  is_innode(.84,23
+00002da0: 3032 0a20 2020 2062 6f6f 6c20 6973 5f6f  02.    bool is_o
+00002db0: 7574 6e6f 6465 287f 3839 2c32 3531 380a  utnode(.89,2518.
+00002dc0: 2020 2020 626f 6f6c 2069 735f 6f70 6e6f      bool is_opno
+00002dd0: 6465 287f 3934 2c32 3737 320a 2020 2020  de(.94,2772.    
+00002de0: 626f 6f6c 2069 735f 6964 656e 7469 7479  bool is_identity
+00002df0: 287f 3939 2c33 3030 380a 2020 2020 626f  (.99,3008.    bo
+00002e00: 6f6c 2069 735f 6861 6461 6d61 7264 287f  ol is_hadamard(.
+00002e10: 3130 352c 3332 3832 0a20 2020 2062 6f6f  105,3282.    boo
+00002e20: 6c20 6973 5f72 6f74 6174 696f 6e28 7f31  l is_rotation(.1
+00002e30: 3130 2c33 3438 330a 2020 2020 626f 6f6c  10,3483.    bool
+00002e40: 2069 735f 636e 6f74 287f 3131 352c 3336   is_cnot(.115,36
+00002e50: 3737 0a20 2020 2062 6f6f 6c20 6973 5f69  77.    bool is_i
+00002e60: 6e63 6c75 6465 6428 7f31 3231 2c33 3935  ncluded(.121,395
+00002e70: 320a 2020 2020 626f 6f6c 206d 6572 6765  2.    bool merge
+00002e80: 6162 6c65 287f 3133 312c 3432 3938 0a20  able(.131,4298. 
+00002e90: 2020 2062 6f6f 6c20 636f 6d6d 7574 6162     bool commutab
+00002ea0: 6c65 287f 3133 372c 3436 3036 0a20 2020  le(.137,4606.   
+00002eb0: 2076 6f69 6420 6d65 7267 6528 7f31 3432   void merge(.142
+00002ec0: 2c34 3832 340a 2020 636c 6173 7320 4441  ,4824.  class DA
+00002ed0: 4745 6467 657f 3135 302c 3439 3938 0a20  GEdge.150,4998. 
+00002ee0: 2020 2044 4147 4564 6765 4b69 6e64 206b     DAGEdgeKind k
+00002ef0: 696e 645f 3b7f 3135 332c 3530 3239 0a20  ind_;.153,5029. 
+00002f00: 2020 2075 696e 7433 325f 7420 715f 3b7f     uint32_t q_;.
+00002f10: 3135 342c 3531 3032 0a20 2020 2075 696e  154,5102.    uin
+00002f20: 7433 325f 7420 746f 5f3b 7f31 3535 2c35  t32_t to_;.155,5
+00002f30: 3135 330a 2020 2020 4441 4745 6467 6528  153.    DAGEdge(
+00002f40: 7f31 3633 2c35 3431 340a 2020 2020 4441  .163,5414.    DA
+00002f50: 4745 6467 6528 7f31 3639 2c35 3636 360a  GEdge(.169,5666.
+00002f60: 2020 2020 4441 4745 6467 654b 696e 6420      DAGEdgeKind 
+00002f70: 6b69 6e64 287f 3137 312c 3537 3738 0a20  kind(.171,5778. 
+00002f80: 2020 2075 696e 7433 325f 7420 7128 7f31     uint32_t q(.1
+00002f90: 3733 2c35 3835 300a 2020 2020 7569 6e74  73,5850.    uint
+00002fa0: 3332 5f74 2074 6f28 7f31 3735 2c35 3931  32_t to(.175,591
+00002fb0: 340a 2020 2020 766f 6964 206b 696e 6428  4.    void kind(
+00002fc0: 7f31 3737 2c35 3938 320a 2020 2020 766f  .177,5982.    vo
+00002fd0: 6964 2071 287f 3137 392c 3630 3537 0a20  id q(.179,6057. 
+00002fe0: 2020 2076 6f69 6420 746f 287f 3138 312c     void to(.181,
+00002ff0: 3631 3138 0a20 2020 2062 6f6f 6c20 6973  6118.    bool is
+00003000: 5f66 6f72 7761 7264 287f 3139 312c 3634  _forward(.191,64
+00003010: 3039 0a20 2020 2062 6f6f 6c20 6973 5f62  09.    bool is_b
+00003020: 6163 6b77 6172 6428 7f31 3936 2c36 3632  ackward(.196,662
+00003030: 370a 2020 636c 6173 7320 4441 4743 6972  7.  class DAGCir
+00003040: 637f 3230 352c 3638 3434 0a20 2020 2075  c.205,6844.    u
+00003050: 696e 7433 325f 7420 7175 6269 745f 6e75  int32_t qubit_nu
+00003060: 6d5f 3b7f 3230 382c 3638 3735 0a20 2020  m_;.208,6875.   
+00003070: 2073 7464 3a3a 7665 6374 6f72 3c44 4147   std::vector<DAG
+00003080: 4e6f 6465 3e20 6e6f 6465 735f 3b7f 3230  Node> nodes_;.20
+00003090: 392c 3639 3232 0a20 2020 2073 7464 3a3a  9,6922.    std::
+000030a0: 7665 6374 6f72 3c75 696e 7433 325f 743e  vector<uint32_t>
+000030b0: 2069 6e70 7574 735f 3b7f 3231 302c 3639   inputs_;.210,69
+000030c0: 3930 0a20 2020 2073 7464 3a3a 7665 6374  90.    std::vect
+000030d0: 6f72 3c75 696e 7433 325f 743e 206f 7574  or<uint32_t> out
+000030e0: 7075 7473 5f3b 7f32 3131 2c37 3036 330a  puts_;.211,7063.
+000030f0: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
+00003100: 7374 643a 3a76 6563 746f 723c 4441 4745  std::vector<DAGE
+00003110: 6467 653e 3e20 6164 6a5f 6d61 745f 3b7f  dge>> adj_mat_;.
+00003120: 3231 322c 3731 3338 0a20 2020 2044 4147  212,7138.    DAG
+00003130: 4369 7263 287f 3236 362c 3935 3435 0a20  Circ(.266,9545. 
+00003140: 2020 2075 696e 7433 325f 7420 7175 6269     uint32_t qubi
+00003150: 745f 6e75 6d28 7f32 3730 2c39 3733 370a  t_num(.270,9737.
+00003160: 2020 2020 7374 643a 3a76 6563 746f 723c      std::vector<
+00003170: 4441 474e 6f64 653e 206e 6f64 6573 287f  DAGNode> nodes(.
+00003180: 3237 322c 3938 3230 0a20 2020 2073 7464  272,9820.    std
+00003190: 3a3a 7665 6374 6f72 3c75 696e 7433 325f  ::vector<uint32_
+000031a0: 743e 2069 6e70 7574 7328 7f32 3734 2c39  t> inputs(.274,9
+000031b0: 3930 380a 2020 2020 7374 643a 3a76 6563  908.    std::vec
+000031c0: 746f 723c 7569 6e74 3332 5f74 3e20 6f75  tor<uint32_t> ou
+000031d0: 7470 7574 7328 7f32 3736 2c31 3030 3030  tputs(.276,10000
+000031e0: 0a20 2020 2073 7464 3a3a 7665 6374 6f72  .    std::vector
+000031f0: 3c73 7464 3a3a 7665 6374 6f72 3c44 4147  <std::vector<DAG
+00003200: 4564 6765 3e3e 2061 646a 5f6d 6174 287f  Edge>> adj_mat(.
+00003210: 3237 382c 3130 3039 340a 2020 2020 766f  278,10094.    vo
+00003220: 6964 2071 7562 6974 5f6e 756d 287f 3238  id qubit_num(.28
+00003230: 302c 3130 3230 320a 2020 2020 766f 6964  0,10202.    void
+00003240: 206e 6f64 6573 287f 3238 322c 3130 3330   nodes(.282,1030
+00003250: 340a 2020 2020 766f 6964 2069 6e70 7574  4.    void input
+00003260: 7328 7f32 3834 2c31 3034 3034 0a20 2020  s(.284,10404.   
+00003270: 2076 6f69 6420 6f75 7470 7574 7328 7f32   void outputs(.2
+00003280: 3836 2c31 3035 3130 0a20 2020 2076 6f69  86,10510.    voi
+00003290: 6420 6164 6a5f 6d61 7428 7f32 3838 2c31  d adj_mat(.288,1
+000032a0: 3036 3230 0a20 2020 2076 6f69 6420 7368  0620.    void sh
+000032b0: 6f77 287f 3239 372c 3130 3931 390a 2020  ow(.297,10919.  
+000032c0: 2020 7569 6e74 3332 5f74 2067 6174 655f    uint32_t gate_
+000032d0: 636f 756e 7428 7f33 3031 2c31 3130 3138  count(.301,11018
+000032e0: 0a20 2020 2066 7269 656e 6420 7374 643a  .    friend std:
+000032f0: 3a6f 7374 7265 616d 2620 6f70 6572 6174  :ostream& operat
+00003300: 6f72 3c3c 287f 3339 352c 3134 3931 300a  or<<(.395,14910.
+00003310: 0c0a 7163 6972 632e 682c 3138 3330 0a23  ..qcirc.h,1830.#
+00003320: 6465 6669 6e65 2051 4349 5243 5f48 7f37  define QCIRC_H.7
+00003330: 2c38 300a 2020 636c 6173 7320 5143 6972  ,80.  class QCir
+00003340: 637f 3334 2c34 3932 0a20 2020 2075 696e  c.34,492.    uin
+00003350: 7433 325f 7420 7175 6269 745f 6e75 6d5f  t32_t qubit_num_
+00003360: 3b7f 3337 2c35 3231 0a20 2020 2073 7464  ;.37,521.    std
+00003370: 3a3a 7665 6374 6f72 3c51 4761 7465 3e20  ::vector<QGate> 
+00003380: 7167 6174 6573 5f3b 7f33 382c 3536 380a  qgates_;.38,568.
+00003390: 2020 2020 5143 6972 6328 7f35 392c 3135      QCirc(.59,15
+000033a0: 3530 0a20 2020 2051 4369 7263 287f 3634  50.    QCirc(.64
+000033b0: 2c31 3731 390a 2020 2020 5143 6972 6328  ,1719.    QCirc(
+000033c0: 7f36 392c 3139 3037 0a20 2020 2075 696e  .69,1907.    uin
+000033d0: 7433 325f 7420 7175 6269 745f 6e75 6d28  t32_t qubit_num(
+000033e0: 7f37 312c 3230 3331 0a20 2020 2075 696e  .71,2031.    uin
+000033f0: 7433 325f 7420 6765 745f 7175 6269 745f  t32_t get_qubit_
+00003400: 6e75 6d28 7f37 332c 3231 3138 0a20 2020  num(.73,2118.   
+00003410: 2073 7464 3a3a 7665 6374 6f72 3c51 4761   std::vector<QGa
+00003420: 7465 3e20 7167 6174 6573 287f 3735 2c32  te> qgates(.75,2
+00003430: 3230 360a 2020 2020 766f 6964 2071 7562  206.    void qub
+00003440: 6974 5f6e 756d 287f 3737 2c32 3239 370a  it_num(.77,2297.
+00003450: 2020 2020 766f 6964 2071 6761 7465 7328      void qgates(
+00003460: 7f37 392c 3234 3030 0a20 2020 2075 696e  .79,2400.    uin
+00003470: 7433 325f 7420 7167 6174 655f 6e75 6d28  t32_t qgate_num(
+00003480: 7f38 342c 3235 3735 0a20 2020 2076 6f69  .84,2575.    voi
+00003490: 6420 636c 6561 7228 7f39 382c 3330 3238  d clear(.98,3028
+000034a0: 0a20 2020 2073 7464 3a3a 6d61 703c 7f73  .    std::map<.s
+000034b0: 7464 3a3a 6d61 7001 3130 332c 3331 3930  td::map.103,3190
+000034c0: 0a20 2020 2075 696e 7433 325f 7420 6761  .    uint32_t ga
+000034d0: 7465 5f63 6f75 6e74 287f 3130 382c 3333  te_count(.108,33
+000034e0: 3934 0a20 2020 2075 696e 7433 325f 7420  94.    uint32_t 
+000034f0: 7477 6f71 5f63 6f75 6e74 287f 3135 382c  twoq_count(.158,
+00003500: 3439 3636 0a20 2020 2075 696e 7433 325f  4966.    uint32_
+00003510: 7420 746f 665f 636f 756e 7428 7f31 3733  t tof_count(.173
+00003520: 2c35 3437 320a 2020 2020 766f 6964 2073  ,5472.    void s
+00003530: 686f 7728 7f31 3838 2c36 3030 380a 2020  how(.188,6008.  
+00003540: 2020 766f 6964 2070 7269 6e74 5f71 6369    void print_qci
+00003550: 7263 287f 3139 322c 3631 3634 0a20 2020  rc(.192,6164.   
+00003560: 2051 4369 7263 2620 6164 645f 7167 6174   QCirc& add_qgat
+00003570: 6528 7f32 3138 2c37 3433 320a 2020 2020  e(.218,7432.    
+00003580: 5368 6172 7169 743a 3a51 4761 7465 2067  Sharqit::QGate g
+00003590: 6574 5f71 6761 7465 287f 3235 302c 3932  et_qgate(.250,92
+000035a0: 3030 0a20 2020 2073 7464 3a3a 7665 6374  00.    std::vect
+000035b0: 6f72 3c53 6861 7271 6974 3a3a 5147 6174  or<Sharqit::QGat
+000035c0: 653e 2067 6574 5f71 6761 7465 7328 7f32  e> get_qgates(.2
+000035d0: 3535 2c39 3337 370a 2020 2020 5143 6972  55,9377.    QCir
+000035e0: 6326 2069 6428 7f33 3436 2c31 3236 3137  c& id(.346,12617
+000035f0: 0a20 2020 2051 4369 7263 2620 7828 7f33  .    QCirc& x(.3
+00003600: 3532 2c31 3238 3735 0a20 2020 2051 4369  52,12875.    QCi
+00003610: 7263 2620 7a28 7f33 3538 2c31 3331 3331  rc& z(.358,13131
+00003620: 0a20 2020 2051 4369 7263 2620 7328 7f33  .    QCirc& s(.3
+00003630: 3634 2c31 3333 3831 0a20 2020 2051 4369  64,13381.    QCi
+00003640: 7263 2620 7364 6728 7f33 3730 2c31 3336  rc& sdg(.370,136
+00003650: 3539 0a20 2020 2051 4369 7263 2620 7428  59.    QCirc& t(
+00003660: 7f33 3736 2c31 3339 3133 0a20 2020 2051  .376,13913.    Q
+00003670: 4369 7263 2620 7464 6728 7f33 3832 2c31  Circ& tdg(.382,1
+00003680: 3431 3931 0a20 2020 2051 4369 7263 2620  4191.    QCirc& 
+00003690: 6828 7f33 3838 2c31 3434 3537 0a20 2020  h(.388,14457.   
+000036a0: 2051 4369 7263 2620 727a 287f 3339 352c   QCirc& rz(.395,
+000036b0: 3134 3735 350a 2020 2020 5143 6972 6326  14755.    QCirc&
+000036c0: 2069 6432 287f 3430 322c 3135 3131 340a   id2(.402,15114.
+000036d0: 2020 2020 5143 6972 6326 2063 7828 7f34      QCirc& cx(.4
+000036e0: 3131 2c31 3536 3631 0a20 2020 2051 4369  11,15661.    QCi
+000036f0: 7263 2620 637a 287f 3432 332c 3136 3332  rc& cz(.423,1632
+00003700: 350a 2020 2020 5143 6972 6326 2072 7828  5.    QCirc& rx(
+00003710: 7f34 3333 2c31 3637 3732 0a20 2020 2051  .433,16772.    Q
+00003720: 4369 7263 2620 6363 7828 7f34 3433 2c31  Circ& ccx(.443,1
+00003730: 3734 3236 0a20 2020 2051 4369 7263 2620  7426.    QCirc& 
+00003740: 6363 7a28 7f34 3538 2c31 3832 3539 0a20  ccz(.458,18259. 
+00003750: 2020 2051 4369 7263 2620 7928 7f34 3636     QCirc& y(.466
+00003760: 2c31 3836 3933 0a20 2020 2051 4369 7263  ,18693.    QCirc
+00003770: 2620 7378 287f 3437 322c 3138 3936 310a  & sx(.472,18961.
+00003780: 2020 2020 5143 6972 6326 2073 7864 6728      QCirc& sxdg(
+00003790: 7f34 3738 2c31 3932 3633 0a20 2020 2051  .478,19263.    Q
+000037a0: 4369 7263 2620 7279 287f 3438 352c 3139  Circ& ry(.485,19
+000037b0: 3535 380a 2020 2020 5143 6972 6326 2070  558.    QCirc& p
+000037c0: 287f 3439 332c 3139 3932 340a 2020 2020  (.493,19924.    
+000037d0: 5143 6972 6326 2063 7928 7f35 3030 2c32  QCirc& cy(.500,2
+000037e0: 3032 3637 0a20 2020 2051 4369 7263 2620  0267.    QCirc& 
+000037f0: 6373 7828 7f35 3037 2c32 3036 3334 0a20  csx(.507,20634. 
+00003800: 2020 2051 4369 7263 2620 6373 7864 6728     QCirc& csxdg(
+00003810: 7f35 3134 2c32 3130 3234 0a20 2020 2051  .514,21024.    Q
+00003820: 4369 7263 2620 6368 287f 3532 312c 3231  Circ& ch(.521,21
+00003830: 3430 330a 2020 2020 5143 6972 6326 2063  403.    QCirc& c
+00003840: 7328 7f35 3239 2c32 3138 3233 0a20 2020  s(.529,21823.   
+00003850: 2051 4369 7263 2620 6373 6467 287f 3533   QCirc& csdg(.53
+00003860: 372c 3232 3231 370a 2020 2020 5143 6972  7,22217.    QCir
+00003870: 6326 2063 7428 7f35 3435 2c32 3235 3932  c& ct(.545,22592
+00003880: 0a20 2020 2051 4369 7263 2620 6374 6467  .    QCirc& ctdg
+00003890: 287f 3535 332c 3232 3939 380a 2020 2020  (.553,22998.    
+000038a0: 5143 6972 6326 2063 7278 287f 3536 322c  QCirc& crx(.562,
+000038b0: 3233 3432 370a 2020 2020 5143 6972 6326  23427.    QCirc&
+000038c0: 2063 7279 287f 3537 312c 3233 3836 340a   cry(.571,23864.
+000038d0: 2020 2020 5143 6972 6326 2063 727a 287f      QCirc& crz(.
+000038e0: 3538 302c 3234 3332 360a 2020 2020 5143  580,24326.    QC
+000038f0: 6972 6326 2063 7028 7f35 3839 2c32 3437  irc& cp(.589,247
+00003900: 3837 0a20 2020 2051 4369 7263 2620 7278  87.    QCirc& rx
+00003910: 7828 7f35 3938 2c32 3532 3231 0a20 2020  x(.598,25221.   
+00003920: 2051 4369 7263 2620 7279 7928 7f36 3132   QCirc& ryy(.612
+00003930: 2c32 3537 3039 0a20 2020 2051 4369 7263  ,25709.    QCirc
+00003940: 2620 727a 7a28 7f36 3236 2c32 3632 3437  & rzz(.626,26247
+00003950: 0a20 2020 2051 4369 7263 2620 7377 287f  .    QCirc& sw(.
+00003960: 3633 342c 3236 3630 350a 2020 2020 5143  634,26605.    QC
+00003970: 6972 6326 2063 7377 287f 3634 332c 3237  irc& csw(.643,27
+00003980: 3031 360a 2020 2020 5143 6972 6326 2063  016.    QCirc& c
+00003990: 785f 6465 636f 6d70 287f 3635 322c 3237  x_decomp(.652,27
+000039a0: 3532 310a 2020 2020 5143 6972 6326 2063  521.    QCirc& c
+000039b0: 7a5f 6465 636f 6d70 287f 3636 372c 3238  z_decomp(.667,28
+000039c0: 3133 380a 2020 2020 5143 6972 6326 206f  138.    QCirc& o
+000039d0: 7065 7261 746f 722b 3d28 7f6f 7065 7261  perator+=(.opera
+000039e0: 746f 722b 3d01 3639 362c 3239 3636 320a  tor+=.696,29662.
+000039f0: 2020 2020 6672 6965 6e64 2051 4369 7263      friend QCirc
+00003a00: 206f 7065 7261 746f 722b 287f 3639 372c   operator+(.697,
+00003a10: 3239 3732 390a 2020 2020 6672 6965 6e64  29729.    friend
+00003a20: 2073 7464 3a3a 6f73 7472 6561 6d26 206f   std::ostream& o
+00003a30: 7065 7261 746f 723c 3c28 7f36 3938 2c32  perator<<(.698,2
+00003a40: 3938 3338 0a0c 0a64 6167 6369 7263 2e63  9838...dagcirc.c
+00003a50: 7070 2c31 3632 350a 5368 6172 7169 743a  pp,1625.Sharqit:
+00003a60: 3a44 4147 4369 7263 3a3a 4441 4743 6972  :DAGCirc::DAGCir
+00003a70: 6328 7f44 4147 4369 7263 0138 2c39 320a  c(.DAGCirc.8,92.
+00003a80: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
+00003a90: 3a3a 4441 4743 6972 6328 7f44 4147 4369  ::DAGCirc(.DAGCi
+00003aa0: 7263 0132 392c 3639 390a 7374 643a 3a73  rc.29,699.std::s
+00003ab0: 7472 696e 6720 5368 6172 7169 743a 3a44  tring Sharqit::D
+00003ac0: 4147 4369 7263 3a3a 746f 5f73 7472 696e  AGCirc::to_strin
+00003ad0: 6728 7f74 6f5f 7374 7269 6e67 0135 332c  g(.to_string.53,
+00003ae0: 3133 3933 0a75 696e 7433 325f 7420 5368  1393.uint32_t Sh
+00003af0: 6172 7169 743a 3a44 4147 4369 7263 3a3a  arqit::DAGCirc::
+00003b00: 6170 7065 6e64 5f6e 6f64 6528 7f61 7070  append_node(.app
+00003b10: 656e 645f 6e6f 6465 0137 322c 3138 3632  end_node.72,1862
+00003b20: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+00003b30: 743a 3a44 4147 4369 7263 3a3a 7072 6576  t::DAGCirc::prev
+00003b40: 5f6e 6f64 6528 7f70 7265 765f 6e6f 6465  _node(.prev_node
+00003b50: 0138 302c 3230 3535 0a75 696e 7433 325f  .80,2055.uint32_
+00003b60: 7420 5368 6172 7169 743a 3a44 4147 4369  t Sharqit::DAGCi
+00003b70: 7263 3a3a 6e65 7874 5f6e 6f64 6528 7f6e  rc::next_node(.n
+00003b80: 6578 745f 6e6f 6465 0139 392c 3235 3233  ext_node.99,2523
+00003b90: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
+00003ba0: 4147 4369 7263 3a3a 636f 6e6e 6563 745f  AGCirc::connect_
+00003bb0: 6e6f 6465 7328 7f63 6f6e 6e65 6374 5f6e  nodes(.connect_n
+00003bc0: 6f64 6573 0131 3138 2c32 3938 380a 766f  odes.118,2988.vo
+00003bd0: 6964 2053 6861 7271 6974 3a3a 4441 4743  id Sharqit::DAGC
+00003be0: 6972 633a 3a72 656d 6f76 655f 6e6f 6465  irc::remove_node
+00003bf0: 287f 7265 6d6f 7665 5f6e 6f64 6501 3132  (.remove_node.12
+00003c00: 392c 3334 3733 0a76 6f69 6420 5368 6172  9,3473.void Shar
+00003c10: 7169 743a 3a44 4147 4369 7263 3a3a 7265  qit::DAGCirc::re
+00003c20: 6d6f 7665 5f65 6467 6528 7f72 656d 6f76  move_edge(.remov
+00003c30: 655f 6564 6765 0131 3631 2c34 3132 330a  e_edge.161,4123.
+00003c40: 766f 6964 2053 6861 7271 6974 3a3a 4441  void Sharqit::DA
+00003c50: 4743 6972 633a 3a72 656d 6f76 655f 6564  GCirc::remove_ed
+00003c60: 6765 287f 7265 6d6f 7665 5f65 6467 6501  ge(.remove_edge.
+00003c70: 3137 392c 3435 3238 0a76 6f69 6420 5368  179,4528.void Sh
+00003c80: 6172 7169 743a 3a44 4147 4369 7263 3a3a  arqit::DAGCirc::
+00003c90: 7265 6d6f 7665 5f65 6467 6573 5f6f 665f  remove_edges_of_
+00003ca0: 6e6f 6465 287f 7265 6d6f 7665 5f65 6467  node(.remove_edg
+00003cb0: 6573 5f6f 665f 6e6f 6465 0131 3937 2c34  es_of_node.197,4
+00003cc0: 3938 330a 766f 6964 2053 6861 7271 6974  983.void Sharqit
+00003cd0: 3a3a 4441 4743 6972 633a 3a72 656d 6f76  ::DAGCirc::remov
+00003ce0: 655f 6973 6f6c 6174 6564 5f6e 6f64 6573  e_isolated_nodes
+00003cf0: 287f 7265 6d6f 7665 5f69 736f 6c61 7465  (.remove_isolate
+00003d00: 645f 6e6f 6465 7301 3231 312c 3533 3132  d_nodes.211,5312
+00003d10: 0a53 6861 7271 6974 3a3a 4441 4743 6972  .Sharqit::DAGCir
+00003d20: 6326 2053 6861 7271 6974 3a3a 4441 4743  c& Sharqit::DAGC
+00003d30: 6972 633a 3a61 6464 5f71 6761 7465 287f  irc::add_qgate(.
+00003d40: 6164 645f 7167 6174 6501 3232 372c 3536  add_qgate.227,56
+00003d50: 3331 0a53 6861 7271 6974 3a3a 5143 6972  31.Sharqit::QCir
+00003d60: 6320 5368 6172 7169 743a 3a44 4147 4369  c Sharqit::DAGCi
+00003d70: 7263 3a3a 746f 5f71 6369 7263 287f 746f  rc::to_qcirc(.to
+00003d80: 5f71 6369 7263 0132 3634 2c36 3731 370a  _qcirc.264,6717.
+00003d90: 766f 6964 2053 6861 7271 6974 3a3a 4441  void Sharqit::DA
+00003da0: 4743 6972 633a 3a69 645f 7265 6d6f 7661  GCirc::id_remova
+00003db0: 6c28 7f69 645f 7265 6d6f 7661 6c01 3330  l(.id_removal.30
+00003dc0: 362c 3737 3639 0a76 6f69 6420 5368 6172  6,7769.void Shar
+00003dd0: 7169 743a 3a44 4147 4369 7263 3a3a 6378  qit::DAGCirc::cx
+00003de0: 5f74 6f5f 637a 5f67 6174 6528 7f63 785f  _to_cz_gate(.cx_
+00003df0: 746f 5f63 7a5f 6761 7465 0133 3239 2c38  to_cz_gate.329,8
+00003e00: 3438 340a 766f 6964 2053 6861 7271 6974  484.void Sharqit
+00003e10: 3a3a 4441 4743 6972 633a 3a63 7a5f 746f  ::DAGCirc::cz_to
+00003e20: 5f63 785f 6761 7465 287f 637a 5f74 6f5f  _cx_gate(.cz_to_
+00003e30: 6378 5f67 6174 6501 3335 392c 3933 3037  cx_gate.359,9307
+00003e40: 0a76 6f69 6420 5368 6172 7169 743a 3a44  .void Sharqit::D
+00003e50: 4147 4369 7263 3a3a 6861 6461 6d61 7264  AGCirc::hadamard
+00003e60: 5f67 6174 655f 7265 6475 6374 696f 6e5f  _gate_reduction_
+00003e70: 3128 7f68 6164 616d 6172 645f 6761 7465  1(.hadamard_gate
+00003e80: 5f72 6564 7563 7469 6f6e 5f31 0133 3934  _reduction_1.394
+00003e90: 2c31 3035 3436 0a76 6f69 6420 5368 6172  ,10546.void Shar
+00003ea0: 7169 743a 3a44 4147 4369 7263 3a3a 6861  qit::DAGCirc::ha
+00003eb0: 6461 6d61 7264 5f67 6174 655f 7265 6475  damard_gate_redu
+00003ec0: 6374 696f 6e5f 3228 7f68 6164 616d 6172  ction_2(.hadamar
+00003ed0: 645f 6761 7465 5f72 6564 7563 7469 6f6e  d_gate_reduction
+00003ee0: 5f32 0134 3334 2c31 3138 3036 0a76 6f69  _2.434,11806.voi
+00003ef0: 6420 5368 6172 7169 743a 3a44 4147 4369  d Sharqit::DAGCi
+00003f00: 7263 3a3a 6861 6461 6d61 7264 5f67 6174  rc::hadamard_gat
+00003f10: 655f 7265 6475 6374 696f 6e5f 3328 7f68  e_reduction_3(.h
+00003f20: 6164 616d 6172 645f 6761 7465 5f72 6564  adamard_gate_red
+00003f30: 7563 7469 6f6e 5f33 0134 3735 2c31 3330  uction_3.475,130
+00003f40: 3837 0a75 696e 7433 325f 7420 5368 6172  87.uint32_t Shar
+00003f50: 7169 743a 3a44 4147 4369 7263 3a3a 6861  qit::DAGCirc::ha
+00003f60: 6461 6d61 7264 5f67 6174 655f 7265 6475  damard_gate_redu
+00003f70: 6374 696f 6e28 7f68 6164 616d 6172 645f  ction(.hadamard_
+00003f80: 6761 7465 5f72 6564 7563 7469 6f6e 0135  gate_reduction.5
+00003f90: 3333 2c31 3530 3632 0a75 696e 7433 325f  33,15062.uint32_
+00003fa0: 7420 5368 6172 7169 743a 3a44 4147 4369  t Sharqit::DAGCi
+00003fb0: 7263 3a3a 7369 6e67 6c65 5f71 7562 6974  rc::single_qubit
+00003fc0: 5f67 6174 655f 6361 6e63 656c 6c61 7469  _gate_cancellati
+00003fd0: 6f6e 287f 7369 6e67 6c65 5f71 7562 6974  on(.single_qubit
+00003fe0: 5f67 6174 655f 6361 6e63 656c 6c61 7469  _gate_cancellati
+00003ff0: 6f6e 0135 3434 2c31 3532 3735 0a75 696e  on.544,15275.uin
+00004000: 7433 325f 7420 5368 6172 7169 743a 3a44  t32_t Sharqit::D
+00004010: 4147 4369 7263 3a3a 7477 6f5f 7175 6269  AGCirc::two_qubi
+00004020: 745f 6761 7465 5f63 616e 6365 6c6c 6174  t_gate_cancellat
+00004030: 696f 6e28 7f74 776f 5f71 7562 6974 5f67  ion(.two_qubit_g
+00004040: 6174 655f 6361 6e63 656c 6c61 7469 6f6e  ate_cancellation
+00004050: 0137 3430 2c32 3131 3035 0a76 6f69 6420  .740,21105.void 
+00004060: 5368 6172 7169 743a 3a44 4147 4369 7263  Sharqit::DAGCirc
+00004070: 3a3a 7275 6c65 5f62 6173 6564 5f67 6174  ::rule_based_gat
+00004080: 655f 7265 6475 6374 696f 6e28 7f72 756c  e_reduction(.rul
+00004090: 655f 6261 7365 645f 6761 7465 5f72 6564  e_based_gate_red
+000040a0: 7563 7469 6f6e 0138 3336 2c32 3339 3038  uction.836,23908
+000040b0: 0a0c 0a6c 696e 6561 725f 6d61 702e 6370  ...linear_map.cp
+000040c0: 702c 3434 310a 626f 6f6c 2053 6861 7271  p,441.bool Sharq
+000040d0: 6974 3a3a 4c69 6e65 6172 4d61 703a 3a69  it::LinearMap::i
+000040e0: 735f 7a65 726f 287f 6973 5f7a 6572 6f01  s_zero(.is_zero.
+000040f0: 382c 3130 340a 626f 6f6c 2053 6861 7271  8,104.bool Sharq
+00004100: 6974 3a3a 4c69 6e65 6172 4d61 703a 3a69  it::LinearMap::i
+00004110: 735f 6964 656e 7469 7479 287f 6973 5f69  s_identity(.is_i
+00004120: 6465 6e74 6974 7901 3231 2c34 3434 0a62  dentity.21,444.b
+00004130: 6f6f 6c20 5368 6172 7169 743a 3a4c 696e  ool Sharqit::Lin
+00004140: 6561 724d 6170 3a3a 6973 5f64 6961 676f  earMap::is_diago
+00004150: 6e61 6c28 7f69 735f 6469 6167 6f6e 616c  nal(.is_diagonal
+00004160: 0133 332c 3734 320a 626f 6f6c 2053 6861  .33,742.bool Sha
+00004170: 7271 6974 3a3a 4c69 6e65 6172 4d61 703a  rqit::LinearMap:
+00004180: 3a69 735f 6964 656e 7469 7479 5f6d 756c  :is_identity_mul
+00004190: 7469 706c 655f 636f 6e73 7461 6e74 287f  tiple_constant(.
+000041a0: 6973 5f69 6465 6e74 6974 795f 6d75 6c74  is_identity_mult
+000041b0: 6970 6c65 5f63 6f6e 7374 616e 7401 3435  iple_constant.45
+000041c0: 2c31 3033 360a 626f 6f6c 2053 6861 7271  ,1036.bool Sharq
+000041d0: 6974 3a3a 4c69 6e65 6172 4d61 703a 3a69  it::LinearMap::i
+000041e0: 735f 756e 6974 6172 7928 7f69 735f 756e  s_unitary(.is_un
+000041f0: 6974 6172 7901 3539 2c31 3432 390a 626f  itary.59,1429.bo
+00004200: 6f6c 2053 6861 7271 6974 3a3a 4c69 6e65  ol Sharqit::Line
+00004210: 6172 4d61 703a 3a69 735f 6571 7561 6c28  arMap::is_equal(
+00004220: 7f69 735f 6571 7561 6c01 3730 2c31 3639  .is_equal.70,169
+00004230: 300a 5368 6172 7169 743a 3a4c 696e 6561  0.Sharqit::Linea
+00004240: 724d 6170 2620 5368 6172 7169 743a 3a4c  rMap& Sharqit::L
+00004250: 696e 6561 724d 6170 3a3a 6f70 6572 6174  inearMap::operat
+00004260: 655f 7167 6174 6528 7f6f 7065 7261 7465  e_qgate(.operate
+00004270: 5f71 6761 7465 0138 312c 3139 3433 0a0c  _qgate.81,1943..
+00004280: 0a73 6861 7271 6974 2e68 2c34 390a 2364  .sharqit.h,49.#d
+00004290: 6566 696e 6520 5348 4152 5149 545f 487f  efine SHARQIT_H.
+000042a0: 372c 3838 0a6e 616d 6573 7061 6365 2053  7,88.namespace S
+000042b0: 6861 7271 6974 207f 3139 2c32 3934 0a0c  harqit .19,294..
+000042c0: 0a73 6861 7271 6974 2e63 7070 2c31 3736  .sharqit.cpp,176
+000042d0: 0a76 6f69 6420 7072 696e 745f 6865 6c70  .void print_help
+000042e0: 287f 3131 2c31 3330 0a76 6f69 6420 6f70  (.11,130.void op
+000042f0: 7469 6d69 7a65 287f 3537 2c32 3633 320a  timize(.57,2632.
+00004300: 766f 6964 2076 6572 6966 795f 6571 7561  void verify_equa
+00004310: 6c69 7479 287f 3737 2c33 3134 390a 766f  lity(.77,3149.vo
+00004320: 6964 2072 616e 646f 6d5f 7163 6972 6328  id random_qcirc(
+00004330: 7f39 382c 3337 3134 0a76 6f69 6420 7072  .98,3714.void pr
+00004340: 696e 745f 7374 6174 7328 7f31 3236 2c34  int_stats(.126,4
+00004350: 3530 310a 766f 6964 2073 686f 775f 7163  501.void show_qc
+00004360: 6972 6328 7f31 3432 2c34 3832 300a 696e  irc(.142,4820.in
+00004370: 7420 6d61 696e 287f 3135 392c 3531 3537  t main(.159,5157
+00004380: 0a0c 0a73 696d 706c 6966 792e 6370 702c  ...simplify.cpp,
+00004390: 3131 3536 0a76 6f69 6420 5368 6172 7169  1156.void Sharqi
+000043a0: 743a 3a5a 5844 6961 6772 616d 3a3a 6675  t::ZXDiagram::fu
+000043b0: 7365 5f73 7069 6465 7273 287f 6675 7365  se_spiders(.fuse
+000043c0: 5f73 7069 6465 7273 0138 2c31 3432 0a76  _spiders.8,142.v
+000043d0: 6f69 6420 5368 6172 7169 743a 3a5a 5844  oid Sharqit::ZXD
+000043e0: 6961 6772 616d 3a3a 636f 6e76 5f78 5f74  iagram::conv_x_t
+000043f0: 6f5f 7a28 7f63 6f6e 765f 785f 746f 5f7a  o_z(.conv_x_to_z
+00004400: 0136 382c 3136 3936 0a76 6f69 6420 5368  .68,1696.void Sh
+00004410: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+00004420: 3a3a 7265 6d6f 7665 5f70 6172 616c 6c65  ::remove_paralle
+00004430: 6c5f 7365 6c66 6c6f 6f70 735f 6861 6461  l_selfloops_hada
+00004440: 6d61 7264 5f65 6467 6573 287f 7265 6d6f  mard_edges(.remo
+00004450: 7665 5f70 6172 616c 6c65 6c5f 7365 6c66  ve_parallel_self
+00004460: 6c6f 6f70 735f 6861 6461 6d61 7264 5f65  loops_hadamard_e
+00004470: 6467 6573 0138 372c 3232 3436 0a76 6f69  dges.87,2246.voi
+00004480: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
+00004490: 6772 616d 3a3a 7570 6461 7465 5f6e 6f64  gram::update_nod
+000044a0: 655f 706c 6163 6573 287f 7570 6461 7465  e_places(.update
+000044b0: 5f6e 6f64 655f 706c 6163 6573 0131 3138  _node_places.118
+000044c0: 2c33 3334 340a 766f 6964 2053 6861 7271  ,3344.void Sharq
+000044d0: 6974 3a3a 5a58 4469 6167 7261 6d3a 3a75  it::ZXDiagram::u
+000044e0: 7064 6174 655f 7068 6173 655f 6761 6467  pdate_phase_gadg
+000044f0: 6574 287f 7570 6461 7465 5f70 6861 7365  et(.update_phase
+00004500: 5f67 6164 6765 7401 3134 322c 3431 3036  _gadget.142,4106
+00004510: 0a76 6f69 6420 5368 6172 7169 743a 3a5a  .void Sharqit::Z
+00004520: 5844 6961 6772 616d 3a3a 6772 6170 685f  XDiagram::graph_
+00004530: 6c69 6b65 287f 6772 6170 685f 6c69 6b65  like(.graph_like
+00004540: 0131 3635 2c34 3738 300a 766f 6964 2053  .165,4780.void S
+00004550: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
+00004560: 6d3a 3a6c 636f 6d70 5f6f 6e65 5f74 696d  m::lcomp_one_tim
+00004570: 6528 7f6c 636f 6d70 5f6f 6e65 5f74 696d  e(.lcomp_one_tim
+00004580: 6501 3232 382c 3635 3030 0a75 696e 7433  e.228,6500.uint3
+00004590: 325f 7420 5368 6172 7169 743a 3a5a 5844  2_t Sharqit::ZXD
+000045a0: 6961 6772 616d 3a3a 6c63 6f6d 7028 7f6c  iagram::lcomp(.l
+000045b0: 636f 6d70 0132 3433 2c36 3938 300a 766f  comp.243,6980.vo
+000045c0: 6964 2053 6861 7271 6974 3a3a 5a58 4469  id Sharqit::ZXDi
+000045d0: 6167 7261 6d3a 3a70 6976 6f74 315f 6f6e  agram::pivot1_on
+000045e0: 655f 7469 6d65 287f 7069 766f 7431 5f6f  e_time(.pivot1_o
+000045f0: 6e65 5f74 696d 6501 3239 352c 3833 3436  ne_time.295,8346
+00004600: 0a75 696e 7433 325f 7420 5368 6172 7169  .uint32_t Sharqi
+00004610: 743a 3a5a 5844 6961 6772 616d 3a3a 7069  t::ZXDiagram::pi
+00004620: 766f 7431 287f 7069 766f 7431 0133 3531  vot1(.pivot1.351
+00004630: 2c31 3032 3730 0a76 6f69 6420 5368 6172  ,10270.void Shar
+00004640: 7169 743a 3a5a 5844 6961 6772 616d 3a3a  qit::ZXDiagram::
+00004650: 7069 766f 7432 5f6f 6e65 5f74 696d 6528  pivot2_one_time(
+00004660: 7f70 6976 6f74 325f 6f6e 655f 7469 6d65  .pivot2_one_time
+00004670: 0134 3331 2c31 3232 3830 0a75 696e 7433  .431,12280.uint3
+00004680: 325f 7420 5368 6172 7169 743a 3a5a 5844  2_t Sharqit::ZXD
+00004690: 6961 6772 616d 3a3a 7069 766f 7432 287f  iagram::pivot2(.
+000046a0: 7069 766f 7432 0135 3131 2c31 3439 3736  pivot2.511,14976
+000046b0: 0a76 6f69 6420 5368 6172 7169 743a 3a5a  .void Sharqit::Z
+000046c0: 5844 6961 6772 616d 3a3a 7069 766f 7433  XDiagram::pivot3
+000046d0: 5f6f 6e65 5f74 696d 6528 7f70 6976 6f74  _one_time(.pivot
+000046e0: 335f 6f6e 655f 7469 6d65 0135 3932 2c31  3_one_time.592,1
+000046f0: 3730 3338 0a75 696e 7433 325f 7420 5368  7038.uint32_t Sh
+00004700: 6172 7169 743a 3a5a 5844 6961 6772 616d  arqit::ZXDiagram
+00004710: 3a3a 7069 766f 7433 287f 7069 766f 7433  ::pivot3(.pivot3
+00004720: 0136 3932 2c32 3033 3633 0a76 6f69 6420  .692,20363.void 
+00004730: 5368 6172 7169 743a 3a5a 5844 6961 6772  Sharqit::ZXDiagr
+00004740: 616d 3a3a 6964 5f72 656d 6f76 616c 287f  am::id_removal(.
+00004750: 6964 5f72 656d 6f76 616c 0137 3833 2c32  id_removal.783,2
+00004760: 3236 3930 0a76 6f69 6420 5368 6172 7169  2690.void Sharqi
+00004770: 743a 3a5a 5844 6961 6772 616d 3a3a 6766  t::ZXDiagram::gf
+00004780: 7573 696f 6e5f 6f6e 655f 7469 6d65 287f  usion_one_time(.
+00004790: 6766 7573 696f 6e5f 6f6e 655f 7469 6d65  gfusion_one_time
+000047a0: 0138 3338 2c32 3433 3239 0a75 696e 7433  .838,24329.uint3
+000047b0: 325f 7420 5368 6172 7169 743a 3a5a 5844  2_t Sharqit::ZXD
+000047c0: 6961 6772 616d 3a3a 6766 7573 696f 6e28  iagram::gfusion(
+000047d0: 7f67 6675 7369 6f6e 0138 3436 2c32 3436  .gfusion.846,246
+000047e0: 3438 0a76 6f69 6420 5368 6172 7169 743a  48.void Sharqit:
+000047f0: 3a5a 5844 6961 6772 616d 3a3a 7369 6d70  :ZXDiagram::simp
+00004800: 6c69 6679 287f 7369 6d70 6c69 6679 0139  lify(.simplify.9
+00004810: 3739 2c32 3834 3437 0a0c 0a70 6861 7365  79,28447...phase
+00004820: 2e68 2c39 3134 0a23 6465 6669 6e65 2050  .h,914.#define P
+00004830: 4841 5345 5f48 7f37 2c38 300a 2020 636c  HASE_H.7,80.  cl
+00004840: 6173 7320 5068 6173 657f 3233 2c32 3936  ass Phase.23,296
+00004850: 0a20 2020 2046 7261 6374 696f 6e20 6672  .    Fraction fr
+00004860: 6163 5f3b 7f32 362c 3332 350a 2020 2020  ac_;.26,325.    
+00004870: 5068 6173 6528 7f33 332c 3632 380a 2020  Phase(.33,628.  
+00004880: 2020 5068 6173 6528 7f33 382c 3834 370a    Phase(.38,847.
+00004890: 2020 2020 5068 6173 6528 7f34 332c 3130      Phase(.43,10
+000048a0: 3431 0a20 2020 2050 6861 7365 287f 3438  41.    Phase(.48
+000048b0: 2c31 3136 370a 2020 2020 4672 6163 7469  ,1167.    Fracti
+000048c0: 6f6e 2066 7261 6328 7f35 302c 3132 3439  on frac(.50,1249
+000048d0: 0a20 2020 2076 6f69 6420 6672 6163 287f  .    void frac(.
+000048e0: 3532 2c31 3332 310a 2020 2020 646f 7562  52,1321.    doub
+000048f0: 6c65 2076 616c 7565 287f 3632 2c31 3630  le value(.62,160
+00004900: 380a 2020 2020 626f 6f6c 2069 735f 7a65  8.    bool is_ze
+00004910: 726f 287f 3637 2c31 3830 350a 2020 2020  ro(.67,1805.    
+00004920: 626f 6f6c 2069 735f 706f 7369 7469 7665  bool is_positive
+00004930: 287f 3732 2c31 3938 330a 2020 2020 626f  (.72,1983.    bo
+00004940: 6f6c 2069 735f 6e65 6761 7469 7665 287f  ol is_negative(.
+00004950: 3737 2c32 3136 350a 2020 2020 766f 6964  77,2165.    void
+00004960: 2072 6564 7563 6528 7f38 312c 3233 3032   reduce(.81,2302
+00004970: 0a20 2020 2076 6f69 6420 6d6f 645f 3270  .    void mod_2p
+00004980: 6928 7f38 352c 3233 3931 0a20 2020 2050  i(.85,2391.    P
+00004990: 6861 7365 206f 7065 7261 746f 722b 287f  hase operator+(.
+000049a0: 3939 2c32 3839 320a 2020 2020 5068 6173  99,2892.    Phas
+000049b0: 6520 6f70 6572 6174 6f72 2d28 7f31 3030  e operator-(.100
+000049c0: 2c32 3933 380a 2020 2020 5068 6173 6526  ,2938.    Phase&
+000049d0: 206f 7065 7261 746f 722b 3d28 7f6f 7065   operator+=(.ope
+000049e0: 7261 746f 722b 3d01 3130 312c 3239 3932  rator+=.101,2992
+000049f0: 0a20 2020 2050 6861 7365 2620 6f70 6572  .    Phase& oper
+00004a00: 6174 6f72 2d3d 287f 6f70 6572 6174 6f72  ator-=(.operator
+00004a10: 2d3d 0131 3032 2c33 3037 310a 2020 2020  -=.102,3071.    
+00004a20: 5068 6173 6526 206f 7065 7261 746f 722a  Phase& operator*
+00004a30: 3d28 7f6f 7065 7261 746f 722a 3d01 3130  =(.operator*=.10
+00004a40: 332c 3331 3530 0a20 2020 2050 6861 7365  3,3150.    Phase
+00004a50: 2620 6f70 6572 6174 6f72 2f3d 287f 6f70  & operator/=(.op
+00004a60: 6572 6174 6f72 2f3d 0131 3034 2c33 3232  erator/=.104,322
+00004a70: 330a 2020 2020 6672 6965 6e64 2062 6f6f  3.    friend boo
+00004a80: 6c20 6f70 6572 6174 6f72 3d3d 287f 6f70  l operator==(.op
+00004a90: 6572 6174 6f72 3d3d 0131 3035 2c33 3239  erator==.105,329
+00004aa0: 360a 2020 2020 6672 6965 6e64 2062 6f6f  6.    friend boo
+00004ab0: 6c20 6f70 6572 6174 6f72 213d 287f 6f70  l operator!=(.op
+00004ac0: 6572 6174 6f72 213d 0131 3130 2c33 3530  erator!=.110,350
+00004ad0: 360a 2020 2020 6672 6965 6e64 2050 6861  6.    friend Pha
+00004ae0: 7365 206f 7065 7261 746f 722b 287f 3131  se operator+(.11
+00004af0: 312c 3335 3935 0a20 2020 2066 7269 656e  1,3595.    frien
+00004b00: 6420 5068 6173 6520 6f70 6572 6174 6f72  d Phase operator
+00004b10: 2d28 7f31 3132 2c33 3730 310a 2020 2020  -(.112,3701.    
+00004b20: 6672 6965 6e64 2050 6861 7365 206f 7065  friend Phase ope
+00004b30: 7261 746f 722a 287f 3131 332c 3338 3037  rator*(.113,3807
+00004b40: 0a20 2020 2066 7269 656e 6420 5068 6173  .    friend Phas
+00004b50: 6520 6f70 6572 6174 6f72 2a28 7f31 3134  e operator*(.114
+00004b60: 2c33 3930 370a 2020 2020 6672 6965 6e64  ,3907.    friend
+00004b70: 2050 6861 7365 206f 7065 7261 746f 722f   Phase operator/
+00004b80: 287f 3131 352c 3430 3037 0a20 2020 2066  (.115,4007.    f
+00004b90: 7269 656e 6420 7374 643a 3a6f 7374 7265  riend std::ostre
+00004ba0: 616d 2620 6f70 6572 6174 6f72 3c3c 287f  am& operator<<(.
+00004bb0: 3131 362c 3431 3037 0a0c 0a66 7261 6374  116,4107...fract
+00004bc0: 696f 6e2e 682c 3137 3132 0a23 6465 6669  ion.h,1712.#defi
+00004bd0: 6e65 2046 5241 4354 494f 4e5f 487f 372c  ne FRACTION_H.7,
+00004be0: 3839 0a20 2063 6c61 7373 2046 7261 6374  89.  class Fract
+00004bf0: 696f 6e7f 3138 2c32 3432 0a20 2020 2069  ion.18,242.    i
+00004c00: 6e74 3332 5f74 206e 756d 6572 6174 6f72  nt32_t numerator
+00004c10: 5f3b 7f32 312c 3237 340a 2020 2020 696e  _;.21,274.    in
+00004c20: 7433 325f 7420 6465 6e6f 6d69 6e61 746f  t32_t denominato
+00004c30: 725f 3b7f 3232 2c33 3239 0a20 2020 2046  r_;.22,329.    F
+00004c40: 7261 6374 696f 6e28 7f32 372c 3435 360a  raction(.27,456.
+00004c50: 2020 2020 4672 6163 7469 6f6e 287f 3333      Fraction(.33
+00004c60: 2c36 3739 0a20 2020 2046 7261 6374 696f  ,679.    Fractio
+00004c70: 6e28 7f33 392c 3931 390a 2020 2020 696e  n(.39,919.    in
+00004c80: 7433 325f 7420 6e75 6d65 7261 746f 7228  t32_t numerator(
+00004c90: 7f34 312c 3130 3533 0a20 2020 2069 6e74  .41,1053.    int
+00004ca0: 3332 5f74 2064 656e 6f6d 696e 6174 6f72  32_t denominator
+00004cb0: 287f 3433 2c31 3134 310a 2020 2020 766f  (.43,1141.    vo
+00004cc0: 6964 206e 756d 6572 6174 6f72 287f 3435  id numerator(.45
+00004cd0: 2c31 3233 310a 2020 2020 766f 6964 2064  ,1231.    void d
+00004ce0: 656e 6f6d 696e 6174 6f72 287f 3437 2c31  enominator(.47,1
+00004cf0: 3334 380a 2020 2020 4672 6163 7469 6f6e  348.    Fraction
+00004d00: 2061 6464 287f 3538 2c31 3730 390a 2020   add(.58,1709.  
+00004d10: 2020 4672 6163 7469 6f6e 2061 6464 287f    Fraction add(.
+00004d20: 3639 2c32 3133 300a 2020 2020 4672 6163  69,2130.    Frac
+00004d30: 7469 6f6e 2073 7562 287f 3735 2c32 3334  tion sub(.75,234
+00004d40: 390a 2020 2020 4672 6163 7469 6f6e 2073  9.    Fraction s
+00004d50: 7562 287f 3836 2c32 3737 320a 2020 2020  ub(.86,2772.    
+00004d60: 4672 6163 7469 6f6e 206d 756c 287f 3932  Fraction mul(.92
+00004d70: 2c32 3939 310a 2020 2020 4672 6163 7469  ,2991.    Fracti
+00004d80: 6f6e 206d 756c 287f 3130 332c 3333 3737  on mul(.103,3377
+00004d90: 0a20 2020 2046 7261 6374 696f 6e20 6469  .    Fraction di
+00004da0: 7628 7f31 3039 2c33 3539 310a 2020 2020  v(.109,3591.    
+00004db0: 4672 6163 7469 6f6e 2064 6976 287f 3132  Fraction div(.12
+00004dc0: 302c 3339 3736 0a20 2020 2062 6f6f 6c20  0,3976.    bool 
+00004dd0: 6973 5f7a 6572 6f28 7f31 3235 2c34 3137  is_zero(.125,417
+00004de0: 320a 2020 2020 626f 6f6c 2069 735f 706f  2.    bool is_po
+00004df0: 7369 7469 7665 287f 3133 302c 3433 3532  sitive(.130,4352
+00004e00: 0a20 2020 2062 6f6f 6c20 6973 5f6e 6567  .    bool is_neg
+00004e10: 6174 6976 6528 7f31 3335 2c34 3535 300a  ative(.135,4550.
+00004e20: 2020 2020 766f 6964 2072 6564 7563 6528      void reduce(
+00004e30: 7f31 3339 2c34 3637 310a 2020 2020 7374  .139,4671.    st
+00004e40: 6174 6963 2069 6e74 3332 5f74 2067 6364  atic int32_t gcd
+00004e50: 287f 3136 302c 3532 3739 0a20 2020 2046  (.160,5279.    F
+00004e60: 7261 6374 696f 6e20 6f70 6572 6174 6f72  raction operator
+00004e70: 2b28 7f31 3732 2c35 3533 350a 2020 2020  +(.172,5535.    
+00004e80: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+00004e90: 722d 287f 3137 332c 3535 3834 0a20 2020  r-(.173,5584.   
+00004ea0: 2046 7261 6374 696f 6e26 206f 7065 7261   Fraction& opera
+00004eb0: 746f 722b 3d28 7f6f 7065 7261 746f 722b  tor+=(.operator+
+00004ec0: 3d01 3137 342c 3536 3335 0a20 2020 2046  =.174,5635.    F
+00004ed0: 7261 6374 696f 6e26 206f 7065 7261 746f  raction& operato
+00004ee0: 722b 3d28 7f6f 7065 7261 746f 722b 3d01  r+=(.operator+=.
+00004ef0: 3138 312c 3538 3233 0a20 2020 2046 7261  181,5823.    Fra
+00004f00: 6374 696f 6e26 206f 7065 7261 746f 722d  ction& operator-
+00004f10: 3d28 7f6f 7065 7261 746f 722d 3d01 3138  =(.operator-=.18
+00004f20: 322c 3539 3035 0a20 2020 2046 7261 6374  2,5905.    Fract
+00004f30: 696f 6e26 206f 7065 7261 746f 722d 3d28  ion& operator-=(
+00004f40: 7f6f 7065 7261 746f 722d 3d01 3138 392c  .operator-=.189,
+00004f50: 3630 3933 0a20 2020 2046 7261 6374 696f  6093.    Fractio
+00004f60: 6e26 206f 7065 7261 746f 722a 3d28 7f6f  n& operator*=(.o
+00004f70: 7065 7261 746f 722a 3d01 3139 302c 3631  perator*=.190,61
+00004f80: 3735 0a20 2020 2046 7261 6374 696f 6e26  75.    Fraction&
+00004f90: 206f 7065 7261 746f 722a 3d28 7f6f 7065   operator*=(.ope
+00004fa0: 7261 746f 722a 3d01 3139 372c 3633 3633  rator*=.197,6363
+00004fb0: 0a20 2020 2046 7261 6374 696f 6e26 206f  .    Fraction& o
+00004fc0: 7065 7261 746f 722f 3d28 7f6f 7065 7261  perator/=(.opera
+00004fd0: 746f 722f 3d01 3139 382c 3634 3435 0a20  tor/=.198,6445. 
+00004fe0: 2020 2046 7261 6374 696f 6e26 206f 7065     Fraction& ope
+00004ff0: 7261 746f 722f 3d28 7f6f 7065 7261 746f  rator/=(.operato
+00005000: 722f 3d01 3230 352c 3636 3333 0a20 2020  r/=.205,6633.   
+00005010: 2066 7269 656e 6420 626f 6f6c 206f 7065   friend bool ope
+00005020: 7261 746f 723d 3d28 7f6f 7065 7261 746f  rator==(.operato
+00005030: 723d 3d01 3230 362c 3637 3135 0a20 2020  r==.206,6715.   
+00005040: 2066 7269 656e 6420 626f 6f6c 206f 7065   friend bool ope
+00005050: 7261 746f 7221 3d28 7f6f 7065 7261 746f  rator!=(.operato
+00005060: 7221 3d01 3231 302c 3638 3837 0a20 2020  r!=.210,6887.   
+00005070: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+00005080: 206f 7065 7261 746f 722b 287f 3231 312c   operator+(.211,
+00005090: 3639 3832 0a20 2020 2066 7269 656e 6420  6982.    friend 
+000050a0: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+000050b0: 722b 287f 3231 322c 3730 3739 0a20 2020  r+(.212,7079.   
+000050c0: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+000050d0: 206f 7065 7261 746f 722b 287f 3231 332c   operator+(.213,
+000050e0: 3731 3834 0a20 2020 2066 7269 656e 6420  7184.    friend 
+000050f0: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+00005100: 722d 287f 3231 342c 3732 3839 0a20 2020  r-(.214,7289.   
+00005110: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+00005120: 206f 7065 7261 746f 722d 287f 3231 352c   operator-(.215,
+00005130: 3733 3836 0a20 2020 2066 7269 656e 6420  7386.    friend 
+00005140: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+00005150: 722d 287f 3231 362c 3734 3931 0a20 2020  r-(.216,7491.   
+00005160: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+00005170: 206f 7065 7261 746f 722a 287f 3231 372c   operator*(.217,
+00005180: 3735 3936 0a20 2020 2066 7269 656e 6420  7596.    friend 
+00005190: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+000051a0: 722a 287f 3231 382c 3736 3933 0a20 2020  r*(.218,7693.   
+000051b0: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+000051c0: 206f 7065 7261 746f 722a 287f 3231 392c   operator*(.219,
+000051d0: 3737 3938 0a20 2020 2066 7269 656e 6420  7798.    friend 
+000051e0: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+000051f0: 722f 287f 3232 302c 3739 3033 0a20 2020  r/(.220,7903.   
+00005200: 2066 7269 656e 6420 4672 6163 7469 6f6e   friend Fraction
+00005210: 206f 7065 7261 746f 722f 287f 3232 312c   operator/(.221,
+00005220: 3830 3030 0a20 2020 2066 7269 656e 6420  8000.    friend 
+00005230: 4672 6163 7469 6f6e 206f 7065 7261 746f  Fraction operato
+00005240: 722f 287f 3232 322c 3831 3035 0a20 2020  r/(.222,8105.   
+00005250: 2066 7269 656e 6420 7374 643a 3a6f 7374   friend std::ost
+00005260: 7265 616d 2620 6f70 6572 6174 6f72 3c3c  ream& operator<<
+00005270: 287f 3232 332c 3832 3130 0a0c 0a7a 786e  (.223,8210...zxn
+00005280: 6f64 652e 6370 702c 3435 0a73 7464 3a3a  ode.cpp,45.std::
+00005290: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+000052a0: 5a58 4e6f 6465 3a3a 6e61 6d65 287f 6e61  ZXNode::name(.na
+000052b0: 6d65 0138 2c38 390a 0c0a 7a78 6469 6167  me.8,89...zxdiag
+000052c0: 7261 6d2e 6370 702c 3132 3036 0a53 6861  ram.cpp,1206.Sha
+000052d0: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
+000052e0: 3a5a 5844 6961 6772 616d 287f 5a58 4469  :ZXDiagram(.ZXDi
+000052f0: 6167 7261 6d01 382c 3935 0a73 7464 3a3a  agram.8,95.std::
+00005300: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+00005310: 5a58 4469 6167 7261 6d3a 3a74 6f5f 7374  ZXDiagram::to_st
+00005320: 7269 6e67 287f 746f 5f73 7472 696e 6701  ring(.to_string.
+00005330: 3334 2c38 3935 0a73 7464 3a3a 6d61 703c  34,895.std::map<
+00005340: 7374 643a 3a73 7472 696e 672c 2075 696e  std::string, uin
+00005350: 7433 325f 743e 2053 6861 7271 6974 3a3a  t32_t> Sharqit::
+00005360: 5a58 4469 6167 7261 6d3a 3a73 7461 7473  ZXDiagram::stats
+00005370: 287f 7374 6174 7301 3534 2c31 3430 340a  (.stats.54,1404.
+00005380: 766f 6964 2053 6861 7271 6974 3a3a 5a58  void Sharqit::ZX
+00005390: 4469 6167 7261 6d3a 3a74 6f5f 646f 745f  Diagram::to_dot_
+000053a0: 6669 6c65 287f 746f 5f64 6f74 5f66 696c  file(.to_dot_fil
+000053b0: 6501 3830 2c32 3337 380a 766f 6964 2053  e.80,2378.void S
+000053c0: 6861 7271 6974 3a3a 5a58 4469 6167 7261  harqit::ZXDiagra
+000053d0: 6d3a 3a74 6f5f 7376 675f 6669 6c65 287f  m::to_svg_file(.
+000053e0: 746f 5f73 7667 5f66 696c 6501 3232 342c  to_svg_file.224,
+000053f0: 3639 3039 0a76 6f69 6420 5368 6172 7169  6909.void Sharqi
+00005400: 743a 3a5a 5844 6961 6772 616d 3a3a 6164  t::ZXDiagram::ad
+00005410: 645f 7167 6174 6528 7f61 6464 5f71 6761  d_qgate(.add_qga
+00005420: 7465 0132 3337 2c37 3338 340a 626f 6f6c  te.237,7384.bool
+00005430: 2053 6861 7271 6974 3a3a 5a58 4469 6167   Sharqit::ZXDiag
+00005440: 7261 6d3a 3a63 6865 636b 5f63 6f6e 6e65  ram::check_conne
+00005450: 6374 287f 6368 6563 6b5f 636f 6e6e 6563  ct(.check_connec
+00005460: 7401 3337 382c 3132 3032 350a 766f 6964  t.378,12025.void
+00005470: 2053 6861 7271 6974 3a3a 5a58 4469 6167   Sharqit::ZXDiag
+00005480: 7261 6d3a 3a78 6f72 5f68 6164 616d 6172  ram::xor_hadamar
+00005490: 645f 6564 6765 287f 786f 725f 6861 6461  d_edge(.xor_hada
+000054a0: 6d61 7264 5f65 6467 6501 3430 312c 3132  mard_edge.401,12
+000054b0: 3433 330a 766f 6964 2053 6861 7271 6974  433.void Sharqit
+000054c0: 3a3a 5a58 4469 6167 7261 6d3a 3a78 6f72  ::ZXDiagram::xor
+000054d0: 5f68 6164 616d 6172 645f 6564 6765 7328  _hadamard_edges(
+000054e0: 7f78 6f72 5f68 6164 616d 6172 645f 6564  .xor_hadamard_ed
+000054f0: 6765 7301 3433 342c 3133 3433 370a 5368  ges.434,13437.Sh
+00005500: 6172 7169 743a 3a5a 584e 6f64 654b 696e  arqit::ZXNodeKin
+00005510: 6420 5368 6172 7169 743a 3a5a 5844 6961  d Sharqit::ZXDia
+00005520: 6772 616d 3a3a 7265 6d6f 7665 5f6e 6f64  gram::remove_nod
+00005530: 6528 7f72 656d 6f76 655f 6e6f 6465 0134  e(.remove_node.4
+00005540: 3436 2c31 3338 3037 0a53 6861 7271 6974  46,13807.Sharqit
+00005550: 3a3a 5a58 4564 6765 4b69 6e64 2053 6861  ::ZXEdgeKind Sha
+00005560: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
+00005570: 3a72 656d 6f76 655f 6564 6765 287f 7265  :remove_edge(.re
+00005580: 6d6f 7665 5f65 6467 6501 3438 302c 3134  move_edge.480,14
+00005590: 3530 360a 7569 6e74 3332 5f74 2053 6861  506.uint32_t Sha
+000055a0: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
+000055b0: 3a61 7070 656e 645f 6e6f 6465 287f 6170  :append_node(.ap
+000055c0: 7065 6e64 5f6e 6f64 6501 3530 342c 3135  pend_node.504,15
+000055d0: 3034 370a 7569 6e74 3332 5f74 2053 6861  047.uint32_t Sha
+000055e0: 7271 6974 3a3a 5a58 4469 6167 7261 6d3a  rqit::ZXDiagram:
+000055f0: 3a61 7070 656e 645f 6e6f 6465 287f 6170  :append_node(.ap
+00005600: 7065 6e64 5f6e 6f64 6501 3531 322c 3135  pend_node.512,15
+00005610: 3234 310a 766f 6964 2053 6861 7271 6974  241.void Sharqit
+00005620: 3a3a 5a58 4469 6167 7261 6d3a 3a63 6f6e  ::ZXDiagram::con
+00005630: 6e65 6374 5f6e 6f64 6573 287f 636f 6e6e  nect_nodes(.conn
+00005640: 6563 745f 6e6f 6465 7301 3532 352c 3135  ect_nodes.525,15
+00005650: 3538 330a 766f 6964 2053 6861 7271 6974  583.void Sharqit
+00005660: 3a3a 5a58 4469 6167 7261 6d3a 3a73 7761  ::ZXDiagram::swa
+00005670: 705f 6e6f 6465 7328 7f73 7761 705f 6e6f  p_nodes(.swap_no
+00005680: 6465 7301 3533 332c 3135 3833 390a 766f  des.533,15839.vo
+00005690: 6964 2053 6861 7271 6974 3a3a 5a58 4469  id Sharqit::ZXDi
+000056a0: 6167 7261 6d3a 3a72 656d 6f76 655f 6973  agram::remove_is
+000056b0: 6f6c 6174 6564 5f73 7069 6465 7273 287f  olated_spiders(.
+000056c0: 7265 6d6f 7665 5f69 736f 6c61 7465 645f  remove_isolated_
+000056d0: 7370 6964 6572 7301 3534 382c 3136 3232  spiders.548,1622
+000056e0: 350a 766f 6964 2053 6861 7271 6974 3a3a  5.void Sharqit::
+000056f0: 5a58 4469 6167 7261 6d3a 3a72 6f77 5f6f  ZXDiagram::row_o
+00005700: 7065 7261 7469 6f6e 287f 726f 775f 6f70  peration(.row_op
+00005710: 6572 6174 696f 6e01 3536 342c 3136 3534  eration.564,1654
+00005720: 380a 7374 643a 3a76 6563 746f 723c 7569  8.std::vector<ui
+00005730: 6e74 3332 5f74 3e20 5368 6172 7169 743a  nt32_t> Sharqit:
+00005740: 3a5a 5844 6961 6772 616d 3a3a 6164 6a61  :ZXDiagram::adja
+00005750: 6365 6e74 5f6e 6f64 655f 696e 6465 7865  cent_node_indexe
+00005760: 7328 7f61 646a 6163 656e 745f 6e6f 6465  s(.adjacent_node
+00005770: 5f69 6e64 6578 6573 0135 3733 2c31 3637  _indexes.573,167
+00005780: 3636 0a0c 0a62 696e 6172 795f 6d61 7472  66...binary_matr
+00005790: 6978 2e63 7070 2c31 3632 0a73 7464 3a3a  ix.cpp,162.std::
+000057a0: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+000057b0: 4269 6e61 7279 4d61 7472 6978 3a3a 746f  BinaryMatrix::to
+000057c0: 5f73 7472 696e 6728 7f74 6f5f 7374 7269  _string(.to_stri
+000057d0: 6e67 0138 2c31 3133 0a73 7464 3a3a 7665  ng.8,113.std::ve
+000057e0: 6374 6f72 3c73 7464 3a3a 7061 6972 3c75  ctor<std::pair<u
+000057f0: 696e 7433 325f 742c 2075 696e 7433 325f  int32_t, uint32_
+00005800: 743e 3e20 5368 6172 7169 743a 3a42 696e  t>> Sharqit::Bin
+00005810: 6172 794d 6174 7269 783a 3a67 6175 7373  aryMatrix::gauss
+00005820: 5f72 6564 7563 6528 7f67 6175 7373 5f72  _reduce(.gauss_r
+00005830: 6564 7563 6501 3238 2c34 3930 0a0c 0a7a  educe.28,490...z
+00005840: 782e 682c 3331 3932 0a23 6465 6669 6e65  x.h,3192.#define
+00005850: 205a 585f 487f 3131 2c38 3933 0a20 2065   ZX_H.11,893.  e
+00005860: 6e75 6d20 5a58 4e6f 6465 4b69 6e64 207f  num ZXNodeKind .
+00005870: 3235 2c31 3038 320a 0909 2020 2058 5370  25,1082...   XSp
+00005880: 6964 6572 2c7f 3236 2c31 3130 320a 0909  ider,.26,1102...
+00005890: 2020 205a 5370 6964 6572 2c7f 3237 2c31     ZSpider,.27,1
+000058a0: 3133 300a 0909 2020 2049 6e70 7574 2c7f  130...   Input,.
+000058b0: 3238 2c31 3135 380a 0909 2020 204f 7574  28,1158...   Out
+000058c0: 7075 7420 7f32 392c 3131 3836 0a20 2065  put .29,1186.  e
+000058d0: 6e75 6d20 5a58 4564 6765 4b69 6e64 207f  num ZXEdgeKind .
+000058e0: 3332 2c31 3235 340a 0909 2020 204e 6f6e  32,1254...   Non
+000058f0: 652c 7f33 332c 3132 3734 0a09 0920 2020  e,.33,1274...   
+00005900: 506c 6169 6e2c 7f33 342c 3133 3132 0a09  Plain,.34,1312..
+00005910: 0920 2020 4861 6461 6d61 7264 207f 3335  .   Hadamard .35
+00005920: 2c31 3337 380a 2020 656e 756d 205a 5844  ,1378.  enum ZXD
+00005930: 6961 6772 616d 4b69 6e64 207f 3338 2c31  iagramKind .38,1
+00005940: 3436 310a 0909 2020 2020 2020 4765 6e65  461...      Gene
+00005950: 7261 6c2c 7f33 392c 3134 3834 0a09 0920  ral,.39,1484... 
+00005960: 2020 2020 2047 7261 7068 4c69 6b65 207f       GraphLike .
+00005970: 3430 2c31 3532 350a 2020 656e 756d 205a  40,1525.  enum Z
+00005980: 584e 6f64 6550 6c61 6365 207f 3433 2c31  XNodePlace .43,1
+00005990: 3630 300a 0909 2020 2020 5465 726d 696e  600...    Termin
+000059a0: 616c 2c7f 3434 2c31 3632 310a 0909 2020  al,.44,1621...  
+000059b0: 2020 426f 756e 6461 7279 2c7f 3435 2c31    Boundary,.45,1
+000059c0: 3636 360a 0909 2020 2020 496e 7465 726e  666...    Intern
+000059d0: 616c 207f 3436 2c31 3734 360a 2020 636c  al .46,1746.  cl
+000059e0: 6173 7320 5a58 4e6f 6465 7f35 392c 3232  ass ZXNode.59,22
+000059f0: 3332 0a20 2020 205a 584e 6f64 654b 696e  32.    ZXNodeKin
+00005a00: 6420 6b69 6e64 5f3b 7f36 322c 3232 3632  d kind_;.62,2262
+00005a10: 0a20 2020 2050 6861 7365 2070 6861 7365  .    Phase phase
+00005a20: 5f3b 7f36 332c 3233 3230 0a20 2020 2075  _;.63,2320.    u
+00005a30: 696e 7433 325f 7420 715f 3b7f 3634 2c32  int32_t q_;.64,2
+00005a40: 3337 350a 2020 2020 626f 6f6c 2070 675f  375.    bool pg_
+00005a50: 7068 6173 655f 3b7f 3635 2c32 3434 300a  phase_;.65,2440.
+00005a60: 2020 2020 626f 6f6c 2070 675f 726f 6f74      bool pg_root
+00005a70: 5f3b 7f36 362c 3235 3235 0a20 2020 2062  _;.66,2525.    b
+00005a80: 6f6f 6c20 7067 5f6c 6561 665f 3b7f 3637  ool pg_leaf_;.67
+00005a90: 2c32 3630 380a 2020 2020 5a58 4e6f 6465  ,2608.    ZXNode
+00005aa0: 287f 3738 2c33 3132 370a 2020 2020 5a58  (.78,3127.    ZX
+00005ab0: 4e6f 6465 287f 3835 2c33 3532 320a 2020  Node(.85,3522.  
+00005ac0: 2020 5a58 4e6f 6465 4b69 6e64 206b 696e    ZXNodeKind kin
+00005ad0: 6428 7f38 382c 3337 3230 0a20 2020 2050  d(.88,3720.    P
+00005ae0: 6861 7365 2070 6861 7365 287f 3930 2c33  hase phase(.90,3
+00005af0: 3739 350a 2020 2020 7569 6e74 3332 5f74  795.    uint32_t
+00005b00: 2071 287f 3932 2c33 3836 330a 2020 2020   q(.92,3863.    
+00005b10: 626f 6f6c 2070 675f 7068 6173 6528 7f39  bool pg_phase(.9
+00005b20: 342c 3339 3333 0a20 2020 2062 6f6f 6c20  4,3933.    bool 
+00005b30: 7067 5f72 6f6f 7428 7f39 362c 3430 3132  pg_root(.96,4012
+00005b40: 0a20 2020 2062 6f6f 6c20 7067 5f6c 6561  .    bool pg_lea
+00005b50: 6628 7f39 382c 3430 3839 0a20 2020 2076  f(.98,4089.    v
+00005b60: 6f69 6420 6b69 6e64 287f 3130 302c 3431  oid kind(.100,41
+00005b70: 3633 0a20 2020 2076 6f69 6420 7068 6173  63.    void phas
+00005b80: 6528 7f31 3032 2c34 3234 370a 2020 2020  e(.102,4247.    
+00005b90: 766f 6964 2071 287f 3130 342c 3433 3236  void q(.104,4326
+00005ba0: 0a20 2020 2076 6f69 6420 7067 5f70 6861  .    void pg_pha
+00005bb0: 7365 287f 3130 362c 3433 3939 0a20 2020  se(.106,4399.   
+00005bc0: 2076 6f69 6420 7067 5f72 6f6f 7428 7f31   void pg_root(.1
+00005bd0: 3038 2c34 3439 350a 2020 2020 766f 6964  08,4495.    void
+00005be0: 2070 675f 6c65 6166 287f 3131 302c 3435   pg_leaf(.110,45
+00005bf0: 3837 0a20 2020 2073 7464 3a3a 7374 7269  87.    std::stri
+00005c00: 6e67 206b 696e 645f 7374 7228 7f31 3135  ng kind_str(.115
+00005c10: 2c34 3735 370a 2020 636c 6173 7320 5a58  ,4757.  class ZX
+00005c20: 4564 6765 7f31 3332 2c35 3134 300a 2020  Edge.132,5140.  
+00005c30: 2020 5a58 4564 6765 4b69 6e64 206b 696e    ZXEdgeKind kin
+00005c40: 645f 3b7f 3133 352c 3531 3730 0a20 2020  d_;.135,5170.   
+00005c50: 2075 696e 7433 325f 7420 746f 5f3b 7f31   uint32_t to_;.1
+00005c60: 3336 2c35 3232 380a 2020 2020 5a58 4564  36,5228.    ZXEd
+00005c70: 6765 287f 3134 332c 3534 3839 0a20 2020  ge(.143,5489.   
+00005c80: 205a 5845 6467 6528 7f31 3438 2c35 3638   ZXEdge(.148,568
+00005c90: 380a 2020 2020 5a58 4564 6765 4b69 6e64  8.    ZXEdgeKind
+00005ca0: 206b 696e 6428 7f31 3530 2c35 3738 350a   kind(.150,5785.
+00005cb0: 2020 2020 7569 6e74 3332 5f74 2074 6f28      uint32_t to(
+00005cc0: 7f31 3532 2c35 3835 370a 2020 2020 766f  .152,5857.    vo
+00005cd0: 6964 206b 696e 6428 7f31 3534 2c35 3932  id kind(.154,592
+00005ce0: 350a 2020 2020 766f 6964 2074 6f28 7f31  5.    void to(.1
+00005cf0: 3536 2c36 3030 360a 2020 2020 7374 643a  56,6006.    std:
+00005d00: 3a73 7472 696e 6720 6b69 6e64 5f73 7472  :string kind_str
+00005d10: 287f 3136 312c 3631 3630 0a20 2020 2073  (.161,6160.    s
+00005d20: 7464 3a3a 7374 7269 6e67 206e 616d 6528  td::string name(
+00005d30: 7f31 3639 2c36 3338 370a 2020 2020 766f  .169,6387.    vo
+00005d40: 6964 2072 6576 6572 7365 5f6b 696e 6428  id reverse_kind(
+00005d50: 7f31 3831 2c36 3732 360a 2020 636c 6173  .181,6726.  clas
+00005d60: 7320 5a58 4469 6167 7261 6d7f 3139 382c  s ZXDiagram.198,
+00005d70: 3737 3134 0a20 2020 205a 5844 6961 6772  7714.    ZXDiagr
+00005d80: 616d 4b69 6e64 206b 696e 645f 3b7f 3230  amKind kind_;.20
+00005d90: 312c 3737 3437 0a20 2020 2075 696e 7433  1,7747.    uint3
+00005da0: 325f 7420 7175 6269 745f 6e75 6d5f 3b7f  2_t qubit_num_;.
+00005db0: 3230 322c 3738 3030 0a20 2020 2073 7464  202,7800.    std
+00005dc0: 3a3a 7665 6374 6f72 3c5a 584e 6f64 653e  ::vector<ZXNode>
+00005dd0: 206e 6f64 6573 5f3b 7f32 3033 2c37 3834   nodes_;.203,784
+00005de0: 370a 2020 2020 7374 643a 3a76 6563 746f  7.    std::vecto
+00005df0: 723c 7569 6e74 3332 5f74 3e20 696e 7075  r<uint32_t> inpu
+00005e00: 7473 5f3b 7f32 3034 2c37 3931 330a 2020  ts_;.204,7913.  
+00005e10: 2020 7374 643a 3a76 6563 746f 723c 7569    std::vector<ui
+00005e20: 6e74 3332 5f74 3e20 6f75 7470 7574 735f  nt32_t> outputs_
+00005e30: 3b7f 3230 352c 3739 3836 0a20 2020 2073  ;.205,7986.    s
+00005e40: 7464 3a3a 7665 6374 6f72 3c73 7464 3a3a  td::vector<std::
+00005e50: 7665 6374 6f72 3c5a 5845 6467 653e 3e20  vector<ZXEdge>> 
+00005e60: 6164 6a5f 6d61 745f 3b7f 3230 362c 3830  adj_mat_;.206,80
+00005e70: 3631 0a20 2020 2073 7464 3a3a 7665 6374  61.    std::vect
+00005e80: 6f72 3c5a 584e 6f64 6550 6c61 6365 3e20  or<ZXNodePlace> 
+00005e90: 6e6f 6465 5f70 6c61 6365 735f 3b7f 3230  node_places_;.20
+00005ea0: 372c 3831 3437 0a20 2020 2075 696e 7433  7,8147.    uint3
+00005eb0: 325f 7420 6d61 785f 6164 6a5f 6e75 6d28  2_t max_adj_num(
+00005ec0: 7f32 3131 2c38 3332 370a 2020 2020 626f  .211,8327.    bo
+00005ed0: 6f6c 2063 6865 636b 5f78 5f73 7069 6465  ol check_x_spide
+00005ee0: 7228 7f32 3234 2c38 3734 300a 2020 2020  r(.224,8740.    
+00005ef0: 626f 6f6c 2063 6865 636b 5f7a 5f73 7069  bool check_z_spi
+00005f00: 6465 7228 7f32 3330 2c39 3038 370a 2020  der(.230,9087.  
+00005f10: 2020 626f 6f6c 2063 6865 636b 5f7a 6572    bool check_zer
+00005f20: 6f5f 7068 6173 655f 7370 6964 6572 287f  o_phase_spider(.
+00005f30: 3233 362c 3934 3532 0a20 2020 2062 6f6f  236,9452.    boo
+00005f40: 6c20 6368 6563 6b5f 7061 756c 695f 7370  l check_pauli_sp
+00005f50: 6964 6572 287f 3234 372c 3939 3537 0a20  ider(.247,9957. 
+00005f60: 2020 2062 6f6f 6c20 6368 6563 6b5f 7072     bool check_pr
+00005f70: 6f70 6572 5f63 6c69 6666 6f72 645f 7370  oper_clifford_sp
+00005f80: 6964 6572 287f 3235 382c 3130 3531 390a  ider(.258,10519.
+00005f90: 2020 2020 626f 6f6c 2063 6865 636b 5f63      bool check_c
+00005fa0: 6c69 6666 6f72 645f 7370 6964 6572 287f  lifford_spider(.
+00005fb0: 3236 392c 3131 3038 310a 2020 2020 626f  269,11081.    bo
+00005fc0: 6f6c 2063 6865 636b 5f6e 6f6e 5f63 6c69  ol check_non_cli
+00005fd0: 6666 6f72 645f 7370 6964 6572 287f 3237  fford_spider(.27
+00005fe0: 382c 3131 3439 300a 2020 2020 626f 6f6c  8,11490.    bool
+00005ff0: 2063 6865 636b 5f69 6e74 6572 6e61 6c5f   check_internal_
+00006000: 6e6f 6465 287f 3238 342c 3131 3833 350a  node(.284,11835.
+00006010: 2020 2020 626f 6f6c 2063 6865 636b 5f62      bool check_b
+00006020: 6f75 6e64 6172 795f 6e6f 6465 287f 3239  oundary_node(.29
+00006030: 302c 3132 3138 390a 2020 2020 626f 6f6c  0,12189.    bool
+00006040: 2063 6865 636b 5f70 675f 7068 6173 655f   check_pg_phase_
+00006050: 6e6f 6465 287f 3239 362c 3132 3537 330a  node(.296,12573.
+00006060: 2020 2020 626f 6f6c 2063 6865 636b 5f70      bool check_p
+00006070: 675f 726f 6f74 5f6e 6f64 6528 7f33 3032  g_root_node(.302
+00006080: 2c31 3239 3335 0a20 2020 2062 6f6f 6c20  ,12935.    bool 
+00006090: 6368 6563 6b5f 7067 5f6c 6561 665f 6e6f  check_pg_leaf_no
+000060a0: 6465 287f 3330 382c 3133 3239 350a 2020  de(.308,13295.  
+000060b0: 2020 626f 6f6c 2063 6865 636b 5f70 6861    bool check_pha
+000060c0: 7365 5f67 6164 6765 745f 6e6f 6465 287f  se_gadget_node(.
+000060d0: 3331 342c 3133 3637 370a 2020 2020 626f  314,13677.    bo
+000060e0: 6f6c 2063 6865 636b 5f69 6e70 7574 5f6e  ol check_input_n
+000060f0: 6f64 6528 7f33 3231 2c31 3430 3437 0a20  ode(.321,14047. 
+00006100: 2020 2062 6f6f 6c20 6368 6563 6b5f 6f75     bool check_ou
+00006110: 7470 7574 5f6e 6f64 6528 7f33 3237 2c31  tput_node(.327,1
+00006120: 3434 3032 0a20 2020 2062 6f6f 6c20 6368  4402.    bool ch
+00006130: 6563 6b5f 636f 6e6e 6563 745f 696e 7075  eck_connect_inpu
+00006140: 745f 6e6f 6465 287f 3333 332c 3134 3736  t_node(.333,1476
+00006150: 390a 2020 2020 626f 6f6c 2063 6865 636b  9.    bool check
+00006160: 5f63 6f6e 6e65 6374 5f6f 7574 7075 745f  _connect_output_
+00006170: 6e6f 6465 287f 3334 352c 3135 3232 320a  node(.345,15222.
+00006180: 2020 2020 626f 6f6c 2063 6865 636b 5f63      bool check_c
+00006190: 6f6e 6e65 6374 5f70 6861 7365 5f67 6164  onnect_phase_gad
+000061a0: 6765 7428 7f33 3537 2c31 3537 3131 0a20  get(.357,15711. 
+000061b0: 2020 2076 6f69 6420 7265 6d6f 7665 5f65     void remove_e
+000061c0: 6467 6573 5f6f 665f 6e6f 6465 287f 3339  dges_of_node(.39
+000061d0: 322c 3137 3035 370a 2020 2020 7569 6e74  2,17057.    uint
+000061e0: 3332 5f74 2064 6567 7265 655f 6f66 5f6e  32_t degree_of_n
+000061f0: 6f64 6528 7f34 3039 2c31 3735 3631 0a20  ode(.409,17561. 
+00006200: 2020 205a 584e 6f64 654b 696e 6420 6b69     ZXNodeKind ki
+00006210: 6e64 5f6f 665f 6e6f 6465 287f 3431 352c  nd_of_node(.415,
+00006220: 3137 3830 350a 2020 2020 7374 643a 3a76  17805.    std::v
+00006230: 6563 746f 723c 7f73 7464 3a3a 7665 6374  ector<.std::vect
+00006240: 6f72 0135 3232 2c32 3234 3039 0a20 2020  or.522,22409.   
+00006250: 205a 5844 6961 6772 616d 287f 3533 332c   ZXDiagram(.533,
+00006260: 3232 3737 390a 2020 2020 5a58 4469 6167  22779.    ZXDiag
+00006270: 7261 6d4b 696e 6420 6b69 6e64 287f 3533  ramKind kind(.53
+00006280: 382c 3233 3032 330a 2020 2020 7569 6e74  8,23023.    uint
+00006290: 3332 5f74 2071 7562 6974 5f6e 756d 287f  32_t qubit_num(.
+000062a0: 3534 302c 3233 3130 350a 2020 2020 7374  540,23105.    st
+000062b0: 643a 3a76 6563 746f 723c 5a58 4e6f 6465  d::vector<ZXNode
+000062c0: 3e20 6e6f 6465 7328 7f35 3432 2c32 3331  > nodes(.542,231
+000062d0: 3838 0a20 2020 2073 7464 3a3a 7665 6374  88.    std::vect
+000062e0: 6f72 3c75 696e 7433 325f 743e 2069 6e70  or<uint32_t> inp
+000062f0: 7574 7328 7f35 3434 2c32 3332 3735 0a20  uts(.544,23275. 
+00006300: 2020 2073 7464 3a3a 7665 6374 6f72 3c75     std::vector<u
+00006310: 696e 7433 325f 743e 206f 7574 7075 7473  int32_t> outputs
+00006320: 287f 3534 362c 3233 3336 370a 2020 2020  (.546,23367.    
+00006330: 7374 643a 3a76 6563 746f 723c 7374 643a  std::vector<std:
+00006340: 3a76 6563 746f 723c 5a58 4564 6765 3e3e  :vector<ZXEdge>>
+00006350: 2061 646a 5f6d 6174 287f 3534 382c 3233   adj_mat(.548,23
+00006360: 3436 310a 2020 2020 766f 6964 206b 696e  461.    void kin
+00006370: 6428 7f35 3530 2c32 3335 3633 0a20 2020  d(.550,23563.   
+00006380: 2076 6f69 6420 7175 6269 745f 6e75 6d28   void qubit_num(
+00006390: 7f35 3532 2c32 3336 3534 0a20 2020 2076  .552,23654.    v
+000063a0: 6f69 6420 6e6f 6465 7328 7f35 3534 2c32  oid nodes(.554,2
+000063b0: 3337 3536 0a20 2020 2076 6f69 6420 696e  3756.    void in
+000063c0: 7075 7473 287f 3535 362c 3233 3835 350a  puts(.556,23855.
+000063d0: 2020 2020 766f 6964 206f 7574 7075 7473      void outputs
+000063e0: 287f 3535 382c 3233 3936 310a 2020 2020  (.558,23961.    
+000063f0: 766f 6964 2061 646a 5f6d 6174 287f 3536  void adj_mat(.56
+00006400: 302c 3234 3037 310a 2020 2020 766f 6964  0,24071.    void
+00006410: 2073 686f 7728 7f35 3730 2c32 3433 3734   show(.570,24374
+00006420: 0a20 2020 2073 7464 3a3a 6d61 703c 7f73  .    std::map<.s
+00006430: 7464 3a3a 6d61 7001 3537 352c 3234 3533  td::map.575,2453
+00006440: 360a 2020 2020 7569 6e74 3332 5f74 2073  6.    uint32_t s
+00006450: 7069 6465 725f 636f 756e 7428 7f35 3839  pider_count(.589
+00006460: 2c32 3439 3336 0a20 2020 2075 696e 7433  ,24936.    uint3
+00006470: 325f 7420 6e6f 6e5f 636c 6966 666f 7264  2_t non_clifford
+00006480: 5f63 6f75 6e74 287f 3539 332c 3235 3038  _count(.593,2508
+00006490: 380a 2020 2020 6672 6965 6e64 2073 7464  8.    friend std
+000064a0: 3a3a 6f73 7472 6561 6d26 206f 7065 7261  ::ostream& opera
+000064b0: 746f 723c 3c28 7f36 3833 2c32 3739 3238  tor<<(.683,27928
+000064c0: 0a0c 0a6f 7074 696d 697a 6572 2e68 2c31  ...optimizer.h,1
+000064d0: 3232 330a 2364 6566 696e 6520 4f50 5449  223.#define OPTI
+000064e0: 4d49 5a45 525f 487f 372c 3932 0a20 2065  MIZER_H.7,92.  e
+000064f0: 6e75 6d20 4f70 7469 6d69 7a65 724b 696e  num OptimizerKin
+00006500: 6420 7f31 392c 3235 310a 0909 2020 2020  d .19,251...    
+00006510: 2020 5a58 4361 6c63 756c 7573 2c7f 3230    ZXCalculus,.20
+00006520: 2c32 3734 0a09 0920 2020 2020 2050 6861  ,274...      Pha
+00006530: 7365 506f 6c79 6e6f 6d69 616c 207f 3231  sePolynomial .21
+00006540: 2c33 3137 0a20 2063 6c61 7373 204f 7074  ,317.  class Opt
+00006550: 696d 697a 6572 7f32 382c 3434 350a 2020  imizer.28,445.  
+00006560: 2020 4f70 7469 6d69 7a65 724b 696e 6420    OptimizerKind 
+00006570: 6b69 6e64 5f3b 7f33 312c 3437 380a 2020  kind_;.31,478.  
+00006580: 2020 646f 7562 6c65 2070 726f 635f 7469    double proc_ti
+00006590: 6d65 5f3b 7f33 322c 3533 360a 2020 2020  me_;.32,536.    
+000065a0: 7374 643a 3a6d 6170 3c7f 7374 643a 3a6d  std::map<.std::m
+000065b0: 6170 0133 332c 3538 300a 2020 2020 7374  ap.33,580.    st
+000065c0: 643a 3a6d 6170 3c73 7464 3a3a 7374 7269  d::map<std::stri
+000065d0: 6e67 2c20 7569 6e74 3332 5f74 3e20 7374  ng, uint32_t> st
+000065e0: 6174 735f 696e 5f3b 7f33 332c 3538 300a  ats_in_;.33,580.
+000065f0: 2020 2020 7374 643a 3a6d 6170 3c7f 7374      std::map<.st
+00006600: 643a 3a6d 6170 0133 342c 3637 330a 2020  d::map.34,673.  
+00006610: 2020 7374 643a 3a6d 6170 3c73 7464 3a3a    std::map<std::
+00006620: 7374 7269 6e67 2c20 7569 6e74 3332 5f74  string, uint32_t
+00006630: 3e20 7374 6174 735f 6f75 745f 3b7f 3334  > stats_out_;.34
+00006640: 2c36 3733 0a20 2020 2073 7464 3a3a 6d61  ,673.    std::ma
+00006650: 703c 7f73 7464 3a3a 6d61 7001 3335 2c37  p<.std::map.35,7
+00006660: 3636 0a20 2020 2073 7464 3a3a 6d61 703c  66.    std::map<
+00006670: 7374 643a 3a73 7472 696e 672c 2075 696e  std::string, uin
+00006680: 7433 325f 743e 207a 785f 7374 6174 735f  t32_t> zx_stats_
+00006690: 696e 5f3b 7f33 352c 3736 360a 2020 2020  in_;.35,766.    
+000066a0: 7374 643a 3a6d 6170 3c7f 7374 643a 3a6d  std::map<.std::m
+000066b0: 6170 0133 362c 3836 370a 2020 2020 7374  ap.36,867.    st
+000066c0: 643a 3a6d 6170 3c73 7464 3a3a 7374 7269  d::map<std::stri
+000066d0: 6e67 2c20 7569 6e74 3332 5f74 3e20 7a78  ng, uint32_t> zx
+000066e0: 5f73 7461 7473 5f6f 7574 5f3b 7f33 362c  _stats_out_;.36,
+000066f0: 3836 370a 2020 2020 4f70 7469 6d69 7a65  867.    Optimize
+00006700: 724b 696e 6420 6b69 6e64 287f 3339 2c31  rKind kind(.39,1
+00006710: 3030 360a 2020 2020 646f 7562 6c65 2070  006.    double p
+00006720: 726f 635f 7469 6d65 287f 3431 2c31 3038  roc_time(.41,108
+00006730: 380a 2020 2020 646f 7562 6c65 2067 6574  8.    double get
+00006740: 5f70 726f 635f 7469 6d65 287f 3433 2c31  _proc_time(.43,1
+00006750: 3137 330a 2020 2020 7374 643a 3a6d 6170  173.    std::map
+00006760: 3c7f 7374 643a 3a6d 6170 0134 352c 3132  <.std::map.45,12
+00006770: 3631 0a20 2020 2073 7464 3a3a 6d61 703c  61.    std::map<
+00006780: 7374 643a 3a73 7472 696e 672c 2075 696e  std::string, uin
+00006790: 7433 325f 743e 2073 7461 7473 5f69 6e28  t32_t> stats_in(
+000067a0: 7f34 352c 3132 3631 0a20 2020 2073 7464  .45,1261.    std
+000067b0: 3a3a 6d61 703c 7f73 7464 3a3a 6d61 7001  ::map<.std::map.
+000067c0: 3437 2c31 3337 330a 2020 2020 7374 643a  47,1373.    std:
+000067d0: 3a6d 6170 3c73 7464 3a3a 7374 7269 6e67  :map<std::string
+000067e0: 2c20 7569 6e74 3332 5f74 3e20 7374 6174  , uint32_t> stat
+000067f0: 735f 6f75 7428 7f34 372c 3133 3733 0a20  s_out(.47,1373. 
+00006800: 2020 2073 7464 3a3a 6d61 703c 7f73 7464     std::map<.std
+00006810: 3a3a 6d61 7001 3439 2c31 3438 390a 2020  ::map.49,1489.  
+00006820: 2020 7374 643a 3a6d 6170 3c73 7464 3a3a    std::map<std::
+00006830: 7374 7269 6e67 2c20 7569 6e74 3332 5f74  string, uint32_t
+00006840: 3e20 7a78 5f73 7461 7473 5f69 6e28 7f34  > zx_stats_in(.4
+00006850: 392c 3134 3839 0a20 2020 2073 7464 3a3a  9,1489.    std::
+00006860: 6d61 703c 7f73 7464 3a3a 6d61 7001 3531  map<.std::map.51
+00006870: 2c31 3631 300a 2020 2020 7374 643a 3a6d  ,1610.    std::m
+00006880: 6170 3c73 7464 3a3a 7374 7269 6e67 2c20  ap<std::string, 
+00006890: 7569 6e74 3332 5f74 3e20 7a78 5f73 7461  uint32_t> zx_sta
+000068a0: 7473 5f6f 7574 287f 3531 2c31 3631 300a  ts_out(.51,1610.
+000068b0: 2020 2020 766f 6964 206b 696e 6428 7f35      void kind(.5
+000068c0: 332c 3137 3235 0a20 2020 2076 6f69 6420  3,1725.    void 
+000068d0: 7072 6f63 5f74 696d 6528 7f35 352c 3138  proc_time(.55,18
+000068e0: 3136 0a20 2020 2076 6f69 6420 7374 6174  16.    void stat
+000068f0: 735f 696e 287f 3537 2c31 3931 390a 2020  s_in(.57,1919.  
+00006900: 2020 766f 6964 2073 7461 7473 5f6f 7574    void stats_out
+00006910: 287f 3539 2c32 3034 350a 2020 2020 766f  (.59,2045.    vo
+00006920: 6964 207a 785f 7374 6174 735f 696e 287f  id zx_stats_in(.
+00006930: 3631 2c32 3137 360a 2020 2020 766f 6964  61,2176.    void
+00006940: 207a 785f 7374 6174 735f 6f75 7428 7f36   zx_stats_out(.6
+00006950: 332c 3233 3137 0a20 2020 2076 6f69 6420  3,2317.    void 
+00006960: 7368 6f77 287f 3737 2c32 3737 340a 2020  show(.77,2774.  
+00006970: 2020 6672 6965 6e64 2073 7464 3a3a 6f73    friend std::os
+00006980: 7472 6561 6d26 206f 7065 7261 746f 723c  tream& operator<
+00006990: 3c28 7f39 372c 3336 3539 0a0c 0a64 6167  <(.97,3659...dag
+000069a0: 6564 6765 2e63 7070 2c34 360a 7374 643a  edge.cpp,46.std:
+000069b0: 3a73 7472 696e 6720 5368 6172 7169 743a  :string Sharqit:
+000069c0: 3a44 4147 4564 6765 3a3a 6e61 6d65 287f  :DAGEdge::name(.
+000069d0: 6e61 6d65 0138 2c39 320a 0c0a 6461 676e  name.8,92...dagn
+000069e0: 6f64 652e 6370 702c 3436 0a73 7464 3a3a  ode.cpp,46.std::
+000069f0: 7374 7269 6e67 2053 6861 7271 6974 3a3a  string Sharqit::
+00006a00: 4441 474e 6f64 653a 3a6e 616d 6528 7f6e  DAGNode::name(.n
+00006a10: 616d 6501 382c 3932 0a0c 0a6f 7074 696d  ame.8,92...optim
+00006a20: 697a 6572 2e63 7070 2c33 3738 0a23 6465  izer.cpp,378.#de
+00006a30: 6669 6e65 2044 4542 5547 7f38 2c31 3032  fine DEBUG.8,102
+00006a40: 0a73 7464 3a3a 7374 7269 6e67 2053 6861  .std::string Sha
+00006a50: 7271 6974 3a3a 4f70 7469 6d69 7a65 723a  rqit::Optimizer:
+00006a60: 3a74 6f5f 7374 7269 6e67 287f 746f 5f73  :to_string(.to_s
+00006a70: 7472 696e 6701 3130 2c31 3137 0a73 7464  tring.10,117.std
+00006a80: 3a3a 7374 7269 6e67 2053 6861 7271 6974  ::string Sharqit
+00006a90: 3a3a 4f70 7469 6d69 7a65 723a 3a6e 616d  ::Optimizer::nam
+00006aa0: 6528 7f6e 616d 6501 3533 2c32 3530 350a  e(.name.53,2505.
+00006ab0: 5368 6172 7169 743a 3a51 4369 7263 2053  Sharqit::QCirc S
+00006ac0: 6861 7271 6974 3a3a 4f70 7469 6d69 7a65  harqit::Optimize
+00006ad0: 723a 3a72 6564 7563 655f 6761 7465 735f  r::reduce_gates_
+00006ae0: 7573 696e 675f 7a78 287f 7265 6475 6365  using_zx(.reduce
+00006af0: 5f67 6174 6573 5f75 7369 6e67 5f7a 7801  _gates_using_zx.
+00006b00: 3634 2c32 3834 300a 5368 6172 7169 743a  64,2840.Sharqit:
+00006b10: 3a51 4369 7263 2053 6861 7271 6974 3a3a  :QCirc Sharqit::
+00006b20: 4f70 7469 6d69 7a65 723a 3a72 6564 7563  Optimizer::reduc
+00006b30: 655f 6761 7465 735f 7573 696e 675f 7070  e_gates_using_pp
+00006b40: 287f 7265 6475 6365 5f67 6174 6573 5f75  (.reduce_gates_u
+00006b50: 7369 6e67 5f70 7001 3933 2c33 3533 360a  sing_pp.93,3536.
+00006b60: 5368 6172 7169 743a 3a51 4369 7263 2053  Sharqit::QCirc S
+00006b70: 6861 7271 6974 3a3a 4f70 7469 6d69 7a65  harqit::Optimize
+00006b80: 723a 3a72 6564 7563 655f 6761 7465 7328  r::reduce_gates(
+00006b90: 7f72 6564 7563 655f 6761 7465 7301 3134  .reduce_gates.14
+00006ba0: 322c 3439 3132 0a0c 0a71 6761 7465 2e68  2,4912...qgate.h
+00006bb0: 2c31 3634 380a 2364 6566 696e 6520 5147  ,1648.#define QG
+00006bc0: 4154 455f 487f 372c 3830 0a20 2065 6e75  ATE_H.7,80.  enu
+00006bd0: 6d20 5147 6174 654b 696e 6420 7f31 392c  m QGateKind .19,
+00006be0: 3234 310a 0909 2020 582c 7f32 302c 3236  241...  X,.20,26
+00006bf0: 300a 0909 2020 5a2c 7f32 312c 3238 350a  0...  Z,.21,285.
+00006c00: 0909 2020 532c 7f32 322c 3331 300a 0909  ..  S,.22,310...
+00006c10: 2020 5364 672c 7f32 332c 3332 390a 0909    Sdg,.23,329...
+00006c20: 2020 542c 7f32 342c 3338 340a 0909 2020    T,.24,384...  
+00006c30: 5464 672c 7f32 352c 3430 330a 0909 2020  Tdg,.25,403...  
+00006c40: 482c 7f32 362c 3435 380a 0909 2020 525a  H,.26,458...  RZ
+00006c50: 2c7f 3237 2c34 3838 0a09 0920 2043 582c  ,.27,488...  CX,
+00006c60: 7f32 382c 3530 390a 0909 2020 435a 2c7f  .28,509...  CZ,.
+00006c70: 3239 2c35 3332 0a09 0920 2043 4358 2c7f  29,532...  CCX,.
+00006c80: 3330 2c35 3533 0a09 0920 2043 435a 2c7f  30,553...  CCZ,.
+00006c90: 3331 2c35 3736 0a09 0920 2049 642c 7f33  31,576...  Id,.3
+00006ca0: 322c 3539 390a 0909 2020 4964 322c 7f33  2,599...  Id2,.3
+00006cb0: 332c 3633 390a 2020 636c 6173 7320 5147  3,639.  class QG
+00006cc0: 6174 657f 3430 2c37 3337 0a20 2020 2051  ate.40,737.    Q
+00006cd0: 4761 7465 4b69 6e64 206b 696e 645f 3b7f  GateKind kind_;.
+00006ce0: 3433 2c37 3636 0a20 2020 2073 7464 3a3a  43,766.    std::
+00006cf0: 7665 6374 6f72 3c75 696e 7433 325f 743e  vector<uint32_t>
+00006d00: 2071 6964 5f3b 7f34 342c 3831 330a 2020   qid_;.44,813.  
+00006d10: 2020 5068 6173 6520 7068 6173 655f 3b7f    Phase phase_;.
+00006d20: 3435 2c38 3734 0a20 2020 2073 7464 3a3a  45,874.    std::
+00006d30: 7665 6374 6f72 3c75 696e 7433 325f 743e  vector<uint32_t>
+00006d40: 2063 6f6e 7472 6f6c 5f70 6174 7465 726e   control_pattern
+00006d50: 5f3b 7f34 362c 3932 300a 2020 2020 7374  _;.46,920.    st
+00006d60: 643a 3a76 6563 746f 723c 7374 643a 3a76  d::vector<std::v
+00006d70: 6563 746f 723c 7374 643a 3a63 6f6d 706c  ector<std::compl
+00006d80: 6578 3c64 6f75 626c 653e 3e3e 206f 705f  ex<double>>> op_
+00006d90: 3b7f 3437 2c31 3030 350a 2020 2020 5147  ;.47,1005.    QG
+00006da0: 6174 6528 7f37 372c 3234 3936 0a20 2020  ate(.77,2496.   
+00006db0: 2051 4761 7465 4b69 6e64 206b 696e 6428   QGateKind kind(
+00006dc0: 7f38 302c 3236 3830 0a20 2020 2073 7464  .80,2680.    std
+00006dd0: 3a3a 7665 6374 6f72 3c75 696e 7433 325f  ::vector<uint32_
+00006de0: 743e 2071 6964 287f 3832 2c32 3735 320a  t> qid(.82,2752.
+00006df0: 2020 2020 5068 6173 6520 7068 6173 6528      Phase phase(
+00006e00: 7f38 342c 3238 3336 0a20 2020 2050 6861  .84,2836.    Pha
+00006e10: 7365 2067 6574 5f70 6861 7365 287f 3836  se get_phase(.86
+00006e20: 2c32 3930 380a 2020 2020 7374 643a 3a76  ,2908.    std::v
+00006e30: 6563 746f 723c 7569 6e74 3332 5f74 3e20  ector<uint32_t> 
+00006e40: 636f 6e74 726f 6c5f 7061 7474 6572 6e28  control_pattern(
+00006e50: 7f38 382c 3239 3934 0a20 2020 2073 7464  .88,2994.    std
+00006e60: 3a3a 7665 6374 6f72 3c73 7464 3a3a 7665  ::vector<std::ve
+00006e70: 6374 6f72 3c73 7464 3a3a 636f 6d70 6c65  ctor<std::comple
+00006e80: 783c 646f 7562 6c65 3e3e 3e20 6f70 287f  x<double>>> op(.
+00006e90: 3930 2c33 3039 390a 2020 2020 766f 6964  90,3099.    void
+00006ea0: 206b 696e 6428 7f39 322c 3332 3035 0a20   kind(.92,3205. 
+00006eb0: 2020 2076 6f69 6420 7169 6428 7f39 342c     void qid(.94,
+00006ec0: 3332 3836 0a20 2020 2076 6f69 6420 7068  3286.    void ph
+00006ed0: 6173 6528 7f39 362c 3333 3738 0a20 2020  ase(.96,3378.   
+00006ee0: 2076 6f69 6420 636f 6e74 726f 6c5f 7061   void control_pa
+00006ef0: 7474 6572 6e28 7f39 382c 3334 3732 0a20  ttern(.98,3472. 
+00006f00: 2020 2076 6f69 6420 6f70 287f 3130 302c     void op(.100,
+00006f10: 3336 3039 0a20 2020 2075 696e 7433 325f  3609.    uint32_
+00006f20: 7420 7175 6269 745f 6e75 6d28 7f31 3137  t qubit_num(.117
+00006f30: 2c34 3233 380a 2020 2020 626f 6f6c 2069  ,4238.    bool i
+00006f40: 735f 4964 5f67 6174 6528 7f31 3232 2c34  s_Id_gate(.122,4
+00006f50: 3433 320a 2020 2020 626f 6f6c 2069 735f  432.    bool is_
+00006f60: 4964 325f 6761 7465 287f 3132 372c 3436  Id2_gate(.127,46
+00006f70: 3330 0a20 2020 2062 6f6f 6c20 6973 5f58  30.    bool is_X
+00006f80: 5f67 6174 6528 7f31 3332 2c34 3830 370a  _gate(.132,4807.
+00006f90: 2020 2020 626f 6f6c 2069 735f 5a5f 6761      bool is_Z_ga
+00006fa0: 7465 287f 3133 372c 3530 3037 0a20 2020  te(.137,5007.   
+00006fb0: 2062 6f6f 6c20 6973 5f48 5f67 6174 6528   bool is_H_gate(
+00006fc0: 7f31 3437 2c35 3239 350a 2020 2020 626f  .147,5295.    bo
+00006fd0: 6f6c 2069 735f 535f 6761 7465 287f 3135  ol is_S_gate(.15
+00006fe0: 322c 3535 3032 0a20 2020 2062 6f6f 6c20  2,5502.    bool 
+00006ff0: 6973 5f53 315f 6761 7465 287f 3136 352c  is_S1_gate(.165,
+00007000: 3538 3939 0a20 2020 2062 6f6f 6c20 6973  5899.    bool is
+00007010: 5f53 335f 6761 7465 287f 3137 362c 3632  _S3_gate(.176,62
+00007020: 3332 0a20 2020 2062 6f6f 6c20 6973 5f54  32.    bool is_T
+00007030: 5f67 6174 6528 7f31 3837 2c36 3538 300a  _gate(.187,6580.
+00007040: 2020 2020 626f 6f6c 2069 735f 5431 5f67      bool is_T1_g
+00007050: 6174 6528 7f32 3030 2c36 3937 370a 2020  ate(.200,6977.  
+00007060: 2020 626f 6f6c 2069 735f 5437 5f67 6174    bool is_T7_gat
+00007070: 6528 7f32 3133 2c37 3332 370a 2020 2020  e(.213,7327.    
+00007080: 626f 6f6c 2069 735f 4358 5f67 6174 6528  bool is_CX_gate(
+00007090: 7f32 3236 2c37 3635 350a 2020 2020 626f  .226,7655.    bo
+000070a0: 6f6c 2069 735f 435a 5f67 6174 6528 7f32  ol is_CZ_gate(.2
+000070b0: 3331 2c37 3832 300a 2020 2020 626f 6f6c  31,7820.    bool
+000070c0: 2069 735f 4343 585f 6761 7465 287f 3233   is_CCX_gate(.23
+000070d0: 362c 3739 3837 0a20 2020 2062 6f6f 6c20  6,7987.    bool 
+000070e0: 6973 5f43 435a 5f67 6174 6528 7f32 3431  is_CCZ_gate(.241
+000070f0: 2c38 3135 360a 2020 2020 626f 6f6c 2069  ,8156.    bool i
+00007100: 735f 525a 5f67 6174 6528 7f32 3436 2c38  s_RZ_gate(.246,8
+00007110: 3332 330a 2020 2020 626f 6f6c 2069 735f  323.    bool is_
+00007120: 7061 756c 695f 6761 7465 287f 3235 332c  pauli_gate(.253,
+00007130: 3836 3639 0a20 2020 2062 6f6f 6c20 6973  8669.    bool is
+00007140: 5f70 726f 7065 725f 636c 6966 666f 7264  _proper_clifford
+00007150: 5f67 6174 6528 7f32 3538 2c38 3838 330a  _gate(.258,8883.
+00007160: 2020 2020 626f 6f6c 2069 735f 636c 6966      bool is_clif
+00007170: 666f 7264 5f67 6174 6528 7f32 3633 2c39  ford_gate(.263,9
+00007180: 3036 300a 2020 2020 626f 6f6c 2069 735f  060.    bool is_
+00007190: 6e6f 6e5f 636c 6966 666f 7264 5f67 6174  non_clifford_gat
+000071a0: 6528 7f32 3638 2c39 3238 390a 2020 2020  e(.268,9289.    
+000071b0: 626f 6f6c 2069 735f 696e 636c 7564 6564  bool is_included
+000071c0: 287f 3237 342c 3935 3134 0a20 2020 2073  (.274,9514.    s
+000071d0: 7461 7469 6320 7374 643a 3a74 7570 6c65  tatic std::tuple
+000071e0: 3c7f 7374 643a 3a74 7570 6c65 0133 3138  <.std::tuple.318
+000071f0: 2c31 3130 3334 0a20 2020 2066 7269 656e  ,11034.    frien
+00007200: 6420 7374 643a 3a6f 7374 7265 616d 2620  d std::ostream& 
+00007210: 6f70 6572 6174 6f72 3c3c 287f 3331 392c  operator<<(.319,
+00007220: 3131 3131 300a 0c0a 6672 6163 7469 6f6e  11110...fraction
+00007230: 2e63 7070 2c35 370a 7374 643a 3a73 7472  .cpp,57.std::str
+00007240: 696e 6720 5368 6172 7169 743a 3a46 7261  ing Sharqit::Fra
+00007250: 6374 696f 6e3a 3a74 6f5f 7374 7269 6e67  ction::to_string
+00007260: 287f 746f 5f73 7472 696e 6701 382c 3939  (.to_string.8,99
+00007270: 0a                                       .
```

### Comparing `sharqit-0.2.2/sharqit/cpp/binary_matrix.cpp` & `sharqit-0.2.3/sharqit/cpp/binary_matrix.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/binary_matrix.h` & `sharqit-0.2.3/sharqit/cpp/binary_matrix.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/dag.h` & `sharqit-0.2.3/sharqit/cpp/dag.h`

 * *Files 0% similar despite different names*

```diff
@@ -383,14 +383,15 @@
      * @brief cannlel the two-qubit gates
      * @return total gate-count after the cancellation
      * @sa Yunseong Nam, Neil J. Ross, Yuan Su, Andrew M. Childs, Dmitri Maslov, "Automated optimization of large quantum circuits with continuous parameters", [arXiv:1710.07345](https://arxiv.org/abs/1710.07345)
      */
     uint32_t two_qubit_gate_cancellation();
     /**
      * @brief execute the rule-based gate reduction
+     * @param [in] full full reduction or not
      * @sa Yunseong Nam, Neil J. Ross, Yuan Su, Andrew M. Childs, Dmitri Maslov, "Automated optimization of large quantum circuits with continuous parameters", [arXiv:1710.07345](https://arxiv.org/abs/1710.07345)
      */
     void rule_based_gate_reduction();
     friend std::ostream& operator<<(std::ostream& ost, const DAGCirc& dc) { ost << dc.to_string(); return ost; }
   };
 }
```

### Comparing `sharqit-0.2.2/sharqit/cpp/dagcirc.cpp` & `sharqit-0.2.3/sharqit/cpp/dagcirc.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -533,15 +533,14 @@
 uint32_t Sharqit::DAGCirc::hadamard_gate_reduction()
 {
   cx_to_cz_gate();
   cz_to_cx_gate();
   hadamard_gate_reduction_1();
   hadamard_gate_reduction_2();
   hadamard_gate_reduction_3();
-
   return gate_count();
 }
 
 uint32_t Sharqit::DAGCirc::single_qubit_gate_cancellation()
 {
   for (uint32_t q = 0; q < qubit_num_; ++q) {
 
@@ -593,48 +592,48 @@
      q[0] ---------*---------*--
      q[1] --RZ(1)--X--RZ(2)--X--
      is equal to
      q[0] --*---------*---------
      q[1] --X--RZ(2)--X--RZ(1)--
    */
   for (uint32_t q = 0; q < qubit_num_; ++q) {
-
+  
     for (uint32_t ori = next_node(inputs_[q], q); !nodes_[ori].is_outnode(); ori = next_node(ori, q)) {
-
+  
       if (nodes_[ori].is_outnode()) break;
       if (nodes_[ori].is_identity()) continue;
-
+  
       if (nodes_[ori].is_rotation()) {
-
-	uint32_t tar = q;
-
-	for (uint32_t now_tar = next_node(ori, tar); !nodes_[now_tar].is_outnode(); now_tar = next_node(now_tar, tar)) {
-	  if (nodes_[ori].commutable(nodes_[now_tar])) {
-	    continue;
-	  }
-	  else if (nodes_[now_tar].is_cnot() && nodes_[now_tar].qgate().qid()[1] == tar) {
-	    uint32_t con = nodes_[now_tar].qgate().qid()[0];
-	    uint32_t now_con = now_tar;
-	    now_tar = next_node(now_tar, tar);
-	    if (!nodes_[now_tar].is_outnode() && nodes_[now_tar].is_rotation()) {
-	      now_tar = next_node(now_tar, tar);
-	      now_con = next_node(now_con, con);
-	      if (now_tar == now_con && nodes_[now_tar].is_cnot() && nodes_[now_tar].qgate().qid()[1] == tar) {
-		uint32_t next_tar = next_node(now_tar, tar);
-		DAGNode ins_node = nodes_[ori];
-		uint32_t ins = append_node(ins_node);
-		remove_edge(now_tar, next_tar, tar);
-		connect_nodes(now_tar, ins, tar);
-		connect_nodes(ins, next_tar, tar);
-		nodes_[ori].qgate(Sharqit::QGate(Sharqit::QGateKind::Id, {tar}));
-	      }
-	    }
-	  }
-	  break;
-	}
+  
+  	uint32_t tar = q;
+  
+  	for (uint32_t now_tar = next_node(ori, tar); !nodes_[now_tar].is_outnode(); now_tar = next_node(now_tar, tar)) {
+  	  if (nodes_[ori].commutable(nodes_[now_tar])) {
+  	    continue;
+  	  }
+  	  else if (nodes_[now_tar].is_cnot() && nodes_[now_tar].qgate().qid()[1] == tar) {
+  	    uint32_t con = nodes_[now_tar].qgate().qid()[0];
+  	    uint32_t now_con = now_tar;
+  	    now_tar = next_node(now_tar, tar);
+  	    if (!nodes_[now_tar].is_outnode() && nodes_[now_tar].is_rotation()) {
+  	      now_tar = next_node(now_tar, tar);
+  	      now_con = next_node(now_con, con);
+  	      if (now_tar == now_con && nodes_[now_tar].is_cnot() && nodes_[now_tar].qgate().qid()[1] == tar) {
+  		uint32_t next_tar = next_node(now_tar, tar);
+  		DAGNode ins_node = nodes_[ori];
+  		uint32_t ins = append_node(ins_node);
+  		remove_edge(now_tar, next_tar, tar);
+  		connect_nodes(now_tar, ins, tar);
+  		connect_nodes(ins, next_tar, tar);
+  		nodes_[ori].qgate(Sharqit::QGate(Sharqit::QGateKind::Id, {tar}));
+  	      }
+  	    }
+  	  }
+  	  break;
+  	}
       }
     }
   }
   id_removal();
 
   return gate_count();
 }
```

### Comparing `sharqit-0.2.2/sharqit/cpp/extract_qcirc.cpp` & `sharqit-0.2.3/sharqit/cpp/extract_qcirc.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/fraction.h` & `sharqit-0.2.3/sharqit/cpp/fraction.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/linear_map.cpp` & `sharqit-0.2.3/sharqit/cpp/linear_map.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/linear_map.h` & `sharqit-0.2.3/sharqit/cpp/linear_map.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/merge_rotation.cpp` & `sharqit-0.2.3/sharqit/cpp/merge_rotation.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -65,16 +65,22 @@
   for (uint32_t i = 0; i < P.size() - 1; ++i) {
     if (rotation_index_used[i] == 1) continue;
     uint32_t q_i = rotation_index[i];
     for (uint32_t j = i + 1; j < P.size(); ++j) {
       if (std::equal(P[i].cbegin(), P[i].cend(), P[j].cbegin())) {
 	uint32_t q_j = rotation_index[j];
 	Sharqit::Phase phase = qgates_[q_i].phase() + qgates_[q_j].phase();
-	Sharqit::Phase zero(0);
+	phase.mod_2pi();
 	qgates_[q_i].phase(phase);
+	std::complex I(0.0, 1.0);
+	std::vector<std::vector<std::complex<double>>> op = {{std::exp(-I*phase.value()/2.0), 0.0},
+							     {0.0, std::exp(I*phase.value()/2.0)}};
+	qgates_[q_i].op(op);
+
+	Sharqit::Phase zero(0);
 	qgates_[q_j].phase(zero);
 	rotation_index_used[j] = 1;
       }
     }
   }
 }
 
@@ -93,15 +99,14 @@
   uint32_t tar = 0;
 
   std::queue<uint32_t> cnot_anchor;
   std::vector<uint8_t> cnot_visits(qgate_num(), 0);
   std::vector<uint32_t> ppc_qid; // qid of the phase polynomial circuit
   std::vector<std::pair<uint32_t, uint32_t>> term_border(qubit_num());
 
-  //while (end < qgate_num() - 1) {
   while (true) {
 
     start = 100000000;
     //start = std::numeric_limits<uint32_t>::max();
     end = 0;
     ppc_qid.clear();
     for (auto it = term_border.begin(); it != term_border.end(); ++it) {
```

### Comparing `sharqit-0.2.2/sharqit/cpp/nb_sharqit.cpp` & `sharqit-0.2.3/sharqit/cpp/nb_sharqit.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -8,149 +8,248 @@
 #include <nanobind/stl/string.h>
 #include <nanobind/stl/vector.h>
 #include <nanobind/stl/tuple.h>
 #include <nanobind/stl/map.h>
 #include <nanobind/stl/pair.h>
 #include <nanobind/stl/set.h>
 #include <nanobind/stl/list.h>
+#include <nanobind/stl/optional.h>
+#include <nanobind/stl/bind_vector.h>
 
 namespace nb = nanobind;
 
 #include "sharqit.h"
 
 NB_MODULE(sharqit_base, m) {
   nb::class_<Sharqit::Phase>(m, "Phase")
     .def(nb::init<const int32_t>())
     .def(nb::init<const int32_t, const int32_t>())
     .def(nb::init<const std::string&>())
-    .def("to_string", &Sharqit::Phase::to_string, nb::arg("pi_str") = false, "get a string of the Phase.")
+    .def("to_string", &Sharqit::Phase::to_string, nb::arg("pi_str") = false,
+	 "get a string of the Phase.")
     .def("__str__", &Sharqit::Phase::to_string, nb::arg("pi_str") = false)
     .def(nb::self + nb::self)
     .def(nb::self - nb::self)
     .def(nb::self += nb::self)
     .def(nb::self -= nb::self)
     .def(nb::self *= int32_t())
     .def(nb::self /= int32_t())
     .def(int() * nb::self)
     .def(nb::self * int())
     .def(nb::self / int())
     .doc() = "Phase of rotation gate"
     ;
   nb::enum_<Sharqit::QGateKind>(m, "QGateKind")
-    .value("X", Sharqit::QGateKind::X, "Pauli-X gate")
-    .value("Z", Sharqit::QGateKind::Z, "Pauli-X gate")
-    .value("S", Sharqit::QGateKind::S, "S gate")
-    .value("Sdg", Sharqit::QGateKind::Sdg, "Hermitian conjugate of S gate")
-    .value("T", Sharqit::QGateKind::T, "T gate")
-    .value("Tdg", Sharqit::QGateKind::Tdg, "Hermitian conjugate of T gate")
-    .value("H", Sharqit::QGateKind::H, "Hadamard gate")
-    .value("RZ", Sharqit::QGateKind::RZ, "RZ gate")
-    .value("CX", Sharqit::QGateKind::CX, "CNOT gate")
-    .value("CZ", Sharqit::QGateKind::CZ, "controlled RZ gate")
-    .value("Id", Sharqit::QGateKind::Id, "single qubit identity gate")
-    .value("Id2", Sharqit::QGateKind::Id2, "two qubit identity gate")
+    .value("X", Sharqit::QGateKind::X,
+	   "Pauli-X gate")
+    .value("Z", Sharqit::QGateKind::Z,
+	   "Pauli-X gate")
+    .value("S", Sharqit::QGateKind::S,
+	   "S gate")
+    .value("Sdg", Sharqit::QGateKind::Sdg,
+	   "Hermitian conjugate of S gate")
+    .value("T", Sharqit::QGateKind::T,
+	   "T gate")
+    .value("Tdg", Sharqit::QGateKind::Tdg,
+	   "Hermitian conjugate of T gate")
+    .value("H", Sharqit::QGateKind::H,
+	   "Hadamard gate")
+    .value("RZ", Sharqit::QGateKind::RZ,
+	   "RZ gate")
+    .value("CX", Sharqit::QGateKind::CX,
+	   "CNOT gate")
+    .value("CZ", Sharqit::QGateKind::CZ,
+	   "controlled RZ gate")
+    .value("Id", Sharqit::QGateKind::Id,
+	   "single qubit identity gate")
+    .value("Id2", Sharqit::QGateKind::Id2,
+	   "two qubit identity gate")
     .export_values();
   nb::class_<Sharqit::QGate>(m, "QGate")
-    .def(nb::init<const Sharqit::QGateKind, const std::vector<uint32_t>&>())
-    .def(nb::init<const Sharqit::QGateKind, const std::vector<uint32_t>&, const Sharqit::Phase&>())
-    .def(nb::init<const std::string&>())
-    .def("to_string", &Sharqit::QGate::to_string, nb::arg("pi_str") = false, "get a string of the QGate.")
+    .def(nb::init<const Sharqit::QGateKind, const std::vector<uint32_t>&, const Sharqit::Phase&,
+	 const std::vector<uint32_t>>(), nb::arg("kind") = Sharqit::QGateKind::Id,
+	 nb::arg("qid") = std::vector<uint32_t>(1, 0),
+	 nb::arg("phase") = Sharqit::Phase(0),
+	 nb::arg("pol") = std::vector<uint32_t>(0))
+    .def(nb::init<const std::string&>(), nb::arg("qgate_str"))
+    .def("to_string", &Sharqit::QGate::to_string, nb::arg("pi_str") = false,
+	 "get a string of the QGate.")
     .def("__str__", &Sharqit::QGate::to_string, nb::arg("pi_str") = false)
-    .def("name", &Sharqit::QGate::name, nb::arg("pi_str") = false, "get a string of the QGate name.")
+    .def("name", &Sharqit::QGate::name, nb::arg("pi_str") = false,
+	 "get a string of the QGate name.")
     .def_prop_rw("kind",
 		 [](Sharqit::QGate& qgate) { return qgate.kind() ; },
 		 [](Sharqit::QGate& qgate, Sharqit::QGateKind kind) { qgate.kind(kind) ; },
 		 "kind of the QGate.")
     .def_prop_rw("qid",
 		 [](Sharqit::QGate& qgate) { return qgate.qid() ; },
 		 [](Sharqit::QGate& qgate, std::vector<uint32_t>& qid) { qgate.qid(qid) ; },
 		 "qubit indexes of the QGate")
     .def_prop_rw("phase",
 		 [](Sharqit::QGate& qgate) { return qgate.phase() ; },
 		 [](Sharqit::QGate& qgate, Sharqit::Phase& phase) { qgate.phase(phase) ; },
 		 "phase of the rotation gate.")
+    .def_prop_rw("pol",
+		 [](Sharqit::QGate& qgate) { return qgate.pol() ; },
+		 [](Sharqit::QGate& qgate, std::vector<uint32_t>& pol) { qgate.pol(pol) ; },
+		 "polarities of control qubits.")
     .doc() = "Quantum Gate"
      ;
   nb::class_<Sharqit::QCirc>(m, "QCirc")
     .def(nb::init<>())
     .def("to_string", &Sharqit::QCirc::to_string, nb::arg("width") = 100,
 	 "show the quantum circuit diagram as an ascii string.")
     .def("__str__", &Sharqit::QCirc::to_string, nb::arg("width") = 100)
     .def("show", &Sharqit::QCirc::show, nb::arg("width") = 100,
 	 "show the quantum circuit diagram as an ascii string.")
-    .def("print_stats", &Sharqit::QCirc::print_stats, "print stats of the QCirc.")
-    .def("is_equal", &Sharqit::QCirc::is_equal, "is the quantum circuit equal to the other.")
-    .def("save", &Sharqit::QCirc::save, "save the quantum circuit to a file.")
-    .def("load", &Sharqit::QCirc::load, "load the quantum circuit from a file.")
-    .def("id", &Sharqit::QCirc::id, "add an identity gate to the quantum circuit.")
-    .def("x", &Sharqit::QCirc::x, "add a pauli-X gate to the quantum circuit.")
-    .def("z", &Sharqit::QCirc::z, "add a pauli-Z gate to the quantum circuit")
-    .def("s", &Sharqit::QCirc::s, "add a S gate to the quantum circuit.")
-    .def("sdg", &Sharqit::QCirc::sdg, "add a S+ (Hermitian conjugate of the S gate) gate to the quantum circuit.")
-    .def("t", &Sharqit::QCirc::t, "add a T gate to the quantum circuit.")
-    .def("tdg", &Sharqit::QCirc::tdg, "add a T+ (Hermitian conjugate of the T gate) gate to the quantum circuit.")
-    .def("h", &Sharqit::QCirc::h, "add an H (hadamard) gate to the quantum circuit.")
-    .def("rz", &Sharqit::QCirc::rz, "add a RZ gate to the quantum circuit.")
-    .def("id2", &Sharqit::QCirc::id2, "add a two-qubit identity gate.")
-    .def("cx", &Sharqit::QCirc::cx, "add a CX (CNOT) gate to the quantum circuit.")
-    .def("cz", &Sharqit::QCirc::cz, "add a CZ gate to the quantum circuit.")
-    .def("rx", &Sharqit::QCirc::rx, "add a CX (CNOT) gate to the quantum circuit.")
-    .def("y", &Sharqit::QCirc::y, "add a pauli-Y gate to the quamtum circuit.")
-    .def("sx", &Sharqit::QCirc::sx, "add a sqrt-X (squre root of pauli-X) gate to the quantum circuit.")
-    .def("sxdg", &Sharqit::QCirc::sxdg, "add a sqrt-X+ (squre root of pauli-X) gate to the quantum circuit.")
-    .def("ry", &Sharqit::QCirc::ry, "add a RY gate to the quantum circuit.")
-    .def("p", &Sharqit::QCirc::p, "add a P (phase shift) gate to the quantum circuit.")
-    .def("cy", &Sharqit::QCirc::cy, "add a CY (controlled-Y) gate to the quantum circuit.")
-    .def("csx", &Sharqit::QCirc::csx, "add a controlled-sqrt-X gate to the quantum circuit.")
-    .def("csxdg", &Sharqit::QCirc::csxdg, "add a hermitian conjugate of controlled-sqrt-X gate to the quantum circuit.")
-    .def("ch", &Sharqit::QCirc::ch, "add a CH (controlled-hadamard) gate to the quantum circuit.")
-    .def("cs", &Sharqit::QCirc::cs, "add a CS (controlled-S) gate to the quantum circuit.")
-    .def("csdg", &Sharqit::QCirc::csdg, "add a CS+ (hermitian conjugate of controlled-S) gate to the quantum circuit.")
-    .def("ct", &Sharqit::QCirc::ct, "add a CT (controlled-T) gate to the quantum circuit.")
-    .def("ctdg", &Sharqit::QCirc::ctdg, "add a CT+ (hermitian conjugate of controlled-T) gate to the quantum circuit.")
-    .def("crx", &Sharqit::QCirc::crx, "add a controlled-RX gate to the quantum circuit.")
-    .def("cry", &Sharqit::QCirc::cry, "add a controlled-RY gate to the quantum circuit.")
-    .def("crz", &Sharqit::QCirc::crz, "add a controlled-RZ gate to the quantum circuit.")
-    .def("cp", &Sharqit::QCirc::cp, "add a controlled-P gate to the quantum circuit.")
-    .def("rxx", &Sharqit::QCirc::rxx, "add a ising coupling gate (XX-interaction) to the quantum circuit.")
-    .def("ryy", &Sharqit::QCirc::ryy, "add a ising coupling gate (YY-interaction) to the quantum circuit.")
-    .def("rzz", &Sharqit::QCirc::rzz, "add a ising coupling gate (ZZ-interaction) to the quantum circuit.")
-    .def("sw", &Sharqit::QCirc::sw, "add a swap gate to the quantum circuit.")
-    .def("csw", &Sharqit::QCirc::csw, "add a controlled swap (fredkin) gate to the quantum circuit.")
-    .def("ccx", &Sharqit::QCirc::ccx, "add a controlled cnot (toffoli) gate to the quantum circuit.")
-    .def("ccz", &Sharqit::QCirc::ccz, "add a controlled CZ gate to the quantum circuit.")
-    .def("x_count", &Sharqit::QCirc::x_count, "get a number of pauli-X gates in the quantum circuit.")
-    .def("z_count", &Sharqit::QCirc::z_count, "get a number of pauli-Z gates in the quantum circuit.")
-    .def("h_count", &Sharqit::QCirc::h_count, "get a number of H gates in the quantum circuit.")
-    .def("s_count", &Sharqit::QCirc::s_count, "get a number of S and S+ gates in the quantum circuit.")
-    .def("t_count", &Sharqit::QCirc::t_count, "get a number of T and T+ gates in the quantum circuit.")
-    .def("rz_count", &Sharqit::QCirc::rz_count, "get a number of RZ gates in the quantum circuit.")
-    .def("cx_count", &Sharqit::QCirc::cx_count, "get a number of CX (CNOT) gates in the quantum circuit.")
-    .def("cz_count", &Sharqit::QCirc::cz_count, "get a number of CZ gates in the quantum circuit.")
-    .def("twoq_count", &Sharqit::QCirc::twoq_count, "get a number of two-qubit gates in the quantum circuit.")
-    .def("ccx_count", &Sharqit::QCirc::ccx_count, "get a number of CCX gates in the quantum circuit.")
-    .def("ccz_count", &Sharqit::QCirc::ccz_count, "get a number of CCZ gates in the quantum circuit.")
-    .def("tof_count", &Sharqit::QCirc::tof_count, "get a number of Toffoli gates (CCX and CCZ gates) in the quantum circuit.")
-    .def("gate_count", &Sharqit::QCirc::gate_count, "get a number of the quantum gates except to identity gates.")
-    .def("depth", &Sharqit::QCirc::depth, "get a depth of the quantum circuit.")
-    .def("qubit_num", [](Sharqit::QCirc& qc) { return qc.qubit_num(); }, "get a number of the qubits.")
-    .def("add_random", &Sharqit::QCirc::add_random_str, "add a random quantum circuit to the quantum circuit.")
-    .def("add_qgate", nb::overload_cast<const std::string&>(&Sharqit::QCirc::add_qgate), "add a quantum gate to the quantum circuit.")
-    .def("add_qgate", nb::overload_cast<const Sharqit::QGate&>(&Sharqit::QCirc::add_qgate), "add a quantum gate to the quantum circuit.")
+    .def("print_qcirc", &Sharqit::QCirc::print_qcirc,
+	 "print the QCirc.")
+    .def("print_stats", &Sharqit::QCirc::print_stats,
+	 "print stats of the QCirc.")
+    .def("is_equal", [](Sharqit::QCirc& qc, Sharqit::QCirc& other) { return qc.is_equal(other); },
+      "is the quantum circuit equal to the other.")
+    .def("save", &Sharqit::QCirc::save, nb::arg("file_name"),
+	 "save the quantum circuit to a file.")
+    .def("load", &Sharqit::QCirc::load, nb::arg("file_name"),
+	 "load the quantum circuit from a file.")
+    .def("id", &Sharqit::QCirc::id, nb::arg("q"),
+	 "add an identity gate to the quantum circuit.")
+    .def("x", &Sharqit::QCirc::x, nb::arg("q"),
+	 "add a pauli-X gate to the quantum circuit.")
+    .def("z", &Sharqit::QCirc::z, nb::arg("q"),
+	 "add a pauli-Z gate to the quantum circuit")
+    .def("s", &Sharqit::QCirc::s, nb::arg("q"),
+	 "add a S gate to the quantum circuit.")
+    .def("sdg", &Sharqit::QCirc::sdg, nb::arg("q"),
+	 "add a S+ (Hermitian conjugate of the S gate) gate to the quantum circuit.")
+    .def("t", &Sharqit::QCirc::t, nb::arg("q"),
+	 "add a T gate to the quantum circuit.")
+    .def("tdg", &Sharqit::QCirc::tdg, nb::arg("q"),
+	 "add a T+ (Hermitian conjugate of the T gate) gate to the quantum circuit.")
+    .def("h", &Sharqit::QCirc::h, nb::arg("q"),
+	 "add an H (hadamard) gate to the quantum circuit.")
+    .def("rz", &Sharqit::QCirc::rz, nb::arg("q"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a RZ gate to the quantum circuit.")
+    .def("id2", &Sharqit::QCirc::id2, nb::arg("q0"), nb::arg("q1"),
+	 "add a two-qubit identity gate.")
+    .def("cx", &Sharqit::QCirc::cx, nb::arg("con"), nb::arg("tar"), nb::arg("pol") = std::vector<uint32_t>(1,0),
+	 "add a CX (CNOT) gate to the quantum circuit.")
+    .def("cz", &Sharqit::QCirc::cz, nb::arg("con"), nb::arg("tar"), nb::arg("pol") = std::vector<uint32_t>(1,0),
+	 "add a CZ gate to the quantum circuit.")
+    .def("rx", &Sharqit::QCirc::rx, nb::arg("q"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a CX (CNOT) gate to the quantum circuit.")
+    .def("y", &Sharqit::QCirc::y, nb::arg("q"),
+	 "add a pauli-Y gate to the quamtum circuit.")
+    .def("sx", &Sharqit::QCirc::sx, nb::arg("q"),
+	 "add a sqrt-X (squre root of pauli-X) gate to the quantum circuit.")
+    .def("sxdg", &Sharqit::QCirc::sxdg, nb::arg("q"),
+	 "add a sqrt-X+ (squre root of pauli-X) gate to the quantum circuit.")
+    .def("ry", &Sharqit::QCirc::ry, nb::arg("q"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a RY gate to the quantum circuit.")
+    .def("p", &Sharqit::QCirc::p, nb::arg("q"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a P (phase shift) gate to the quantum circuit.")
+    .def("cy", &Sharqit::QCirc::cy, nb::arg("con"), nb::arg("tar"),
+	 "add a CY (controlled-Y) gate to the quantum circuit.")
+    .def("csx", &Sharqit::QCirc::csx, nb::arg("con"), nb::arg("tar"),
+	 "add a controlled-sqrt-X gate to the quantum circuit.")
+    .def("csxdg", &Sharqit::QCirc::csxdg, nb::arg("con"), nb::arg("tar"),
+	 "add a hermitian conjugate of controlled-sqrt-X gate to the quantum circuit.")
+    .def("ch", &Sharqit::QCirc::ch, nb::arg("con"), nb::arg("tar"),
+	 "add a CH (controlled-hadamard) gate to the quantum circuit.")
+    .def("cs", &Sharqit::QCirc::cs, nb::arg("con"), nb::arg("tar"),
+	 "add a CS (controlled-S) gate to the quantum circuit.")
+    .def("csdg", &Sharqit::QCirc::csdg, nb::arg("con"), nb::arg("tar"),
+	 "add a CS+ (hermitian conjugate of controlled-S) gate to the quantum circuit.")
+    .def("ct", &Sharqit::QCirc::ct, nb::arg("con"), nb::arg("tar"),
+	 "add a CT (controlled-T) gate to the quantum circuit.")
+    .def("ctdg", &Sharqit::QCirc::ctdg, nb::arg("con"), nb::arg("tar"),
+	 "add a CT+ (hermitian conjugate of controlled-T) gate to the quantum circuit.")
+    .def("crx", &Sharqit::QCirc::crx, nb::arg("con"), nb::arg("tar"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a controlled-RX gate to the quantum circuit.")
+    .def("cry", &Sharqit::QCirc::cry, nb::arg("con"), nb::arg("tar"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a controlled-RY gate to the quantum circuit.")
+    .def("crz", &Sharqit::QCirc::crz, nb::arg("con"), nb::arg("tar"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a controlled-RZ gate to the quantum circuit.")
+    .def("cp", &Sharqit::QCirc::cp, nb::arg("con"), nb::arg("tar"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a controlled-P gate to the quantum circuit.")
+    .def("rxx", &Sharqit::QCirc::rxx, nb::arg("q0"), nb::arg("q1"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a ising coupling gate (XX-interaction) to the quantum circuit.")
+    .def("ryy", &Sharqit::QCirc::ryy, nb::arg("q0"), nb::arg("q1"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a ising coupling gate (YY-interaction) to the quantum circuit.")
+    .def("rzz", &Sharqit::QCirc::rzz, nb::arg("q0"), nb::arg("q1"), nb::arg("phase") = Sharqit::Phase(0),
+	 "add a ising coupling gate (ZZ-interaction) to the quantum circuit.")
+    .def("sw", &Sharqit::QCirc::sw, nb::arg("q0"), nb::arg("q1"),
+	 "add a swap gate to the quantum circuit.")
+    .def("csw", &Sharqit::QCirc::csw, nb::arg("con"), nb::arg("q0"), nb::arg("q1"),
+	 "add a controlled swap (fredkin) gate to the quantum circuit.")
+    .def("ccx", &Sharqit::QCirc::ccx, nb::arg("c0"), nb::arg("c1"), nb::arg("tar"),
+	 nb::arg("pol") = std::vector<uint32_t>(2, 0),
+	 "add a controlled cnot (toffoli) gate to the quantum circuit.")
+    .def("ccz", &Sharqit::QCirc::ccz, nb::arg("c0"), nb::arg("c1"), nb::arg("tar"),
+	 nb::arg("pol") = std::vector<uint32_t>(2, 0),
+	 "add a controlled CZ gate to the quantum circuit.")
+    .def("x_count", &Sharqit::QCirc::x_count,
+	 "get a number of pauli-X gates in the quantum circuit.")
+    .def("z_count", &Sharqit::QCirc::z_count,
+	 "get a number of pauli-Z gates in the quantum circuit.")
+    .def("h_count", &Sharqit::QCirc::h_count,
+	 "get a number of H gates in the quantum circuit.")
+    .def("s_count", &Sharqit::QCirc::s_count,
+	 "get a number of S and S+ gates in the quantum circuit.")
+    .def("t_count", &Sharqit::QCirc::t_count,
+	 "get a number of T and T+ gates in the quantum circuit.")
+    .def("rz_count", &Sharqit::QCirc::rz_count,
+	 "get a number of RZ gates in the quantum circuit.")
+    .def("cx_count", &Sharqit::QCirc::cx_count,
+	 "get a number of CX (CNOT) gates in the quantum circuit.")
+    .def("cz_count", &Sharqit::QCirc::cz_count,
+	 "get a number of CZ gates in the quantum circuit.")
+    .def("twoq_count", &Sharqit::QCirc::twoq_count,
+	 "get a number of two-qubit gates in the quantum circuit.")
+    .def("ccx_count", &Sharqit::QCirc::ccx_count,
+	 "get a number of CCX gates in the quantum circuit.")
+    .def("ccz_count", &Sharqit::QCirc::ccz_count,
+	 "get a number of CCZ gates in the quantum circuit.")
+    .def("tof_count", &Sharqit::QCirc::tof_count,
+	 "get a number of Toffoli gates (CCX and CCZ gates) in the quantum circuit.")
+    .def("gate_count", &Sharqit::QCirc::gate_count,
+	 "get a number of the quantum gates except to identity gates.")
+    .def("depth", &Sharqit::QCirc::depth,
+	 "get a depth of the quantum circuit.")
+    .def("qubit_num", [](Sharqit::QCirc& qc) { return qc.qubit_num(); },
+	 "get a number of the qubits.")
+    .def("add_random", &Sharqit::QCirc::add_random_str, nb::arg("qubit_num"), nb::arg("qgate_num"), nb::arg("probs"),
+	 "add a random quantum circuit to the quantum circuit.")
+    .def("add_qgate", nb::overload_cast<const std::string&>(&Sharqit::QCirc::add_qgate), nb::arg("qgate_str"),
+	 "add a quantum gate to the quantum circuit.")
+    .def("add_qgate", nb::overload_cast<const Sharqit::QGate&>(&Sharqit::QCirc::add_qgate), nb::arg("qgate"),
+	 "add a quantum gate to the quantum circuit.")
     .def("add_qgate", nb::overload_cast<const Sharqit::QGateKind, const std::vector<uint32_t>&,
-	 const Sharqit::Phase&>(&Sharqit::QCirc::add_qgate), "add a quantum gate to the quantum circuit.")
-    .def("add_qcirc", &Sharqit::QCirc::add_qcirc, "add a quantum circuit to the quantum circuit.")
-    .def("get_qgate", &Sharqit::QCirc::get_qgate, "get a quantum gate.")
-    .def("get_qgates", &Sharqit::QCirc::get_qgates, "get a list of quantum gates.")
-    .def("decomp_tof", &Sharqit::QCirc::decomp_tof, "decompose Toffoli gates.")
+	 const Sharqit::Phase&, const std::vector<uint32_t>&>(&Sharqit::QCirc::add_qgate),
+	 nb::arg("kind"), nb::arg("qid"), nb::arg("phase") = Sharqit::Phase(0),
+	 nb::arg("pol") = std::vector<uint32_t>(0), 
+	 "add a quantum gate to the quantum circuit.")
+    .def("add_qcirc", &Sharqit::QCirc::add_qcirc, nb::arg("qc"),
+	 "add a quantum circuit to the quantum circuit.")
+    .def("get_qgate", &Sharqit::QCirc::get_qgate, nb::arg("i"),
+	 "get a quantum gate.")
+    .def("get_qgates", &Sharqit::QCirc::get_qgates,
+	 "get a list of quantum gates.")
+    .def("inverse", &Sharqit::QCirc::inverse,
+	 "inverse gates.")
+    .def("decomp_tof", &Sharqit::QCirc::decomp_tof,
+	 "decompose Toffoli gates.")
     .def(nb::self + nb::self)
     .def(nb::self += nb::self)
     .doc() = "Quantum Circuit"
     ;
   nb::class_<Sharqit::Optimizer>(m, "Optimizer")
     .def(nb::init<>())
-    .def("show", &Sharqit::Optimizer::show, "show the optimizing result.")
-    .def("proc_time", &Sharqit::Optimizer::get_proc_time, "get the processing time (sec).")
-    .def("reduce_gates", &Sharqit::Optimizer::reduce_gates, "reduce the gate count.")
+    .def("show", &Sharqit::Optimizer::show,
+	 "show the optimizing result.")
+    .def("proc_time", &Sharqit::Optimizer::get_proc_time,
+	 "get the processing time (sec).")
+    .def("reduce_gates", &Sharqit::Optimizer::reduce_gates, nb::arg("qc"), nb::arg("method") = "zx",
+	 "reduce the gate count.")
     .doc() = "Quantum Optimizer"
     ;
 }
```

### Comparing `sharqit-0.2.2/sharqit/cpp/optimizer.cpp` & `sharqit-0.2.3/sharqit/cpp/optimizer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 /**
  * @file optimizer.cpp
  * @brief member functions of Optimizer class
  */
 
 #include "optimizer.h"
 
+#define DEBUG
+
 std::string Sharqit::Optimizer::to_string() const
 {
   std::map<std::string, uint32_t> stats_in = stats_in_;
   std::map<std::string, uint32_t> stats_out = stats_out_;
   std::map<std::string, uint32_t> zx_stats_in = zx_stats_in_;
   std::map<std::string, uint32_t> zx_stats_out = zx_stats_out_;
   std::stringstream ss;
@@ -111,14 +113,15 @@
 
 Sharqit::QCirc Sharqit::Optimizer::reduce_gates(const Sharqit::QCirc& qc, const std::string& method)
 {
   auto start = std::chrono::system_clock::now();
 
   /* decompose CCX or CCZ */
   Sharqit::QCirc qc_in = qc;
+  qc_in.decomp_tof(method);
   
   /* kind of optimizer */
   if (method == "zx") {
     kind_ = Sharqit::OptimizerKind::ZXCalculus;
   }
   else if (method == "pp") {
     kind_ = Sharqit::OptimizerKind::PhasePolynomial;
```

### Comparing `sharqit-0.2.2/sharqit/cpp/optimizer.h` & `sharqit-0.2.3/sharqit/cpp/optimizer.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/phase.cpp` & `sharqit-0.2.3/sharqit/cpp/phase.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/phase.h` & `sharqit-0.2.3/sharqit/cpp/phase.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/propagate_pauli_x.cpp` & `sharqit-0.2.3/sharqit/cpp/propagate_pauli_x.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/qcirc.cpp` & `sharqit-0.2.3/sharqit/cpp/qcirc.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -209,16 +209,18 @@
       for (auto& str:str_list) {
 	if (str.size() < max_strlen) {
 	  str.insert(str.size(), max_strlen - str.size(), '-');
 	}
       }
       uint32_t c = qgate.qid()[0];
       uint32_t t = qgate.qid()[1];
+      std::vector<uint32_t> pol = qgate.pol();
       for (uint32_t i = 0; i < qubit_num_; ++i) {
-	if (i == c) str_list[i] += "*--";
+	if (i == c && pol[0] == 0) str_list[i] += "*--";
+	else if (i == c && pol[0] == 1) str_list[i] += "o--";
 	else if (i == t && qgate.kind() == Sharqit::QGateKind::Id2) str_list[i] += "I--";
 	else if (i == t && qgate.kind() == Sharqit::QGateKind::CX) str_list[i] += "X--";
 	else if (i == t && qgate.kind() == Sharqit::QGateKind::CZ) str_list[i] += "*--";
 	else if (c < t && c < i && i < t) str_list[i] += "|--";
 	else if (t < c && t < i && i < c) str_list[i] += "|--";
 	else str_list[i] += "---";
       }
@@ -229,19 +231,22 @@
 	if (str.size() < max_strlen) {
 	  str.insert(str.size(), max_strlen - str.size(), '-');
 	}
       }
       uint32_t c0 = qgate.qid()[0];
       uint32_t c1 = qgate.qid()[1];
       uint32_t t = qgate.qid()[2];
+      std::vector<uint32_t> pol = qgate.pol();
       for (uint32_t i = 0; i < qubit_num_; ++i) {
-	if (i == c0) str_list[i] += "*--";
-	else if (i == c1) str_list[i] += "*--";
+	if (i == c0 && pol[0] == 0) str_list[i] += "*--";
+	else if (i == c0 && pol[0] == 1) str_list[i] += "o--";
+	else if (i == c1 && pol[1] == 0) str_list[i] += "*--";
+	else if (i == c1 && pol[1] == 1) str_list[i] += "o--";
 	else if (i == t && qgate.kind() == Sharqit::QGateKind::CCX) str_list[i] += "X--";
-	else if (i == t && qgate.kind() == Sharqit::QGateKind::CCZ) str_list[i] += "Z--";
+	else if (i == t && qgate.kind() == Sharqit::QGateKind::CCZ) str_list[i] += "*--";
 	else if (i < c0 && i < c1 && i < t) str_list[i] += "---";
 	else if (i > c0 && i > c1 && i > t) str_list[i] += "---";
 	else str_list[i] += "|--";
       }
       max_strlen = str_list[0].size();
     }
   }
@@ -285,17 +290,18 @@
     if (q >= qubit_num_) qubit_num_ = q + 1;
   }
   return *this;
 }
 
 Sharqit::QCirc& Sharqit::QCirc::add_qgate(const Sharqit::QGateKind kind,
 					  const std::vector<uint32_t>& qid,
-					  const Sharqit::Phase& phase)
+					  const Sharqit::Phase& phase,
+					  const std::vector<uint32_t>& pol)
 {
-  Sharqit::QGate qgate(kind, qid, phase);
+  Sharqit::QGate qgate(kind, qid, phase, pol);
   qgates_.push_back(qgate);
 
   for (auto& q:qid) {
     if (q >= qubit_num_) qubit_num_ = q + 1;
   }
   return *this;
 }
@@ -396,17 +402,17 @@
     }
     add_qgate(kind, qid, phase);
   }
   return *this;
 }
 
 Sharqit::QCirc& Sharqit::QCirc::add_random_str(const uint32_t qubit_num, const uint32_t qgate_num,
-					       const std::string probs)
+					       const std::string probs_str)
 {
-  std::vector<std::string> args = Sharqit::split(probs, ',');
+  std::vector<std::string> args = Sharqit::split(probs_str, ',');
   nlohmann::json probs_json;
   for (uint32_t i = 0; i < args.size(); ++i) {
     std::vector<std::string> key_value = Sharqit::split(args[i], ':');
     std::string gate_str = key_value[0];
     std::string prob_str = key_value[1];
     probs_json[gate_str] = atof(prob_str.c_str());
   }
@@ -491,14 +497,15 @@
 
   std::string label = "";
   std::string shape = "";
   std::string width = "";
   std::string height = "";
   std::string color = "";
   std::string fillcolor = "";
+  std::string fillcolor2 = "";
   std::string fontcolor = "";
   
   /* inputs */
   for (uint32_t i = 0; i < qubit_num_; ++i) {
     label = "q_" + std::to_string(i);;
     shape = "box";
     width = "0.5";
@@ -567,24 +574,30 @@
       /* control */
       label = "";
       shape = "circle";
       width = "0.1";
       height = "0.1";
       color = "black";
       fillcolor = "black";
+      fillcolor2 = "white";
       fontcolor = "black";
 
       nodes.push_back("node_" + std::to_string(cnt + offset));
       edges.push_back({lasts[qgate.qid()[0]], "node_"+ std::to_string(cnt + offset)});
       lasts[qgate.qid()[0]] = "node_"+ std::to_string(cnt + offset);
 
       ofs << "  node_" << cnt + offset << " [label = " << "\"" << label << "\"";
       ofs << ", shape = " << shape;
       ofs << ", width = " << width << ", height = " << height << ", color = " << color;
-      ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      if (qgate.pol()[0] == 0)
+	ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else if (qgate.pol()[0] == 1)
+	ofs << ", fillcolor = " << fillcolor2 << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else
+	throw std::runtime_error("control pattern of the control qubit must be 0 or 1.");
       ++cnt;
       
       /* target */
       if (qgate.kind() == Sharqit::QGateKind::CX) {
 	label = "+";
 	shape = "circle";
 	width = "0.2";
@@ -625,34 +638,45 @@
       /* control */
       label = "";
       shape = "circle";
       width = "0.1";
       height = "0.1";
       color = "black";
       fillcolor = "black";
+      fillcolor2 = "white";
       fontcolor = "black";
 
       nodes.push_back("node_" + std::to_string(cnt + offset));
       edges.push_back({lasts[qgate.qid()[0]], "node_"+ std::to_string(cnt + offset)});
       lasts[qgate.qid()[0]] = "node_"+ std::to_string(cnt + offset);
 
       ofs << "  node_" << cnt + offset << " [label = " << "\"" << label << "\"";
       ofs << ", shape = " << shape;
       ofs << ", width = " << width << ", height = " << height << ", color = " << color;
-      ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      if (qgate.pol()[0] == 0)
+	ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else if (qgate.pol()[0] == 1)
+	ofs << ", fillcolor = " << fillcolor2 << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else
+	throw std::runtime_error("control pattern of the control qubit must be 0 or 1.");
       ++cnt;
       
       nodes.push_back("node_" + std::to_string(cnt + offset));
       edges.push_back({lasts[qgate.qid()[1]], "node_"+ std::to_string(cnt + offset)});
       lasts[qgate.qid()[1]] = "node_"+ std::to_string(cnt + offset);
 
       ofs << "  node_" << cnt + offset << " [label = " << "\"" << label << "\"";
       ofs << ", shape = " << shape;
       ofs << ", width = " << width << ", height = " << height << ", color = " << color;
-      ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      if (qgate.pol()[1] == 0)
+	ofs << ", fillcolor = " << fillcolor << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else if (qgate.pol()[1] == 1)
+	ofs << ", fillcolor = " << fillcolor2 << ", fontcolor = " << fontcolor << "];" << std::endl;
+      else
+	throw std::runtime_error("control pattern of the control qubit must be 0 or 1.");
       ++cnt;
 
       /* target */
       if (qgate.kind() == Sharqit::QGateKind::CCX) {
 	label = "+";
 	shape = "circle";
 	width = "0.2";
@@ -848,39 +872,179 @@
     }
   }
 
   std::vector<QGate> qgates_vec(qgates_list.begin(), qgates_list.end());
   qgates_ = qgates_vec;
 }
 
-void Sharqit::QCirc::decomp_tof()
+Sharqit::QCirc& Sharqit::QCirc::ccx_decomp(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+					   const std::vector<uint32_t>& pol, const std::string& method)
+{
+  if (method == "zx") {
+    if (pol[0] == 0 && pol[1] == 0) {
+      h(tar);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); t(con1); t(tar); cx(con0,con1); t(con0); tdg(con1); cx(con0,con1);
+      h(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 0) {
+      x(con0); 
+      h(tar);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); t(con1); t(tar); cx(con0,con1); t(con0); tdg(con1); cx(con0,con1);
+      h(tar);
+      x(con0);
+    }
+    else if (pol[0] == 0 && pol[1] == 1) {
+      x(con1);
+      h(tar);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); t(con1); t(tar); cx(con0,con1); t(con0); tdg(con1); cx(con0,con1);
+      h(tar);
+      x(con1);
+    }
+    else if (pol[0] == 1 && pol[1] == 1) {
+      x(con0); x(con1);
+      h(tar);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); t(con1); t(tar); cx(con0,con1); t(con0); tdg(con1); cx(con0,con1);
+      h(tar);
+      x(con0); x(con1);
+    }
+    else {
+      throw std::runtime_error("element of control pattern must be 0 or 1.");
+    }
+  }
+  else if (method == "pp") {
+    if (pol[0] == 0 && pol[1] == 0) {
+      h(tar);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+      h(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 0) {
+      h(tar);
+      cx(con1,tar); t(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); tdg(con1); tdg(tar);
+      h(tar);
+    }
+    else if (pol[0] == 0 && pol[1] == 1) {
+      h(tar);
+      cx(con0,tar); t(tar); cx(con1,tar); t(tar); cx(con0,tar); tdg(tar);
+      cx(con1,tar); cx(con1,con0); tdg(con0); cx(con1,con0); t(con1); tdg(con0); tdg(tar);
+      h(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 1) {
+      h(tar);
+      cx(con1,tar); t(tar); cx(con0,tar); t(tar); cx(con1,tar); t(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); tdg(con0); tdg(con1); t(tar);
+      h(tar);
+    }
+    else {
+      throw std::runtime_error("element of control pattern must be 0 or 1.");
+    }
+  }
+  else {
+    throw std::runtime_error("method must be zx or pp.");
+  }
+      
+  return *this;
+}
+
+Sharqit::QCirc& Sharqit::QCirc::ccz_decomp(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+					   const std::vector<uint32_t>& pol, const std::string& method)
+{
+  if (method == "zx") {
+    if (pol[0] == 0 && pol[1] == 0) {
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 0) {
+      x(con0);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+      x(con0);
+    }
+    else if (pol[0] == 0 && pol[1] == 1) {
+      x(con1);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+      x(con1);
+    }
+    else if (pol[0] == 1 && pol[1] == 1) {
+      x(con0); x(con1);
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+      x(con0); x(con1);
+    }
+    else {
+      throw std::runtime_error("element of control pattern must be 0 or 1.");
+    }
+  }
+  else if (method == "pp") {
+    if (pol[0] == 0 && pol[1] == 0) {
+      cx(con1,tar); tdg(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); t(con1); t(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 0) {
+      cx(con1,tar); t(tar); cx(con0,tar); t(tar); cx(con1,tar); tdg(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); t(con0); tdg(con1); tdg(tar);
+    }
+    else if (pol[0] == 0 && pol[1] == 1) {
+      cx(con0,tar); t(tar); cx(con1,tar); t(tar); cx(con0,tar); tdg(tar);
+      cx(con1,tar); cx(con1,con0); tdg(con0); cx(con1,con0); t(con1); tdg(con0); tdg(tar);
+    }
+    else if (pol[0] == 1 && pol[1] == 1) {
+      cx(con1,tar); t(tar); cx(con0,tar); t(tar); cx(con1,tar); t(tar);
+      cx(con0,tar); cx(con0,con1); tdg(con1); cx(con0,con1); tdg(con0); tdg(con1); t(tar);
+    }
+    else {
+      throw std::runtime_error("element of control pattern must be 0 or 1.");
+    }
+  }
+  else {
+    throw std::runtime_error("method must be zx or pp.");
+  }
+  
+  return *this;
+}
+
+void Sharqit::QCirc::decomp_tof(const std::string& method)
 {
   if (include_tof()) {
     Sharqit::QCirc qc;
     for (auto& gate:qgates_) {
-      if (gate.is_CCX_gate()) {
-	std::vector<uint32_t> qid = gate.qid();
-	qc.ccx_decomp(qid[0], qid[1], qid[2]);
+      std::vector<uint32_t> qid = gate.qid();
+      if (gate.is_CX_gate()) {
+	qc.cx_decomp(qid[0], qid[1], gate.pol());
+      }
+      else if (gate.is_CZ_gate()) {
+	qc.cz_decomp(qid[0], qid[1], gate.pol());
+      }
+      else if (gate.is_CCX_gate()) {
+	qc.ccx_decomp(qid[0], qid[1], qid[2], gate.pol(), method);
       }
       else if (gate.is_CCZ_gate()) {
-	std::vector<uint32_t> qid = gate.qid();
-	qc.ccz_decomp(qid[0], qid[1], qid[2]);
+	qc.ccz_decomp(qid[0], qid[1], qid[2], gate.pol(), method);
       }
       else {
 	qc.add_qgate(gate);
       }
     }
-    *this = qc;
+    qubit_num(qc.qubit_num());
+    qgates(qc.qgates());
   }
 }
 
 bool Sharqit::QCirc::include_tof() const
 {
   for (auto& gate:qgates_) {
     if (gate.is_CCX_gate() || gate.is_CCZ_gate()) return true;
+    else if (gate.is_CX_gate() && gate.pol()[0] == 1) return true;
+    else if (gate.is_CZ_gate() && gate.pol()[0] == 1) return true;
   }
   return false;
 }
 
 /* remove Ids and RZ(0)s */
 void Sharqit::QCirc::remove_id()
 {
```

### Comparing `sharqit-0.2.2/sharqit/cpp/qcirc.h` & `sharqit-0.2.3/sharqit/cpp/qcirc.h`

 * *Files 6% similar despite different names*

```diff
@@ -197,15 +197,16 @@
     /**
      * @brief add a quantum gate to the quantum circuit
      * @param [in] kind kind of the quantum gate
      * @param [in] qid qubit id od the quantum gate ({q} for single-qubit gate, {control,target} for two-qubit gate)
      * @param [in] phase phase of the rotation gate
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& add_qgate(const QGateKind kind, const std::vector<uint32_t>& qid, const Phase& phase = 0);
+    QCirc& add_qgate(const QGateKind kind, const std::vector<uint32_t>& qid, const Phase& phase = 0,
+		     const std::vector<uint32_t>& pol = {});
     /**
      * @brief add a quantum gate to the quantum circuit
      * @param [in] qgate QGate object
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& add_qgate(const QGate& qgate);
     /**
@@ -230,20 +231,20 @@
      *       usage: @n qc.add_random(5, 100, {{"X", 1},{"H", 1},{"Sdg", 1},{"CX", 3},{"CZ", 2},{"RZ(1/4)", 1}});
      */
     QCirc& add_random(const uint32_t qubit_num, const uint32_t qgate_num, const nlohmann::json& probs);
     /**
      * @brief add a random quantum circuit to the quantum circuit
      * @param [in] qubit_num number of qubits of the quantum circuit
      * @param [in] qgate_num number of quantum gates in the quantum circuit
-     * @param [in] probs probability of each quantum gate
+     * @param [in] probs_str string expression of probability of each quantum gate
      * @return reference of the QCirc after adding the quantum circuit
      * @note example of probs: @n "X:4,T:5,CX:3" @n "H:0.3,S:0.2,RZ(1/4):0.4" @n
      *       usage: @n qc.add_random(5, 100, "H:2,T:3,RZ(1/2):5");
      */
-    QCirc& add_random_str(const uint32_t qubit_num, const uint32_t qgate_num, const std::string probs);
+    QCirc& add_random_str(const uint32_t qubit_num, const uint32_t qgate_num, const std::string probs_str);
     /**
      * @brief get a quantum gate
      * @param [in] i position of quantum gate 
      * @return QGate object
      */
     Sharqit::QGate get_qgate(const uint32_t i) const { return qgates_[i]; }
     /**
@@ -325,17 +326,18 @@
     void propagate_pauli_x();
     /**
      * @brief all CZ gates are converted to CX gates
      */
     void cz_to_cx();
     /**
      * @brief decompose all Toffoli gates (CCX and CCZ gates) to basic gats
+     * @param [in] method optimization method ("zx" or "pp")
      * @return QCirc object after decomposing
      */
-    void decomp_tof();
+    void decomp_tof(const std::string& method = "zx");
     /**
      * @brief whether any Toffoli gates (CCX or CCZ gates) are included or not
      * @return QCirc object after decomposing
      */
     bool include_tof() const;
     /**
      * @brief add an identity gate to the quantum circuit
@@ -393,52 +395,66 @@
     QCirc& rz(const uint32_t q, const Phase& phase) { return add_qgate(QGateKind::RZ, {q}, phase); }
     /**
      * @brief add a two-qubit identity gate to the quantum circuit
      * @param [in] c qubit id (control) to be applied
      * @param [in] t qubit id (target) to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& id2(const uint32_t c, const uint32_t t) { return add_qgate(QGateKind::Id2, {c, t}); }
+    QCirc& id2(const uint32_t q0, const uint32_t q1) { return add_qgate(QGateKind::Id2, {q0, q1}); }
     /**
      * @brief add a CX (CNOT) gate to the quantum circuit
-     * @param [in] c qubit id (control) to be applied
-     * @param [in] t qubit id (target) to be applied
+     * @param [in] con qubit id (control) to be applied
+     * @param [in] tar qubit id (target) to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& cx(const uint32_t c, const uint32_t t) { return add_qgate(QGateKind::CX, {c, t}); }
+    QCirc& cx(const uint32_t con, const uint32_t tar, const std::vector<uint32_t>& pol = std::vector<uint32_t>(1, 0))
+    {
+      return add_qgate(QGateKind::CX, {con, tar}, Sharqit::Phase(0), pol);
+    }
     /**
      * @brief add a CZ gate to the quantum circuit
-     * @param [in] c qubit id (control) to be applied
-     * @param [in] t qubit id (target) to be applied
+     * @param [in] con qubit id (control) to be applied
+     * @param [in] tar qubit id (target) to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& cz(const uint32_t c, const uint32_t t) { return add_qgate(QGateKind::CZ, {c, t}); }
+    QCirc& cz(const uint32_t con, const uint32_t tar, const std::vector<uint32_t>& pol = std::vector<uint32_t>(1, 0))
+    {
+      return add_qgate(QGateKind::CZ, {con, tar}, Sharqit::Phase(0), pol);
+    }
     /**
      * @brief add a RX gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @param [in] phase phase of the rotation
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& rx(const uint32_t q, const Phase& phase) { h(q); rz(q,phase); h(q); return *this; }
     /**
      * @brief add a CCX gate to the quantum circuit
-     * @param [in] c0 qubit id (control) to be applied
-     * @param [in] c1 qubit id (control) to be applied
+     * @param [in] con0 qubit id (control) to be applied
+     * @param [in] con1 qubit id (control) to be applied
      * @param [in] tar qubit id (target) to be applied
+     * @param [in] pol polarities of control qubits
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& ccx(const uint32_t c0, const uint32_t c1, const uint32_t tar) { return add_qgate(QGateKind::CCX, {c0, c1, tar}); }
+    QCirc& ccx(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+	       const std::vector<uint32_t>& pol = std::vector<uint32_t>(2, 0))
+    {
+      return add_qgate(QGateKind::CCX, {con0, con1, tar}, Sharqit::Phase(0), pol);
+    }
     /**
      * @brief add a CCZ gate to the quantum circuit
-     * @param [in] c0 qubit id (control) to be applied
-     * @param [in] c1 qubit id (control) to be applied
+     * @param [in] con0 qubit id (control) to be applied
+     * @param [in] con1 qubit id (control) to be applied
      * @param [in] tar qubit id (target) to be applied
+     * @param [in] pol polarities of control qubits
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& ccz(const uint32_t c0, const uint32_t c1, const uint32_t tar) { return add_qgate(QGateKind::CCZ, {c0, c1, tar}); }
+    QCirc& ccz(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+	       const std::vector<uint32_t>& pol = std::vector<uint32_t>(2, 0))
+    { return add_qgate(QGateKind::CCZ, {con0, con1, tar}, Sharqit::Phase(0), pol); }
     /**
      * @brief add a pauli-Y gate to the quantum circuit
      * @param [in] q qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& y(const uint32_t q) { x(q); z(q); return *this; }
     /**
@@ -616,41 +632,67 @@
      * @param [in] q0 qubit id to be applied
      * @param [in] q1 qubit id to be applied
      * @return reference of the QCirc after adding the quantum gate
      */
     QCirc& csw(const uint32_t con, const uint32_t q0, const uint32_t q1) // Fredkin gate
     { cx(q1,q0); ccx(con,q0,q1); cx(q1,q0); return *this; }
     /**
-     * @brief add a controlled cnot (toffoli) gate to the quantum circuit
-     * @param [in] c0 qubit id (control) to be applied
-     * @param [in] c1 qubit id (control) to be applied
+     * @brief decompose a cnot gate to the basic quantum gates
+     * @param [in] con qubit id (control) to be applied
      * @param [in] tar qubit id to be applied
+     * @param [in] pol polarity of control qubits
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& ccx_decomp(const uint32_t c0, const uint32_t c1, const uint32_t tar)
+    QCirc& cx_decomp(const uint32_t con, const uint32_t tar,
+		     const std::vector<uint32_t>& pol = std::vector<uint32_t>(1, 0))
     {
-      h(tar);
-      cx(c1,tar); tdg(tar); cx(c0,tar); t(tar); cx(c1,tar); tdg(tar);
-      cx(c0,tar); cx(c0,c1); tdg(c1); cx(c0,c1); t(c0); t(c1); t(tar);
-      h(tar);
+      if (pol[0] == 1) x(con);
+      cx(con,tar);
+      if (pol[0] == 1) x(con);
       return *this;
     }
     /**
-     * @brief add a controlled CZ gate to the quantum circuit
-     * @param [in] c0 qubit id (control) to be applied
-     * @param [in] c1 qubit id (control) to be applied
+     * @brief decompose a CZ gate to the basic quantum gates
+     * @param [in] con qubit id (control) to be applied
      * @param [in] tar qubit id to be applied
+     * @param [in] pol polarity of control qubits
      * @return reference of the QCirc after adding the quantum gate
      */
-    QCirc& ccz_decomp(const uint32_t c0, const uint32_t c1, const uint32_t tar)
+    QCirc& cz_decomp(const uint32_t con, const uint32_t tar,
+		     const std::vector<uint32_t>& pol = std::vector<uint32_t>(1, 0))
     {
-      cx(c1,tar); tdg(tar); cx(c0,tar); t(tar); cx(c1,tar); tdg(tar);
-      cx(c0,tar); cx(c0,c1); tdg(c1); cx(c0,c1); t(c0); t(c1); t(tar);
+      if (pol[0] == 1) x(con);
+      cz(con,tar);
+      if (pol[0] == 1) x(con);
       return *this;
     }
+    /**
+     * @brief decompose a controlled cnot (toffoli) gate to basic quantum gates
+     * @param [in] con0 qubit id (control) to be applied
+     * @param [in] con1 qubit id (control) to be applied
+     * @param [in] tar qubit id to be applied
+     * @param [in] pol polarities of control qubits
+     * @param [in] method optimization method ("zx" or "pp")
+     * @return reference of the QCirc after adding the quantum gate
+     */
+    QCirc& ccx_decomp(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+		      const std::vector<uint32_t>& pol = std::vector<uint32_t>(2, 0),
+		      const std::string& method = "zx");
+    /**
+     * @brief decompose a controlled CZ gate to basic quantum gates
+     * @param [in] con0 qubit id (control) to be applied
+     * @param [in] con1 qubit id (control) to be applied
+     * @param [in] tar qubit id to be applied
+     * @param [in] pol polarities of control qubits
+     * @param [in] method optimization method ("zx" or "pp")
+     * @return reference of the QCirc after adding the quantum gate
+     */
+    QCirc& ccz_decomp(const uint32_t con0, const uint32_t con1, const uint32_t tar,
+		      const std::vector<uint32_t>& pol = std::vector<uint32_t>(2, 0),
+		      const std::string& method = "zx");
     QCirc& operator+=(const QCirc& rhs) { return add_qcirc(rhs); }
     friend QCirc operator+(const QCirc& lhs, const QCirc& rhs) { QCirc qc = lhs; return qc.add_qcirc(rhs); }
     friend std::ostream& operator<<(std::ostream& ost, const QCirc& qc) { ost << qc.to_string(); return ost; }
   };
 }
 
 #endif
```

### Comparing `sharqit-0.2.2/sharqit/cpp/qgate.cpp` & `sharqit-0.2.3/sharqit/cpp/qgate.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * @file qgate.cpp
  * @brief member functions of QGate class
  */
 
 #include "qgate.h"
 
 Sharqit::QGate::QGate(const Sharqit::QGateKind kind, const std::vector<uint32_t>& qid,
-		      const Sharqit::Phase& phase)
+		      const Sharqit::Phase& phase, const std::vector<uint32_t>& pol)
 {
   Sharqit::Phase p = phase;
   p.mod_2pi();
   
   switch (kind) {
   case Sharqit::QGateKind::Id:
   case Sharqit::QGateKind::X:
@@ -23,63 +23,98 @@
     if (qid.size() != 1) {
       throw std::runtime_error("related qubit number must be 1.");
     }
     if (p.is_zero() == false) {
       throw std::runtime_error("phase parameter must be zero.");
     }
     break;
+    pol_ = {};
   case Sharqit::QGateKind::RZ:
     if (qid.size() != 1) {
       throw std::runtime_error("related qubit number must be 1.");
     }
+    pol_ = {};
     break;
   case Sharqit::QGateKind::Id2:
+    if (qid.size() != 2) {
+      throw std::runtime_error("related qubit number must be 2.");
+    }
+    if (p.is_zero() == false) {
+      throw std::runtime_error("phase parameter must be zero.");
+    }
+    pol_ = {};
+    break;
   case Sharqit::QGateKind::CX:
   case Sharqit::QGateKind::CZ:
     if (qid.size() != 2) {
       throw std::runtime_error("related qubit number must be 2.");
     }
     if (p.is_zero() == false) {
       throw std::runtime_error("phase parameter must be zero.");
     }
+    if (pol.size() == 0) pol_ = {0};
+    else if (pol.size() != 1) throw std::runtime_error("size of the control pattern must be 1.");
+    else pol_ = pol;
     break;
   case Sharqit::QGateKind::CCX:
   case Sharqit::QGateKind::CCZ:
     if (qid.size() != 3) {
       throw std::runtime_error("related qubit number must be 3.");
     }
     if (p.is_zero() == false) {
       throw std::runtime_error("phase parameter must be zero.");
     }
+    if (pol.size() == 0) pol_ = {0, 0};
+    else if (pol.size() != 2) throw std::runtime_error("size of the control pattern must be 2.");
+    else pol_ = pol;
     break;
   default:
     throw std::runtime_error("unknown QGateKind.");
   }
 
   kind_ = kind;
   qid_ = qid;
   phase_ = p;
   op_ = kind_to_op(kind_, phase_);
 }
 
 Sharqit::QGate::QGate(const std::string& qgate_str)
 {
+  /* kind and phase */
   uint32_t pos = qgate_str.find(" ");
   std::string kind_phase_str = qgate_str.substr(0, pos);
   std::tuple<QGateKind, Phase> kp = kind_phase(kind_phase_str);
   kind_ = std::get<0>(kp);
   phase_ = std::get<1>(kp);
 
+  /* qid */
   pos = qgate_str.find(" ");
   std::string s = qgate_str.substr(pos, qgate_str.size()-pos);
   std::string qid_str = Sharqit::trim(s);
+  std::vector<uint32_t> positives; /* flags that each control qubit is posi or nega */
   for (auto& qstr:Sharqit::split(qid_str, ' ')) {
-    qid_.push_back(stoi(qstr));
+    std::string q;
+    if (qstr[0] == '-') {
+      q = Sharqit::trim(qstr, "-");
+      positives.push_back(1);
+    }
+    else {
+      q = qstr;
+      positives.push_back(0);
+    }
+    qid_.push_back(stoi(q));
   }
-  
+  if (positives[positives.size() - 1] == 1) { /* target qubit must have positive flag */
+    throw std::runtime_error("Target qubit must have positive flag");
+  }
+  /* pol */
+  positives.pop_back(); /* remove an element for target qubit */
+  pol_ = positives;
+
+  /* op */
   op_ = kind_to_op(kind_, phase_);
 }
 
 std::vector<std::vector<std::complex<double>>> Sharqit::QGate::kind_to_op(const Sharqit::QGateKind kind,
 									const Sharqit::Phase& phase)
 {
   std::vector<std::vector<std::complex<double>>> op;
@@ -174,23 +209,20 @@
   return s[kind_] + p_str;
 }
 
 std::string Sharqit::QGate::to_string(bool pi_str) const
 {
   std::stringstream ss;
   ss << name(pi_str) << " ";
-  if (qid()[0] != qid()[1]) {
-    for (auto& q:qid()) {
-      ss << q << " ";
+  if (qid().size() > 0) {
+    for (uint32_t i = 0; i < qid().size(); ++i) {
+      if (i < qid().size() - 1 && pol()[i] == 1) ss << "-";
+      ss << std::to_string(qid()[i]) << " ";
     }
   }
-  else {
-    ss << qid()[0] << " ";
-  }
-
   std::string s = ss.str();
   s.pop_back();
 
   return s;
 }
 
 std::tuple<Sharqit::QGateKind, Sharqit::Phase> Sharqit::QGate::kind_phase(const std::string& str)
@@ -344,14 +376,15 @@
     qgate_inv.kind(Sharqit::QGateKind::CCZ);
     qgate_inv.qid(qid_);
     qgate_inv.op(kind_to_op(Sharqit::QGateKind::CCZ));
     break;
   default:
     throw std::runtime_error("unknown QGateKind.");
   }
+  qgate_inv.pol(pol_);
   return qgate_inv;
 }
 
 bool Sharqit::QGate::is_identical(QGate& other) const
 {
   if (kind_ != other.kind()) return false;
   if (qid_.size() != other.qid().size()) return false;
@@ -461,16 +494,20 @@
     else if (other.kind() == Sharqit::QGateKind::S) p += Sharqit::Phase(1,2);
     else if (other.kind() == Sharqit::QGateKind::Sdg) p += Sharqit::Phase(-1,2);
     else if (other.kind() == Sharqit::QGateKind::T) p += Sharqit::Phase(1,4);
     else if (other.kind() == Sharqit::QGateKind::Tdg) p += Sharqit::Phase(-1,4);
     else if (other.kind() == Sharqit::QGateKind::RZ) p += other.phase();
     else if (other.kind() == Sharqit::QGateKind::Id) p += Sharqit::Phase(0);
 
+    p.mod_2pi();
     if (p == Phase(0)) {
       kind(Sharqit::QGateKind::Id);
+      phase(p);
+      op(kind_to_op(kind_, phase_));
     }
     else {
       kind(Sharqit::QGateKind::RZ);
       phase(p);
+      op(kind_to_op(kind_, phase_));
     }
   }
 }
```

### Comparing `sharqit-0.2.2/sharqit/cpp/qgate.h` & `sharqit-0.2.3/sharqit/cpp/qgate.h`

 * *Files 2% similar despite different names*

```diff
@@ -39,57 +39,65 @@
   */
   class QGate
   {
   private:
     QGateKind kind_; //!< kind of quantum gate
     std::vector<uint32_t> qid_; //!< vector of qubit indexes
     Phase phase_; //!< phase of rotation gate
+    std::vector<uint32_t> pol_; //!< polarities of control qubits
     std::vector<std::vector<std::complex<double>>> op_; //!< complex matrix for the quantum gate operation
     /**
      * @brief get an operation matrix from kind of the quantum gate
      * @param [in] kind kind of the quantum gate
      * @param [in] phase phase of the rotation
      * @return operation matrix of the quantum gate
      */
     static std::vector<std::vector<std::complex<double>>> kind_to_op(const QGateKind kind, const Phase& phase = 0);
   public:
     /**
      * @brief constructor of the QGate
      * @param [in] kind kind of the quantum gate
      * @param [in] qid vector of qubit indexes of the quantum gate
      * @param [in] phase phase of the rotation gate
+     * @param [in] pol polarities of controll qubits
      */
-    QGate(const QGateKind kind = QGateKind::Id, const std::vector<uint32_t>& qid = {0}, const Phase& phase = 0);
+    QGate(const QGateKind kind = QGateKind::Id, const std::vector<uint32_t>& qid = {0},
+	  const Phase& phase = 0, const std::vector<uint32_t>& pol = {});
     /**
      * @brief constructor of the QGate
      * @param [in] qgate_str string representation of the quantum gate
      * @note [examples] @n qgate_str = "x 1", "CX 0 1", "RZ(1/4) 2" ...
      */
     QGate(const std::string& qgate_str);
     /**
      * @brief copy constructor of the QGate
      * @param [in] qgate QGate object
      */
-    QGate(const QGate& qgate) : kind_(qgate.kind_), qid_(qgate.qid_), phase_(qgate.phase_), op_(qgate.op_) {}
+    QGate(const QGate& qgate) : kind_(qgate.kind_), qid_(qgate.qid_), phase_(qgate.phase_),
+				pol_(qgate.pol_), op_(qgate.op_) {}
     //! getter of the kind_
     QGateKind kind() const { return kind_; }
     //! getter of the qid_
     std::vector<uint32_t> qid() const { return qid_; }
     //! getter of the phase_
     Phase phase() const { return phase_; }
     //! getter of the phase_
     Phase get_phase() const { return phase_; }
+    //! getter of the pol_
+    std::vector<uint32_t> pol() const { return pol_; }
     //! getter of the op_
     std::vector<std::vector<std::complex<double>>> op() const { return op_; }
     //! setter of the kind_
     void kind(const QGateKind kind) { kind_ = kind; }
     //! setter of the qid_
     void qid(const std::vector<uint32_t>& qid) { qid_ = qid; }
     //! setter of the phase_
     void phase(const Phase& phase) { phase_ = phase; }
+    //! setter of the pol_
+    void pol(const std::vector<uint32_t>& pol) { pol_ = pol; }
     //! setter of the op_
     void op(const std::vector<std::vector<std::complex<double>>>& op) { op_ = op; }
     /**
      * @brief get a name of the quantum gates
      * @param [in] pi_str whether to include a pi string
      * @return name of the quantum gates
      */
```

### Comparing `sharqit-0.2.2/sharqit/cpp/sharqit.cpp` & `sharqit-0.2.3/sharqit/cpp/sharqit.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/simplify.cpp` & `sharqit-0.2.3/sharqit/cpp/simplify.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/util.h` & `sharqit-0.2.3/sharqit/cpp/util.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/zx.h` & `sharqit-0.2.3/sharqit/cpp/zx.h`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/zxdiagram.cpp` & `sharqit-0.2.3/sharqit/cpp/zxdiagram.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit/cpp/zxnode.cpp` & `sharqit-0.2.3/sharqit/cpp/zxnode.cpp`

 * *Files identical despite different names*

### Comparing `sharqit-0.2.2/sharqit.egg-info/SOURCES.txt` & `sharqit-0.2.3/sharqit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

